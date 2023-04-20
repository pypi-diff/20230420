# Comparing `tmp/cardsort-0.2.1.tar.gz` & `tmp/cardsort-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardsort-0.2.1.tar", max compression
+gzip compressed data, was "cardsort-0.2.2.tar", max compression
```

## Comparing `cardsort-0.2.1.tar` & `cardsort-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1077 2023-04-20 10:24:55.337721 cardsort-0.2.1/LICENSE
--rw-r--r--   0        0        0     2320 2023-04-20 10:24:55.337721 cardsort-0.2.1/README.md
--rw-r--r--   0        0        0     1330 2023-04-20 10:25:36.985576 cardsort-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      110 2023-04-20 10:24:55.341721 cardsort-0.2.1/src/cardsort/__init__.py
--rw-r--r--   0        0        0     9780 2023-04-20 10:24:55.341721 cardsort-0.2.1/src/cardsort/analysis.py
--rw-r--r--   0        0        0     3034 1970-01-01 00:00:00.000000 cardsort-0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-04-20 10:55:23.483884 cardsort-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2320 2023-04-20 10:55:23.483884 cardsort-0.2.2/README.md
+-rw-r--r--   0        0        0     1393 2023-04-20 10:56:05.635603 cardsort-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-04-20 10:55:23.487884 cardsort-0.2.2/src/cardsort/__init__.py
+-rw-r--r--   0        0        0     9780 2023-04-20 10:55:23.487884 cardsort-0.2.2/src/cardsort/analysis.py
+-rw-r--r--   0        0        0     3034 1970-01-01 00:00:00.000000 cardsort-0.2.2/PKG-INFO
```

### Comparing `cardsort-0.2.1/LICENSE` & `cardsort-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cardsort-0.2.1/README.md` & `cardsort-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cardsort-0.2.1/pyproject.toml` & `cardsort-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cardsort"
-version = "0.2.1"
+version = "0.2.2"
 description = "Analyse data from open card sorting"
 authors = ["Katharina Kloppenborg"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
@@ -27,15 +27,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version" # version location
-version_source = "tag"
+version_source = "tag"                      # getting release version from GitHub tag
 branch = "main"                             # branch to make releases of
 changelog_file = "CHANGELOG.md"             # changelog file
 build_command = "poetry build"              # build dists
 dist_path = "dist/"                         # where to put dists
 upload_to_release = true                    # auto-create GitHub release
 upload_to_pypi = false                      # don't auto-upload to PyPI
 remove_dist = false                         # don't remove dists
```

### Comparing `cardsort-0.2.1/src/cardsort/analysis.py` & `cardsort-0.2.2/src/cardsort/analysis.py`

 * *Files identical despite different names*

### Comparing `cardsort-0.2.1/PKG-INFO` & `cardsort-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardsort
-Version: 0.2.1
+Version: 0.2.2
 Summary: Analyse data from open card sorting
 License: MIT
 Author: Katharina Kloppenborg
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

