# Comparing `tmp/exampleData-8.0.tar.gz` & `tmp/exampleData-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exampleData-8.0.tar", last modified: Thu Apr 20 09:38:53 2023, max compression
+gzip compressed data, was "exampleData-9.0.tar", last modified: Thu Apr 20 09:40:01 2023, max compression
```

## Comparing `exampleData-8.0.tar` & `exampleData-9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 09:38:53.364677 exampleData-8.0/
--rw-rw-rw-   0        0        0      300 2023-04-20 09:38:53.358233 exampleData-8.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-20 09:38:53.347018 exampleData-8.0/exampleData/
--rw-rw-rw-   0        0        0      175 2023-04-20 09:38:32.000000 exampleData-8.0/exampleData/__init__.py
--rw-rw-rw-   0        0        0     2395 2023-04-16 02:11:42.000000 exampleData-8.0/exampleData/getdata.py
-drwxrwxrwx   0        0        0        0 2023-04-20 09:38:53.357231 exampleData-8.0/exampleData.egg-info/
--rw-rw-rw-   0        0        0      300 2023-04-20 09:38:53.000000 exampleData-8.0/exampleData.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-04-20 09:38:53.000000 exampleData-8.0/exampleData.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 09:38:53.000000 exampleData-8.0/exampleData.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-20 09:38:53.000000 exampleData-8.0/exampleData.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-20 09:38:53.000000 exampleData-8.0/exampleData.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 09:38:53.364677 exampleData-8.0/setup.cfg
--rw-rw-rw-   0        0        0      535 2023-04-20 09:38:43.000000 exampleData-8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:40:01.953347 exampleData-9.0/
+-rw-rw-rw-   0        0        0      300 2023-04-20 09:40:01.952345 exampleData-9.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-20 09:40:01.936879 exampleData-9.0/exampleData/
+-rw-rw-rw-   0        0        0       33 2023-04-20 09:39:34.000000 exampleData-9.0/exampleData/__init__.py
+-rw-rw-rw-   0        0        0     2395 2023-04-16 02:11:42.000000 exampleData-9.0/exampleData/getdata.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:40:01.952345 exampleData-9.0/exampleData.egg-info/
+-rw-rw-rw-   0        0        0      300 2023-04-20 09:40:01.000000 exampleData-9.0/exampleData.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-04-20 09:40:01.000000 exampleData-9.0/exampleData.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 09:40:01.000000 exampleData-9.0/exampleData.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-20 09:40:01.000000 exampleData-9.0/exampleData.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 09:40:01.000000 exampleData-9.0/exampleData.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 09:40:01.953347 exampleData-9.0/setup.cfg
+-rw-rw-rw-   0        0        0      535 2023-04-20 09:39:41.000000 exampleData-9.0/setup.py
```

### Comparing `exampleData-8.0/exampleData/getdata.py` & `exampleData-9.0/exampleData/getdata.py`

 * *Files identical despite different names*

### Comparing `exampleData-8.0/setup.py` & `exampleData-9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="exampleData",
-    version="8.0",
+    version="9.0",
     packages=find_packages(include=['*', 'exampleData.*']),
     install_requires=[
         "numpy",
         "requests"
     ],
     author="NCQH",
     author_email="ncquochuy21@gmail.com",
```

