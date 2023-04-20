# Comparing `tmp/pymathematics-2023.4.20.tar.gz` & `tmp/pymathematics-2023.4.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.20.tar", last modified: Thu Apr 20 13:13:23 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.20.1.tar", last modified: Thu Apr 20 13:27:44 2023, max compression
```

## Comparing `pymathematics-2023.4.20.tar` & `pymathematics-2023.4.20.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-20 13:13:22.946279 pymathematics-2023.4.20/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.20/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-20 13:13:22.899279 pymathematics-2023.4.20/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      118 2023-04-20 13:03:45.000000 pymathematics-2023.4.20/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-20 13:13:22.562279 pymathematics-2023.4.20/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    15030 2023-04-20 13:00:09.000000 pymathematics-2023.4.20/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-20 13:02:21.000000 pymathematics-2023.4.20/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-20 13:13:22.809277 pymathematics-2023.4.20/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-20 13:13:19.000000 pymathematics-2023.4.20/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-20 13:13:19.000000 pymathematics-2023.4.20/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-20 13:13:19.000000 pymathematics-2023.4.20/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-20 13:13:19.000000 pymathematics-2023.4.20/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-20 13:13:22.950282 pymathematics-2023.4.20/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-20 13:02:30.000000 pymathematics-2023.4.20/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-20 13:27:44.284042 pymathematics-2023.4.20.1/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.20.1/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-20 13:27:44.275037 pymathematics-2023.4.20.1/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      120 2023-04-20 13:23:25.000000 pymathematics-2023.4.20.1/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-20 13:27:44.045541 pymathematics-2023.4.20.1/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    15044 2023-04-20 13:23:01.000000 pymathematics-2023.4.20.1/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      113 2023-04-20 13:23:07.000000 pymathematics-2023.4.20.1/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-20 13:27:44.225534 pymathematics-2023.4.20.1/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-20 13:27:43.000000 pymathematics-2023.4.20.1/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-20 13:27:43.000000 pymathematics-2023.4.20.1/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-20 13:27:43.000000 pymathematics-2023.4.20.1/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-20 13:27:43.000000 pymathematics-2023.4.20.1/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-20 13:27:44.287043 pymathematics-2023.4.20.1/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      691 2023-04-20 13:23:20.000000 pymathematics-2023.4.20.1/setup.py
```

### Comparing `pymathematics-2023.4.20/LICENSE` & `pymathematics-2023.4.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.20/pymathematics/__init__.py` & `pymathematics-2023.4.20.1/pymathematics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# from .info import (
-#     author,version,homepage
-# )
+from .info import (
+    author,version,homepage
+)
 
-# author = author
-# version = version
-# homepage = homepage
+class about:
+    author = author
+    version = version
+    homepage = homepage
 
 class constants:
     pi = 3.1415926535897932384626433832795
     e = 2.7182818284590452353602874713527
 
 class vector:
     def cross_product(vector1:list,vector2:list) -> int|float:
```

### Comparing `pymathematics-2023.4.20/setup.py` & `pymathematics-2023.4.20.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.20",
+    version = "2023.4.20.1",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

