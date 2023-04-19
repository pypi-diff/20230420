# Comparing `tmp/ml_botting_core-1.0.0.tar.gz` & `tmp/ml_botting_core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_botting_core-1.0.0.tar", last modified: Wed Apr 19 00:58:47 2023, max compression
+gzip compressed data, was "ml_botting_core-1.0.1.tar", last modified: Wed Apr 19 23:08:57 2023, max compression
```

## Comparing `ml_botting_core-1.0.0.tar` & `ml_botting_core-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.597889 ml_botting_core-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.597889 ml_botting_core-1.0.0/src/ml_botting_core/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.597889 ml_botting_core-1.0.0/src/ml_botting_core/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/classification/universal_classifier_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/src/ml_botting_core/model_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/model_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/model_management/download_models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/model_management/load_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/model_management/model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/src/ml_botting_core/prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/prediction/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/src/ml_botting_core/regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/src/ml_botting_core/regression/universal_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.597889 ml_botting_core-1.0.0/src/ml_botting_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-19 00:58:47.000000 ml_botting_core-1.0.0/src/ml_botting_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-19 00:58:47.000000 ml_botting_core-1.0.0/src/ml_botting_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:58:47.000000 ml_botting_core-1.0.0/src/ml_botting_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 00:58:47.000000 ml_botting_core-1.0.0/src/ml_botting_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:58:47.601889 ml_botting_core-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 00:57:27.000000 ml_botting_core-1.0.0/tests/test_universal_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.802300 ml_botting_core-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.802300 ml_botting_core-1.0.1/src/ml_botting_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/src/ml_botting_core/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/classification/universal_classifier_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/src/ml_botting_core/model_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/model_management/download_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/model_management/load_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/model_management/model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/src/ml_botting_core/prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/prediction/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/src/ml_botting_core/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/regression/universal_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/src/ml_botting_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-19 23:08:57.000000 ml_botting_core-1.0.1/src/ml_botting_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-19 23:08:57.000000 ml_botting_core-1.0.1/src/ml_botting_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:08:57.000000 ml_botting_core-1.0.1/src/ml_botting_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 23:08:57.000000 ml_botting_core-1.0.1/src/ml_botting_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/tests/test_universal_predictor.py
```

### Comparing `ml_botting_core-1.0.0/LICENSE` & `ml_botting_core-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.0/setup.cfg` & `ml_botting_core-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ml_botting_core
-version = 1.0.0
+version = 1.0.1
 author = Ryan Susman
 author_email = ryansusman@gmail.com
 description = Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/darkmatter2222/ml_botting_core
 project_urls =
```

### Comparing `ml_botting_core-1.0.0/src/ml_botting_core/base.py` & `ml_botting_core-1.0.1/src/ml_botting_core/base.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.0/src/ml_botting_core/classification/universal_classifier_trainer.py` & `ml_botting_core-1.0.1/src/ml_botting_core/classification/universal_classifier_trainer.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.0/src/ml_botting_core/model_management/download_models.py` & `ml_botting_core-1.0.1/src/ml_botting_core/model_management/download_models.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.0/src/ml_botting_core/model_management/model_manager.py` & `ml_botting_core-1.0.1/src/ml_botting_core/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.0/src/ml_botting_core/prediction/prediction.py` & `ml_botting_core-1.0.1/src/ml_botting_core/prediction/prediction.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.0/src/ml_botting_core.egg-info/SOURCES.txt` & `ml_botting_core-1.0.1/src/ml_botting_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

