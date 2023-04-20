# Comparing `tmp/pdpp-bhi-0.0.3.tar.gz` & `tmp/pdpp-bhi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdpp-bhi-0.0.3.tar", last modified: Thu Apr 20 15:46:02 2023, max compression
+gzip compressed data, was "pdpp-bhi-0.0.4.tar", last modified: Thu Apr 20 15:49:27 2023, max compression
```

## Comparing `pdpp-bhi-0.0.3.tar` & `pdpp-bhi-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:46:02.437893 pdpp-bhi-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 15:46:02.437893 pdpp-bhi-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 15:45:40.000000 pdpp-bhi-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:46:02.437893 pdpp-bhi-0.0.3/pdpp_bhi/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 15:45:40.000000 pdpp-bhi-0.0.3/pdpp_bhi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-04-20 15:45:40.000000 pdpp-bhi-0.0.3/pdpp_bhi/pdpp_bhi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:46:02.437893 pdpp-bhi-0.0.3/pdpp_bhi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 15:46:02.000000 pdpp-bhi-0.0.3/pdpp_bhi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-20 15:46:02.000000 pdpp-bhi-0.0.3/pdpp_bhi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:46:02.000000 pdpp-bhi-0.0.3/pdpp_bhi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 15:46:02.000000 pdpp-bhi-0.0.3/pdpp_bhi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 15:46:02.000000 pdpp-bhi-0.0.3/pdpp_bhi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:46:02.437893 pdpp-bhi-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-20 15:45:40.000000 pdpp-bhi-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:49:27.796075 pdpp-bhi-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 15:49:27.796075 pdpp-bhi-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 15:49:16.000000 pdpp-bhi-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:49:27.796075 pdpp-bhi-0.0.4/pdpp_bhi/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:49:16.000000 pdpp-bhi-0.0.4/pdpp_bhi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-04-20 15:49:16.000000 pdpp-bhi-0.0.4/pdpp_bhi/pdpp_bhi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:49:27.796075 pdpp-bhi-0.0.4/pdpp_bhi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 15:49:27.000000 pdpp-bhi-0.0.4/pdpp_bhi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-20 15:49:27.000000 pdpp-bhi-0.0.4/pdpp_bhi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:49:27.000000 pdpp-bhi-0.0.4/pdpp_bhi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 15:49:27.000000 pdpp-bhi-0.0.4/pdpp_bhi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 15:49:27.000000 pdpp-bhi-0.0.4/pdpp_bhi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:49:27.796075 pdpp-bhi-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-20 15:49:16.000000 pdpp-bhi-0.0.4/setup.py
```

### Comparing `pdpp-bhi-0.0.3/pdpp_bhi/pdpp_bhi.py` & `pdpp-bhi-0.0.4/pdpp_bhi/pdpp_bhi.py`

 * *Files identical despite different names*

### Comparing `pdpp-bhi-0.0.3/setup.py` & `pdpp-bhi-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pdpp-bhi",
     packages=find_packages(exclude=[]),
     include_package_data=True,
-    version="0.0.3",
+    version="0.0.4",
     license="MIT",
     description="PDPP - BHI",
     author="Dohoon Lee",
     author_email="dohlee.bioinfo@gmail.com",
     long_description_content_type="text/markdown",
     url="https://github.com/dohlee/pdpp",
     keywords=[
```

