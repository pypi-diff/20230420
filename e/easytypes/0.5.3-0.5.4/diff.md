# Comparing `tmp/easytypes-0.5.3.tar.gz` & `tmp/easytypes-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytypes-0.5.3.tar", max compression
+gzip compressed data, was "easytypes-0.5.4.tar", max compression
```

## Comparing `easytypes-0.5.3.tar` & `easytypes-0.5.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-04-13 15:46:26.605413 easytypes-0.5.3/LICENSE
--rw-r--r--   0        0        0     2627 2023-04-13 15:46:26.605413 easytypes-0.5.3/README.md
--rw-r--r--   0        0        0      368 2023-04-13 15:46:26.605413 easytypes-0.5.3/easytypes/__init__.py
--rw-r--r--   0        0        0     4449 2023-04-13 15:46:26.605413 easytypes-0.5.3/easytypes/easytypes_impl.py
--rw-r--r--   0        0        0     4639 2023-04-13 15:46:26.605413 easytypes-0.5.3/easytypes/easytypes_test.py
--rw-r--r--   0        0        0      866 2023-04-13 15:46:26.605413 easytypes-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3597 1970-01-01 00:00:00.000000 easytypes-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-20 16:02:07.635435 easytypes-0.5.4/LICENSE
+-rw-r--r--   0        0        0     2629 2023-04-20 16:02:07.635435 easytypes-0.5.4/README.md
+-rw-r--r--   0        0        0      368 2023-04-20 16:02:07.635435 easytypes-0.5.4/easytypes/__init__.py
+-rw-r--r--   0        0        0     4449 2023-04-20 16:02:07.635435 easytypes-0.5.4/easytypes/easytypes_impl.py
+-rw-r--r--   0        0        0     4639 2023-04-20 16:02:07.635435 easytypes-0.5.4/easytypes/easytypes_test.py
+-rw-r--r--   0        0        0      866 2023-04-20 16:02:07.635435 easytypes-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 easytypes-0.5.4/PKG-INFO
```

### Comparing `easytypes-0.5.3/LICENSE` & `easytypes-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easytypes-0.5.3/README.md` & `easytypes-0.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from easytypes import disable_all_checks, enable_all_checks
 
 @safe_type  # You cannot: add new attrs; not set (or delete) the required attrs; assign wrong types
 class A:
     a: int  # Type checking, not required, no default value
     b: str = '5'  # Type checking, not required, the default value is '5'
     c: float = Required()  # Type checking, required, no default value
-    d: Tuple[int, int] = Required(2, 3)  # Type checking, required, the default value is (2, 3)
+    d: Tuple[int, int] = Required((2, 3))  # Type checking, required, the default value is (2, 3)
 ```
 ## ...and how does the class work
 ```
 va = A(a=2, b='b', c=1.0, d=(2,4))  # Ok
 assert va.a == 2
 va.a = 5
 assert va.a == 5
```

### Comparing `easytypes-0.5.3/easytypes/easytypes_impl.py` & `easytypes-0.5.4/easytypes/easytypes_impl.py`

 * *Files identical despite different names*

### Comparing `easytypes-0.5.3/easytypes/easytypes_test.py` & `easytypes-0.5.4/easytypes/easytypes_test.py`

 * *Files identical despite different names*

### Comparing `easytypes-0.5.3/pyproject.toml` & `easytypes-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easytypes"
-version = "0.5.3"
+version = "0.5.4"
 description = "Easy declaration of data structures with runtime type checking"
 authors = ["Reim, Elijah <Elijah.Reim@wartsila.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/e-reim/easytypes"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `easytypes-0.5.3/PKG-INFO` & `easytypes-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytypes
-Version: 0.5.3
+Version: 0.5.4
 Summary: Easy declaration of data structures with runtime type checking
 Home-page: https://github.com/e-reim/easytypes
 License: Apache-2.0
 Author: Reim, Elijah
 Author-email: Elijah.Reim@wartsila.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -43,15 +43,15 @@
 from easytypes import disable_all_checks, enable_all_checks
 
 @safe_type  # You cannot: add new attrs; not set (or delete) the required attrs; assign wrong types
 class A:
     a: int  # Type checking, not required, no default value
     b: str = '5'  # Type checking, not required, the default value is '5'
     c: float = Required()  # Type checking, required, no default value
-    d: Tuple[int, int] = Required(2, 3)  # Type checking, required, the default value is (2, 3)
+    d: Tuple[int, int] = Required((2, 3))  # Type checking, required, the default value is (2, 3)
 ```
 ## ...and how does the class work
 ```
 va = A(a=2, b='b', c=1.0, d=(2,4))  # Ok
 assert va.a == 2
 va.a = 5
 assert va.a == 5
```

