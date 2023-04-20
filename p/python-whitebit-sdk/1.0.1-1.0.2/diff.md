# Comparing `tmp/python-whitebit-sdk-1.0.1.tar.gz` & `tmp/python-whitebit-sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-whitebit-sdk-1.0.1.tar", last modified: Thu Apr 20 10:36:13 2023, max compression
+gzip compressed data, was "python-whitebit-sdk-1.0.2.tar", last modified: Thu Apr 20 10:49:43 2023, max compression
```

## Comparing `python-whitebit-sdk-1.0.1.tar` & `python-whitebit-sdk-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:36:13.989400 python-whitebit-sdk-1.0.1/
--rw-r--r--   0 Artur      (502) staff       (20)     1075 2023-04-20 07:31:18.000000 python-whitebit-sdk-1.0.1/LICENSE
--rw-r--r--   0 Artur      (502) staff       (20)     4604 2023-04-20 10:36:13.989199 python-whitebit-sdk-1.0.1/PKG-INFO
--rw-r--r--   0 Artur      (502) staff       (20)     3813 2023-04-20 10:31:11.000000 python-whitebit-sdk-1.0.1/README.md
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:36:13.987571 python-whitebit-sdk-1.0.1/python_whitebit_sdk.egg-info/
--rw-r--r--   0 Artur      (502) staff       (20)     4604 2023-04-20 10:36:13.000000 python-whitebit-sdk-1.0.1/python_whitebit_sdk.egg-info/PKG-INFO
--rw-r--r--   0 Artur      (502) staff       (20)      354 2023-04-20 10:36:13.000000 python-whitebit-sdk-1.0.1/python_whitebit_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 Artur      (502) staff       (20)        1 2023-04-20 10:36:13.000000 python-whitebit-sdk-1.0.1/python_whitebit_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 Artur      (502) staff       (20)      129 2023-04-20 10:36:13.000000 python-whitebit-sdk-1.0.1/python_whitebit_sdk.egg-info/requires.txt
--rw-r--r--   0 Artur      (502) staff       (20)        9 2023-04-20 10:36:13.000000 python-whitebit-sdk-1.0.1/python_whitebit_sdk.egg-info/top_level.txt
--rw-r--r--   0 Artur      (502) staff       (20)       38 2023-04-20 10:36:13.989448 python-whitebit-sdk-1.0.1/setup.cfg
--rwxr-xr-x   0 Artur      (502) staff       (20)     5649 2023-04-20 10:25:16.000000 python-whitebit-sdk-1.0.1/setup.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:36:13.987995 python-whitebit-sdk-1.0.1/whitebit/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-1.0.1/whitebit/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)      109 2023-04-20 10:36:04.000000 python-whitebit-sdk-1.0.1/whitebit/__version__.py
--rw-r--r--   0 Artur      (502) staff       (20)     3193 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.1/whitebit/client.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:36:13.988587 python-whitebit-sdk-1.0.1/whitebit/stream/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.1/whitebit/stream/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)    21217 2023-04-19 15:02:27.000000 python-whitebit-sdk-1.0.1/whitebit/stream/ws.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:49:43.262725 python-whitebit-sdk-1.0.2/
+-rw-r--r--   0 Artur      (502) staff       (20)     1075 2023-04-20 07:31:18.000000 python-whitebit-sdk-1.0.2/LICENSE
+-rw-r--r--   0 Artur      (502) staff       (20)     4604 2023-04-20 10:49:43.262544 python-whitebit-sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 Artur      (502) staff       (20)     3813 2023-04-20 10:31:11.000000 python-whitebit-sdk-1.0.2/README.md
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:49:43.260707 python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/
+-rw-r--r--   0 Artur      (502) staff       (20)     4604 2023-04-20 10:49:43.000000 python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 Artur      (502) staff       (20)      354 2023-04-20 10:49:43.000000 python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 Artur      (502) staff       (20)        1 2023-04-20 10:49:43.000000 python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 Artur      (502) staff       (20)      129 2023-04-20 10:49:43.000000 python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/requires.txt
+-rw-r--r--   0 Artur      (502) staff       (20)        9 2023-04-20 10:49:43.000000 python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/top_level.txt
+-rw-r--r--   0 Artur      (502) staff       (20)       38 2023-04-20 10:49:43.262782 python-whitebit-sdk-1.0.2/setup.cfg
+-rwxr-xr-x   0 Artur      (502) staff       (20)     5649 2023-04-20 10:25:16.000000 python-whitebit-sdk-1.0.2/setup.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:49:43.261296 python-whitebit-sdk-1.0.2/whitebit/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-1.0.2/whitebit/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)      109 2023-04-20 10:49:22.000000 python-whitebit-sdk-1.0.2/whitebit/__version__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     3193 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.2/whitebit/client.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:49:43.261779 python-whitebit-sdk-1.0.2/whitebit/stream/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.2/whitebit/stream/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)    21217 2023-04-19 15:02:27.000000 python-whitebit-sdk-1.0.2/whitebit/stream/ws.py
```

### Comparing `python-whitebit-sdk-1.0.1/LICENSE` & `python-whitebit-sdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.1/PKG-INFO` & `python-whitebit-sdk-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-whitebit-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Clients and methods to interact with the Whitebit exchange.
 Home-page: https://github.com/whitebit-exchange/python-sdk
 Author: UAB Clear White Technologies
 Author-email: support@whitebit.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `python-whitebit-sdk-1.0.1/README.md` & `python-whitebit-sdk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.1/python_whitebit_sdk.egg-info/PKG-INFO` & `python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-whitebit-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Clients and methods to interact with the Whitebit exchange.
 Home-page: https://github.com/whitebit-exchange/python-sdk
 Author: UAB Clear White Technologies
 Author-email: support@whitebit.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `python-whitebit-sdk-1.0.1/setup.py` & `python-whitebit-sdk-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.1/whitebit/client.py` & `python-whitebit-sdk-1.0.2/whitebit/client.py`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.1/whitebit/stream/ws.py` & `python-whitebit-sdk-1.0.2/whitebit/stream/ws.py`

 * *Files identical despite different names*

