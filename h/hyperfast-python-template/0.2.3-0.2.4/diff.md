# Comparing `tmp/hyperfast_python_template-0.2.3.tar.gz` & `tmp/hyperfast_python_template-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.2.3.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.2.4.tar", max compression
```

## Comparing `hyperfast_python_template-0.2.3.tar` & `hyperfast_python_template-0.2.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1071 2023-04-20 08:55:05.864086 hyperfast_python_template-0.2.3/LICENSE
--rw-r--r--   0        0        0     5698 2023-04-20 08:54:59.675956 hyperfast_python_template-0.2.3/README.md
--rw-r--r--   0        0        0     2889 2023-04-20 08:55:21.840434 hyperfast_python_template-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6231 1970-01-01 00:00:00.000000 hyperfast_python_template-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-20 09:03:31.481380 hyperfast_python_template-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5698 2023-04-20 09:03:20.777439 hyperfast_python_template-0.2.4/README.md
+-rw-r--r--   0        0        0     2889 2023-04-20 09:03:47.361399 hyperfast_python_template-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6231 1970-01-01 00:00:00.000000 hyperfast_python_template-0.2.4/PKG-INFO
```

### Comparing `hyperfast_python_template-0.2.3/LICENSE` & `hyperfast_python_template-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.2.3/README.md` & `hyperfast_python_template-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.2.3/pyproject.toml` & `hyperfast_python_template-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.2.3"
+version = "0.2.4"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
 
 [tool.poetry.scripts]
```

### Comparing `hyperfast_python_template-0.2.3/PKG-INFO` & `hyperfast_python_template-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.2.3
+Version: 0.2.4
 Summary: A python template that helps you jump start your project
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

