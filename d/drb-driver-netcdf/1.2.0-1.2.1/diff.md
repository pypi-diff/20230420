# Comparing `tmp/drb-driver-netcdf-1.2.0.tar.gz` & `tmp/drb-driver-netcdf-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-netcdf-1.2.0.tar", last modified: Wed Apr 19 08:20:50 2023, max compression
+gzip compressed data, was "drb-driver-netcdf-1.2.1.tar", last modified: Thu Apr 20 15:05:16 2023, max compression
```

## Comparing `drb-driver-netcdf-1.2.0.tar` & `drb-driver-netcdf-1.2.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.941820 drb-driver-netcdf-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 12:41:04.000000 drb-driver-netcdf-1.2.0/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2579 2023-04-19 08:20:50.941820 drb-driver-netcdf-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2030 2022-12-19 14:52:00.000000 drb-driver-netcdf-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.921820 drb-driver-netcdf-1.2.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.917820 drb-driver-netcdf-1.2.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.945820 drb-driver-netcdf-1.2.0/drb/drivers/netcdf/
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/drb/drivers/netcdf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-04-19 08:20:50.945820 drb-driver-netcdf-1.2.0/drb/drivers/netcdf/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    11690 2023-04-18 15:24:17.000000 drb-driver-netcdf-1.2.0/drb/drivers/netcdf/netcdf.py
--rw-rw-rw-   0 root         (0) root         (0)     3395 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.0/drb/drivers/netcdf/netcdf_node_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.929820 drb-driver-netcdf-1.2.0/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)      190 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.0/drb/exceptions/netcdf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.921820 drb-driver-netcdf-1.2.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.929820 drb-driver-netcdf-1.2.0/drb/topics/netcdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.0/drb/topics/netcdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-04-19 08:19:37.000000 drb-driver-netcdf-1.2.0/drb/topics/netcdf/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.933820 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2579 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      861 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-19 08:20:50.000000 drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1114 2023-04-19 08:20:50.945820 drb-driver-netcdf-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:20:50.941820 drb-driver-netcdf-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4307 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_dimension.py
--rw-rw-rw-   0 root         (0) root         (0)     7152 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_group.py
--rw-rw-rw-   0 root         (0) root         (0)     1354 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)     3823 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_list.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_node_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1984 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_signature.py
--rw-rw-rw-   0 root         (0) root         (0)     1941 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_temporary_file.py
--rw-rw-rw-   0 root         (0) root         (0)     8735 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_variable.py
--rw-rw-rw-   0 root         (0) root         (0)    80044 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:05:16.122594 drb-driver-netcdf-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 12:41:04.000000 drb-driver-netcdf-1.2.1/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       60 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-04-20 15:05:16.122594 drb-driver-netcdf-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2022-12-19 14:52:00.000000 drb-driver-netcdf-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:05:16.102594 drb-driver-netcdf-1.2.1/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:05:16.098594 drb-driver-netcdf-1.2.1/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:05:16.126595 drb-driver-netcdf-1.2.1/drb/drivers/netcdf/
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.1/drb/drivers/netcdf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-20 15:05:16.126595 drb-driver-netcdf-1.2.1/drb/drivers/netcdf/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    11690 2023-04-18 15:24:17.000000 drb-driver-netcdf-1.2.1/drb/drivers/netcdf/netcdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3395 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.1/drb/drivers/netcdf/netcdf_node_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:05:16.110594 drb-driver-netcdf-1.2.1/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.1/drb/exceptions/netcdf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:05:16.102594 drb-driver-netcdf-1.2.1/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:05:16.110594 drb-driver-netcdf-1.2.1/drb/topics/netcdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.1/drb/topics/netcdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-04-20 15:04:12.000000 drb-driver-netcdf-1.2.1/drb/topics/netcdf/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:05:16.114594 drb-driver-netcdf-1.2.1/drb_driver_netcdf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-04-20 15:05:16.000000 drb-driver-netcdf-1.2.1/drb_driver_netcdf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      876 2023-04-20 15:05:16.000000 drb-driver-netcdf-1.2.1/drb_driver_netcdf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 15:05:16.000000 drb-driver-netcdf-1.2.1/drb_driver_netcdf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-20 15:05:16.000000 drb-driver-netcdf-1.2.1/drb_driver_netcdf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 15:05:15.000000 drb-driver-netcdf-1.2.1/drb_driver_netcdf.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-20 15:05:16.000000 drb-driver-netcdf-1.2.1/drb_driver_netcdf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-20 15:05:16.000000 drb-driver-netcdf-1.2.1/drb_driver_netcdf.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-20 14:15:20.000000 drb-driver-netcdf-1.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2023-04-20 15:05:16.122594 drb-driver-netcdf-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:05:16.122594 drb-driver-netcdf-1.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_dimension.py
+-rw-rw-rw-   0 root         (0) root         (0)     7152 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)     3823 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_node_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     1941 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_temporary_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-04-18 13:42:57.000000 drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_variable.py
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2022-12-19 13:45:22.000000 drb-driver-netcdf-1.2.1/versioneer.py
```

### Comparing `drb-driver-netcdf-1.2.0/LICENCE.txt` & `drb-driver-netcdf-1.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/PKG-INFO` & `drb-driver-netcdf-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-driver-netcdf
-Version: 1.2.0
+Version: 1.2.1
 Summary: DRB NetCDF Driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Documentation, http://drb-python.gitlab.io/impl/netcdf
 Project-URL: Source, https://gitlab.com/drb-python/impl/netcdf
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drb-driver-netcdf-1.2.0/README.md` & `drb-driver-netcdf-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/drb/drivers/netcdf/__init__.py` & `drb-driver-netcdf-1.2.1/drb/drivers/netcdf/__init__.py`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/drb/drivers/netcdf/netcdf.py` & `drb-driver-netcdf-1.2.1/drb/drivers/netcdf/netcdf.py`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/drb/drivers/netcdf/netcdf_node_factory.py` & `drb-driver-netcdf-1.2.1/drb/drivers/netcdf/netcdf_node_factory.py`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/PKG-INFO` & `drb-driver-netcdf-1.2.1/drb_driver_netcdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-driver-netcdf
-Version: 1.2.0
+Version: 1.2.1
 Summary: DRB NetCDF Driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Documentation, http://drb-python.gitlab.io/impl/netcdf
 Project-URL: Source, https://gitlab.com/drb-python/impl/netcdf
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drb-driver-netcdf-1.2.0/drb_driver_netcdf.egg-info/SOURCES.txt` & `drb-driver-netcdf-1.2.1/drb_driver_netcdf.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENCE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 drb/drivers/netcdf/__init__.py
 drb/drivers/netcdf/_version.py
 drb/drivers/netcdf/netcdf.py
```

### Comparing `drb-driver-netcdf-1.2.0/setup.cfg` & `drb-driver-netcdf-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_dimension.py` & `drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_dimension.py`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_group.py` & `drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_group.py`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_hdf5.py` & `drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_hdf5.py`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_list.py` & `drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_list.py`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_node_factory.py` & `drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_node_factory.py`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_signature.py` & `drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_signature.py`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_temporary_file.py` & `drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_temporary_file.py`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/tests/test_drb_netcdf_variable.py` & `drb-driver-netcdf-1.2.1/tests/test_drb_netcdf_variable.py`

 * *Files identical despite different names*

### Comparing `drb-driver-netcdf-1.2.0/versioneer.py` & `drb-driver-netcdf-1.2.1/versioneer.py`

 * *Files identical despite different names*

