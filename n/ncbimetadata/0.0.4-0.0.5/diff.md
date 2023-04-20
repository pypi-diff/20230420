# Comparing `tmp/ncbimetadata-0.0.4.tar.gz` & `tmp/ncbimetadata-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbimetadata-0.0.4.tar", last modified: Thu Apr 20 08:51:41 2023, max compression
+gzip compressed data, was "ncbimetadata-0.0.5.tar", last modified: Thu Apr 20 09:08:10 2023, max compression
```

## Comparing `ncbimetadata-0.0.4.tar` & `ncbimetadata-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 08:51:41.054423 ncbimetadata-0.0.4/
--rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.0.4/LICENSE
--rw-r--r--   0 taiyuan    (501) staff       (20)     3049 2023-04-20 08:51:41.054302 ncbimetadata-0.0.4/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.0.4/README.md
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 08:51:41.053115 ncbimetadata-0.0.4/bin/
--rw-r--r--   0 taiyuan    (501) staff       (20)      152 2023-04-20 08:50:52.000000 ncbimetadata-0.0.4/bin/ncbimetadata
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 08:51:41.054112 ncbimetadata-0.0.4/ncbimetadata.egg-info/
--rw-r--r--   0 taiyuan    (501) staff       (20)     3049 2023-04-20 08:51:41.000000 ncbimetadata-0.0.4/ncbimetadata.egg-info/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)      257 2023-04-20 08:51:41.000000 ncbimetadata-0.0.4/ncbimetadata.egg-info/SOURCES.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 08:51:41.000000 ncbimetadata-0.0.4/ncbimetadata.egg-info/dependency_links.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 08:51:40.000000 ncbimetadata-0.0.4/ncbimetadata.egg-info/not-zip-safe
--rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 08:51:41.000000 ncbimetadata-0.0.4/ncbimetadata.egg-info/requires.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 08:51:41.000000 ncbimetadata-0.0.4/ncbimetadata.egg-info/top_level.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 08:51:41.054467 ncbimetadata-0.0.4/setup.cfg
--rw-r--r--   0 taiyuan    (501) staff       (20)      719 2023-04-20 08:51:30.000000 ncbimetadata-0.0.4/setup.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:08:10.055548 ncbimetadata-0.0.5/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.0.5/LICENSE
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3049 2023-04-20 09:08:10.055428 ncbimetadata-0.0.5/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.0.5/README.md
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:08:10.054167 ncbimetadata-0.0.5/bin/
+-rw-r--r--   0 taiyuan    (501) staff       (20)      152 2023-04-20 08:50:52.000000 ncbimetadata-0.0.5/bin/ncbimetadata
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:08:10.055247 ncbimetadata-0.0.5/ncbimetadata.egg-info/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3049 2023-04-20 09:08:10.000000 ncbimetadata-0.0.5/ncbimetadata.egg-info/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)      257 2023-04-20 09:08:10.000000 ncbimetadata-0.0.5/ncbimetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 09:08:10.000000 ncbimetadata-0.0.5/ncbimetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 09:08:09.000000 ncbimetadata-0.0.5/ncbimetadata.egg-info/not-zip-safe
+-rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 09:08:10.000000 ncbimetadata-0.0.5/ncbimetadata.egg-info/requires.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 09:08:10.000000 ncbimetadata-0.0.5/ncbimetadata.egg-info/top_level.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 09:08:10.055637 ncbimetadata-0.0.5/setup.cfg
+-rw-r--r--   0 taiyuan    (501) staff       (20)      719 2023-04-20 09:08:03.000000 ncbimetadata-0.0.5/setup.py
```

### Comparing `ncbimetadata-0.0.4/LICENSE` & `ncbimetadata-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.4/PKG-INFO` & `ncbimetadata-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.0.4
+Version: 0.0.5
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbi_metadata_parser
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
```

### Comparing `ncbimetadata-0.0.4/README.md` & `ncbimetadata-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.4/ncbimetadata.egg-info/PKG-INFO` & `ncbimetadata-0.0.5/ncbimetadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.0.4
+Version: 0.0.5
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbi_metadata_parser
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
```

### Comparing `ncbimetadata-0.0.4/setup.py` & `ncbimetadata-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readfile(filename):
     with open(filename, 'r+') as f:
         return f.read()
 
 
 setup(
     name="ncbimetadata",
-    version="0.0.4",
+    version="0.0.5",
     description="ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!",
     long_description=readfile('README.md'),
     long_description_content_type='text/markdown',
     author="Ryan Alloriadonis",
     author_email="yuantai78@gmail.com",
     url="https://github.com/RyanYuanSun/ncbi_metadata_parser",
     py_modules=['ncbimetadata'],
```

