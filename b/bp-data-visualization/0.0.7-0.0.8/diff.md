# Comparing `tmp/bp_data_visualization-0.0.7.tar.gz` & `tmp/bp-data-visualization-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_visualization-0.0.7.tar", last modified: Wed Apr 19 07:42:21 2023, max compression
+gzip compressed data, was "bp-data-visualization-0.0.8.tar", last modified: Thu Apr 20 06:54:11 2023, max compression
```

## Comparing `bp_data_visualization-0.0.7.tar` & `bp-data-visualization-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:42:21.010039 bp_data_visualization-0.0.7/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-19 06:01:44.000000 bp_data_visualization-0.0.7/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       53 2023-04-19 06:01:44.000000 bp_data_visualization-0.0.7/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      294 2023-04-19 07:42:21.009728 bp_data_visualization-0.0.7/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       21 2023-04-19 06:01:44.000000 bp_data_visualization-0.0.7/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:42:20.998928 bp_data_visualization-0.0.7/bp_data_visualization.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      294 2023-04-19 07:42:20.000000 bp_data_visualization-0.0.7/bp_data_visualization.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      527 2023-04-19 07:42:20.000000 bp_data_visualization-0.0.7/bp_data_visualization.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-19 07:42:20.000000 bp_data_visualization-0.0.7/bp_data_visualization.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-19 07:42:20.000000 bp_data_visualization-0.0.7/bp_data_visualization.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       19 2023-04-19 07:42:20.000000 bp_data_visualization-0.0.7/bp_data_visualization.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:42:21.000412 bp_data_visualization-0.0.7/data_visualization/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2091 2023-04-19 07:26:38.000000 bp_data_visualization-0.0.7/data_visualization/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:42:20.993386 bp_data_visualization-0.0.7/data_visualization/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:42:21.002050 bp_data_visualization-0.0.7/data_visualization/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:42:21.008791 bp_data_visualization-0.0.7/data_visualization/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1959381 2023-04-19 06:49:19.000000 bp_data_visualization-0.0.7/data_visualization/frontend/dist/assets/index-80a55e32.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-19 06:49:19.000000 bp_data_visualization-0.0.7/data_visualization/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      457 2023-04-19 06:52:40.000000 bp_data_visualization-0.0.7/data_visualization/frontend/dist/index.html
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-19 06:49:18.000000 bp_data_visualization-0.0.7/data_visualization/frontend/dist/vite.svg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-19 06:01:44.000000 bp_data_visualization-0.0.7/data_visualization/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-19 07:42:21.010144 bp_data_visualization-0.0.7/setup.cfg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      628 2023-04-19 07:40:05.000000 bp_data_visualization-0.0.7/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 06:54:11.351459 bp-data-visualization-0.0.8/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-19 06:01:44.000000 bp-data-visualization-0.0.8/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       53 2023-04-19 06:01:44.000000 bp-data-visualization-0.0.8/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      294 2023-04-20 06:54:11.350927 bp-data-visualization-0.0.8/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       21 2023-04-19 06:01:44.000000 bp-data-visualization-0.0.8/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 06:54:11.343253 bp-data-visualization-0.0.8/bp_data_visualization.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      294 2023-04-20 06:54:11.000000 bp-data-visualization-0.0.8/bp_data_visualization.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      527 2023-04-20 06:54:11.000000 bp-data-visualization-0.0.8/bp_data_visualization.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-20 06:54:11.000000 bp-data-visualization-0.0.8/bp_data_visualization.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-20 06:54:11.000000 bp-data-visualization-0.0.8/bp_data_visualization.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       19 2023-04-20 06:54:11.000000 bp-data-visualization-0.0.8/bp_data_visualization.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 06:54:11.344205 bp-data-visualization-0.0.8/data_visualization/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2091 2023-04-20 06:41:53.000000 bp-data-visualization-0.0.8/data_visualization/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 06:54:11.339534 bp-data-visualization-0.0.8/data_visualization/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 06:54:11.345187 bp-data-visualization-0.0.8/data_visualization/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 06:54:11.350168 bp-data-visualization-0.0.8/data_visualization/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1959381 2023-04-20 06:42:10.000000 bp-data-visualization-0.0.8/data_visualization/frontend/dist/assets/index-80a55e32.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-20 06:42:10.000000 bp-data-visualization-0.0.8/data_visualization/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      457 2023-04-20 06:42:31.000000 bp-data-visualization-0.0.8/data_visualization/frontend/dist/index.html
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-20 06:42:09.000000 bp-data-visualization-0.0.8/data_visualization/frontend/dist/vite.svg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-19 06:01:44.000000 bp-data-visualization-0.0.8/data_visualization/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-20 06:54:11.351626 bp-data-visualization-0.0.8/setup.cfg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      628 2023-04-20 06:53:00.000000 bp-data-visualization-0.0.8/setup.py
```

### Comparing `bp_data_visualization-0.0.7/LICENSE` & `bp-data-visualization-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_visualization-0.0.7/bp_data_visualization.egg-info/SOURCES.txt` & `bp-data-visualization-0.0.8/bp_data_visualization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bp_data_visualization-0.0.7/data_visualization/__init__.py` & `bp-data-visualization-0.0.8/data_visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_data_visualization-0.0.7/data_visualization/frontend/dist/assets/index-80a55e32.js` & `bp-data-visualization-0.0.8/data_visualization/frontend/dist/assets/index-80a55e32.js`

 * *Files identical despite different names*

### Comparing `bp_data_visualization-0.0.7/data_visualization/frontend/dist/vite.svg` & `bp-data-visualization-0.0.8/data_visualization/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `bp_data_visualization-0.0.7/data_visualization/register.py` & `bp-data-visualization-0.0.8/data_visualization/register.py`

 * *Files identical despite different names*

### Comparing `bp_data_visualization-0.0.7/setup.py` & `bp-data-visualization-0.0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
-    name="bp_data_visualization",
-    version="0.0.7",
+    name="bp-data-visualization",
+    version="0.0.8",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="Show data in charts",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

