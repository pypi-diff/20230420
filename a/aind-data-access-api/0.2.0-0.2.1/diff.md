# Comparing `tmp/aind-data-access-api-0.2.0.tar.gz` & `tmp/aind-data-access-api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-data-access-api-0.2.0.tar", last modified: Mon Mar 27 18:22:08 2023, max compression
+gzip compressed data, was "aind-data-access-api-0.2.1.tar", last modified: Wed Apr 19 23:17:31 2023, max compression
```

## Comparing `aind-data-access-api-0.2.0.tar` & `aind-data-access-api-0.2.1.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:08.393646 aind-data-access-api-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:08.385646 aind-data-access-api-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:08.385646 aind-data-access-api-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:08.385646 aind-data-access-api-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/.github/workflows/init.yml
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-03-27 18:22:08.393646 aind-data-access-api-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:08.385646 aind-data-access-api-0.2.0/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:08.389646 aind-data-access-api-0.2.0/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:08.389646 aind-data-access-api-0.2.0/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:22:08.393646 aind-data-access-api-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:08.385646 aind-data-access-api-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:08.389646 aind-data-access-api-0.2.0/src/aind_data_access_api/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-27 18:21:48.000000 aind-data-access-api-0.2.0/src/aind_data_access_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/src/aind_data_access_api/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/src/aind_data_access_api/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/src/aind_data_access_api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/src/aind_data_access_api/rds_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:08.389646 aind-data-access-api-0.2.0/src/aind_data_access_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-03-27 18:22:08.000000 aind-data-access-api-0.2.0/src/aind_data_access_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-27 18:22:08.000000 aind-data-access-api-0.2.0/src/aind_data_access_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:22:08.000000 aind-data-access-api-0.2.0/src/aind_data_access_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-27 18:22:08.000000 aind-data-access-api-0.2.0/src/aind_data_access_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:22:08.000000 aind-data-access-api-0.2.0/src/aind_data_access_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:08.393646 aind-data-access-api-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/tests/test_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-03-27 18:21:47.000000 aind-data-access-api-0.2.0/tests/test_rds_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.355052 aind-data-access-api-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.347052 aind-data-access-api-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.github/workflows/init.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-19 23:17:31.355052 aind-data-access-api-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:17:31.355052 aind-data-access-api-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/src/aind_data_access_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/src/aind_data_access_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/src/aind_data_access_api/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/src/aind_data_access_api/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/src/aind_data_access_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/src/aind_data_access_api/rds_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/src/aind_data_access_api/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.355052 aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-19 23:17:31.000000 aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-19 23:17:31.000000 aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:17:31.000000 aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-19 23:17:31.000000 aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-19 23:17:31.000000 aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.355052 aind-data-access-api-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/tests/test_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/tests/test_rds_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/tests/test_secrets_access.py
```

### Comparing `aind-data-access-api-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/.github/ISSUE_TEMPLATE/user-story.md` & `aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/.github/workflows/init.yml` & `aind-data-access-api-0.2.1/.github/workflows/init.yml`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/.github/workflows/tag_and_publish.yml` & `aind-data-access-api-0.2.1/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/.github/workflows/test_and_lint.yml` & `aind-data-access-api-0.2.1/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/.gitignore` & `aind-data-access-api-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/LICENSE` & `aind-data-access-api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/PKG-INFO` & `aind-data-access-api-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: aind-data-access-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: API to interact with a few AIND databases
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: secrets
+Provides-Extra: full
 License-File: LICENSE
 
 # aind-data-access-api
 
 [![License](https://img.shields.io/badge/license-MIT-brightgreen)](LICENSE)
 ![Code Style](https://img.shields.io/badge/code%20style-black-black)
 [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
```

### Comparing `aind-data-access-api-0.2.0/README.md` & `aind-data-access-api-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/doc_template/Makefile` & `aind-data-access-api-0.2.1/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/doc_template/make.bat` & `aind-data-access-api-0.2.1/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/doc_template/source/_static/dark-logo.svg` & `aind-data-access-api-0.2.1/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/doc_template/source/_static/favicon.ico` & `aind-data-access-api-0.2.1/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/doc_template/source/_static/light-logo.svg` & `aind-data-access-api-0.2.1/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/doc_template/source/conf.py` & `aind-data-access-api-0.2.1/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/pyproject.toml` & `aind-data-access-api-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,33 +13,37 @@
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
 readme = "README.md"
 dynamic = ["version"]
 
 dependencies = [
-    "boto3",
-    "pandas",
-    "psycopg2-binary",
-    "pydantic",
-    "pymongo",
-    "SQLAlchemy",
+    "boto3"
 ]
 
 [project.optional-dependencies]
 dev = [
     'black',
     'coverage',
     'flake8',
     'interrogate',
     'isort',
     'Sphinx',
-    'furo'
+    'furo',
+    'aind-data-access-api[full]'
+]
+secrets = []
+full = [
+    'aind-data-access-api[secrets]',
+    "pandas",
+    "psycopg2-binary",
+    "pydantic",
+    "pymongo",
+    "SQLAlchemy",
 ]
-
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.dynamic]
 version = {attr = "aind_data_access_api.__version__"}
 
 [tool.black]
```

### Comparing `aind-data-access-api-0.2.0/src/aind_data_access_api/credentials.py` & `aind-data-access-api-0.2.1/src/aind_data_access_api/credentials.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/src/aind_data_access_api/document_store.py` & `aind-data-access-api-0.2.1/src/aind_data_access_api/document_store.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/src/aind_data_access_api/models.py` & `aind-data-access-api-0.2.1/src/aind_data_access_api/models.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/src/aind_data_access_api/rds_tables.py` & `aind-data-access-api-0.2.1/src/aind_data_access_api/rds_tables.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/src/aind_data_access_api.egg-info/PKG-INFO` & `aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: aind-data-access-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: API to interact with a few AIND databases
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: secrets
+Provides-Extra: full
 License-File: LICENSE
 
 # aind-data-access-api
 
 [![License](https://img.shields.io/badge/license-MIT-brightgreen)](LICENSE)
 ![Code Style](https://img.shields.io/badge/code%20style-black-black)
 [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
```

### Comparing `aind-data-access-api-0.2.0/src/aind_data_access_api.egg-info/SOURCES.txt` & `aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,19 @@
 doc_template/source/_static/favicon.ico
 doc_template/source/_static/light-logo.svg
 src/aind_data_access_api/__init__.py
 src/aind_data_access_api/credentials.py
 src/aind_data_access_api/document_store.py
 src/aind_data_access_api/models.py
 src/aind_data_access_api/rds_tables.py
+src/aind_data_access_api/secrets.py
 src/aind_data_access_api.egg-info/PKG-INFO
 src/aind_data_access_api.egg-info/SOURCES.txt
 src/aind_data_access_api.egg-info/dependency_links.txt
 src/aind_data_access_api.egg-info/requires.txt
 src/aind_data_access_api.egg-info/top_level.txt
 tests/__init__.py
 tests/test_credentials.py
 tests/test_document_store.py
 tests/test_models.py
-tests/test_rds_tables.py
+tests/test_rds_tables.py
+tests/test_secrets_access.py
```

### Comparing `aind-data-access-api-0.2.0/tests/test_credentials.py` & `aind-data-access-api-0.2.1/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/tests/test_document_store.py` & `aind-data-access-api-0.2.1/tests/test_document_store.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/tests/test_models.py` & `aind-data-access-api-0.2.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.0/tests/test_rds_tables.py` & `aind-data-access-api-0.2.1/tests/test_rds_tables.py`

 * *Files identical despite different names*

