# Comparing `tmp/hyfi_template-0.1.4.tar.gz` & `tmp/hyfi_template-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.1.4.tar", max compression
+gzip compressed data, was "hyfi_template-0.1.5.tar", max compression
```

## Comparing `hyfi_template-0.1.4.tar` & `hyfi_template-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/LICENSE
--rw-r--r--   0        0        0     6602 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/README.md
--rw-r--r--   0        0        0     3034 2023-04-20 11:12:12.775123 hyfi_template-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      181 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/__cli__.py
--rw-r--r--   0        0        0      876 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/__init__.py
--rw-r--r--   0        0        0       22 2023-04-20 11:12:12.723122 hyfi_template-0.1.4/src/hyfi_template/_version.py
--rw-r--r--   0        0        0        0 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/conf/task/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/project.toml
--rw-r--r--   0        0        0        0 2023-04-20 11:11:46.730931 hyfi_template-0.1.4/src/hyfi_template/py.typed
--rw-r--r--   0        0        0     7250 1970-01-01 00:00:00.000000 hyfi_template-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-20 11:54:54.607942 hyfi_template-0.1.5/LICENSE
+-rw-r--r--   0        0        0     6602 2023-04-20 11:54:54.607942 hyfi_template-0.1.5/README.md
+-rw-r--r--   0        0        0     3086 2023-04-20 11:55:24.780315 hyfi_template-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      181 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/__cli__.py
+-rw-r--r--   0        0        0      882 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-20 11:55:24.728315 hyfi_template-0.1.5/src/hyfi_template/_version.py
+-rw-r--r--   0        0        0        0 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/project.toml
+-rw-r--r--   0        0        0        0 2023-04-20 11:54:54.611942 hyfi_template-0.1.5/src/hyfi_template/py.typed
+-rw-r--r--   0        0        0     7255 1970-01-01 00:00:00.000000 hyfi_template-0.1.5/PKG-INFO
```

### Comparing `hyfi_template-0.1.4/LICENSE` & `hyfi_template-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.4/README.md` & `hyfi_template-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.4/pyproject.toml` & `hyfi_template-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.1.4"
+version = "0.1.5"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/hyfi-template"
 readme = "README.md"
 packages = [{ include = "hyfi_template", from = "src" }]
 
 [tool.poetry.scripts]
 hyfi_template = 'hyfi_template.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.6"
+hyfi = {extras = ["all"], version = "^0.2.6"}
 toml = "^0.10.2"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 setuptools-scm = "^7.1.0"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
+ipykernel = "^6.22.0"
 
 [tool.black]
 exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.isort]
 profile = "black"
 skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
```

### Comparing `hyfi_template-0.1.4/src/hyfi_template/__init__.py` & `hyfi_template-0.1.5/src/hyfi_template/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 import toml
-from hyfi import about, global_config
+from hyfi import HyFI, about, global_config
 
 from ._version import __version__
 
 # Read and parse pyproject.toml
 current_dir = os.path.dirname(os.path.abspath(__file__))
 pyproject_path = os.path.join(current_dir, "project.toml")
```

### Comparing `hyfi_template-0.1.4/src/hyfi_template/conf/dotenv/__init__.yaml` & `hyfi_template-0.1.5/src/hyfi_template/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.4/src/hyfi_template/conf/hydra/help/help.yaml` & `hyfi_template-0.1.5/src/hyfi_template/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.4/src/hyfi_template/conf/mode/__init__.yaml` & `hyfi_template-0.1.5/src/hyfi_template/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.4/src/hyfi_template/conf/path/__default__.yaml` & `hyfi_template-0.1.5/src/hyfi_template/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.4/src/hyfi_template/conf/path/__init__.yaml` & `hyfi_template-0.1.5/src/hyfi_template/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.4/PKG-INFO` & `hyfi_template-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.1.4
+Version: 0.1.5
 Summary: A GitHub Template Repository for HyFI-based Projects
 Home-page: https://entelecheia.github.io/hyfi-template
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.2.6,<0.3.0)
+Requires-Dist: hyfi[all] (>=0.2.6,<0.3.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # HyFI-Template: A Template for HyFI-based Projects
 
 [![pypi-image]][pypi-url]
 [![license-image]][license-url]
```

