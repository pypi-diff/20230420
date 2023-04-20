# Comparing `tmp/smc-go-0.0.0.tar.gz` & `tmp/smc-go-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smc-go-0.0.0.tar", last modified: Thu Apr 20 10:10:45 2023, max compression
+gzip compressed data, was "smc-go-1.0.0.tar", last modified: Mon Mar 13 09:34:55 2023, max compression
```

## Comparing `smc-go-0.0.0.tar` & `smc-go-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 ruijuan.fu   (503) staff       (20)        0 2023-04-20 10:10:45.725458 smc-go-0.0.0/
--rw-r--r--   0 ruijuan.fu   (503) staff       (20)      752 2023-04-20 10:10:45.725228 smc-go-0.0.0/PKG-INFO
--rwxr-xr-x   0 ruijuan.fu   (503) staff       (20)        6 2023-04-20 10:10:45.000000 smc-go-0.0.0/README.md
--rw-r--r--   0 ruijuan.fu   (503) staff       (20)       38 2023-04-20 10:10:45.725532 smc-go-0.0.0/setup.cfg
--rwxr-xr-x   0 ruijuan.fu   (503) staff       (20)     1074 2023-04-20 10:10:45.000000 smc-go-0.0.0/setup.py
-drwxr-xr-x   0 ruijuan.fu   (503) staff       (20)        0 2023-04-20 10:10:45.724921 smc-go-0.0.0/smc_go.egg-info/
--rw-r--r--   0 ruijuan.fu   (503) staff       (20)      752 2023-04-20 10:10:45.000000 smc-go-0.0.0/smc_go.egg-info/PKG-INFO
--rw-r--r--   0 ruijuan.fu   (503) staff       (20)      138 2023-04-20 10:10:45.000000 smc-go-0.0.0/smc_go.egg-info/SOURCES.txt
--rw-r--r--   0 ruijuan.fu   (503) staff       (20)        1 2023-04-20 10:10:45.000000 smc-go-0.0.0/smc_go.egg-info/dependency_links.txt
--rw-r--r--   0 ruijuan.fu   (503) staff       (20)        1 2023-04-20 10:10:45.000000 smc-go-0.0.0/smc_go.egg-info/top_level.txt
+drwxr-xr-x   0 ruijuan.fu   (503) staff       (20)        0 2023-03-13 09:34:55.050346 smc-go-1.0.0/
+-rw-r--r--   0 ruijuan.fu   (503) staff       (20)      752 2023-03-13 09:34:55.050038 smc-go-1.0.0/PKG-INFO
+-rwxr-xr-x   0 ruijuan.fu   (503) staff       (20)        6 2023-03-13 09:34:54.000000 smc-go-1.0.0/README.md
+-rw-r--r--   0 ruijuan.fu   (503) staff       (20)       38 2023-03-13 09:34:55.050463 smc-go-1.0.0/setup.cfg
+-rwxr-xr-x   0 ruijuan.fu   (503) staff       (20)     1074 2023-03-13 09:34:54.000000 smc-go-1.0.0/setup.py
+drwxr-xr-x   0 ruijuan.fu   (503) staff       (20)        0 2023-03-13 09:34:55.049566 smc-go-1.0.0/smc_go.egg-info/
+-rw-r--r--   0 ruijuan.fu   (503) staff       (20)      752 2023-03-13 09:34:54.000000 smc-go-1.0.0/smc_go.egg-info/PKG-INFO
+-rw-r--r--   0 ruijuan.fu   (503) staff       (20)      138 2023-03-13 09:34:55.000000 smc-go-1.0.0/smc_go.egg-info/SOURCES.txt
+-rw-r--r--   0 ruijuan.fu   (503) staff       (20)        1 2023-03-13 09:34:54.000000 smc-go-1.0.0/smc_go.egg-info/dependency_links.txt
+-rw-r--r--   0 ruijuan.fu   (503) staff       (20)        1 2023-03-13 09:34:54.000000 smc-go-1.0.0/smc_go.egg-info/top_level.txt
```

### Comparing `smc-go-0.0.0/PKG-INFO` & `smc-go-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smc-go
-Version: 0.0.0
+Version: 1.0.0
 Summary: A small example package
 Home-page: 
 Author: sc
 Author-email: 
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `smc-go-0.0.0/setup.py` & `smc-go-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.md", "r") as f:
   long_description = f.read()
 
 setup(name='smc-go',  
-      version='0.0.0',  
+      version='1.0.0',  
       description='A small example package',
       long_description=long_description,
       author='sc',
       author_email='',
       url='',
       install_requires=[],
       license='BSD License',
```

### Comparing `smc-go-0.0.0/smc_go.egg-info/PKG-INFO` & `smc-go-1.0.0/smc_go.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smc-go
-Version: 0.0.0
+Version: 1.0.0
 Summary: A small example package
 Home-page: 
 Author: sc
 Author-email: 
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

