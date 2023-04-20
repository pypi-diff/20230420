# Comparing `tmp/pyempaq-0.3.0.tar.gz` & `tmp/pyempaq-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyempaq-0.3.0.tar", last modified: Wed Apr 19 21:48:06 2023, max compression
+gzip compressed data, was "pyempaq-0.3.1.tar", last modified: Thu Apr 20 14:27:20 2023, max compression
```

## Comparing `pyempaq-0.3.0.tar` & `pyempaq-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2023-04-19 21:48:06.680242 pyempaq-0.3.0/
--rw-rw-r--   0 facundo   (1000) facundo   (1000)    35149 2021-07-15 22:17:23.000000 pyempaq-0.3.0/LICENSE
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       59 2021-09-26 15:51:02.000000 pyempaq-0.3.0/MANIFEST.in
--rw-rw-r--   0 facundo   (1000) facundo   (1000)    12899 2023-04-19 21:48:06.680242 pyempaq-0.3.0/PKG-INFO
--rw-rw-r--   0 facundo   (1000) facundo   (1000)    12207 2023-04-19 21:19:57.000000 pyempaq-0.3.0/README.md
-drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2023-04-19 21:48:06.680242 pyempaq-0.3.0/pyempaq/
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      267 2023-02-19 18:32:46.000000 pyempaq-0.3.0/pyempaq/__init__.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      258 2021-07-17 21:32:58.000000 pyempaq-0.3.0/pyempaq/__main__.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      488 2023-04-19 21:39:32.000000 pyempaq-0.3.0/pyempaq/_version.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     1485 2022-06-19 15:17:40.000000 pyempaq-0.3.0/pyempaq/common.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     6381 2023-04-17 17:23:34.000000 pyempaq-0.3.0/pyempaq/config_manager.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     9659 2023-04-17 17:23:34.000000 pyempaq-0.3.0/pyempaq/main.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     6526 2023-04-19 21:19:57.000000 pyempaq-0.3.0/pyempaq/unpacker.py
-drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2023-04-19 21:48:06.680242 pyempaq-0.3.0/pyempaq.egg-info/
--rw-rw-r--   0 facundo   (1000) facundo   (1000)    12899 2023-04-19 21:48:06.000000 pyempaq-0.3.0/pyempaq.egg-info/PKG-INFO
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      383 2023-04-19 21:48:06.000000 pyempaq-0.3.0/pyempaq.egg-info/SOURCES.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)        1 2023-04-19 21:48:06.000000 pyempaq-0.3.0/pyempaq.egg-info/dependency_links.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       47 2023-04-19 21:48:06.000000 pyempaq-0.3.0/pyempaq.egg-info/entry_points.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       28 2023-04-19 21:48:06.000000 pyempaq-0.3.0/pyempaq.egg-info/requires.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)        8 2023-04-19 21:48:06.000000 pyempaq-0.3.0/pyempaq.egg-info/top_level.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       28 2022-04-15 13:03:12.000000 pyempaq-0.3.0/requirements.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       38 2023-04-19 21:48:06.680242 pyempaq-0.3.0/setup.cfg
--rwxrwxr-x   0 facundo   (1000) facundo   (1000)     1776 2023-04-19 21:47:43.000000 pyempaq-0.3.0/setup.py
+drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2023-04-20 14:27:20.355540 pyempaq-0.3.1/
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)    35149 2021-07-15 22:17:23.000000 pyempaq-0.3.1/LICENSE
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       59 2021-09-26 15:51:02.000000 pyempaq-0.3.1/MANIFEST.in
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)    12899 2023-04-20 14:27:20.355540 pyempaq-0.3.1/PKG-INFO
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)    12207 2023-04-19 21:19:57.000000 pyempaq-0.3.1/README.md
+drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2023-04-20 14:27:20.355540 pyempaq-0.3.1/pyempaq/
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)      267 2023-02-19 18:32:46.000000 pyempaq-0.3.1/pyempaq/__init__.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)      258 2021-07-17 21:32:58.000000 pyempaq-0.3.1/pyempaq/__main__.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)      488 2023-04-20 14:27:16.000000 pyempaq-0.3.1/pyempaq/_version.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)     1485 2022-06-19 15:17:40.000000 pyempaq-0.3.1/pyempaq/common.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)     6381 2023-04-17 17:23:34.000000 pyempaq-0.3.1/pyempaq/config_manager.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)     9755 2023-04-20 14:26:40.000000 pyempaq-0.3.1/pyempaq/main.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)     6600 2023-04-20 14:26:40.000000 pyempaq-0.3.1/pyempaq/unpacker.py
+drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2023-04-20 14:27:20.355540 pyempaq-0.3.1/pyempaq.egg-info/
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)    12899 2023-04-20 14:27:20.000000 pyempaq-0.3.1/pyempaq.egg-info/PKG-INFO
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)      383 2023-04-20 14:27:20.000000 pyempaq-0.3.1/pyempaq.egg-info/SOURCES.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)        1 2023-04-20 14:27:20.000000 pyempaq-0.3.1/pyempaq.egg-info/dependency_links.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       47 2023-04-20 14:27:20.000000 pyempaq-0.3.1/pyempaq.egg-info/entry_points.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       28 2023-04-20 14:27:20.000000 pyempaq-0.3.1/pyempaq.egg-info/requires.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)        8 2023-04-20 14:27:20.000000 pyempaq-0.3.1/pyempaq.egg-info/top_level.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       28 2022-04-15 13:03:12.000000 pyempaq-0.3.1/requirements.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       38 2023-04-20 14:27:20.355540 pyempaq-0.3.1/setup.cfg
+-rwxrwxr-x   0 facundo   (1000) facundo   (1000)     1776 2023-04-19 21:47:43.000000 pyempaq-0.3.1/setup.py
```

### Comparing `pyempaq-0.3.0/LICENSE` & `pyempaq-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyempaq-0.3.0/PKG-INFO` & `pyempaq-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyempaq
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python packer to run anywhwere any project with any virtualenv dependencies.
 Home-page: https://github.com/facundobatista/pyempaq
 Author: Facundo Batista
 Author-email: facundo@taniquetil.com.ar
 License: GPL-v3
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pyempaq-0.3.0/README.md` & `pyempaq-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyempaq-0.3.0/pyempaq/common.py` & `pyempaq-0.3.1/pyempaq/common.py`

 * *Files identical despite different names*

### Comparing `pyempaq-0.3.0/pyempaq/config_manager.py` & `pyempaq-0.3.1/pyempaq/config_manager.py`

 * *Files identical despite different names*

### Comparing `pyempaq-0.3.0/pyempaq/main.py` & `pyempaq-0.3.1/pyempaq/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 logging.basicConfig(
     format='%(asctime)s.%(msecs)03d %(levelname)-5s %(message)s', datefmt='%H:%M:%S')
 logger = logging.getLogger(__name__)
 
 # collected arguments
 Args = namedtuple("Args", "project_name basedir entrypoint requirement_files")
 
+# dependencies needed for the unpacker to run ok
+UNPACKER_DEPS = ["appdirs", "packaging"]
+
 
 def get_pip():
     """Ensure an usable version of `pip`."""
     useful_pip = Path("pip3")
     # try to see if it's already installed
     try:
         logged_exec([useful_pip, "--version"])
@@ -204,15 +207,15 @@
     unpacker_final_main = tmpdir / "__main__.py"
     shutil.copy(unpacker_src, unpacker_final_main)
 
     # build a dir with the dependencies needed by the unpacker
     logger.debug("Building internal dependencies dir")
     venv_dir = tmpdir / "venv"
     pip = get_pip()
-    cmd = [pip, "install", "appdirs", f"--target={venv_dir}"]
+    cmd = [pip, "install", *UNPACKER_DEPS, f"--target={venv_dir}"]
     logged_exec(cmd)
 
     metadata = prepare_metadata(origdir, config)
     metadata_file = tmpdir / "metadata.json"
     with metadata_file.open("wt", encoding="utf8") as fh:
         json.dump(metadata, fh)
```

### Comparing `pyempaq-0.3.0/pyempaq/unpacker.py` & `pyempaq-0.3.1/pyempaq/unpacker.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 import platform
 import shutil
 import subprocess
 import sys
 import time
 import venv
 import zipfile
+from types import ModuleType
 from typing import List, Dict, Any
 
-from packaging import version
-
 from pyempaq.common import find_venv_bin, logged_exec
 
 
 # this is the directory for the NEW virtualenv created for the project (not the packed
 # one to run unpacker itself)
 PROJECT_VENV_DIR = "project_venv"
 
@@ -131,15 +130,15 @@
         logged_exec(cmd)
         log("Virtualenv setup finished")
     else:
         log("Skipping virtualenv (no requirements)")
     (project_dir / COMPLETE_FLAG_FILE).touch()
 
 
-def restrictions_ok(restrictions: Dict[str, Any]) -> bool:
+def restrictions_ok(version: ModuleType, restrictions: Dict[str, Any]) -> bool:
     """Enforce the unpacking restrictions, if any; return True if all ok to continue."""
     if not restrictions:
         return True
     ignored_restrictions = os.environ.get("PYEMPAQ_IGNORE_RESTRICTIONS", "").split(",")
 
     mpv = restrictions.get("minimum_python_version")
     if mpv is not None:
@@ -161,20 +160,23 @@
     log("Pyempaq start")
 
     # parse pyempaq metadata from the zip file
     pyempaq_filepath = pathlib.Path.cwd() / sys.argv[0]
     zf = zipfile.ZipFile(pyempaq_filepath)
     metadata = json.loads(zf.read("metadata.json").decode("utf8"))
     log("Loaded metadata: %s", metadata)
-    if not restrictions_ok(metadata["unpack_restrictions"]):
-        exit(1)
 
-    # load appdirs from the builtin venv
+    # load appdirs and packaging from the builtin venv (not at top of file because
+    # paths needed to be fixed)
     sys.path.insert(0, f"{pyempaq_filepath}/venv/")
-    import appdirs  # NOQA: this is an import not at top of file because paths needed to be fixed
+    import appdirs  # NOQA
+    from packaging import version  # NOQA
+
+    if not restrictions_ok(version, metadata["unpack_restrictions"]):
+        exit(1)
 
     pyempaq_dir = pathlib.Path(appdirs.user_data_dir()) / 'pyempaq'
     pyempaq_dir.mkdir(parents=True, exist_ok=True)
     log("Temp base dir: %r", str(pyempaq_dir))
 
     # create a temp dir and extract the project there
     timestamp = time.strftime("%Y%m%d%H%M%S", time.gmtime(pyempaq_filepath.stat().st_ctime))
```

### Comparing `pyempaq-0.3.0/pyempaq.egg-info/PKG-INFO` & `pyempaq-0.3.1/pyempaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyempaq
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python packer to run anywhwere any project with any virtualenv dependencies.
 Home-page: https://github.com/facundobatista/pyempaq
 Author: Facundo Batista
 Author-email: facundo@taniquetil.com.ar
 License: GPL-v3
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pyempaq-0.3.0/setup.py` & `pyempaq-0.3.1/setup.py`

 * *Files identical despite different names*

