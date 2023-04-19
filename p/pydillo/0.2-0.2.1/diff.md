# Comparing `tmp/pydillo-0.2.tar.gz` & `tmp/pydillo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydillo-0.2.tar", last modified: Tue Mar  7 17:03:33 2023, max compression
+gzip compressed data, was "pydillo-0.2.1.tar", last modified: Wed Apr 19 22:49:49 2023, max compression
```

## Comparing `pydillo-0.2.tar` & `pydillo-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ermiry    (1000) ermiry    (1000)        0 2023-03-07 17:03:33.621949 pydillo-0.2/
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      793 2023-03-07 17:03:33.621949 pydillo-0.2/PKG-INFO
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      440 2022-11-09 02:45:37.000000 pydillo-0.2/README.md
-drwxr-xr-x   0 ermiry    (1000) ermiry    (1000)        0 2023-03-07 17:03:33.620949 pydillo-0.2/dillo/
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)     3642 2023-03-06 18:43:33.000000 pydillo-0.2/dillo/__init__.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)     2931 2023-03-06 18:16:51.000000 pydillo-0.2/dillo/auth.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      122 2023-03-06 18:27:31.000000 pydillo-0.2/dillo/lib.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)     1622 2023-03-06 18:37:47.000000 pydillo-0.2/dillo/magic.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)     3335 2023-03-06 18:17:08.000000 pydillo-0.2/dillo/routes.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      480 2023-03-06 18:17:21.000000 pydillo-0.2/dillo/service.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      578 2023-02-16 14:06:07.000000 pydillo-0.2/dillo/validation.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)     1487 2023-03-07 17:02:17.000000 pydillo-0.2/dillo/version.py
-drwxr-xr-x   0 ermiry    (1000) ermiry    (1000)        0 2023-03-07 17:03:33.621949 pydillo-0.2/pydillo.egg-info/
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      793 2023-03-07 17:03:33.000000 pydillo-0.2/pydillo.egg-info/PKG-INFO
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      297 2023-03-07 17:03:33.000000 pydillo-0.2/pydillo.egg-info/SOURCES.txt
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)        1 2023-03-07 17:03:33.000000 pydillo-0.2/pydillo.egg-info/dependency_links.txt
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)        6 2023-03-07 17:03:33.000000 pydillo-0.2/pydillo.egg-info/top_level.txt
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)       98 2022-11-09 02:45:52.000000 pydillo-0.2/pyproject.toml
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      441 2023-03-07 17:03:33.621949 pydillo-0.2/setup.cfg
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)       39 2022-11-09 02:43:23.000000 pydillo-0.2/setup.py
+drwxr-xr-x   0 ermiry    (1000) ermiry    (1000)        0 2023-04-19 22:49:49.342453 pydillo-0.2.1/
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      795 2023-04-19 22:49:49.342453 pydillo-0.2.1/PKG-INFO
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      440 2023-04-19 21:57:16.000000 pydillo-0.2.1/README.md
+drwxr-xr-x   0 ermiry    (1000) ermiry    (1000)        0 2023-04-19 22:49:49.342453 pydillo-0.2.1/dillo/
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)     3644 2023-04-19 22:47:29.000000 pydillo-0.2.1/dillo/__init__.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)     2931 2023-04-19 21:57:16.000000 pydillo-0.2.1/dillo/auth.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      122 2023-04-19 21:57:16.000000 pydillo-0.2.1/dillo/lib.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)     2150 2023-04-19 22:43:20.000000 pydillo-0.2.1/dillo/magic.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)     3335 2023-04-19 21:57:16.000000 pydillo-0.2.1/dillo/routes.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      480 2023-04-19 21:57:16.000000 pydillo-0.2.1/dillo/service.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      578 2023-04-19 21:57:16.000000 pydillo-0.2.1/dillo/validation.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)     1491 2023-04-19 22:47:39.000000 pydillo-0.2.1/dillo/version.py
+drwxr-xr-x   0 ermiry    (1000) ermiry    (1000)        0 2023-04-19 22:49:49.342453 pydillo-0.2.1/pydillo.egg-info/
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      795 2023-04-19 22:49:49.000000 pydillo-0.2.1/pydillo.egg-info/PKG-INFO
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      297 2023-04-19 22:49:49.000000 pydillo-0.2.1/pydillo.egg-info/SOURCES.txt
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)        1 2023-04-19 22:49:49.000000 pydillo-0.2.1/pydillo.egg-info/dependency_links.txt
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)        6 2023-04-19 22:49:49.000000 pydillo-0.2.1/pydillo.egg-info/top_level.txt
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)       98 2023-04-19 21:57:16.000000 pydillo-0.2.1/pyproject.toml
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      443 2023-04-19 22:49:49.343453 pydillo-0.2.1/setup.cfg
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)       39 2023-04-19 21:57:16.000000 pydillo-0.2.1/setup.py
```

### Comparing `pydillo-0.2/PKG-INFO` & `pydillo-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydillo
-Version: 0.2
+Version: 0.2.1
 Summary: Common Dillo Development Module
 Author: Erick Salas
 Author-email: it@dillostores.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pydillo-0.2/dillo/__init__.py` & `pydillo-0.2.1/dillo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,8 +81,8 @@
 from .version import dillo_libauth_version_print_full
 from .version import dillo_libauth_version_print_version_id
 from .version import dillo_libauth_version_print_version_name
 from .version import pydillo_version_print_full
 from .version import pydillo_version_print_version_id
 from .version import pydillo_version_print_version_name
 
-__version__ = "0.2"
+__version__ = "0.2.1"
```

### Comparing `pydillo-0.2/dillo/auth.py` & `pydillo-0.2.1/dillo/auth.py`

 * *Files identical despite different names*

### Comparing `pydillo-0.2/dillo/magic.py` & `pydillo-0.2.1/dillo/magic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 from ctypes import c_void_p, c_char_p, c_int, c_uint
 
 from .lib import libmagic
 
+SERVICE_STATUS_NONE = 0
+SERVICE_STATUS_CONNECTED = 1
+SERVICE_STATUS_READY = 2
+SERVICE_STATUS_IDLE = 3
+SERVICE_STATUS_WORK = 4
+SERVICE_STATUS_DISCONNECTED = 5
+SERVICE_STATUS_ENDING = 6
+SERVICE_STATUS_ERROR = 7
+
+service_status_to_string = libmagic.service_status_to_string
+service_status_to_string.argtypes = [c_int]
+service_status_to_string.restype = c_char_p
+
+service_status_description = libmagic.service_status_description
+service_status_description.argtypes = [c_int]
+service_status_description.restype = c_char_p
+
 MAGIC_REQUEST_NONE = 0
 MAGIC_REQUEST_STORE_REGISTER = 1
 MAGIC_REQUEST_STORE_UNREGISTER = 2
 MAGIC_REQUEST_STORE_STATUS = 3
 MAGIC_REQUEST_STORE_OPEN = 4
 MAGIC_REQUEST_STORE_CLOSE = 5
 MAGIC_REQUEST_STORE_DISABLE = 6
@@ -41,9 +58,9 @@
 magic_init = libmagic.magic_init
 magic_init.argtypes = [c_char_p, c_char_p, c_void_p, c_void_p]
 magic_init.restype = c_uint
 
 magic_end = libmagic.magic_end
 
 magic_handler_make_request = libmagic.magic_handler_make_request
-magic_handler_make_request.argtypes = [c_void_p, c_int, c_char_p, c_char_p]
+magic_handler_make_request.argtypes = [c_void_p, c_int, c_char_p, c_char_p, c_char_p]
 magic_handler_make_request.restype = c_uint
```

### Comparing `pydillo-0.2/dillo/routes.py` & `pydillo-0.2.1/dillo/routes.py`

 * *Files identical despite different names*

### Comparing `pydillo-0.2/dillo/validation.py` & `pydillo-0.2.1/dillo/validation.py`

 * *Files identical despite different names*

### Comparing `pydillo-0.2/dillo/version.py` & `pydillo-0.2.1/dillo/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from cerver.utils.log import LOG_TYPE_NONE, cerver_log_both
 
 from .lib import libauth, libmagic
 
-DILLO_VERSION = "0.2"
-DILLO_VERSION_NAME = "Version 0.2"
-DILLO_VERSION_DATE = "07/03/2023"
-DILLO_VERSION_TIME = "11:02 CST"
+DILLO_VERSION = "0.2.1"
+DILLO_VERSION_NAME = "Version 0.2.1"
+DILLO_VERSION_DATE = "19/04/2023"
+DILLO_VERSION_TIME = "16:47 CST"
 DILLO_VERSION_AUTHOR = "Erick Salas"
 
 version = {
 	"id": DILLO_VERSION,
 	"name": DILLO_VERSION_NAME,
 	"date": DILLO_VERSION_DATE,
 	"time": DILLO_VERSION_TIME,
```

### Comparing `pydillo-0.2/pydillo.egg-info/PKG-INFO` & `pydillo-0.2.1/pydillo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydillo
-Version: 0.2
+Version: 0.2.1
 Summary: Common Dillo Development Module
 Author: Erick Salas
 Author-email: it@dillostores.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

