# Comparing `tmp/ml_botting_core-1.0.1.tar.gz` & `tmp/ml_botting_core-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_botting_core-1.0.1.tar", last modified: Wed Apr 19 23:08:57 2023, max compression
+gzip compressed data, was "ml_botting_core-1.0.2.tar", last modified: Thu Apr 20 00:13:16 2023, max compression
```

## Comparing `ml_botting_core-1.0.1.tar` & `ml_botting_core-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.802300 ml_botting_core-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.802300 ml_botting_core-1.0.1/src/ml_botting_core/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/src/ml_botting_core/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/classification/universal_classifier_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/src/ml_botting_core/model_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/model_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/model_management/download_models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/model_management/load_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/model_management/model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/src/ml_botting_core/prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/prediction/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/src/ml_botting_core/regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/src/ml_botting_core/regression/universal_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/src/ml_botting_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-19 23:08:57.000000 ml_botting_core-1.0.1/src/ml_botting_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-19 23:08:57.000000 ml_botting_core-1.0.1/src/ml_botting_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:08:57.000000 ml_botting_core-1.0.1/src/ml_botting_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 23:08:57.000000 ml_botting_core-1.0.1/src/ml_botting_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:08:57.806300 ml_botting_core-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 23:07:38.000000 ml_botting_core-1.0.1/tests/test_universal_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.475421 ml_botting_core-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.475421 ml_botting_core-1.0.2/src/ml_botting_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/src/ml_botting_core/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/classification/universal_classifier_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/src/ml_botting_core/model_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/model_management/download_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/model_management/load_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/model_management/model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/src/ml_botting_core/prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/prediction/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/src/ml_botting_core/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/src/ml_botting_core/regression/universal_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/src/ml_botting_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-20 00:13:16.000000 ml_botting_core-1.0.2/src/ml_botting_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-20 00:13:16.000000 ml_botting_core-1.0.2/src/ml_botting_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:13:16.000000 ml_botting_core-1.0.2/src/ml_botting_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 00:13:16.000000 ml_botting_core-1.0.2/src/ml_botting_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:13:16.479421 ml_botting_core-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-20 00:11:39.000000 ml_botting_core-1.0.2/tests/test_universal_predictor.py
```

### Comparing `ml_botting_core-1.0.1/LICENSE` & `ml_botting_core-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.1/PKG-INFO` & `ml_botting_core-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_botting_core
-Version: 1.0.1
+Version: 1.0.2
 Summary: Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 Home-page: https://github.com/darkmatter2222/ml_botting_core
 Author: Ryan Susman
 Author-email: ryansusman@gmail.com
 Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml_botting_core-1.0.1/README.md` & `ml_botting_core-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.1/setup.cfg` & `ml_botting_core-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ml_botting_core
-version = 1.0.1
+version = 1.0.2
 author = Ryan Susman
 author_email = ryansusman@gmail.com
 description = Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/darkmatter2222/ml_botting_core
 project_urls =
```

### Comparing `ml_botting_core-1.0.1/src/ml_botting_core/base.py` & `ml_botting_core-1.0.2/src/ml_botting_core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
             error = "universal_predictor missing configuration"
             logger.error(error)
             raise Exception(error)
         # endregion
 
         self.classifiers = {}
         self.regressors = {}
+
+        self.load_models()
         logger.debug('universal_predictor initialized')
 
     # region ----- load
     def load_models(self):
         self.classifiers = load_models_from_config(self.config)
         return None
```

### Comparing `ml_botting_core-1.0.1/src/ml_botting_core/classification/universal_classifier_trainer.py` & `ml_botting_core-1.0.2/src/ml_botting_core/classification/universal_classifier_trainer.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.1/src/ml_botting_core/model_management/download_models.py` & `ml_botting_core-1.0.2/src/ml_botting_core/model_management/download_models.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.1/src/ml_botting_core/model_management/model_manager.py` & `ml_botting_core-1.0.2/src/ml_botting_core/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.1/src/ml_botting_core/prediction/prediction.py` & `ml_botting_core-1.0.2/src/ml_botting_core/prediction/prediction.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.1/src/ml_botting_core.egg-info/PKG-INFO` & `ml_botting_core-1.0.2/src/ml_botting_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-botting-core
-Version: 1.0.1
+Version: 1.0.2
 Summary: Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 Home-page: https://github.com/darkmatter2222/ml_botting_core
 Author: Ryan Susman
 Author-email: ryansusman@gmail.com
 Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml_botting_core-1.0.1/src/ml_botting_core.egg-info/SOURCES.txt` & `ml_botting_core-1.0.2/src/ml_botting_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

