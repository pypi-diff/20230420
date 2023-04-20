# Comparing `tmp/swiftgalaxy-1.0.1.tar.gz` & `tmp/swiftgalaxy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftgalaxy-1.0.1.tar", last modified: Wed Apr 12 16:39:01 2023, max compression
+gzip compressed data, was "swiftgalaxy-1.0.2.tar", last modified: Thu Apr 20 10:46:47 2023, max compression
```

## Comparing `swiftgalaxy-1.0.1.tar` & `swiftgalaxy-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:39:01.051945 swiftgalaxy-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-12 16:39:01.051945 swiftgalaxy-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:39:01.051945 swiftgalaxy-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:39:01.051945 swiftgalaxy-1.0.1/swiftgalaxy/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/swiftgalaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/swiftgalaxy/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/swiftgalaxy/halo_finders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/swiftgalaxy/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    67805 2023-04-12 16:38:25.000000 swiftgalaxy-1.0.1/swiftgalaxy/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:39:01.051945 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-12 16:39:00.000000 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-12 16:39:00.000000 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:39:00.000000 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:38:58.000000 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 16:39:00.000000 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 16:39:00.000000 swiftgalaxy-1.0.1/swiftgalaxy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:46:47.392055 swiftgalaxy-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-20 10:46:47.392055 swiftgalaxy-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:46:47.392055 swiftgalaxy-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:46:47.388055 swiftgalaxy-1.0.2/swiftgalaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/swiftgalaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/swiftgalaxy/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/swiftgalaxy/halo_finders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/swiftgalaxy/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67805 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/swiftgalaxy/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:46:47.388055 swiftgalaxy-1.0.2/swiftgalaxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-20 10:46:47.000000 swiftgalaxy-1.0.2/swiftgalaxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-20 10:46:47.000000 swiftgalaxy-1.0.2/swiftgalaxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:46:47.000000 swiftgalaxy-1.0.2/swiftgalaxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 10:46:47.000000 swiftgalaxy-1.0.2/swiftgalaxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 10:46:47.000000 swiftgalaxy-1.0.2/swiftgalaxy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:46:47.388055 swiftgalaxy-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20970 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/tests/test_coordinate_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/tests/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23837 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/tests/test_derived_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/tests/test_halo_finders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-20 10:46:02.000000 swiftgalaxy-1.0.2/tests/test_masking.py
```

### Comparing `swiftgalaxy-1.0.1/LICENSE.md` & `swiftgalaxy-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `swiftgalaxy-1.0.1/README.rst` & `swiftgalaxy-1.0.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 SWIFTGalaxy
 ===========
 
 |Build status| |Documentation status|
 
 .. |Build status| image:: https://github.com/SWIFTSIM/swiftgalaxy/actions/workflows/black_pytest.yml/badge.svg
-    :target: https://github.com/SWIFTSIM/swiftgalaxy/actions/workflows/pytest.yml
+    :target: https://github.com/SWIFTSIM/swiftgalaxy/actions/workflows/black_pytest.yml
     :alt: Build Status
 .. |Documentation status| image:: https://readthedocs.org/projects/swiftgalaxy/badge/?version=latest
     :target: https://swiftgalaxy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. INTRO_START_LABEL
```

### Comparing `swiftgalaxy-1.0.1/swiftgalaxy/halo_finders.py` & `swiftgalaxy-1.0.2/swiftgalaxy/halo_finders.py`

 * *Files identical despite different names*

### Comparing `swiftgalaxy-1.0.1/swiftgalaxy/masks.py` & `swiftgalaxy-1.0.2/swiftgalaxy/masks.py`

 * *Files identical despite different names*

### Comparing `swiftgalaxy-1.0.1/swiftgalaxy/reader.py` & `swiftgalaxy-1.0.2/swiftgalaxy/reader.py`

 * *Files identical despite different names*

