# Comparing `tmp/python-whitebit-sdk-0.0.0.tar.gz` & `tmp/python-whitebit-sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-whitebit-sdk-0.0.0.tar", last modified: Thu Apr 20 10:04:03 2023, max compression
+gzip compressed data, was "python-whitebit-sdk-1.0.0.tar", last modified: Thu Apr 20 10:08:45 2023, max compression
```

## Comparing `python-whitebit-sdk-0.0.0.tar` & `python-whitebit-sdk-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:04:03.823951 python-whitebit-sdk-0.0.0/
--rw-r--r--   0 Artur      (502) staff       (20)     1075 2023-04-20 07:31:18.000000 python-whitebit-sdk-0.0.0/LICENSE
--rw-r--r--   0 Artur      (502) staff       (20)     4609 2023-04-20 10:04:03.823814 python-whitebit-sdk-0.0.0/PKG-INFO
--rw-r--r--   0 Artur      (502) staff       (20)     3817 2023-04-19 15:00:10.000000 python-whitebit-sdk-0.0.0/README.md
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:04:03.822587 python-whitebit-sdk-0.0.0/python_whitebit_sdk.egg-info/
--rw-r--r--   0 Artur      (502) staff       (20)     4609 2023-04-20 10:04:03.000000 python-whitebit-sdk-0.0.0/python_whitebit_sdk.egg-info/PKG-INFO
--rw-r--r--   0 Artur      (502) staff       (20)      354 2023-04-20 10:04:03.000000 python-whitebit-sdk-0.0.0/python_whitebit_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 Artur      (502) staff       (20)        1 2023-04-20 10:04:03.000000 python-whitebit-sdk-0.0.0/python_whitebit_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 Artur      (502) staff       (20)      130 2023-04-20 10:04:03.000000 python-whitebit-sdk-0.0.0/python_whitebit_sdk.egg-info/requires.txt
--rw-r--r--   0 Artur      (502) staff       (20)        9 2023-04-20 10:04:03.000000 python-whitebit-sdk-0.0.0/python_whitebit_sdk.egg-info/top_level.txt
--rw-r--r--   0 Artur      (502) staff       (20)       38 2023-04-20 10:04:03.823991 python-whitebit-sdk-0.0.0/setup.cfg
--rwxr-xr-x   0 Artur      (502) staff       (20)     5651 2023-04-20 10:00:42.000000 python-whitebit-sdk-0.0.0/setup.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:04:03.822953 python-whitebit-sdk-0.0.0/whitebit/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-0.0.0/whitebit/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)      109 2023-04-20 09:11:16.000000 python-whitebit-sdk-0.0.0/whitebit/__version__.py
--rw-r--r--   0 Artur      (502) staff       (20)     3193 2023-04-19 15:00:10.000000 python-whitebit-sdk-0.0.0/whitebit/client.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:04:03.823302 python-whitebit-sdk-0.0.0/whitebit/stream/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-0.0.0/whitebit/stream/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)    21217 2023-04-19 15:02:27.000000 python-whitebit-sdk-0.0.0/whitebit/stream/ws.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:08:45.958371 python-whitebit-sdk-1.0.0/
+-rw-r--r--   0 Artur      (502) staff       (20)     1075 2023-04-20 07:31:18.000000 python-whitebit-sdk-1.0.0/LICENSE
+-rw-r--r--   0 Artur      (502) staff       (20)     4609 2023-04-20 10:08:45.958258 python-whitebit-sdk-1.0.0/PKG-INFO
+-rw-r--r--   0 Artur      (502) staff       (20)     3817 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.0/README.md
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:08:45.957089 python-whitebit-sdk-1.0.0/python_whitebit_sdk.egg-info/
+-rw-r--r--   0 Artur      (502) staff       (20)     4609 2023-04-20 10:08:45.000000 python-whitebit-sdk-1.0.0/python_whitebit_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 Artur      (502) staff       (20)      354 2023-04-20 10:08:45.000000 python-whitebit-sdk-1.0.0/python_whitebit_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 Artur      (502) staff       (20)        1 2023-04-20 10:08:45.000000 python-whitebit-sdk-1.0.0/python_whitebit_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 Artur      (502) staff       (20)      130 2023-04-20 10:08:45.000000 python-whitebit-sdk-1.0.0/python_whitebit_sdk.egg-info/requires.txt
+-rw-r--r--   0 Artur      (502) staff       (20)        9 2023-04-20 10:08:45.000000 python-whitebit-sdk-1.0.0/python_whitebit_sdk.egg-info/top_level.txt
+-rw-r--r--   0 Artur      (502) staff       (20)       38 2023-04-20 10:08:45.958410 python-whitebit-sdk-1.0.0/setup.cfg
+-rwxr-xr-x   0 Artur      (502) staff       (20)     5651 2023-04-20 10:00:42.000000 python-whitebit-sdk-1.0.0/setup.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:08:45.957454 python-whitebit-sdk-1.0.0/whitebit/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-1.0.0/whitebit/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)      109 2023-04-20 10:08:32.000000 python-whitebit-sdk-1.0.0/whitebit/__version__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     3193 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.0/whitebit/client.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:08:45.957784 python-whitebit-sdk-1.0.0/whitebit/stream/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.0/whitebit/stream/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)    21217 2023-04-19 15:02:27.000000 python-whitebit-sdk-1.0.0/whitebit/stream/ws.py
```

### Comparing `python-whitebit-sdk-0.0.0/LICENSE` & `python-whitebit-sdk-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-0.0.0/PKG-INFO` & `python-whitebit-sdk-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-whitebit-sdk
-Version: 0.0.0
+Version: 1.0.0
 Summary: Clients and methods to interact with the Whitebit exchange.
 Home-page: https://github.com/whitebit-exchange/python-sdk
 Author: UAB Clear White Technologies
 Author-email: support@whitebit.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `python-whitebit-sdk-0.0.0/README.md` & `python-whitebit-sdk-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-0.0.0/python_whitebit_sdk.egg-info/PKG-INFO` & `python-whitebit-sdk-1.0.0/python_whitebit_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-whitebit-sdk
-Version: 0.0.0
+Version: 1.0.0
 Summary: Clients and methods to interact with the Whitebit exchange.
 Home-page: https://github.com/whitebit-exchange/python-sdk
 Author: UAB Clear White Technologies
 Author-email: support@whitebit.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `python-whitebit-sdk-0.0.0/setup.py` & `python-whitebit-sdk-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-0.0.0/whitebit/client.py` & `python-whitebit-sdk-1.0.0/whitebit/client.py`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-0.0.0/whitebit/stream/ws.py` & `python-whitebit-sdk-1.0.0/whitebit/stream/ws.py`

 * *Files identical despite different names*

