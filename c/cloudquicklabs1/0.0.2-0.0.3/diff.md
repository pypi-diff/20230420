# Comparing `tmp/cloudquicklabs1-0.0.2.tar.gz` & `tmp/cloudquicklabs1-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudquicklabs1-0.0.2.tar", last modified: Thu Apr 20 03:24:12 2023, max compression
+gzip compressed data, was "cloudquicklabs1-0.0.3.tar", last modified: Thu Apr 20 03:33:56 2023, max compression
```

## Comparing `cloudquicklabs1-0.0.2.tar` & `cloudquicklabs1-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:24:12.574392 cloudquicklabs1-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 03:24:12.574392 cloudquicklabs1-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 03:24:06.000000 cloudquicklabs1-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:24:12.574392 cloudquicklabs1-0.0.2/cloudquicklabs1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 03:24:12.000000 cloudquicklabs1-0.0.2/cloudquicklabs1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-20 03:24:12.000000 cloudquicklabs1-0.0.2/cloudquicklabs1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 03:24:12.000000 cloudquicklabs1-0.0.2/cloudquicklabs1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 03:24:12.000000 cloudquicklabs1-0.0.2/cloudquicklabs1.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 03:24:12.000000 cloudquicklabs1-0.0.2/cloudquicklabs1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 03:24:12.000000 cloudquicklabs1-0.0.2/cloudquicklabs1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 03:24:12.574392 cloudquicklabs1-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-20 03:24:06.000000 cloudquicklabs1-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:24:12.574392 cloudquicklabs1-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:24:06.000000 cloudquicklabs1-0.0.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-20 03:24:06.000000 cloudquicklabs1-0.0.2/src/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-20 03:24:06.000000 cloudquicklabs1-0.0.2/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:33:56.709084 cloudquicklabs1-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 03:33:56.709084 cloudquicklabs1-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 03:33:50.000000 cloudquicklabs1-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:33:56.709084 cloudquicklabs1-0.0.3/cloudquicklabs1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 03:33:56.000000 cloudquicklabs1-0.0.3/cloudquicklabs1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-20 03:33:56.000000 cloudquicklabs1-0.0.3/cloudquicklabs1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 03:33:56.000000 cloudquicklabs1-0.0.3/cloudquicklabs1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 03:33:56.000000 cloudquicklabs1-0.0.3/cloudquicklabs1.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 03:33:56.000000 cloudquicklabs1-0.0.3/cloudquicklabs1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 03:33:56.000000 cloudquicklabs1-0.0.3/cloudquicklabs1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 03:33:56.709084 cloudquicklabs1-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-20 03:33:50.000000 cloudquicklabs1-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:33:56.709084 cloudquicklabs1-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 03:33:50.000000 cloudquicklabs1-0.0.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-20 03:33:50.000000 cloudquicklabs1-0.0.3/src/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-20 03:33:50.000000 cloudquicklabs1-0.0.3/src/main.py
```

### Comparing `cloudquicklabs1-0.0.2/setup.py` & `cloudquicklabs1-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cloudquicklabs1",
-    version="0.0.2",
+    version="0.0.3",
     author="Rekhu Chinnarathod",
     author_email="vrchinnarathod@gmail.com",
     url="https://www.youtube.com/channel/UCv9MUffHWyo2GgLIDLVu0KQ",
     description="An application that informs you of the time in different locations and timezones",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=["click", "pytz"],
-    entry_points={"console_scripts": ["timechecker = src.main:main"]},
+    entry_points={"console_scripts": ["cloudquicklabs1 = src.main:main"]},
 )
```

### Comparing `cloudquicklabs1-0.0.2/src/logic.py` & `cloudquicklabs1-0.0.3/src/logic.py`

 * *Files identical despite different names*

