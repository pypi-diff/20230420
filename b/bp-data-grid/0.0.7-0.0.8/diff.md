# Comparing `tmp/bp_data_grid-0.0.7.tar.gz` & `tmp/bp_data_grid-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_grid-0.0.7.tar", last modified: Wed Apr 19 05:42:09 2023, max compression
+gzip compressed data, was "bp_data_grid-0.0.8.tar", last modified: Thu Apr 20 10:20:44 2023, max compression
```

## Comparing `bp_data_grid-0.0.7.tar` & `bp_data_grid-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 05:42:09.494524 bp_data_grid-0.0.7/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-10 18:26:13.000000 bp_data_grid-0.0.7/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       44 2023-04-10 18:26:13.000000 bp_data_grid-0.0.7/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      289 2023-04-19 05:42:09.494082 bp_data_grid-0.0.7/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       21 2023-04-10 05:35:41.000000 bp_data_grid-0.0.7/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 05:42:09.483649 bp_data_grid-0.0.7/bp_data_grid.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      289 2023-04-19 05:42:09.000000 bp_data_grid-0.0.7/bp_data_grid.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      619 2023-04-19 05:42:09.000000 bp_data_grid-0.0.7/bp_data_grid.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-19 05:42:09.000000 bp_data_grid-0.0.7/bp_data_grid.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-19 05:42:09.000000 bp_data_grid-0.0.7/bp_data_grid.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       10 2023-04-19 05:42:09.000000 bp_data_grid-0.0.7/bp_data_grid.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 05:42:09.484730 bp_data_grid-0.0.7/data_grid/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2096 2023-04-18 06:06:34.000000 bp_data_grid-0.0.7/data_grid/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 05:42:09.479204 bp_data_grid-0.0.7/data_grid/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 05:42:09.485904 bp_data_grid-0.0.7/data_grid/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 05:42:09.493340 bp_data_grid-0.0.7/data_grid/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   202328 2023-04-19 05:40:54.000000 bp_data_grid-0.0.7/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1524859 2023-04-19 05:40:54.000000 bp_data_grid-0.0.7/data_grid/frontend/dist/assets/index-5b084c18.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-19 05:40:54.000000 bp_data_grid-0.0.7/data_grid/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   150073 2023-04-19 05:40:54.000000 bp_data_grid-0.0.7/data_grid/frontend/dist/assets/index.es-12db6927-aca7de2c.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)    21573 2023-04-19 05:40:54.000000 bp_data_grid-0.0.7/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      450 2023-04-19 05:41:12.000000 bp_data_grid-0.0.7/data_grid/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-19 05:40:53.000000 bp_data_grid-0.0.7/data_grid/frontend/dist/vite.svg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-10 09:19:07.000000 bp_data_grid-0.0.7/data_grid/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-19 05:42:09.494679 bp_data_grid-0.0.7/setup.cfg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      623 2023-04-19 05:41:19.000000 bp_data_grid-0.0.7/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 10:20:44.016161 bp_data_grid-0.0.8/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-10 18:26:13.000000 bp_data_grid-0.0.8/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       44 2023-04-10 18:26:13.000000 bp_data_grid-0.0.8/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-20 10:20:44.015772 bp_data_grid-0.0.8/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       21 2023-04-10 05:35:41.000000 bp_data_grid-0.0.8/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 10:20:44.001055 bp_data_grid-0.0.8/bp_data_grid.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-20 10:20:43.000000 bp_data_grid-0.0.8/bp_data_grid.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      619 2023-04-20 10:20:43.000000 bp_data_grid-0.0.8/bp_data_grid.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-20 10:20:43.000000 bp_data_grid-0.0.8/bp_data_grid.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-20 10:20:43.000000 bp_data_grid-0.0.8/bp_data_grid.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       10 2023-04-20 10:20:43.000000 bp_data_grid-0.0.8/bp_data_grid.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 10:20:44.002151 bp_data_grid-0.0.8/data_grid/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2096 2023-04-18 06:06:34.000000 bp_data_grid-0.0.8/data_grid/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 10:20:43.997255 bp_data_grid-0.0.8/data_grid/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 10:20:44.003689 bp_data_grid-0.0.8/data_grid/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-20 10:20:44.015113 bp_data_grid-0.0.8/data_grid/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   202328 2023-04-19 05:40:54.000000 bp_data_grid-0.0.8/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1524859 2023-04-19 05:40:54.000000 bp_data_grid-0.0.8/data_grid/frontend/dist/assets/index-5b084c18.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-19 05:40:54.000000 bp_data_grid-0.0.8/data_grid/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   150073 2023-04-19 05:40:54.000000 bp_data_grid-0.0.8/data_grid/frontend/dist/assets/index.es-12db6927-aca7de2c.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)    21573 2023-04-19 05:40:54.000000 bp_data_grid-0.0.8/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      450 2023-04-19 05:41:12.000000 bp_data_grid-0.0.8/data_grid/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-19 05:40:53.000000 bp_data_grid-0.0.8/data_grid/frontend/dist/vite.svg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-10 09:19:07.000000 bp_data_grid-0.0.8/data_grid/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-20 10:20:44.016299 bp_data_grid-0.0.8/setup.cfg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      623 2023-04-20 10:19:11.000000 bp_data_grid-0.0.8/setup.py
```

### Comparing `bp_data_grid-0.0.7/LICENSE` & `bp_data_grid-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.7/bp_data_grid.egg-info/SOURCES.txt` & `bp_data_grid-0.0.8/bp_data_grid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.7/data_grid/__init__.py` & `bp_data_grid-0.0.8/data_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.7/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js` & `bp_data_grid-0.0.8/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.7/data_grid/frontend/dist/assets/index-5b084c18.js` & `bp_data_grid-0.0.8/data_grid/frontend/dist/assets/index-5b084c18.js`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.7/data_grid/frontend/dist/assets/index.es-12db6927-aca7de2c.js` & `bp_data_grid-0.0.8/data_grid/frontend/dist/assets/index.es-12db6927-aca7de2c.js`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.7/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js` & `bp_data_grid-0.0.8/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.7/data_grid/frontend/dist/vite.svg` & `bp_data_grid-0.0.8/data_grid/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.7/data_grid/register.py` & `bp_data_grid-0.0.8/data_grid/register.py`

 * *Files identical despite different names*

### Comparing `bp_data_grid-0.0.7/setup.py` & `bp_data_grid-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bp_data_grid",
-    version="0.0.7",
+    version="0.0.8",
     author="Bluepinapple",
     author_email="vivek.sthul@bluepinapple.com",
     description="Show data in data grid",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

