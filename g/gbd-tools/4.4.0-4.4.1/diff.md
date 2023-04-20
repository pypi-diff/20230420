# Comparing `tmp/gbd_tools-4.4.0.tar.gz` & `tmp/gbd_tools-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.4.0.tar", last modified: Sun Apr 16 15:26:24 2023, max compression
+gzip compressed data, was "gbd_tools-4.4.1.tar", last modified: Thu Apr 20 08:29:41 2023, max compression
```

## Comparing `gbd_tools-4.4.0.tar` & `gbd_tools-4.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:26:24.082157 gbd_tools-4.4.0/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.4.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3757 2023-04-16 15:26:24.082157 gbd_tools-4.4.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.4.0/README.md
--rwxrwxr-x   0 root         (0) root         (0)    10950 2023-02-07 16:30:01.000000 gbd_tools-4.4.0/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:26:24.078157 gbd_tools-4.4.0/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.4.0/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8294 2023-02-07 16:30:01.000000 gbd_tools-4.4.0/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     1151 2023-01-02 08:37:48.000000 gbd_tools-4.4.0/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    10046 2023-02-15 10:46:17.000000 gbd_tools-4.4.0/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     5050 2023-02-07 16:30:01.000000 gbd_tools-4.4.0/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5479 2023-01-09 18:14:00.000000 gbd_tools-4.4.0/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12347 2023-02-15 10:51:41.000000 gbd_tools-4.4.0/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4628 2023-01-02 08:38:26.000000 gbd_tools-4.4.0/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3355 2023-01-05 08:44:08.000000 gbd_tools-4.4.0/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:26:24.078157 gbd_tools-4.4.0/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.4.0/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7676 2023-01-05 09:18:19.000000 gbd_tools-4.4.0/gbd_init/cnf_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     3853 2023-01-05 10:39:03.000000 gbd_tools-4.4.0/gbd_init/cnf_transformers.py
--rw-rw-r--   0 root         (0) root         (0)     2033 2023-01-02 08:38:45.000000 gbd_tools-4.4.0/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3458 2023-01-05 09:55:11.000000 gbd_tools-4.4.0/gbd_init/initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:26:24.078157 gbd_tools-4.4.0/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.4.0/gbd_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:26:24.078157 gbd_tools-4.4.0/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:26:24.082157 gbd_tools-4.4.0/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.4.0/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.4.0/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.4.0/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.4.0/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.4.0/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:26:24.082157 gbd_tools-4.4.0/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.4.0/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:26:24.082157 gbd_tools-4.4.0/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3757 2023-04-16 15:26:23.000000 gbd_tools-4.4.0/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2023-04-16 15:26:23.000000 gbd_tools-4.4.0/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 15:26:23.000000 gbd_tools-4.4.0/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-16 15:26:23.000000 gbd_tools-4.4.0/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-16 15:26:23.000000 gbd_tools-4.4.0/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-16 15:26:23.000000 gbd_tools-4.4.0/gbd_tools.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)    12040 2023-02-10 15:21:05.000000 gbd_tools-4.4.0/server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 15:26:24.082157 gbd_tools-4.4.0/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1034 2023-04-16 15:25:57.000000 gbd_tools-4.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:29:41.159203 gbd_tools-4.4.1/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.4.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-04-20 08:29:41.159203 gbd_tools-4.4.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.4.1/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    10950 2023-04-20 08:28:49.000000 gbd_tools-4.4.1/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:29:41.151203 gbd_tools-4.4.1/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.4.1/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8294 2023-02-07 16:30:01.000000 gbd_tools-4.4.1/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.4.1/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    10046 2023-02-15 10:46:17.000000 gbd_tools-4.4.1/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     5050 2023-02-07 16:30:01.000000 gbd_tools-4.4.1/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5479 2023-01-09 18:14:00.000000 gbd_tools-4.4.1/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12347 2023-04-20 08:28:49.000000 gbd_tools-4.4.1/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.4.1/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3355 2023-01-05 08:44:08.000000 gbd_tools-4.4.1/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:29:41.151203 gbd_tools-4.4.1/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.4.1/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7647 2023-04-20 08:28:49.000000 gbd_tools-4.4.1/gbd_init/cnf_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.4.1/gbd_init/cnf_transformers.py
+-rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.4.1/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.4.1/gbd_init/initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:29:41.151203 gbd_tools-4.4.1/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.4.1/gbd_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:29:41.151203 gbd_tools-4.4.1/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:29:41.155203 gbd_tools-4.4.1/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.4.1/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.4.1/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.4.1/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.4.1/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.4.1/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:29:41.155203 gbd_tools-4.4.1/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.4.1/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:29:41.159203 gbd_tools-4.4.1/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-04-20 08:29:40.000000 gbd_tools-4.4.1/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      772 2023-04-20 08:29:40.000000 gbd_tools-4.4.1/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 08:29:40.000000 gbd_tools-4.4.1/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-20 08:29:40.000000 gbd_tools-4.4.1/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-20 08:29:40.000000 gbd_tools-4.4.1/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-20 08:29:40.000000 gbd_tools-4.4.1/gbd_tools.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    12040 2023-02-10 15:21:05.000000 gbd_tools-4.4.1/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 08:29:41.159203 gbd_tools-4.4.1/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1034 2023-04-20 08:28:49.000000 gbd_tools-4.4.1/setup.py
```

### Comparing `gbd_tools-4.4.0/LICENSE` & `gbd_tools-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/PKG-INFO` & `gbd_tools-4.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_tools
-Version: 4.4.0
+Version: 4.4.1
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.4.0/README.md` & `gbd_tools-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd.py` & `gbd_tools-4.4.1/gbd.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from gbd_core.grammar import ParserException
 from gbd_core import util, contexts, schema
 from gbd_core.util_argparse import *
 
 
 ### Command-Line Interface Entry Points
 def cli_hash(api: GBD, args):
-    from gbd_init.gbdhash import gbd_hash
-    print(gbd_hash(args.path))
+    from gbd_init.gbdhash import identify
+    print(identify(args.path))
 
 
 def cli_init_local(api: GBD, args):
     from gbd_init.cnf_extractors import init_local
     rlimits = { 'jobs': args.jobs, 'tlim': args.tlim, 'mlim': args.mlim, 'flim': args.flim }
     init_local(api, args.context, rlimits, args.path, target_db=args.target_db)
```

### Comparing `gbd_tools-4.4.0/gbd_core/api.py` & `gbd_tools-4.4.1/gbd_core/api.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd_core/contexts.py` & `gbd_tools-4.4.1/gbd_core/contexts.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,23 +16,43 @@
 
 packed = [ "", ".gz", ".lzma", ".xz", ".bz2" ]
 
 context_data = {
     "cnf" : {
         "id" : 100,
         "suffixes" : [ ".cnf" + p for p in packed ],
+        "description" : "Conjunctive Normal Form (CNF) in DIMACS format",
     },
     "sancnf" : {
         "id" : 101,
         "suffixes" : [ ".sanitized.cnf" + p for p in packed ],
+        "description" : "Sanitized Conjunctive Normal Form (CNF) in DIMACS format",
     },
     "kis" : {
         "id" : 200,
         "suffixes" : [ ".kis" + p for p in packed ],
-    }
+        "description" : "k-Independent Set (KIS) in DIMACS-like graph format",
+    },
+    "opb" : {
+        "id" : 300,
+        "suffixes" : [ ".opb" + p for p in packed ],
+        "description" : "Pseudo-Boolean Optimization Problem in OPB format",
+    },
+    "wecnf" : {
+        "id" : 400,
+        "suffixes" : [ ".wecnf" + p for p in packed ],
+        "description" : "Weighted Extended Conjunctive Normal Form (WECNF)",
+    },
 }
 
 def suffix_list(context):
     return context_data[context]['suffixes']
 
 def contexts():
     return context_data.keys()
+
+def get_context_by_suffix(filename):
+    for context in contexts():
+        for suffix in suffix_list(context):
+            if filename.endswith(suffix):
+                return context
+    return None
```

### Comparing `gbd_tools-4.4.0/gbd_core/database.py` & `gbd_tools-4.4.1/gbd_core/database.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd_core/grammar.py` & `gbd_tools-4.4.1/gbd_core/grammar.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd_core/query.py` & `gbd_tools-4.4.1/gbd_core/query.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd_core/schema.py` & `gbd_tools-4.4.1/gbd_core/schema.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd_core/util.py` & `gbd_tools-4.4.1/gbd_core/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 
 # The above copyright notice and this permission notice shall be included in all
 # copies or substantial portions of the Software.
 
 import sys
-import bz2
-import gzip
-import lzma
 import os
 
 
 # Thanks to Boris V. for this code https://stackoverflow.com/questions/4675728/redirect-stdout-to-a-file-in-python
 from contextlib import contextmanager
 
 def fileno(file_or_fd):
@@ -75,30 +72,14 @@
             float(s)
             return True
     except ValueError:
         return False
     return False
 
 
-def open_cnf_file(filename, mode):
-    """
-    Opens a CNF file (this is badly guarded, by file-extension only)
-    """
-    if filename.endswith('.cnf.gz'):
-        return gzip.open(filename, mode)
-    elif filename.endswith('.cnf.bz2'):
-        return bz2.open(filename, mode)
-    elif filename.endswith('.cnf.lzma') or filename.endswith('.cnf.xz'):
-        return lzma.open(filename, mode)
-    elif filename.endswith('.cnf'):
-        return open(filename, mode)
-    else:
-        raise Exception("Unknown File Extension. Use .cnf, .cnf.bz2, .cnf.lzma, .cnf.xz, or .cnf.gz")
-
-
 def eprint(*args, **kwargs):
     print(*args, file=sys.stderr, **kwargs)
 
 
 def read_hashes():
     eprint("Reading hashes from stdin ...")
     hashes = list()
```

### Comparing `gbd_tools-4.4.0/gbd_core/util_argparse.py` & `gbd_tools-4.4.1/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd_init/cnf_extractors.py` & `gbd_tools-4.4.1/gbd_init/cnf_extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,29 +17,28 @@
 import os
 import glob
 
 from gbd_core.contexts import suffix_list
 from gbd_core.api import GBD, GBDException
 from gbd_core.util import eprint, confirm
 from gbd_init.initializer import Initializer
-from gbd_init.gbdhash import gbd_hash
+from gbd_init.gbdhash import identify
 
 from gbdc import extract_base_features, extract_gate_features, isohash
 
 
 ## GBDHash
 def compute_hash(hash, path, limits):
     eprint('Hashing {}'.format(path))
-    hash = gbd_hash(path)
+    hash = identify(path)
     return [ ("local", hash, path), ("filename", hash, os.path.basename(path)) ]
 
 def init_local(api: GBD, context, rlimits, root, target_db):
-    contexts = [ 'cnf', 'sancnf' ]
     features = [ ("local", None), ("filename", None) ]
-    extractor = Initializer(contexts, contexts, api, context, rlimits, target_db, features, compute_hash)
+    extractor = Initializer([ context ], [ context ], api, context, rlimits, target_db, features, compute_hash)
     extractor.create_features()
 
     df = api.query(group_by="local")
     
     dfilter = df["local"].apply(lambda x: not x or not os.path.isfile(x))
     missing = df[dfilter]
     if len(missing) and confirm("{} files not found. Remove stale entries from local table?".format(len(missing))):
```

### Comparing `gbd_tools-4.4.0/gbd_init/cnf_transformers.py` & `gbd_tools-4.4.1/gbd_init/cnf_transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import os
 from functools import reduce
 
 from gbd_core import contexts
 from gbd_core.api import GBD, GBDException
 from gbd_core import util
 
-from gbd_init.gbdhash import gbd_hash
+from gbd_init.gbdhash import identify
 from gbd_init.initializer import Initializer
 
 import gbdc
 
 
 # Transform SAT Problem to k-Independent Set Problem
 def kis_filename(path):
@@ -71,15 +71,15 @@
 def sanitize_cnf(hash, path, limits):
     util.eprint('Sanitizing {}'.format(path))
 
     sanname = sanitized_filename(path)
     try:
         with open(sanname, 'w') as f, util.stdout_redirected(f):
             if gbdc.sanitize(path): 
-                sanhash = gbd_hash(sanname)
+                sanhash = identify(sanname)
                 return [ ('local', sanhash, sanname), ('to_cnf', sanhash, hash) ]
             else:
                 raise GBDException("Sanitization failed for {}".format(path))
     except Exception as e:
         util.eprint(str(e))
         os.remove(sanname)
```

### Comparing `gbd_tools-4.4.0/gbd_init/gbdhash.py` & `gbd_tools-4.4.1/gbd_init/gbdhash.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,28 +9,43 @@
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 
 # The above copyright notice and this permission notice shall be included in all
 # copies or substantial portions of the Software.
 
-
 import io
 import hashlib
 
-from gbd_core.util import open_cnf_file
+import gzip
+import bz2
+import lzma
+
+from gbd_core.contexts import get_context_by_suffix
+
+
+def open_file(filename, mode):
+    if filename.endswith('.gz'):
+        return gzip.open(filename, mode)
+    elif filename.endswith('.bz2'):
+        return bz2.open(filename, mode)
+    elif filename.endswith('.lzma') or filename.endswith('.xz'):
+        return lzma.open(filename, mode)
+    else:
+        return open(filename, mode)
+
 
 try:
-    from gbdc import gbdhash as gbd_hash
+    from gbdc import gbdhash as cnf_hash
 except ImportError:
     try:
-        from gbdhashc import gbdhash as gbd_hash
+        from gbdhashc import gbdhash as cnf_hash
     except ImportError:
-        def gbd_hash(filename):
-            file = open_cnf_file(filename, 'rb')
+        def cnf_hash(filename):
+            file = open_file(filename, 'rb')
             buff = io.BufferedReader(file, io.DEFAULT_BUFFER_SIZE * 16)
 
             space = False
             skip = False
             start = True
             cldelim = True
             hash_md5 = hashlib.md5()
@@ -50,8 +65,26 @@
                     skip = True  # do not hash comment and header line
 
             if not cldelim:
                 hash_md5.update(b' 0')
 
             file.close()
 
-            return hash_md5.hexdigest()
+            return hash_md5.hexdigest()
+
+
+try:
+    from gbdc import opbhash as opb_hash
+except ImportError:
+    raise Exception("Unable to import opbhash. Please install or update gbdc.")
+    
+
+def identify(path, ct=None):
+    context = ct or get_context_by_suffix(path)
+    if context is None:
+        raise Exception("Unable to associate context: " + path)
+    elif context in ['cnf', 'sancnf', 'kis', 'wecnf']:
+        return cnf_hash(path)
+    elif context in ['opb']:
+        return opb_hash(path)
+    else:
+        raise Exception("Unable to identify: " + path)
```

### Comparing `gbd_tools-4.4.0/gbd_init/initializer.py` & `gbd_tools-4.4.1/gbd_init/initializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.target_db = target_db
         self.features = features
         self.initfunc = initfunc
         self.rlimits = rlimits
         if not context in source_contexts:
             raise GBDException("Context '{}' not supported by '{}'".format(context, self.__class__.__name__))
         if not api.database.dcontext(target_db) in target_contexts:
-            raise GBDException("Target database '{}' has incompatible context '{}'".format(target_db, api.database.dcontext(target_db)))
+            raise GBDException("Target database '{}' has incompatible context '{}'. Database context can be specified by filename prefix.".format(target_db, api.database.dcontext(target_db)))
 
 
     def create_features(self):
         for (name, default) in self.features:
             self.api.database.create_feature(name, default, self.target_db, True)
         self.api.database.commit()
```

### Comparing `gbd_tools-4.4.0/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.4.1/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.4.1/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.4.1/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd_server/static/main.css` & `gbd_tools-4.4.1/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd_server/static/w3.js` & `gbd_tools-4.4.1/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd_server/templates/index.html` & `gbd_tools-4.4.1/gbd_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.4.1/gbd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-tools
-Version: 4.4.0
+Version: 4.4.1
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.4.0/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.4.1/gbd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/server.py` & `gbd_tools-4.4.1/server.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.0/setup.py` & `gbd_tools-4.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.4.0',
+  version='4.4.1',
   description='GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser, Karlsruhe Institute of Technology (KIT)',
   author_email='markus.iser@kit.edu',
   packages=[
```

