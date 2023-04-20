# Comparing `tmp/ncbimetadata-0.0.2.tar.gz` & `tmp/ncbimetadata-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbimetadata-0.0.2.tar", last modified: Thu Apr 20 08:31:30 2023, max compression
+gzip compressed data, was "ncbimetadata-0.0.3.tar", last modified: Thu Apr 20 08:39:48 2023, max compression
```

## Comparing `ncbimetadata-0.0.2.tar` & `ncbimetadata-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 08:31:30.168891 ncbimetadata-0.0.2/
--rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.0.2/LICENSE
--rw-r--r--   0 taiyuan    (501) staff       (20)     3049 2023-04-20 08:31:30.168776 ncbimetadata-0.0.2/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.0.2/README.md
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 08:31:30.167470 ncbimetadata-0.0.2/bin/
--rw-r--r--   0 taiyuan    (501) staff       (20)      152 2023-04-20 07:52:12.000000 ncbimetadata-0.0.2/bin/ncbimetadata
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 08:31:30.168600 ncbimetadata-0.0.2/ncbimetadata.egg-info/
--rw-r--r--   0 taiyuan    (501) staff       (20)     3049 2023-04-20 08:31:30.000000 ncbimetadata-0.0.2/ncbimetadata.egg-info/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)      257 2023-04-20 08:31:30.000000 ncbimetadata-0.0.2/ncbimetadata.egg-info/SOURCES.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 08:31:30.000000 ncbimetadata-0.0.2/ncbimetadata.egg-info/dependency_links.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 08:18:37.000000 ncbimetadata-0.0.2/ncbimetadata.egg-info/not-zip-safe
--rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 08:31:30.000000 ncbimetadata-0.0.2/ncbimetadata.egg-info/requires.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 08:31:30.000000 ncbimetadata-0.0.2/ncbimetadata.egg-info/top_level.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 08:31:30.168934 ncbimetadata-0.0.2/setup.cfg
--rw-r--r--   0 taiyuan    (501) staff       (20)      719 2023-04-20 08:31:22.000000 ncbimetadata-0.0.2/setup.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 08:39:48.302685 ncbimetadata-0.0.3/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.0.3/LICENSE
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3049 2023-04-20 08:39:48.302557 ncbimetadata-0.0.3/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.0.3/README.md
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 08:39:48.301306 ncbimetadata-0.0.3/bin/
+-rw-r--r--   0 taiyuan    (501) staff       (20)      153 2023-04-20 08:39:38.000000 ncbimetadata-0.0.3/bin/ncbimetadata
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 08:39:48.302352 ncbimetadata-0.0.3/ncbimetadata.egg-info/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3049 2023-04-20 08:39:48.000000 ncbimetadata-0.0.3/ncbimetadata.egg-info/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)      257 2023-04-20 08:39:48.000000 ncbimetadata-0.0.3/ncbimetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 08:39:48.000000 ncbimetadata-0.0.3/ncbimetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 08:37:36.000000 ncbimetadata-0.0.3/ncbimetadata.egg-info/not-zip-safe
+-rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 08:39:48.000000 ncbimetadata-0.0.3/ncbimetadata.egg-info/requires.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 08:39:48.000000 ncbimetadata-0.0.3/ncbimetadata.egg-info/top_level.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 08:39:48.302730 ncbimetadata-0.0.3/setup.cfg
+-rw-r--r--   0 taiyuan    (501) staff       (20)      719 2023-04-20 08:37:08.000000 ncbimetadata-0.0.3/setup.py
```

### Comparing `ncbimetadata-0.0.2/LICENSE` & `ncbimetadata-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.2/PKG-INFO` & `ncbimetadata-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.0.2
+Version: 0.0.3
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbi_metadata_parser
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
```

### Comparing `ncbimetadata-0.0.2/README.md` & `ncbimetadata-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.2/ncbimetadata.egg-info/PKG-INFO` & `ncbimetadata-0.0.3/ncbimetadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.0.2
+Version: 0.0.3
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbi_metadata_parser
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
```

### Comparing `ncbimetadata-0.0.2/setup.py` & `ncbimetadata-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readfile(filename):
     with open(filename, 'r+') as f:
         return f.read()
 
 
 setup(
     name="ncbimetadata",
-    version="0.0.2",
+    version="0.0.3",
     description="ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!",
     long_description=readfile('README.md'),
     long_description_content_type='text/markdown',
     author="Ryan Alloriadonis",
     author_email="yuantai78@gmail.com",
     url="https://github.com/RyanYuanSun/ncbi_metadata_parser",
     py_modules=['ncbimetadata'],
```

