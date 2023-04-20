# Comparing `tmp/jcopvision-0.2.3.tar.gz` & `tmp/jcopvision-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcopvision-0.2.3.tar", last modified: Tue Apr 18 17:30:55 2023, max compression
+gzip compressed data, was "jcopvision-0.2.4.tar", last modified: Thu Apr 20 16:43:59 2023, max compression
```

## Comparing `jcopvision-0.2.3.tar` & `jcopvision-0.2.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.375317 jcopvision-0.2.3/
--rw-r--r--   0 bmduser    (501) staff       (20)     1513 2023-02-10 18:31:03.000000 jcopvision-0.2.3/LICENSE
--rw-r--r--   0 bmduser    (501) staff       (20)     1065 2023-04-18 17:30:55.375424 jcopvision-0.2.3/PKG-INFO
--rw-r--r--   0 bmduser    (501) staff       (20)      283 2023-02-10 18:31:03.000000 jcopvision-0.2.3/README.md
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.367180 jcopvision-0.2.3/jcopvision/
--rw-r--r--   0 bmduser    (501) staff       (20)       80 2023-04-18 16:38:02.000000 jcopvision-0.2.3/jcopvision/__init__.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.370400 jcopvision-0.2.3/jcopvision/draw/
--rw-r--r--   0 bmduser    (501) staff       (20)      192 2023-04-18 17:18:39.000000 jcopvision-0.2.3/jcopvision/draw/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)     2660 2023-04-18 17:10:33.000000 jcopvision-0.2.3/jcopvision/draw/bbox.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1142 2023-04-18 17:10:47.000000 jcopvision-0.2.3/jcopvision/draw/circle.py
--rw-r--r--   0 bmduser    (501) staff       (20)      850 2023-02-17 17:03:56.000000 jcopvision-0.2.3/jcopvision/draw/imshow.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1230 2023-04-18 17:17:49.000000 jcopvision-0.2.3/jcopvision/draw/line.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1544 2023-04-18 17:10:58.000000 jcopvision-0.2.3/jcopvision/draw/text.py
--rw-r--r--   0 bmduser    (501) staff       (20)      146 2023-02-17 11:27:53.000000 jcopvision-0.2.3/jcopvision/exception.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.371468 jcopvision-0.2.3/jcopvision/image_processing/
--rw-r--r--   0 bmduser    (501) staff       (20)      137 2023-02-17 17:21:06.000000 jcopvision-0.2.3/jcopvision/image_processing/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1360 2023-02-17 17:04:55.000000 jcopvision-0.2.3/jcopvision/image_processing/blending.py
--rw-r--r--   0 bmduser    (501) staff       (20)      415 2023-02-17 17:05:43.000000 jcopvision-0.2.3/jcopvision/image_processing/enhancement.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1888 2023-02-17 17:06:45.000000 jcopvision-0.2.3/jcopvision/image_processing/masking.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.373167 jcopvision-0.2.3/jcopvision/io/
--rw-r--r--   0 bmduser    (501) staff       (20)      161 2023-02-17 17:20:33.000000 jcopvision-0.2.3/jcopvision/io/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)      701 2023-02-17 17:12:22.000000 jcopvision-0.2.3/jcopvision/io/jupyter.py
--rw-r--r--   0 bmduser    (501) staff       (20)     4347 2023-02-21 06:58:23.000000 jcopvision-0.2.3/jcopvision/io/reader.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1527 2023-02-17 17:08:47.000000 jcopvision-0.2.3/jcopvision/io/utils.py
--rw-r--r--   0 bmduser    (501) staff       (20)     3026 2023-02-17 17:16:45.000000 jcopvision-0.2.3/jcopvision/io/writer.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.375069 jcopvision-0.2.3/jcopvision/utils/
--rw-r--r--   0 bmduser    (501) staff       (20)      436 2023-04-18 16:49:05.000000 jcopvision-0.2.3/jcopvision/utils/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)      260 2023-02-17 17:23:09.000000 jcopvision-0.2.3/jcopvision/utils/background.py
--rw-r--r--   0 bmduser    (501) staff       (20)     2018 2023-02-17 17:23:57.000000 jcopvision-0.2.3/jcopvision/utils/bbox.py
--rw-r--r--   0 bmduser    (501) staff       (20)      860 2023-04-18 17:08:49.000000 jcopvision-0.2.3/jcopvision/utils/color.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1810 2023-02-17 17:26:23.000000 jcopvision-0.2.3/jcopvision/utils/filter.py
--rw-r--r--   0 bmduser    (501) staff       (20)      505 2023-04-18 17:00:09.000000 jcopvision-0.2.3/jcopvision/utils/image.py
--rw-r--r--   0 bmduser    (501) staff       (20)      537 2023-02-17 17:27:38.000000 jcopvision-0.2.3/jcopvision/utils/landmark.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-18 17:30:55.368567 jcopvision-0.2.3/jcopvision.egg-info/
--rw-r--r--   0 bmduser    (501) staff       (20)     1065 2023-04-18 17:30:55.000000 jcopvision-0.2.3/jcopvision.egg-info/PKG-INFO
--rw-r--r--   0 bmduser    (501) staff       (20)      881 2023-04-18 17:30:55.000000 jcopvision-0.2.3/jcopvision.egg-info/SOURCES.txt
--rw-r--r--   0 bmduser    (501) staff       (20)        1 2023-04-18 17:30:55.000000 jcopvision-0.2.3/jcopvision.egg-info/dependency_links.txt
--rw-r--r--   0 bmduser    (501) staff       (20)       38 2023-04-18 17:30:55.000000 jcopvision-0.2.3/jcopvision.egg-info/requires.txt
--rw-r--r--   0 bmduser    (501) staff       (20)       11 2023-04-18 17:30:55.000000 jcopvision-0.2.3/jcopvision.egg-info/top_level.txt
--rw-r--r--   0 bmduser    (501) staff       (20)       67 2023-04-18 17:30:55.375878 jcopvision-0.2.3/setup.cfg
--rw-r--r--   0 bmduser    (501) staff       (20)     1093 2023-02-10 18:31:03.000000 jcopvision-0.2.3/setup.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-20 16:43:59.107828 jcopvision-0.2.4/
+-rw-r--r--   0 bmduser    (501) staff       (20)     1513 2023-02-10 18:31:03.000000 jcopvision-0.2.4/LICENSE
+-rw-r--r--   0 bmduser    (501) staff       (20)     1065 2023-04-20 16:43:59.107949 jcopvision-0.2.4/PKG-INFO
+-rw-r--r--   0 bmduser    (501) staff       (20)      283 2023-02-10 18:31:03.000000 jcopvision-0.2.4/README.md
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-20 16:43:59.092313 jcopvision-0.2.4/jcopvision/
+-rw-r--r--   0 bmduser    (501) staff       (20)       80 2023-04-20 16:41:22.000000 jcopvision-0.2.4/jcopvision/__init__.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-20 16:43:59.097981 jcopvision-0.2.4/jcopvision/draw/
+-rw-r--r--   0 bmduser    (501) staff       (20)      192 2023-04-18 17:18:39.000000 jcopvision-0.2.4/jcopvision/draw/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     2660 2023-04-18 17:10:33.000000 jcopvision-0.2.4/jcopvision/draw/bbox.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1142 2023-04-18 17:10:47.000000 jcopvision-0.2.4/jcopvision/draw/circle.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      850 2023-02-17 17:03:56.000000 jcopvision-0.2.4/jcopvision/draw/imshow.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1230 2023-04-18 17:17:49.000000 jcopvision-0.2.4/jcopvision/draw/line.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1544 2023-04-18 17:10:58.000000 jcopvision-0.2.4/jcopvision/draw/text.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      146 2023-02-17 11:27:53.000000 jcopvision-0.2.4/jcopvision/exception.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-20 16:43:59.100473 jcopvision-0.2.4/jcopvision/image_processing/
+-rw-r--r--   0 bmduser    (501) staff       (20)      137 2023-02-17 17:21:06.000000 jcopvision-0.2.4/jcopvision/image_processing/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1360 2023-02-17 17:04:55.000000 jcopvision-0.2.4/jcopvision/image_processing/blending.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      415 2023-02-17 17:05:43.000000 jcopvision-0.2.4/jcopvision/image_processing/enhancement.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1888 2023-02-17 17:06:45.000000 jcopvision-0.2.4/jcopvision/image_processing/masking.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-20 16:43:59.103304 jcopvision-0.2.4/jcopvision/io/
+-rw-r--r--   0 bmduser    (501) staff       (20)      161 2023-02-17 17:20:33.000000 jcopvision-0.2.4/jcopvision/io/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      701 2023-02-17 17:12:22.000000 jcopvision-0.2.4/jcopvision/io/jupyter.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     6981 2023-04-20 16:40:29.000000 jcopvision-0.2.4/jcopvision/io/reader.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1527 2023-02-17 17:08:47.000000 jcopvision-0.2.4/jcopvision/io/utils.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     3026 2023-02-17 17:16:45.000000 jcopvision-0.2.4/jcopvision/io/writer.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-20 16:43:59.107436 jcopvision-0.2.4/jcopvision/utils/
+-rw-r--r--   0 bmduser    (501) staff       (20)      436 2023-04-18 16:49:05.000000 jcopvision-0.2.4/jcopvision/utils/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      260 2023-02-17 17:23:09.000000 jcopvision-0.2.4/jcopvision/utils/background.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     2018 2023-02-17 17:23:57.000000 jcopvision-0.2.4/jcopvision/utils/bbox.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      860 2023-04-18 17:08:49.000000 jcopvision-0.2.4/jcopvision/utils/color.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1810 2023-02-17 17:26:23.000000 jcopvision-0.2.4/jcopvision/utils/filter.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      505 2023-04-18 17:00:09.000000 jcopvision-0.2.4/jcopvision/utils/image.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      537 2023-02-17 17:27:38.000000 jcopvision-0.2.4/jcopvision/utils/landmark.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-04-20 16:43:59.094202 jcopvision-0.2.4/jcopvision.egg-info/
+-rw-r--r--   0 bmduser    (501) staff       (20)     1065 2023-04-20 16:43:58.000000 jcopvision-0.2.4/jcopvision.egg-info/PKG-INFO
+-rw-r--r--   0 bmduser    (501) staff       (20)      881 2023-04-20 16:43:58.000000 jcopvision-0.2.4/jcopvision.egg-info/SOURCES.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)        1 2023-04-20 16:43:58.000000 jcopvision-0.2.4/jcopvision.egg-info/dependency_links.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)       60 2023-04-20 16:43:58.000000 jcopvision-0.2.4/jcopvision.egg-info/requires.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)       11 2023-04-20 16:43:58.000000 jcopvision-0.2.4/jcopvision.egg-info/top_level.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)       67 2023-04-20 16:43:59.108574 jcopvision-0.2.4/setup.cfg
+-rw-r--r--   0 bmduser    (501) staff       (20)     1118 2023-04-20 09:24:32.000000 jcopvision-0.2.4/setup.py
```

### Comparing `jcopvision-0.2.3/LICENSE` & `jcopvision-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/PKG-INFO` & `jcopvision-0.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcopvision
-Version: 0.2.3
+Version: 0.2.4
 Summary: J.COp Vision consists of helper tools for computer vision
 Home-page: https://github.com/WiraDKP/jcopvision
 Author: Wira Dharma Kencana Putra
 Author-email: wiradharma_kencanaputra@yahoo.com
 Keywords: computer vision dl jcop indonesia
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

### Comparing `jcopvision-0.2.3/jcopvision/draw/bbox.py` & `jcopvision-0.2.4/jcopvision/draw/bbox.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/draw/circle.py` & `jcopvision-0.2.4/jcopvision/draw/circle.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/draw/imshow.py` & `jcopvision-0.2.4/jcopvision/draw/imshow.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/draw/line.py` & `jcopvision-0.2.4/jcopvision/draw/line.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/draw/text.py` & `jcopvision-0.2.4/jcopvision/draw/text.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/image_processing/blending.py` & `jcopvision-0.2.4/jcopvision/image_processing/blending.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/image_processing/masking.py` & `jcopvision-0.2.4/jcopvision/image_processing/masking.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/io/jupyter.py` & `jcopvision-0.2.4/jcopvision/io/jupyter.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/io/utils.py` & `jcopvision-0.2.4/jcopvision/io/utils.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/io/writer.py` & `jcopvision-0.2.4/jcopvision/io/writer.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/utils/bbox.py` & `jcopvision-0.2.4/jcopvision/utils/bbox.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/utils/color.py` & `jcopvision-0.2.4/jcopvision/utils/color.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/utils/filter.py` & `jcopvision-0.2.4/jcopvision/utils/filter.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision/utils/landmark.py` & `jcopvision-0.2.4/jcopvision/utils/landmark.py`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/jcopvision.egg-info/PKG-INFO` & `jcopvision-0.2.4/jcopvision.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcopvision
-Version: 0.2.3
+Version: 0.2.4
 Summary: J.COp Vision consists of helper tools for computer vision
 Home-page: https://github.com/WiraDKP/jcopvision
 Author: Wira Dharma Kencana Putra
 Author-email: wiradharma_kencanaputra@yahoo.com
 Keywords: computer vision dl jcop indonesia
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

### Comparing `jcopvision-0.2.3/jcopvision.egg-info/SOURCES.txt` & `jcopvision-0.2.4/jcopvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jcopvision-0.2.3/setup.py` & `jcopvision-0.2.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     version=jcopvision.__version__,
     author="Wira Dharma Kencana Putra",
     author_email="wiradharma_kencanaputra@yahoo.com",
     description="J.COp Vision consists of helper tools for computer vision",
     long_description=description,
     long_description_content_type="text/markdown",
     python_requires=">=3.6.7",
-    install_requires=["opencv-python", "numpy", "pillow", "matplotlib"],
+    install_requires=["opencv-python", "opencv-contrib-python", "numpy", "pillow", "matplotlib"],
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
```

