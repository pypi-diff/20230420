# Comparing `tmp/vutils-validator-0.1.2.tar.gz` & `tmp/vutils-validator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vutils-validator-0.1.2.tar", last modified: Wed Apr 19 13:48:26 2023, max compression
+gzip compressed data, was "vutils-validator-0.1.3.tar", last modified: Thu Apr 20 20:59:56 2023, max compression
```

## Comparing `vutils-validator-0.1.2.tar` & `vutils-validator-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.521265 vutils-validator-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-19 13:48:26.521265 vutils-validator-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-19 13:48:26.521265 vutils-validator-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.513265 vutils-validator-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.513265 vutils-validator-0.1.2/src/vutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.517265 vutils-validator-0.1.2/src/vutils/validator/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/value.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.521265 vutils-validator-0.1.2/src/vutils_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-19 13:48:26.000000 vutils-validator-0.1.2/src/vutils_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-19 13:48:26.000000 vutils-validator-0.1.2/src/vutils_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:48:26.000000 vutils-validator-0.1.2/src/vutils_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:48:26.000000 vutils-validator-0.1.2/src/vutils_validator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 13:48:26.000000 vutils-validator-0.1.2/src/vutils_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 13:48:26.000000 vutils-validator-0.1.2/src/vutils_validator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.513265 vutils-validator-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.521265 vutils-validator-0.1.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/tests/unit/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/tests/unit/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/tests/unit/test_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:59:56.871439 vutils-validator-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-20 20:59:56.871439 vutils-validator-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-20 20:59:56.875439 vutils-validator-0.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:59:56.867439 vutils-validator-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:59:56.867439 vutils-validator-0.1.3/src/vutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:59:56.871439 vutils-validator-0.1.3/src/vutils/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/src/vutils/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/src/vutils/validator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/src/vutils/validator/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/src/vutils/validator/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/src/vutils/validator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/src/vutils/validator/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/src/vutils/validator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:59:56.871439 vutils-validator-0.1.3/src/vutils_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-20 20:59:56.000000 vutils-validator-0.1.3/src/vutils_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-20 20:59:56.000000 vutils-validator-0.1.3/src/vutils_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:59:56.000000 vutils-validator-0.1.3/src/vutils_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:59:56.000000 vutils-validator-0.1.3/src/vutils_validator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 20:59:56.000000 vutils-validator-0.1.3/src/vutils_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 20:59:56.000000 vutils-validator-0.1.3/src/vutils_validator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:59:56.867439 vutils-validator-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:59:56.871439 vutils-validator-0.1.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/tests/unit/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/tests/unit/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/tests/unit/test_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-20 20:59:40.000000 vutils-validator-0.1.3/tox.ini
```

### Comparing `vutils-validator-0.1.2/LICENSE` & `vutils-validator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.2/PKG-INFO` & `vutils-validator-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-validator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data validation utilities
 Home-page: https://github.com/i386x/vutils-validator
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-validator/issues
 Project-URL: Source, https://github.com/i386x/vutils-validator
```

### Comparing `vutils-validator-0.1.2/README.md` & `vutils-validator-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.2/pyproject.toml` & `vutils-validator-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.2/setup.cfg` & `vutils-validator-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.2/src/vutils/validator/basic.py` & `vutils-validator-0.1.3/src/vutils/validator/basic.py`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.2/src/vutils/validator/errors.py` & `vutils-validator-0.1.3/src/vutils/validator/errors.py`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.2/src/vutils/validator/value.py` & `vutils-validator-0.1.3/src/vutils/validator/value.py`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.2/src/vutils_validator.egg-info/PKG-INFO` & `vutils-validator-0.1.3/src/vutils_validator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-validator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data validation utilities
 Home-page: https://github.com/i386x/vutils-validator
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-validator/issues
 Project-URL: Source, https://github.com/i386x/vutils-validator
```

### Comparing `vutils-validator-0.1.2/src/vutils_validator.egg-info/SOURCES.txt` & `vutils-validator-0.1.3/src/vutils_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.2/tests/unit/test_basic.py` & `vutils-validator-0.1.3/tests/unit/test_basic.py`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.2/tests/unit/test_errors.py` & `vutils-validator-0.1.3/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.2/tests/unit/test_value.py` & `vutils-validator-0.1.3/tests/unit/test_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 # SPDX-License-Identifier: MIT
 #
 """
 Test :mod:`vutils.validator.value` module.
 
 .. |Location| replace:: :class:`~vutils.validator.value.Location`
 .. |Location.__str__| replace::
-   :meth:`~vutils.validator.value.Location.__str__`
+   :meth:`Location.__str__ <vutils.validator.value.Location.__str__>`
 .. |ValueHolder| replace:: :class:`~vutils.validator.value.ValueHolder`
 .. |ValueHolder.__str__| replace::
-   :meth:`~vutils.validator.value.ValueHolder.__str__`
+   :meth:`ValueHolder.__str__ <vutils.validator.value.ValueHolder.__str__>`
 .. |ValueHolder.detail| replace::
-   :meth:`~vutils.validator.value.ValueHolder.detail`
+   :meth:`ValueHolder.detail <vutils.validator.value.ValueHolder.detail>`
 """
 
 from vutils.testing.testcase import TestCase
 
 from vutils.validator.value import Location, ValueHolder
```

### Comparing `vutils-validator-0.1.2/tests/unit/test_version.py` & `vutils-validator-0.1.3/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.2/tox.ini` & `vutils-validator-0.1.3/tox.ini`

 * *Files identical despite different names*

