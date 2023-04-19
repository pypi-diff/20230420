# Comparing `tmp/rian-alba-tools-0.1.tar.gz` & `tmp/rian-alba-tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rian-alba-tools-0.1.tar", last modified: Wed Apr 19 21:59:25 2023, max compression
+gzip compressed data, was "rian-alba-tools-0.1.1.tar", last modified: Wed Apr 19 22:47:17 2023, max compression
```

## Comparing `rian-alba-tools-0.1.tar` & `rian-alba-tools-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
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
+drwxrwxrwx   0        0        0        0 2023-04-19 22:47:17.142530 rian-alba-tools-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2023-04-19 21:58:09.000000 rian-alba-tools-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      201 2023-04-19 22:47:17.123530 rian-alba-tools-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2023-04-19 21:58:10.000000 rian-alba-tools-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 22:47:17.095370 rian-alba-tools-0.1.1/rian_alba_tools.egg-info/
+-rw-rw-rw-   0        0        0      201 2023-04-19 22:47:14.000000 rian-alba-tools-0.1.1/rian_alba_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-04-19 22:47:15.000000 rian-alba-tools-0.1.1/rian_alba_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 22:47:14.000000 rian-alba-tools-0.1.1/rian_alba_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-04-19 22:47:14.000000 rian-alba-tools-0.1.1/rian_alba_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 22:47:14.000000 rian-alba-tools-0.1.1/rian_alba_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 22:47:17.144530 rian-alba-tools-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      632 2023-04-19 22:44:49.000000 rian-alba-tools-0.1.1/setup.py
```

### Comparing `rian-alba-tools-0.1/LICENSE` & `rian-alba-tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rian-alba-tools-0.1/setup.py` & `rian-alba-tools-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rian-alba-tools',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'nilearn',
         'numpy',
         'openpyxl',
         'pandas',
```

