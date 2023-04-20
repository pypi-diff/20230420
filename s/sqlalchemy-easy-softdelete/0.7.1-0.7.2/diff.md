# Comparing `tmp/sqlalchemy_easy_softdelete-0.7.1.tar.gz` & `tmp/sqlalchemy_easy_softdelete-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_easy_softdelete-0.7.1.tar", max compression
+gzip compressed data, was "sqlalchemy_easy_softdelete-0.7.2.tar", max compression
```

## Comparing `sqlalchemy_easy_softdelete-0.7.1.tar` & `sqlalchemy_easy_softdelete-0.7.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1497 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/LICENSE
--rw-r--r--   0        0        0     2875 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/README.md
--rw-r--r--   0        0        0     2314 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      140 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/__init__.py
--rw-r--r--   0        0        0       65 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/handler/__init__.py
--rw-r--r--   0        0        0     6089 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py
--rw-r--r--   0        0        0      850 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py
--rw-r--r--   0        0        0     1623 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/mixin.py
--rw-r--r--   0        0        0       56 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0     1971 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/tests/conftest.py
--rw-r--r--   0        0        0     2580 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/tests/model.py
--rw-r--r--   0        0        0      360 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/tests/seed_data/__init__.py
--rw-r--r--   0        0        0     2025 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/tests/seed_data/parent_child_childchild.py
--rw-r--r--   0        0        0        0 2023-04-10 22:33:17.770859 sqlalchemy_easy_softdelete-0.7.1/tests/snapshots/__init__.py
--rw-r--r--   0        0        0     6518 2023-04-10 22:33:17.770859 sqlalchemy_easy_softdelete-0.7.1/tests/snapshots/snap_test_queries.py
--rw-r--r--   0        0        0     9931 2023-04-10 22:33:17.770859 sqlalchemy_easy_softdelete-0.7.1/tests/snapshots/snap_test_seed_data.py
--rw-r--r--   0        0        0     6340 2023-04-10 22:33:17.770859 sqlalchemy_easy_softdelete-0.7.1/tests/test_queries.py
--rw-r--r--   0        0        0      595 2023-04-10 22:33:17.770859 sqlalchemy_easy_softdelete-0.7.1/tests/test_seed_data.py
--rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-04-20 16:00:56.614862 sqlalchemy_easy_softdelete-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2875 2023-04-20 16:00:56.614862 sqlalchemy_easy_softdelete-0.7.2/README.md
+-rw-r--r--   0        0        0     2264 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/handler/__init__.py
+-rw-r--r--   0        0        0     6089 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py
+-rw-r--r--   0        0        0      850 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py
+-rw-r--r--   0        0        0     1623 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/mixin.py
+-rw-r--r--   0        0        0       56 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/__init__.py
+-rw-r--r--   0        0        0     1971 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/conftest.py
+-rw-r--r--   0        0        0     2580 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/model.py
+-rw-r--r--   0        0        0      360 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/seed_data/__init__.py
+-rw-r--r--   0        0        0     2025 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/seed_data/parent_child_childchild.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0     6518 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/snapshots/snap_test_queries.py
+-rw-r--r--   0        0        0     9931 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/snapshots/snap_test_seed_data.py
+-rw-r--r--   0        0        0     6340 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/test_queries.py
+-rw-r--r--   0        0        0      595 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/test_seed_data.py
+-rw-r--r--   0        0        0     4478 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.7.2/PKG-INFO
```

### Comparing `sqlalchemy_easy_softdelete-0.7.1/LICENSE` & `sqlalchemy_easy_softdelete-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.1/README.md` & `sqlalchemy_easy_softdelete-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.1/pyproject.toml` & `sqlalchemy_easy_softdelete-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "sqlalchemy-easy-softdelete"
-version = "0.7.1"
+version = "0.7.2"
 homepage = "https://github.com/flipbit03/sqlalchemy-easy-softdelete"
 description = "Easily add soft-deletion to your SQLAlchemy Models."
 authors = ["Cadu <cadu.coelho@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
@@ -18,16 +18,15 @@
     { include = "sqlalchemy_easy_softdelete" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 SQLAlchemy = ">=1.4,<2.1"
-certifi = ">=2022.12.07"
-cryptography = ">=38.0.3"
+
 
 black  = { version = "^21.5b2", optional = true}
 isort  = { version = "^5.8.0", optional = true}
 flake8  = { version = "^3.9.2", optional = true}
 flake8-docstrings = { version = "^1.6.0", optional = true }
 pytest  = { version = "^6.2.4", optional = true}
 pytest-cov  = { version = "^2.12.0", optional = true}
```

### Comparing `sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py` & `sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py` & `sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/mixin.py` & `sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/mixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.1/tests/conftest.py` & `sqlalchemy_easy_softdelete-0.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.1/tests/model.py` & `sqlalchemy_easy_softdelete-0.7.2/tests/model.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.1/tests/seed_data/parent_child_childchild.py` & `sqlalchemy_easy_softdelete-0.7.2/tests/seed_data/parent_child_childchild.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.1/tests/snapshots/snap_test_queries.py` & `sqlalchemy_easy_softdelete-0.7.2/tests/snapshots/snap_test_queries.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.1/tests/snapshots/snap_test_seed_data.py` & `sqlalchemy_easy_softdelete-0.7.2/tests/snapshots/snap_test_seed_data.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.1/tests/test_queries.py` & `sqlalchemy_easy_softdelete-0.7.2/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.1/tests/test_seed_data.py` & `sqlalchemy_easy_softdelete-0.7.2/tests/test_seed_data.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.1/PKG-INFO` & `sqlalchemy_easy_softdelete-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-easy-softdelete
-Version: 0.7.1
+Version: 0.7.2
 Summary: Easily add soft-deletion to your SQLAlchemy Models.
 Home-page: https://github.com/flipbit03/sqlalchemy-easy-softdelete
 License: BSD-3-Clause
 Author: Cadu
 Author-email: cadu.coelho@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,16 +17,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: dev
 Provides-Extra: test
 Requires-Dist: SQLAlchemy (>=1.4,<2.1)
 Requires-Dist: black (>=21.5b2,<22.0) ; extra == "test"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
-Requires-Dist: certifi (>=2022.12.07)
-Requires-Dist: cryptography (>=38.0.3)
 Requires-Dist: flake8 (>=3.9.2,<4.0.0) ; extra == "test"
 Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
 Requires-Dist: isort (>=5.8.0,<6.0.0) ; extra == "test"
 Requires-Dist: pip ; extra == "dev"
 Requires-Dist: pre-commit (>=2.12.0,<3.0.0) ; extra == "dev"
 Requires-Dist: pytest (>=6.2.4,<7.0.0) ; extra == "test"
 Requires-Dist: pytest-cov (>=2.12.0,<3.0.0) ; extra == "test"
```

