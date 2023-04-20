# Comparing `tmp/np_tools-0.1.3.tar.gz` & `tmp/np_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_tools-0.1.3.tar", last modified: Wed Apr 19 21:45:17 2023, max compression
+gzip compressed data, was "np_tools-0.1.4.tar", last modified: Thu Apr 20 00:00:12 2023, max compression
```

## Comparing `np_tools-0.1.3.tar` & `np_tools-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      273 2023-04-13 18:32:03.410128 np_tools-0.1.3/README.md
--rw-r--r--   0        0        0     2417 2023-04-19 21:45:17.183930 np_tools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-19 20:41:36.127176 np_tools-0.1.3/src/np_tools/__init__.py
--rw-r--r--   0        0        0      268 2023-04-13 18:53:25.697520 np_tools-0.1.3/src/np_tools/config.py
--rw-r--r--   0        0        0     8654 2023-04-19 21:43:54.151453 np_tools-0.1.3/src/np_tools/openephys.py
--rw-r--r--   0        0        0     4196 2023-04-19 20:13:12.296840 np_tools-0.1.3/src/np_tools/remote.py
--rw-r--r--   0        0        0     2811 2023-04-19 20:43:03.942122 np_tools-0.1.3/src/np_tools/tools.py
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 np_tools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      273 2023-04-13 18:32:03.410128 np_tools-0.1.4/README.md
+-rw-r--r--   0        0        0     2417 2023-04-20 00:00:12.394667 np_tools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-19 20:41:36.127176 np_tools-0.1.4/src/np_tools/__init__.py
+-rw-r--r--   0        0        0      268 2023-04-13 18:53:25.697520 np_tools-0.1.4/src/np_tools/config.py
+-rw-r--r--   0        0        0     8517 2023-04-19 23:59:55.459560 np_tools-0.1.4/src/np_tools/openephys.py
+-rw-r--r--   0        0        0     4196 2023-04-19 20:13:12.296840 np_tools-0.1.4/src/np_tools/remote.py
+-rw-r--r--   0        0        0     2754 2023-04-19 22:12:49.593247 np_tools-0.1.4/src/np_tools/tools.py
+-rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 np_tools-0.1.4/PKG-INFO
```

### Comparing `np_tools-0.1.3/pyproject.toml` & `np_tools-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 ]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "np_tools"
-version = "0.1.3"
+version = "0.1.4"
 description = "General-purpose tools for common tasks encountered in Mindscope Neuropixels workflows."
 authors = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "fabric>=3.0.0",
     "np-config>=0.4.17",
```

### Comparing `np_tools-0.1.3/src/np_tools/openephys.py` & `np_tools-0.1.4/src/np_tools/openephys.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,22 +44,22 @@
         if not next(path.rglob(glob), None):
             logger.debug(f'Could not find {glob} in {path}')
             return False
     return True
 
 
 def is_valid_ephys_folder(
-    path: pathlib.Path, min_size_gb: int | float = 275
+    path: pathlib.Path, min_size_gb: Optional[int | float] = None,
 ) -> bool:
     """Check a single dir of raw data for size and v0.6.x+ Open Ephys."""
     if not path.is_dir():
         return False
     if not is_new_ephys_folder(path):
         return False
-    if not tools.dir_size(path) > min_size_gb * 1024**3:   # GB
+    if min_size_gb is not None and tools.dir_size(path) < min_size_gb * 1024**3: # GB
         return False
     return True
 
 
 def get_ephys_root(path: pathlib.Path) -> pathlib.Path:
     """Returns the parent of the first `Record Node *` found in the supplied
     path.
@@ -75,49 +75,41 @@
         p.parent
         for p in path.parents
         if 'Record Node'.lower() in p.name.lower()
     )
 
 
 def get_raw_ephys_subfolders(
-    path: pathlib.Path, min_size_gb: int | float = 50
+    path: pathlib.Path, min_size_gb: Optional[int | float] = None
 ) -> tuple[pathlib.Path, ...]:
     """
     Return raw ephys recording folders, defined as the root that Open Ephys
     records to, e.g. `A:/1233245678_366122_20220618_probeABC`.
     """
 
     subfolders = set()
 
     for f in pathlib.Path(path).rglob('*.dat'):
 
-        if not f.is_dir():
-            continue
-
         if any(
             k in f.as_posix().lower()
             for k in [
                 'sorted',
                 'extracted',
                 'curated',
             ]
         ):
             # skip sorted/extracted folders
             continue
 
-        if not is_new_ephys_folder(f):
-            # skip old or incomplete ephys folders
-            continue
-
-        if tools.dir_size(f) < min_size_gb * 1024**3:
-            # skip folders that aren't above min size threshold (GB)
-            continue
-
         subfolders.add(get_ephys_root(f))
 
+    if min_size_gb is not None:
+        subfolders = {_ for _ in subfolders if tools.dir_size(_) < min_size_gb * 1024**3}
+
     return tuple(sorted(list(subfolders), key=lambda s: str(s)))
 
 
 # - If we have probeABC and probeDEF raw data folders, each one has an oebin file:
 #     we'll need to merge the oebin files and the data folders to create a single session
 #     that can be processed in parallel
 def get_single_oebin_path(path: pathlib.Path) -> pathlib.Path:
```

### Comparing `np_tools-0.1.3/src/np_tools/remote.py` & `np_tools-0.1.4/src/np_tools/remote.py`

 * *Files identical despite different names*

### Comparing `np_tools-0.1.3/src/np_tools/tools.py` & `np_tools-0.1.4/src/np_tools/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,26 +50,25 @@
             return
         shutil.copy2(src, dest)
         attempts += 1
     logger.debug(f'Copied {src} to {dest} with checksum-validation')
 
 
 def symlink(src: pathlib.Path, dest: pathlib.Path) -> None:
-    """Create a symlink from at `dest`, pointing to `src`.
+    """Create a symlink at `dest` pointing to `src`.
 
     - creates parent dirs if needed
     - ignores if symlink already exists and points to `src`
     - replaces existing symlink if it points to a different location
 
     """
     if 'win' in sys.platform:
         # Remote to remote symlink creation is disabled by default
         subprocess.run('fsutil behavior set SymlinkEvaluation R2R:1')
-    if not pathlib.Path(dest).parent.exists():
-        pathlib.Path(dest).parent.mkdir(parents=True, exist_ok=True)
+    pathlib.Path(dest).parent.mkdir(parents=True, exist_ok=True)
     if dest.is_symlink() and dest.resolve() == src.resolve():
         logger.debug(f'Symlink already exists to {src} from {dest}')
         return
     dest.unlink(missing_ok=True)
     with contextlib.suppress(FileExistsError):
         dest.symlink_to(src)
     logger.debug(f'Created symlink to {src} from {dest}')
```

### Comparing `np_tools-0.1.3/PKG-INFO` & `np_tools-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: General-purpose tools for common tasks encountered in Mindscope Neuropixels workflows.
 Author-Email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

