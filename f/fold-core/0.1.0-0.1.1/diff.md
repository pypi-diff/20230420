# Comparing `tmp/fold_core-0.1.0.tar.gz` & `tmp/fold_core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fold_core-0.1.0.tar", max compression
+gzip compressed data, was "fold_core-0.1.1.tar", max compression
```

## Comparing `fold_core-0.1.0.tar` & `fold_core-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     3870 2023-04-19 14:22:30.042023 fold_core-0.1.0/LICENSE
--rw-r--r--   0        0        0    10111 2023-04-19 14:22:30.042023 fold_core-0.1.0/README.md
--rw-r--r--   0        0        0     3768 2023-04-19 14:22:30.074022 fold_core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      474 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/__init__.py
--rw-r--r--   0        0        0     5273 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/base.py
--rw-r--r--   0        0        0      529 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/__init__.py
--rw-r--r--   0        0        0    10261 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/columns.py
--rw-r--r--   0        0        0     1577 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/common.py
--rw-r--r--   0        0        0     6272 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/concat.py
--rw-r--r--   0        0        0     2226 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/ensemble.py
--rw-r--r--   0        0        0     6359 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/metalabeling.py
--rw-r--r--   0        0        0     4760 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/residual.py
--rw-r--r--   0        0        0     3261 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/sample.py
--rw-r--r--   0        0        0     2064 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/select.py
--rw-r--r--   0        0        0     4545 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/composites/target.py
--rw-r--r--   0        0        0      345 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/__init__.py
--rw-r--r--   0        0        0     1355 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/backend/__init__.py
--rw-r--r--   0        0        0     2408 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/backend/ray.py
--rw-r--r--   0        0        0     1931 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/backend/sequential.py
--rw-r--r--   0        0        0     3198 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/backtesting.py
--rw-r--r--   0        0        0      590 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/checks.py
--rw-r--r--   0        0        0     9922 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/common.py
--rw-r--r--   0        0        0     2109 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/convenience.py
--rw-r--r--   0        0        0     7138 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/encase.py
--rw-r--r--   0        0        0     2993 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/memory.py
--rw-r--r--   0        0        0     5735 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/training.py
--rw-r--r--   0        0        0     1845 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/loop/types.py
--rw-r--r--   0        0        0      381 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/models/__init__.py
--rw-r--r--   0        0        0     3212 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/models/base.py
--rw-r--r--   0        0        0     1927 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/models/baseline.py
--rw-r--r--   0        0        0     4349 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/models/dummy.py
--rw-r--r--   0        0        0     2187 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/models/random.py
--rw-r--r--   0        0        0     4310 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/models/sklearn.py
--rw-r--r--   0        0        0        0 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/py.typed
--rw-r--r--   0        0        0     6724 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/splitters.py
--rw-r--r--   0        0        0      928 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/__init__.py
--rw-r--r--   0        0        0     6034 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/columns.py
--rw-r--r--   0        0        0     8593 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/date.py
--rw-r--r--   0        0        0     4264 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/dev.py
--rw-r--r--   0        0        0     2906 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/difference.py
--rw-r--r--   0        0        0      798 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/function.py
--rw-r--r--   0        0        0     6569 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/holidays.py
--rw-r--r--   0        0        0     5675 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/lags.py
--rw-r--r--   0        0        0     7573 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/math.py
--rw-r--r--   0        0        0     3734 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/sklearn.py
--rw-r--r--   0        0        0      887 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/update.py
--rw-r--r--   0        0        0     4414 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/transformations/window.py
--rw-r--r--   0        0        0     2171 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/utils/checks.py
--rw-r--r--   0        0        0     2240 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/utils/dataset.py
--rw-r--r--   0        0        0     1591 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/utils/list.py
--rw-r--r--   0        0        0     2955 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/utils/tests.py
--rw-r--r--   0        0        0     1716 2023-04-19 14:22:30.074022 fold_core-0.1.0/src/fold/utils/trim.py
--rw-r--r--   0        0        0    12881 1970-01-01 00:00:00.000000 fold_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3870 2023-04-20 10:26:58.907169 fold_core-0.1.1/LICENSE
+-rw-r--r--   0        0        0    10111 2023-04-20 10:26:58.907169 fold_core-0.1.1/README.md
+-rw-r--r--   0        0        0     3818 2023-04-20 10:26:58.951172 fold_core-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/__init__.py
+-rw-r--r--   0        0        0     5273 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/base.py
+-rw-r--r--   0        0        0      529 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/__init__.py
+-rw-r--r--   0        0        0    10261 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/columns.py
+-rw-r--r--   0        0        0     1577 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/common.py
+-rw-r--r--   0        0        0     6272 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/concat.py
+-rw-r--r--   0        0        0     2226 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/ensemble.py
+-rw-r--r--   0        0        0     6359 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/metalabeling.py
+-rw-r--r--   0        0        0     4760 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/residual.py
+-rw-r--r--   0        0        0     3261 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/sample.py
+-rw-r--r--   0        0        0     2064 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/select.py
+-rw-r--r--   0        0        0     4545 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/target.py
+-rw-r--r--   0        0        0      345 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/__init__.py
+-rw-r--r--   0        0        0     1355 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/backend/__init__.py
+-rw-r--r--   0        0        0     2408 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/backend/ray.py
+-rw-r--r--   0        0        0     1931 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/backend/sequential.py
+-rw-r--r--   0        0        0     3198 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/backtesting.py
+-rw-r--r--   0        0        0      590 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/checks.py
+-rw-r--r--   0        0        0     9922 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/common.py
+-rw-r--r--   0        0        0     2109 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/convenience.py
+-rw-r--r--   0        0        0     7138 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/encase.py
+-rw-r--r--   0        0        0     2993 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/memory.py
+-rw-r--r--   0        0        0     5735 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/training.py
+-rw-r--r--   0        0        0     1845 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/types.py
+-rw-r--r--   0        0        0      381 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/models/__init__.py
+-rw-r--r--   0        0        0     3212 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/models/base.py
+-rw-r--r--   0        0        0     1926 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/models/baseline.py
+-rw-r--r--   0        0        0     4349 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/models/dummy.py
+-rw-r--r--   0        0        0     2187 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/models/random.py
+-rw-r--r--   0        0        0     4310 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/models/sklearn.py
+-rw-r--r--   0        0        0        0 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/py.typed
+-rw-r--r--   0        0        0     6724 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/splitters.py
+-rw-r--r--   0        0        0      928 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/__init__.py
+-rw-r--r--   0        0        0     6034 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/columns.py
+-rw-r--r--   0        0        0     8593 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/date.py
+-rw-r--r--   0        0        0     4264 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/dev.py
+-rw-r--r--   0        0        0     2906 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/difference.py
+-rw-r--r--   0        0        0      798 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/function.py
+-rw-r--r--   0        0        0     6569 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/holidays.py
+-rw-r--r--   0        0        0     5675 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/lags.py
+-rw-r--r--   0        0        0     7573 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/math.py
+-rw-r--r--   0        0        0     3734 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/sklearn.py
+-rw-r--r--   0        0        0      887 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/update.py
+-rw-r--r--   0        0        0     4414 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/window.py
+-rw-r--r--   0        0        0     2171 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/utils/checks.py
+-rw-r--r--   0        0        0     2240 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/utils/dataset.py
+-rw-r--r--   0        0        0     1591 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/utils/list.py
+-rw-r--r--   0        0        0     2955 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/utils/tests.py
+-rw-r--r--   0        0        0     1716 2023-04-20 10:26:58.955173 fold_core-0.1.1/src/fold/utils/trim.py
+-rw-r--r--   0        0        0    12906 1970-01-01 00:00:00.000000 fold_core-0.1.1/PKG-INFO
```

### Comparing `fold_core-0.1.0/LICENSE` & `fold_core-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/README.md` & `fold_core-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/pyproject.toml` & `fold_core-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.5"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fold-core"
 packages = [
     { include="fold", from="./src" },
 ]
-version = "0.1.0"
+version = "0.1.1"
 authors = ["Mark Aron Szulyovszky", "Daniel Szemerey" ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -24,15 +24,15 @@
 ]
 description = "A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour."
 keywords = ["time-series", "machine-learning", "forecasting", "forecast", "nowcast", "models", "time-series-regression", "time-series-classification", "financial-machine-learning"]
 license = "Proprietary"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.7"
+python = ">=3.7,<4.0"
 pandas = ">=1.2"
 numpy = ">=1.16"
 scikit-learn = ">=0.22"
 tqdm = ">=4.0"
 iteration_utilities = ">=0.11"
 
 black = {version = "~=22.12.0", optional = true}
@@ -40,23 +40,24 @@
 isort = {version = "~=5.10.1", optional = true}
 pre-commit = {version = "~=2.20.0", optional = true}
 pytest = {version = "~=7.1.2", optional = true}
 pytest-cov = {version = ">=4.0", optional = true}
 imbalanced-learn = {version = ">=0.7.0", optional = true}
 holidays = {version = ">=0.10", optional = true}
 krisi = {version = "~=0.0.8", optional = true}
+mkdocs = {version = ">=1.2", optional = true}
 mkdocs-material = {version = ">=9.0.0", optional = true}
 mkdocstrings-python = {version = ">=0.9.0", optional = true}
 mkdocs-include-markdown-plugin = {version = ">=4.0", optional = true}
-mkdocs-autorefs = {version = ">=0.4.0", optional = true}
-mkdocs-jupyter = {version = ">=0.24.0", optional = true}
+mkdocs-autorefs = {version = ">=0.4", optional = true}
+mkdocs-jupyter = {version = ">=0.22", optional = true}
 image = {version = ">=1.5.33", optional = true}
-mkdocs-gallery = {version = ">=0.7.0", optional = true}
-mkdocs-glightbox = {version = ">=0.3.0", optional = true}
-ray = {version = ">=1.4.0", optional = true}
+mkdocs-gallery = {version = ">=0.7", optional = true}
+mkdocs-glightbox = {version = ">=0.3", optional = true}
+ray = {version = ">=1.4", optional = true}
 
 [project.urls]
 Documentation = "https://dream-faster.github.io/fold"
 Issues = "https://github.com/dream-faster/fold/issues"
 Source = "https://github.com/dream-faster/fold"
 
 [tool.poetry.extras]
@@ -123,15 +124,15 @@
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "0.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `fold_core-0.1.0/src/fold/base.py` & `fold_core-0.1.1/src/fold/base.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/composites/__init__.py` & `fold_core-0.1.1/src/fold/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/composites/columns.py` & `fold_core-0.1.1/src/fold/composites/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/composites/common.py` & `fold_core-0.1.1/src/fold/composites/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/composites/concat.py` & `fold_core-0.1.1/src/fold/composites/concat.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/composites/ensemble.py` & `fold_core-0.1.1/src/fold/composites/ensemble.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/composites/metalabeling.py` & `fold_core-0.1.1/src/fold/composites/metalabeling.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/composites/residual.py` & `fold_core-0.1.1/src/fold/composites/residual.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/composites/sample.py` & `fold_core-0.1.1/src/fold/composites/sample.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/composites/select.py` & `fold_core-0.1.1/src/fold/composites/select.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/composites/target.py` & `fold_core-0.1.1/src/fold/composites/target.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/loop/backend/__init__.py` & `fold_core-0.1.1/src/fold/loop/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/loop/backend/ray.py` & `fold_core-0.1.1/src/fold/loop/backend/ray.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/loop/backend/sequential.py` & `fold_core-0.1.1/src/fold/loop/backend/sequential.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/loop/backtesting.py` & `fold_core-0.1.1/src/fold/loop/backtesting.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/loop/checks.py` & `fold_core-0.1.1/src/fold/loop/checks.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/loop/common.py` & `fold_core-0.1.1/src/fold/loop/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/loop/convenience.py` & `fold_core-0.1.1/src/fold/loop/convenience.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/loop/encase.py` & `fold_core-0.1.1/src/fold/loop/encase.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/loop/memory.py` & `fold_core-0.1.1/src/fold/loop/memory.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/loop/training.py` & `fold_core-0.1.1/src/fold/loop/training.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/loop/types.py` & `fold_core-0.1.1/src/fold/loop/types.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/models/base.py` & `fold_core-0.1.1/src/fold/models/base.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/models/baseline.py` & `fold_core-0.1.1/src/fold/models/baseline.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     """
 
     name = "Naive"
     properties = TimeSeriesModel.Properties(
         requires_X=False,
         mode=TimeSeriesModel.Properties.Mode.online,
         memory_size=1,
-        _internal_supports_minibatch_backtesting=False,
+        _internal_supports_minibatch_backtesting=True,
     )
 
     def predict(
         self, X: pd.DataFrame, past_y: pd.Series
     ) -> Union[pd.Series, pd.DataFrame]:
         # it's an online transformation, so len(X) will be always 1,
         return pd.Series(past_y.iloc[-1].squeeze(), index=X.index[-1:None])
```

### Comparing `fold_core-0.1.0/src/fold/models/dummy.py` & `fold_core-0.1.1/src/fold/models/dummy.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/models/random.py` & `fold_core-0.1.1/src/fold/models/random.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/models/sklearn.py` & `fold_core-0.1.1/src/fold/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/splitters.py` & `fold_core-0.1.1/src/fold/splitters.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/transformations/__init__.py` & `fold_core-0.1.1/src/fold/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/transformations/columns.py` & `fold_core-0.1.1/src/fold/transformations/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/transformations/date.py` & `fold_core-0.1.1/src/fold/transformations/date.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/transformations/dev.py` & `fold_core-0.1.1/src/fold/transformations/dev.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/transformations/difference.py` & `fold_core-0.1.1/src/fold/transformations/difference.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/transformations/function.py` & `fold_core-0.1.1/src/fold/transformations/function.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/transformations/holidays.py` & `fold_core-0.1.1/src/fold/transformations/holidays.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/transformations/lags.py` & `fold_core-0.1.1/src/fold/transformations/lags.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/transformations/math.py` & `fold_core-0.1.1/src/fold/transformations/math.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/transformations/sklearn.py` & `fold_core-0.1.1/src/fold/transformations/sklearn.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/transformations/update.py` & `fold_core-0.1.1/src/fold/transformations/update.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/transformations/window.py` & `fold_core-0.1.1/src/fold/transformations/window.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/utils/checks.py` & `fold_core-0.1.1/src/fold/utils/checks.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/utils/dataset.py` & `fold_core-0.1.1/src/fold/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/utils/list.py` & `fold_core-0.1.1/src/fold/utils/list.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/utils/tests.py` & `fold_core-0.1.1/src/fold/utils/tests.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/src/fold/utils/trim.py` & `fold_core-0.1.1/src/fold/utils/trim.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.0/PKG-INFO` & `fold_core-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: fold-core
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour.
 License: Proprietary
 Keywords: time-series,machine-learning,forecasting,forecast,nowcast,models,time-series-regression,time-series-classification,financial-machine-learning
 Author: Mark Aron Szulyovszky
-Requires-Python: >=3.7
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -32,27 +32,28 @@
 Requires-Dist: flake8 (>=4.0.1,<4.1.0) ; extra == "quality"
 Requires-Dist: holidays (>=0.10) ; extra == "tests" or extra == "extras"
 Requires-Dist: image (>=1.5.33) ; extra == "docs"
 Requires-Dist: imbalanced-learn (>=0.7.0) ; extra == "tests"
 Requires-Dist: isort (>=5.10.1,<5.11.0) ; extra == "quality"
 Requires-Dist: iteration_utilities (>=0.11)
 Requires-Dist: krisi (>=0.0.8,<0.1.0) ; extra == "extras"
-Requires-Dist: mkdocs-autorefs (>=0.4.0) ; extra == "docs"
-Requires-Dist: mkdocs-gallery (>=0.7.0) ; extra == "docs"
-Requires-Dist: mkdocs-glightbox (>=0.3.0) ; extra == "docs"
+Requires-Dist: mkdocs (>=1.2)
+Requires-Dist: mkdocs-autorefs (>=0.4) ; extra == "docs"
+Requires-Dist: mkdocs-gallery (>=0.7) ; extra == "docs"
+Requires-Dist: mkdocs-glightbox (>=0.3) ; extra == "docs"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0) ; extra == "docs"
-Requires-Dist: mkdocs-jupyter (>=0.24.0) ; extra == "docs"
+Requires-Dist: mkdocs-jupyter (>=0.22) ; extra == "docs"
 Requires-Dist: mkdocs-material (>=9.0.0) ; extra == "docs"
 Requires-Dist: mkdocstrings-python (>=0.9.0) ; extra == "docs"
 Requires-Dist: numpy (>=1.16)
 Requires-Dist: pandas (>=1.2)
 Requires-Dist: pre-commit (>=2.20.0,<2.21.0) ; extra == "quality"
 Requires-Dist: pytest (>=7.1.2,<7.2.0) ; extra == "tests"
 Requires-Dist: pytest-cov (>=4.0) ; extra == "tests"
-Requires-Dist: ray (>=1.4.0) ; extra == "ray" or extra == "extras"
+Requires-Dist: ray (>=1.4) ; extra == "ray" or extra == "extras"
 Requires-Dist: scikit-learn (>=0.22)
 Requires-Dist: tqdm (>=4.0)
 Description-Content-Type: text/markdown
 
 <!-- # fold -->
 
 <p align="center" style="display:flex; width:100%; align-items:center; justify-content:center;">
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: fold-core Version: 0.1.0 Summary: A Time Series
+Metadata-Version: 2.1 Name: fold-core Version: 0.1.1 Summary: A Time Series
 Cross-Validation library that lets you build, deploy and update composite
 models easily. An order of magnitude speed-up, combined with flexibility and
 rigour. License: Proprietary Keywords: time-series,machine-
 learning,forecasting,forecast,nowcast,models,time-series-regression,time-
 series-classification,financial-machine-learning Author: Mark Aron Szulyovszky
-Requires-Python: >=3.7 Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: Other/Proprietary License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
+Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
+Stable Classifier: License :: Other/Proprietary License Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -19,26 +19,26 @@
 Provides-Extra: docs Provides-Extra: extras Provides-Extra: quality Provides-
 Extra: ray Provides-Extra: tests Requires-Dist: black (>=22.12.0,<22.13.0) ;
 extra == "quality" Requires-Dist: flake8 (>=4.0.1,<4.1.0) ; extra == "quality"
 Requires-Dist: holidays (>=0.10) ; extra == "tests" or extra == "extras"
 Requires-Dist: image (>=1.5.33) ; extra == "docs" Requires-Dist: imbalanced-
 learn (>=0.7.0) ; extra == "tests" Requires-Dist: isort (>=5.10.1,<5.11.0) ;
 extra == "quality" Requires-Dist: iteration_utilities (>=0.11) Requires-Dist:
-krisi (>=0.0.8,<0.1.0) ; extra == "extras" Requires-Dist: mkdocs-autorefs
-(>=0.4.0) ; extra == "docs" Requires-Dist: mkdocs-gallery (>=0.7.0) ; extra ==
-"docs" Requires-Dist: mkdocs-glightbox (>=0.3.0) ; extra == "docs" Requires-
-Dist: mkdocs-include-markdown-plugin (>=4.0) ; extra == "docs" Requires-Dist:
-mkdocs-jupyter (>=0.24.0) ; extra == "docs" Requires-Dist: mkdocs-material
-(>=9.0.0) ; extra == "docs" Requires-Dist: mkdocstrings-python (>=0.9.0) ;
-extra == "docs" Requires-Dist: numpy (>=1.16) Requires-Dist: pandas (>=1.2)
-Requires-Dist: pre-commit (>=2.20.0,<2.21.0) ; extra == "quality" Requires-
-Dist: pytest (>=7.1.2,<7.2.0) ; extra == "tests" Requires-Dist: pytest-cov
-(>=4.0) ; extra == "tests" Requires-Dist: ray (>=1.4.0) ; extra == "ray" or
-extra == "extras" Requires-Dist: scikit-learn (>=0.22) Requires-Dist: tqdm
-(>=4.0) Description-Content-Type: text/markdown
+krisi (>=0.0.8,<0.1.0) ; extra == "extras" Requires-Dist: mkdocs (>=1.2)
+Requires-Dist: mkdocs-autorefs (>=0.4) ; extra == "docs" Requires-Dist: mkdocs-
+gallery (>=0.7) ; extra == "docs" Requires-Dist: mkdocs-glightbox (>=0.3) ;
+extra == "docs" Requires-Dist: mkdocs-include-markdown-plugin (>=4.0) ; extra
+== "docs" Requires-Dist: mkdocs-jupyter (>=0.22) ; extra == "docs" Requires-
+Dist: mkdocs-material (>=9.0.0) ; extra == "docs" Requires-Dist: mkdocstrings-
+python (>=0.9.0) ; extra == "docs" Requires-Dist: numpy (>=1.16) Requires-Dist:
+pandas (>=1.2) Requires-Dist: pre-commit (>=2.20.0,<2.21.0) ; extra ==
+"quality" Requires-Dist: pytest (>=7.1.2,<7.2.0) ; extra == "tests" Requires-
+Dist: pytest-cov (>=4.0) ; extra == "tests" Requires-Dist: ray (>=1.4) ; extra
+== "ray" or extra == "extras" Requires-Dist: scikit-learn (>=0.22) Requires-
+Dist: tqdm (>=4.0) Description-Content-Type: text/markdown
       [Docs] [https://codecov.io/gh/dream-faster/fold/branch/main/graph/
 badge.svg?token=Z7I2XSF188] [Tests] [Discord_Community] [Book_a_call_with_us!]
 
                                     [Logo]
                                    **** FOLD
                                  (/fold/) ****
   A Time_Series_Continuous_Validation library that lets you build, deploy and
```

