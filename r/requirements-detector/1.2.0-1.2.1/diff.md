# Comparing `tmp/requirements_detector-1.2.0.tar.gz` & `tmp/requirements_detector-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirements_detector-1.2.0.tar", max compression
+gzip compressed data, was "requirements_detector-1.2.1.tar", max compression
```

## Comparing `requirements_detector-1.2.0.tar` & `requirements_detector-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1040 2022-03-19 11:44:46.946135 requirements_detector-1.2.0/LICENSE
--rw-r--r--   0        0        0     2577 2023-02-16 05:08:33.143003 requirements_detector-1.2.0/README.md
--rw-r--r--   0        0        0     1406 2023-04-20 15:33:32.678929 requirements_detector-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      269 2023-02-15 08:01:47.968235 requirements_detector-1.2.0/requirements_detector/__init__.py
--rw-r--r--   0        0        0       59 2023-02-15 07:58:21.737143 requirements_detector-1.2.0/requirements_detector/__main__.py
--rw-r--r--   0        0        0     5880 2023-04-20 15:33:19.539008 requirements_detector-1.2.0/requirements_detector/detect.py
--rw-r--r--   0        0        0      103 2022-03-19 11:44:46.950136 requirements_detector-1.2.0/requirements_detector/exceptions.py
--rw-r--r--   0        0        0      340 2023-02-15 07:58:21.737143 requirements_detector-1.2.0/requirements_detector/formatters.py
--rw-r--r--   0        0        0     3999 2023-02-15 08:48:59.156933 requirements_detector-1.2.0/requirements_detector/handle_setup.py
--rw-r--r--   0        0        0      261 2023-04-20 15:33:13.427044 requirements_detector-1.2.0/requirements_detector/poetry_semver/README.md
--rw-r--r--   0        0        0     4681 2023-04-20 15:33:13.427044 requirements_detector-1.2.0/requirements_detector/poetry_semver/__init__.py
--rw-r--r--   0        0        0      562 2023-04-20 15:33:13.427044 requirements_detector-1.2.0/requirements_detector/poetry_semver/empty_constraint.py
--rw-r--r--   0        0        0       46 2023-04-20 15:33:13.427044 requirements_detector-1.2.0/requirements_detector/poetry_semver/exceptions.py
--rw-r--r--   0        0        0      741 2023-04-20 15:33:13.427044 requirements_detector-1.2.0/requirements_detector/poetry_semver/patterns.py
--rw-r--r--   0        0        0    12192 2023-04-20 15:33:13.427044 requirements_detector-1.2.0/requirements_detector/poetry_semver/version.py
--rw-r--r--   0        0        0      870 2023-04-20 15:33:13.427044 requirements_detector-1.2.0/requirements_detector/poetry_semver/version_constraint.py
--rw-r--r--   0        0        0    13179 2023-04-20 15:33:13.427044 requirements_detector-1.2.0/requirements_detector/poetry_semver/version_range.py
--rw-r--r--   0        0        0     7931 2023-04-20 15:33:13.427044 requirements_detector-1.2.0/requirements_detector/poetry_semver/version_union.py
--rw-r--r--   0        0        0     5548 2023-02-15 08:01:47.968235 requirements_detector-1.2.0/requirements_detector/requirement.py
--rw-r--r--   0        0        0      861 2023-02-15 07:58:21.737143 requirements_detector-1.2.0/requirements_detector/run.py
--rw-r--r--   0        0        0     3566 1970-01-01 00:00:00.000000 requirements_detector-1.2.0/setup.py
--rw-r--r--   0        0        0     3899 1970-01-01 00:00:00.000000 requirements_detector-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1040 2022-03-19 11:44:46.946135 requirements_detector-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2577 2023-02-16 05:08:33.143003 requirements_detector-1.2.1/README.md
+-rw-r--r--   0        0        0     1424 2023-04-20 15:45:08.638766 requirements_detector-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      269 2023-02-15 08:01:47.968235 requirements_detector-1.2.1/requirements_detector/__init__.py
+-rw-r--r--   0        0        0       59 2023-02-15 07:58:21.737143 requirements_detector-1.2.1/requirements_detector/__main__.py
+-rw-r--r--   0        0        0     5880 2023-04-20 15:33:19.539008 requirements_detector-1.2.1/requirements_detector/detect.py
+-rw-r--r--   0        0        0      103 2022-03-19 11:44:46.950136 requirements_detector-1.2.1/requirements_detector/exceptions.py
+-rw-r--r--   0        0        0      340 2023-02-15 07:58:21.737143 requirements_detector-1.2.1/requirements_detector/formatters.py
+-rw-r--r--   0        0        0     3999 2023-02-15 08:48:59.156933 requirements_detector-1.2.1/requirements_detector/handle_setup.py
+-rw-r--r--   0        0        0      261 2023-04-20 15:33:13.427044 requirements_detector-1.2.1/requirements_detector/poetry_semver/README.md
+-rw-r--r--   0        0        0     4681 2023-04-20 15:33:13.427044 requirements_detector-1.2.1/requirements_detector/poetry_semver/__init__.py
+-rw-r--r--   0        0        0      562 2023-04-20 15:33:13.427044 requirements_detector-1.2.1/requirements_detector/poetry_semver/empty_constraint.py
+-rw-r--r--   0        0        0       46 2023-04-20 15:33:13.427044 requirements_detector-1.2.1/requirements_detector/poetry_semver/exceptions.py
+-rw-r--r--   0        0        0      741 2023-04-20 15:33:13.427044 requirements_detector-1.2.1/requirements_detector/poetry_semver/patterns.py
+-rw-r--r--   0        0        0    12192 2023-04-20 15:33:13.427044 requirements_detector-1.2.1/requirements_detector/poetry_semver/version.py
+-rw-r--r--   0        0        0      870 2023-04-20 15:33:13.427044 requirements_detector-1.2.1/requirements_detector/poetry_semver/version_constraint.py
+-rw-r--r--   0        0        0    13179 2023-04-20 15:33:13.427044 requirements_detector-1.2.1/requirements_detector/poetry_semver/version_range.py
+-rw-r--r--   0        0        0     7931 2023-04-20 15:33:13.427044 requirements_detector-1.2.1/requirements_detector/poetry_semver/version_union.py
+-rw-r--r--   0        0        0     5548 2023-02-15 08:01:47.968235 requirements_detector-1.2.1/requirements_detector/requirement.py
+-rw-r--r--   0        0        0      861 2023-02-15 07:58:21.737143 requirements_detector-1.2.1/requirements_detector/run.py
+-rw-r--r--   0        0        0     3593 1970-01-01 00:00:00.000000 requirements_detector-1.2.1/setup.py
+-rw-r--r--   0        0        0     3938 1970-01-01 00:00:00.000000 requirements_detector-1.2.1/PKG-INFO
```

### Comparing `requirements_detector-1.2.0/LICENSE` & `requirements_detector-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/README.md` & `requirements_detector-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/pyproject.toml` & `requirements_detector-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "requirements-detector"
-version = "1.2.0"
+version = "1.2.1"
 authors = ["Landscape.io <code@landscape.io>"]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Intended Audience :: Developers',
     'Operating System :: Unix',
     'Topic :: Software Development :: Quality Assurance',
@@ -32,14 +32,15 @@
 detect-requirements = 'requirements_detector.run:run'
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 astroid = "^2.0"
 packaging = ">=21.3"
 toml = "^0.10.2"
+semver = "^3.0.0"
 
 [tool.poetry.dev-dependencies]
 tox = "^3.24.5"
 pre-commit = "^2.17.0"
 pytest = "^6.2.4"
 coverage = "^5.5"
 twine = "^3.8.0"
```

### Comparing `requirements_detector-1.2.0/requirements_detector/detect.py` & `requirements_detector-1.2.1/requirements_detector/detect.py`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/requirements_detector/handle_setup.py` & `requirements_detector-1.2.1/requirements_detector/handle_setup.py`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/requirements_detector/poetry_semver/__init__.py` & `requirements_detector-1.2.1/requirements_detector/poetry_semver/__init__.py`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/requirements_detector/poetry_semver/empty_constraint.py` & `requirements_detector-1.2.1/requirements_detector/poetry_semver/empty_constraint.py`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/requirements_detector/poetry_semver/patterns.py` & `requirements_detector-1.2.1/requirements_detector/poetry_semver/patterns.py`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/requirements_detector/poetry_semver/version.py` & `requirements_detector-1.2.1/requirements_detector/poetry_semver/version.py`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/requirements_detector/poetry_semver/version_constraint.py` & `requirements_detector-1.2.1/requirements_detector/poetry_semver/version_constraint.py`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/requirements_detector/poetry_semver/version_range.py` & `requirements_detector-1.2.1/requirements_detector/poetry_semver/version_range.py`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/requirements_detector/poetry_semver/version_union.py` & `requirements_detector-1.2.1/requirements_detector/poetry_semver/version_union.py`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/requirements_detector/requirement.py` & `requirements_detector-1.2.1/requirements_detector/requirement.py`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/requirements_detector/run.py` & `requirements_detector-1.2.1/requirements_detector/run.py`

 * *Files identical despite different names*

### Comparing `requirements_detector-1.2.0/setup.py` & `requirements_detector-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 packages = \
 ['requirements_detector', 'requirements_detector.poetry_semver']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['astroid>=2.0,<3.0', 'packaging>=21.3', 'toml>=0.10.2,<0.11.0']
+['astroid>=2.0,<3.0',
+ 'packaging>=21.3',
+ 'semver>=3.0.0,<4.0.0',
+ 'toml>=0.10.2,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['detect-requirements = requirements_detector.run:run']}
 
 setup_kwargs = {
     'name': 'requirements-detector',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': 'Python tool to find and list requirements of a Python project',
     'long_description': '# Requirements Detector\n\n## Status\n\n[![Latest Version](https://img.shields.io/pypi/v/requirements-detector.svg?label=version&style=flat)](https://pypi.python.org/pypi/requirements-detector)\n[![Build Satus](https://github.com/landscapeio/requirements-detector/actions/workflows/ci.yaml/badge.svg)](https://github.com/landscapeio/requirements-detector/actions/workflows/ci.yaml)\n[![Health](https://landscape.io/github/landscapeio/requirements-detector/master/landscape.svg?style=flat)](https://landscape.io/github/landscapeio/requirements-detector/master)\n[![Coverage Status](https://img.shields.io/coveralls/landscapeio/requirements-detector.svg?style=flat)](https://coveralls.io/r/landscapeio/requirements-detector)\n[![Documentation](https://readthedocs.org/projects/requirements-detector/badge/?version=master)](https://readthedocs.org/projects/requirements-detector/)\n\n## About\n\n`requirements-detector` is a simple Python tool which attempts to find and list the requirements of a Python project.\n\nWhen run from the root of a Python project, it will try to ascertain which libraries and the versions of those libraries that the project depends on.\n\nIt uses the following methods in order, in the root of the project:\n\n1. Parse `setup.py` (if this is successful, the remaining steps are skipped)\n2. Parse `pyproject.yoml` (if a `tool.poetry.dependencies` section is found, the remaining steps are skipped)\n3. Parse `requirements.txt` or `requirements.pip`\n4. Parse all `*.txt` and `*.pip` files inside a folder called `requirements`\n5. Parse all files in the root folder matching `*requirements*.txt` or `reqs.txt` (so for example, `pip_requirements.txt` would match, as would `requirements_common.txt`)\n\n### Usage\n\n```\ndetect-requirements [path]\n```\nIf `path` is not specified, the current working directory will be used.\n\n### Output\n\nThe output will be plaintext, and match that of a [pip requirements file](http://www.pip-installer.org/en/latest/logic.html), for example:\n\n```\nDjango==1.5.2\nSouth>=0.8\nanyjson\ncelery>=2.2,<3\n```\n\n### Usage From Python\n\n```\n>>> import os\n>>> from requirements_detector import find_requirements\n>>> find_requirements(os.getcwd())\n[DetectedRequirement:Django==1.5.2, DetectedRequirement:South>=0.8, ...]\n```\n\n\nIf you know the relevant file or directory,  you can use `from_requirements_txt`, `from_setup_py` or `from_requirements_dir` directly.\n\n```\n>>> from requirements_detector import from_requirements_txt\n>>> from_requirements_txt("/path/to/requirements.txt")\n[DetectedRequirement:Django==1.5.2, DetectedRequirement:South>=0.8, ...]\n```\n',
     'author': 'Landscape.io',
     'author_email': 'code@landscape.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/landscapeio/requirements-detector',
```

### Comparing `requirements_detector-1.2.0/PKG-INFO` & `requirements_detector-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirements-detector
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python tool to find and list requirements of a Python project
 Home-page: https://github.com/landscapeio/requirements-detector
 License: MIT
 Keywords: python,requirements detector
 Author: Landscape.io
 Author-email: code@landscape.io
 Requires-Python: >=3.7,<4.0
@@ -23,14 +23,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: astroid (>=2.0,<3.0)
 Requires-Dist: packaging (>=21.3)
+Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Requirements Detector
 
 ## Status
```

