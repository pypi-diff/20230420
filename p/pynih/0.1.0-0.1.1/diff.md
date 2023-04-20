# Comparing `tmp/pynih-0.1.0.tar.gz` & `tmp/pynih-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynih-0.1.0.tar", max compression
+gzip compressed data, was "pynih-0.1.1.tar", max compression
```

## Comparing `pynih-0.1.0.tar` & `pynih-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-19 23:22:41.416589 pynih-0.1.0/LICENSE
--rw-r--r--   0        0        0      504 2023-04-19 23:29:16.062477 pynih-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-19 23:22:41.416589 pynih-0.1.0/pynih/__init__.py
--rw-r--r--   0        0        0     3070 2023-04-19 23:22:41.416589 pynih-0.1.0/pynih/apis.py
--rw-r--r--   0        0        0      573 2023-04-19 23:23:19.432383 pynih-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 pynih-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-20 15:06:30.922387 pynih-0.1.1/LICENSE
+-rw-r--r--   0        0        0      811 2023-04-20 15:06:30.922387 pynih-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 15:06:30.922387 pynih-0.1.1/pynih/__init__.py
+-rw-r--r--   0        0        0     3070 2023-04-20 15:06:30.922387 pynih-0.1.1/pynih/apis.py
+-rw-r--r--   0        0        0      573 2023-04-20 15:06:30.922387 pynih-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 pynih-0.1.1/PKG-INFO
```

### Comparing `pynih-0.1.0/LICENSE` & `pynih-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynih-0.1.0/pynih/apis.py` & `pynih-0.1.1/pynih/apis.py`

 * *Files identical despite different names*

### Comparing `pynih-0.1.0/pyproject.toml` & `pynih-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynih"
-version = "0.1.0"
+version = "0.1.1"
 description = "python wrapper for nih reporter apis --> https://api.reporter.nih.gov/"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pynih"}]
 
 license = "MIT"
```

### Comparing `pynih-0.1.0/PKG-INFO` & `pynih-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: pynih
-Version: 0.1.0
+Version: 0.1.1
 Summary: python wrapper for nih reporter apis --> https://api.reporter.nih.gov/
 License: MIT
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
-# pynih - nih reporter api access via python
+[![Python application](https://github.com/jermwatt/pynih/actions/workflows/python-app.yml/badge.svg)](https://github.com/jermwatt/pynih/actions/workflows/python-app.yml)
 
-pynih is a python library that provides easy access to the NIH's set of [Reporter APIs](https://api.reporter.nih.gov/).
+# pynih - a Python interface for the NIH's Reporter APIs
+
+pynih is a Python library that provides easy access to the NIH's [Reporter APIs](https://api.reporter.nih.gov/).
 
 ## Installation
 
 `pip install pynih`
 
 ## Example usage
 
 ```
 from pynih import apis
 
 # illustration of project api usage
 search_criteria = {'appl_id':'9795459'}
-include_fields = ['ApplId', 'ProjectTitle', 'ProjectStart', 'Project']
+include_fields = ['ApplId', 'ProjectTitle']
 project_data = apis.query_project_api(include_fields=include_fields, search_criteria=search_criteria)
+
+# illustration of publication api usage
+search_criteria = {'pmid':'26657764'}
+publication_data = apis.query_publication_api(search_criteria=search_criteria)
 ```
```

