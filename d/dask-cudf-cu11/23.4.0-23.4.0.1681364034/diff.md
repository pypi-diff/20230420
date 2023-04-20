# Comparing `tmp/dask_cudf_cu11-23.4.0.tar.gz` & `tmp/dask_cudf_cu11-23.4.0.1681364034.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask_cudf_cu11-23.4.0.tar", last modified: Thu Apr 20 17:52:41 2023, max compression
+gzip compressed data, was "dask_cudf_cu11-23.4.0.1681364034.tar", last modified: Thu Apr 13 19:14:59 2023, max compression
```

## Comparing `dask_cudf_cu11-23.4.0.tar` & `dask_cudf_cu11-23.4.0.1681364034.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-20 17:52:41.705444 dask_cudf_cu11-23.4.0/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      446 2023-04-20 17:52:41.000000 dask_cudf_cu11-23.4.0/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 18:19:20.000000 dask_cudf_cu11-23.4.0/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       14 2023-04-20 17:52:41.000000 dask_cudf_cu11-23.4.0/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-04-20 17:52:41.705444 dask_cudf_cu11-23.4.0/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2023-04-20 17:52:41.000000 dask_cudf_cu11-23.4.0/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-20 17:52:41.704445 dask_cudf_cu11-23.4.0/dask_cudf_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-04-20 17:52:41.000000 dask_cudf_cu11-23.4.0/dask_cudf_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      205 2023-04-20 17:52:41.000000 dask_cudf_cu11-23.4.0/dask_cudf_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-20 17:52:41.000000 dask_cudf_cu11-23.4.0/dask_cudf_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-20 17:52:41.000000 dask_cudf_cu11-23.4.0/dask_cudf_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-20 17:52:41.705444 dask_cudf_cu11-23.4.0/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 18:19:20.000000 dask_cudf_cu11-23.4.0/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:14:59.400119 dask_cudf_cu11-23.4.0.1681364034/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      446 2023-04-13 19:14:59.000000 dask_cudf_cu11-23.4.0.1681364034/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-13 18:19:20.000000 dask_cudf_cu11-23.4.0.1681364034/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       14 2023-04-13 19:14:59.000000 dask_cudf_cu11-23.4.0.1681364034/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1615 2023-04-13 19:14:59.400119 dask_cudf_cu11-23.4.0.1681364034/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2023-04-13 19:14:59.000000 dask_cudf_cu11-23.4.0.1681364034/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-04-13 19:14:59.400119 dask_cudf_cu11-23.4.0.1681364034/dask_cudf_cu11.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1615 2023-04-13 19:14:59.000000 dask_cudf_cu11-23.4.0.1681364034/dask_cudf_cu11.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      205 2023-04-13 19:14:59.000000 dask_cudf_cu11-23.4.0.1681364034/dask_cudf_cu11.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:14:59.000000 dask_cudf_cu11-23.4.0.1681364034/dask_cudf_cu11.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-04-13 19:14:59.000000 dask_cudf_cu11-23.4.0.1681364034/dask_cudf_cu11.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-04-13 19:14:59.400119 dask_cudf_cu11-23.4.0.1681364034/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-13 18:19:20.000000 dask_cudf_cu11-23.4.0.1681364034/setup.py
```

### Comparing `dask_cudf_cu11-23.4.0/LICENSE.md` & `dask_cudf_cu11-23.4.0.1681364034/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dask_cudf_cu11-23.4.0/PKG-INFO` & `dask_cudf_cu11-23.4.0.1681364034/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask_cudf_cu11
-Version: 23.4.0
+Version: 23.4.0.1681364034
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `dask_cudf_cu11-23.4.0/dask_cudf_cu11.egg-info/PKG-INFO` & `dask_cudf_cu11-23.4.0.1681364034/dask_cudf_cu11.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cudf-cu11
-Version: 23.4.0
+Version: 23.4.0.1681364034
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `dask_cudf_cu11-23.4.0/setup.py` & `dask_cudf_cu11-23.4.0.1681364034/setup.py`

 * *Files identical despite different names*

