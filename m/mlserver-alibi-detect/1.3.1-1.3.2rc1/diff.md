# Comparing `tmp/mlserver-alibi-detect-1.3.1.tar.gz` & `tmp/mlserver-alibi-detect-1.3.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-alibi-detect-1.3.1.tar", last modified: Fri Apr 14 18:06:41 2023, max compression
+gzip compressed data, was "mlserver-alibi-detect-1.3.2rc1.tar", last modified: Thu Apr 20 16:09:14 2023, max compression
```

## Comparing `mlserver-alibi-detect-1.3.1.tar` & `mlserver-alibi-detect-1.3.2rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:41.817361 mlserver-alibi-detect-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-14 18:05:58.000000 mlserver-alibi-detect-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-14 18:06:41.817361 mlserver-alibi-detect-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-14 18:05:58.000000 mlserver-alibi-detect-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:41.817361 mlserver-alibi-detect-1.3.1/mlserver_alibi_detect/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 18:05:58.000000 mlserver-alibi-detect-1.3.1/mlserver_alibi_detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-04-14 18:05:58.000000 mlserver-alibi-detect-1.3.1/mlserver_alibi_detect/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 18:05:58.000000 mlserver-alibi-detect-1.3.1/mlserver_alibi_detect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:41.817361 mlserver-alibi-detect-1.3.1/mlserver_alibi_detect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-14 18:06:41.000000 mlserver-alibi-detect-1.3.1/mlserver_alibi_detect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-14 18:06:41.000000 mlserver-alibi-detect-1.3.1/mlserver_alibi_detect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:06:41.000000 mlserver-alibi-detect-1.3.1/mlserver_alibi_detect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-14 18:06:41.000000 mlserver-alibi-detect-1.3.1/mlserver_alibi_detect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 18:06:41.000000 mlserver-alibi-detect-1.3.1/mlserver_alibi_detect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:06:41.817361 mlserver-alibi-detect-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-14 18:05:58.000000 mlserver-alibi-detect-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:14.885846 mlserver-alibi-detect-1.3.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-20 16:08:25.000000 mlserver-alibi-detect-1.3.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-20 16:09:14.885846 mlserver-alibi-detect-1.3.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-20 16:08:25.000000 mlserver-alibi-detect-1.3.2rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:14.881846 mlserver-alibi-detect-1.3.2rc1/mlserver_alibi_detect/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 16:08:25.000000 mlserver-alibi-detect-1.3.2rc1/mlserver_alibi_detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-04-20 16:08:25.000000 mlserver-alibi-detect-1.3.2rc1/mlserver_alibi_detect/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 16:08:25.000000 mlserver-alibi-detect-1.3.2rc1/mlserver_alibi_detect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:14.885846 mlserver-alibi-detect-1.3.2rc1/mlserver_alibi_detect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-20 16:09:14.000000 mlserver-alibi-detect-1.3.2rc1/mlserver_alibi_detect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-20 16:09:14.000000 mlserver-alibi-detect-1.3.2rc1/mlserver_alibi_detect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:09:14.000000 mlserver-alibi-detect-1.3.2rc1/mlserver_alibi_detect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 16:09:14.000000 mlserver-alibi-detect-1.3.2rc1/mlserver_alibi_detect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 16:09:14.000000 mlserver-alibi-detect-1.3.2rc1/mlserver_alibi_detect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:09:14.885846 mlserver-alibi-detect-1.3.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-20 16:08:25.000000 mlserver-alibi-detect-1.3.2rc1/setup.py
```

### Comparing `mlserver-alibi-detect-1.3.1/LICENSE` & `mlserver-alibi-detect-1.3.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-detect-1.3.1/PKG-INFO` & `mlserver-alibi-detect-1.3.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-alibi-detect
-Version: 1.3.1
+Version: 1.3.2rc1
 Summary: Alibi-Detect runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # Alibi-Detect runtime for MLServer
```

### Comparing `mlserver-alibi-detect-1.3.1/README.md` & `mlserver-alibi-detect-1.3.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-detect-1.3.1/mlserver_alibi_detect.egg-info/PKG-INFO` & `mlserver-alibi-detect-1.3.2rc1/mlserver_alibi_detect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-alibi-detect
-Version: 1.3.1
+Version: 1.3.2rc1
 Summary: Alibi-Detect runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # Alibi-Detect runtime for MLServer
```

### Comparing `mlserver-alibi-detect-1.3.1/setup.py` & `mlserver-alibi-detect-1.3.2rc1/setup.py`

 * *Files identical despite different names*

