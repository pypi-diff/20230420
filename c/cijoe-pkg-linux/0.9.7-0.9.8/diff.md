# Comparing `tmp/cijoe-pkg-linux-0.9.7.tar.gz` & `tmp/cijoe-pkg-linux-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cijoe-pkg-linux-0.9.7.tar", last modified: Wed Apr 12 23:38:15 2023, max compression
+gzip compressed data, was "cijoe-pkg-linux-0.9.8.tar", last modified: Thu Apr 20 09:03:05 2023, max compression
```

## Comparing `cijoe-pkg-linux-0.9.7.tar` & `cijoe-pkg-linux-0.9.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.919793 cijoe-pkg-linux-0.9.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.919793 cijoe-pkg-linux-0.9.7/src/cijoe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/src/cijoe/linux/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/src/cijoe/linux/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/configs/default-config.toml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/kmemleak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/null_blk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/build_kdebs.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/null_blk.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/sysinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/transfer_and_install_kdebs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/src/cijoe/linux/selftest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/selftest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/selftest/test_kmemleak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/selftest/test_null_blk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/src/cijoe/linux/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/workflows/example-worklets.workflow
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/workflows/example.workflow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-12 23:38:15.000000 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-12 23:38:15.000000 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:38:15.000000 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:38:15.000000 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 23:38:15.000000 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 23:38:15.000000 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:05.211490 cijoe-pkg-linux-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-20 09:03:05.211490 cijoe-pkg-linux-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-20 09:03:05.215490 cijoe-pkg-linux-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:05.211490 cijoe-pkg-linux-0.9.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:05.207490 cijoe-pkg-linux-0.9.8/src/cijoe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:05.211490 cijoe-pkg-linux-0.9.8/src/cijoe/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:05.211490 cijoe-pkg-linux-0.9.8/src/cijoe/linux/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/configs/default-config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/kmemleak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/null_blk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:05.211490 cijoe-pkg-linux-0.9.8/src/cijoe/linux/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/scripts/build_kdebs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/scripts/null_blk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/scripts/sysinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/scripts/transfer_and_install_kdebs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:05.211490 cijoe-pkg-linux-0.9.8/src/cijoe/linux/selftest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/selftest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/selftest/test_kmemleak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/selftest/test_null_blk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:05.211490 cijoe-pkg-linux-0.9.8/src/cijoe/linux/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/workflows/example-worklets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 09:02:56.000000 cijoe-pkg-linux-0.9.8/src/cijoe/linux/workflows/example.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:03:05.211490 cijoe-pkg-linux-0.9.8/src/cijoe_pkg_linux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-20 09:03:05.000000 cijoe-pkg-linux-0.9.8/src/cijoe_pkg_linux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-20 09:03:05.000000 cijoe-pkg-linux-0.9.8/src/cijoe_pkg_linux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:03:05.000000 cijoe-pkg-linux-0.9.8/src/cijoe_pkg_linux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:03:05.000000 cijoe-pkg-linux-0.9.8/src/cijoe_pkg_linux.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 09:03:05.000000 cijoe-pkg-linux-0.9.8/src/cijoe_pkg_linux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 09:03:05.000000 cijoe-pkg-linux-0.9.8/src/cijoe_pkg_linux.egg-info/top_level.txt
```

### Comparing `cijoe-pkg-linux-0.9.7/LICENSE` & `cijoe-pkg-linux-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.7/PKG-INFO` & `cijoe-pkg-linux-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cijoe-pkg-linux
-Version: 0.9.7
+Version: 0.9.8
 Summary: A loosely coupled approach to systems development and testing
 Home-page: UNKNOWN
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
 Maintainer: Simon A. F. Lund
 Maintainer-email: os@safl.dk
 License: BSD-3-Clause
```

### Comparing `cijoe-pkg-linux-0.9.7/README.rst` & `cijoe-pkg-linux-0.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.7/setup.cfg` & `cijoe-pkg-linux-0.9.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.7/src/cijoe/linux/configs/default-config.toml` & `cijoe-pkg-linux-0.9.8/src/cijoe/linux/configs/default-config.toml`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.7/src/cijoe/linux/kmemleak.py` & `cijoe-pkg-linux-0.9.8/src/cijoe/linux/kmemleak.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.7/src/cijoe/linux/null_blk.py` & `cijoe-pkg-linux-0.9.8/src/cijoe/linux/null_blk.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/build_kdebs.py` & `cijoe-pkg-linux-0.9.8/src/cijoe/linux/scripts/build_kdebs.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/null_blk.py` & `cijoe-pkg-linux-0.9.8/src/cijoe/linux/scripts/null_blk.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/sysinfo.py` & `cijoe-pkg-linux-0.9.8/src/cijoe/linux/scripts/sysinfo.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/transfer_and_install_kdebs.py` & `cijoe-pkg-linux-0.9.8/src/cijoe/linux/scripts/transfer_and_install_kdebs.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.7/src/cijoe/linux/selftest/test_kmemleak.py` & `cijoe-pkg-linux-0.9.8/src/cijoe/linux/selftest/test_kmemleak.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.7/src/cijoe/linux/selftest/test_null_blk.py` & `cijoe-pkg-linux-0.9.8/src/cijoe/linux/selftest/test_null_blk.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/PKG-INFO` & `cijoe-pkg-linux-0.9.8/src/cijoe_pkg_linux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cijoe-pkg-linux
-Version: 0.9.7
+Version: 0.9.8
 Summary: A loosely coupled approach to systems development and testing
 Home-page: UNKNOWN
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
 Maintainer: Simon A. F. Lund
 Maintainer-email: os@safl.dk
 License: BSD-3-Clause
```

### Comparing `cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/SOURCES.txt` & `cijoe-pkg-linux-0.9.8/src/cijoe_pkg_linux.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 src/cijoe/linux/scripts/null_blk.py
 src/cijoe/linux/scripts/sysinfo.py
 src/cijoe/linux/scripts/transfer_and_install_kdebs.py
 src/cijoe/linux/selftest/__init__.py
 src/cijoe/linux/selftest/test_kmemleak.py
 src/cijoe/linux/selftest/test_null_blk.py
 src/cijoe/linux/workflows/__init__.py
-src/cijoe/linux/workflows/example-worklets.workflow
-src/cijoe/linux/workflows/example.workflow
+src/cijoe/linux/workflows/example-worklets.yaml
+src/cijoe/linux/workflows/example.yaml
 src/cijoe_pkg_linux.egg-info/PKG-INFO
 src/cijoe_pkg_linux.egg-info/SOURCES.txt
 src/cijoe_pkg_linux.egg-info/dependency_links.txt
 src/cijoe_pkg_linux.egg-info/not-zip-safe
 src/cijoe_pkg_linux.egg-info/requires.txt
 src/cijoe_pkg_linux.egg-info/top_level.txt
```

