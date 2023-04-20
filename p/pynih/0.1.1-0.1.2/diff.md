# Comparing `tmp/pynih-0.1.1.tar.gz` & `tmp/pynih-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynih-0.1.1.tar", max compression
+gzip compressed data, was "pynih-0.1.2.tar", max compression
```

## Comparing `pynih-0.1.1.tar` & `pynih-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-20 15:06:30.922387 pynih-0.1.1/LICENSE
--rw-r--r--   0        0        0      811 2023-04-20 15:06:30.922387 pynih-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-20 15:06:30.922387 pynih-0.1.1/pynih/__init__.py
--rw-r--r--   0        0        0     3070 2023-04-20 15:06:30.922387 pynih-0.1.1/pynih/apis.py
--rw-r--r--   0        0        0      573 2023-04-20 15:06:30.922387 pynih-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 pynih-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-20 15:11:27.766601 pynih-0.1.2/LICENSE
+-rw-r--r--   0        0        0      811 2023-04-20 15:11:27.766601 pynih-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 15:11:27.766601 pynih-0.1.2/pynih/__init__.py
+-rw-r--r--   0        0        0     3070 2023-04-20 15:11:27.766601 pynih-0.1.2/pynih/apis.py
+-rw-r--r--   0        0        0      621 2023-04-20 15:11:27.766601 pynih-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 pynih-0.1.2/PKG-INFO
```

### Comparing `pynih-0.1.1/LICENSE` & `pynih-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynih-0.1.1/README.md` & `pynih-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pynih-0.1.1/pynih/apis.py` & `pynih-0.1.2/pynih/apis.py`

 * *Files identical despite different names*

### Comparing `pynih-0.1.1/pyproject.toml` & `pynih-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [tool.poetry]
 name = "pynih"
-version = "0.1.1"
+version = "0.1.2"
 description = "python wrapper for nih reporter apis --> https://api.reporter.nih.gov/"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pynih"}]
 
 license = "MIT"
 
+homepage = "https://github.com/jermwatt/pynih"
+
 [tool.poetry.dependencies]
 python = ">=3.9.1,<3.11"
 requests = "^2.28.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 flake8 = "^4.0.1"
```

### Comparing `pynih-0.1.1/PKG-INFO` & `pynih-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pynih
-Version: 0.1.1
+Version: 0.1.2
 Summary: python wrapper for nih reporter apis --> https://api.reporter.nih.gov/
+Home-page: https://github.com/jermwatt/pynih
 License: MIT
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

