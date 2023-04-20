# Comparing `tmp/datacheck-0.3.0.tar.gz` & `tmp/datacheck-0.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacheck-0.3.0.tar", last modified: Thu Apr 20 19:37:01 2023, max compression
+gzip compressed data, was "datacheck-0.3.0rc0.tar", last modified: Thu Apr 20 19:13:58 2023, max compression
```

## Comparing `datacheck-0.3.0.tar` & `datacheck-0.3.0rc0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:37:01.690176 datacheck-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-20 19:36:52.000000 datacheck-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 19:37:01.690176 datacheck-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-20 19:36:52.000000 datacheck-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:37:01.686176 datacheck-0.3.0/datacheck/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 19:36:52.000000 datacheck-0.3.0/datacheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-20 19:36:52.000000 datacheck-0.3.0/datacheck/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-20 19:36:52.000000 datacheck-0.3.0/datacheck/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-20 19:36:52.000000 datacheck-0.3.0/datacheck/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-20 19:36:52.000000 datacheck-0.3.0/datacheck/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:37:01.690176 datacheck-0.3.0/datacheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 19:37:01.000000 datacheck-0.3.0/datacheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-20 19:37:01.000000 datacheck-0.3.0/datacheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:37:01.000000 datacheck-0.3.0/datacheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 19:37:01.000000 datacheck-0.3.0/datacheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 19:37:01.000000 datacheck-0.3.0/datacheck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:37:01.690176 datacheck-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-20 19:36:52.000000 datacheck-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:13:58.482067 datacheck-0.3.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 19:13:58.482067 datacheck-0.3.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:13:58.482067 datacheck-0.3.0rc0/datacheck/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/datacheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/datacheck/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/datacheck/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/datacheck/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/datacheck/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:13:58.482067 datacheck-0.3.0rc0/datacheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-20 19:13:58.000000 datacheck-0.3.0rc0/datacheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-20 19:13:58.000000 datacheck-0.3.0rc0/datacheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:13:58.000000 datacheck-0.3.0rc0/datacheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 19:13:58.000000 datacheck-0.3.0rc0/datacheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 19:13:58.000000 datacheck-0.3.0rc0/datacheck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:13:58.482067 datacheck-0.3.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-20 19:13:49.000000 datacheck-0.3.0rc0/setup.py
```

### Comparing `datacheck-0.3.0/LICENSE` & `datacheck-0.3.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `datacheck-0.3.0/PKG-INFO` & `datacheck-0.3.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: datacheck
-Version: 0.3.0
+Version: 0.3.0rc0
 Summary: data validation library
 Home-page: https://github.com/csdev/datacheck
 Author: Christopher Sang
 License: MIT
-Classifier: Development Status :: 7 - Inactive
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 License-File: LICENSE
```

### Comparing `datacheck-0.3.0/datacheck/compat.py` & `datacheck-0.3.0rc0/datacheck/compat.py`

 * *Files identical despite different names*

### Comparing `datacheck-0.3.0/datacheck/core.py` & `datacheck-0.3.0rc0/datacheck/core.py`

 * *Files identical despite different names*

### Comparing `datacheck-0.3.0/datacheck/exceptions.py` & `datacheck-0.3.0rc0/datacheck/exceptions.py`

 * *Files identical despite different names*

### Comparing `datacheck-0.3.0/datacheck/path.py` & `datacheck-0.3.0rc0/datacheck/path.py`

 * *Files identical despite different names*

### Comparing `datacheck-0.3.0/datacheck.egg-info/PKG-INFO` & `datacheck-0.3.0rc0/datacheck.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: datacheck
-Version: 0.3.0
+Version: 0.3.0rc0
 Summary: data validation library
 Home-page: https://github.com/csdev/datacheck
 Author: Christopher Sang
 License: MIT
-Classifier: Development Status :: 7 - Inactive
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 License-File: LICENSE
```

### Comparing `datacheck-0.3.0/setup.py` & `datacheck-0.3.0rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,24 +32,24 @@
     def initialize_options(self):
         TestCommand.initialize_options(self)
         self.tox_args = '-r'
 
 
 setup(
     name='datacheck',
-    version='0.3.0',
+    version='0.3.0-rc0',
     packages=['datacheck'],
     url='https://github.com/csdev/datacheck',
     license='MIT',
     author='Christopher Sang',
     description='data validation library',
     long_description='data validation library',
 
     classifiers=[
-        'Development Status :: 7 - Inactive',
+        'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Utilities',
     ],
```

