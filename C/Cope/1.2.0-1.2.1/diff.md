# Comparing `tmp/Cope-1.2.0.tar.gz` & `tmp/Cope-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cope-1.2.0.tar", last modified: Thu Apr 20 01:49:45 2023, max compression
+gzip compressed data, was "Cope-1.2.1.tar", last modified: Thu Apr 20 02:18:10 2023, max compression
```

## Comparing `Cope-1.2.0.tar` & `Cope-1.2.1.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 01:49:45.668332 Cope-1.2.0/
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 01:49:45.666332 Cope-1.2.0/Cope/
--rw-r--r--   0 leonard   (1000) leonard   (1000)      509 2023-04-19 19:49:02.000000 Cope-1.2.0/Cope/Psuedonym.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)       56 2023-04-19 19:39:52.000000 Cope-1.2.0/Cope/_None.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      393 2023-04-19 20:53:14.000000 Cope-1.2.0/Cope/__init__.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2410 2023-04-19 19:39:57.000000 Cope-1.2.0/Cope/bak.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     5659 2023-04-19 19:40:20.000000 Cope-1.2.0/Cope/colors.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1680 2023-04-19 19:41:11.000000 Cope-1.2.0/Cope/constants.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    16853 2023-04-20 00:39:52.000000 Cope-1.2.0/Cope/debugging.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     6994 2023-04-19 19:43:42.000000 Cope-1.2.0/Cope/decorators.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)       41 2023-04-19 20:53:26.000000 Cope-1.2.0/Cope/errors.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1678 2023-04-19 19:43:55.000000 Cope-1.2.0/Cope/func.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1762 2023-04-19 19:54:46.000000 Cope-1.2.0/Cope/geometry.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     4771 2023-04-20 01:04:12.000000 Cope-1.2.0/Cope/imports.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    19332 2023-04-19 20:04:30.000000 Cope-1.2.0/Cope/iterables.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    29346 2023-04-19 19:48:23.000000 Cope-1.2.0/Cope/key.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    10115 2023-04-20 01:12:08.000000 Cope-1.2.0/Cope/linalg.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      757 2023-04-19 19:48:30.000000 Cope-1.2.0/Cope/logging.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    12141 2023-04-19 20:47:52.000000 Cope-1.2.0/Cope/misc.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2838 2023-04-19 19:48:50.000000 Cope-1.2.0/Cope/point.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      818 2023-04-19 19:48:58.000000 Cope-1.2.0/Cope/prettyTable.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1226 2023-04-19 19:49:09.000000 Cope-1.2.0/Cope/pygame.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2325 2023-04-19 19:49:10.000000 Cope-1.2.0/Cope/timing.py
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 01:49:45.666332 Cope-1.2.0/Cope.egg-info/
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1196 2023-04-20 01:49:45.000000 Cope-1.2.0/Cope.egg-info/PKG-INFO
--rw-r--r--   0 leonard   (1000) leonard   (1000)      757 2023-04-20 01:49:45.000000 Cope-1.2.0/Cope.egg-info/SOURCES.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)        1 2023-04-20 01:49:45.000000 Cope-1.2.0/Cope.egg-info/dependency_links.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)        5 2023-04-20 01:49:45.000000 Cope-1.2.0/Cope.egg-info/top_level.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1196 2023-04-20 01:49:45.668332 Cope-1.2.0/PKG-INFO
--rw-r--r--   0 leonard   (1000) leonard   (1000)      628 2023-04-19 20:00:19.000000 Cope-1.2.0/README.md
--rw-r--r--   0 leonard   (1000) leonard   (1000)      563 2023-04-20 01:49:44.000000 Cope-1.2.0/pyproject.toml
--rw-r--r--   0 leonard   (1000) leonard   (1000)       38 2023-04-20 01:49:45.668332 Cope-1.2.0/setup.cfg
--rw-r--r--   0 leonard   (1000) leonard   (1000)      821 2023-04-20 01:39:10.000000 Cope-1.2.0/setup.py
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 01:49:45.667332 Cope-1.2.0/tests/
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1186 2022-09-10 20:02:11.000000 Cope-1.2.0/tests/test_colors.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2353 2022-10-28 20:40:40.000000 Cope-1.2.0/tests/test_debugging.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     3045 2022-09-10 20:02:11.000000 Cope-1.2.0/tests/test_decorators.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      194 2022-09-10 20:02:11.000000 Cope-1.2.0/tests/test_func.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      943 2022-09-10 20:02:11.000000 Cope-1.2.0/tests/test_geometry.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      309 2022-09-10 20:02:11.000000 Cope-1.2.0/tests/test_imports.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1743 2022-09-10 20:02:11.000000 Cope-1.2.0/tests/test_iterables.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1262 2022-09-10 20:02:11.000000 Cope-1.2.0/tests/test_key.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      228 2022-09-10 20:02:11.000000 Cope-1.2.0/tests/test_logging.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1717 2022-09-10 20:02:11.000000 Cope-1.2.0/tests/test_misc.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      462 2022-09-10 20:02:11.000000 Cope-1.2.0/tests/test_point.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      437 2022-09-10 20:02:11.000000 Cope-1.2.0/tests/test_psuedonym.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      280 2022-09-10 20:02:11.000000 Cope-1.2.0/tests/test_timing.py
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 02:18:10.876068 Cope-1.2.1/
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 02:18:10.874069 Cope-1.2.1/Cope/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      509 2023-04-19 19:49:02.000000 Cope-1.2.1/Cope/Psuedonym.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       56 2023-04-19 19:39:52.000000 Cope-1.2.1/Cope/_None.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      415 2023-04-20 02:14:29.000000 Cope-1.2.1/Cope/__init__.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2410 2023-04-19 19:39:57.000000 Cope-1.2.1/Cope/bak.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     5659 2023-04-19 19:40:20.000000 Cope-1.2.1/Cope/colors.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1680 2023-04-19 19:41:11.000000 Cope-1.2.1/Cope/constants.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    16853 2023-04-20 00:39:52.000000 Cope-1.2.1/Cope/debugging.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     6994 2023-04-19 19:43:42.000000 Cope-1.2.1/Cope/decorators.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       41 2023-04-19 20:53:26.000000 Cope-1.2.1/Cope/errors.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1678 2023-04-19 19:43:55.000000 Cope-1.2.1/Cope/func.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1762 2023-04-19 19:54:46.000000 Cope-1.2.1/Cope/geometry.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     4771 2023-04-20 01:04:12.000000 Cope-1.2.1/Cope/imports.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    19332 2023-04-19 20:04:30.000000 Cope-1.2.1/Cope/iterables.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    29346 2023-04-19 19:48:23.000000 Cope-1.2.1/Cope/key.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    10139 2023-04-20 02:17:50.000000 Cope-1.2.1/Cope/linalg.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      757 2023-04-19 19:48:30.000000 Cope-1.2.1/Cope/logging.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    12141 2023-04-19 20:47:52.000000 Cope-1.2.1/Cope/misc.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2838 2023-04-19 19:48:50.000000 Cope-1.2.1/Cope/point.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      818 2023-04-19 19:48:58.000000 Cope-1.2.1/Cope/prettyTable.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1226 2023-04-19 19:49:09.000000 Cope-1.2.1/Cope/pygame.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2325 2023-04-19 19:49:10.000000 Cope-1.2.1/Cope/timing.py
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 02:18:10.875069 Cope-1.2.1/Cope.egg-info/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2132 2023-04-20 02:18:10.000000 Cope-1.2.1/Cope.egg-info/PKG-INFO
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      796 2023-04-20 02:18:10.000000 Cope-1.2.1/Cope.egg-info/SOURCES.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)        1 2023-04-20 02:18:10.000000 Cope-1.2.1/Cope.egg-info/dependency_links.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)        5 2023-04-20 02:18:10.000000 Cope-1.2.1/Cope.egg-info/top_level.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     9755 2023-04-20 01:57:58.000000 Cope-1.2.1/LICENSE-APACHE
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1072 2023-04-20 01:57:58.000000 Cope-1.2.1/LICENSE-MIT
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       61 2023-04-20 01:57:58.000000 Cope-1.2.1/MANIFEST.in
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2132 2023-04-20 02:18:10.876068 Cope-1.2.1/PKG-INFO
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1117 2023-04-20 02:04:21.000000 Cope-1.2.1/README.md
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      448 2023-04-20 02:14:44.000000 Cope-1.2.1/pyproject.toml
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       38 2023-04-20 02:18:10.876068 Cope-1.2.1/setup.cfg
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2115 2023-04-20 02:14:35.000000 Cope-1.2.1/setup.py
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 02:18:10.876068 Cope-1.2.1/tests/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1186 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_colors.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2353 2022-10-28 20:40:40.000000 Cope-1.2.1/tests/test_debugging.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     3045 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_decorators.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      194 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_func.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      943 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_geometry.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      309 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_imports.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1743 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_iterables.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1262 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_key.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      228 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_logging.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1717 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_misc.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      462 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_point.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      437 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_psuedonym.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      280 2022-09-10 20:02:11.000000 Cope-1.2.1/tests/test_timing.py
```

### Comparing `Cope-1.2.0/Cope/bak.py` & `Cope-1.2.1/Cope/bak.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/colors.py` & `Cope-1.2.1/Cope/colors.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/constants.py` & `Cope-1.2.1/Cope/constants.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/debugging.py` & `Cope-1.2.1/Cope/debugging.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/decorators.py` & `Cope-1.2.1/Cope/decorators.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/func.py` & `Cope-1.2.1/Cope/func.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/geometry.py` & `Cope-1.2.1/Cope/geometry.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/imports.py` & `Cope-1.2.1/Cope/imports.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/iterables.py` & `Cope-1.2.1/Cope/iterables.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/key.py` & `Cope-1.2.1/Cope/key.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/linalg.py` & `Cope-1.2.1/Cope/linalg.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .debugging import debug
 from .imports import dependsOnPackage, ensureImported
 
 # import numpy as np
 # from sympy import Matrix, ImmutableMatrix, sympify, latex
 # from sympy.matrices.matrices import MatrixSubspaces
 # ensureImported('sympy', as_='sp')
+ensureImported('sympy')
 import sympy as sp
 
 
 @dependsOnPackage('clipboard', 'copy')
 @dependsOnPackage('sympy', ('Matrix', 'ImmutableMatrix', 'latex', 'sympify'))
 def matrix(string, rows=None, cols=None, cp=False, np=False, immutable=False, verbose=False):
     # from sympy import latex
```

### Comparing `Cope-1.2.0/Cope/logging.py` & `Cope-1.2.1/Cope/logging.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/misc.py` & `Cope-1.2.1/Cope/misc.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/point.py` & `Cope-1.2.1/Cope/point.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/prettyTable.py` & `Cope-1.2.1/Cope/prettyTable.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/pygame.py` & `Cope-1.2.1/Cope/pygame.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope/timing.py` & `Cope-1.2.1/Cope/timing.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/Cope.egg-info/SOURCES.txt` & `Cope-1.2.1/Cope.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+LICENSE-APACHE
+LICENSE-MIT
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 Cope/Psuedonym.py
 Cope/_None.py
 Cope/__init__.py
 Cope/bak.py
```

### Comparing `Cope-1.2.0/tests/test_colors.py` & `Cope-1.2.1/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/tests/test_debugging.py` & `Cope-1.2.1/tests/test_debugging.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/tests/test_decorators.py` & `Cope-1.2.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/tests/test_geometry.py` & `Cope-1.2.1/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/tests/test_iterables.py` & `Cope-1.2.1/tests/test_iterables.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/tests/test_key.py` & `Cope-1.2.1/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `Cope-1.2.0/tests/test_misc.py` & `Cope-1.2.1/tests/test_misc.py`

 * *Files identical despite different names*

