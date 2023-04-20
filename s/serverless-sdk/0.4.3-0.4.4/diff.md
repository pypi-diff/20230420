# Comparing `tmp/serverless-sdk-0.4.3.tar.gz` & `tmp/serverless-sdk-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-yntfdawy/serverless-sdk-0.4.3.tar", last modified: Thu Apr 20 12:15:32 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-voyigiic/serverless-sdk-0.4.4.tar", last modified: Thu Apr 20 20:12:25 2023, max compression
```

## Comparing `serverless-sdk-0.4.3.tar` & `serverless-sdk-0.4.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/serverless_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/sls_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/sls_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/sls_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/instrumentation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/instrumentation/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/sls_sdk/lib/warning_captured_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:15:32.000000 serverless-sdk-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/tests/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/tests/test_sdk_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-20 12:15:05.000000 serverless-sdk-0.4.3/tests/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/warning_captured_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.4.3/PKG-INFO` & `serverless-sdk-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.3
+Version: 0.4.4
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Requires-Python: >=3.7
```

### Comparing `serverless-sdk-0.4.3/README.md` & `serverless-sdk-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/pyproject.toml` & `serverless-sdk-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
     "setuptools>=65.6.3",
     "wheel>=0.38.4",
 ]
 
 [project]
 name = "serverless-sdk"
-version = "0.4.3"
+version = "0.4.4"
 description = "Serverless SDK for Python"
 readme = "README.md"
 authors = [{ name = "serverlessinc" }]
 requires-python = ">=3.7"
 dependencies = [
     "backports.cached-property", # included in Python >=3.8
     "blinker>=1.5",
```

### Comparing `serverless-sdk-0.4.3/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.4.4/serverless_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.3
+Version: 0.4.4
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Requires-Python: >=3.7
```

### Comparing `serverless-sdk-0.4.3/serverless_sdk.egg-info/SOURCES.txt` & `serverless-sdk-0.4.4/serverless_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/__init__.py` & `serverless-sdk-0.4.4/sls_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/exceptions.py` & `serverless-sdk-0.4.4/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/captured_event.py` & `serverless-sdk-0.4.4/sls_sdk/lib/captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/emitter.py` & `serverless-sdk-0.4.4/sls_sdk/lib/emitter.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/error.py` & `serverless-sdk-0.4.4/sls_sdk/lib/error.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/error_captured_event.py` & `serverless-sdk-0.4.4/sls_sdk/lib/error_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/instrumentation/flask.py` & `serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/instrumentation/http.py` & `serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/http.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/instrumentation/import_hook.py` & `serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/import_hook.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/name.py` & `serverless-sdk-0.4.4/sls_sdk/lib/name.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/tags.py` & `serverless-sdk-0.4.4/sls_sdk/lib/tags.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/trace.py` & `serverless-sdk-0.4.4/sls_sdk/lib/trace.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/warning.py` & `serverless-sdk-0.4.4/sls_sdk/lib/warning.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/sls_sdk/lib/warning_captured_event.py` & `serverless-sdk-0.4.4/sls_sdk/lib/warning_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/tests/test_sdk.py` & `serverless-sdk-0.4.4/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.3/tests/test_thread_safety.py` & `serverless-sdk-0.4.4/tests/test_thread_safety.py`

 * *Files identical despite different names*

