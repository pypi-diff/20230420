# Comparing `tmp/exampleData-5.0.tar.gz` & `tmp/exampleData-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exampleData-5.0.tar", last modified: Thu Apr 20 09:13:45 2023, max compression
+gzip compressed data, was "exampleData-6.0.tar", last modified: Thu Apr 20 09:16:35 2023, max compression
```

## Comparing `exampleData-5.0.tar` & `exampleData-6.0.tar`

### file list

```diff
@@ -1,13 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 09:13:45.477304 exampleData-5.0/
--rw-rw-rw-   0        0        0      300 2023-04-20 09:13:45.477304 exampleData-5.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-20 09:13:45.468008 exampleData-5.0/exampleData/
--rw-rw-rw-   0        0        0      163 2023-04-20 09:07:09.000000 exampleData-5.0/exampleData/__init__.py
--rw-rw-rw-   0        0        0     2395 2023-04-16 02:11:42.000000 exampleData-5.0/exampleData/getdata.py
-drwxrwxrwx   0        0        0        0 2023-04-20 09:13:45.476088 exampleData-5.0/exampleData.egg-info/
--rw-rw-rw-   0        0        0      300 2023-04-20 09:13:45.000000 exampleData-5.0/exampleData.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-04-20 09:13:45.000000 exampleData-5.0/exampleData.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 09:13:45.000000 exampleData-5.0/exampleData.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-20 09:13:45.000000 exampleData-5.0/exampleData.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 09:13:45.000000 exampleData-5.0/exampleData.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 09:13:45.477304 exampleData-5.0/setup.cfg
--rw-rw-rw-   0        0        0      526 2023-04-20 09:13:15.000000 exampleData-5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:16:35.034485 exampleData-6.0/
+-rw-rw-rw-   0        0        0      300 2023-04-20 09:16:35.034485 exampleData-6.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-20 09:16:35.033484 exampleData-6.0/exampleData.egg-info/
+-rw-rw-rw-   0        0        0      300 2023-04-20 09:16:34.000000 exampleData-6.0/exampleData.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-20 09:16:34.000000 exampleData-6.0/exampleData.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 09:16:34.000000 exampleData-6.0/exampleData.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-20 09:16:34.000000 exampleData-6.0/exampleData.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 09:16:34.000000 exampleData-6.0/exampleData.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 09:16:35.034485 exampleData-6.0/setup.cfg
+-rw-rw-rw-   0        0        0      526 2023-04-20 09:16:28.000000 exampleData-6.0/setup.py
```

### Comparing `exampleData-5.0/setup.py` & `exampleData-6.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="exampleData",
-    version="5.0",
+    version="6.0",
     packages=find_packages(include='exampleData'),
     install_requires=[
         "numpy",
         "requests"
     ],
     author="NCQH",
     author_email="ncquochuy21@gmail.com",
```

