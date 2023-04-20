# Comparing `tmp/python-whitebit-sdk-1.0.2.tar.gz` & `tmp/python-whitebit-sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-whitebit-sdk-1.0.2.tar", last modified: Thu Apr 20 10:49:43 2023, max compression
+gzip compressed data, was "python-whitebit-sdk-1.0.3.tar", last modified: Thu Apr 20 12:09:00 2023, max compression
```

## Comparing `python-whitebit-sdk-1.0.2.tar` & `python-whitebit-sdk-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,46 @@
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:49:43.262725 python-whitebit-sdk-1.0.2/
--rw-r--r--   0 Artur      (502) staff       (20)     1075 2023-04-20 07:31:18.000000 python-whitebit-sdk-1.0.2/LICENSE
--rw-r--r--   0 Artur      (502) staff       (20)     4604 2023-04-20 10:49:43.262544 python-whitebit-sdk-1.0.2/PKG-INFO
--rw-r--r--   0 Artur      (502) staff       (20)     3813 2023-04-20 10:31:11.000000 python-whitebit-sdk-1.0.2/README.md
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:49:43.260707 python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/
--rw-r--r--   0 Artur      (502) staff       (20)     4604 2023-04-20 10:49:43.000000 python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/PKG-INFO
--rw-r--r--   0 Artur      (502) staff       (20)      354 2023-04-20 10:49:43.000000 python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 Artur      (502) staff       (20)        1 2023-04-20 10:49:43.000000 python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 Artur      (502) staff       (20)      129 2023-04-20 10:49:43.000000 python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/requires.txt
--rw-r--r--   0 Artur      (502) staff       (20)        9 2023-04-20 10:49:43.000000 python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/top_level.txt
--rw-r--r--   0 Artur      (502) staff       (20)       38 2023-04-20 10:49:43.262782 python-whitebit-sdk-1.0.2/setup.cfg
--rwxr-xr-x   0 Artur      (502) staff       (20)     5649 2023-04-20 10:25:16.000000 python-whitebit-sdk-1.0.2/setup.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:49:43.261296 python-whitebit-sdk-1.0.2/whitebit/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-1.0.2/whitebit/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)      109 2023-04-20 10:49:22.000000 python-whitebit-sdk-1.0.2/whitebit/__version__.py
--rw-r--r--   0 Artur      (502) staff       (20)     3193 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.2/whitebit/client.py
-drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 10:49:43.261779 python-whitebit-sdk-1.0.2/whitebit/stream/
--rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.2/whitebit/stream/__init__.py
--rw-r--r--   0 Artur      (502) staff       (20)    21217 2023-04-19 15:02:27.000000 python-whitebit-sdk-1.0.2/whitebit/stream/ws.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.683591 python-whitebit-sdk-1.0.3/
+-rw-r--r--   0 Artur      (502) staff       (20)     1075 2023-04-20 07:31:18.000000 python-whitebit-sdk-1.0.3/LICENSE
+-rw-r--r--   0 Artur      (502) staff       (20)     4605 2023-04-20 12:09:00.683446 python-whitebit-sdk-1.0.3/PKG-INFO
+-rw-r--r--   0 Artur      (502) staff       (20)     3813 2023-04-20 10:31:11.000000 python-whitebit-sdk-1.0.3/README.md
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.679431 python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/
+-rw-r--r--   0 Artur      (502) staff       (20)     4605 2023-04-20 12:09:00.000000 python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 Artur      (502) staff       (20)      932 2023-04-20 12:09:00.000000 python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 Artur      (502) staff       (20)        1 2023-04-20 12:09:00.000000 python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 Artur      (502) staff       (20)      107 2023-04-20 12:09:00.000000 python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/requires.txt
+-rw-r--r--   0 Artur      (502) staff       (20)        9 2023-04-20 12:09:00.000000 python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/top_level.txt
+-rw-r--r--   0 Artur      (502) staff       (20)       38 2023-04-20 12:09:00.683640 python-whitebit-sdk-1.0.3/setup.cfg
+-rwxr-xr-x   0 Artur      (502) staff       (20)     5623 2023-04-20 12:08:52.000000 python-whitebit-sdk-1.0.3/setup.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.679770 python-whitebit-sdk-1.0.3/whitebit/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-1.0.3/whitebit/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)      109 2023-04-20 12:08:52.000000 python-whitebit-sdk-1.0.3/whitebit/__version__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     3193 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/client.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.680013 python-whitebit-sdk-1.0.3/whitebit/collateral/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/__init__.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.680232 python-whitebit-sdk-1.0.3/whitebit/collateral/account/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/account/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     2261 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/account/account.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.680643 python-whitebit-sdk-1.0.3/whitebit/collateral/market/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/market/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)      481 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/market/market.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.680966 python-whitebit-sdk-1.0.3/whitebit/collateral/order/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/order/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     3347 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/collateral/order/order.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.681222 python-whitebit-sdk-1.0.3/whitebit/main/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-1.0.3/whitebit/main/__init__.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.681444 python-whitebit-sdk-1.0.3/whitebit/main/account/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/main/account/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     3645 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/main/account/account.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.681736 python-whitebit-sdk-1.0.3/whitebit/stream/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/stream/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)    21217 2023-04-19 15:02:27.000000 python-whitebit-sdk-1.0.3/whitebit/stream/ws.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.682201 python-whitebit-sdk-1.0.3/whitebit/trade/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:08:18.000000 python-whitebit-sdk-1.0.3/whitebit/trade/__init__.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.682480 python-whitebit-sdk-1.0.3/whitebit/trade/account/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/trade/account/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     3217 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/trade/account/account.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.682850 python-whitebit-sdk-1.0.3/whitebit/trade/market/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/trade/market/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     3437 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/trade/market/market.py
+drwxr-xr-x   0 Artur      (502) staff       (20)        0 2023-04-20 12:09:00.683149 python-whitebit-sdk-1.0.3/whitebit/trade/order/
+-rw-r--r--   0 Artur      (502) staff       (20)        0 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/trade/order/__init__.py
+-rw-r--r--   0 Artur      (502) staff       (20)     2862 2023-04-19 15:00:10.000000 python-whitebit-sdk-1.0.3/whitebit/trade/order/order.py
```

### Comparing `python-whitebit-sdk-1.0.2/LICENSE` & `python-whitebit-sdk-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.2/PKG-INFO` & `python-whitebit-sdk-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: python-whitebit-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Clients and methods to interact with the Whitebit exchange.
 Home-page: https://github.com/whitebit-exchange/python-sdk
 Author: UAB Clear White Technologies
 Author-email: support@whitebit.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >3.10.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 
 ## A Python SDK for [whitebit](https://www.whitebit.com)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `python-whitebit-sdk-1.0.2/README.md` & `python-whitebit-sdk-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.2/python_whitebit_sdk.egg-info/PKG-INFO` & `python-whitebit-sdk-1.0.3/python_whitebit_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: python-whitebit-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Clients and methods to interact with the Whitebit exchange.
 Home-page: https://github.com/whitebit-exchange/python-sdk
 Author: UAB Clear White Technologies
 Author-email: support@whitebit.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >3.10.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 
 ## A Python SDK for [whitebit](https://www.whitebit.com)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `python-whitebit-sdk-1.0.2/setup.py` & `python-whitebit-sdk-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 # Package meta-data.
 NAME = 'python-whitebit-sdk'
 DESCRIPTION = 'Clients and methods to interact with the Whitebit exchange.'
 URL = 'https://github.com/whitebit-exchange/python-sdk'
 EMAIL = 'support@whitebit.com'
 AUTHOR = 'UAB Clear White Technologies'
-REQUIRES_PYTHON = '>3.10.0'
+REQUIRES_PYTHON = '>=3.10.0'
 VERSION = None
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'python_version > 3.10.0', 'websockets>=10.4.0', 'asyncio>=3.4', 'requests>=2.28.1', 'responses>=0.23.1',
+    'websockets>=10.4.0', 'asyncio>=3.4', 'requests>=2.28.1', 'responses>=0.23.1',
     'urllib3==1.26.15'
 ]
 
 
 # What packages are optional?
 EXTRAS = {
     'testing': ['pytest', 'tqdm']
```

### Comparing `python-whitebit-sdk-1.0.2/whitebit/client.py` & `python-whitebit-sdk-1.0.3/whitebit/client.py`

 * *Files identical despite different names*

### Comparing `python-whitebit-sdk-1.0.2/whitebit/stream/ws.py` & `python-whitebit-sdk-1.0.3/whitebit/stream/ws.py`

 * *Files identical despite different names*

