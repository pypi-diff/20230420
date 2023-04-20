# Comparing `tmp/mlserver-lightgbm-1.3.1.tar.gz` & `tmp/mlserver-lightgbm-1.3.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-lightgbm-1.3.1.tar", last modified: Fri Apr 14 18:06:34 2023, max compression
+gzip compressed data, was "mlserver-lightgbm-1.3.2rc1.tar", last modified: Thu Apr 20 16:09:08 2023, max compression
```

## Comparing `mlserver-lightgbm-1.3.1.tar` & `mlserver-lightgbm-1.3.2rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:34.432996 mlserver-lightgbm-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-14 18:05:57.000000 mlserver-lightgbm-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-14 18:06:34.432996 mlserver-lightgbm-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-14 18:05:57.000000 mlserver-lightgbm-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:34.428996 mlserver-lightgbm-1.3.1/mlserver_lightgbm/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 18:05:57.000000 mlserver-lightgbm-1.3.1/mlserver_lightgbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-14 18:05:57.000000 mlserver-lightgbm-1.3.1/mlserver_lightgbm/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 18:05:57.000000 mlserver-lightgbm-1.3.1/mlserver_lightgbm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:34.428996 mlserver-lightgbm-1.3.1/mlserver_lightgbm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-14 18:06:34.000000 mlserver-lightgbm-1.3.1/mlserver_lightgbm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-14 18:06:34.000000 mlserver-lightgbm-1.3.1/mlserver_lightgbm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:06:34.000000 mlserver-lightgbm-1.3.1/mlserver_lightgbm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 18:06:34.000000 mlserver-lightgbm-1.3.1/mlserver_lightgbm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 18:06:34.000000 mlserver-lightgbm-1.3.1/mlserver_lightgbm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:06:34.432996 mlserver-lightgbm-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-14 18:05:57.000000 mlserver-lightgbm-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:08.943377 mlserver-lightgbm-1.3.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-20 16:08:23.000000 mlserver-lightgbm-1.3.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-20 16:09:08.943377 mlserver-lightgbm-1.3.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-20 16:08:23.000000 mlserver-lightgbm-1.3.2rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:08.939377 mlserver-lightgbm-1.3.2rc1/mlserver_lightgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 16:08:23.000000 mlserver-lightgbm-1.3.2rc1/mlserver_lightgbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-20 16:08:23.000000 mlserver-lightgbm-1.3.2rc1/mlserver_lightgbm/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 16:08:23.000000 mlserver-lightgbm-1.3.2rc1/mlserver_lightgbm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:08.943377 mlserver-lightgbm-1.3.2rc1/mlserver_lightgbm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-20 16:09:08.000000 mlserver-lightgbm-1.3.2rc1/mlserver_lightgbm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-20 16:09:08.000000 mlserver-lightgbm-1.3.2rc1/mlserver_lightgbm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:09:08.000000 mlserver-lightgbm-1.3.2rc1/mlserver_lightgbm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 16:09:08.000000 mlserver-lightgbm-1.3.2rc1/mlserver_lightgbm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 16:09:08.000000 mlserver-lightgbm-1.3.2rc1/mlserver_lightgbm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:09:08.943377 mlserver-lightgbm-1.3.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-20 16:08:23.000000 mlserver-lightgbm-1.3.2rc1/setup.py
```

### Comparing `mlserver-lightgbm-1.3.1/LICENSE` & `mlserver-lightgbm-1.3.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-lightgbm-1.3.1/PKG-INFO` & `mlserver-lightgbm-1.3.2rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-lightgbm
-Version: 1.3.1
+Version: 1.3.2rc1
 Summary: LightGBM runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # LightGBM runtime for MLServer
```

### Comparing `mlserver-lightgbm-1.3.1/README.md` & `mlserver-lightgbm-1.3.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-lightgbm-1.3.1/mlserver_lightgbm/lightgbm.py` & `mlserver-lightgbm-1.3.2rc1/mlserver_lightgbm/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mlserver-lightgbm-1.3.1/mlserver_lightgbm.egg-info/PKG-INFO` & `mlserver-lightgbm-1.3.2rc1/mlserver_lightgbm.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-lightgbm
-Version: 1.3.1
+Version: 1.3.2rc1
 Summary: LightGBM runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # LightGBM runtime for MLServer
```

### Comparing `mlserver-lightgbm-1.3.1/setup.py` & `mlserver-lightgbm-1.3.2rc1/setup.py`

 * *Files identical despite different names*

