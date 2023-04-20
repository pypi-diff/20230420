# Comparing `tmp/fold_core-0.1.1.tar.gz` & `tmp/fold_core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fold_core-0.1.1.tar", max compression
+gzip compressed data, was "fold_core-0.1.2.tar", max compression
```

## Comparing `fold_core-0.1.1.tar` & `fold_core-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     3870 2023-04-20 10:26:58.907169 fold_core-0.1.1/LICENSE
--rw-r--r--   0        0        0    10111 2023-04-20 10:26:58.907169 fold_core-0.1.1/README.md
--rw-r--r--   0        0        0     3818 2023-04-20 10:26:58.951172 fold_core-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      474 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/__init__.py
--rw-r--r--   0        0        0     5273 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/base.py
--rw-r--r--   0        0        0      529 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/__init__.py
--rw-r--r--   0        0        0    10261 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/columns.py
--rw-r--r--   0        0        0     1577 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/common.py
--rw-r--r--   0        0        0     6272 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/concat.py
--rw-r--r--   0        0        0     2226 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/ensemble.py
--rw-r--r--   0        0        0     6359 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/metalabeling.py
--rw-r--r--   0        0        0     4760 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/residual.py
--rw-r--r--   0        0        0     3261 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/sample.py
--rw-r--r--   0        0        0     2064 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/select.py
--rw-r--r--   0        0        0     4545 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/composites/target.py
--rw-r--r--   0        0        0      345 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/__init__.py
--rw-r--r--   0        0        0     1355 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/backend/__init__.py
--rw-r--r--   0        0        0     2408 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/backend/ray.py
--rw-r--r--   0        0        0     1931 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/backend/sequential.py
--rw-r--r--   0        0        0     3198 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/backtesting.py
--rw-r--r--   0        0        0      590 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/checks.py
--rw-r--r--   0        0        0     9922 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/common.py
--rw-r--r--   0        0        0     2109 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/convenience.py
--rw-r--r--   0        0        0     7138 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/encase.py
--rw-r--r--   0        0        0     2993 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/memory.py
--rw-r--r--   0        0        0     5735 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/training.py
--rw-r--r--   0        0        0     1845 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/loop/types.py
--rw-r--r--   0        0        0      381 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/models/__init__.py
--rw-r--r--   0        0        0     3212 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/models/base.py
--rw-r--r--   0        0        0     1926 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/models/baseline.py
--rw-r--r--   0        0        0     4349 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/models/dummy.py
--rw-r--r--   0        0        0     2187 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/models/random.py
--rw-r--r--   0        0        0     4310 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/models/sklearn.py
--rw-r--r--   0        0        0        0 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/py.typed
--rw-r--r--   0        0        0     6724 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/splitters.py
--rw-r--r--   0        0        0      928 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/__init__.py
--rw-r--r--   0        0        0     6034 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/columns.py
--rw-r--r--   0        0        0     8593 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/date.py
--rw-r--r--   0        0        0     4264 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/dev.py
--rw-r--r--   0        0        0     2906 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/difference.py
--rw-r--r--   0        0        0      798 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/function.py
--rw-r--r--   0        0        0     6569 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/holidays.py
--rw-r--r--   0        0        0     5675 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/lags.py
--rw-r--r--   0        0        0     7573 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/math.py
--rw-r--r--   0        0        0     3734 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/sklearn.py
--rw-r--r--   0        0        0      887 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/update.py
--rw-r--r--   0        0        0     4414 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/transformations/window.py
--rw-r--r--   0        0        0     2171 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/utils/checks.py
--rw-r--r--   0        0        0     2240 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/utils/dataset.py
--rw-r--r--   0        0        0     1591 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/utils/list.py
--rw-r--r--   0        0        0     2955 2023-04-20 10:26:58.951172 fold_core-0.1.1/src/fold/utils/tests.py
--rw-r--r--   0        0        0     1716 2023-04-20 10:26:58.955173 fold_core-0.1.1/src/fold/utils/trim.py
--rw-r--r--   0        0        0    12906 1970-01-01 00:00:00.000000 fold_core-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3870 2023-04-20 10:47:50.852017 fold_core-0.1.2/LICENSE
+-rw-r--r--   0        0        0    10111 2023-04-20 10:47:50.852017 fold_core-0.1.2/README.md
+-rw-r--r--   0        0        0     3818 2023-04-20 10:47:50.892019 fold_core-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-04-20 10:47:50.892019 fold_core-0.1.2/src/fold/__init__.py
+-rw-r--r--   0        0        0     5273 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/base.py
+-rw-r--r--   0        0        0      529 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/__init__.py
+-rw-r--r--   0        0        0    10261 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/columns.py
+-rw-r--r--   0        0        0     1577 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/common.py
+-rw-r--r--   0        0        0     6272 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/concat.py
+-rw-r--r--   0        0        0     2226 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/ensemble.py
+-rw-r--r--   0        0        0     6359 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/metalabeling.py
+-rw-r--r--   0        0        0     4760 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/residual.py
+-rw-r--r--   0        0        0     3261 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/sample.py
+-rw-r--r--   0        0        0     2064 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/select.py
+-rw-r--r--   0        0        0     4545 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/target.py
+-rw-r--r--   0        0        0      345 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/__init__.py
+-rw-r--r--   0        0        0     1355 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/backend/__init__.py
+-rw-r--r--   0        0        0     2408 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/backend/ray.py
+-rw-r--r--   0        0        0     1931 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/backend/sequential.py
+-rw-r--r--   0        0        0     3198 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/backtesting.py
+-rw-r--r--   0        0        0      590 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/checks.py
+-rw-r--r--   0        0        0     9922 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/common.py
+-rw-r--r--   0        0        0     2109 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/convenience.py
+-rw-r--r--   0        0        0     7138 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/encase.py
+-rw-r--r--   0        0        0     2993 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/memory.py
+-rw-r--r--   0        0        0     5735 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/training.py
+-rw-r--r--   0        0        0     1845 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/types.py
+-rw-r--r--   0        0        0      381 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/models/__init__.py
+-rw-r--r--   0        0        0     3212 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/models/base.py
+-rw-r--r--   0        0        0     1926 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/models/baseline.py
+-rw-r--r--   0        0        0     4349 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/models/dummy.py
+-rw-r--r--   0        0        0     2187 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/models/random.py
+-rw-r--r--   0        0        0     4310 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/models/sklearn.py
+-rw-r--r--   0        0        0        0 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/py.typed
+-rw-r--r--   0        0        0     6724 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/splitters.py
+-rw-r--r--   0        0        0      928 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/__init__.py
+-rw-r--r--   0        0        0     6034 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/columns.py
+-rw-r--r--   0        0        0     8593 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/date.py
+-rw-r--r--   0        0        0     4264 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/dev.py
+-rw-r--r--   0        0        0     2906 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/difference.py
+-rw-r--r--   0        0        0      798 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/function.py
+-rw-r--r--   0        0        0     6569 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/holidays.py
+-rw-r--r--   0        0        0     5675 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/lags.py
+-rw-r--r--   0        0        0     7573 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/math.py
+-rw-r--r--   0        0        0     3734 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/sklearn.py
+-rw-r--r--   0        0        0      887 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/update.py
+-rw-r--r--   0        0        0     4414 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/window.py
+-rw-r--r--   0        0        0     2171 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/utils/checks.py
+-rw-r--r--   0        0        0     2240 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/utils/dataset.py
+-rw-r--r--   0        0        0     1591 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/utils/list.py
+-rw-r--r--   0        0        0     2955 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/utils/tests.py
+-rw-r--r--   0        0        0     1716 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/utils/trim.py
+-rw-r--r--   0        0        0    12906 1970-01-01 00:00:00.000000 fold_core-0.1.2/PKG-INFO
```

### Comparing `fold_core-0.1.1/LICENSE` & `fold_core-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/README.md` & `fold_core-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/pyproject.toml` & `fold_core-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fold-core"
 packages = [
     { include="fold", from="./src" },
 ]
-version = "0.1.1"
+version = "0.1.2"
 authors = ["Mark Aron Szulyovszky", "Daniel Szemerey" ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -124,15 +124,15 @@
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.1"
+current_version = "0.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `fold_core-0.1.1/src/fold/base.py` & `fold_core-0.1.2/src/fold/base.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/composites/__init__.py` & `fold_core-0.1.2/src/fold/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/composites/columns.py` & `fold_core-0.1.2/src/fold/composites/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/composites/common.py` & `fold_core-0.1.2/src/fold/composites/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/composites/concat.py` & `fold_core-0.1.2/src/fold/composites/concat.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/composites/ensemble.py` & `fold_core-0.1.2/src/fold/composites/ensemble.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/composites/metalabeling.py` & `fold_core-0.1.2/src/fold/composites/metalabeling.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/composites/residual.py` & `fold_core-0.1.2/src/fold/composites/residual.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/composites/sample.py` & `fold_core-0.1.2/src/fold/composites/sample.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/composites/select.py` & `fold_core-0.1.2/src/fold/composites/select.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/composites/target.py` & `fold_core-0.1.2/src/fold/composites/target.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/loop/backend/__init__.py` & `fold_core-0.1.2/src/fold/loop/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/loop/backend/ray.py` & `fold_core-0.1.2/src/fold/loop/backend/ray.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/loop/backend/sequential.py` & `fold_core-0.1.2/src/fold/loop/backend/sequential.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/loop/backtesting.py` & `fold_core-0.1.2/src/fold/loop/backtesting.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/loop/checks.py` & `fold_core-0.1.2/src/fold/loop/checks.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/loop/common.py` & `fold_core-0.1.2/src/fold/loop/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/loop/convenience.py` & `fold_core-0.1.2/src/fold/loop/convenience.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/loop/encase.py` & `fold_core-0.1.2/src/fold/loop/encase.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/loop/memory.py` & `fold_core-0.1.2/src/fold/loop/memory.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/loop/training.py` & `fold_core-0.1.2/src/fold/loop/training.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/loop/types.py` & `fold_core-0.1.2/src/fold/loop/types.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/models/base.py` & `fold_core-0.1.2/src/fold/models/base.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/models/baseline.py` & `fold_core-0.1.2/src/fold/models/baseline.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/models/dummy.py` & `fold_core-0.1.2/src/fold/models/dummy.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/models/random.py` & `fold_core-0.1.2/src/fold/models/random.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/models/sklearn.py` & `fold_core-0.1.2/src/fold/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/splitters.py` & `fold_core-0.1.2/src/fold/splitters.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/transformations/__init__.py` & `fold_core-0.1.2/src/fold/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/transformations/columns.py` & `fold_core-0.1.2/src/fold/transformations/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/transformations/date.py` & `fold_core-0.1.2/src/fold/transformations/date.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/transformations/dev.py` & `fold_core-0.1.2/src/fold/transformations/dev.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/transformations/difference.py` & `fold_core-0.1.2/src/fold/transformations/difference.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/transformations/function.py` & `fold_core-0.1.2/src/fold/transformations/function.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/transformations/holidays.py` & `fold_core-0.1.2/src/fold/transformations/holidays.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/transformations/lags.py` & `fold_core-0.1.2/src/fold/transformations/lags.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/transformations/math.py` & `fold_core-0.1.2/src/fold/transformations/math.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/transformations/sklearn.py` & `fold_core-0.1.2/src/fold/transformations/sklearn.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/transformations/update.py` & `fold_core-0.1.2/src/fold/transformations/update.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/transformations/window.py` & `fold_core-0.1.2/src/fold/transformations/window.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/utils/checks.py` & `fold_core-0.1.2/src/fold/utils/checks.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/utils/dataset.py` & `fold_core-0.1.2/src/fold/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/utils/list.py` & `fold_core-0.1.2/src/fold/utils/list.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/utils/tests.py` & `fold_core-0.1.2/src/fold/utils/tests.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/src/fold/utils/trim.py` & `fold_core-0.1.2/src/fold/utils/trim.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.1/PKG-INFO` & `fold_core-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fold-core
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour.
 License: Proprietary
 Keywords: time-series,machine-learning,forecasting,forecast,nowcast,models,time-series-regression,time-series-classification,financial-machine-learning
 Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fold-core Version: 0.1.1 Summary: A Time Series
+Metadata-Version: 2.1 Name: fold-core Version: 0.1.2 Summary: A Time Series
 Cross-Validation library that lets you build, deploy and update composite
 models easily. An order of magnitude speed-up, combined with flexibility and
 rigour. License: Proprietary Keywords: time-series,machine-
 learning,forecasting,forecast,nowcast,models,time-series-regression,time-
 series-classification,financial-machine-learning Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: Other/Proprietary License Classifier: Operating
```

