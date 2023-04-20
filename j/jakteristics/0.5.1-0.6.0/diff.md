# Comparing `tmp/jakteristics-0.5.1.tar.gz` & `tmp/jakteristics-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jakteristics-0.5.1.tar", last modified: Tue Apr 11 15:00:47 2023, max compression
+gzip compressed data, was "jakteristics-0.6.0.tar", last modified: Thu Apr 20 17:47:30 2023, max compression
```

## Comparing `jakteristics-0.5.1.tar` & `jakteristics-0.6.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:00:47.641589 jakteristics-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1397 2023-04-11 15:00:07.000000 jakteristics-0.5.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-04-11 15:00:07.000000 jakteristics-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3848 2023-04-11 15:00:47.641589 jakteristics-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1857 2023-04-11 15:00:07.000000 jakteristics-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:00:47.633589 jakteristics-0.5.1/jakteristics/
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:00:47.637589 jakteristics-0.5.1/jakteristics/ckdtree/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:00:47.637589 jakteristics-0.5.1/jakteristics/ckdtree/_lib/
--rw-r--r--   0 runner    (1001) docker     (122)     4804 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/_lib/_c99compat.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:00:47.629589 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:00:47.641589 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/
--rw-r--r--   0 runner    (1001) docker     (122)     7212 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/build.cxx
--rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/ckdtree_decl.h
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/coo_entries.h
--rw-r--r--   0 runner    (1001) docker     (122)    10227 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/count_neighbors.cxx
--rw-r--r--   0 runner    (1001) docker     (122)     8671 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/distance.h
--rw-r--r--   0 runner    (1001) docker     (122)     6966 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/distance_base.h
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/ordered_pair.h
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/partial_sort.h
--rw-r--r--   0 runner    (1001) docker     (122)    16106 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/query.cxx
--rw-r--r--   0 runner    (1001) docker     (122)     4671 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/query_ball_point.cxx
--rw-r--r--   0 runner    (1001) docker     (122)     7198 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/query_ball_tree.cxx
--rw-r--r--   0 runner    (1001) docker     (122)     7926 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/query_pairs.cxx
--rw-r--r--   0 runner    (1001) docker     (122)     8122 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/rectangle.h
--rw-r--r--   0 runner    (1001) docker     (122)     5442 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/sparse_distances.cxx
--rw-r--r--   0 runner    (1001) docker     (122)  1679533 2023-04-11 15:00:42.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    54227 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/ckdtree/ckdtree.pyx
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)   998913 2023-04-11 15:00:44.000000 jakteristics-0.5.1/jakteristics/extension.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8641 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/extension.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/las_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/main.py
--rw-r--r--   0 runner    (1001) docker     (122)   908553 2023-04-11 15:00:47.000000 jakteristics-0.5.1/jakteristics/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/utils.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     4305 2023-04-11 15:00:07.000000 jakteristics-0.5.1/jakteristics/utils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:00:47.633589 jakteristics-0.5.1/jakteristics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3848 2023-04-11 15:00:47.000000 jakteristics-0.5.1/jakteristics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-04-11 15:00:47.000000 jakteristics-0.5.1/jakteristics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 15:00:47.000000 jakteristics-0.5.1/jakteristics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-11 15:00:47.000000 jakteristics-0.5.1/jakteristics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 15:00:47.000000 jakteristics-0.5.1/jakteristics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 15:00:47.000000 jakteristics-0.5.1/jakteristics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-11 15:00:47.000000 jakteristics-0.5.1/jakteristics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-04-11 15:00:07.000000 jakteristics-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 15:00:07.000000 jakteristics-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 15:00:47.641589 jakteristics-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     3759 2023-04-11 15:00:07.000000 jakteristics-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 17:47:30.384108 jakteristics-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-04-20 17:46:57.000000 jakteristics-0.6.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-04-20 17:46:57.000000 jakteristics-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-04-20 17:47:30.384108 jakteristics-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1899 2023-04-20 17:46:57.000000 jakteristics-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 17:47:30.380108 jakteristics-0.6.0/jakteristics/
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 17:47:30.380108 jakteristics-0.6.0/jakteristics/ckdtree/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 17:47:30.380108 jakteristics-0.6.0/jakteristics/ckdtree/_lib/
+-rw-r--r--   0 runner    (1001) docker     (122)     4804 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/_lib/_c99compat.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 17:47:30.376108 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 17:47:30.384108 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     7212 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/build.cxx
+-rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/ckdtree_decl.h
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/coo_entries.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10227 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/count_neighbors.cxx
+-rw-r--r--   0 runner    (1001) docker     (122)     8671 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/distance.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6966 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/distance_base.h
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/ordered_pair.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/partial_sort.h
+-rw-r--r--   0 runner    (1001) docker     (122)    16106 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/query.cxx
+-rw-r--r--   0 runner    (1001) docker     (122)     4671 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/query_ball_point.cxx
+-rw-r--r--   0 runner    (1001) docker     (122)     7198 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/query_ball_tree.cxx
+-rw-r--r--   0 runner    (1001) docker     (122)     7926 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/query_pairs.cxx
+-rw-r--r--   0 runner    (1001) docker     (122)     8122 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/rectangle.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5442 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/sparse_distances.cxx
+-rw-r--r--   0 runner    (1001) docker     (122)  1679533 2023-04-20 17:47:26.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)    54227 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/ckdtree/ckdtree.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      523 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)  1022284 2023-04-20 17:47:27.000000 jakteristics-0.6.0/jakteristics/extension.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10135 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/extension.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/las_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)   908553 2023-04-20 17:47:30.000000 jakteristics-0.6.0/jakteristics/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     4305 2023-04-20 17:46:57.000000 jakteristics-0.6.0/jakteristics/utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 17:47:30.380108 jakteristics-0.6.0/jakteristics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-04-20 17:47:30.000000 jakteristics-0.6.0/jakteristics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-04-20 17:47:30.000000 jakteristics-0.6.0/jakteristics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 17:47:30.000000 jakteristics-0.6.0/jakteristics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-20 17:47:30.000000 jakteristics-0.6.0/jakteristics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 17:47:30.000000 jakteristics-0.6.0/jakteristics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 17:47:30.000000 jakteristics-0.6.0/jakteristics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-20 17:47:30.000000 jakteristics-0.6.0/jakteristics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-04-20 17:46:57.000000 jakteristics-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 17:46:57.000000 jakteristics-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 17:47:30.384108 jakteristics-0.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3759 2023-04-20 17:46:57.000000 jakteristics-0.6.0/setup.py
```

### Comparing `jakteristics-0.5.1/HISTORY.rst` & `jakteristics-0.6.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 History
 -------
 
 Unreleased
 ----------
 
 
+0.6.0 (2023-04-20)
+------------------
+
+* add: number_of_neighbors feature
+* add: eigenvalues and eigenvectors features
+
+
 0.5.1 (2023-04-11)
 ------------------
 
 * fix: computing features when kdtree is not built from the same points for which we want to compute the features
 * drop python 3.6, add wheels for python 3.7-3.11 on linux and windows
 
 0.5.0 (2022-01-26)
```

### Comparing `jakteristics-0.5.1/PKG-INFO` & `jakteristics-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jakteristics
-Version: 0.5.1
+Version: 0.6.0
 Summary: Point cloud geometric properties from python.
 Home-page: https://github.com/jakarto3d/jakteristics
 Author: David Caron
 Author-email: david.caron@jakarto.com
 License: BSD
 Keywords: jakteristics
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -70,15 +70,15 @@
 From python
 -----------
 
 .. code:: python
 
     from jakteristics import compute_features
 
-    features = compute_features(xyz, search_radius=0.15)
+    features = compute_features(xyz, search_radius=0.15, feature_names=['planarity', 'linearity'])
 
 
 CLI
 ---
 
 Once the package is installed, you can use the `jakteristics` command:
 
@@ -101,14 +101,21 @@
 History
 -------
 
 Unreleased
 ----------
 
 
+0.6.0 (2023-04-20)
+------------------
+
+* add: number_of_neighbors feature
+* add: eigenvalues and eigenvectors features
+
+
 0.5.1 (2023-04-11)
 ------------------
 
 * fix: computing features when kdtree is not built from the same points for which we want to compute the features
 * drop python 3.6, add wheels for python 3.7-3.11 on linux and windows
 
 0.5.0 (2022-01-26)
```

### Comparing `jakteristics-0.5.1/README.rst` & `jakteristics-0.6.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 From python
 -----------
 
 .. code:: python
 
     from jakteristics import compute_features
 
-    features = compute_features(xyz, search_radius=0.15)
+    features = compute_features(xyz, search_radius=0.15, feature_names=['planarity', 'linearity'])
 
 
 CLI
 ---
 
 Once the package is installed, you can use the `jakteristics` command:
```

### Comparing `jakteristics-0.5.1/jakteristics/__main__.py` & `jakteristics-0.6.0/jakteristics/__main__.py`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/__init__.py` & `jakteristics-0.6.0/jakteristics/ckdtree/__init__.py`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/_lib/_c99compat.h` & `jakteristics-0.6.0/jakteristics/ckdtree/_lib/_c99compat.h`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/build.cxx` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/build.cxx`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/ckdtree_decl.h` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/ckdtree_decl.h`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/count_neighbors.cxx` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/count_neighbors.cxx`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/distance.h` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/distance.h`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/distance_base.h` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/distance_base.h`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/partial_sort.h` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/partial_sort.h`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/query.cxx` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/query.cxx`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/query_ball_point.cxx` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/query_ball_point.cxx`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/query_ball_tree.cxx` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/query_ball_tree.cxx`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/query_pairs.cxx` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/query_pairs.cxx`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/rectangle.h` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/rectangle.h`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree/src/sparse_distances.cxx` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree/src/sparse_distances.cxx`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree.cpp` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,26 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "1"
             ]
         ],
         "depends": [
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/npy_math.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/npy_math.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "jakteristics/ckdtree/ckdtree/src/ckdtree_decl.h",
             "jakteristics/ckdtree/ckdtree/src/coo_entries.h",
             "jakteristics/ckdtree/ckdtree/src/ordered_pair.h"
         ],
         "include_dirs": [
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include",
             "jakteristics/ckdtree/ckdtree/src",
             "jakteristics/ckdtree/_lib"
         ],
         "language": "c++",
         "name": "jakteristics.ckdtree.ckdtree",
         "sources": [
             "jakteristics/ckdtree/ckdtree.pyx",
@@ -1159,195 +1159,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1384,42 +1384,42 @@
 struct __pyx_obj_12jakteristics_7ckdtree_7ckdtree___pyx_scope_struct__query;
 struct __pyx_obj_12jakteristics_7ckdtree_7ckdtree___pyx_scope_struct_1_query_ball_point;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -17470,15 +17470,15 @@
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_start);
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_end);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -17487,29 +17487,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -17520,15 +17520,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -17537,29 +17537,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -17570,15 +17570,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -17587,29 +17587,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -17620,15 +17620,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -17637,29 +17637,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -17670,15 +17670,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -17687,29 +17687,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -17720,212 +17720,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -17941,15 +17941,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -17957,53 +17957,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
@@ -18011,30 +18011,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18049,15 +18049,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18073,15 +18073,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18089,53 +18089,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
@@ -18143,30 +18143,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18181,15 +18181,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18205,15 +18205,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18221,53 +18221,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
@@ -18275,30 +18275,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18313,176 +18313,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -34217,26 +34217,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__32);
   __Pyx_GIVEREF(__pyx_tuple__32);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(3, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(3, 950, __pyx_L1_error)
```

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree.pxd` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree.pxd`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/ckdtree/ckdtree.pyx` & `jakteristics-0.6.0/jakteristics/ckdtree/ckdtree.pyx`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/extension.cpp` & `jakteristics-0.6.0/jakteristics/extension.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "1"
             ]
         ],
         "depends": [
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "jakteristics/ckdtree/ckdtree/src/ckdtree_decl.h"
         ],
         "extra_compile_args": [
             "-fopenmp"
         ],
         "extra_link_args": [
             "-fopenmp"
         ],
         "include_dirs": [
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include",
             "jakteristics/ckdtree/ckdtree/src",
             "jakteristics/ckdtree/_lib"
         ],
         "language": "c++",
         "name": "jakteristics.extension",
         "sources": [
             "jakteristics/extension.pyx",
@@ -1169,195 +1169,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1390,42 +1390,42 @@
 struct __pyx_obj_12jakteristics_7ckdtree_7ckdtree_cKDTreeNode;
 struct __pyx_obj_12jakteristics_7ckdtree_7ckdtree_cKDTree;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2565,15 +2565,15 @@
 static PyObject *generic = 0;
 static PyObject *strided = 0;
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
 static PyObject *indirect_contiguous = 0;
 static int __pyx_memoryview_thread_locks_used;
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
-static CYTHON_INLINE void __pyx_f_12jakteristics_9extension_compute_features_from_eigenvectors(__Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, std::map<std::string,uint8_t>  &); /*proto*/
+static CYTHON_INLINE void __pyx_f_12jakteristics_9extension_compute_features_from_eigenvectors(int, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, std::map<std::string,uint8_t>  &); /*proto*/
 static std::vector<__pyx_t_5numpy_intp_t>  ***__pyx_f_12jakteristics_9extension_init_result_vectors(int); /*proto*/
 static void __pyx_f_12jakteristics_9extension_free_result_vectors(std::vector<__pyx_t_5numpy_intp_t>  ***, int); /*proto*/
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
 static void *__pyx_align_pointer(void *, size_t); /*proto*/
 static PyObject *__pyx_memoryview_new(PyObject *, int, int, __Pyx_TypeInfo *); /*proto*/
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *); /*proto*/
@@ -2704,25 +2704,37 @@
 static const char __pyx_k_fill_value[] = "fill_value";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_sphericity[] = "sphericity";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
+static const char __pyx_k_eigenvalue1[] = "eigenvalue1";
+static const char __pyx_k_eigenvalue2[] = "eigenvalue2";
+static const char __pyx_k_eigenvalue3[] = "eigenvalue3";
 static const char __pyx_k_eigenvalues[] = "eigenvalues";
 static const char __pyx_k_neighbor_id[] = "neighbor_id";
 static const char __pyx_k_num_threads[] = "num_threads";
 static const char __pyx_k_verticality[] = "verticality";
 static const char __pyx_k_eigenentropy[] = "eigenentropy";
 static const char __pyx_k_eigenvectors[] = "eigenvectors";
 static const char __pyx_k_features_map[] = "features_map";
 static const char __pyx_k_omnivariance[] = "omnivariance";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_FEATURE_NAMES[] = "FEATURE_NAMES";
+static const char __pyx_k_eigenvector1x[] = "eigenvector1x";
+static const char __pyx_k_eigenvector1y[] = "eigenvector1y";
+static const char __pyx_k_eigenvector1z[] = "eigenvector1z";
+static const char __pyx_k_eigenvector2x[] = "eigenvector2x";
+static const char __pyx_k_eigenvector2y[] = "eigenvector2y";
+static const char __pyx_k_eigenvector2z[] = "eigenvector2z";
+static const char __pyx_k_eigenvector3x[] = "eigenvector3x";
+static const char __pyx_k_eigenvector3y[] = "eigenvector3y";
+static const char __pyx_k_eigenvector3z[] = "eigenvector3z";
 static const char __pyx_k_feature_names[] = "feature_names";
 static const char __pyx_k_pyx_getbuffer[] = "__pyx_getbuffer";
 static const char __pyx_k_radius_vector[] = "radius_vector";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_return_length[] = "return_length";
 static const char __pyx_k_search_radius[] = "search_radius";
 static const char __pyx_k_eigenvalue_sum[] = "eigenvalue_sum";
@@ -2738,14 +2750,15 @@
 static const char __pyx_k_compute_features[] = "compute_features";
 static const char __pyx_k_n_neighbors_at_id[] = "n_neighbors_at_id";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_surface_variation[] = "surface_variation";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_euclidean_distance[] = "euclidean_distance";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
+static const char __pyx_k_number_of_neighbors[] = "number_of_neighbors";
 static const char __pyx_k_Unknown_feature_name[] = "Unknown feature name: ";
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_jakteristics_extension[] = "jakteristics.extension";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
@@ -2859,14 +2872,15 @@
 static PyObject *__pyx_n_s_ndim;
 static PyObject *__pyx_n_s_neighbor_id;
 static PyObject *__pyx_n_s_neighbor_points;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_num_threads;
+static PyObject *__pyx_n_s_number_of_neighbors;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_s_order;
 static PyObject *__pyx_n_s_p;
 static PyObject *__pyx_n_s_pack;
@@ -3142,14 +3156,15 @@
   __Pyx_memviewslice __pyx_v_eigenvalues = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_v_i;
   int __pyx_v_j;
   int __pyx_v_k;
   uint32_t __pyx_v_neighbor_id;
   uint32_t __pyx_v_n_neighbors_at_id;
   int __pyx_v_thread_id;
+  int __pyx_v_number_of_neighbors;
   __Pyx_memviewslice __pyx_v_features = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_radius_vector = { 0, 0, { 0 }, { 0 }, { 0 } };
   __pyx_t_5numpy_float64_t __pyx_v_p;
   __pyx_t_5numpy_float64_t __pyx_v_eps_scipy;
   std::vector<__pyx_t_5numpy_intp_t>  ***__pyx_v_threaded_vvres;
   int __pyx_v_return_length;
   PyObject *__pyx_v_n = NULL;
@@ -3203,556 +3218,556 @@
  * 
  *         int64_t n_points = points.shape[0]             # <<<<<<<<<<<<<<
  *         double [::1, :] neighbor_points
  *         double [::1, :] eigenvectors
  */
   __pyx_v_n_points = (__pyx_v_points.shape[0]);
 
-  /* "jakteristics/extension.pyx":53
- *         int thread_id
+  /* "jakteristics/extension.pyx":54
+ *         int number_of_neighbors
  * 
  *         float [:, :] features = np.full((n_points, len(feature_names)), float("NaN"), dtype=np.float32)             # <<<<<<<<<<<<<<
  * 
  *         const np.float64_t[:, ::1] radius_vector
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_full); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_full); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int64_t(__pyx_v_n_points); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int64_t(__pyx_v_n_points); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyObject_Length(__pyx_v_feature_names); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 53, __pyx_L1_error)
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Length(__pyx_v_feature_names); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyNumber_Float(__pyx_n_u_NaN); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyNumber_Float(__pyx_n_u_NaN); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
   __pyx_t_5 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_features = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "jakteristics/extension.pyx":56
+  /* "jakteristics/extension.pyx":57
  * 
  *         const np.float64_t[:, ::1] radius_vector
  *         np.float64_t p = 2 if euclidean_distance else 1             # <<<<<<<<<<<<<<
  *         np.float64_t eps_scipy = 0.0
  *         vector[np.intp_t] *** threaded_vvres
  */
   if ((__pyx_v_euclidean_distance != 0)) {
     __pyx_t_8 = 2.0;
   } else {
     __pyx_t_8 = 1.0;
   }
   __pyx_v_p = __pyx_t_8;
 
-  /* "jakteristics/extension.pyx":57
+  /* "jakteristics/extension.pyx":58
  *         const np.float64_t[:, ::1] radius_vector
  *         np.float64_t p = 2 if euclidean_distance else 1
  *         np.float64_t eps_scipy = 0.0             # <<<<<<<<<<<<<<
  *         vector[np.intp_t] *** threaded_vvres
  *         int return_length = <int> False
  */
   __pyx_v_eps_scipy = 0.0;
 
-  /* "jakteristics/extension.pyx":59
+  /* "jakteristics/extension.pyx":60
  *         np.float64_t eps_scipy = 0.0
  *         vector[np.intp_t] *** threaded_vvres
  *         int return_length = <int> False             # <<<<<<<<<<<<<<
  * 
  *     if not points.shape[1] == 3:
  */
   __pyx_v_return_length = ((int)0);
 
-  /* "jakteristics/extension.pyx":61
+  /* "jakteristics/extension.pyx":62
  *         int return_length = <int> False
  * 
  *     if not points.shape[1] == 3:             # <<<<<<<<<<<<<<
  *         raise ValueError("You must provide an (n x 3) numpy array.")
  * 
  */
   __pyx_t_9 = ((!(((__pyx_v_points.shape[1]) == 3) != 0)) != 0);
   if (unlikely(__pyx_t_9)) {
 
-    /* "jakteristics/extension.pyx":62
+    /* "jakteristics/extension.pyx":63
  * 
  *     if not points.shape[1] == 3:
  *         raise ValueError("You must provide an (n x 3) numpy array.")             # <<<<<<<<<<<<<<
  * 
  *     if num_threads == -1:
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 62, __pyx_L1_error)
+    __PYX_ERR(0, 63, __pyx_L1_error)
 
-    /* "jakteristics/extension.pyx":61
+    /* "jakteristics/extension.pyx":62
  *         int return_length = <int> False
  * 
  *     if not points.shape[1] == 3:             # <<<<<<<<<<<<<<
  *         raise ValueError("You must provide an (n x 3) numpy array.")
  * 
  */
   }
 
-  /* "jakteristics/extension.pyx":64
+  /* "jakteristics/extension.pyx":65
  *         raise ValueError("You must provide an (n x 3) numpy array.")
  * 
  *     if num_threads == -1:             # <<<<<<<<<<<<<<
  *         num_threads = multiprocessing.cpu_count()
  * 
  */
   __pyx_t_9 = ((__pyx_v_num_threads == -1L) != 0);
   if (__pyx_t_9) {
 
-    /* "jakteristics/extension.pyx":65
+    /* "jakteristics/extension.pyx":66
  * 
  *     if num_threads == -1:
  *         num_threads = multiprocessing.cpu_count()             # <<<<<<<<<<<<<<
  * 
  *     if kdtree is None:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_multiprocessing); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_multiprocessing); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_cpu_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_cpu_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 65, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_t_6); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_t_6); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_num_threads = __pyx_t_10;
 
-    /* "jakteristics/extension.pyx":64
+    /* "jakteristics/extension.pyx":65
  *         raise ValueError("You must provide an (n x 3) numpy array.")
  * 
  *     if num_threads == -1:             # <<<<<<<<<<<<<<
  *         num_threads = multiprocessing.cpu_count()
  * 
  */
   }
 
-  /* "jakteristics/extension.pyx":67
+  /* "jakteristics/extension.pyx":68
  *         num_threads = multiprocessing.cpu_count()
  * 
  *     if kdtree is None:             # <<<<<<<<<<<<<<
  *         kdtree = cKDTree(points)
  * 
  */
   __pyx_t_9 = (((PyObject *)__pyx_v_kdtree) == Py_None);
   __pyx_t_11 = (__pyx_t_9 != 0);
   if (__pyx_t_11) {
 
-    /* "jakteristics/extension.pyx":68
+    /* "jakteristics/extension.pyx":69
  * 
  *     if kdtree is None:
  *         kdtree = cKDTree(points)             # <<<<<<<<<<<<<<
  * 
  *     for n, name in enumerate(feature_names):
  */
-    __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_points, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_points, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_12jakteristics_7ckdtree_7ckdtree_cKDTree), __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_12jakteristics_7ckdtree_7ckdtree_cKDTree), __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF_SET(__pyx_v_kdtree, ((struct __pyx_obj_12jakteristics_7ckdtree_7ckdtree_cKDTree *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "jakteristics/extension.pyx":67
+    /* "jakteristics/extension.pyx":68
  *         num_threads = multiprocessing.cpu_count()
  * 
  *     if kdtree is None:             # <<<<<<<<<<<<<<
  *         kdtree = cKDTree(points)
  * 
  */
   }
 
-  /* "jakteristics/extension.pyx":70
+  /* "jakteristics/extension.pyx":71
  *         kdtree = cKDTree(points)
  * 
  *     for n, name in enumerate(feature_names):             # <<<<<<<<<<<<<<
  *         if name not in FEATURE_NAMES:
  *             raise ValueError(f"Unknown feature name: {name}")
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_t_1 = __pyx_int_0;
   if (likely(PyList_CheckExact(__pyx_v_feature_names)) || PyTuple_CheckExact(__pyx_v_feature_names)) {
     __pyx_t_6 = __pyx_v_feature_names; __Pyx_INCREF(__pyx_t_6); __pyx_t_3 = 0;
     __pyx_t_12 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_feature_names); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 70, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_feature_names); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_12 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 70, __pyx_L1_error)
+    __pyx_t_12 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 71, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_12)) {
       if (likely(PyList_CheckExact(__pyx_t_6))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_6)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 70, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 71, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_6, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_6, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 70, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 71, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_6, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_6, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_12(__pyx_t_6);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 70, __pyx_L1_error)
+          else __PYX_ERR(0, 71, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_n, __pyx_t_1);
-    __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1);
     __pyx_t_1 = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "jakteristics/extension.pyx":71
+    /* "jakteristics/extension.pyx":72
  * 
  *     for n, name in enumerate(feature_names):
  *         if name not in FEATURE_NAMES:             # <<<<<<<<<<<<<<
  *             raise ValueError(f"Unknown feature name: {name}")
  *         features_map[name.encode()] = n
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FEATURE_NAMES); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FEATURE_NAMES); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_11 = (__Pyx_PySequence_ContainsTF(__pyx_v_name, __pyx_t_4, Py_NE)); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 71, __pyx_L1_error)
+    __pyx_t_11 = (__Pyx_PySequence_ContainsTF(__pyx_v_name, __pyx_t_4, Py_NE)); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 72, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = (__pyx_t_11 != 0);
     if (unlikely(__pyx_t_9)) {
 
-      /* "jakteristics/extension.pyx":72
+      /* "jakteristics/extension.pyx":73
  *     for n, name in enumerate(feature_names):
  *         if name not in FEATURE_NAMES:
  *             raise ValueError(f"Unknown feature name: {name}")             # <<<<<<<<<<<<<<
  *         features_map[name.encode()] = n
  * 
  */
-      __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unknown_feature_name, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unknown_feature_name, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 72, __pyx_L1_error)
+      __PYX_ERR(0, 73, __pyx_L1_error)
 
-      /* "jakteristics/extension.pyx":71
+      /* "jakteristics/extension.pyx":72
  * 
  *     for n, name in enumerate(feature_names):
  *         if name not in FEATURE_NAMES:             # <<<<<<<<<<<<<<
  *             raise ValueError(f"Unknown feature name: {name}")
  *         features_map[name.encode()] = n
  */
     }
 
-    /* "jakteristics/extension.pyx":73
+    /* "jakteristics/extension.pyx":74
  *         if name not in FEATURE_NAMES:
  *             raise ValueError(f"Unknown feature name: {name}")
  *         features_map[name.encode()] = n             # <<<<<<<<<<<<<<
  * 
  *     radius_vector = np.full((num_threads, 3), fill_value=search_radius)
  */
-    __pyx_t_13 = __Pyx_PyInt_As_uint8_t(__pyx_v_n); if (unlikely((__pyx_t_13 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_uint8_t(__pyx_v_n); if (unlikely((__pyx_t_13 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 74, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_14 = __pyx_convert_string_from_py_std__in_string(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L1_error)
+    __pyx_t_14 = __pyx_convert_string_from_py_std__in_string(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     (__pyx_v_features_map[__pyx_t_14]) = __pyx_t_13;
 
-    /* "jakteristics/extension.pyx":70
+    /* "jakteristics/extension.pyx":71
  *         kdtree = cKDTree(points)
  * 
  *     for n, name in enumerate(feature_names):             # <<<<<<<<<<<<<<
  *         if name not in FEATURE_NAMES:
  *             raise ValueError(f"Unknown feature name: {name}")
  */
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "jakteristics/extension.pyx":75
+  /* "jakteristics/extension.pyx":76
  *         features_map[name.encode()] = n
  * 
  *     radius_vector = np.full((num_threads, 3), fill_value=search_radius)             # <<<<<<<<<<<<<<
  *     neighbor_points = np.zeros([3, max_k_neighbors * num_threads], dtype=np.float64, order="F")
  *     eigenvectors = np.zeros([3, 3 * num_threads], dtype=np.float64, order="F")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_full); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_full); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_num_threads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_num_threads); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_int_3);
   __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_search_radius); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_search_radius); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_fill_value, __pyx_t_2) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_fill_value, __pyx_t_2) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_15 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_5numpy_float64_t__const__(__pyx_t_2, 0); if (unlikely(!__pyx_t_15.memview)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_5numpy_float64_t__const__(__pyx_t_2, 0); if (unlikely(!__pyx_t_15.memview)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_radius_vector = __pyx_t_15;
   __pyx_t_15.memview = NULL;
   __pyx_t_15.data = NULL;
 
-  /* "jakteristics/extension.pyx":76
+  /* "jakteristics/extension.pyx":77
  * 
  *     radius_vector = np.full((num_threads, 3), fill_value=search_radius)
  *     neighbor_points = np.zeros([3, max_k_neighbors * num_threads], dtype=np.float64, order="F")             # <<<<<<<<<<<<<<
  *     eigenvectors = np.zeros([3, 3 * num_threads], dtype=np.float64, order="F")
  *     eigenvalues = np.zeros(3 * num_threads, dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int((__pyx_v_max_k_neighbors * __pyx_v_num_threads)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int((__pyx_v_max_k_neighbors * __pyx_v_num_threads)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_int_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_order, __pyx_n_u_F) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_order, __pyx_n_u_F) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_dcd__double(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_dcd__double(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_neighbor_points = __pyx_t_16;
   __pyx_t_16.memview = NULL;
   __pyx_t_16.data = NULL;
 
-  /* "jakteristics/extension.pyx":77
+  /* "jakteristics/extension.pyx":78
  *     radius_vector = np.full((num_threads, 3), fill_value=search_radius)
  *     neighbor_points = np.zeros([3, max_k_neighbors * num_threads], dtype=np.float64, order="F")
  *     eigenvectors = np.zeros([3, 3 * num_threads], dtype=np.float64, order="F")             # <<<<<<<<<<<<<<
  *     eigenvalues = np.zeros(3 * num_threads, dtype=np.float64)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_long((3 * __pyx_v_num_threads)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_long((3 * __pyx_v_num_threads)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_int_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_order, __pyx_n_u_F) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_order, __pyx_n_u_F) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_dcd__double(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_dcd__double(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_eigenvectors = __pyx_t_16;
   __pyx_t_16.memview = NULL;
   __pyx_t_16.data = NULL;
 
-  /* "jakteristics/extension.pyx":78
+  /* "jakteristics/extension.pyx":79
  *     neighbor_points = np.zeros([3, max_k_neighbors * num_threads], dtype=np.float64, order="F")
  *     eigenvectors = np.zeros([3, 3 * num_threads], dtype=np.float64, order="F")
  *     eigenvalues = np.zeros(3 * num_threads, dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     threaded_vvres = init_result_vectors(num_threads)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_From_long((3 * __pyx_v_num_threads)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_long((3 * __pyx_v_num_threads)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_17 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_17.memview)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_17 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_17.memview)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_eigenvalues = __pyx_t_17;
   __pyx_t_17.memview = NULL;
   __pyx_t_17.data = NULL;
 
-  /* "jakteristics/extension.pyx":80
+  /* "jakteristics/extension.pyx":81
  *     eigenvalues = np.zeros(3 * num_threads, dtype=np.float64)
  * 
  *     threaded_vvres = init_result_vectors(num_threads)             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
   __pyx_v_threaded_vvres = __pyx_f_12jakteristics_9extension_init_result_vectors(__pyx_v_num_threads);
 
-  /* "jakteristics/extension.pyx":82
+  /* "jakteristics/extension.pyx":83
  *     threaded_vvres = init_result_vectors(num_threads)
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         for i in prange(n_points, nogil=True, num_threads=num_threads):
  *             thread_id = openmp.omp_get_thread_num()
  */
   /*try:*/ {
 
-    /* "jakteristics/extension.pyx":83
+    /* "jakteristics/extension.pyx":84
  * 
  *     try:
  *         for i in prange(n_points, nogil=True, num_threads=num_threads):             # <<<<<<<<<<<<<<
  *             thread_id = openmp.omp_get_thread_num()
  * 
  */
     {
@@ -3767,14 +3782,15 @@
           {
               int __pyx_parallel_temp0 = ((int)0xbad0bad0);
               int __pyx_parallel_temp1 = ((int)0xbad0bad0);
               int __pyx_parallel_temp2 = ((int)0xbad0bad0);
               uint32_t __pyx_parallel_temp3 = ((uint32_t)0xbad0bad0);
               uint32_t __pyx_parallel_temp4 = ((uint32_t)0xbad0bad0);
               int __pyx_parallel_temp5 = ((int)0xbad0bad0);
+              int __pyx_parallel_temp6 = ((int)0xbad0bad0);
               const char *__pyx_parallel_filename = NULL; int __pyx_parallel_lineno = 0, __pyx_parallel_clineno = 0;
               PyObject *__pyx_parallel_exc_type = NULL, *__pyx_parallel_exc_value = NULL, *__pyx_parallel_exc_tb = NULL;
               int __pyx_parallel_why;
               __pyx_parallel_why = 0;
               #if ((defined(__APPLE__) || defined(__OSX__)) && (defined(__GNUC__) && (__GNUC__ > 2 || (__GNUC__ == 2 && (__GNUC_MINOR__ > 95)))))
                   #undef likely
                   #undef unlikely
@@ -3791,66 +3807,67 @@
                       #ifdef _OPENMP
                       #ifdef WITH_THREAD
                       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
                       #endif
                       Py_BEGIN_ALLOW_THREADS
                       #endif /* _OPENMP */
                       #ifdef _OPENMP
-                      #pragma omp for firstprivate(__pyx_v_i) lastprivate(__pyx_v_i) lastprivate(__pyx_v_j) lastprivate(__pyx_v_k) lastprivate(__pyx_v_n_neighbors_at_id) lastprivate(__pyx_v_neighbor_id) lastprivate(__pyx_v_thread_id)
+                      #pragma omp for firstprivate(__pyx_v_i) lastprivate(__pyx_v_i) lastprivate(__pyx_v_j) lastprivate(__pyx_v_k) lastprivate(__pyx_v_n_neighbors_at_id) lastprivate(__pyx_v_neighbor_id) lastprivate(__pyx_v_number_of_neighbors) lastprivate(__pyx_v_thread_id)
                       #endif /* _OPENMP */
                       for (__pyx_t_19 = 0; __pyx_t_19 < __pyx_t_20; __pyx_t_19++){
                           if (__pyx_parallel_why < 2)
                           {
                               __pyx_v_i = (int)(0 + 1 * __pyx_t_19);
                               /* Initialize private variables to invalid values */
                               __pyx_v_j = ((int)0xbad0bad0);
                               __pyx_v_k = ((int)0xbad0bad0);
                               __pyx_v_n_neighbors_at_id = ((uint32_t)0xbad0bad0);
                               __pyx_v_neighbor_id = ((uint32_t)0xbad0bad0);
+                              __pyx_v_number_of_neighbors = ((int)0xbad0bad0);
                               __pyx_v_thread_id = ((int)0xbad0bad0);
 
-                              /* "jakteristics/extension.pyx":84
+                              /* "jakteristics/extension.pyx":85
  *     try:
  *         for i in prange(n_points, nogil=True, num_threads=num_threads):
  *             thread_id = openmp.omp_get_thread_num()             # <<<<<<<<<<<<<<
  * 
  *             threaded_vvres[thread_id][0].clear()
  */
                               __pyx_v_thread_id = omp_get_thread_num();
 
-                              /* "jakteristics/extension.pyx":86
+                              /* "jakteristics/extension.pyx":87
  *             thread_id = openmp.omp_get_thread_num()
  * 
  *             threaded_vvres[thread_id][0].clear()             # <<<<<<<<<<<<<<
  *             query_ball_point(
  *                 kdtree.cself,
  */
                               ((__pyx_v_threaded_vvres[__pyx_v_thread_id])[0])->clear();
 
-                              /* "jakteristics/extension.pyx":89
+                              /* "jakteristics/extension.pyx":90
  *             query_ball_point(
  *                 kdtree.cself,
  *                 &points[i, 0],             # <<<<<<<<<<<<<<
  *                 &radius_vector[thread_id, 0],
  *                 p,
  */
                               __pyx_t_21 = __pyx_v_i;
                               __pyx_t_22 = 0;
 
-                              /* "jakteristics/extension.pyx":90
+                              /* "jakteristics/extension.pyx":91
  *                 kdtree.cself,
  *                 &points[i, 0],
  *                 &radius_vector[thread_id, 0],             # <<<<<<<<<<<<<<
  *                 p,
  *                 eps_scipy,
  */
                               __pyx_t_23 = __pyx_v_thread_id;
                               __pyx_t_24 = 0;
 
-                              /* "jakteristics/extension.pyx":87
+                              /* "jakteristics/extension.pyx":88
  * 
  *             threaded_vvres[thread_id][0].clear()
  *             query_ball_point(             # <<<<<<<<<<<<<<
  *                 kdtree.cself,
  *                 &points[i, 0],
  */
                               try {
@@ -3859,129 +3876,138 @@
                                 #ifdef WITH_THREAD
                                 PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
                                 #endif
                                 __Pyx_CppExn2PyErr();
                                 #ifdef WITH_THREAD
                                 __Pyx_PyGILState_Release(__pyx_gilstate_save);
                                 #endif
-                                __PYX_ERR(0, 87, __pyx_L17_error)
+                                __PYX_ERR(0, 88, __pyx_L17_error)
                               }
 
-                              /* "jakteristics/extension.pyx":98
+                              /* "jakteristics/extension.pyx":99
  *             )
  * 
  *             n_neighbors_at_id = threaded_vvres[thread_id][0].size()             # <<<<<<<<<<<<<<
+ *             number_of_neighbors = n_neighbors_at_id
  * 
- *             if n_neighbors_at_id > max_k_neighbors:
  */
                               __pyx_v_n_neighbors_at_id = ((__pyx_v_threaded_vvres[__pyx_v_thread_id])[0])->size();
 
                               /* "jakteristics/extension.pyx":100
+ * 
  *             n_neighbors_at_id = threaded_vvres[thread_id][0].size()
+ *             number_of_neighbors = n_neighbors_at_id             # <<<<<<<<<<<<<<
+ * 
+ *             if n_neighbors_at_id > max_k_neighbors:
+ */
+                              __pyx_v_number_of_neighbors = __pyx_v_n_neighbors_at_id;
+
+                              /* "jakteristics/extension.pyx":102
+ *             number_of_neighbors = n_neighbors_at_id
  * 
  *             if n_neighbors_at_id > max_k_neighbors:             # <<<<<<<<<<<<<<
  *                 n_neighbors_at_id = max_k_neighbors
  *             elif n_neighbors_at_id == 0:
  */
                               __pyx_t_9 = ((__pyx_v_n_neighbors_at_id > __pyx_v_max_k_neighbors) != 0);
                               if (__pyx_t_9) {
 
-                                /* "jakteristics/extension.pyx":101
+                                /* "jakteristics/extension.pyx":103
  * 
  *             if n_neighbors_at_id > max_k_neighbors:
  *                 n_neighbors_at_id = max_k_neighbors             # <<<<<<<<<<<<<<
  *             elif n_neighbors_at_id == 0:
  *                 continue
  */
                                 __pyx_v_n_neighbors_at_id = __pyx_v_max_k_neighbors;
 
-                                /* "jakteristics/extension.pyx":100
- *             n_neighbors_at_id = threaded_vvres[thread_id][0].size()
+                                /* "jakteristics/extension.pyx":102
+ *             number_of_neighbors = n_neighbors_at_id
  * 
  *             if n_neighbors_at_id > max_k_neighbors:             # <<<<<<<<<<<<<<
  *                 n_neighbors_at_id = max_k_neighbors
  *             elif n_neighbors_at_id == 0:
  */
                                 goto __pyx_L19;
                               }
 
-                              /* "jakteristics/extension.pyx":102
+                              /* "jakteristics/extension.pyx":104
  *             if n_neighbors_at_id > max_k_neighbors:
  *                 n_neighbors_at_id = max_k_neighbors
  *             elif n_neighbors_at_id == 0:             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
                               __pyx_t_9 = ((__pyx_v_n_neighbors_at_id == 0) != 0);
                               if (__pyx_t_9) {
 
-                                /* "jakteristics/extension.pyx":103
+                                /* "jakteristics/extension.pyx":105
  *                 n_neighbors_at_id = max_k_neighbors
  *             elif n_neighbors_at_id == 0:
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             for j in range(n_neighbors_at_id):
  */
                                 goto __pyx_L15_continue;
 
-                                /* "jakteristics/extension.pyx":102
+                                /* "jakteristics/extension.pyx":104
  *             if n_neighbors_at_id > max_k_neighbors:
  *                 n_neighbors_at_id = max_k_neighbors
  *             elif n_neighbors_at_id == 0:             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
                               }
                               __pyx_L19:;
 
-                              /* "jakteristics/extension.pyx":105
+                              /* "jakteristics/extension.pyx":107
  *                 continue
  * 
  *             for j in range(n_neighbors_at_id):             # <<<<<<<<<<<<<<
  *                 neighbor_id = threaded_vvres[thread_id][0][0][j]
  *                 for k in range(3):
  */
                               __pyx_t_25 = __pyx_v_n_neighbors_at_id;
                               __pyx_t_26 = __pyx_t_25;
                               for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_26; __pyx_t_10+=1) {
                                 __pyx_v_j = __pyx_t_10;
 
-                                /* "jakteristics/extension.pyx":106
+                                /* "jakteristics/extension.pyx":108
  * 
  *             for j in range(n_neighbors_at_id):
  *                 neighbor_id = threaded_vvres[thread_id][0][0][j]             # <<<<<<<<<<<<<<
  *                 for k in range(3):
  *                     neighbor_points[k, thread_id * max_k_neighbors + j] = kdtree.cself.raw_data[neighbor_id * 3 + k]
  */
                                 __pyx_v_neighbor_id = ((((__pyx_v_threaded_vvres[__pyx_v_thread_id])[0])[0])[__pyx_v_j]);
 
-                                /* "jakteristics/extension.pyx":107
+                                /* "jakteristics/extension.pyx":109
  *             for j in range(n_neighbors_at_id):
  *                 neighbor_id = threaded_vvres[thread_id][0][0][j]
  *                 for k in range(3):             # <<<<<<<<<<<<<<
  *                     neighbor_points[k, thread_id * max_k_neighbors + j] = kdtree.cself.raw_data[neighbor_id * 3 + k]
  * 
  */
                                 for (__pyx_t_27 = 0; __pyx_t_27 < 3; __pyx_t_27+=1) {
                                   __pyx_v_k = __pyx_t_27;
 
-                                  /* "jakteristics/extension.pyx":108
+                                  /* "jakteristics/extension.pyx":110
  *                 neighbor_id = threaded_vvres[thread_id][0][0][j]
  *                 for k in range(3):
  *                     neighbor_points[k, thread_id * max_k_neighbors + j] = kdtree.cself.raw_data[neighbor_id * 3 + k]             # <<<<<<<<<<<<<<
  * 
  *             utils.c_covariance(
  */
                                   __pyx_t_24 = __pyx_v_k;
                                   __pyx_t_23 = ((__pyx_v_thread_id * __pyx_v_max_k_neighbors) + __pyx_v_j);
                                   *((double *) ( /* dim=1 */ (( /* dim=0 */ ((char *) (((double *) __pyx_v_neighbor_points.data) + __pyx_t_24)) ) + __pyx_t_23 * __pyx_v_neighbor_points.strides[1]) )) = (__pyx_v_kdtree->cself->raw_data[((__pyx_v_neighbor_id * 3) + __pyx_v_k)]);
                                 }
                               }
 
-                              /* "jakteristics/extension.pyx":111
+                              /* "jakteristics/extension.pyx":113
  * 
  *             utils.c_covariance(
  *                 neighbor_points[:, thread_id * max_k_neighbors:thread_id * max_k_neighbors + n_neighbors_at_id],             # <<<<<<<<<<<<<<
  *                 eigenvectors[:, thread_id * 3:(thread_id + 1) * 3],
  *             )
  */
                               __pyx_t_16.data = __pyx_v_neighbor_points.data;
@@ -4002,20 +4028,20 @@
     ((__pyx_v_thread_id * __pyx_v_max_k_neighbors) + __pyx_v_n_neighbors_at_id),
     0,
     1,
     1,
     0,
     1) < 0))
 {
-    __PYX_ERR(0, 111, __pyx_L17_error)
+    __PYX_ERR(0, 113, __pyx_L17_error)
 }
 
 __pyx_t_28.data = __pyx_v_eigenvectors.data;
 
-                              /* "jakteristics/extension.pyx":112
+                              /* "jakteristics/extension.pyx":114
  *             utils.c_covariance(
  *                 neighbor_points[:, thread_id * max_k_neighbors:thread_id * max_k_neighbors + n_neighbors_at_id],
  *                 eigenvectors[:, thread_id * 3:(thread_id + 1) * 3],             # <<<<<<<<<<<<<<
  *             )
  *             utils.c_eigenvectors(
  */
                               __pyx_t_28.memview = __pyx_v_eigenvectors.memview;
@@ -4035,34 +4061,34 @@
     ((__pyx_v_thread_id + 1) * 3),
     0,
     1,
     1,
     0,
     1) < 0))
 {
-    __PYX_ERR(0, 112, __pyx_L17_error)
+    __PYX_ERR(0, 114, __pyx_L17_error)
 }
 
 __pyx_f_12jakteristics_5utils_c_covariance(__pyx_t_16, __pyx_t_28);
 
-                              /* "jakteristics/extension.pyx":110
+                              /* "jakteristics/extension.pyx":112
  *                     neighbor_points[k, thread_id * max_k_neighbors + j] = kdtree.cself.raw_data[neighbor_id * 3 + k]
  * 
  *             utils.c_covariance(             # <<<<<<<<<<<<<<
  *                 neighbor_points[:, thread_id * max_k_neighbors:thread_id * max_k_neighbors + n_neighbors_at_id],
  *                 eigenvectors[:, thread_id * 3:(thread_id + 1) * 3],
  */
                               __PYX_XDEC_MEMVIEW(&__pyx_t_16, 0);
                               __pyx_t_16.memview = NULL;
                               __pyx_t_16.data = NULL;
                               __PYX_XDEC_MEMVIEW(&__pyx_t_28, 0);
                               __pyx_t_28.memview = NULL;
                               __pyx_t_28.data = NULL;
 
-                              /* "jakteristics/extension.pyx":115
+                              /* "jakteristics/extension.pyx":117
  *             )
  *             utils.c_eigenvectors(
  *                 eigenvectors[:, thread_id * 3:(thread_id + 1) * 3],             # <<<<<<<<<<<<<<
  *                 eigenvalues[thread_id * 3:(thread_id + 1) * 3],
  *             )
  */
                               __pyx_t_28.data = __pyx_v_eigenvectors.data;
@@ -4083,20 +4109,20 @@
     ((__pyx_v_thread_id + 1) * 3),
     0,
     1,
     1,
     0,
     1) < 0))
 {
-    __PYX_ERR(0, 115, __pyx_L17_error)
+    __PYX_ERR(0, 117, __pyx_L17_error)
 }
 
 __pyx_t_17.data = __pyx_v_eigenvalues.data;
 
-                              /* "jakteristics/extension.pyx":116
+                              /* "jakteristics/extension.pyx":118
  *             utils.c_eigenvectors(
  *                 eigenvectors[:, thread_id * 3:(thread_id + 1) * 3],
  *                 eigenvalues[thread_id * 3:(thread_id + 1) * 3],             # <<<<<<<<<<<<<<
  *             )
  * 
  */
                               __pyx_t_17.memview = __pyx_v_eigenvalues.memview;
@@ -4112,36 +4138,36 @@
     ((__pyx_v_thread_id + 1) * 3),
     0,
     1,
     1,
     0,
     1) < 0))
 {
-    __PYX_ERR(0, 116, __pyx_L17_error)
+    __PYX_ERR(0, 118, __pyx_L17_error)
 }
 
 __pyx_f_12jakteristics_5utils_c_eigenvectors(__pyx_t_28, __pyx_t_17);
 
-                              /* "jakteristics/extension.pyx":114
+                              /* "jakteristics/extension.pyx":116
  *                 eigenvectors[:, thread_id * 3:(thread_id + 1) * 3],
  *             )
  *             utils.c_eigenvectors(             # <<<<<<<<<<<<<<
  *                 eigenvectors[:, thread_id * 3:(thread_id + 1) * 3],
  *                 eigenvalues[thread_id * 3:(thread_id + 1) * 3],
  */
                               __PYX_XDEC_MEMVIEW(&__pyx_t_28, 0);
                               __pyx_t_28.memview = NULL;
                               __pyx_t_28.data = NULL;
                               __PYX_XDEC_MEMVIEW(&__pyx_t_17, 0);
                               __pyx_t_17.memview = NULL;
                               __pyx_t_17.data = NULL;
 
-                              /* "jakteristics/extension.pyx":120
- * 
+                              /* "jakteristics/extension.pyx":123
  *             compute_features_from_eigenvectors(
+ *                 number_of_neighbors,
  *                 eigenvalues[thread_id * 3 : thread_id * 3 + 3],             # <<<<<<<<<<<<<<
  *                 eigenvectors[:, thread_id * 3 : thread_id * 3 + 3],
  *                 features[i, :],
  */
                               __pyx_t_17.data = __pyx_v_eigenvalues.data;
                               __pyx_t_17.memview = __pyx_v_eigenvalues.memview;
                               __PYX_INC_MEMVIEW(&__pyx_t_17, 0);
@@ -4156,21 +4182,21 @@
     ((__pyx_v_thread_id * 3) + 3),
     0,
     1,
     1,
     0,
     1) < 0))
 {
-    __PYX_ERR(0, 120, __pyx_L17_error)
+    __PYX_ERR(0, 123, __pyx_L17_error)
 }
 
 __pyx_t_28.data = __pyx_v_eigenvectors.data;
 
-                              /* "jakteristics/extension.pyx":121
- *             compute_features_from_eigenvectors(
+                              /* "jakteristics/extension.pyx":124
+ *                 number_of_neighbors,
  *                 eigenvalues[thread_id * 3 : thread_id * 3 + 3],
  *                 eigenvectors[:, thread_id * 3 : thread_id * 3 + 3],             # <<<<<<<<<<<<<<
  *                 features[i, :],
  *                 features_map,
  */
                               __pyx_t_28.memview = __pyx_v_eigenvectors.memview;
                               __PYX_INC_MEMVIEW(&__pyx_t_28, 0);
@@ -4189,20 +4215,20 @@
     ((__pyx_v_thread_id * 3) + 3),
     0,
     1,
     1,
     0,
     1) < 0))
 {
-    __PYX_ERR(0, 121, __pyx_L17_error)
+    __PYX_ERR(0, 124, __pyx_L17_error)
 }
 
 __pyx_t_29.data = __pyx_v_features.data;
 
-                              /* "jakteristics/extension.pyx":122
+                              /* "jakteristics/extension.pyx":125
  *                 eigenvalues[thread_id * 3 : thread_id * 3 + 3],
  *                 eigenvectors[:, thread_id * 3 : thread_id * 3 + 3],
  *                 features[i, :],             # <<<<<<<<<<<<<<
  *                 features_map,
  *             )
  */
                               __pyx_t_29.memview = __pyx_v_features.memview;
@@ -4213,22 +4239,22 @@
         __pyx_t_29.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
 __pyx_t_29.shape[0] = __pyx_v_features.shape[1];
 __pyx_t_29.strides[0] = __pyx_v_features.strides[1];
     __pyx_t_29.suboffsets[0] = -1;
 
-__pyx_f_12jakteristics_9extension_compute_features_from_eigenvectors(__pyx_t_17, __pyx_t_28, __pyx_t_29, __pyx_v_features_map);
+__pyx_f_12jakteristics_9extension_compute_features_from_eigenvectors(__pyx_v_number_of_neighbors, __pyx_t_17, __pyx_t_28, __pyx_t_29, __pyx_v_features_map);
 
-                              /* "jakteristics/extension.pyx":119
+                              /* "jakteristics/extension.pyx":121
  *             )
  * 
  *             compute_features_from_eigenvectors(             # <<<<<<<<<<<<<<
+ *                 number_of_neighbors,
  *                 eigenvalues[thread_id * 3 : thread_id * 3 + 3],
- *                 eigenvectors[:, thread_id * 3 : thread_id * 3 + 3],
  */
                               __PYX_XDEC_MEMVIEW(&__pyx_t_17, 0);
                               __pyx_t_17.memview = NULL;
                               __pyx_t_17.data = NULL;
                               __PYX_XDEC_MEMVIEW(&__pyx_t_28, 0);
                               __pyx_t_28.memview = NULL;
                               __pyx_t_28.data = NULL;
@@ -4263,15 +4289,16 @@
                               #endif /* _OPENMP */
                               {
                                   __pyx_parallel_temp0 = __pyx_v_i;
                                   __pyx_parallel_temp1 = __pyx_v_j;
                                   __pyx_parallel_temp2 = __pyx_v_k;
                                   __pyx_parallel_temp3 = __pyx_v_n_neighbors_at_id;
                                   __pyx_parallel_temp4 = __pyx_v_neighbor_id;
-                                  __pyx_parallel_temp5 = __pyx_v_thread_id;
+                                  __pyx_parallel_temp5 = __pyx_v_number_of_neighbors;
+                                  __pyx_parallel_temp6 = __pyx_v_thread_id;
                               }
                               __pyx_L25:;
                               #ifdef _OPENMP
                               #pragma omp flush(__pyx_parallel_why)
                               #endif /* _OPENMP */
                           }
                       }
@@ -4302,15 +4329,16 @@
               }
               if (__pyx_parallel_why) {
                 __pyx_v_i = __pyx_parallel_temp0;
                 __pyx_v_j = __pyx_parallel_temp1;
                 __pyx_v_k = __pyx_parallel_temp2;
                 __pyx_v_n_neighbors_at_id = __pyx_parallel_temp3;
                 __pyx_v_neighbor_id = __pyx_parallel_temp4;
-                __pyx_v_thread_id = __pyx_parallel_temp5;
+                __pyx_v_number_of_neighbors = __pyx_parallel_temp5;
+                __pyx_v_thread_id = __pyx_parallel_temp6;
                 switch (__pyx_parallel_why) {
                       case 4:
                   {
                       #ifdef WITH_THREAD
                       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
                       #endif
                       __Pyx_GIVEREF(__pyx_parallel_exc_type);
@@ -4328,15 +4356,15 @@
               #undef likely
               #undef unlikely
               #define likely(x)   __builtin_expect(!!(x), 1)
               #define unlikely(x) __builtin_expect(!!(x), 0)
           #endif
         }
 
-        /* "jakteristics/extension.pyx":83
+        /* "jakteristics/extension.pyx":84
  * 
  *     try:
  *         for i in prange(n_points, nogil=True, num_threads=num_threads):             # <<<<<<<<<<<<<<
  *             thread_id = openmp.omp_get_thread_num()
  * 
  */
         /*finally:*/ {
@@ -4355,15 +4383,15 @@
             goto __pyx_L10_error;
           }
           __pyx_L14:;
         }
     }
   }
 
-  /* "jakteristics/extension.pyx":127
+  /* "jakteristics/extension.pyx":130
  * 
  *     finally:
  *         free_result_vectors(threaded_vvres, num_threads)             # <<<<<<<<<<<<<<
  * 
  *     return np.asarray(features)
  */
   /*finally:*/ {
@@ -4412,43 +4440,43 @@
       __pyx_t_31 = 0; __pyx_t_32 = 0; __pyx_t_33 = 0; __pyx_t_34 = 0; __pyx_t_35 = 0; __pyx_t_36 = 0;
       __pyx_lineno = __pyx_t_10; __pyx_clineno = __pyx_t_27; __pyx_filename = __pyx_t_30;
       goto __pyx_L1_error;
     }
     __pyx_L11:;
   }
 
-  /* "jakteristics/extension.pyx":129
+  /* "jakteristics/extension.pyx":132
  *         free_result_vectors(threaded_vvres, num_threads)
  * 
  *     return np.asarray(features)             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_features, 2, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_features, 2, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_2, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
   /* "jakteristics/extension.pyx":29
@@ -4485,23 +4513,23 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_points, 1);
   __Pyx_XDECREF((PyObject *)__pyx_v_kdtree);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jakteristics/extension.pyx":134
+/* "jakteristics/extension.pyx":137
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * cdef inline void compute_features_from_eigenvectors(             # <<<<<<<<<<<<<<
+ *     int number_of_neighbors,
  *     double [:] eigenvalues,
- *     double [:, :] eigenvectors,
  */
 
-static CYTHON_INLINE void __pyx_f_12jakteristics_9extension_compute_features_from_eigenvectors(__Pyx_memviewslice __pyx_v_eigenvalues, __Pyx_memviewslice __pyx_v_eigenvectors, __Pyx_memviewslice __pyx_v_out, std::map<std::string,uint8_t>  &__pyx_v_out_map) {
+static CYTHON_INLINE void __pyx_f_12jakteristics_9extension_compute_features_from_eigenvectors(int __pyx_v_number_of_neighbors, __Pyx_memviewslice __pyx_v_eigenvalues, __Pyx_memviewslice __pyx_v_eigenvectors, __Pyx_memviewslice __pyx_v_out, std::map<std::string,uint8_t>  &__pyx_v_out_map) {
   float __pyx_v_l1;
   float __pyx_v_l2;
   float __pyx_v_l3;
   float __pyx_v_eigenvalue_sum;
   float __pyx_v_n0;
   float __pyx_v_n1;
   float __pyx_v_n2;
@@ -4515,754 +4543,1318 @@
   __Pyx_FakeReference<uint8_t> __pyx_t_7;
   __Pyx_FakeReference<uint8_t> __pyx_t_8;
   __Pyx_FakeReference<uint8_t> __pyx_t_9;
   __Pyx_FakeReference<uint8_t> __pyx_t_10;
   __Pyx_FakeReference<uint8_t> __pyx_t_11;
   __Pyx_FakeReference<uint8_t> __pyx_t_12;
   __Pyx_FakeReference<uint8_t> __pyx_t_13;
-  Py_ssize_t __pyx_t_14;
+  __Pyx_FakeReference<uint8_t> __pyx_t_14;
   __Pyx_FakeReference<uint8_t> __pyx_t_15;
-  int __pyx_t_16;
-  Py_ssize_t __pyx_t_17;
+  __Pyx_FakeReference<uint8_t> __pyx_t_16;
+  __Pyx_FakeReference<uint8_t> __pyx_t_17;
   Py_ssize_t __pyx_t_18;
-  Py_ssize_t __pyx_t_19;
-  Py_ssize_t __pyx_t_20;
+  __Pyx_FakeReference<uint8_t> __pyx_t_19;
+  int __pyx_t_20;
   Py_ssize_t __pyx_t_21;
   Py_ssize_t __pyx_t_22;
-  __Pyx_FakeReference<uint8_t> __pyx_t_23;
-  __Pyx_FakeReference<uint8_t> __pyx_t_24;
-  __Pyx_FakeReference<uint8_t> __pyx_t_25;
+  Py_ssize_t __pyx_t_23;
+  Py_ssize_t __pyx_t_24;
+  Py_ssize_t __pyx_t_25;
+  Py_ssize_t __pyx_t_26;
+  __Pyx_FakeReference<uint8_t> __pyx_t_27;
+  __Pyx_FakeReference<uint8_t> __pyx_t_28;
+  __Pyx_FakeReference<uint8_t> __pyx_t_29;
+  __Pyx_FakeReference<uint8_t> __pyx_t_30;
+  __Pyx_FakeReference<uint8_t> __pyx_t_31;
+  __Pyx_FakeReference<uint8_t> __pyx_t_32;
+  __Pyx_FakeReference<uint8_t> __pyx_t_33;
+  __Pyx_FakeReference<uint8_t> __pyx_t_34;
+  __Pyx_FakeReference<uint8_t> __pyx_t_35;
+  __Pyx_FakeReference<uint8_t> __pyx_t_36;
+  __Pyx_FakeReference<uint8_t> __pyx_t_37;
+  __Pyx_FakeReference<uint8_t> __pyx_t_38;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "jakteristics/extension.pyx":146
+  /* "jakteristics/extension.pyx":150
  *         float norm
  * 
  *     l1 = eigenvalues[0]             # <<<<<<<<<<<<<<
  *     l2 = eigenvalues[1]
  *     l3 = eigenvalues[2]
  */
   __pyx_t_1 = 0;
   __pyx_v_l1 = (*((double *) ( /* dim=0 */ (__pyx_v_eigenvalues.data + __pyx_t_1 * __pyx_v_eigenvalues.strides[0]) )));
 
-  /* "jakteristics/extension.pyx":147
+  /* "jakteristics/extension.pyx":151
  * 
  *     l1 = eigenvalues[0]
  *     l2 = eigenvalues[1]             # <<<<<<<<<<<<<<
  *     l3 = eigenvalues[2]
  * 
  */
   __pyx_t_1 = 1;
   __pyx_v_l2 = (*((double *) ( /* dim=0 */ (__pyx_v_eigenvalues.data + __pyx_t_1 * __pyx_v_eigenvalues.strides[0]) )));
 
-  /* "jakteristics/extension.pyx":148
+  /* "jakteristics/extension.pyx":152
  *     l1 = eigenvalues[0]
  *     l2 = eigenvalues[1]
  *     l3 = eigenvalues[2]             # <<<<<<<<<<<<<<
  * 
  *     # Those features are inspired from cloud compare implementation (https://github.com/CloudCompare/CloudCompare/blob/master/CC/src/Neighbourhood.cpp#L871)
  */
   __pyx_t_1 = 2;
   __pyx_v_l3 = (*((double *) ( /* dim=0 */ (__pyx_v_eigenvalues.data + __pyx_t_1 * __pyx_v_eigenvalues.strides[0]) )));
 
-  /* "jakteristics/extension.pyx":154
+  /* "jakteristics/extension.pyx":158
  * 
  *     # Sum of eigenvalues equals the original variance of the data
  *     eigenvalue_sum = l1 + l2 + l3             # <<<<<<<<<<<<<<
  * 
- *     if out_map.count(b"eigenvalue_sum"):
+ *     if out_map.count(b"eigenvalue1"):
  */
   __pyx_v_eigenvalue_sum = ((__pyx_v_l1 + __pyx_v_l2) + __pyx_v_l3);
 
-  /* "jakteristics/extension.pyx":156
+  /* "jakteristics/extension.pyx":160
+ *     eigenvalue_sum = l1 + l2 + l3
+ * 
+ *     if out_map.count(b"eigenvalue1"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvalue1")] = l1
+ *     if out_map.count(b"eigenvalue2"):
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvalue1) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":161
+ * 
+ *     if out_map.count(b"eigenvalue1"):
+ *         out[out_map.at(b"eigenvalue1")] = l1             # <<<<<<<<<<<<<<
+ *     if out_map.count(b"eigenvalue2"):
+ *         out[out_map.at(b"eigenvalue2")] = l2
+ */
+    try {
+      __pyx_t_3 = __pyx_v_out_map.at(__pyx_k_eigenvalue1);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 161, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_3;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = __pyx_v_l1;
+
+    /* "jakteristics/extension.pyx":160
  *     eigenvalue_sum = l1 + l2 + l3
  * 
+ *     if out_map.count(b"eigenvalue1"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvalue1")] = l1
+ *     if out_map.count(b"eigenvalue2"):
+ */
+  }
+
+  /* "jakteristics/extension.pyx":162
+ *     if out_map.count(b"eigenvalue1"):
+ *         out[out_map.at(b"eigenvalue1")] = l1
+ *     if out_map.count(b"eigenvalue2"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvalue2")] = l2
+ *     if out_map.count(b"eigenvalue3"):
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvalue2) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":163
+ *         out[out_map.at(b"eigenvalue1")] = l1
+ *     if out_map.count(b"eigenvalue2"):
+ *         out[out_map.at(b"eigenvalue2")] = l2             # <<<<<<<<<<<<<<
+ *     if out_map.count(b"eigenvalue3"):
+ *         out[out_map.at(b"eigenvalue3")] = l3
+ */
+    try {
+      __pyx_t_5 = __pyx_v_out_map.at(__pyx_k_eigenvalue2);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 163, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_5;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = __pyx_v_l2;
+
+    /* "jakteristics/extension.pyx":162
+ *     if out_map.count(b"eigenvalue1"):
+ *         out[out_map.at(b"eigenvalue1")] = l1
+ *     if out_map.count(b"eigenvalue2"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvalue2")] = l2
+ *     if out_map.count(b"eigenvalue3"):
+ */
+  }
+
+  /* "jakteristics/extension.pyx":164
+ *     if out_map.count(b"eigenvalue2"):
+ *         out[out_map.at(b"eigenvalue2")] = l2
+ *     if out_map.count(b"eigenvalue3"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvalue3")] = l3
+ * 
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvalue3) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":165
+ *         out[out_map.at(b"eigenvalue2")] = l2
+ *     if out_map.count(b"eigenvalue3"):
+ *         out[out_map.at(b"eigenvalue3")] = l3             # <<<<<<<<<<<<<<
+ * 
+ *     if out_map.count(b"number_of_neighbors"):
+ */
+    try {
+      __pyx_t_6 = __pyx_v_out_map.at(__pyx_k_eigenvalue3);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 165, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_6;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = __pyx_v_l3;
+
+    /* "jakteristics/extension.pyx":164
+ *     if out_map.count(b"eigenvalue2"):
+ *         out[out_map.at(b"eigenvalue2")] = l2
+ *     if out_map.count(b"eigenvalue3"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvalue3")] = l3
+ * 
+ */
+  }
+
+  /* "jakteristics/extension.pyx":167
+ *         out[out_map.at(b"eigenvalue3")] = l3
+ * 
+ *     if out_map.count(b"number_of_neighbors"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"number_of_neighbors")] = number_of_neighbors
+ * 
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_number_of_neighbors) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":168
+ * 
+ *     if out_map.count(b"number_of_neighbors"):
+ *         out[out_map.at(b"number_of_neighbors")] = number_of_neighbors             # <<<<<<<<<<<<<<
+ * 
+ *     if out_map.count(b"eigenvalue_sum"):
+ */
+    try {
+      __pyx_t_7 = __pyx_v_out_map.at(__pyx_k_number_of_neighbors);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 168, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_7;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = __pyx_v_number_of_neighbors;
+
+    /* "jakteristics/extension.pyx":167
+ *         out[out_map.at(b"eigenvalue3")] = l3
+ * 
+ *     if out_map.count(b"number_of_neighbors"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"number_of_neighbors")] = number_of_neighbors
+ * 
+ */
+  }
+
+  /* "jakteristics/extension.pyx":170
+ *         out[out_map.at(b"number_of_neighbors")] = number_of_neighbors
+ * 
  *     if out_map.count(b"eigenvalue_sum"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"eigenvalue_sum")] = eigenvalue_sum
  * 
  */
   __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvalue_sum) != 0);
   if (__pyx_t_2) {
 
-    /* "jakteristics/extension.pyx":157
+    /* "jakteristics/extension.pyx":171
  * 
  *     if out_map.count(b"eigenvalue_sum"):
  *         out[out_map.at(b"eigenvalue_sum")] = eigenvalue_sum             # <<<<<<<<<<<<<<
  * 
  *     if out_map.count(b"omnivariance"):
  */
     try {
-      __pyx_t_3 = __pyx_v_out_map.at(__pyx_k_eigenvalue_sum);
+      __pyx_t_8 = __pyx_v_out_map.at(__pyx_k_eigenvalue_sum);
     } catch(...) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       __Pyx_CppExn2PyErr();
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 157, __pyx_L1_error)
+      __PYX_ERR(0, 171, __pyx_L1_error)
     }
-    __pyx_t_4 = __pyx_t_3;
+    __pyx_t_4 = __pyx_t_8;
     *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = __pyx_v_eigenvalue_sum;
 
-    /* "jakteristics/extension.pyx":156
- *     eigenvalue_sum = l1 + l2 + l3
+    /* "jakteristics/extension.pyx":170
+ *         out[out_map.at(b"number_of_neighbors")] = number_of_neighbors
  * 
  *     if out_map.count(b"eigenvalue_sum"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"eigenvalue_sum")] = eigenvalue_sum
  * 
  */
   }
 
-  /* "jakteristics/extension.pyx":159
+  /* "jakteristics/extension.pyx":173
  *         out[out_map.at(b"eigenvalue_sum")] = eigenvalue_sum
  * 
  *     if out_map.count(b"omnivariance"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"omnivariance")] = pow(l1 * l2 * l3, 1.0 / 3.0)
  * 
  */
   __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_omnivariance) != 0);
   if (__pyx_t_2) {
 
-    /* "jakteristics/extension.pyx":160
+    /* "jakteristics/extension.pyx":174
  * 
  *     if out_map.count(b"omnivariance"):
  *         out[out_map.at(b"omnivariance")] = pow(l1 * l2 * l3, 1.0 / 3.0)             # <<<<<<<<<<<<<<
  * 
  *     if out_map.count(b"eigenentropy"):
  */
     try {
-      __pyx_t_5 = __pyx_v_out_map.at(__pyx_k_omnivariance);
+      __pyx_t_9 = __pyx_v_out_map.at(__pyx_k_omnivariance);
     } catch(...) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       __Pyx_CppExn2PyErr();
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 160, __pyx_L1_error)
+      __PYX_ERR(0, 174, __pyx_L1_error)
     }
-    __pyx_t_4 = __pyx_t_5;
+    __pyx_t_4 = __pyx_t_9;
     *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = pow(((__pyx_v_l1 * __pyx_v_l2) * __pyx_v_l3), (1.0 / 3.0));
 
-    /* "jakteristics/extension.pyx":159
+    /* "jakteristics/extension.pyx":173
  *         out[out_map.at(b"eigenvalue_sum")] = eigenvalue_sum
  * 
  *     if out_map.count(b"omnivariance"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"omnivariance")] = pow(l1 * l2 * l3, 1.0 / 3.0)
  * 
  */
   }
 
-  /* "jakteristics/extension.pyx":162
+  /* "jakteristics/extension.pyx":176
  *         out[out_map.at(b"omnivariance")] = pow(l1 * l2 * l3, 1.0 / 3.0)
  * 
  *     if out_map.count(b"eigenentropy"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"eigenentropy")] = -(l1 * log(l1) + l2 * log(l2) + l3 * log(l3))
  * 
  */
   __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenentropy) != 0);
   if (__pyx_t_2) {
 
-    /* "jakteristics/extension.pyx":163
+    /* "jakteristics/extension.pyx":177
  * 
  *     if out_map.count(b"eigenentropy"):
  *         out[out_map.at(b"eigenentropy")] = -(l1 * log(l1) + l2 * log(l2) + l3 * log(l3))             # <<<<<<<<<<<<<<
  * 
  *     # Anisotropy is the difference between the most principal direction of the point subset.
  */
     try {
-      __pyx_t_6 = __pyx_v_out_map.at(__pyx_k_eigenentropy);
+      __pyx_t_10 = __pyx_v_out_map.at(__pyx_k_eigenentropy);
     } catch(...) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       __Pyx_CppExn2PyErr();
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 163, __pyx_L1_error)
+      __PYX_ERR(0, 177, __pyx_L1_error)
     }
-    __pyx_t_4 = __pyx_t_6;
+    __pyx_t_4 = __pyx_t_10;
     *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (-(((__pyx_v_l1 * log(__pyx_v_l1)) + (__pyx_v_l2 * log(__pyx_v_l2))) + (__pyx_v_l3 * log(__pyx_v_l3))));
 
-    /* "jakteristics/extension.pyx":162
+    /* "jakteristics/extension.pyx":176
  *         out[out_map.at(b"omnivariance")] = pow(l1 * l2 * l3, 1.0 / 3.0)
  * 
  *     if out_map.count(b"eigenentropy"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"eigenentropy")] = -(l1 * log(l1) + l2 * log(l2) + l3 * log(l3))
  * 
  */
   }
 
-  /* "jakteristics/extension.pyx":169
+  /* "jakteristics/extension.pyx":183
  *     # a difference close to zero (l3 close to l1) means that the subset of points are equally spread in the 3 principal directions
  *     # If the anisotropy is close to 1 (mean l3 close to zero), the subset of points is strongly related only in the first principal component. It depends mainly on one direction.
  *     if out_map.count(b"anisotropy"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"anisotropy")] = (l1 - l3) / l1
  *     if out_map.count(b"planarity"):
  */
   __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_anisotropy) != 0);
   if (__pyx_t_2) {
 
-    /* "jakteristics/extension.pyx":170
+    /* "jakteristics/extension.pyx":184
  *     # If the anisotropy is close to 1 (mean l3 close to zero), the subset of points is strongly related only in the first principal component. It depends mainly on one direction.
  *     if out_map.count(b"anisotropy"):
  *         out[out_map.at(b"anisotropy")] = (l1 - l3) / l1             # <<<<<<<<<<<<<<
  *     if out_map.count(b"planarity"):
  *         out[out_map.at(b"planarity")] = (l2 - l3) / l1
  */
     try {
-      __pyx_t_7 = __pyx_v_out_map.at(__pyx_k_anisotropy);
+      __pyx_t_11 = __pyx_v_out_map.at(__pyx_k_anisotropy);
     } catch(...) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       __Pyx_CppExn2PyErr();
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 170, __pyx_L1_error)
+      __PYX_ERR(0, 184, __pyx_L1_error)
     }
-    __pyx_t_4 = __pyx_t_7;
+    __pyx_t_4 = __pyx_t_11;
     *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = ((__pyx_v_l1 - __pyx_v_l3) / __pyx_v_l1);
 
-    /* "jakteristics/extension.pyx":169
+    /* "jakteristics/extension.pyx":183
  *     # a difference close to zero (l3 close to l1) means that the subset of points are equally spread in the 3 principal directions
  *     # If the anisotropy is close to 1 (mean l3 close to zero), the subset of points is strongly related only in the first principal component. It depends mainly on one direction.
  *     if out_map.count(b"anisotropy"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"anisotropy")] = (l1 - l3) / l1
  *     if out_map.count(b"planarity"):
  */
   }
 
-  /* "jakteristics/extension.pyx":171
+  /* "jakteristics/extension.pyx":185
  *     if out_map.count(b"anisotropy"):
  *         out[out_map.at(b"anisotropy")] = (l1 - l3) / l1
  *     if out_map.count(b"planarity"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"planarity")] = (l2 - l3) / l1
  *     if out_map.count(b"linearity"):
  */
   __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_planarity) != 0);
   if (__pyx_t_2) {
 
-    /* "jakteristics/extension.pyx":172
+    /* "jakteristics/extension.pyx":186
  *         out[out_map.at(b"anisotropy")] = (l1 - l3) / l1
  *     if out_map.count(b"planarity"):
  *         out[out_map.at(b"planarity")] = (l2 - l3) / l1             # <<<<<<<<<<<<<<
  *     if out_map.count(b"linearity"):
  *         out[out_map.at(b"linearity")] = (l1 - l2) / l1
  */
     try {
-      __pyx_t_8 = __pyx_v_out_map.at(__pyx_k_planarity);
+      __pyx_t_12 = __pyx_v_out_map.at(__pyx_k_planarity);
     } catch(...) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       __Pyx_CppExn2PyErr();
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 172, __pyx_L1_error)
+      __PYX_ERR(0, 186, __pyx_L1_error)
     }
-    __pyx_t_4 = __pyx_t_8;
+    __pyx_t_4 = __pyx_t_12;
     *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = ((__pyx_v_l2 - __pyx_v_l3) / __pyx_v_l1);
 
-    /* "jakteristics/extension.pyx":171
+    /* "jakteristics/extension.pyx":185
  *     if out_map.count(b"anisotropy"):
  *         out[out_map.at(b"anisotropy")] = (l1 - l3) / l1
  *     if out_map.count(b"planarity"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"planarity")] = (l2 - l3) / l1
  *     if out_map.count(b"linearity"):
  */
   }
 
-  /* "jakteristics/extension.pyx":173
+  /* "jakteristics/extension.pyx":187
  *     if out_map.count(b"planarity"):
  *         out[out_map.at(b"planarity")] = (l2 - l3) / l1
  *     if out_map.count(b"linearity"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"linearity")] = (l1 - l2) / l1
  *     if out_map.count(b"PCA1"):
  */
   __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_linearity) != 0);
   if (__pyx_t_2) {
 
-    /* "jakteristics/extension.pyx":174
+    /* "jakteristics/extension.pyx":188
  *         out[out_map.at(b"planarity")] = (l2 - l3) / l1
  *     if out_map.count(b"linearity"):
  *         out[out_map.at(b"linearity")] = (l1 - l2) / l1             # <<<<<<<<<<<<<<
  *     if out_map.count(b"PCA1"):
  *         out[out_map.at(b"PCA1")] = l1 / eigenvalue_sum
  */
     try {
-      __pyx_t_9 = __pyx_v_out_map.at(__pyx_k_linearity);
+      __pyx_t_13 = __pyx_v_out_map.at(__pyx_k_linearity);
     } catch(...) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       __Pyx_CppExn2PyErr();
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 174, __pyx_L1_error)
+      __PYX_ERR(0, 188, __pyx_L1_error)
     }
-    __pyx_t_4 = __pyx_t_9;
+    __pyx_t_4 = __pyx_t_13;
     *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = ((__pyx_v_l1 - __pyx_v_l2) / __pyx_v_l1);
 
-    /* "jakteristics/extension.pyx":173
+    /* "jakteristics/extension.pyx":187
  *     if out_map.count(b"planarity"):
  *         out[out_map.at(b"planarity")] = (l2 - l3) / l1
  *     if out_map.count(b"linearity"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"linearity")] = (l1 - l2) / l1
  *     if out_map.count(b"PCA1"):
  */
   }
 
-  /* "jakteristics/extension.pyx":175
+  /* "jakteristics/extension.pyx":189
  *     if out_map.count(b"linearity"):
  *         out[out_map.at(b"linearity")] = (l1 - l2) / l1
  *     if out_map.count(b"PCA1"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"PCA1")] = l1 / eigenvalue_sum
  *     if out_map.count(b"PCA2"):
  */
   __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_PCA1) != 0);
   if (__pyx_t_2) {
 
-    /* "jakteristics/extension.pyx":176
+    /* "jakteristics/extension.pyx":190
  *         out[out_map.at(b"linearity")] = (l1 - l2) / l1
  *     if out_map.count(b"PCA1"):
  *         out[out_map.at(b"PCA1")] = l1 / eigenvalue_sum             # <<<<<<<<<<<<<<
  *     if out_map.count(b"PCA2"):
  *         out[out_map.at(b"PCA2")] = l2 / eigenvalue_sum
  */
     try {
-      __pyx_t_10 = __pyx_v_out_map.at(__pyx_k_PCA1);
+      __pyx_t_14 = __pyx_v_out_map.at(__pyx_k_PCA1);
     } catch(...) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       __Pyx_CppExn2PyErr();
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 176, __pyx_L1_error)
+      __PYX_ERR(0, 190, __pyx_L1_error)
     }
-    __pyx_t_4 = __pyx_t_10;
+    __pyx_t_4 = __pyx_t_14;
     *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (__pyx_v_l1 / __pyx_v_eigenvalue_sum);
 
-    /* "jakteristics/extension.pyx":175
+    /* "jakteristics/extension.pyx":189
  *     if out_map.count(b"linearity"):
  *         out[out_map.at(b"linearity")] = (l1 - l2) / l1
  *     if out_map.count(b"PCA1"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"PCA1")] = l1 / eigenvalue_sum
  *     if out_map.count(b"PCA2"):
  */
   }
 
-  /* "jakteristics/extension.pyx":177
+  /* "jakteristics/extension.pyx":191
  *     if out_map.count(b"PCA1"):
  *         out[out_map.at(b"PCA1")] = l1 / eigenvalue_sum
  *     if out_map.count(b"PCA2"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"PCA2")] = l2 / eigenvalue_sum
  *     # Surface variance is how the third component contributes to the sum of the eigenvalues
  */
   __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_PCA2) != 0);
   if (__pyx_t_2) {
 
-    /* "jakteristics/extension.pyx":178
+    /* "jakteristics/extension.pyx":192
  *         out[out_map.at(b"PCA1")] = l1 / eigenvalue_sum
  *     if out_map.count(b"PCA2"):
  *         out[out_map.at(b"PCA2")] = l2 / eigenvalue_sum             # <<<<<<<<<<<<<<
  *     # Surface variance is how the third component contributes to the sum of the eigenvalues
  *     if out_map.count(b"surface_variation"):
  */
     try {
-      __pyx_t_11 = __pyx_v_out_map.at(__pyx_k_PCA2);
+      __pyx_t_15 = __pyx_v_out_map.at(__pyx_k_PCA2);
     } catch(...) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       __Pyx_CppExn2PyErr();
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 178, __pyx_L1_error)
+      __PYX_ERR(0, 192, __pyx_L1_error)
     }
-    __pyx_t_4 = __pyx_t_11;
+    __pyx_t_4 = __pyx_t_15;
     *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (__pyx_v_l2 / __pyx_v_eigenvalue_sum);
 
-    /* "jakteristics/extension.pyx":177
+    /* "jakteristics/extension.pyx":191
  *     if out_map.count(b"PCA1"):
  *         out[out_map.at(b"PCA1")] = l1 / eigenvalue_sum
  *     if out_map.count(b"PCA2"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"PCA2")] = l2 / eigenvalue_sum
  *     # Surface variance is how the third component contributes to the sum of the eigenvalues
  */
   }
 
-  /* "jakteristics/extension.pyx":180
+  /* "jakteristics/extension.pyx":194
  *         out[out_map.at(b"PCA2")] = l2 / eigenvalue_sum
  *     # Surface variance is how the third component contributes to the sum of the eigenvalues
  *     if out_map.count(b"surface_variation"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"surface_variation")] = l3 / eigenvalue_sum
  *     if out_map.count(b"sphericity"):
  */
   __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_surface_variation) != 0);
   if (__pyx_t_2) {
 
-    /* "jakteristics/extension.pyx":181
+    /* "jakteristics/extension.pyx":195
  *     # Surface variance is how the third component contributes to the sum of the eigenvalues
  *     if out_map.count(b"surface_variation"):
  *         out[out_map.at(b"surface_variation")] = l3 / eigenvalue_sum             # <<<<<<<<<<<<<<
  *     if out_map.count(b"sphericity"):
  *         out[out_map.at(b"sphericity")] = l3 / l1
  */
     try {
-      __pyx_t_12 = __pyx_v_out_map.at(__pyx_k_surface_variation);
+      __pyx_t_16 = __pyx_v_out_map.at(__pyx_k_surface_variation);
     } catch(...) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       __Pyx_CppExn2PyErr();
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 181, __pyx_L1_error)
+      __PYX_ERR(0, 195, __pyx_L1_error)
     }
-    __pyx_t_4 = __pyx_t_12;
+    __pyx_t_4 = __pyx_t_16;
     *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (__pyx_v_l3 / __pyx_v_eigenvalue_sum);
 
-    /* "jakteristics/extension.pyx":180
+    /* "jakteristics/extension.pyx":194
  *         out[out_map.at(b"PCA2")] = l2 / eigenvalue_sum
  *     # Surface variance is how the third component contributes to the sum of the eigenvalues
  *     if out_map.count(b"surface_variation"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"surface_variation")] = l3 / eigenvalue_sum
  *     if out_map.count(b"sphericity"):
  */
   }
 
-  /* "jakteristics/extension.pyx":182
+  /* "jakteristics/extension.pyx":196
  *     if out_map.count(b"surface_variation"):
  *         out[out_map.at(b"surface_variation")] = l3 / eigenvalue_sum
  *     if out_map.count(b"sphericity"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"sphericity")] = l3 / l1
  * 
  */
   __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_sphericity) != 0);
   if (__pyx_t_2) {
 
-    /* "jakteristics/extension.pyx":183
+    /* "jakteristics/extension.pyx":197
  *         out[out_map.at(b"surface_variation")] = l3 / eigenvalue_sum
  *     if out_map.count(b"sphericity"):
  *         out[out_map.at(b"sphericity")] = l3 / l1             # <<<<<<<<<<<<<<
  * 
  *     if out_map.count(b"verticality"):
  */
     try {
-      __pyx_t_13 = __pyx_v_out_map.at(__pyx_k_sphericity);
+      __pyx_t_17 = __pyx_v_out_map.at(__pyx_k_sphericity);
     } catch(...) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       __Pyx_CppExn2PyErr();
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 183, __pyx_L1_error)
+      __PYX_ERR(0, 197, __pyx_L1_error)
     }
-    __pyx_t_4 = __pyx_t_13;
+    __pyx_t_4 = __pyx_t_17;
     *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (__pyx_v_l3 / __pyx_v_l1);
 
-    /* "jakteristics/extension.pyx":182
+    /* "jakteristics/extension.pyx":196
  *     if out_map.count(b"surface_variation"):
  *         out[out_map.at(b"surface_variation")] = l3 / eigenvalue_sum
  *     if out_map.count(b"sphericity"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"sphericity")] = l3 / l1
  * 
  */
   }
 
-  /* "jakteristics/extension.pyx":185
+  /* "jakteristics/extension.pyx":199
  *         out[out_map.at(b"sphericity")] = l3 / l1
  * 
  *     if out_map.count(b"verticality"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"verticality")] = 1.0 - fabs(eigenvectors[2, 2])
  * 
  */
   __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_verticality) != 0);
   if (__pyx_t_2) {
 
-    /* "jakteristics/extension.pyx":186
+    /* "jakteristics/extension.pyx":200
  * 
  *     if out_map.count(b"verticality"):
  *         out[out_map.at(b"verticality")] = 1.0 - fabs(eigenvectors[2, 2])             # <<<<<<<<<<<<<<
  * 
  *     # eigenvectors is col-major
  */
     __pyx_t_1 = 2;
-    __pyx_t_14 = 2;
+    __pyx_t_18 = 2;
     try {
-      __pyx_t_15 = __pyx_v_out_map.at(__pyx_k_verticality);
+      __pyx_t_19 = __pyx_v_out_map.at(__pyx_k_verticality);
     } catch(...) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       __Pyx_CppExn2PyErr();
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 186, __pyx_L1_error)
+      __PYX_ERR(0, 200, __pyx_L1_error)
     }
-    __pyx_t_4 = __pyx_t_15;
-    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (1.0 - fabs((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_1 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_14 * __pyx_v_eigenvectors.strides[1]) )))));
+    __pyx_t_4 = __pyx_t_19;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (1.0 - fabs((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_1 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_18 * __pyx_v_eigenvectors.strides[1]) )))));
 
-    /* "jakteristics/extension.pyx":185
+    /* "jakteristics/extension.pyx":199
  *         out[out_map.at(b"sphericity")] = l3 / l1
  * 
  *     if out_map.count(b"verticality"):             # <<<<<<<<<<<<<<
  *         out[out_map.at(b"verticality")] = 1.0 - fabs(eigenvectors[2, 2])
  * 
  */
   }
 
-  /* "jakteristics/extension.pyx":189
+  /* "jakteristics/extension.pyx":203
  * 
  *     # eigenvectors is col-major
  *     if out_map.count(b"nx") or out_map.count(b"ny") or out_map.count(b"nz"):             # <<<<<<<<<<<<<<
  *         n0 = eigenvectors[0, 1] * eigenvectors[1, 2] - eigenvectors[0, 2] * eigenvectors[1, 1]
  *         n1 = eigenvectors[0, 2] * eigenvectors[1, 0] - eigenvectors[0, 0] * eigenvectors[1, 2]
  */
-  __pyx_t_16 = (__pyx_v_out_map.count(__pyx_k_nx) != 0);
-  if (!__pyx_t_16) {
+  __pyx_t_20 = (__pyx_v_out_map.count(__pyx_k_nx) != 0);
+  if (!__pyx_t_20) {
   } else {
-    __pyx_t_2 = __pyx_t_16;
-    goto __pyx_L15_bool_binop_done;
+    __pyx_t_2 = __pyx_t_20;
+    goto __pyx_L19_bool_binop_done;
   }
-  __pyx_t_16 = (__pyx_v_out_map.count(__pyx_k_ny) != 0);
-  if (!__pyx_t_16) {
+  __pyx_t_20 = (__pyx_v_out_map.count(__pyx_k_ny) != 0);
+  if (!__pyx_t_20) {
   } else {
-    __pyx_t_2 = __pyx_t_16;
-    goto __pyx_L15_bool_binop_done;
+    __pyx_t_2 = __pyx_t_20;
+    goto __pyx_L19_bool_binop_done;
   }
-  __pyx_t_16 = (__pyx_v_out_map.count(__pyx_k_nz) != 0);
-  __pyx_t_2 = __pyx_t_16;
-  __pyx_L15_bool_binop_done:;
+  __pyx_t_20 = (__pyx_v_out_map.count(__pyx_k_nz) != 0);
+  __pyx_t_2 = __pyx_t_20;
+  __pyx_L19_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "jakteristics/extension.pyx":190
+    /* "jakteristics/extension.pyx":204
  *     # eigenvectors is col-major
  *     if out_map.count(b"nx") or out_map.count(b"ny") or out_map.count(b"nz"):
  *         n0 = eigenvectors[0, 1] * eigenvectors[1, 2] - eigenvectors[0, 2] * eigenvectors[1, 1]             # <<<<<<<<<<<<<<
  *         n1 = eigenvectors[0, 2] * eigenvectors[1, 0] - eigenvectors[0, 0] * eigenvectors[1, 2]
  *         n2 = eigenvectors[0, 0] * eigenvectors[1, 1] - eigenvectors[0, 1] * eigenvectors[1, 0]
  */
-    __pyx_t_14 = 0;
+    __pyx_t_18 = 0;
     __pyx_t_1 = 1;
-    __pyx_t_17 = 1;
-    __pyx_t_18 = 2;
-    __pyx_t_19 = 0;
-    __pyx_t_20 = 2;
     __pyx_t_21 = 1;
-    __pyx_t_22 = 1;
-    __pyx_v_n0 = (((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_14 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_1 * __pyx_v_eigenvectors.strides[1]) ))) * (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_17 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_18 * __pyx_v_eigenvectors.strides[1]) )))) - ((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_19 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_20 * __pyx_v_eigenvectors.strides[1]) ))) * (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_21 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_22 * __pyx_v_eigenvectors.strides[1]) )))));
+    __pyx_t_22 = 2;
+    __pyx_t_23 = 0;
+    __pyx_t_24 = 2;
+    __pyx_t_25 = 1;
+    __pyx_t_26 = 1;
+    __pyx_v_n0 = (((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_18 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_1 * __pyx_v_eigenvectors.strides[1]) ))) * (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_21 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_22 * __pyx_v_eigenvectors.strides[1]) )))) - ((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_23 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_24 * __pyx_v_eigenvectors.strides[1]) ))) * (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_25 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_26 * __pyx_v_eigenvectors.strides[1]) )))));
 
-    /* "jakteristics/extension.pyx":191
+    /* "jakteristics/extension.pyx":205
  *     if out_map.count(b"nx") or out_map.count(b"ny") or out_map.count(b"nz"):
  *         n0 = eigenvectors[0, 1] * eigenvectors[1, 2] - eigenvectors[0, 2] * eigenvectors[1, 1]
  *         n1 = eigenvectors[0, 2] * eigenvectors[1, 0] - eigenvectors[0, 0] * eigenvectors[1, 2]             # <<<<<<<<<<<<<<
  *         n2 = eigenvectors[0, 0] * eigenvectors[1, 1] - eigenvectors[0, 1] * eigenvectors[1, 0]
  *         norm = sqrt(n0 * n0 + n1 * n1 + n2 * n2)
  */
+    __pyx_t_26 = 0;
+    __pyx_t_25 = 2;
+    __pyx_t_24 = 1;
+    __pyx_t_23 = 0;
     __pyx_t_22 = 0;
-    __pyx_t_21 = 2;
-    __pyx_t_20 = 1;
-    __pyx_t_19 = 0;
-    __pyx_t_18 = 0;
-    __pyx_t_17 = 0;
+    __pyx_t_21 = 0;
     __pyx_t_1 = 1;
-    __pyx_t_14 = 2;
-    __pyx_v_n1 = (((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_22 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_21 * __pyx_v_eigenvectors.strides[1]) ))) * (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_20 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_19 * __pyx_v_eigenvectors.strides[1]) )))) - ((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_18 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_17 * __pyx_v_eigenvectors.strides[1]) ))) * (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_1 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_14 * __pyx_v_eigenvectors.strides[1]) )))));
+    __pyx_t_18 = 2;
+    __pyx_v_n1 = (((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_26 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_25 * __pyx_v_eigenvectors.strides[1]) ))) * (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_24 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_23 * __pyx_v_eigenvectors.strides[1]) )))) - ((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_22 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_21 * __pyx_v_eigenvectors.strides[1]) ))) * (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_1 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_18 * __pyx_v_eigenvectors.strides[1]) )))));
 
-    /* "jakteristics/extension.pyx":192
+    /* "jakteristics/extension.pyx":206
  *         n0 = eigenvectors[0, 1] * eigenvectors[1, 2] - eigenvectors[0, 2] * eigenvectors[1, 1]
  *         n1 = eigenvectors[0, 2] * eigenvectors[1, 0] - eigenvectors[0, 0] * eigenvectors[1, 2]
  *         n2 = eigenvectors[0, 0] * eigenvectors[1, 1] - eigenvectors[0, 1] * eigenvectors[1, 0]             # <<<<<<<<<<<<<<
  *         norm = sqrt(n0 * n0 + n1 * n1 + n2 * n2)
  *         if out_map.count(b"nx"):
  */
-    __pyx_t_14 = 0;
+    __pyx_t_18 = 0;
     __pyx_t_1 = 0;
-    __pyx_t_17 = 1;
-    __pyx_t_18 = 1;
-    __pyx_t_19 = 0;
-    __pyx_t_20 = 1;
     __pyx_t_21 = 1;
-    __pyx_t_22 = 0;
-    __pyx_v_n2 = (((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_14 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_1 * __pyx_v_eigenvectors.strides[1]) ))) * (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_17 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_18 * __pyx_v_eigenvectors.strides[1]) )))) - ((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_19 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_20 * __pyx_v_eigenvectors.strides[1]) ))) * (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_21 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_22 * __pyx_v_eigenvectors.strides[1]) )))));
+    __pyx_t_22 = 1;
+    __pyx_t_23 = 0;
+    __pyx_t_24 = 1;
+    __pyx_t_25 = 1;
+    __pyx_t_26 = 0;
+    __pyx_v_n2 = (((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_18 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_1 * __pyx_v_eigenvectors.strides[1]) ))) * (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_21 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_22 * __pyx_v_eigenvectors.strides[1]) )))) - ((*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_23 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_24 * __pyx_v_eigenvectors.strides[1]) ))) * (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_25 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_26 * __pyx_v_eigenvectors.strides[1]) )))));
 
-    /* "jakteristics/extension.pyx":193
+    /* "jakteristics/extension.pyx":207
  *         n1 = eigenvectors[0, 2] * eigenvectors[1, 0] - eigenvectors[0, 0] * eigenvectors[1, 2]
  *         n2 = eigenvectors[0, 0] * eigenvectors[1, 1] - eigenvectors[0, 1] * eigenvectors[1, 0]
  *         norm = sqrt(n0 * n0 + n1 * n1 + n2 * n2)             # <<<<<<<<<<<<<<
  *         if out_map.count(b"nx"):
  *             out[out_map.at(b"nx")] = n0 / norm
  */
     __pyx_v_norm = sqrt((((__pyx_v_n0 * __pyx_v_n0) + (__pyx_v_n1 * __pyx_v_n1)) + (__pyx_v_n2 * __pyx_v_n2)));
 
-    /* "jakteristics/extension.pyx":194
+    /* "jakteristics/extension.pyx":208
  *         n2 = eigenvectors[0, 0] * eigenvectors[1, 1] - eigenvectors[0, 1] * eigenvectors[1, 0]
  *         norm = sqrt(n0 * n0 + n1 * n1 + n2 * n2)
  *         if out_map.count(b"nx"):             # <<<<<<<<<<<<<<
  *             out[out_map.at(b"nx")] = n0 / norm
  *         if out_map.count(b"ny"):
  */
     __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_nx) != 0);
     if (__pyx_t_2) {
 
-      /* "jakteristics/extension.pyx":195
+      /* "jakteristics/extension.pyx":209
  *         norm = sqrt(n0 * n0 + n1 * n1 + n2 * n2)
  *         if out_map.count(b"nx"):
  *             out[out_map.at(b"nx")] = n0 / norm             # <<<<<<<<<<<<<<
  *         if out_map.count(b"ny"):
  *             out[out_map.at(b"ny")] = n1 / norm
  */
       try {
-        __pyx_t_23 = __pyx_v_out_map.at(__pyx_k_nx);
+        __pyx_t_27 = __pyx_v_out_map.at(__pyx_k_nx);
       } catch(...) {
         #ifdef WITH_THREAD
         PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
         #endif
         __Pyx_CppExn2PyErr();
         #ifdef WITH_THREAD
         __Pyx_PyGILState_Release(__pyx_gilstate_save);
         #endif
-        __PYX_ERR(0, 195, __pyx_L1_error)
+        __PYX_ERR(0, 209, __pyx_L1_error)
       }
-      __pyx_t_4 = __pyx_t_23;
+      __pyx_t_4 = __pyx_t_27;
       *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (__pyx_v_n0 / __pyx_v_norm);
 
-      /* "jakteristics/extension.pyx":194
+      /* "jakteristics/extension.pyx":208
  *         n2 = eigenvectors[0, 0] * eigenvectors[1, 1] - eigenvectors[0, 1] * eigenvectors[1, 0]
  *         norm = sqrt(n0 * n0 + n1 * n1 + n2 * n2)
  *         if out_map.count(b"nx"):             # <<<<<<<<<<<<<<
  *             out[out_map.at(b"nx")] = n0 / norm
  *         if out_map.count(b"ny"):
  */
     }
 
-    /* "jakteristics/extension.pyx":196
+    /* "jakteristics/extension.pyx":210
  *         if out_map.count(b"nx"):
  *             out[out_map.at(b"nx")] = n0 / norm
  *         if out_map.count(b"ny"):             # <<<<<<<<<<<<<<
  *             out[out_map.at(b"ny")] = n1 / norm
  *         if out_map.count(b"nz"):
  */
     __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_ny) != 0);
     if (__pyx_t_2) {
 
-      /* "jakteristics/extension.pyx":197
+      /* "jakteristics/extension.pyx":211
  *             out[out_map.at(b"nx")] = n0 / norm
  *         if out_map.count(b"ny"):
  *             out[out_map.at(b"ny")] = n1 / norm             # <<<<<<<<<<<<<<
  *         if out_map.count(b"nz"):
  *             out[out_map.at(b"nz")] = n2 / norm
  */
       try {
-        __pyx_t_24 = __pyx_v_out_map.at(__pyx_k_ny);
+        __pyx_t_28 = __pyx_v_out_map.at(__pyx_k_ny);
       } catch(...) {
         #ifdef WITH_THREAD
         PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
         #endif
         __Pyx_CppExn2PyErr();
         #ifdef WITH_THREAD
         __Pyx_PyGILState_Release(__pyx_gilstate_save);
         #endif
-        __PYX_ERR(0, 197, __pyx_L1_error)
+        __PYX_ERR(0, 211, __pyx_L1_error)
       }
-      __pyx_t_4 = __pyx_t_24;
+      __pyx_t_4 = __pyx_t_28;
       *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (__pyx_v_n1 / __pyx_v_norm);
 
-      /* "jakteristics/extension.pyx":196
+      /* "jakteristics/extension.pyx":210
  *         if out_map.count(b"nx"):
  *             out[out_map.at(b"nx")] = n0 / norm
  *         if out_map.count(b"ny"):             # <<<<<<<<<<<<<<
  *             out[out_map.at(b"ny")] = n1 / norm
  *         if out_map.count(b"nz"):
  */
     }
 
-    /* "jakteristics/extension.pyx":198
+    /* "jakteristics/extension.pyx":212
  *         if out_map.count(b"ny"):
  *             out[out_map.at(b"ny")] = n1 / norm
  *         if out_map.count(b"nz"):             # <<<<<<<<<<<<<<
  *             out[out_map.at(b"nz")] = n2 / norm
  * 
  */
     __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_nz) != 0);
     if (__pyx_t_2) {
 
-      /* "jakteristics/extension.pyx":199
+      /* "jakteristics/extension.pyx":213
  *             out[out_map.at(b"ny")] = n1 / norm
  *         if out_map.count(b"nz"):
  *             out[out_map.at(b"nz")] = n2 / norm             # <<<<<<<<<<<<<<
  * 
- * 
+ *     if out_map.count(b"eigenvector1x"):
  */
       try {
-        __pyx_t_25 = __pyx_v_out_map.at(__pyx_k_nz);
+        __pyx_t_29 = __pyx_v_out_map.at(__pyx_k_nz);
       } catch(...) {
         #ifdef WITH_THREAD
         PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
         #endif
         __Pyx_CppExn2PyErr();
         #ifdef WITH_THREAD
         __Pyx_PyGILState_Release(__pyx_gilstate_save);
         #endif
-        __PYX_ERR(0, 199, __pyx_L1_error)
+        __PYX_ERR(0, 213, __pyx_L1_error)
       }
-      __pyx_t_4 = __pyx_t_25;
+      __pyx_t_4 = __pyx_t_29;
       *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (__pyx_v_n2 / __pyx_v_norm);
 
-      /* "jakteristics/extension.pyx":198
+      /* "jakteristics/extension.pyx":212
  *         if out_map.count(b"ny"):
  *             out[out_map.at(b"ny")] = n1 / norm
  *         if out_map.count(b"nz"):             # <<<<<<<<<<<<<<
  *             out[out_map.at(b"nz")] = n2 / norm
  * 
  */
     }
 
-    /* "jakteristics/extension.pyx":189
+    /* "jakteristics/extension.pyx":203
  * 
  *     # eigenvectors is col-major
  *     if out_map.count(b"nx") or out_map.count(b"ny") or out_map.count(b"nz"):             # <<<<<<<<<<<<<<
  *         n0 = eigenvectors[0, 1] * eigenvectors[1, 2] - eigenvectors[0, 2] * eigenvectors[1, 1]
  *         n1 = eigenvectors[0, 2] * eigenvectors[1, 0] - eigenvectors[0, 0] * eigenvectors[1, 2]
  */
   }
 
-  /* "jakteristics/extension.pyx":134
+  /* "jakteristics/extension.pyx":215
+ *             out[out_map.at(b"nz")] = n2 / norm
+ * 
+ *     if out_map.count(b"eigenvector1x"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector1x")] = eigenvectors[0, 0]
+ *     if out_map.count(b"eigenvector1y"):
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvector1x) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":216
+ * 
+ *     if out_map.count(b"eigenvector1x"):
+ *         out[out_map.at(b"eigenvector1x")] = eigenvectors[0, 0]             # <<<<<<<<<<<<<<
+ *     if out_map.count(b"eigenvector1y"):
+ *         out[out_map.at(b"eigenvector1y")] = eigenvectors[0, 1]
+ */
+    __pyx_t_26 = 0;
+    __pyx_t_25 = 0;
+    try {
+      __pyx_t_30 = __pyx_v_out_map.at(__pyx_k_eigenvector1x);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 216, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_30;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_26 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_25 * __pyx_v_eigenvectors.strides[1]) )));
+
+    /* "jakteristics/extension.pyx":215
+ *             out[out_map.at(b"nz")] = n2 / norm
+ * 
+ *     if out_map.count(b"eigenvector1x"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector1x")] = eigenvectors[0, 0]
+ *     if out_map.count(b"eigenvector1y"):
+ */
+  }
+
+  /* "jakteristics/extension.pyx":217
+ *     if out_map.count(b"eigenvector1x"):
+ *         out[out_map.at(b"eigenvector1x")] = eigenvectors[0, 0]
+ *     if out_map.count(b"eigenvector1y"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector1y")] = eigenvectors[0, 1]
+ *     if out_map.count(b"eigenvector1z"):
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvector1y) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":218
+ *         out[out_map.at(b"eigenvector1x")] = eigenvectors[0, 0]
+ *     if out_map.count(b"eigenvector1y"):
+ *         out[out_map.at(b"eigenvector1y")] = eigenvectors[0, 1]             # <<<<<<<<<<<<<<
+ *     if out_map.count(b"eigenvector1z"):
+ *         out[out_map.at(b"eigenvector1z")] = eigenvectors[0, 2]
+ */
+    __pyx_t_25 = 0;
+    __pyx_t_26 = 1;
+    try {
+      __pyx_t_31 = __pyx_v_out_map.at(__pyx_k_eigenvector1y);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 218, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_31;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_25 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_26 * __pyx_v_eigenvectors.strides[1]) )));
+
+    /* "jakteristics/extension.pyx":217
+ *     if out_map.count(b"eigenvector1x"):
+ *         out[out_map.at(b"eigenvector1x")] = eigenvectors[0, 0]
+ *     if out_map.count(b"eigenvector1y"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector1y")] = eigenvectors[0, 1]
+ *     if out_map.count(b"eigenvector1z"):
+ */
+  }
+
+  /* "jakteristics/extension.pyx":219
+ *     if out_map.count(b"eigenvector1y"):
+ *         out[out_map.at(b"eigenvector1y")] = eigenvectors[0, 1]
+ *     if out_map.count(b"eigenvector1z"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector1z")] = eigenvectors[0, 2]
+ * 
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvector1z) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":220
+ *         out[out_map.at(b"eigenvector1y")] = eigenvectors[0, 1]
+ *     if out_map.count(b"eigenvector1z"):
+ *         out[out_map.at(b"eigenvector1z")] = eigenvectors[0, 2]             # <<<<<<<<<<<<<<
+ * 
+ *     if out_map.count(b"eigenvector2x"):
+ */
+    __pyx_t_26 = 0;
+    __pyx_t_25 = 2;
+    try {
+      __pyx_t_32 = __pyx_v_out_map.at(__pyx_k_eigenvector1z);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 220, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_32;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_26 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_25 * __pyx_v_eigenvectors.strides[1]) )));
+
+    /* "jakteristics/extension.pyx":219
+ *     if out_map.count(b"eigenvector1y"):
+ *         out[out_map.at(b"eigenvector1y")] = eigenvectors[0, 1]
+ *     if out_map.count(b"eigenvector1z"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector1z")] = eigenvectors[0, 2]
+ * 
+ */
+  }
+
+  /* "jakteristics/extension.pyx":222
+ *         out[out_map.at(b"eigenvector1z")] = eigenvectors[0, 2]
+ * 
+ *     if out_map.count(b"eigenvector2x"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector2x")] = eigenvectors[1, 0]
+ *     if out_map.count(b"eigenvector2y"):
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvector2x) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":223
+ * 
+ *     if out_map.count(b"eigenvector2x"):
+ *         out[out_map.at(b"eigenvector2x")] = eigenvectors[1, 0]             # <<<<<<<<<<<<<<
+ *     if out_map.count(b"eigenvector2y"):
+ *         out[out_map.at(b"eigenvector2y")] = eigenvectors[1, 1]
+ */
+    __pyx_t_25 = 1;
+    __pyx_t_26 = 0;
+    try {
+      __pyx_t_33 = __pyx_v_out_map.at(__pyx_k_eigenvector2x);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 223, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_33;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_25 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_26 * __pyx_v_eigenvectors.strides[1]) )));
+
+    /* "jakteristics/extension.pyx":222
+ *         out[out_map.at(b"eigenvector1z")] = eigenvectors[0, 2]
+ * 
+ *     if out_map.count(b"eigenvector2x"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector2x")] = eigenvectors[1, 0]
+ *     if out_map.count(b"eigenvector2y"):
+ */
+  }
+
+  /* "jakteristics/extension.pyx":224
+ *     if out_map.count(b"eigenvector2x"):
+ *         out[out_map.at(b"eigenvector2x")] = eigenvectors[1, 0]
+ *     if out_map.count(b"eigenvector2y"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector2y")] = eigenvectors[1, 1]
+ *     if out_map.count(b"eigenvector2z"):
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvector2y) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":225
+ *         out[out_map.at(b"eigenvector2x")] = eigenvectors[1, 0]
+ *     if out_map.count(b"eigenvector2y"):
+ *         out[out_map.at(b"eigenvector2y")] = eigenvectors[1, 1]             # <<<<<<<<<<<<<<
+ *     if out_map.count(b"eigenvector2z"):
+ *         out[out_map.at(b"eigenvector2z")] = eigenvectors[1, 2]
+ */
+    __pyx_t_26 = 1;
+    __pyx_t_25 = 1;
+    try {
+      __pyx_t_34 = __pyx_v_out_map.at(__pyx_k_eigenvector2y);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 225, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_34;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_26 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_25 * __pyx_v_eigenvectors.strides[1]) )));
+
+    /* "jakteristics/extension.pyx":224
+ *     if out_map.count(b"eigenvector2x"):
+ *         out[out_map.at(b"eigenvector2x")] = eigenvectors[1, 0]
+ *     if out_map.count(b"eigenvector2y"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector2y")] = eigenvectors[1, 1]
+ *     if out_map.count(b"eigenvector2z"):
+ */
+  }
+
+  /* "jakteristics/extension.pyx":226
+ *     if out_map.count(b"eigenvector2y"):
+ *         out[out_map.at(b"eigenvector2y")] = eigenvectors[1, 1]
+ *     if out_map.count(b"eigenvector2z"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector2z")] = eigenvectors[1, 2]
+ * 
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvector2z) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":227
+ *         out[out_map.at(b"eigenvector2y")] = eigenvectors[1, 1]
+ *     if out_map.count(b"eigenvector2z"):
+ *         out[out_map.at(b"eigenvector2z")] = eigenvectors[1, 2]             # <<<<<<<<<<<<<<
+ * 
+ *     if out_map.count(b"eigenvector3x"):
+ */
+    __pyx_t_25 = 1;
+    __pyx_t_26 = 2;
+    try {
+      __pyx_t_35 = __pyx_v_out_map.at(__pyx_k_eigenvector2z);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 227, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_35;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_25 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_26 * __pyx_v_eigenvectors.strides[1]) )));
+
+    /* "jakteristics/extension.pyx":226
+ *     if out_map.count(b"eigenvector2y"):
+ *         out[out_map.at(b"eigenvector2y")] = eigenvectors[1, 1]
+ *     if out_map.count(b"eigenvector2z"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector2z")] = eigenvectors[1, 2]
+ * 
+ */
+  }
+
+  /* "jakteristics/extension.pyx":229
+ *         out[out_map.at(b"eigenvector2z")] = eigenvectors[1, 2]
+ * 
+ *     if out_map.count(b"eigenvector3x"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector3x")] = eigenvectors[2, 0]
+ *     if out_map.count(b"eigenvector3y"):
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvector3x) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":230
+ * 
+ *     if out_map.count(b"eigenvector3x"):
+ *         out[out_map.at(b"eigenvector3x")] = eigenvectors[2, 0]             # <<<<<<<<<<<<<<
+ *     if out_map.count(b"eigenvector3y"):
+ *         out[out_map.at(b"eigenvector3y")] = eigenvectors[2, 1]
+ */
+    __pyx_t_26 = 2;
+    __pyx_t_25 = 0;
+    try {
+      __pyx_t_36 = __pyx_v_out_map.at(__pyx_k_eigenvector3x);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 230, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_36;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_26 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_25 * __pyx_v_eigenvectors.strides[1]) )));
+
+    /* "jakteristics/extension.pyx":229
+ *         out[out_map.at(b"eigenvector2z")] = eigenvectors[1, 2]
+ * 
+ *     if out_map.count(b"eigenvector3x"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector3x")] = eigenvectors[2, 0]
+ *     if out_map.count(b"eigenvector3y"):
+ */
+  }
+
+  /* "jakteristics/extension.pyx":231
+ *     if out_map.count(b"eigenvector3x"):
+ *         out[out_map.at(b"eigenvector3x")] = eigenvectors[2, 0]
+ *     if out_map.count(b"eigenvector3y"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector3y")] = eigenvectors[2, 1]
+ *     if out_map.count(b"eigenvector3z"):
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvector3y) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":232
+ *         out[out_map.at(b"eigenvector3x")] = eigenvectors[2, 0]
+ *     if out_map.count(b"eigenvector3y"):
+ *         out[out_map.at(b"eigenvector3y")] = eigenvectors[2, 1]             # <<<<<<<<<<<<<<
+ *     if out_map.count(b"eigenvector3z"):
+ *         out[out_map.at(b"eigenvector3z")] = eigenvectors[2, 2]
+ */
+    __pyx_t_25 = 2;
+    __pyx_t_26 = 1;
+    try {
+      __pyx_t_37 = __pyx_v_out_map.at(__pyx_k_eigenvector3y);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 232, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_37;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_25 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_26 * __pyx_v_eigenvectors.strides[1]) )));
+
+    /* "jakteristics/extension.pyx":231
+ *     if out_map.count(b"eigenvector3x"):
+ *         out[out_map.at(b"eigenvector3x")] = eigenvectors[2, 0]
+ *     if out_map.count(b"eigenvector3y"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector3y")] = eigenvectors[2, 1]
+ *     if out_map.count(b"eigenvector3z"):
+ */
+  }
+
+  /* "jakteristics/extension.pyx":233
+ *     if out_map.count(b"eigenvector3y"):
+ *         out[out_map.at(b"eigenvector3y")] = eigenvectors[2, 1]
+ *     if out_map.count(b"eigenvector3z"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector3z")] = eigenvectors[2, 2]
+ * 
+ */
+  __pyx_t_2 = (__pyx_v_out_map.count(__pyx_k_eigenvector3z) != 0);
+  if (__pyx_t_2) {
+
+    /* "jakteristics/extension.pyx":234
+ *         out[out_map.at(b"eigenvector3y")] = eigenvectors[2, 1]
+ *     if out_map.count(b"eigenvector3z"):
+ *         out[out_map.at(b"eigenvector3z")] = eigenvectors[2, 2]             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+    __pyx_t_26 = 2;
+    __pyx_t_25 = 2;
+    try {
+      __pyx_t_38 = __pyx_v_out_map.at(__pyx_k_eigenvector3z);
+    } catch(...) {
+      #ifdef WITH_THREAD
+      PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      __Pyx_CppExn2PyErr();
+      #ifdef WITH_THREAD
+      __Pyx_PyGILState_Release(__pyx_gilstate_save);
+      #endif
+      __PYX_ERR(0, 234, __pyx_L1_error)
+    }
+    __pyx_t_4 = __pyx_t_38;
+    *((float *) ( /* dim=0 */ (__pyx_v_out.data + __pyx_t_4 * __pyx_v_out.strides[0]) )) = (*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_eigenvectors.data + __pyx_t_26 * __pyx_v_eigenvectors.strides[0]) ) + __pyx_t_25 * __pyx_v_eigenvectors.strides[1]) )));
+
+    /* "jakteristics/extension.pyx":233
+ *     if out_map.count(b"eigenvector3y"):
+ *         out[out_map.at(b"eigenvector3y")] = eigenvectors[2, 1]
+ *     if out_map.count(b"eigenvector3z"):             # <<<<<<<<<<<<<<
+ *         out[out_map.at(b"eigenvector3z")] = eigenvectors[2, 2]
+ * 
+ */
+  }
+
+  /* "jakteristics/extension.pyx":137
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * cdef inline void compute_features_from_eigenvectors(             # <<<<<<<<<<<<<<
+ *     int number_of_neighbors,
  *     double [:] eigenvalues,
- *     double [:, :] eigenvectors,
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("jakteristics.extension.compute_features_from_eigenvectors", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_L0:;
 }
 
-/* "jakteristics/extension.pyx":202
+/* "jakteristics/extension.pyx":237
  * 
  * 
  * cdef vector[np.intp_t] *** init_result_vectors(int num_threads):             # <<<<<<<<<<<<<<
  *     """Allocate memory for result vectors, based on thread count"""
  *     threaded_vvres = <vector[np.intp_t] ***> PyMem_Malloc(num_threads * sizeof(void*))
  */
 
@@ -5277,145 +5869,145 @@
   int __pyx_t_4;
   std::vector<__pyx_t_5numpy_intp_t>  *__pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("init_result_vectors", 0);
 
-  /* "jakteristics/extension.pyx":204
+  /* "jakteristics/extension.pyx":239
  * cdef vector[np.intp_t] *** init_result_vectors(int num_threads):
  *     """Allocate memory for result vectors, based on thread count"""
  *     threaded_vvres = <vector[np.intp_t] ***> PyMem_Malloc(num_threads * sizeof(void*))             # <<<<<<<<<<<<<<
  *     if not threaded_vvres:
  *         raise MemoryError()
  */
   __pyx_v_threaded_vvres = ((std::vector<__pyx_t_5numpy_intp_t>  ***)PyMem_Malloc((__pyx_v_num_threads * (sizeof(void *)))));
 
-  /* "jakteristics/extension.pyx":205
+  /* "jakteristics/extension.pyx":240
  *     """Allocate memory for result vectors, based on thread count"""
  *     threaded_vvres = <vector[np.intp_t] ***> PyMem_Malloc(num_threads * sizeof(void*))
  *     if not threaded_vvres:             # <<<<<<<<<<<<<<
  *         raise MemoryError()
  *     memset(<void*> threaded_vvres, 0, num_threads * sizeof(void*))
  */
   __pyx_t_1 = ((!(__pyx_v_threaded_vvres != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "jakteristics/extension.pyx":206
+    /* "jakteristics/extension.pyx":241
  *     threaded_vvres = <vector[np.intp_t] ***> PyMem_Malloc(num_threads * sizeof(void*))
  *     if not threaded_vvres:
  *         raise MemoryError()             # <<<<<<<<<<<<<<
  *     memset(<void*> threaded_vvres, 0, num_threads * sizeof(void*))
  *     for i in range(num_threads):
  */
-    PyErr_NoMemory(); __PYX_ERR(0, 206, __pyx_L1_error)
+    PyErr_NoMemory(); __PYX_ERR(0, 241, __pyx_L1_error)
 
-    /* "jakteristics/extension.pyx":205
+    /* "jakteristics/extension.pyx":240
  *     """Allocate memory for result vectors, based on thread count"""
  *     threaded_vvres = <vector[np.intp_t] ***> PyMem_Malloc(num_threads * sizeof(void*))
  *     if not threaded_vvres:             # <<<<<<<<<<<<<<
  *         raise MemoryError()
  *     memset(<void*> threaded_vvres, 0, num_threads * sizeof(void*))
  */
   }
 
-  /* "jakteristics/extension.pyx":207
+  /* "jakteristics/extension.pyx":242
  *     if not threaded_vvres:
  *         raise MemoryError()
  *     memset(<void*> threaded_vvres, 0, num_threads * sizeof(void*))             # <<<<<<<<<<<<<<
  *     for i in range(num_threads):
  *         threaded_vvres[i] = <vector[np.intp_t] **> PyMem_Malloc(sizeof(void*))
  */
   (void)(memset(((void *)__pyx_v_threaded_vvres), 0, (__pyx_v_num_threads * (sizeof(void *)))));
 
-  /* "jakteristics/extension.pyx":208
+  /* "jakteristics/extension.pyx":243
  *         raise MemoryError()
  *     memset(<void*> threaded_vvres, 0, num_threads * sizeof(void*))
  *     for i in range(num_threads):             # <<<<<<<<<<<<<<
  *         threaded_vvres[i] = <vector[np.intp_t] **> PyMem_Malloc(sizeof(void*))
  *         if not threaded_vvres[i]:
  */
   __pyx_t_2 = __pyx_v_num_threads;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "jakteristics/extension.pyx":209
+    /* "jakteristics/extension.pyx":244
  *     memset(<void*> threaded_vvres, 0, num_threads * sizeof(void*))
  *     for i in range(num_threads):
  *         threaded_vvres[i] = <vector[np.intp_t] **> PyMem_Malloc(sizeof(void*))             # <<<<<<<<<<<<<<
  *         if not threaded_vvres[i]:
  *             raise MemoryError()
  */
     (__pyx_v_threaded_vvres[__pyx_v_i]) = ((std::vector<__pyx_t_5numpy_intp_t>  **)PyMem_Malloc((sizeof(void *))));
 
-    /* "jakteristics/extension.pyx":210
+    /* "jakteristics/extension.pyx":245
  *     for i in range(num_threads):
  *         threaded_vvres[i] = <vector[np.intp_t] **> PyMem_Malloc(sizeof(void*))
  *         if not threaded_vvres[i]:             # <<<<<<<<<<<<<<
  *             raise MemoryError()
  *         memset(<void*> threaded_vvres[i], 0, sizeof(void*))
  */
     __pyx_t_1 = ((!((__pyx_v_threaded_vvres[__pyx_v_i]) != 0)) != 0);
     if (unlikely(__pyx_t_1)) {
 
-      /* "jakteristics/extension.pyx":211
+      /* "jakteristics/extension.pyx":246
  *         threaded_vvres[i] = <vector[np.intp_t] **> PyMem_Malloc(sizeof(void*))
  *         if not threaded_vvres[i]:
  *             raise MemoryError()             # <<<<<<<<<<<<<<
  *         memset(<void*> threaded_vvres[i], 0, sizeof(void*))
  *         threaded_vvres[i][0] = new vector[np.intp_t]()
  */
-      PyErr_NoMemory(); __PYX_ERR(0, 211, __pyx_L1_error)
+      PyErr_NoMemory(); __PYX_ERR(0, 246, __pyx_L1_error)
 
-      /* "jakteristics/extension.pyx":210
+      /* "jakteristics/extension.pyx":245
  *     for i in range(num_threads):
  *         threaded_vvres[i] = <vector[np.intp_t] **> PyMem_Malloc(sizeof(void*))
  *         if not threaded_vvres[i]:             # <<<<<<<<<<<<<<
  *             raise MemoryError()
  *         memset(<void*> threaded_vvres[i], 0, sizeof(void*))
  */
     }
 
-    /* "jakteristics/extension.pyx":212
+    /* "jakteristics/extension.pyx":247
  *         if not threaded_vvres[i]:
  *             raise MemoryError()
  *         memset(<void*> threaded_vvres[i], 0, sizeof(void*))             # <<<<<<<<<<<<<<
  *         threaded_vvres[i][0] = new vector[np.intp_t]()
  *     return threaded_vvres
  */
     (void)(memset(((void *)(__pyx_v_threaded_vvres[__pyx_v_i])), 0, (sizeof(void *))));
 
-    /* "jakteristics/extension.pyx":213
+    /* "jakteristics/extension.pyx":248
  *             raise MemoryError()
  *         memset(<void*> threaded_vvres[i], 0, sizeof(void*))
  *         threaded_vvres[i][0] = new vector[np.intp_t]()             # <<<<<<<<<<<<<<
  *     return threaded_vvres
  * 
  */
     try {
       __pyx_t_5 = new std::vector<__pyx_t_5numpy_intp_t> ();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 213, __pyx_L1_error)
+      __PYX_ERR(0, 248, __pyx_L1_error)
     }
     ((__pyx_v_threaded_vvres[__pyx_v_i])[0]) = __pyx_t_5;
   }
 
-  /* "jakteristics/extension.pyx":214
+  /* "jakteristics/extension.pyx":249
  *         memset(<void*> threaded_vvres[i], 0, sizeof(void*))
  *         threaded_vvres[i][0] = new vector[np.intp_t]()
  *     return threaded_vvres             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_threaded_vvres;
   goto __pyx_L0;
 
-  /* "jakteristics/extension.pyx":202
+  /* "jakteristics/extension.pyx":237
  * 
  * 
  * cdef vector[np.intp_t] *** init_result_vectors(int num_threads):             # <<<<<<<<<<<<<<
  *     """Allocate memory for result vectors, based on thread count"""
  *     threaded_vvres = <vector[np.intp_t] ***> PyMem_Malloc(num_threads * sizeof(void*))
  */
 
@@ -5424,15 +6016,15 @@
   __Pyx_WriteUnraisable("jakteristics.extension.init_result_vectors", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jakteristics/extension.pyx":217
+/* "jakteristics/extension.pyx":252
  * 
  * 
  * cdef void free_result_vectors(vector[np.intp_t] *** threaded_vvres, int num_threads):             # <<<<<<<<<<<<<<
  *     """Free memory for result vectors"""
  *     if threaded_vvres != NULL:
  */
 
@@ -5441,102 +6033,104 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   __Pyx_RefNannySetupContext("free_result_vectors", 0);
 
-  /* "jakteristics/extension.pyx":219
+  /* "jakteristics/extension.pyx":254
  * cdef void free_result_vectors(vector[np.intp_t] *** threaded_vvres, int num_threads):
  *     """Free memory for result vectors"""
  *     if threaded_vvres != NULL:             # <<<<<<<<<<<<<<
  *         for i in range(num_threads):
  *             if threaded_vvres[i] != NULL:
  */
   __pyx_t_1 = ((__pyx_v_threaded_vvres != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "jakteristics/extension.pyx":220
+    /* "jakteristics/extension.pyx":255
  *     """Free memory for result vectors"""
  *     if threaded_vvres != NULL:
  *         for i in range(num_threads):             # <<<<<<<<<<<<<<
  *             if threaded_vvres[i] != NULL:
  *                 del threaded_vvres[i][0]
  */
     __pyx_t_2 = __pyx_v_num_threads;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "jakteristics/extension.pyx":221
+      /* "jakteristics/extension.pyx":256
  *     if threaded_vvres != NULL:
  *         for i in range(num_threads):
  *             if threaded_vvres[i] != NULL:             # <<<<<<<<<<<<<<
  *                 del threaded_vvres[i][0]
  *             PyMem_Free(threaded_vvres[i])
  */
       __pyx_t_1 = (((__pyx_v_threaded_vvres[__pyx_v_i]) != NULL) != 0);
       if (__pyx_t_1) {
 
-        /* "jakteristics/extension.pyx":222
+        /* "jakteristics/extension.pyx":257
  *         for i in range(num_threads):
  *             if threaded_vvres[i] != NULL:
  *                 del threaded_vvres[i][0]             # <<<<<<<<<<<<<<
  *             PyMem_Free(threaded_vvres[i])
  *         PyMem_Free(threaded_vvres)
  */
         delete ((__pyx_v_threaded_vvres[__pyx_v_i])[0]);
 
-        /* "jakteristics/extension.pyx":221
+        /* "jakteristics/extension.pyx":256
  *     if threaded_vvres != NULL:
  *         for i in range(num_threads):
  *             if threaded_vvres[i] != NULL:             # <<<<<<<<<<<<<<
  *                 del threaded_vvres[i][0]
  *             PyMem_Free(threaded_vvres[i])
  */
       }
 
-      /* "jakteristics/extension.pyx":223
+      /* "jakteristics/extension.pyx":258
  *             if threaded_vvres[i] != NULL:
  *                 del threaded_vvres[i][0]
  *             PyMem_Free(threaded_vvres[i])             # <<<<<<<<<<<<<<
  *         PyMem_Free(threaded_vvres)
+ * 
  */
       PyMem_Free((__pyx_v_threaded_vvres[__pyx_v_i]));
     }
 
-    /* "jakteristics/extension.pyx":224
+    /* "jakteristics/extension.pyx":259
  *                 del threaded_vvres[i][0]
  *             PyMem_Free(threaded_vvres[i])
  *         PyMem_Free(threaded_vvres)             # <<<<<<<<<<<<<<
+ * 
  */
     PyMem_Free(__pyx_v_threaded_vvres);
 
-    /* "jakteristics/extension.pyx":219
+    /* "jakteristics/extension.pyx":254
  * cdef void free_result_vectors(vector[np.intp_t] *** threaded_vvres, int num_threads):
  *     """Free memory for result vectors"""
  *     if threaded_vvres != NULL:             # <<<<<<<<<<<<<<
  *         for i in range(num_threads):
  *             if threaded_vvres[i] != NULL:
  */
   }
 
-  /* "jakteristics/extension.pyx":217
+  /* "jakteristics/extension.pyx":252
  * 
  * 
  * cdef void free_result_vectors(vector[np.intp_t] *** threaded_vvres, int num_threads):             # <<<<<<<<<<<<<<
  *     """Free memory for result vectors"""
  *     if threaded_vvres != NULL:
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5545,29 +6139,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5578,15 +6172,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5595,29 +6189,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5628,15 +6222,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5645,29 +6239,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5678,15 +6272,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5695,29 +6289,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5728,15 +6322,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5745,29 +6339,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5778,212 +6372,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5999,15 +6593,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6015,53 +6609,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -6069,30 +6663,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6107,15 +6701,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6131,15 +6725,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6147,53 +6741,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -6201,30 +6795,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6239,15 +6833,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6263,15 +6857,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6279,53 +6873,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -6333,30 +6927,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6371,176 +6965,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -20516,14 +21110,15 @@
   {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
   {&__pyx_n_s_neighbor_id, __pyx_k_neighbor_id, sizeof(__pyx_k_neighbor_id), 0, 0, 1, 1},
   {&__pyx_n_s_neighbor_points, __pyx_k_neighbor_points, sizeof(__pyx_k_neighbor_points), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_num_threads, __pyx_k_num_threads, sizeof(__pyx_k_num_threads), 0, 0, 1, 1},
+  {&__pyx_n_s_number_of_neighbors, __pyx_k_number_of_neighbors, sizeof(__pyx_k_number_of_neighbors), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_s_order, __pyx_k_order, sizeof(__pyx_k_order), 0, 0, 1, 1},
   {&__pyx_n_s_p, __pyx_k_p, sizeof(__pyx_k_p), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
@@ -20563,55 +21158,55 @@
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 62, __pyx_L1_error)
-  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 70, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 105, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 241, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "jakteristics/extension.pyx":62
+  /* "jakteristics/extension.pyx":63
  * 
  *     if not points.shape[1] == 3:
  *         raise ValueError("You must provide an (n x 3) numpy array.")             # <<<<<<<<<<<<<<
  * 
  *     if num_threads == -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_You_must_provide_an_n_x_3_numpy); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_You_must_provide_an_n_x_3_numpy); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -20816,18 +21411,18 @@
   /* "jakteristics/extension.pyx":29
  * @cython.initializedcheck(False)
  * @cython.cdivision(True)
  * def compute_features(             # <<<<<<<<<<<<<<
  *     double [:, ::1] points,
  *     float search_radius,
  */
-  __pyx_tuple__24 = PyTuple_Pack(27, __pyx_n_s_points, __pyx_n_s_search_radius, __pyx_n_s_kdtree, __pyx_n_s_num_threads, __pyx_n_s_max_k_neighbors, __pyx_n_s_euclidean_distance, __pyx_n_s_feature_names, __pyx_n_s_eps, __pyx_n_s_features_map, __pyx_n_s_n_points, __pyx_n_s_neighbor_points, __pyx_n_s_eigenvectors, __pyx_n_s_eigenvalues, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_neighbor_id, __pyx_n_s_n_neighbors_at_id, __pyx_n_s_thread_id, __pyx_n_s_features, __pyx_n_s_radius_vector, __pyx_n_s_p, __pyx_n_s_eps_scipy, __pyx_n_s_threaded_vvres, __pyx_n_s_return_length, __pyx_n_s_n, __pyx_n_s_name); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(28, __pyx_n_s_points, __pyx_n_s_search_radius, __pyx_n_s_kdtree, __pyx_n_s_num_threads, __pyx_n_s_max_k_neighbors, __pyx_n_s_euclidean_distance, __pyx_n_s_feature_names, __pyx_n_s_eps, __pyx_n_s_features_map, __pyx_n_s_n_points, __pyx_n_s_neighbor_points, __pyx_n_s_eigenvectors, __pyx_n_s_eigenvalues, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_neighbor_id, __pyx_n_s_n_neighbors_at_id, __pyx_n_s_thread_id, __pyx_n_s_number_of_neighbors, __pyx_n_s_features, __pyx_n_s_radius_vector, __pyx_n_s_p, __pyx_n_s_eps_scipy, __pyx_n_s_threaded_vvres, __pyx_n_s_return_length, __pyx_n_s_n, __pyx_n_s_name); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 6, 27, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jakteristics_extension_pyx, __pyx_n_s_compute_features, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 6, 28, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jakteristics_extension_pyx, __pyx_n_s_compute_features, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 29, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
```

### Comparing `jakteristics-0.5.1/jakteristics/extension.pyx` & `jakteristics-0.6.0/jakteristics/extension.pyx`

 * *Files 23% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         double [::1, :] eigenvectors
         double [:] eigenvalues
 
         int i, j, k
         uint32_t neighbor_id
         uint32_t n_neighbors_at_id
         int thread_id
+        int number_of_neighbors
 
         float [:, :] features = np.full((n_points, len(feature_names)), float("NaN"), dtype=np.float32)
 
         const np.float64_t[:, ::1] radius_vector
         np.float64_t p = 2 if euclidean_distance else 1
         np.float64_t eps_scipy = 0.0
         vector[np.intp_t] *** threaded_vvres
@@ -92,14 +93,15 @@
                 eps_scipy,
                 1,
                 threaded_vvres[thread_id],
                 return_length,
             )
 
             n_neighbors_at_id = threaded_vvres[thread_id][0].size()
+            number_of_neighbors = n_neighbors_at_id
 
             if n_neighbors_at_id > max_k_neighbors:
                 n_neighbors_at_id = max_k_neighbors
             elif n_neighbors_at_id == 0:
                 continue
 
             for j in range(n_neighbors_at_id):
@@ -113,14 +115,15 @@
             )
             utils.c_eigenvectors(
                 eigenvectors[:, thread_id * 3:(thread_id + 1) * 3],
                 eigenvalues[thread_id * 3:(thread_id + 1) * 3],
             )
 
             compute_features_from_eigenvectors(
+                number_of_neighbors,
                 eigenvalues[thread_id * 3 : thread_id * 3 + 3],
                 eigenvectors[:, thread_id * 3 : thread_id * 3 + 3],
                 features[i, :],
                 features_map,
             )
 
     finally:
@@ -128,14 +131,15 @@
 
     return np.asarray(features)
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.cdivision(True)
 cdef inline void compute_features_from_eigenvectors(
+    int number_of_neighbors,
     double [:] eigenvalues,
     double [:, :] eigenvectors,
     float [:] out,
     cppmap [string, uint8_t] & out_map,
 ) nogil:
     cdef:
         float l1, l2, l3
@@ -149,14 +153,24 @@
 
     # Those features are inspired from cloud compare implementation (https://github.com/CloudCompare/CloudCompare/blob/master/CC/src/Neighbourhood.cpp#L871)
     # Those features are also implemented in CGAL (https://doc.cgal.org/4.12/Classification/group__PkgClassificationFeatures.html)
 
     # Sum of eigenvalues equals the original variance of the data
     eigenvalue_sum = l1 + l2 + l3
 
+    if out_map.count(b"eigenvalue1"):
+        out[out_map.at(b"eigenvalue1")] = l1
+    if out_map.count(b"eigenvalue2"):
+        out[out_map.at(b"eigenvalue2")] = l2
+    if out_map.count(b"eigenvalue3"):
+        out[out_map.at(b"eigenvalue3")] = l3
+
+    if out_map.count(b"number_of_neighbors"):
+        out[out_map.at(b"number_of_neighbors")] = number_of_neighbors
+
     if out_map.count(b"eigenvalue_sum"):
         out[out_map.at(b"eigenvalue_sum")] = eigenvalue_sum
 
     if out_map.count(b"omnivariance"):
         out[out_map.at(b"omnivariance")] = pow(l1 * l2 * l3, 1.0 / 3.0)
 
     if out_map.count(b"eigenentropy"):
@@ -194,14 +208,35 @@
         if out_map.count(b"nx"):
             out[out_map.at(b"nx")] = n0 / norm
         if out_map.count(b"ny"):
             out[out_map.at(b"ny")] = n1 / norm
         if out_map.count(b"nz"):
             out[out_map.at(b"nz")] = n2 / norm
 
+    if out_map.count(b"eigenvector1x"):
+        out[out_map.at(b"eigenvector1x")] = eigenvectors[0, 0]
+    if out_map.count(b"eigenvector1y"):
+        out[out_map.at(b"eigenvector1y")] = eigenvectors[0, 1]
+    if out_map.count(b"eigenvector1z"):
+        out[out_map.at(b"eigenvector1z")] = eigenvectors[0, 2]
+
+    if out_map.count(b"eigenvector2x"):
+        out[out_map.at(b"eigenvector2x")] = eigenvectors[1, 0]
+    if out_map.count(b"eigenvector2y"):
+        out[out_map.at(b"eigenvector2y")] = eigenvectors[1, 1]
+    if out_map.count(b"eigenvector2z"):
+        out[out_map.at(b"eigenvector2z")] = eigenvectors[1, 2]
+
+    if out_map.count(b"eigenvector3x"):
+        out[out_map.at(b"eigenvector3x")] = eigenvectors[2, 0]
+    if out_map.count(b"eigenvector3y"):
+        out[out_map.at(b"eigenvector3y")] = eigenvectors[2, 1]
+    if out_map.count(b"eigenvector3z"):
+        out[out_map.at(b"eigenvector3z")] = eigenvectors[2, 2]
+
 
 cdef vector[np.intp_t] *** init_result_vectors(int num_threads):
     """Allocate memory for result vectors, based on thread count"""
     threaded_vvres = <vector[np.intp_t] ***> PyMem_Malloc(num_threads * sizeof(void*))
     if not threaded_vvres:
         raise MemoryError()
     memset(<void*> threaded_vvres, 0, num_threads * sizeof(void*))
@@ -217,8 +252,9 @@
 cdef void free_result_vectors(vector[np.intp_t] *** threaded_vvres, int num_threads):
     """Free memory for result vectors"""
     if threaded_vvres != NULL:
         for i in range(num_threads):
             if threaded_vvres[i] != NULL:
                 del threaded_vvres[i][0]
             PyMem_Free(threaded_vvres[i])
-        PyMem_Free(threaded_vvres)
+        PyMem_Free(threaded_vvres)
+
```

### Comparing `jakteristics-0.5.1/jakteristics/las_utils.py` & `jakteristics-0.6.0/jakteristics/las_utils.py`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics/main.py` & `jakteristics-0.6.0/jakteristics/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import List
+from typing import List, Optional
+import warnings
 
 import numpy as np
 
 import jakteristics.extension
 from jakteristics.ckdtree import ckdtree
 
 from .constants import FEATURE_NAMES
@@ -12,15 +13,15 @@
     points: np.ndarray,
     search_radius: float,
     *,
     kdtree: ckdtree.cKDTree = None,
     num_threads: int = -1,
     max_k_neighbors: int = 50000,
     euclidean_distance: bool = True,
-    feature_names: List[str] = FEATURE_NAMES,
+    feature_names: Optional[List[str]] = None,
     eps: float = 0.0,
 ) -> np.ndarray:
     """
     Compute features for a set of points.
 
     Parameters:
         points:
@@ -54,14 +55,21 @@
             distance to the real k-th nearest neighbor.
 
     Returns:
         The computed features, one row per query point, and one column
         per requested feature.
     """
 
+    if feature_names is None:
+        warnings.warn(
+            "The `feature_names` argument of `compute_features` will be required "
+            "in a future version of jakteristics."
+        )
+        feature_names = FEATURE_NAMES
+
     points = np.ascontiguousarray(points)
 
     return jakteristics.extension.compute_features(
         points,
         search_radius,
         kdtree=kdtree,
         num_threads=num_threads,
```

### Comparing `jakteristics-0.5.1/jakteristics/utils.cpp` & `jakteristics-0.6.0/jakteristics/utils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "1"
             ]
         ],
         "depends": [
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/core/include"
+            "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "jakteristics.utils",
         "sources": [
             "jakteristics/utils.pyx"
         ]
     },
@@ -1136,195 +1136,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1391,42 +1391,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -4097,15 +4097,15 @@
   __Pyx_XDECREF(__pyx_v_eigenvalues);
   __Pyx_XDECREF(__pyx_v_a);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4114,29 +4114,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4147,15 +4147,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4164,29 +4164,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4197,15 +4197,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4214,29 +4214,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4247,15 +4247,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4264,29 +4264,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4297,15 +4297,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4314,29 +4314,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4347,212 +4347,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4568,15 +4568,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4584,53 +4584,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -4638,30 +4638,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4676,15 +4676,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4700,15 +4700,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4716,53 +4716,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -4770,30 +4770,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4808,15 +4808,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4832,15 +4832,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4848,53 +4848,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -4902,30 +4902,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4940,176 +4940,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19055,26 +19055,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
```

### Comparing `jakteristics-0.5.1/jakteristics/utils.pyx` & `jakteristics-0.6.0/jakteristics/utils.pyx`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/jakteristics.egg-info/PKG-INFO` & `jakteristics-0.6.0/jakteristics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jakteristics
-Version: 0.5.1
+Version: 0.6.0
 Summary: Point cloud geometric properties from python.
 Home-page: https://github.com/jakarto3d/jakteristics
 Author: David Caron
 Author-email: david.caron@jakarto.com
 License: BSD
 Keywords: jakteristics
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -70,15 +70,15 @@
 From python
 -----------
 
 .. code:: python
 
     from jakteristics import compute_features
 
-    features = compute_features(xyz, search_radius=0.15)
+    features = compute_features(xyz, search_radius=0.15, feature_names=['planarity', 'linearity'])
 
 
 CLI
 ---
 
 Once the package is installed, you can use the `jakteristics` command:
 
@@ -101,14 +101,21 @@
 History
 -------
 
 Unreleased
 ----------
 
 
+0.6.0 (2023-04-20)
+------------------
+
+* add: number_of_neighbors feature
+* add: eigenvalues and eigenvectors features
+
+
 0.5.1 (2023-04-11)
 ------------------
 
 * fix: computing features when kdtree is not built from the same points for which we want to compute the features
 * drop python 3.6, add wheels for python 3.7-3.11 on linux and windows
 
 0.5.0 (2022-01-26)
```

### Comparing `jakteristics-0.5.1/jakteristics.egg-info/SOURCES.txt` & `jakteristics-0.6.0/jakteristics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jakteristics-0.5.1/setup.py` & `jakteristics-0.6.0/setup.py`

 * *Files identical despite different names*

