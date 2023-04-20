# Comparing `tmp/sqlite_ml-0.0.0.tar.gz` & `tmp/sqlite_ml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite_ml-0.0.0.tar", max compression
+gzip compressed data, was "sqlite_ml-0.1.0.tar", max compression
```

## Comparing `sqlite_ml-0.0.0.tar` & `sqlite_ml-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-04-20 12:02:57.379599 sqlite_ml-0.0.0/LICENSE
--rw-r--r--   0        0        0     2341 2023-04-20 12:06:29.169324 sqlite_ml-0.0.0/README.md
--rw-r--r--   0        0        0     1005 2023-04-20 13:42:28.313033 sqlite_ml-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 12:01:01.446286 sqlite_ml-0.0.0/sqlite_ml/__init__.py
--rw-r--r--   0        0        0     2477 2023-04-20 12:35:58.989987 sqlite_ml-0.0.0/sqlite_ml/sql/schema.sql
--rw-r--r--   0        0        0    16409 2023-04-20 12:07:11.449863 sqlite_ml-0.0.0/sqlite_ml/sqml.py
--rw-r--r--   0        0        0     2878 1970-01-01 00:00:00.000000 sqlite_ml-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-20 14:20:51.950911 sqlite_ml-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2842 2023-04-20 14:20:51.950911 sqlite_ml-0.1.0/README.md
+-rw-r--r--   0        0        0     1045 2023-04-20 14:20:51.950911 sqlite_ml-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 14:20:51.950911 sqlite_ml-0.1.0/sqlite_ml/__init__.py
+-rw-r--r--   0        0        0     2477 2023-04-20 14:20:51.950911 sqlite_ml-0.1.0/sqlite_ml/sql/schema.sql
+-rw-r--r--   0        0        0    16409 2023-04-20 14:20:51.950911 sqlite_ml-0.1.0/sqlite_ml/sqml.py
+-rw-r--r--   0        0        0     3419 1970-01-01 00:00:00.000000 sqlite_ml-0.1.0/PKG-INFO
```

### Comparing `sqlite_ml-0.0.0/LICENSE` & `sqlite_ml-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite_ml-0.0.0/README.md` & `sqlite_ml-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # sqlite-ml
 
 > An SQLite extension for machine learning
 
 Train machine learning models and run predictions directly from your SQLite database.
 Inspired by [PostgresML](https://postgresml.org).
 
+[![PyPI](https://img.shields.io/pypi/v/sqlite-ml.svg)](https://pypi.org/project/sqlite-ml/)
+[![CI/CD](https://github.com/rclement/sqlite-ml/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/rclement/sqlite-ml/actions/workflows/ci-cd.yml)
+[![Coverage Status](https://img.shields.io/codecov/c/github/rclement/sqlite-ml)](https://codecov.io/gh/rclement/sqlite-ml)
+[![License](https://img.shields.io/github/license/rclement/sqlite-ml)](https://github.com/rclement/sqlite-ml/blob/master/LICENSE)
+
 ## Why?
 
 Why bother running Machine Learning workloads in SQLite? Good question!
 Here are some answers:
 
 - Machine Learning number one problem is data
 - Instead of trying to bring the data to the model, why not bring a model along the data?
```

### Comparing `sqlite_ml-0.0.0/pyproject.toml` & `sqlite_ml-0.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sqlite-ml"
-version = "0.0.0"
-description = ""
+version = "0.1.0"
+description = "An SQLite extension for machine learning"
 authors = ["Romain Clement <contact@romain-clement.net>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 packages = [{include = "sqlite_ml"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `sqlite_ml-0.0.0/sqlite_ml/sql/schema.sql` & `sqlite_ml-0.1.0/sqlite_ml/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `sqlite_ml-0.0.0/sqlite_ml/sqml.py` & `sqlite_ml-0.1.0/sqlite_ml/sqml.py`

 * *Files identical despite different names*

### Comparing `sqlite_ml-0.0.0/PKG-INFO` & `sqlite_ml-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sqlite-ml
-Version: 0.0.0
-Summary: 
+Version: 0.1.0
+Summary: An SQLite extension for machine learning
 License: Apache License, Version 2.0
 Author: Romain Clement
 Author-email: contact@romain-clement.net
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -18,14 +18,19 @@
 # sqlite-ml
 
 > An SQLite extension for machine learning
 
 Train machine learning models and run predictions directly from your SQLite database.
 Inspired by [PostgresML](https://postgresml.org).
 
+[![PyPI](https://img.shields.io/pypi/v/sqlite-ml.svg)](https://pypi.org/project/sqlite-ml/)
+[![CI/CD](https://github.com/rclement/sqlite-ml/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/rclement/sqlite-ml/actions/workflows/ci-cd.yml)
+[![Coverage Status](https://img.shields.io/codecov/c/github/rclement/sqlite-ml)](https://codecov.io/gh/rclement/sqlite-ml)
+[![License](https://img.shields.io/github/license/rclement/sqlite-ml)](https://github.com/rclement/sqlite-ml/blob/master/LICENSE)
+
 ## Why?
 
 Why bother running Machine Learning workloads in SQLite? Good question!
 Here are some answers:
 
 - Machine Learning number one problem is data
 - Instead of trying to bring the data to the model, why not bring a model along the data?
```

