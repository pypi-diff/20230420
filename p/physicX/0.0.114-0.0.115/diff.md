# Comparing `tmp/physicX-0.0.114.tar.gz` & `tmp/physicX-0.0.115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicX-0.0.114.tar", last modified: Sun Apr  2 00:36:02 2023, max compression
+gzip compressed data, was "physicX-0.0.115.tar", last modified: Wed Apr 19 22:45:09 2023, max compression
```

## Comparing `physicX-0.0.114.tar` & `physicX-0.0.115.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-04-02 00:36:02.428685 physicX-0.0.114/
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      876 2023-04-02 00:36:02.428685 physicX-0.0.114/PKG-INFO
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      260 2023-04-02 00:27:49.000000 physicX-0.0.114/README.md
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      710 2023-04-02 00:35:44.000000 physicX-0.0.114/pyproject.toml
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)       38 2023-04-02 00:36:02.428685 physicX-0.0.114/setup.cfg
-drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-04-02 00:36:02.428685 physicX-0.0.114/src/
-drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-04-02 00:36:02.428685 physicX-0.0.114/src/physicX/
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)       50 2023-04-02 00:27:49.000000 physicX-0.0.114/src/physicX/__init__.py
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      340 2023-04-02 00:27:49.000000 physicX-0.0.114/src/physicX/constants.py
-drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-04-02 00:36:02.428685 physicX-0.0.114/src/physicX.egg-info/
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      876 2023-04-02 00:36:02.000000 physicX-0.0.114/src/physicX.egg-info/PKG-INFO
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      213 2023-04-02 00:36:02.000000 physicX-0.0.114/src/physicX.egg-info/SOURCES.txt
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)        1 2023-04-02 00:36:02.000000 physicX-0.0.114/src/physicX.egg-info/dependency_links.txt
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)        8 2023-04-02 00:36:02.000000 physicX-0.0.114/src/physicX.egg-info/top_level.txt
+drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-04-19 22:45:09.101896 physicX-0.0.115/
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)      826 2023-04-19 22:45:09.101896 physicX-0.0.115/PKG-INFO
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)      260 2023-04-14 12:09:52.000000 physicX-0.0.115/README.md
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)      771 2023-04-19 22:44:38.000000 physicX-0.0.115/pyproject.toml
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)       31 2023-04-19 22:02:53.000000 physicX-0.0.115/requirements.txt
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)       38 2023-04-19 22:45:09.101896 physicX-0.0.115/setup.cfg
+drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-04-19 22:45:09.101896 physicX-0.0.115/src/
+drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-04-19 22:45:09.101896 physicX-0.0.115/src/physicX/
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)       50 2023-04-14 12:09:52.000000 physicX-0.0.115/src/physicX/__init__.py
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)      402 2023-04-19 22:37:55.000000 physicX-0.0.115/src/physicX/constants.py
+drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-04-19 22:45:09.101896 physicX-0.0.115/src/physicX.egg-info/
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)      826 2023-04-19 22:45:09.000000 physicX-0.0.115/src/physicX.egg-info/PKG-INFO
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)      264 2023-04-19 22:45:09.000000 physicX-0.0.115/src/physicX.egg-info/SOURCES.txt
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)        1 2023-04-19 22:45:09.000000 physicX-0.0.115/src/physicX.egg-info/dependency_links.txt
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)       31 2023-04-19 22:45:09.000000 physicX-0.0.115/src/physicX.egg-info/requires.txt
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)        8 2023-04-19 22:45:09.000000 physicX-0.0.115/src/physicX.egg-info/top_level.txt
```

### Comparing `physicX-0.0.114/PKG-INFO` & `physicX-0.0.115/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: physicX
-Version: 0.0.114
-Summary: Mathematics and physics library
+Version: 0.0.115
+Summary: mathematics and physics library
 Author-email: anonymous14725 <anonymous14725@yahoo.com>
 Project-URL: Homepage, https://github.com/anonymous14725/physicX
 Project-URL: Bug Tracker, https://github.com/anonymous14725/physicX/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Other
+Classifier: Operating System :: Other OS
+Classifier: Environment :: GPU :: NVIDIA CUDA
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # PhysicX library for python
 This project with LICENSE GNU-GPLv3, in fact created for developers , physicist , mathematicians and this project
 <pre>pre-released</pre>
 github:https://github.com/anonymous14725/physicX <br/>
```

### Comparing `physicX-0.0.114/src/physicX.egg-info/PKG-INFO` & `physicX-0.0.115/src/physicX.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: physicX
-Version: 0.0.114
-Summary: Mathematics and physics library
+Version: 0.0.115
+Summary: mathematics and physics library
 Author-email: anonymous14725 <anonymous14725@yahoo.com>
 Project-URL: Homepage, https://github.com/anonymous14725/physicX
 Project-URL: Bug Tracker, https://github.com/anonymous14725/physicX/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Other
+Classifier: Operating System :: Other OS
+Classifier: Environment :: GPU :: NVIDIA CUDA
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # PhysicX library for python
 This project with LICENSE GNU-GPLv3, in fact created for developers , physicist , mathematicians and this project
 <pre>pre-released</pre>
 github:https://github.com/anonymous14725/physicX <br/>
```

