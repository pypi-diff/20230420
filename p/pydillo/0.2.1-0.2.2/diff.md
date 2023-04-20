# Comparing `tmp/pydillo-0.2.1.tar.gz` & `tmp/pydillo-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydillo-0.2.1.tar", last modified: Wed Apr 19 22:49:49 2023, max compression
+gzip compressed data, was "pydillo-0.2.2.tar", last modified: Thu Apr 20 17:24:45 2023, max compression
```

## Comparing `pydillo-0.2.1.tar` & `pydillo-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ermiry    (1000) ermiry    (1000)        0 2023-04-19 22:49:49.342453 pydillo-0.2.1/
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      795 2023-04-19 22:49:49.342453 pydillo-0.2.1/PKG-INFO
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      440 2023-04-19 21:57:16.000000 pydillo-0.2.1/README.md
-drwxr-xr-x   0 ermiry    (1000) ermiry    (1000)        0 2023-04-19 22:49:49.342453 pydillo-0.2.1/dillo/
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)     3644 2023-04-19 22:47:29.000000 pydillo-0.2.1/dillo/__init__.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)     2931 2023-04-19 21:57:16.000000 pydillo-0.2.1/dillo/auth.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      122 2023-04-19 21:57:16.000000 pydillo-0.2.1/dillo/lib.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)     2150 2023-04-19 22:43:20.000000 pydillo-0.2.1/dillo/magic.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)     3335 2023-04-19 21:57:16.000000 pydillo-0.2.1/dillo/routes.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      480 2023-04-19 21:57:16.000000 pydillo-0.2.1/dillo/service.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      578 2023-04-19 21:57:16.000000 pydillo-0.2.1/dillo/validation.py
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)     1491 2023-04-19 22:47:39.000000 pydillo-0.2.1/dillo/version.py
-drwxr-xr-x   0 ermiry    (1000) ermiry    (1000)        0 2023-04-19 22:49:49.342453 pydillo-0.2.1/pydillo.egg-info/
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      795 2023-04-19 22:49:49.000000 pydillo-0.2.1/pydillo.egg-info/PKG-INFO
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      297 2023-04-19 22:49:49.000000 pydillo-0.2.1/pydillo.egg-info/SOURCES.txt
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)        1 2023-04-19 22:49:49.000000 pydillo-0.2.1/pydillo.egg-info/dependency_links.txt
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)        6 2023-04-19 22:49:49.000000 pydillo-0.2.1/pydillo.egg-info/top_level.txt
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)       98 2023-04-19 21:57:16.000000 pydillo-0.2.1/pyproject.toml
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)      443 2023-04-19 22:49:49.343453 pydillo-0.2.1/setup.cfg
--rw-r--r--   0 ermiry    (1000) ermiry    (1000)       39 2023-04-19 21:57:16.000000 pydillo-0.2.1/setup.py
+drwxr-xr-x   0 ermiry    (1000) ermiry    (1000)        0 2023-04-20 17:24:45.825236 pydillo-0.2.2/
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      795 2023-04-20 17:24:45.825236 pydillo-0.2.2/PKG-INFO
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      440 2023-04-19 21:57:16.000000 pydillo-0.2.2/README.md
+drwxr-xr-x   0 ermiry    (1000) ermiry    (1000)        0 2023-04-20 17:24:45.824236 pydillo-0.2.2/dillo/
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)     4063 2023-04-20 17:16:55.000000 pydillo-0.2.2/dillo/__init__.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)     2931 2023-04-19 21:57:16.000000 pydillo-0.2.2/dillo/auth.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      122 2023-04-19 21:57:16.000000 pydillo-0.2.2/dillo/lib.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)     2168 2023-04-20 17:16:47.000000 pydillo-0.2.2/dillo/magic.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)     3335 2023-04-19 21:57:16.000000 pydillo-0.2.2/dillo/routes.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      480 2023-04-19 21:57:16.000000 pydillo-0.2.2/dillo/service.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      578 2023-04-19 21:57:16.000000 pydillo-0.2.2/dillo/validation.py
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)     1491 2023-04-20 17:23:56.000000 pydillo-0.2.2/dillo/version.py
+drwxr-xr-x   0 ermiry    (1000) ermiry    (1000)        0 2023-04-20 17:24:45.825236 pydillo-0.2.2/pydillo.egg-info/
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      795 2023-04-20 17:24:45.000000 pydillo-0.2.2/pydillo.egg-info/PKG-INFO
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      297 2023-04-20 17:24:45.000000 pydillo-0.2.2/pydillo.egg-info/SOURCES.txt
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)        1 2023-04-20 17:24:45.000000 pydillo-0.2.2/pydillo.egg-info/dependency_links.txt
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)        6 2023-04-20 17:24:45.000000 pydillo-0.2.2/pydillo.egg-info/top_level.txt
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)       98 2023-04-19 21:57:16.000000 pydillo-0.2.2/pyproject.toml
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)      443 2023-04-20 17:24:45.825236 pydillo-0.2.2/setup.cfg
+-rw-r--r--   0 ermiry    (1000) ermiry    (1000)       39 2023-04-19 21:57:16.000000 pydillo-0.2.2/setup.py
```

### Comparing `pydillo-0.2.1/PKG-INFO` & `pydillo-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydillo
-Version: 0.2.1
+Version: 0.2.2
 Summary: Common Dillo Development Module
 Author: Erick Salas
 Author-email: it@dillostores.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pydillo-0.2.1/dillo/__init__.py` & `pydillo-0.2.2/dillo/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,24 @@
 from .auth import dillo_auth_get_token_user
 from .auth import dillo_auth_get_token_username
 from .auth import dillo_auth_get_mask
 from .auth import dillo_auth_create
 from .auth import dillo_auth_print_token
 from .auth import dillo_custom_authentication_handler
 
+from .magic import SERVICE_STATUS_NONE
+from .magic import SERVICE_STATUS_CONNECTED
+from .magic import SERVICE_STATUS_READY
+from .magic import SERVICE_STATUS_IDLE
+from .magic import SERVICE_STATUS_WORK
+from .magic import SERVICE_STATUS_DISCONNECTED
+from .magic import SERVICE_STATUS_ENDING
+from .magic import SERVICE_STATUS_ERROR
+from .magic import service_status_to_string
+from .magic import service_status_description
 from .magic import MAGIC_REQUEST_NONE
 from .magic import MAGIC_REQUEST_STORE_REGISTER
 from .magic import MAGIC_REQUEST_STORE_UNREGISTER
 from .magic import MAGIC_REQUEST_STORE_STATUS
 from .magic import MAGIC_REQUEST_STORE_OPEN
 from .magic import MAGIC_REQUEST_STORE_CLOSE
 from .magic import MAGIC_REQUEST_STORE_DISABLE
@@ -81,8 +91,8 @@
 from .version import dillo_libauth_version_print_full
 from .version import dillo_libauth_version_print_version_id
 from .version import dillo_libauth_version_print_version_name
 from .version import pydillo_version_print_full
 from .version import pydillo_version_print_version_id
 from .version import pydillo_version_print_version_name
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `pydillo-0.2.1/dillo/auth.py` & `pydillo-0.2.2/dillo/auth.py`

 * *Files identical despite different names*

### Comparing `pydillo-0.2.1/dillo/magic.py` & `pydillo-0.2.2/dillo/magic.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 magic_request_type_to_string.restype = c_char_p
 
 magic_request_type_description = libmagic.magic_request_type_description
 magic_request_type_description.argtypes = [c_int]
 magic_request_type_description.restype = c_char_p
 
 magic_init = libmagic.magic_init
-magic_init.argtypes = [c_char_p, c_char_p, c_void_p, c_void_p]
+magic_init.argtypes = [c_char_p, c_uint, c_char_p, c_char_p, c_void_p, c_void_p]
 magic_init.restype = c_uint
 
 magic_end = libmagic.magic_end
 
 magic_handler_make_request = libmagic.magic_handler_make_request
 magic_handler_make_request.argtypes = [c_void_p, c_int, c_char_p, c_char_p, c_char_p]
 magic_handler_make_request.restype = c_uint
```

### Comparing `pydillo-0.2.1/dillo/routes.py` & `pydillo-0.2.2/dillo/routes.py`

 * *Files identical despite different names*

### Comparing `pydillo-0.2.1/dillo/validation.py` & `pydillo-0.2.2/dillo/validation.py`

 * *Files identical despite different names*

### Comparing `pydillo-0.2.1/dillo/version.py` & `pydillo-0.2.2/dillo/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from cerver.utils.log import LOG_TYPE_NONE, cerver_log_both
 
 from .lib import libauth, libmagic
 
-DILLO_VERSION = "0.2.1"
-DILLO_VERSION_NAME = "Version 0.2.1"
-DILLO_VERSION_DATE = "19/04/2023"
-DILLO_VERSION_TIME = "16:47 CST"
+DILLO_VERSION = "0.2.2"
+DILLO_VERSION_NAME = "Version 0.2.2"
+DILLO_VERSION_DATE = "20/04/2023"
+DILLO_VERSION_TIME = "11:23 CST"
 DILLO_VERSION_AUTHOR = "Erick Salas"
 
 version = {
 	"id": DILLO_VERSION,
 	"name": DILLO_VERSION_NAME,
 	"date": DILLO_VERSION_DATE,
 	"time": DILLO_VERSION_TIME,
```

### Comparing `pydillo-0.2.1/pydillo.egg-info/PKG-INFO` & `pydillo-0.2.2/pydillo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydillo
-Version: 0.2.1
+Version: 0.2.2
 Summary: Common Dillo Development Module
 Author: Erick Salas
 Author-email: it@dillostores.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

