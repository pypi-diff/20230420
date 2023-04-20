# Comparing `tmp/aib_logging-0.6.tar.gz` & `tmp/aib_logging-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aib_logging-0.6.tar", last modified: Fri Apr  7 07:44:46 2023, max compression
+gzip compressed data, was "aib_logging-0.7.tar", last modified: Thu Apr 20 10:16:27 2023, max compression
```

## Comparing `aib_logging-0.6.tar` & `aib_logging-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-07 07:44:46.508152 aib_logging-0.6/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-0.6/LICENSE.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      526 2023-04-07 07:44:46.508152 aib_logging-0.6/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-0.6/README.md
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      621 2023-04-07 07:44:32.000000 aib_logging-0.6/pyproject.toml
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-04-07 07:44:46.508152 aib_logging-0.6/setup.cfg
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-07 07:44:46.504152 aib_logging-0.6/src/
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-07 07:44:46.506152 aib_logging-0.6/src/aib_logging/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-0.6/src/aib_logging/__init__.py
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     6523 2023-04-07 07:41:47.000000 aib_logging-0.6/src/aib_logging/logger.py
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-07 07:44:46.508152 aib_logging-0.6/src/aib_logging.egg-info/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      526 2023-04-07 07:44:46.000000 aib_logging-0.6/src/aib_logging.egg-info/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-04-07 07:44:46.000000 aib_logging-0.6/src/aib_logging.egg-info/SOURCES.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-04-07 07:44:46.000000 aib_logging-0.6/src/aib_logging.egg-info/dependency_links.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       21 2023-04-07 07:44:46.000000 aib_logging-0.6/src/aib_logging.egg-info/requires.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-04-07 07:44:46.000000 aib_logging-0.6/src/aib_logging.egg-info/top_level.txt
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-20 10:16:27.898704 aib_logging-0.7/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-0.7/LICENSE.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      526 2023-04-20 10:16:27.898704 aib_logging-0.7/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-0.7/README.md
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      621 2023-04-20 09:54:45.000000 aib_logging-0.7/pyproject.toml
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-04-20 10:16:27.898704 aib_logging-0.7/setup.cfg
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-20 10:16:27.894704 aib_logging-0.7/src/
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-20 10:16:27.897704 aib_logging-0.7/src/aib_logging/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-0.7/src/aib_logging/__init__.py
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    12390 2023-04-20 09:39:28.000000 aib_logging-0.7/src/aib_logging/logger.py
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-20 10:16:27.898704 aib_logging-0.7/src/aib_logging.egg-info/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      526 2023-04-20 10:16:27.000000 aib_logging-0.7/src/aib_logging.egg-info/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-04-20 10:16:27.000000 aib_logging-0.7/src/aib_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-04-20 10:16:27.000000 aib_logging-0.7/src/aib_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       21 2023-04-20 10:16:27.000000 aib_logging-0.7/src/aib_logging.egg-info/requires.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-04-20 10:16:27.000000 aib_logging-0.7/src/aib_logging.egg-info/top_level.txt
```

### Comparing `aib_logging-0.6/LICENSE.txt` & `aib_logging-0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aib_logging-0.6/PKG-INFO` & `aib_logging-0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aib_logging
-Version: 0.6
+Version: 0.7
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aib_logging-0.6/pyproject.toml` & `aib_logging-0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aib_logging"
-version = "0.6"
+version = "0.7"
 authors = [
   { name="akib Shaikh", email="shaikhakib.k@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aib_logging-0.6/src/aib_logging.egg-info/PKG-INFO` & `aib_logging-0.7/src/aib_logging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aib-logging
-Version: 0.6
+Version: 0.7
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

