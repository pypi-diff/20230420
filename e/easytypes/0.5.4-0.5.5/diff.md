# Comparing `tmp/easytypes-0.5.4.tar.gz` & `tmp/easytypes-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytypes-0.5.4.tar", max compression
+gzip compressed data, was "easytypes-0.5.5.tar", max compression
```

## Comparing `easytypes-0.5.4.tar` & `easytypes-0.5.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-04-20 16:02:07.635435 easytypes-0.5.4/LICENSE
--rw-r--r--   0        0        0     2629 2023-04-20 16:02:07.635435 easytypes-0.5.4/README.md
--rw-r--r--   0        0        0      368 2023-04-20 16:02:07.635435 easytypes-0.5.4/easytypes/__init__.py
--rw-r--r--   0        0        0     4449 2023-04-20 16:02:07.635435 easytypes-0.5.4/easytypes/easytypes_impl.py
--rw-r--r--   0        0        0     4639 2023-04-20 16:02:07.635435 easytypes-0.5.4/easytypes/easytypes_test.py
--rw-r--r--   0        0        0      866 2023-04-20 16:02:07.635435 easytypes-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 easytypes-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-20 16:32:17.629416 easytypes-0.5.5/LICENSE
+-rw-r--r--   0        0        0     2629 2023-04-20 16:32:17.629416 easytypes-0.5.5/README.md
+-rw-r--r--   0        0        0      368 2023-04-20 16:32:17.629416 easytypes-0.5.5/easytypes/__init__.py
+-rw-r--r--   0        0        0     4457 2023-04-20 16:32:17.629416 easytypes-0.5.5/easytypes/easytypes_impl.py
+-rw-r--r--   0        0        0     4639 2023-04-20 16:32:17.629416 easytypes-0.5.5/easytypes/easytypes_test.py
+-rw-r--r--   0        0        0      866 2023-04-20 16:32:17.629416 easytypes-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 easytypes-0.5.5/PKG-INFO
```

### Comparing `easytypes-0.5.4/LICENSE` & `easytypes-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easytypes-0.5.4/README.md` & `easytypes-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `easytypes-0.5.4/easytypes/easytypes_impl.py` & `easytypes-0.5.5/easytypes/easytypes_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 from typing import Any, Type, Dict
 
 import typeguard
 
-_DISABLE_ALL_CHECKS = False
+_DISABLE_ALL_CHECKS = not __debug__
 
 
 def disable_all_checks() -> None:
     global _DISABLE_ALL_CHECKS
     _DISABLE_ALL_CHECKS = True
```

### Comparing `easytypes-0.5.4/easytypes/easytypes_test.py` & `easytypes-0.5.5/easytypes/easytypes_test.py`

 * *Files identical despite different names*

### Comparing `easytypes-0.5.4/pyproject.toml` & `easytypes-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easytypes"
-version = "0.5.4"
+version = "0.5.5"
 description = "Easy declaration of data structures with runtime type checking"
 authors = ["Reim, Elijah <Elijah.Reim@wartsila.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/e-reim/easytypes"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `easytypes-0.5.4/PKG-INFO` & `easytypes-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytypes
-Version: 0.5.4
+Version: 0.5.5
 Summary: Easy declaration of data structures with runtime type checking
 Home-page: https://github.com/e-reim/easytypes
 License: Apache-2.0
 Author: Reim, Elijah
 Author-email: Elijah.Reim@wartsila.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

