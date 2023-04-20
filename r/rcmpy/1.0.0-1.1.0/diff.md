# Comparing `tmp/rcmpy-1.0.0.tar.gz` & `tmp/rcmpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-1.0.0.tar", last modified: Wed Apr 12 06:23:36 2023, max compression
+gzip compressed data, was "rcmpy-1.1.0.tar", last modified: Thu Apr 20 07:35:17 2023, max compression
```

## Comparing `rcmpy-1.0.0.tar` & `rcmpy-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 06:22:17.000000 rcmpy-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-12 06:23:36.110685 rcmpy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-12 06:22:17.000000 rcmpy-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-12 06:22:17.000000 rcmpy-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.106685 rcmpy-1.0.0/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.106685 rcmpy-1.0.0/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-12 06:23:36.000000 rcmpy-1.0.0/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-12 06:23:36.000000 rcmpy-1.0.0/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 06:23:36.000000 rcmpy-1.0.0/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 06:23:36.000000 rcmpy-1.0.0/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-12 06:23:36.000000 rcmpy-1.0.0/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 06:23:36.000000 rcmpy-1.0.0/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 06:23:36.114685 rcmpy-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-12 06:22:17.000000 rcmpy-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-12 06:22:17.000000 rcmpy-1.0.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 06:22:17.000000 rcmpy-1.0.0/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 06:22:17.000000 rcmpy-1.0.0/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.429541 rcmpy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 07:34:06.000000 rcmpy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-20 07:35:17.425541 rcmpy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-20 07:34:06.000000 rcmpy-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-20 07:34:06.000000 rcmpy-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/config/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.421541 rcmpy-1.1.0/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-20 07:34:06.000000 rcmpy-1.1.0/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-20 07:35:17.000000 rcmpy-1.1.0/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-20 07:35:17.000000 rcmpy-1.1.0/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:35:17.000000 rcmpy-1.1.0/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 07:35:17.000000 rcmpy-1.1.0/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 07:35:17.000000 rcmpy-1.1.0/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 07:35:17.000000 rcmpy-1.1.0/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 07:35:17.429541 rcmpy-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-20 07:34:06.000000 rcmpy-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:35:17.425541 rcmpy-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-20 07:34:06.000000 rcmpy-1.1.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 07:34:06.000000 rcmpy-1.1.0/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-20 07:34:06.000000 rcmpy-1.1.0/tests/test_xdg.py
```

### Comparing `rcmpy-1.0.0/LICENSE` & `rcmpy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/PKG-INFO` & `rcmpy-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.0.0
+Version: 1.1.0
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=4e253e82b70bf6a2a6479e0620da720b
+    hash=d6cd0e307dd25044b7eb3a7adaf13b33
     =====================================
 -->
 
-# rcmpy ([1.0.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.1.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -169,18 +169,20 @@
 ## Sub-command Options
 
 ### `apply`
 
 ```
 $ ./venv3.8/bin/rcmpy apply -h
 
-usage: rcmpy apply [-h]
+usage: rcmpy apply [-h] [-f] [-d]
 
 optional arguments:
-  -h, --help  show this help message and exit
+  -h, --help     show this help message and exit
+  -f, --force    whether or not to forcibly render all outputs
+  -d, --dry-run  whether or not to update output files
 
 ```
 
 ### `use`
 
 ```
 $ ./venv3.8/bin/rcmpy use -h
```

### Comparing `rcmpy-1.0.0/README.md` & `rcmpy-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=4e253e82b70bf6a2a6479e0620da720b
+    hash=d6cd0e307dd25044b7eb3a7adaf13b33
     =====================================
 -->
 
-# rcmpy ([1.0.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.1.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -145,18 +145,20 @@
 ## Sub-command Options
 
 ### `apply`
 
 ```
 $ ./venv3.8/bin/rcmpy apply -h
 
-usage: rcmpy apply [-h]
+usage: rcmpy apply [-h] [-f] [-d]
 
 optional arguments:
-  -h, --help  show this help message and exit
+  -h, --help     show this help message and exit
+  -f, --force    whether or not to forcibly render all outputs
+  -d, --dry-run  whether or not to update output files
 
 ```
 
 ### `use`
 
 ```
 $ ./venv3.8/bin/rcmpy use -h
```

### Comparing `rcmpy-1.0.0/pyproject.toml` & `rcmpy-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "rcmpy"
-version = "1.0.0"
+version = "1.1.0"
 description = "A configuration-file management system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `rcmpy-1.0.0/rcmpy/app.py` & `rcmpy-1.1.0/rcmpy/app.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/rcmpy/commands/all.py` & `rcmpy-1.1.0/rcmpy/commands/all.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/rcmpy/commands/use.py` & `rcmpy-1.1.0/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/rcmpy/commands/variant.py` & `rcmpy-1.1.0/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/rcmpy/commands/watch.py` & `rcmpy-1.1.0/rcmpy/commands/watch.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/rcmpy/entry.py` & `rcmpy-1.1.0/rcmpy/entry.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/rcmpy/environment/__init__.py` & `rcmpy-1.1.0/rcmpy/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/rcmpy/environment/template.py` & `rcmpy-1.1.0/rcmpy/environment/template.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/rcmpy/paths/__init__.py` & `rcmpy-1.1.0/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/rcmpy/schemas.py` & `rcmpy-1.1.0/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/rcmpy/state/__init__.py` & `rcmpy-1.1.0/rcmpy/state/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 class State(_RcmpyDictCodec):
     """The top-level configuration object for the package."""
 
     directory: Path
     variant: str
     variables_new: bool
     configs_new: bool
+    manifest: Dict[str, Any]
+    manifest_new: bool
 
     def init(self, data: _JsonObject) -> None:
         """Perform implementation-specific initialization."""
 
         self.logger = LOG
 
         self.directory = normalize(
@@ -60,22 +62,34 @@
 
         # Configs.
         self.configs: Dict[str, Any] = {}
         self.configs_new = False
         self.previous.setdefault("configs", {})
         self._load_configs()
 
+        # Manifest configuration.
+        self.manifest: Dict[str, Any] = cast(
+            Dict[str, Any], data.get("manifest", {})
+        )
+        self.manifest_new: bool = False
+
     def is_new(self) -> bool:
         """Determine if state has changed."""
         return (
             self.variant != self.previous["variant"]
             or self.variables_new
             or self.configs_new
+            or self.manifest_new
         )
 
+    def update_manifest(self, data: Dict[str, Any]) -> None:
+        """Set new manifest data."""
+        self.manifest_new = self.manifest != data
+        self.manifest = data
+
     def root_directories(self, subdir: str) -> List[Path]:
         """
         Get up to a pair of directories from some sub-directory of the current
         root.
         """
 
         root = self.directory.joinpath(subdir)
@@ -103,14 +117,15 @@
                     self.configs,
                     ARBITER.decode_directory(
                         path,
                         logger=self.logger,
                         require_success=True,
                         recurse=True,
                         includes_key="includes",
+                        expect_overwrite=True,
                         preprocessor=preprocessor,
                     ).data,
                     logger=self.logger,
                 )
 
         self.configs_new = self.configs != self.previous["configs"]
         self.previous["configs"] = self.configs
@@ -126,14 +141,15 @@
                 self.variables,
                 ARBITER.decode_directory(
                     path,
                     logger=self.logger,
                     require_success=True,
                     recurse=True,
                     includes_key="includes",
+                    expect_overwrite=True,
                 ).data,
                 logger=self.logger,
             )
 
         self.variables_new = self.variables != self.previous["variables"]
         self.previous["variables"] = self.variables
 
@@ -167,14 +183,15 @@
     def asdict(self) -> _JsonObject:
         """Obtain a dictionary representing this instance."""
 
         return {
             "directory": str(self.directory),
             "variant": self.variant,
             "previous": self.previous,
+            "manifest": self.manifest,
         }
 
 
 @contextmanager
 def load_state(
     root: Pathlike = None, name: str = "state.json"
 ) -> Iterator[State]:
```

### Comparing `rcmpy-1.0.0/rcmpy/xdg/__init__.py` & `rcmpy-1.1.0/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/rcmpy.egg-info/PKG-INFO` & `rcmpy-1.1.0/rcmpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.0.0
+Version: 1.1.0
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=4e253e82b70bf6a2a6479e0620da720b
+    hash=d6cd0e307dd25044b7eb3a7adaf13b33
     =====================================
 -->
 
-# rcmpy ([1.0.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.1.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -169,18 +169,20 @@
 ## Sub-command Options
 
 ### `apply`
 
 ```
 $ ./venv3.8/bin/rcmpy apply -h
 
-usage: rcmpy apply [-h]
+usage: rcmpy apply [-h] [-f] [-d]
 
 optional arguments:
-  -h, --help  show this help message and exit
+  -h, --help     show this help message and exit
+  -f, --force    whether or not to forcibly render all outputs
+  -d, --dry-run  whether or not to update output files
 
 ```
 
 ### `use`
 
 ```
 $ ./venv3.8/bin/rcmpy use -h
```

### Comparing `rcmpy-1.0.0/rcmpy.egg-info/SOURCES.txt` & `rcmpy-1.1.0/rcmpy.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 rcmpy/commands/all.py
 rcmpy/commands/apply.py
 rcmpy/commands/common.py
 rcmpy/commands/use.py
 rcmpy/commands/variant.py
 rcmpy/commands/watch.py
 rcmpy/config/__init__.py
+rcmpy/config/file.py
 rcmpy/data/schemas/Config.yaml
 rcmpy/data/schemas/ManagedFile.yaml
 rcmpy/data/schemas/State.yaml
 rcmpy/environment/__init__.py
 rcmpy/environment/base.py
 rcmpy/environment/template.py
 rcmpy/paths/__init__.py
```

### Comparing `rcmpy-1.0.0/setup.py` & `rcmpy-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.0.0/tests/test_entry.py` & `rcmpy-1.1.0/tests/test_entry.py`

 * *Files identical despite different names*

