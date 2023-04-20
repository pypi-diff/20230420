# Comparing `tmp/hyperfast_python_template-0.2.2.tar.gz` & `tmp/hyperfast_python_template-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.2.2.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.2.3.tar", max compression
```

## Comparing `hyperfast_python_template-0.2.2.tar` & `hyperfast_python_template-0.2.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1071 2023-04-20 07:02:19.857720 hyperfast_python_template-0.2.2/LICENSE
--rw-r--r--   0        0        0     5698 2023-04-20 07:02:13.669735 hyperfast_python_template-0.2.2/README.md
--rw-r--r--   0        0        0     2882 2023-04-20 07:02:36.561697 hyperfast_python_template-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6232 1970-01-01 00:00:00.000000 hyperfast_python_template-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-20 08:55:05.864086 hyperfast_python_template-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5698 2023-04-20 08:54:59.675956 hyperfast_python_template-0.2.3/README.md
+-rw-r--r--   0        0        0     2889 2023-04-20 08:55:21.840434 hyperfast_python_template-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6231 1970-01-01 00:00:00.000000 hyperfast_python_template-0.2.3/PKG-INFO
```

### Comparing `hyperfast_python_template-0.2.2/LICENSE` & `hyperfast_python_template-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.2.2/README.md` & `hyperfast_python_template-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.2.2/pyproject.toml` & `hyperfast_python_template-0.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.2.2"
+version = "0.2.3"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
 
 [tool.poetry.scripts]
 hyperfastpy = 'hyperfastpy.__cli__:main'
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = ">=3.8.1,<3.12"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 setuptools-scm = "^7.1.0"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
```

### Comparing `hyperfast_python_template-0.2.2/PKG-INFO` & `hyperfast_python_template-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python template that helps you jump start your project
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

