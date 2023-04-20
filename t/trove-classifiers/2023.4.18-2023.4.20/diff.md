# Comparing `tmp/trove-classifiers-2023.4.18.tar.gz` & `tmp/trove-classifiers-2023.4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trove-classifiers-2023.4.18.tar", last modified: Tue Apr 18 13:46:58 2023, max compression
+gzip compressed data, was "trove-classifiers-2023.4.20.tar", last modified: Thu Apr 20 15:34:19 2023, max compression
```

## Comparing `trove-classifiers-2023.4.18.tar` & `trove-classifiers-2023.4.20.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:46:58.637746 trove-classifiers-2023.4.18/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-18 13:46:58.637746 trove-classifiers-2023.4.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:46:58.633746 trove-classifiers-2023.4.18/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/bin/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:46:58.633746 trove-classifiers-2023.4.18/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:46:58.637746 trove-classifiers-2023.4.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:46:58.633746 trove-classifiers-2023.4.18/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:46:58.633746 trove-classifiers-2023.4.18/src/trove_classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)    39832 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/src/trove_classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/src/trove_classifiers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/src/trove_classifiers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:46:58.637746 trove-classifiers-2023.4.18/src/trove_classifiers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-18 13:46:58.000000 trove-classifiers-2023.4.18/src/trove_classifiers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-18 13:46:58.000000 trove-classifiers-2023.4.18/src/trove_classifiers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:46:58.000000 trove-classifiers-2023.4.18/src/trove_classifiers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 13:46:58.000000 trove-classifiers-2023.4.18/src/trove_classifiers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:46:58.637746 trove-classifiers-2023.4.18/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:46:58.637746 trove-classifiers-2023.4.18/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/tests/lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-18 13:46:24.000000 trove-classifiers-2023.4.18/tests/test_classifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:34:19.497183 trove-classifiers-2023.4.20/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-20 15:34:19.497183 trove-classifiers-2023.4.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:34:19.493183 trove-classifiers-2023.4.20/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/bin/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:34:19.493183 trove-classifiers-2023.4.20/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:34:19.497183 trove-classifiers-2023.4.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:34:19.493183 trove-classifiers-2023.4.20/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:34:19.493183 trove-classifiers-2023.4.20/src/trove_classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)    39865 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/src/trove_classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/src/trove_classifiers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/src/trove_classifiers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:34:19.493183 trove-classifiers-2023.4.20/src/trove_classifiers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-20 15:34:19.000000 trove-classifiers-2023.4.20/src/trove_classifiers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 15:34:19.000000 trove-classifiers-2023.4.20/src/trove_classifiers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:34:19.000000 trove-classifiers-2023.4.20/src/trove_classifiers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 15:34:19.000000 trove-classifiers-2023.4.20/src/trove_classifiers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:34:19.493183 trove-classifiers-2023.4.20/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:34:19.497183 trove-classifiers-2023.4.20/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/tests/lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-20 15:33:37.000000 trove-classifiers-2023.4.20/tests/test_classifiers.py
```

### Comparing `trove-classifiers-2023.4.18/CONTRIBUTING.md` & `trove-classifiers-2023.4.20/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.18/LICENSE` & `trove-classifiers-2023.4.20/LICENSE`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.18/Makefile` & `trove-classifiers-2023.4.20/Makefile`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.18/PKG-INFO` & `trove-classifiers-2023.4.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trove-classifiers
-Version: 2023.4.18
+Version: 2023.4.20
 Summary: Canonical source for classifiers on PyPI (pypi.org).
 Home-page: https://github.com/pypa/trove-classifiers
 Author: The PyPI Admins
 Author-email: admin@pypi.org
 Keywords: classifiers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `trove-classifiers-2023.4.18/README.md` & `trove-classifiers-2023.4.20/README.md`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.18/bin/sort.py` & `trove-classifiers-2023.4.20/bin/sort.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.18/setup.py` & `trove-classifiers-2023.4.20/setup.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.18/src/trove_classifiers/__init__.py` & `trove-classifiers-2023.4.20/src/trove_classifiers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,15 @@
     "Framework :: TurboGears :: Widgets",
     "Framework :: Twisted",
     "Framework :: Wagtail",
     "Framework :: Wagtail :: 1",
     "Framework :: Wagtail :: 2",
     "Framework :: Wagtail :: 3",
     "Framework :: Wagtail :: 4",
+    "Framework :: Wagtail :: 5",
     "Framework :: ZODB",
     "Framework :: Zope",
     "Framework :: Zope2",
     "Framework :: Zope3",
     "Framework :: Zope :: 2",
     "Framework :: Zope :: 3",
     "Framework :: Zope :: 4",
```

### Comparing `trove-classifiers-2023.4.18/src/trove_classifiers.egg-info/PKG-INFO` & `trove-classifiers-2023.4.20/src/trove_classifiers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trove-classifiers
-Version: 2023.4.18
+Version: 2023.4.20
 Summary: Canonical source for classifiers on PyPI (pypi.org).
 Home-page: https://github.com/pypa/trove-classifiers
 Author: The PyPI Admins
 Author-email: admin@pypi.org
 Keywords: classifiers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `trove-classifiers-2023.4.18/tests/lib/__init__.py` & `trove-classifiers-2023.4.20/tests/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.4.18/tests/test_classifiers.py` & `trove-classifiers-2023.4.20/tests/test_classifiers.py`

 * *Files identical despite different names*

