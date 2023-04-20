# Comparing `tmp/hyfi_template-0.1.1.tar.gz` & `tmp/hyfi_template-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.1.1.tar", max compression
+gzip compressed data, was "hyfi_template-0.1.2.tar", max compression
```

## Comparing `hyfi_template-0.1.1.tar` & `hyfi_template-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-04-20 03:37:27.530058 hyfi_template-0.1.1/LICENSE
--rw-r--r--   0        0        0     6602 2023-04-20 03:37:27.530058 hyfi_template-0.1.1/README.md
--rw-r--r--   0        0        0     2937 2023-04-20 03:37:50.366170 hyfi_template-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      325 2023-04-20 03:37:27.530058 hyfi_template-0.1.1/src/hyfi_template/__cli__.py
--rw-r--r--   0        0        0      135 2023-04-20 03:37:27.530058 hyfi_template-0.1.1/src/hyfi_template/__init__.py
--rw-r--r--   0        0        0       17 2023-04-20 03:37:50.306170 hyfi_template-0.1.1/src/hyfi_template/_version.py
--rw-r--r--   0        0        0        0 2023-04-20 03:37:27.530058 hyfi_template-0.1.1/src/hyfi_template/py.typed
--rw-r--r--   0        0        0     7120 1970-01-01 00:00:00.000000 hyfi_template-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-20 08:17:00.963930 hyfi_template-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6602 2023-04-20 08:17:00.963930 hyfi_template-0.1.2/README.md
+-rw-r--r--   0        0        0     2960 2023-04-20 08:28:04.482053 hyfi_template-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-04-20 08:17:00.963930 hyfi_template-0.1.2/src/hyfi_template/__cli__.py
+-rw-r--r--   0        0        0      549 2023-04-20 08:17:00.963930 hyfi_template-0.1.2/src/hyfi_template/__init__.py
+-rw-r--r--   0        0        0       17 2023-04-20 08:28:04.430052 hyfi_template-0.1.2/src/hyfi_template/_version.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:17:00.963930 hyfi_template-0.1.2/src/hyfi_template/py.typed
+-rw-r--r--   0        0        0     7156 1970-01-01 00:00:00.000000 hyfi_template-0.1.2/PKG-INFO
```

### Comparing `hyfi_template-0.1.1/LICENSE` & `hyfi_template-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.1/README.md` & `hyfi_template-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.1/pyproject.toml` & `hyfi_template-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.1.1"
+version = "0.1.2"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyfi_template", from = "src" }]
 
 [tool.poetry.scripts]
 hyfi_template = 'hyfi_template.__cli__:main'
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = ">=3.8.1,<3.12"
+hyfi = "^0.2.4"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 setuptools-scm = "^7.1.0"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
```

### Comparing `hyfi_template-0.1.1/PKG-INFO` & `hyfi_template-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.1.1
+Version: 0.1.2
 Summary: A GitHub Template Repository for HyFI-based Projects
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
+Requires-Dist: hyfi (>=0.2.4,<0.3.0)
 Description-Content-Type: text/markdown
 
 # HyFI-Template: A Template for HyFI-based Projects
 
 [![pypi-image]][pypi-url]
 [![license-image]][license-url]
 [![version-image]][release-url]
```

