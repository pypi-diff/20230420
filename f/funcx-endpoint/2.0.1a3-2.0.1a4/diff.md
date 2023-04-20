# Comparing `tmp/funcx-endpoint-2.0.1a3.tar.gz` & `tmp/funcx-endpoint-2.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-endpoint-2.0.1a3.tar", last modified: Tue Apr 18 22:07:44 2023, max compression
+gzip compressed data, was "funcx-endpoint-2.0.1a4.tar", last modified: Thu Apr 20 15:09:14 2023, max compression
```

## Comparing `funcx-endpoint-2.0.1a3.tar` & `funcx-endpoint-2.0.1a4.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:07:44.857228 funcx-endpoint-2.0.1a3/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a3/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-18 19:39:56.000000 funcx-endpoint-2.0.1a3/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     2042 2023-04-18 22:07:44.857276 funcx-endpoint-2.0.1a3/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1115 2023-04-18 19:39:56.000000 funcx-endpoint-2.0.1a3/PyPI.md
--rw-r--r--   0 lei        (501) staff       (20)      430 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a3/README.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:07:44.856297 funcx-endpoint-2.0.1a3/funcx_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      122 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a3/funcx_endpoint/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:07:44.857126 funcx-endpoint-2.0.1a3/funcx_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      107 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a3/funcx_endpoint/executors/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      245 2023-04-18 22:04:30.000000 funcx-endpoint-2.0.1a3/funcx_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:07:44.857013 funcx-endpoint-2.0.1a3/funcx_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     2042 2023-04-18 22:07:44.000000 funcx-endpoint-2.0.1a3/funcx_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      376 2023-04-18 22:07:44.000000 funcx-endpoint-2.0.1a3/funcx_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-18 22:07:44.000000 funcx-endpoint-2.0.1a3/funcx_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      329 2023-04-18 22:07:44.000000 funcx-endpoint-2.0.1a3/funcx_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)       33 2023-04-18 22:07:44.000000 funcx-endpoint-2.0.1a3/funcx_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       15 2023-04-18 22:07:44.000000 funcx-endpoint-2.0.1a3/funcx_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      305 2023-04-18 22:07:44.857497 funcx-endpoint-2.0.1a3/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     2032 2023-04-18 22:04:26.000000 funcx-endpoint-2.0.1a3/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:09:14.775516 funcx-endpoint-2.0.1a4/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a4/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 funcx-endpoint-2.0.1a4/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     2042 2023-04-20 15:09:14.775570 funcx-endpoint-2.0.1a4/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     1115 2023-04-20 03:21:56.000000 funcx-endpoint-2.0.1a4/PyPI.md
+-rw-r--r--   0 lei        (501) staff       (20)      430 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a4/README.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:09:14.773621 funcx-endpoint-2.0.1a4/funcx_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      122 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a4/funcx_endpoint/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:09:14.774493 funcx-endpoint-2.0.1a4/funcx_endpoint/endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-endpoint-2.0.1a4/funcx_endpoint/endpoint/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:09:14.774722 funcx-endpoint-2.0.1a4/funcx_endpoint/endpoint/utils/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-endpoint-2.0.1a4/funcx_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)       89 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a4/funcx_endpoint/endpoint/utils/config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:09:14.774872 funcx-endpoint-2.0.1a4/funcx_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      107 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a4/funcx_endpoint/executors/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:09:14.775369 funcx-endpoint-2.0.1a4/funcx_endpoint/executors/high_throughput/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-endpoint-2.0.1a4/funcx_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      101 2023-04-20 03:22:06.000000 funcx-endpoint-2.0.1a4/funcx_endpoint/executors/high_throughput/funcx_manager.py
+-rw-r--r--   0 lei        (501) staff       (20)      114 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a4/funcx_endpoint/executors/high_throughput/funcx_worker.py
+-rw-r--r--   0 lei        (501) staff       (20)      245 2023-04-20 15:04:14.000000 funcx-endpoint-2.0.1a4/funcx_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:09:14.774358 funcx-endpoint-2.0.1a4/funcx_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     2042 2023-04-20 15:09:14.000000 funcx-endpoint-2.0.1a4/funcx_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      662 2023-04-20 15:09:14.000000 funcx-endpoint-2.0.1a4/funcx_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-20 15:09:14.000000 funcx-endpoint-2.0.1a4/funcx_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      329 2023-04-20 15:09:14.000000 funcx-endpoint-2.0.1a4/funcx_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)       33 2023-04-20 15:09:14.000000 funcx-endpoint-2.0.1a4/funcx_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       15 2023-04-20 15:09:14.000000 funcx-endpoint-2.0.1a4/funcx_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      305 2023-04-20 15:09:14.775797 funcx-endpoint-2.0.1a4/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     2032 2023-04-20 15:04:05.000000 funcx-endpoint-2.0.1a4/setup.py
```

### Comparing `funcx-endpoint-2.0.1a3/LICENSE` & `funcx-endpoint-2.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.0.1a3/PKG-INFO` & `funcx-endpoint-2.0.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx-endpoint
-Version: 2.0.1a3
+Version: 2.0.1a4
 Summary: funcX: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-endpoint-2.0.1a3/PyPI.md` & `funcx-endpoint-2.0.1a4/PyPI.md`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.0.1a3/funcx_endpoint.egg-info/PKG-INFO` & `funcx-endpoint-2.0.1a4/funcx_endpoint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx-endpoint
-Version: 2.0.1a3
+Version: 2.0.1a4
 Summary: funcX: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-endpoint-2.0.1a3/setup.py` & `funcx-endpoint-2.0.1a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
-    "globus-compute-endpoint>=2.0.1a3",
+    "globus-compute-endpoint>=2.0.1a4",
 ]
 
 version_ns = {}
 with open(os.path.join("funcx_endpoint", "version.py")) as f:
     exec(f.read(), version_ns)
 version = version_ns["__version__"]
```

