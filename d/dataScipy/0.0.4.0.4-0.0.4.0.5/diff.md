# Comparing `tmp/dataScipy-0.0.4.0.4.tar.gz` & `tmp/dataScipy-0.0.4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataScipy-0.0.4.0.4.tar", last modified: Fri Apr  7 12:31:20 2023, max compression
+gzip compressed data, was "dataScipy-0.0.4.0.5.tar", last modified: Thu Apr 20 20:09:48 2023, max compression
```

## Comparing `dataScipy-0.0.4.0.4.tar` & `dataScipy-0.0.4.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bora       (501) staff       (20)        0 2023-04-07 12:31:20.562195 dataScipy-0.0.4.0.4/
--rw-r--r--   0 bora       (501) staff       (20)       66 2023-03-24 16:14:24.000000 dataScipy-0.0.4.0.4/AUTHORS.md
--rw-r--r--   0 bora       (501) staff       (20)     1066 2023-03-24 16:14:37.000000 dataScipy-0.0.4.0.4/LICENCE
--rw-r--r--   0 bora       (501) staff       (20)     1141 2023-04-07 12:31:20.562092 dataScipy-0.0.4.0.4/PKG-INFO
--rw-r--r--   0 bora       (501) staff       (20)      252 2023-03-24 16:14:44.000000 dataScipy-0.0.4.0.4/README.md
--rw-r--r--   0 bora       (501) staff       (20)     1030 2023-04-07 12:30:15.000000 dataScipy-0.0.4.0.4/pyproject.toml
--rw-r--r--   0 bora       (501) staff       (20)       38 2023-04-07 12:31:20.562224 dataScipy-0.0.4.0.4/setup.cfg
-drwxr-xr-x   0 bora       (501) staff       (20)        0 2023-04-07 12:31:20.560053 dataScipy-0.0.4.0.4/src/
-drwxr-xr-x   0 bora       (501) staff       (20)        0 2023-04-07 12:31:20.561196 dataScipy-0.0.4.0.4/src/dataScipy/
--rw-r--r--   0 bora       (501) staff       (20)    29031 2023-04-07 12:29:05.000000 dataScipy-0.0.4.0.4/src/dataScipy/DataScience.py
--rw-r--r--   0 bora       (501) staff       (20)      127 2023-04-07 12:28:23.000000 dataScipy-0.0.4.0.4/src/dataScipy/__init__.py
-drwxr-xr-x   0 bora       (501) staff       (20)        0 2023-04-07 12:31:20.561962 dataScipy-0.0.4.0.4/src/dataScipy.egg-info/
--rw-r--r--   0 bora       (501) staff       (20)     1141 2023-04-07 12:31:20.000000 dataScipy-0.0.4.0.4/src/dataScipy.egg-info/PKG-INFO
--rw-r--r--   0 bora       (501) staff       (20)      282 2023-04-07 12:31:20.000000 dataScipy-0.0.4.0.4/src/dataScipy.egg-info/SOURCES.txt
--rw-r--r--   0 bora       (501) staff       (20)        1 2023-04-07 12:31:20.000000 dataScipy-0.0.4.0.4/src/dataScipy.egg-info/dependency_links.txt
--rw-r--r--   0 bora       (501) staff       (20)       50 2023-04-07 12:31:20.000000 dataScipy-0.0.4.0.4/src/dataScipy.egg-info/requires.txt
--rw-r--r--   0 bora       (501) staff       (20)       10 2023-04-07 12:31:20.000000 dataScipy-0.0.4.0.4/src/dataScipy.egg-info/top_level.txt
+drwxr-xr-x   0 bora       (501) staff       (20)        0 2023-04-20 20:09:48.706694 dataScipy-0.0.4.0.5/
+-rw-r--r--   0 bora       (501) staff       (20)       66 2023-03-24 16:14:24.000000 dataScipy-0.0.4.0.5/AUTHORS.md
+-rw-r--r--   0 bora       (501) staff       (20)     1066 2023-03-24 16:14:37.000000 dataScipy-0.0.4.0.5/LICENCE
+-rw-r--r--   0 bora       (501) staff       (20)     1141 2023-04-20 20:09:48.706516 dataScipy-0.0.4.0.5/PKG-INFO
+-rw-r--r--   0 bora       (501) staff       (20)      252 2023-03-24 16:14:44.000000 dataScipy-0.0.4.0.5/README.md
+-rw-r--r--   0 bora       (501) staff       (20)     1030 2023-04-20 20:08:29.000000 dataScipy-0.0.4.0.5/pyproject.toml
+-rw-r--r--   0 bora       (501) staff       (20)       38 2023-04-20 20:09:48.706744 dataScipy-0.0.4.0.5/setup.cfg
+drwxr-xr-x   0 bora       (501) staff       (20)        0 2023-04-20 20:09:48.703714 dataScipy-0.0.4.0.5/src/
+drwxr-xr-x   0 bora       (501) staff       (20)        0 2023-04-20 20:09:48.705374 dataScipy-0.0.4.0.5/src/dataScipy/
+-rw-r--r--   0 bora       (501) staff       (20)    29039 2023-04-20 20:06:58.000000 dataScipy-0.0.4.0.5/src/dataScipy/DataScience.py
+-rw-r--r--   0 bora       (501) staff       (20)      127 2023-04-20 20:07:24.000000 dataScipy-0.0.4.0.5/src/dataScipy/__init__.py
+drwxr-xr-x   0 bora       (501) staff       (20)        0 2023-04-20 20:09:48.706298 dataScipy-0.0.4.0.5/src/dataScipy.egg-info/
+-rw-r--r--   0 bora       (501) staff       (20)     1141 2023-04-20 20:09:48.000000 dataScipy-0.0.4.0.5/src/dataScipy.egg-info/PKG-INFO
+-rw-r--r--   0 bora       (501) staff       (20)      282 2023-04-20 20:09:48.000000 dataScipy-0.0.4.0.5/src/dataScipy.egg-info/SOURCES.txt
+-rw-r--r--   0 bora       (501) staff       (20)        1 2023-04-20 20:09:48.000000 dataScipy-0.0.4.0.5/src/dataScipy.egg-info/dependency_links.txt
+-rw-r--r--   0 bora       (501) staff       (20)       50 2023-04-20 20:09:48.000000 dataScipy-0.0.4.0.5/src/dataScipy.egg-info/requires.txt
+-rw-r--r--   0 bora       (501) staff       (20)       10 2023-04-20 20:09:48.000000 dataScipy-0.0.4.0.5/src/dataScipy.egg-info/top_level.txt
```

### Comparing `dataScipy-0.0.4.0.4/LICENCE` & `dataScipy-0.0.4.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `dataScipy-0.0.4.0.4/PKG-INFO` & `dataScipy-0.0.4.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataScipy
-Version: 0.0.4.0.4
+Version: 0.0.4.0.5
 Summary: Python Library for some data-science tasks
 Author-email: Bora Aktas <baktas19@ku.edu.tr>
 Project-URL: Homepage, https://github.com/boraaktas/dataScipy
 Project-URL: Bug Tracker, https://github.com/boraaktas/dataScipy/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `dataScipy-0.0.4.0.4/pyproject.toml` & `dataScipy-0.0.4.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataScipy"
-version = "0.0.4.0.4"
+version = "0.0.4.0.5"
 authors = [
   { name="Bora Aktas", email="baktas19@ku.edu.tr" },
 ]
 description = "Python Library for some data-science tasks"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `dataScipy-0.0.4.0.4/src/dataScipy/DataScience.py` & `dataScipy-0.0.4.0.5/src/dataScipy/DataScience.py`

 * *Files 0% similar despite different names*

```diff
@@ -867,15 +867,15 @@
 
     AR_process = []
 
     for i in range(lenght_of_series + 1):
         if i == 0:
             AR_process.append(c)
         else:
-            AR_process.append(c + sum([phi[j] * AR_process[i - j - 1] for j in range(len(phi))]) + errors[i])
+            AR_process.append(c + sum([phi[j] * AR_process[i - j - 1] for j in range(len(phi))]) + errors[i - 1])
 
     return AR_process
 
 
 
 def generate_MA_process(c, theta, errors, lenght_of_series):
 
@@ -894,11 +894,11 @@
 
     MA_process = []
 
     for i in range(lenght_of_series + 1):
         if i == 0:
             MA_process.append(c)
         else:
-            MA_process.append(c + sum([theta[j] * errors[i - j - 1] for j in range(len(theta))]) + errors[i])
+            MA_process.append(c + sum([theta[j] * errors[i - j - 1] for j in range(len(theta))]) + errors[i - 1])
 
     return MA_process
```

### Comparing `dataScipy-0.0.4.0.4/src/dataScipy.egg-info/PKG-INFO` & `dataScipy-0.0.4.0.5/src/dataScipy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataScipy
-Version: 0.0.4.0.4
+Version: 0.0.4.0.5
 Summary: Python Library for some data-science tasks
 Author-email: Bora Aktas <baktas19@ku.edu.tr>
 Project-URL: Homepage, https://github.com/boraaktas/dataScipy
 Project-URL: Bug Tracker, https://github.com/boraaktas/dataScipy/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

