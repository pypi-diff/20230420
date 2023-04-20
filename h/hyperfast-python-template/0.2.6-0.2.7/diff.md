# Comparing `tmp/hyperfast_python_template-0.2.6.tar.gz` & `tmp/hyperfast_python_template-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.2.6.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.2.7.tar", max compression
```

## Comparing `hyperfast_python_template-0.2.6.tar` & `hyperfast_python_template-0.2.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1071 2023-04-20 10:23:43.279410 hyperfast_python_template-0.2.6/LICENSE
--rw-r--r--   0        0        0     5698 2023-04-20 10:23:31.539437 hyperfast_python_template-0.2.6/README.md
--rw-r--r--   0        0        0     2942 2023-04-20 10:23:59.843305 hyperfast_python_template-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     6282 1970-01-01 00:00:00.000000 hyperfast_python_template-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-20 10:55:21.898077 hyperfast_python_template-0.2.7/LICENSE
+-rw-r--r--   0        0        0     5698 2023-04-20 10:55:13.746173 hyperfast_python_template-0.2.7/README.md
+-rw-r--r--   0        0        0     2942 2023-04-20 10:55:38.693860 hyperfast_python_template-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     6282 1970-01-01 00:00:00.000000 hyperfast_python_template-0.2.7/PKG-INFO
```

### Comparing `hyperfast_python_template-0.2.6/LICENSE` & `hyperfast_python_template-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.2.6/README.md` & `hyperfast_python_template-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.2.6/pyproject.toml` & `hyperfast_python_template-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.2.6"
+version = "0.2.7"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyperfast-python.entelecheia.cc"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
```

### Comparing `hyperfast_python_template-0.2.6/PKG-INFO` & `hyperfast_python_template-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.2.6
+Version: 0.2.7
 Summary: A python template that helps you jump start your project
 Home-page: https://hyperfast-python.entelecheia.cc
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

