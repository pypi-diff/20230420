# Comparing `tmp/ncbimetadata-0.0.6.tar.gz` & `tmp/ncbimetadata-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbimetadata-0.0.6.tar", last modified: Thu Apr 20 09:17:15 2023, max compression
+gzip compressed data, was "ncbimetadata-0.0.7.tar", last modified: Thu Apr 20 09:29:35 2023, max compression
```

## Comparing `ncbimetadata-0.0.6.tar` & `ncbimetadata-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:17:15.476474 ncbimetadata-0.0.6/
--rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.0.6/LICENSE
--rw-r--r--   0 taiyuan    (501) staff       (20)     3049 2023-04-20 09:17:15.476355 ncbimetadata-0.0.6/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.0.6/README.md
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:17:15.474877 ncbimetadata-0.0.6/bin/
--rw-r--r--   0 taiyuan    (501) staff       (20)      152 2023-04-20 08:50:52.000000 ncbimetadata-0.0.6/bin/ncbimetadata
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:17:15.475211 ncbimetadata-0.0.6/ncbimetadata/
--rw-r--r--   0 taiyuan    (501) staff       (20)    11112 2023-04-20 08:02:11.000000 ncbimetadata-0.0.6/ncbimetadata/__init__.py
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:17:15.476111 ncbimetadata-0.0.6/ncbimetadata.egg-info/
--rw-r--r--   0 taiyuan    (501) staff       (20)     3049 2023-04-20 09:17:15.000000 ncbimetadata-0.0.6/ncbimetadata.egg-info/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)      282 2023-04-20 09:17:15.000000 ncbimetadata-0.0.6/ncbimetadata.egg-info/SOURCES.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 09:17:15.000000 ncbimetadata-0.0.6/ncbimetadata.egg-info/dependency_links.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 09:17:15.000000 ncbimetadata-0.0.6/ncbimetadata.egg-info/not-zip-safe
--rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 09:17:15.000000 ncbimetadata-0.0.6/ncbimetadata.egg-info/requires.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 09:17:15.000000 ncbimetadata-0.0.6/ncbimetadata.egg-info/top_level.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 09:17:15.476527 ncbimetadata-0.0.6/setup.cfg
--rw-r--r--   0 taiyuan    (501) staff       (20)      750 2023-04-20 09:16:45.000000 ncbimetadata-0.0.6/setup.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:29:35.191340 ncbimetadata-0.0.7/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.0.7/LICENSE
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3041 2023-04-20 09:29:35.191226 ncbimetadata-0.0.7/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.0.7/README.md
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:29:35.189670 ncbimetadata-0.0.7/bin/
+-rw-r--r--   0 taiyuan    (501) staff       (20)      152 2023-04-20 08:50:52.000000 ncbimetadata-0.0.7/bin/ncbimetadata
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:29:35.190011 ncbimetadata-0.0.7/ncbimetadata/
+-rw-r--r--   0 taiyuan    (501) staff       (20)    11112 2023-04-20 08:02:11.000000 ncbimetadata-0.0.7/ncbimetadata/__init__.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:29:35.191064 ncbimetadata-0.0.7/ncbimetadata.egg-info/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3041 2023-04-20 09:29:35.000000 ncbimetadata-0.0.7/ncbimetadata.egg-info/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)      282 2023-04-20 09:29:35.000000 ncbimetadata-0.0.7/ncbimetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 09:29:35.000000 ncbimetadata-0.0.7/ncbimetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 09:29:35.000000 ncbimetadata-0.0.7/ncbimetadata.egg-info/not-zip-safe
+-rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 09:29:35.000000 ncbimetadata-0.0.7/ncbimetadata.egg-info/requires.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 09:29:35.000000 ncbimetadata-0.0.7/ncbimetadata.egg-info/top_level.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 09:29:35.191383 ncbimetadata-0.0.7/setup.cfg
+-rw-r--r--   0 taiyuan    (501) staff       (20)      742 2023-04-20 09:29:19.000000 ncbimetadata-0.0.7/setup.py
```

### Comparing `ncbimetadata-0.0.6/LICENSE` & `ncbimetadata-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.6/PKG-INFO` & `ncbimetadata-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.0.6
+Version: 0.0.7
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
-Home-page: https://github.com/RyanYuanSun/ncbi_metadata_parser
+Home-page: https://github.com/RyanYuanSun/ncbimetadata
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ncbimetadata-0.0.6/README.md` & `ncbimetadata-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.6/ncbimetadata/__init__.py` & `ncbimetadata-0.0.7/ncbimetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.6/ncbimetadata.egg-info/PKG-INFO` & `ncbimetadata-0.0.7/ncbimetadata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.0.6
+Version: 0.0.7
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
-Home-page: https://github.com/RyanYuanSun/ncbi_metadata_parser
+Home-page: https://github.com/RyanYuanSun/ncbimetadata
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ncbimetadata-0.0.6/setup.py` & `ncbimetadata-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 def readfile(filename):
     with open(filename, 'r+') as f:
         return f.read()
 
 
 setup(
     name="ncbimetadata",
-    version="0.0.6",
+    version="0.0.7",
     description="ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!",
     long_description=readfile('README.md'),
     long_description_content_type='text/markdown',
     author="Ryan Alloriadonis",
     author_email="yuantai78@gmail.com",
-    url="https://github.com/RyanYuanSun/ncbi_metadata_parser",
+    url="https://github.com/RyanYuanSun/ncbimetadata",
     py_modules=['ncbimetadata'],
     packages=['ncbimetadata'],
     license=readfile('LICENSE'),
     scripts=['bin/ncbimetadata'],
     install_requires=[
           'requests',
       ],
```

