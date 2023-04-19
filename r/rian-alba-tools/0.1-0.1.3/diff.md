# Comparing `tmp/rian-alba-tools-0.1.tar.gz` & `tmp/rian-alba-tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rian-alba-tools-0.1.tar", last modified: Wed Apr 19 21:59:25 2023, max compression
+gzip compressed data, was "rian-alba-tools-0.1.3.tar", last modified: Wed Apr 19 23:19:01 2023, max compression
```

## Comparing `rian-alba-tools-0.1.tar` & `rian-alba-tools-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 21:59:25.191069 rian-alba-tools-0.1/
--rw-rw-rw-   0        0        0     1089 2023-04-19 21:58:09.000000 rian-alba-tools-0.1/LICENSE
--rw-rw-rw-   0        0        0      199 2023-04-19 21:59:25.173266 rian-alba-tools-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      114 2023-04-19 21:58:10.000000 rian-alba-tools-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 21:59:25.137080 rian-alba-tools-0.1/rian_alba_tools.egg-info/
--rw-rw-rw-   0        0        0      199 2023-04-19 21:59:21.000000 rian-alba-tools-0.1/rian_alba_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-19 21:59:23.000000 rian-alba-tools-0.1/rian_alba_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 21:59:21.000000 rian-alba-tools-0.1/rian_alba_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2023-04-19 21:59:21.000000 rian-alba-tools-0.1/rian_alba_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 21:59:21.000000 rian-alba-tools-0.1/rian_alba_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 21:59:25.194070 rian-alba-tools-0.1/setup.cfg
--rw-rw-rw-   0        0        0      630 2023-04-19 21:58:11.000000 rian-alba-tools-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 23:19:01.260689 rian-alba-tools-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-19 21:58:09.000000 rian-alba-tools-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      201 2023-04-19 23:19:01.231689 rian-alba-tools-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2023-04-19 21:58:10.000000 rian-alba-tools-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 23:19:01.154883 rian-alba-tools-0.1.3/rian_alba_tools.egg-info/
+-rw-rw-rw-   0        0        0      201 2023-04-19 23:18:55.000000 rian-alba-tools-0.1.3/rian_alba_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-04-19 23:18:59.000000 rian-alba-tools-0.1.3/rian_alba_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 23:18:55.000000 rian-alba-tools-0.1.3/rian_alba_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-04-19 23:18:55.000000 rian-alba-tools-0.1.3/rian_alba_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 23:18:55.000000 rian-alba-tools-0.1.3/rian_alba_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 23:19:01.262689 rian-alba-tools-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      632 2023-04-19 23:17:41.000000 rian-alba-tools-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 23:19:01.212650 rian-alba-tools-0.1.3/utils/
+-rw-rw-rw-   0        0        0       43 2023-04-19 22:53:40.000000 rian-alba-tools-0.1.3/utils/__init__.py
+-rw-rw-rw-   0        0        0      290 2023-04-19 22:52:07.000000 rian-alba-tools-0.1.3/utils/test.py
```

### Comparing `rian-alba-tools-0.1/LICENSE` & `rian-alba-tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rian-alba-tools-0.1/setup.py` & `rian-alba-tools-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rian-alba-tools',
-    version='0.1',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'nilearn',
         'numpy',
         'openpyxl',
         'pandas',
```

