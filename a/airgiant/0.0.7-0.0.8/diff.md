# Comparing `tmp/airgiant-0.0.7.tar.gz` & `tmp/airgiant-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airgiant-0.0.7.tar", last modified: Wed Apr 19 15:08:19 2023, max compression
+gzip compressed data, was "airgiant-0.0.8.tar", last modified: Wed Apr 19 15:25:59 2023, max compression
```

## Comparing `airgiant-0.0.7.tar` & `airgiant-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 15:08:19.676944 airgiant-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-04-18 15:04:47.000000 airgiant-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      544 2023-04-19 15:08:19.675943 airgiant-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-04-18 15:22:04.000000 airgiant-0.0.7/README.md
--rw-rw-rw-   0        0        0      595 2023-04-19 15:08:04.000000 airgiant-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 15:08:19.676944 airgiant-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 15:08:19.645944 airgiant-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:08:19.649942 airgiant-0.0.7/src/airgiant/
--rw-rw-rw-   0        0        0       46 2023-04-19 14:01:17.000000 airgiant-0.0.7/src/airgiant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:08:19.673941 airgiant-0.0.7/src/airgiant/state/
--rw-rw-rw-   0        0        0       24 2023-04-19 15:07:26.000000 airgiant-0.0.7/src/airgiant/state/__init__.py
--rw-rw-rw-   0        0        0       38 2023-04-19 15:00:21.000000 airgiant-0.0.7/src/airgiant/state/hello.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:08:19.674944 airgiant-0.0.7/src/airgiant/zed/
--rw-rw-rw-   0        0        0     3970 2023-04-19 14:46:23.000000 airgiant-0.0.7/src/airgiant/zed/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:08:19.666941 airgiant-0.0.7/src/airgiant.egg-info/
--rw-rw-rw-   0        0        0      544 2023-04-19 15:08:19.000000 airgiant-0.0.7/src/airgiant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-04-19 15:08:19.000000 airgiant-0.0.7/src/airgiant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 15:08:19.000000 airgiant-0.0.7/src/airgiant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 15:08:19.000000 airgiant-0.0.7/src/airgiant.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 15:25:59.521826 airgiant-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-04-18 15:04:47.000000 airgiant-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      544 2023-04-19 15:25:59.521826 airgiant-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-04-18 15:22:04.000000 airgiant-0.0.8/README.md
+-rw-rw-rw-   0        0        0      595 2023-04-19 15:25:38.000000 airgiant-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:25:59.522821 airgiant-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 15:25:59.495007 airgiant-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 15:25:59.501524 airgiant-0.0.8/src/airgiant/
+-rw-rw-rw-   0        0        0       46 2023-04-19 14:01:17.000000 airgiant-0.0.8/src/airgiant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:25:59.518727 airgiant-0.0.8/src/airgiant/state/
+-rw-rw-rw-   0        0        0       24 2023-04-19 15:07:26.000000 airgiant-0.0.8/src/airgiant/state/__init__.py
+-rw-rw-rw-   0        0        0       38 2023-04-19 15:00:21.000000 airgiant-0.0.8/src/airgiant/state/hello.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:25:59.520830 airgiant-0.0.8/src/airgiant/zed/
+-rw-rw-rw-   0        0        0      237 2023-04-19 15:18:13.000000 airgiant-0.0.8/src/airgiant/zed/__init__.py
+-rw-rw-rw-   0        0        0     3754 2023-04-19 15:16:49.000000 airgiant-0.0.8/src/airgiant/zed/skeleton.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:25:59.516519 airgiant-0.0.8/src/airgiant.egg-info/
+-rw-rw-rw-   0        0        0      544 2023-04-19 15:25:59.000000 airgiant-0.0.8/src/airgiant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-04-19 15:25:59.000000 airgiant-0.0.8/src/airgiant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:25:59.000000 airgiant-0.0.8/src/airgiant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 15:25:59.000000 airgiant-0.0.8/src/airgiant.egg-info/top_level.txt
```

### Comparing `airgiant-0.0.7/LICENSE` & `airgiant-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `airgiant-0.0.7/PKG-INFO` & `airgiant-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgiant
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `airgiant-0.0.7/pyproject.toml` & `airgiant-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "airgiant"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `airgiant-0.0.7/src/airgiant/zed/__init__.py` & `airgiant-0.0.8/src/airgiant/zed/skeleton.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,8 @@
-import pyzed.sl as sl
-import matplotlib.pyplot as plt
-from mpl_toolkits.mplot3d import Axes3D
-import asyncio
-import math
-import time
-import random
-import websockets
-import json
-import sys
-import logging
-
-async def SkelNeckCoord():
+async def skelneckcoord():
     # Define the keypoints
     global total_pos
     
     
     keypoints = {
         0: 'nose',
         1: 'neck',
```

### Comparing `airgiant-0.0.7/src/airgiant.egg-info/PKG-INFO` & `airgiant-0.0.8/src/airgiant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgiant
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

