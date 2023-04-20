# Comparing `tmp/erddapy-2.0.0.tar.gz` & `tmp/erddapy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erddapy-2.0.0.tar", last modified: Wed Apr 19 11:42:56 2023, max compression
+gzip compressed data, was "erddapy-2.0.1.tar", last modified: Thu Apr 20 17:50:17 2023, max compression
```

## Comparing `erddapy-2.0.0.tar` & `erddapy-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:42:56.054047 erddapy-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-19 11:42:42.000000 erddapy-2.0.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-19 11:42:42.000000 erddapy-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-19 11:42:42.000000 erddapy-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-19 11:42:56.054047 erddapy-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-19 11:42:42.000000 erddapy-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:42:56.050047 erddapy-2.0.0/erddapy/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:42:56.054047 erddapy-2.0.0/erddapy/core/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/core/griddap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/core/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/core/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14312 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/core/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    16215 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/erddapy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/multiple_server_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:42:56.054047 erddapy-2.0.0/erddapy/servers/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/servers/erddaps.json
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/servers/servers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:42:56.054047 erddapy-2.0.0/erddapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-19 11:42:56.000000 erddapy-2.0.0/erddapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-19 11:42:42.000000 erddapy-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-19 11:42:42.000000 erddapy-2.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-19 11:42:42.000000 erddapy-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 11:42:56.054047 erddapy-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:50:17.469162 erddapy-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-20 17:50:03.000000 erddapy-2.0.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-20 17:50:03.000000 erddapy-2.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-20 17:50:03.000000 erddapy-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-20 17:50:17.469162 erddapy-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-20 17:50:03.000000 erddapy-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:50:17.469162 erddapy-2.0.1/erddapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:50:17.469162 erddapy-2.0.1/erddapy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/core/griddap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/core/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/core/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14312 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/core/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16215 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/erddapy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/multiple_server_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:50:17.469162 erddapy-2.0.1/erddapy/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/servers/erddaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/servers/servers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:50:17.469162 erddapy-2.0.1/erddapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-20 17:50:17.000000 erddapy-2.0.1/erddapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-20 17:50:03.000000 erddapy-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-20 17:50:03.000000 erddapy-2.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 17:50:03.000000 erddapy-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 17:50:17.469162 erddapy-2.0.1/setup.cfg
```

### Comparing `erddapy-2.0.0/CHANGES.txt` & `erddapy-2.0.1/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.0/LICENSE.txt` & `erddapy-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.0/PKG-INFO` & `erddapy-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erddapy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python interface for ERDDAP
 Author-email: Filipe Fernandes <ocefpaf+erddapy@gmail.com>
 License: Copyright 2017 Filipe Fernandes
         
         
         Redistribution and use in source and binary forms,
         with or without modification,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: erddapy Version: 2.0.0 Summary: Python interface
+Metadata-Version: 2.1 Name: erddapy Version: 2.0.1 Summary: Python interface
 for ERDDAP Author-email: Filipe Fernandes
 erddapy@gmail.com> License: Copyright 2017 Filipe Fernandes Redistribution and
 use in source and binary forms, with or without modification, are permitted
 provided that the following conditions are met: 1. Redistributions of source
 code must retain the above copyright notice, this list of conditions and the
 following disclaimer. 2. Redistributions in binary form must reproduce the
 above copyright notice, this list of conditions and the following disclaimer in
```

### Comparing `erddapy-2.0.0/README.md` & `erddapy-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.0/erddapy/core/__init__.py` & `erddapy-2.0.1/erddapy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.0/erddapy/core/griddap.py` & `erddapy-2.0.1/erddapy/core/griddap.py`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.0/erddapy/core/interfaces.py` & `erddapy-2.0.1/erddapy/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.0/erddapy/core/netcdf.py` & `erddapy-2.0.1/erddapy/core/netcdf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Handles netCDF responses."""
 
+import platform
 from contextlib import contextmanager
 from pathlib import Path
 from typing import BinaryIO, Dict, Generator, Optional
 from urllib.parse import urlparse
 
 from erddapy.core.url import urlopen
 
@@ -23,16 +24,21 @@
 
 
 @contextmanager
 def _tempnc(data: BinaryIO) -> Generator[str, None, None]:
     """Create a temporary netcdf file."""
     from tempfile import NamedTemporaryFile
 
+    # Let windows handle the file cleanup to avoid its aggressive file lock.
+    delete = True
+    if platform.system().lower() == "windows":
+        delete = False
+
     tmp = None
     try:
-        tmp = NamedTemporaryFile(suffix=".nc", prefix="erddapy_")
+        tmp = NamedTemporaryFile(suffix=".nc", prefix="erddapy_", delete=delete)
         tmp.write(data.read())
         tmp.flush()
         yield tmp.name
     finally:
         if tmp is not None:
             tmp.close()
```

### Comparing `erddapy-2.0.0/erddapy/core/url.py` & `erddapy-2.0.1/erddapy/core/url.py`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.0/erddapy/erddapy.py` & `erddapy-2.0.1/erddapy/erddapy.py`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.0/erddapy/multiple_server_search.py` & `erddapy-2.0.1/erddapy/multiple_server_search.py`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.0/erddapy/servers/erddaps.json` & `erddapy-2.0.1/erddapy/servers/erddaps.json`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.0/erddapy/servers/servers.py` & `erddapy-2.0.1/erddapy/servers/servers.py`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.0/pyproject.toml` & `erddapy-2.0.1/pyproject.toml`

 * *Files identical despite different names*

