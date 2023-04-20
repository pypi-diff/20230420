# Comparing `tmp/datasette_ml-0.1.0.tar.gz` & `tmp/datasette_ml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_ml-0.1.0.tar", max compression
+gzip compressed data, was "datasette_ml-0.1.1.tar", max compression
```

## Comparing `datasette_ml-0.1.0.tar` & `datasette_ml-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-18 16:58:09.138992 datasette_ml-0.1.0/LICENSE
--rw-r--r--   0        0        0    10370 2023-04-18 16:58:09.142992 datasette_ml-0.1.0/README.md
--rw-r--r--   0        0        0      623 2023-04-18 16:58:09.142992 datasette_ml-0.1.0/datasette_ml/__init__.py
--rw-r--r--   0        0        0     3310 2023-04-18 16:58:09.142992 datasette_ml-0.1.0/datasette_ml/sql/samples.sql
--rw-r--r--   0        0        0     2477 2023-04-18 16:58:09.142992 datasette_ml-0.1.0/datasette_ml/sql/schema.sql
--rw-r--r--   0        0        0    16409 2023-04-18 16:58:09.142992 datasette_ml-0.1.0/datasette_ml/sqml.py
--rw-r--r--   0        0        0     1347 2023-04-18 16:58:09.146993 datasette_ml-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11109 1970-01-01 00:00:00.000000 datasette_ml-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-20 15:14:46.825192 datasette_ml-0.1.1/LICENSE
+-rw-r--r--   0        0        0    10370 2023-04-20 15:14:46.825192 datasette_ml-0.1.1/README.md
+-rw-r--r--   0        0        0      632 2023-04-20 15:14:46.825192 datasette_ml-0.1.1/datasette_ml/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:14:46.825192 datasette_ml-0.1.1/datasette_ml/py.typed
+-rw-r--r--   0        0        0     1337 2023-04-20 15:14:46.833192 datasette_ml-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11094 1970-01-01 00:00:00.000000 datasette_ml-0.1.1/PKG-INFO
```

### Comparing `datasette_ml-0.1.0/LICENSE` & `datasette_ml-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette_ml-0.1.0/README.md` & `datasette_ml-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `datasette_ml-0.1.0/datasette_ml/__init__.py` & `datasette_ml-0.1.1/datasette_ml/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sqlite3
 import typing as t
 
 from datasette import hookimpl
 from datasette.database import Database
 
-from .sqml import SQML
+from sqlite_ml.sqml import SQML
 
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from datasette.app import Datasette
 
 
 sqml = SQML()
```

### Comparing `datasette_ml-0.1.0/pyproject.toml` & `datasette_ml-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "datasette-ml"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Datasette plugin providing an MLOps platform to train, eval and predict machine learning models"
 repository = "https://github.com/rclement/datasette-ml"
 authors = ["Romain Clement"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 packages = [{include = "datasette_ml"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 datasette = "*"
-scikit-learn = "*"
-pandas = "*"
+sqlite-ml = "==0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "==23.3.0"
 faker = "==18.4.0"
 flake8 = "==6.0.0"
 importlib-metadata = "==6.5.0"
 mypy = "==1.2.0"
```

### Comparing `datasette_ml-0.1.0/PKG-INFO` & `datasette_ml-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: datasette-ml
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Datasette plugin providing an MLOps platform to train, eval and predict machine learning models
 Home-page: https://github.com/rclement/datasette-ml
 License: Apache License, Version 2.0
 Author: Romain Clement
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: datasette
-Requires-Dist: pandas
-Requires-Dist: scikit-learn
+Requires-Dist: sqlite-ml (==0.1.1)
 Project-URL: Repository, https://github.com/rclement/datasette-ml
 Description-Content-Type: text/markdown
 
 # Datasette ML
 
 > Bringing Machine Learning models near your data, not the other way around!
```

