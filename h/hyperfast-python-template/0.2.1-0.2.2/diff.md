# Comparing `tmp/hyperfast_python_template-0.2.1.tar.gz` & `tmp/hyperfast_python_template-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.2.1.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.2.2.tar", max compression
```

## Comparing `hyperfast_python_template-0.2.1.tar` & `hyperfast_python_template-0.2.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1071 2023-04-20 06:56:23.756860 hyperfast_python_template-0.2.1/LICENSE
--rw-r--r--   0        0        0     5698 2023-04-20 06:56:19.212797 hyperfast_python_template-0.2.1/README.md
--rw-r--r--   0        0        0     2882 2023-04-20 06:56:40.449090 hyperfast_python_template-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6232 1970-01-01 00:00:00.000000 hyperfast_python_template-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-20 07:02:19.857720 hyperfast_python_template-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5698 2023-04-20 07:02:13.669735 hyperfast_python_template-0.2.2/README.md
+-rw-r--r--   0        0        0     2882 2023-04-20 07:02:36.561697 hyperfast_python_template-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6232 1970-01-01 00:00:00.000000 hyperfast_python_template-0.2.2/PKG-INFO
```

### Comparing `hyperfast_python_template-0.2.1/LICENSE` & `hyperfast_python_template-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.2.1/README.md` & `hyperfast_python_template-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.2.1/pyproject.toml` & `hyperfast_python_template-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.2.1"
+version = "0.2.2"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
 
 [tool.poetry.scripts]
```

### Comparing `hyperfast_python_template-0.2.1/PKG-INFO` & `hyperfast_python_template-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python template that helps you jump start your project
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

