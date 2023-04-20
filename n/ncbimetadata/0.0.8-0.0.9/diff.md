# Comparing `tmp/ncbimetadata-0.0.8.tar.gz` & `tmp/ncbimetadata-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbimetadata-0.0.8.tar", last modified: Thu Apr 20 10:14:53 2023, max compression
+gzip compressed data, was "ncbimetadata-0.0.9.tar", last modified: Thu Apr 20 10:29:17 2023, max compression
```

## Comparing `ncbimetadata-0.0.8.tar` & `ncbimetadata-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:14:53.990058 ncbimetadata-0.0.8/
--rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.0.8/LICENSE
--rw-r--r--   0 taiyuan    (501) staff       (20)     3075 2023-04-20 10:14:53.989816 ncbimetadata-0.0.8/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.0.8/README.md
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:14:53.987722 ncbimetadata-0.0.8/bin/
--rw-r--r--   0 taiyuan    (501) staff       (20)      152 2023-04-20 08:50:52.000000 ncbimetadata-0.0.8/bin/ncbimetadata
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:14:53.988068 ncbimetadata-0.0.8/ncbimetadata/
--rw-r--r--   0 taiyuan    (501) staff       (20)    11112 2023-04-20 08:02:11.000000 ncbimetadata-0.0.8/ncbimetadata/__init__.py
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:14:53.989544 ncbimetadata-0.0.8/ncbimetadata.egg-info/
--rw-r--r--   0 taiyuan    (501) staff       (20)     3075 2023-04-20 10:14:53.000000 ncbimetadata-0.0.8/ncbimetadata.egg-info/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)      282 2023-04-20 10:14:53.000000 ncbimetadata-0.0.8/ncbimetadata.egg-info/SOURCES.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 10:14:53.000000 ncbimetadata-0.0.8/ncbimetadata.egg-info/dependency_links.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 10:14:53.000000 ncbimetadata-0.0.8/ncbimetadata.egg-info/not-zip-safe
--rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 10:14:53.000000 ncbimetadata-0.0.8/ncbimetadata.egg-info/requires.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 10:14:53.000000 ncbimetadata-0.0.8/ncbimetadata.egg-info/top_level.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 10:14:53.990155 ncbimetadata-0.0.8/setup.cfg
--rw-r--r--   0 taiyuan    (501) staff       (20)      778 2023-04-20 10:14:46.000000 ncbimetadata-0.0.8/setup.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:29:17.345615 ncbimetadata-0.0.9/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.0.9/LICENSE
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3075 2023-04-20 10:29:17.345491 ncbimetadata-0.0.9/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.0.9/README.md
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:29:17.343789 ncbimetadata-0.0.9/bin/
+-rw-r--r--   0 taiyuan    (501) staff       (20)      152 2023-04-20 08:50:52.000000 ncbimetadata-0.0.9/bin/ncbimetadata
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:29:17.344233 ncbimetadata-0.0.9/ncbimetadata/
+-rw-r--r--   0 taiyuan    (501) staff       (20)    11112 2023-04-20 08:02:11.000000 ncbimetadata-0.0.9/ncbimetadata/__init__.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:29:17.345318 ncbimetadata-0.0.9/ncbimetadata.egg-info/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3075 2023-04-20 10:29:17.000000 ncbimetadata-0.0.9/ncbimetadata.egg-info/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)      282 2023-04-20 10:29:17.000000 ncbimetadata-0.0.9/ncbimetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 10:29:17.000000 ncbimetadata-0.0.9/ncbimetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 10:27:53.000000 ncbimetadata-0.0.9/ncbimetadata.egg-info/not-zip-safe
+-rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 10:29:17.000000 ncbimetadata-0.0.9/ncbimetadata.egg-info/requires.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 10:29:17.000000 ncbimetadata-0.0.9/ncbimetadata.egg-info/top_level.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 10:29:17.345656 ncbimetadata-0.0.9/setup.cfg
+-rw-r--r--   0 taiyuan    (501) staff       (20)      910 2023-04-20 10:27:57.000000 ncbimetadata-0.0.9/setup.py
```

### Comparing `ncbimetadata-0.0.8/LICENSE` & `ncbimetadata-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.8/PKG-INFO` & `ncbimetadata-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.0.8
+Version: 0.0.9
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbimetadata
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
```

### Comparing `ncbimetadata-0.0.8/README.md` & `ncbimetadata-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.8/ncbimetadata/__init__.py` & `ncbimetadata-0.0.9/ncbimetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.8/ncbimetadata.egg-info/PKG-INFO` & `ncbimetadata-0.0.9/ncbimetadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.0.8
+Version: 0.0.9
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbimetadata
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
```

### Comparing `ncbimetadata-0.0.8/setup.py` & `ncbimetadata-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from setuptools import setup
+import sys
+import os
 
 
 def readfile(filename):
     with open(filename, 'r+') as f:
         return f.read()
 
 
+if sys.platform == 'win32' or os.name == 'nt':
+    script = "bin/ncbimetadata.exe"
+else:
+    script = "bin/ncbimetadata"
+
+
 setup(
     name="ncbimetadata",
-    version="0.0.8",
+    version="0.0.9",
     description="ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!",
     long_description=readfile('README.md'),
     long_description_content_type='text/markdown',
     author="Ryan Alloriadonis",
     author_email="yuantai78@gmail.com",
     url="https://github.com/RyanYuanSun/ncbimetadata",
     platforms=['Linux', 'MacOS X'],
     py_modules=['ncbimetadata'],
     packages=['ncbimetadata'],
     license=readfile('LICENSE'),
-    scripts=['bin/ncbimetadata'],
+    scripts=[script],
     install_requires=[
           'requests',
       ],
     zip_safe=False
 )
```

