# Comparing `tmp/bayanpy-0.6.4.tar.gz` & `tmp/bayanpy-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.6.4.tar", last modified: Thu Apr 20 14:11:36 2023, max compression
+gzip compressed data, was "bayanpy-0.6.5.tar", last modified: Thu Apr 20 14:32:35 2023, max compression
```

## Comparing `bayanpy-0.6.4.tar` & `bayanpy-0.6.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-20 14:11:36.150486 bayanpy-0.6.4/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.4/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-20 14:11:36.150486 bayanpy-0.6.4/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5056 2023-04-11 16:11:47.000000 bayanpy-0.6.4/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-20 14:11:36.146486 bayanpy-0.6.4/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    52486 2023-04-13 15:23:37.000000 bayanpy-0.6.4/bayanpy/BayanImplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.6.4/bayanpy/__init__.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-20 14:11:36.150486 bayanpy-0.6.4/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-20 14:11:36.000000 bayanpy-0.6.4/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-04-20 14:11:36.000000 bayanpy-0.6.4/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-20 14:11:36.000000 bayanpy-0.6.4/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       60 2023-04-20 14:11:36.000000 bayanpy-0.6.4/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-20 14:11:36.000000 bayanpy-0.6.4/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-20 14:11:36.150486 bayanpy-0.6.4/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      582 2023-04-20 14:11:09.000000 bayanpy-0.6.4/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-20 14:32:35.021626 bayanpy-0.6.5/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.5/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-20 14:32:35.021626 bayanpy-0.6.5/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5056 2023-04-11 16:11:47.000000 bayanpy-0.6.5/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-20 14:32:35.021626 bayanpy-0.6.5/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    52486 2023-04-13 15:23:37.000000 bayanpy-0.6.5/bayanpy/BayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.6.5/bayanpy/__init__.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-20 14:32:35.021626 bayanpy-0.6.5/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-20 14:32:34.000000 bayanpy-0.6.5/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-04-20 14:32:34.000000 bayanpy-0.6.5/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-20 14:32:34.000000 bayanpy-0.6.5/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       61 2023-04-20 14:32:34.000000 bayanpy-0.6.5/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-20 14:32:34.000000 bayanpy-0.6.5/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-20 14:32:35.021626 bayanpy-0.6.5/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      583 2023-04-20 14:32:28.000000 bayanpy-0.6.5/setup.py
```

### Comparing `bayanpy-0.6.4/LICENSE` & `bayanpy-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.4/README.md` & `bayanpy-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.4/bayanpy/BayanImplied.py` & `bayanpy-0.6.5/bayanpy/BayanImplied.py`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.4/setup.py` & `bayanpy-0.6.5/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.6.4",
+    version="0.6.5",
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
         "cdlib",
 	    "joblib",
-        "pycomb"
+        "pycombo"
     ],
 )
```

