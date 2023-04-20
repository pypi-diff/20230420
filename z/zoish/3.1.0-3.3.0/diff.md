# Comparing `tmp/zoish-3.1.0.tar.gz` & `tmp/zoish-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoish-3.1.0.tar", max compression
+gzip compressed data, was "zoish-3.3.0.tar", max compression
```

## Comparing `zoish-3.1.0.tar` & `zoish-3.3.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1323 2023-01-12 21:31:09.498547 zoish-3.1.0/LICENSE
--rw-r--r--   0        0        0    10191 2023-02-27 01:02:37.046758 zoish-3.1.0/README.md
--rw-r--r--   0        0        0     1321 2023-02-27 01:02:37.052758 zoish-3.1.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-01-12 21:31:09.508832 zoish-3.1.0/zoish/.env
--rw-r--r--   0        0        0      925 2023-02-27 01:02:37.060758 zoish-3.1.0/zoish/__init__.py
--rw-r--r--   0        0        0     1938 2023-02-27 01:02:37.060758 zoish-3.1.0/zoish/abstracs/feature_selector_abstracts.py
--rw-r--r--   0        0        0    60046 2023-02-27 01:02:37.061758 zoish-3.1.0/zoish/base_classes/best_estimator_getters.py
--rw-r--r--   0        0        0      675 2023-02-27 01:02:37.061758 zoish-3.1.0/zoish/config.yaml
--rw-r--r--   0        0        0      375 2023-01-12 21:31:09.512696 zoish-3.1.0/zoish/decorators/decorators.py
--rw-r--r--   0        0        0        0 2023-01-12 21:31:09.513647 zoish-3.1.0/zoish/examples/__init__.py
--rw-r--r--   0        0        0    54613 2023-02-27 01:02:37.063758 zoish-3.1.0/zoish/examples/recursive_addition_features/recursive_addition_grid_search_classification.ipynb
--rw-r--r--   0        0        0    42652 2023-02-27 01:02:37.063758 zoish-3.1.0/zoish/examples/recursive_addition_features/recursive_addition_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    61640 2023-02-27 01:02:37.064758 zoish-3.1.0/zoish/examples/recursive_addition_features/recursive_addition_random_search_classification.ipynb
--rw-r--r--   0        0        0    97297 2023-02-27 01:02:37.065758 zoish-3.1.0/zoish/examples/recursive_addition_features/recursive_addition_tune_gridsearch_classification.ipynb
--rw-r--r--   0        0        0   114986 2023-02-27 01:02:37.065758 zoish-3.1.0/zoish/examples/recursive_addition_features/recursive_addition_tune_search_classification.ipynb
--rw-r--r--   0        0        0    20432 2023-02-27 01:02:37.065758 zoish-3.1.0/zoish/examples/recursive_elimination_features/recursive_elimination_grid_search_classification.ipynb
--rw-r--r--   0        0        0    40581 2023-01-12 21:31:09.518438 zoish-3.1.0/zoish/examples/recursive_elimination_features/recursive_elimination_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    63450 2023-01-12 21:31:09.519173 zoish-3.1.0/zoish/examples/recursive_elimination_features/recursive_elimination_random_search_classification.ipynb
--rw-r--r--   0        0        0    56051 2023-02-27 01:02:37.066758 zoish-3.1.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_gridsearch_classification.ipynb
--rw-r--r--   0        0        0    71923 2023-02-27 01:02:37.066758 zoish-3.1.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_search_classification.ipynb
--rw-r--r--   0        0        0    22310 2023-02-27 01:02:37.068758 zoish-3.1.0/zoish/examples/select_by_shuffling/select_by_shuffling_grid_search_classification.ipynb
--rw-r--r--   0        0        0    53217 2023-01-12 21:31:09.520669 zoish-3.1.0/zoish/examples/select_by_shuffling/select_by_shuffling_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    61941 2023-02-27 01:02:37.068758 zoish-3.1.0/zoish/examples/select_by_shuffling/select_by_shuffling_random_search_classification.ipynb
--rw-r--r--   0        0        0   102159 2023-02-27 01:02:37.069758 zoish-3.1.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_gridsearch_regression.ipynb
--rw-r--r--   0        0        0   118140 2023-02-27 01:02:37.069758 zoish-3.1.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_search_regression.ipynb
--rw-r--r--   0        0        0        0 2023-01-12 21:31:09.521837 zoish-3.1.0/zoish/examples/shap/__init__.py
--rw-r--r--   0        0        0    21194 2023-02-27 01:02:37.070758 zoish-3.1.0/zoish/examples/shap/shap_grid_search_classification.ipynb
--rw-r--r--   0        0        0    58856 2023-02-27 01:02:37.071758 zoish-3.1.0/zoish/examples/shap/shap_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    61444 2023-02-27 01:02:37.120758 zoish-3.1.0/zoish/examples/shap/shap_random_search_classification_1.ipynb
--rw-r--r--   0        0        0   413648 2023-02-27 01:02:37.142758 zoish-3.1.0/zoish/examples/shap/shap_random_search_classification_2.ipynb
--rw-r--r--   0        0        0   465032 2023-02-27 01:02:37.152758 zoish-3.1.0/zoish/examples/shap/shap_random_search_classification_3.ipynb
--rw-r--r--   0        0        0    88426 2023-02-27 01:02:37.153758 zoish-3.1.0/zoish/examples/shap/shap_tune_gridsearch_classification.ipynb
--rw-r--r--   0        0        0    69117 2023-02-27 01:02:37.153758 zoish-3.1.0/zoish/examples/shap/shap_tune_search_regression.ipynb
--rw-r--r--   0        0        0        0 2023-01-12 21:31:09.532637 zoish-3.1.0/zoish/examples/single_feature/__init__.py
--rw-r--r--   0        0        0    40086 2023-01-12 21:31:09.533153 zoish-3.1.0/zoish/examples/single_feature/single_grid_search_classification.ipynb
--rw-r--r--   0        0        0    45581 2023-01-12 21:31:09.533718 zoish-3.1.0/zoish/examples/single_feature/single_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    85377 2023-02-27 01:02:37.153758 zoish-3.1.0/zoish/examples/single_feature/single_random_search_classification.ipynb
--rw-r--r--   0        0        0   106211 2023-02-27 01:02:37.154758 zoish-3.1.0/zoish/examples/single_feature/single_tune_gridsearch_regression.ipynb
--rw-r--r--   0        0        0   122582 2023-02-27 01:02:37.154758 zoish-3.1.0/zoish/examples/single_feature/single_tune_search_regression.ipynb
--rw-r--r--   0        0        0        0 2023-01-12 21:31:09.534933 zoish-3.1.0/zoish/factories/factories.py
--rw-r--r--   0        0        0        0 2023-01-12 21:31:09.535426 zoish-3.1.0/zoish/feature_selectors/__init__.py
--rw-r--r--   0        0        0    85614 2023-02-27 01:02:37.154758 zoish-3.1.0/zoish/feature_selectors/recursive_feature_addition.py
--rw-r--r--   0        0        0    85793 2023-02-27 01:02:37.155758 zoish-3.1.0/zoish/feature_selectors/recursive_feature_elimination.py
--rw-r--r--   0        0        0    85872 2023-02-27 01:02:37.155758 zoish-3.1.0/zoish/feature_selectors/select_by_shuffling.py
--rw-r--r--   0        0        0   100851 2023-02-27 01:02:37.156758 zoish-3.1.0/zoish/feature_selectors/shap_selectors.py
--rw-r--r--   0        0        0    86006 2023-02-27 01:02:37.156758 zoish-3.1.0/zoish/feature_selectors/single_feature_selectors.py
--rw-r--r--   0        0        0        0 2023-01-12 21:31:09.538804 zoish-3.1.0/zoish/logs/zoish.log
--rw-r--r--   0        0        0        0 2023-01-12 21:31:09.539315 zoish-3.1.0/zoish/mediators/mediators.py
--rw-r--r--   0        0        0       95 2023-01-12 21:31:09.539737 zoish-3.1.0/zoish/project_conf.py
--rw-r--r--   0        0        0       48 2023-02-27 01:02:37.156758 zoish-3.1.0/zoish/version.py
--rw-r--r--   0        0        0    12127 1970-01-01 00:00:00.000000 zoish-3.1.0/setup.py
--rw-r--r--   0        0        0    11791 1970-01-01 00:00:00.000000 zoish-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1323 2023-01-12 21:31:09.498547 zoish-3.3.0/LICENSE
+-rw-r--r--   0        0        0    10737 2023-04-19 20:59:30.760192 zoish-3.3.0/README.md
+-rw-r--r--   0        0        0     1264 2023-04-20 04:38:26.470959 zoish-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-01-12 21:31:09.508832 zoish-3.3.0/zoish/.env
+-rw-r--r--   0        0        0      926 2023-04-20 04:38:26.470959 zoish-3.3.0/zoish/__init__.py
+-rw-r--r--   0        0        0     1938 2023-02-26 06:38:46.937754 zoish-3.3.0/zoish/abstracs/feature_selector_abstracts.py
+-rw-r--r--   0        0        0    60046 2023-02-26 06:38:46.939745 zoish-3.3.0/zoish/base_classes/best_estimator_getters.py
+-rw-r--r--   0        0        0      675 2023-02-26 06:38:46.941122 zoish-3.3.0/zoish/config.yaml
+-rw-r--r--   0        0        0      375 2023-01-12 21:31:09.512696 zoish-3.3.0/zoish/decorators/decorators.py
+-rw-r--r--   0        0        0        0 2023-01-12 21:31:09.513647 zoish-3.3.0/zoish/examples/__init__.py
+-rw-r--r--   0        0        0    54613 2023-02-26 06:38:46.943535 zoish-3.3.0/zoish/examples/recursive_addition_features/recursive_addition_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    42652 2023-02-26 06:38:46.945726 zoish-3.3.0/zoish/examples/recursive_addition_features/recursive_addition_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    61640 2023-02-26 06:38:46.947840 zoish-3.3.0/zoish/examples/recursive_addition_features/recursive_addition_random_search_classification.ipynb
+-rw-r--r--   0        0        0    97297 2023-02-26 06:38:46.949142 zoish-3.3.0/zoish/examples/recursive_addition_features/recursive_addition_tune_gridsearch_classification.ipynb
+-rw-r--r--   0        0        0   114986 2023-02-26 06:38:46.950149 zoish-3.3.0/zoish/examples/recursive_addition_features/recursive_addition_tune_search_classification.ipynb
+-rw-r--r--   0        0        0    20432 2023-02-26 06:38:46.952013 zoish-3.3.0/zoish/examples/recursive_elimination_features/recursive_elimination_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    40581 2023-01-12 21:31:09.518438 zoish-3.3.0/zoish/examples/recursive_elimination_features/recursive_elimination_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    63450 2023-01-12 21:31:09.519173 zoish-3.3.0/zoish/examples/recursive_elimination_features/recursive_elimination_random_search_classification.ipynb
+-rw-r--r--   0        0        0    56051 2023-02-26 06:38:46.953061 zoish-3.3.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_gridsearch_classification.ipynb
+-rw-r--r--   0        0        0    71923 2023-02-26 06:38:46.954155 zoish-3.3.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_search_classification.ipynb
+-rw-r--r--   0        0        0    22310 2023-02-26 06:38:46.955592 zoish-3.3.0/zoish/examples/select_by_shuffling/select_by_shuffling_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    53217 2023-01-12 21:31:09.520669 zoish-3.3.0/zoish/examples/select_by_shuffling/select_by_shuffling_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    61941 2023-02-26 06:38:46.956984 zoish-3.3.0/zoish/examples/select_by_shuffling/select_by_shuffling_random_search_classification.ipynb
+-rw-r--r--   0        0        0   102159 2023-02-26 06:38:46.958177 zoish-3.3.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_gridsearch_regression.ipynb
+-rw-r--r--   0        0        0   118140 2023-02-26 06:38:46.959021 zoish-3.3.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_search_regression.ipynb
+-rw-r--r--   0        0        0        0 2023-01-12 21:31:09.521837 zoish-3.3.0/zoish/examples/shap/__init__.py
+-rw-r--r--   0        0        0    21194 2023-02-26 06:38:46.960780 zoish-3.3.0/zoish/examples/shap/shap_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    58856 2023-02-26 06:38:46.962615 zoish-3.3.0/zoish/examples/shap/shap_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    61444 2023-02-26 06:38:46.968599 zoish-3.3.0/zoish/examples/shap/shap_random_search_classification_1.ipynb
+-rw-r--r--   0        0        0   413648 2023-02-26 06:38:46.973091 zoish-3.3.0/zoish/examples/shap/shap_random_search_classification_2.ipynb
+-rw-r--r--   0        0        0   465032 2023-02-26 06:38:46.975364 zoish-3.3.0/zoish/examples/shap/shap_random_search_classification_3.ipynb
+-rw-r--r--   0        0        0    88426 2023-02-26 06:38:46.976776 zoish-3.3.0/zoish/examples/shap/shap_tune_gridsearch_classification.ipynb
+-rw-r--r--   0        0        0    69117 2023-02-26 06:38:46.978221 zoish-3.3.0/zoish/examples/shap/shap_tune_search_regression.ipynb
+-rw-r--r--   0        0        0        0 2023-01-12 21:31:09.532637 zoish-3.3.0/zoish/examples/single_feature/__init__.py
+-rw-r--r--   0        0        0    40086 2023-01-12 21:31:09.533153 zoish-3.3.0/zoish/examples/single_feature/single_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    45581 2023-01-12 21:31:09.533718 zoish-3.3.0/zoish/examples/single_feature/single_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    85377 2023-02-26 06:38:46.980046 zoish-3.3.0/zoish/examples/single_feature/single_random_search_classification.ipynb
+-rw-r--r--   0        0        0   106211 2023-02-26 06:38:46.980981 zoish-3.3.0/zoish/examples/single_feature/single_tune_gridsearch_regression.ipynb
+-rw-r--r--   0        0        0   122582 2023-02-26 06:38:46.981747 zoish-3.3.0/zoish/examples/single_feature/single_tune_search_regression.ipynb
+-rw-r--r--   0        0        0        0 2023-01-12 21:31:09.534933 zoish-3.3.0/zoish/factories/factories.py
+-rw-r--r--   0        0        0        0 2023-01-12 21:31:09.535426 zoish-3.3.0/zoish/feature_selectors/__init__.py
+-rw-r--r--   0        0        0    85614 2023-02-26 06:38:46.983159 zoish-3.3.0/zoish/feature_selectors/recursive_feature_addition.py
+-rw-r--r--   0        0        0    85793 2023-02-26 06:38:46.985219 zoish-3.3.0/zoish/feature_selectors/recursive_feature_elimination.py
+-rw-r--r--   0        0        0    85872 2023-02-26 06:38:46.987033 zoish-3.3.0/zoish/feature_selectors/select_by_shuffling.py
+-rw-r--r--   0        0        0   100851 2023-02-26 06:38:46.988192 zoish-3.3.0/zoish/feature_selectors/shap_selectors.py
+-rw-r--r--   0        0        0    86006 2023-02-26 06:38:46.989316 zoish-3.3.0/zoish/feature_selectors/single_feature_selectors.py
+-rw-r--r--   0        0        0        0 2023-01-12 21:31:09.538804 zoish-3.3.0/zoish/logs/zoish.log
+-rw-r--r--   0        0        0        0 2023-01-12 21:31:09.539315 zoish-3.3.0/zoish/mediators/mediators.py
+-rw-r--r--   0        0        0       95 2023-01-12 21:31:09.539737 zoish-3.3.0/zoish/project_conf.py
+-rw-r--r--   0        0        0       48 2023-04-20 04:38:26.470959 zoish-3.3.0/zoish/version.py
+-rw-r--r--   0        0        0    12618 1970-01-01 00:00:00.000000 zoish-3.3.0/setup.py
+-rw-r--r--   0        0        0    12279 1970-01-01 00:00:00.000000 zoish-3.3.0/PKG-INFO
```

### Comparing `zoish-3.1.0/LICENSE` & `zoish-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/README.md` & `zoish-3.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+
+![GitHub Repo stars](https://img.shields.io/github/stars/TorkamaniLab/zoish?style=social) ![GitHub forks](https://img.shields.io/github/forks/TorkamaniLab/zoish?style=social) ![GitHub language count](https://img.shields.io/github/languages/count/TorkamaniLab/zoish) ![GitHub repo size](https://img.shields.io/github/repo-size/TorkamaniLab/zoish) ![GitHub](https://img.shields.io/github/license/TorkamaniLab/zoish) ![PyPI - Downloads](https://img.shields.io/pypi/dd/zoish) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zoish) 
+
 # Zoish
 
 Zoish is a package built to ease machine learning development by providing various feature-selecting modules such as:  
 - Select By Single Feature Performance
 - Recursive Feature Elimination
 - Recursive Feature Addition
 - Select By Shuffling
```

### Comparing `zoish-3.1.0/pyproject.toml` & `zoish-3.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "zoish"
-version = "3.1.0"
-description = "This project uses shapely values for selecting Top n features compatible with scikit learn pipeline"
+version = "3.3.0"
+description = "Zoish: Automated feature selectoion tools"
+
 authors = ["drhosseinjavedani <h.javedani@gmail.com>"]
 homepage = "https://github.com/drhosseinjavedani/zoish"
 license = "BSD 2-Clause License"
 
 readme = "README.md"
 keywords = [
     "Auto ML",
```

### Comparing `zoish-3.1.0/zoish/__init__.py` & `zoish-3.3.0/zoish/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-__version__ = "3.1.0"
+__version__ = "3.3.0"
+
 
 import logging
 import logging.config
 import os
 
 import yaml
 from dotenv import load_dotenv
```

### Comparing `zoish-3.1.0/zoish/abstracs/feature_selector_abstracts.py` & `zoish-3.3.0/zoish/abstracs/feature_selector_abstracts.py`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/base_classes/best_estimator_getters.py` & `zoish-3.3.0/zoish/base_classes/best_estimator_getters.py`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/config.yaml` & `zoish-3.3.0/zoish/config.yaml`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/recursive_addition_features/recursive_addition_grid_search_classification.ipynb` & `zoish-3.3.0/zoish/examples/recursive_addition_features/recursive_addition_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/recursive_addition_features/recursive_addition_optuna_search_regression.ipynb` & `zoish-3.3.0/zoish/examples/recursive_addition_features/recursive_addition_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/recursive_addition_features/recursive_addition_random_search_classification.ipynb` & `zoish-3.3.0/zoish/examples/recursive_addition_features/recursive_addition_random_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/recursive_addition_features/recursive_addition_tune_gridsearch_classification.ipynb` & `zoish-3.3.0/zoish/examples/recursive_addition_features/recursive_addition_tune_gridsearch_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/recursive_addition_features/recursive_addition_tune_search_classification.ipynb` & `zoish-3.3.0/zoish/examples/recursive_addition_features/recursive_addition_tune_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/recursive_elimination_features/recursive_elimination_grid_search_classification.ipynb` & `zoish-3.3.0/zoish/examples/recursive_elimination_features/recursive_elimination_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/recursive_elimination_features/recursive_elimination_optuna_search_regression.ipynb` & `zoish-3.3.0/zoish/examples/recursive_elimination_features/recursive_elimination_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/recursive_elimination_features/recursive_elimination_random_search_classification.ipynb` & `zoish-3.3.0/zoish/examples/recursive_elimination_features/recursive_elimination_random_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_gridsearch_classification.ipynb` & `zoish-3.3.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_gridsearch_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_search_classification.ipynb` & `zoish-3.3.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/select_by_shuffling/select_by_shuffling_grid_search_classification.ipynb` & `zoish-3.3.0/zoish/examples/select_by_shuffling/select_by_shuffling_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/select_by_shuffling/select_by_shuffling_optuna_search_regression.ipynb` & `zoish-3.3.0/zoish/examples/select_by_shuffling/select_by_shuffling_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/select_by_shuffling/select_by_shuffling_random_search_classification.ipynb` & `zoish-3.3.0/zoish/examples/select_by_shuffling/select_by_shuffling_random_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_gridsearch_regression.ipynb` & `zoish-3.3.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_gridsearch_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_search_regression.ipynb` & `zoish-3.3.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/shap/shap_grid_search_classification.ipynb` & `zoish-3.3.0/zoish/examples/shap/shap_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/shap/shap_optuna_search_regression.ipynb` & `zoish-3.3.0/zoish/examples/shap/shap_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/shap/shap_random_search_classification_1.ipynb` & `zoish-3.3.0/zoish/examples/shap/shap_random_search_classification_1.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/shap/shap_random_search_classification_2.ipynb` & `zoish-3.3.0/zoish/examples/shap/shap_random_search_classification_2.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/shap/shap_random_search_classification_3.ipynb` & `zoish-3.3.0/zoish/examples/shap/shap_random_search_classification_3.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/shap/shap_tune_gridsearch_classification.ipynb` & `zoish-3.3.0/zoish/examples/shap/shap_tune_gridsearch_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/shap/shap_tune_search_regression.ipynb` & `zoish-3.3.0/zoish/examples/shap/shap_tune_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/single_feature/single_grid_search_classification.ipynb` & `zoish-3.3.0/zoish/examples/single_feature/single_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/single_feature/single_optuna_search_regression.ipynb` & `zoish-3.3.0/zoish/examples/single_feature/single_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/single_feature/single_random_search_classification.ipynb` & `zoish-3.3.0/zoish/examples/single_feature/single_random_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/single_feature/single_tune_gridsearch_regression.ipynb` & `zoish-3.3.0/zoish/examples/single_feature/single_tune_gridsearch_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/examples/single_feature/single_tune_search_regression.ipynb` & `zoish-3.3.0/zoish/examples/single_feature/single_tune_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/feature_selectors/recursive_feature_addition.py` & `zoish-3.3.0/zoish/feature_selectors/recursive_feature_addition.py`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/feature_selectors/recursive_feature_elimination.py` & `zoish-3.3.0/zoish/feature_selectors/recursive_feature_elimination.py`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/feature_selectors/select_by_shuffling.py` & `zoish-3.3.0/zoish/feature_selectors/select_by_shuffling.py`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/feature_selectors/shap_selectors.py` & `zoish-3.3.0/zoish/feature_selectors/shap_selectors.py`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/zoish/feature_selectors/single_feature_selectors.py` & `zoish-3.3.0/zoish/feature_selectors/single_feature_selectors.py`

 * *Files identical despite different names*

### Comparing `zoish-3.1.0/setup.py` & `zoish-3.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,17 +42,17 @@
  'scipy>=1.8.1,<2.0.0',
  'shap>=0.41.0,<0.42.0',
  'xgboost>=1.6.1,<2.0.0',
  'xgbse>=0.2.3,<0.3.0']
 
 setup_kwargs = {
     'name': 'zoish',
-    'version': '3.1.0',
-    'description': 'This project uses shapely values for selecting Top n features compatible with scikit learn pipeline',
-    'long_description': '# Zoish\n\nZoish is a package built to ease machine learning development by providing various feature-selecting modules such as:  \n- Select By Single Feature Performance\n- Recursive Feature Elimination\n- Recursive Feature Addition\n- Select By Shuffling\n\nAll of them are compatible with [scikit-learn](https://scikit-learn.org) pipeline. \n\n\n## Introduction\n\nAll of the above-mentioned modules of Zoish have class factories that have various methods and parameters. From an estimator to its tunning parameters and from optimizers to their parameters, the final goal is to automate the feature selection of the ML pipeline in a proper way. Optimizers like [Optuna](https://optuna.org/), [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html) , [RandomizedSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html), [TuneGridSearchCV, and TuneSearchCV](https://github.com/ray-project/tune-sklearn) has critical role in Zoish. They are used to provide the best estimator on a train set that is later used by feature selectors to check what features can improve the accuracy of this best estimator based on desired metrics. In short, Optimizers use information every bit of information in rain set to select the best feature set. \n\nThe main process in Zoish is to split samples to train and validation set, and then optimization will estimate optimal hyper-parameters of the estimators. After that, this best estimator will be input to the feature selection objects and finally, the best subset of features with higher grades will be returned. This subset can be used as the next steps of the ML pipeline. In the next paragraphs, more details about feature selector modules have provided.\n\n### ShapFeatureSelectorFactory\n\nShapFeatureSelectorFactory uses  [SHAP](https://arxiv.org/abs/1705.07874) (SHapley Additive exPlanation)  for a better feature selection. This package uses [FastTreeSHAP](https://arxiv.org/abs/2109.09847) while calculating shap values and [SHAP](https://shap.readthedocs.io/en/latest/index.html) for plotting. Using this module users can : \n\n- find features using the best estimator of tree-based models with the highest shap values after hyper-parameter optimization.\n- draw some shap related plots for selected features.\n- return a  Pandas data frame with a list of features and shap values. \n\n### RecursiveFeatureEliminationFeatureSelectorFactory\n\nThe job of this factory class is to ease the selection of features by following a recursive elimination process. The process uses the best estimator found by the optimizer using all the features. Then it ranks the features according to their importance derived from the best estimator. In the next step, it removes the least important feature and fits again with the best estimator. It calculates the performance of the best estimator again and calculates the performance difference between the new and old results. If the performance drop is below the threshold the feature is removed, and this process will continue until all features have been evaluated. For more information on the logic of the recursive elimination process visit this [RecursiveFeatureElimination](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/RecursiveFeatureElimination.html) page. \n\n### RecursiveFeatureAdditionFeatureSelectorFactory\nIt is very similar to RecursiveFeatureEliminationFeatureSelectorFactory, however, the logic is the opposite. It selects features following a recursive addition process. Visit [RecursiveFeatureAddition](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/RecursiveFeatureAddition.html) for more details. \n\n### SelectByShufflingFeatureSelectorFactory\n\nIn this module, the selection of features is based on determining the drop in machine learning model performance when each feature’s values are randomly shuffled.\n\nIf the variables are important, a random permutation of their values will decrease dramatically the machine learning model performance. Contrarily, the permutation of the values should have little to no effect on the model performance metric we are assessing if the feature is not predictive. To understand how it works completely go to its official page [SelectByShuffling](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/SelectByShuffling.html).\n\n### SingleFeaturePerformanceFeatureSelectorFactory\n\nIt selects features based on the performance of a machine learning model trained to utilize a single feature. In other words, it trains a machine-learning model for every single feature, then determines each model’s performance. If the performance of the model is greater than a user-specified threshold, then the feature is retained, otherwise removed. Go to this [page](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/SelectBySingleFeaturePerformance.html) for more information. \n\n## Installation\n\nZoish package is available on PyPI and can be installed with pip:\n\n```sh\npip install zoish\n```\n\nFor log configuration in development environment use \n\n```sh\nexport env=dev\n\n```\n\nFor log configuration in production environment use \n\n```sh\nexport env=prod\n```\n\n## Examples \n\n### Import required libraries\n```\nfrom zoish.feature_selectors.shap_selectors import ShapFeatureSelector\nimport pandas as pd\nfrom sklearn.model_selection import train_test_split\nimport pandas as pd\nfrom sklearn.pipeline import Pipeline\nfrom sklearn.metrics import r2_score\nfrom feature_engine.imputation import CategoricalImputer, MeanMedianImputer\nfrom category_encoders import OrdinalEncoder\nimport xgboost\nimport optuna\nfrom optuna.samplers import TPESampler\nfrom optuna.pruners import HyperbandPruner\nfrom sklearn.linear_model import LinearRegression\n```\n\n### Computer Hardware Data Set (a classification problem)\n```\nurldata= "https://archive.ics.uci.edu/ml/machine-learning-databases/cpu-performance/machine.data"\n# column names\ncol_names=[\n    "vendor name",\n    "Model Name",\n    "MYCT",\n    "MMIN",\n    "MMAX",\n    "CACH",\n    "CHMIN",\n    "CHMAX",\n    "PRP"\n]\n# read data\ndata = pd.read_csv(urldata,header=None,names=col_names,sep=\',\')\n\n```\n### Train test split\n```\nX = data.loc[:, data.columns != "PRP"]\ny = data.loc[:, data.columns == "PRP"]\n\nX_train, X_test, y_train, y_test =train_test_split(X, y, test_size=0.33, random_state=42)\n```\n### Find feature types for later use\n```\nint_cols =  X_train.select_dtypes(include=[\'int\']).columns.tolist()\nfloat_cols =  X_train.select_dtypes(include=[\'float\']).columns.tolist()\ncat_cols =  X_train.select_dtypes(include=[\'object\']).columns.tolist()\n```\n\n###  Define Feature selector and set its arguments  \n```\nshap_feature_selector_factory = (\n    ShapFeatureSelector.shap_feature_selector_factory.set_model_params(\n        X=X_train,\n        y=y_train,\n        verbose=10,\n        random_state=0,\n        estimator=xgboost.XGBRegressor(),\n        estimator_params={\n            "max_depth": [4, 5],\n        },\n        fit_params = {\n            "callbacks": None,\n        },\n        method="optuna",\n        # if n_features=None only the threshold will be considered as a cut-off of features grades.\n        # if threshold=None only n_features will be considered to select the top n features.\n        # if both of them are set to some values, the threshold has the priority for selecting features.\n        n_features=5,\n        threshold = None,\n        list_of_obligatory_features_that_must_be_in_model=[],\n        list_of_features_to_drop_before_any_selection=[],\n    )\n    .set_shap_params(\n        model_output="raw",\n        feature_perturbation="interventional",\n        algorithm="v2",\n        shap_n_jobs=-1,\n        memory_tolerance=-1,\n        feature_names=None,\n        approximate=False,\n        shortcut=False,\n    )\n    .set_optuna_params(\n            measure_of_accuracy="r2_score(y_true, y_pred)",\n            # optuna params\n            with_stratified=False,\n            test_size=.3,\n            n_jobs=-1,\n            # optuna params\n            # optuna study init params\n            study=optuna.create_study(\n                storage=None,\n                sampler=TPESampler(),\n                pruner=HyperbandPruner(),\n                study_name="example of optuna optimizer",\n                direction="maximize",\n                load_if_exists=False,\n                directions=None,\n            ),\n            # optuna optimization params\n            study_optimize_objective=None,\n            study_optimize_objective_n_trials=20,\n            study_optimize_objective_timeout=600,\n            study_optimize_n_jobs=-1,\n            study_optimize_catch=(),\n            study_optimize_callbacks=None,\n            study_optimize_gc_after_trial=False,\n            study_optimize_show_progress_bar=False,\n            )\n)\n\n```\n### Build sklearn Pipeline  \n```\npipeline =Pipeline([\n            # int missing values imputers\n            (\'intimputer\', MeanMedianImputer(\n                imputation_method=\'median\', variables=int_cols)),\n            # category missing values imputers\n            (\'catimputer\', CategoricalImputer(variables=cat_cols)),\n            #\n            (\'catencoder\', OrdinalEncoder()),\n            # feature selection\n            ("sfsf", shap_feature_selector_factory),\n            # add any regression model from sklearn e.g., LinearRegression\n            (\'regression\', LinearRegression())\n\n\n ])\n```\n### Run Pipeline\n```\npipeline.fit(X_train,y_train)\ny_pred = pipeline.predict(X_test)\n\n```\n### Plots\n```\nShapFeatureSelector.shap_feature_selector_factory.plot_features_all(\n    type_of_plot="summary_plot",\n    path_to_save_plot="../plots/shap_optuna_search_regression_summary_plot"\n)\n```\n\n###  Check performance of the Pipeline\n```\nprint(\'r2 score : \')\nprint(r2_score(y_test,y_pred))\n\n```\n### Get access to feature selector instance\n```\nprint(ShapFeatureSelector.shap_feature_selector_factory.get_feature_selector_instance())\n```\n\n\nMore examples are available in the [examples](https://github.com/drhosseinjavedani/zoish/tree/main/zoish/examples). \n\n## License\nLicensed under the [BSD 2-Clause](https://opensource.org/licenses/BSD-2-Clause) License.',
+    'version': '3.3.0',
+    'description': 'Zoish: Automated feature selectoion tools',
+    'long_description': '\n![GitHub Repo stars](https://img.shields.io/github/stars/TorkamaniLab/zoish?style=social) ![GitHub forks](https://img.shields.io/github/forks/TorkamaniLab/zoish?style=social) ![GitHub language count](https://img.shields.io/github/languages/count/TorkamaniLab/zoish) ![GitHub repo size](https://img.shields.io/github/repo-size/TorkamaniLab/zoish) ![GitHub](https://img.shields.io/github/license/TorkamaniLab/zoish) ![PyPI - Downloads](https://img.shields.io/pypi/dd/zoish) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zoish) \n\n# Zoish\n\nZoish is a package built to ease machine learning development by providing various feature-selecting modules such as:  \n- Select By Single Feature Performance\n- Recursive Feature Elimination\n- Recursive Feature Addition\n- Select By Shuffling\n\nAll of them are compatible with [scikit-learn](https://scikit-learn.org) pipeline. \n\n\n## Introduction\n\nAll of the above-mentioned modules of Zoish have class factories that have various methods and parameters. From an estimator to its tunning parameters and from optimizers to their parameters, the final goal is to automate the feature selection of the ML pipeline in a proper way. Optimizers like [Optuna](https://optuna.org/), [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html) , [RandomizedSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html), [TuneGridSearchCV, and TuneSearchCV](https://github.com/ray-project/tune-sklearn) has critical role in Zoish. They are used to provide the best estimator on a train set that is later used by feature selectors to check what features can improve the accuracy of this best estimator based on desired metrics. In short, Optimizers use information every bit of information in rain set to select the best feature set. \n\nThe main process in Zoish is to split samples to train and validation set, and then optimization will estimate optimal hyper-parameters of the estimators. After that, this best estimator will be input to the feature selection objects and finally, the best subset of features with higher grades will be returned. This subset can be used as the next steps of the ML pipeline. In the next paragraphs, more details about feature selector modules have provided.\n\n### ShapFeatureSelectorFactory\n\nShapFeatureSelectorFactory uses  [SHAP](https://arxiv.org/abs/1705.07874) (SHapley Additive exPlanation)  for a better feature selection. This package uses [FastTreeSHAP](https://arxiv.org/abs/2109.09847) while calculating shap values and [SHAP](https://shap.readthedocs.io/en/latest/index.html) for plotting. Using this module users can : \n\n- find features using the best estimator of tree-based models with the highest shap values after hyper-parameter optimization.\n- draw some shap related plots for selected features.\n- return a  Pandas data frame with a list of features and shap values. \n\n### RecursiveFeatureEliminationFeatureSelectorFactory\n\nThe job of this factory class is to ease the selection of features by following a recursive elimination process. The process uses the best estimator found by the optimizer using all the features. Then it ranks the features according to their importance derived from the best estimator. In the next step, it removes the least important feature and fits again with the best estimator. It calculates the performance of the best estimator again and calculates the performance difference between the new and old results. If the performance drop is below the threshold the feature is removed, and this process will continue until all features have been evaluated. For more information on the logic of the recursive elimination process visit this [RecursiveFeatureElimination](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/RecursiveFeatureElimination.html) page. \n\n### RecursiveFeatureAdditionFeatureSelectorFactory\nIt is very similar to RecursiveFeatureEliminationFeatureSelectorFactory, however, the logic is the opposite. It selects features following a recursive addition process. Visit [RecursiveFeatureAddition](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/RecursiveFeatureAddition.html) for more details. \n\n### SelectByShufflingFeatureSelectorFactory\n\nIn this module, the selection of features is based on determining the drop in machine learning model performance when each feature’s values are randomly shuffled.\n\nIf the variables are important, a random permutation of their values will decrease dramatically the machine learning model performance. Contrarily, the permutation of the values should have little to no effect on the model performance metric we are assessing if the feature is not predictive. To understand how it works completely go to its official page [SelectByShuffling](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/SelectByShuffling.html).\n\n### SingleFeaturePerformanceFeatureSelectorFactory\n\nIt selects features based on the performance of a machine learning model trained to utilize a single feature. In other words, it trains a machine-learning model for every single feature, then determines each model’s performance. If the performance of the model is greater than a user-specified threshold, then the feature is retained, otherwise removed. Go to this [page](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/SelectBySingleFeaturePerformance.html) for more information. \n\n## Installation\n\nZoish package is available on PyPI and can be installed with pip:\n\n```sh\npip install zoish\n```\n\nFor log configuration in development environment use \n\n```sh\nexport env=dev\n\n```\n\nFor log configuration in production environment use \n\n```sh\nexport env=prod\n```\n\n## Examples \n\n### Import required libraries\n```\nfrom zoish.feature_selectors.shap_selectors import ShapFeatureSelector\nimport pandas as pd\nfrom sklearn.model_selection import train_test_split\nimport pandas as pd\nfrom sklearn.pipeline import Pipeline\nfrom sklearn.metrics import r2_score\nfrom feature_engine.imputation import CategoricalImputer, MeanMedianImputer\nfrom category_encoders import OrdinalEncoder\nimport xgboost\nimport optuna\nfrom optuna.samplers import TPESampler\nfrom optuna.pruners import HyperbandPruner\nfrom sklearn.linear_model import LinearRegression\n```\n\n### Computer Hardware Data Set (a classification problem)\n```\nurldata= "https://archive.ics.uci.edu/ml/machine-learning-databases/cpu-performance/machine.data"\n# column names\ncol_names=[\n    "vendor name",\n    "Model Name",\n    "MYCT",\n    "MMIN",\n    "MMAX",\n    "CACH",\n    "CHMIN",\n    "CHMAX",\n    "PRP"\n]\n# read data\ndata = pd.read_csv(urldata,header=None,names=col_names,sep=\',\')\n\n```\n### Train test split\n```\nX = data.loc[:, data.columns != "PRP"]\ny = data.loc[:, data.columns == "PRP"]\n\nX_train, X_test, y_train, y_test =train_test_split(X, y, test_size=0.33, random_state=42)\n```\n### Find feature types for later use\n```\nint_cols =  X_train.select_dtypes(include=[\'int\']).columns.tolist()\nfloat_cols =  X_train.select_dtypes(include=[\'float\']).columns.tolist()\ncat_cols =  X_train.select_dtypes(include=[\'object\']).columns.tolist()\n```\n\n###  Define Feature selector and set its arguments  \n```\nshap_feature_selector_factory = (\n    ShapFeatureSelector.shap_feature_selector_factory.set_model_params(\n        X=X_train,\n        y=y_train,\n        verbose=10,\n        random_state=0,\n        estimator=xgboost.XGBRegressor(),\n        estimator_params={\n            "max_depth": [4, 5],\n        },\n        fit_params = {\n            "callbacks": None,\n        },\n        method="optuna",\n        # if n_features=None only the threshold will be considered as a cut-off of features grades.\n        # if threshold=None only n_features will be considered to select the top n features.\n        # if both of them are set to some values, the threshold has the priority for selecting features.\n        n_features=5,\n        threshold = None,\n        list_of_obligatory_features_that_must_be_in_model=[],\n        list_of_features_to_drop_before_any_selection=[],\n    )\n    .set_shap_params(\n        model_output="raw",\n        feature_perturbation="interventional",\n        algorithm="v2",\n        shap_n_jobs=-1,\n        memory_tolerance=-1,\n        feature_names=None,\n        approximate=False,\n        shortcut=False,\n    )\n    .set_optuna_params(\n            measure_of_accuracy="r2_score(y_true, y_pred)",\n            # optuna params\n            with_stratified=False,\n            test_size=.3,\n            n_jobs=-1,\n            # optuna params\n            # optuna study init params\n            study=optuna.create_study(\n                storage=None,\n                sampler=TPESampler(),\n                pruner=HyperbandPruner(),\n                study_name="example of optuna optimizer",\n                direction="maximize",\n                load_if_exists=False,\n                directions=None,\n            ),\n            # optuna optimization params\n            study_optimize_objective=None,\n            study_optimize_objective_n_trials=20,\n            study_optimize_objective_timeout=600,\n            study_optimize_n_jobs=-1,\n            study_optimize_catch=(),\n            study_optimize_callbacks=None,\n            study_optimize_gc_after_trial=False,\n            study_optimize_show_progress_bar=False,\n            )\n)\n\n```\n### Build sklearn Pipeline  \n```\npipeline =Pipeline([\n            # int missing values imputers\n            (\'intimputer\', MeanMedianImputer(\n                imputation_method=\'median\', variables=int_cols)),\n            # category missing values imputers\n            (\'catimputer\', CategoricalImputer(variables=cat_cols)),\n            #\n            (\'catencoder\', OrdinalEncoder()),\n            # feature selection\n            ("sfsf", shap_feature_selector_factory),\n            # add any regression model from sklearn e.g., LinearRegression\n            (\'regression\', LinearRegression())\n\n\n ])\n```\n### Run Pipeline\n```\npipeline.fit(X_train,y_train)\ny_pred = pipeline.predict(X_test)\n\n```\n### Plots\n```\nShapFeatureSelector.shap_feature_selector_factory.plot_features_all(\n    type_of_plot="summary_plot",\n    path_to_save_plot="../plots/shap_optuna_search_regression_summary_plot"\n)\n```\n\n###  Check performance of the Pipeline\n```\nprint(\'r2 score : \')\nprint(r2_score(y_test,y_pred))\n\n```\n### Get access to feature selector instance\n```\nprint(ShapFeatureSelector.shap_feature_selector_factory.get_feature_selector_instance())\n```\n\n\nMore examples are available in the [examples](https://github.com/drhosseinjavedani/zoish/tree/main/zoish/examples). \n\n## License\nLicensed under the [BSD 2-Clause](https://opensource.org/licenses/BSD-2-Clause) License.',
     'author': 'drhosseinjavedani',
     'author_email': 'h.javedani@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/drhosseinjavedani/zoish',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `zoish-3.1.0/PKG-INFO` & `zoish-3.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zoish
-Version: 3.1.0
-Summary: This project uses shapely values for selecting Top n features compatible with scikit learn pipeline
+Version: 3.3.0
+Summary: Zoish: Automated feature selectoion tools
 Home-page: https://github.com/drhosseinjavedani/zoish
 License: BSD 2-Clause License
 Keywords: Auto ML,Feature Selection,Pipeline,Machine learning,shap
 Author: drhosseinjavedani
 Author-email: h.javedani@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
@@ -33,14 +33,17 @@
 Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Requires-Dist: shap (>=0.41.0,<0.42.0)
 Requires-Dist: xgboost (>=1.6.1,<2.0.0)
 Requires-Dist: xgbse (>=0.2.3,<0.3.0)
 Description-Content-Type: text/markdown
 
+
+![GitHub Repo stars](https://img.shields.io/github/stars/TorkamaniLab/zoish?style=social) ![GitHub forks](https://img.shields.io/github/forks/TorkamaniLab/zoish?style=social) ![GitHub language count](https://img.shields.io/github/languages/count/TorkamaniLab/zoish) ![GitHub repo size](https://img.shields.io/github/repo-size/TorkamaniLab/zoish) ![GitHub](https://img.shields.io/github/license/TorkamaniLab/zoish) ![PyPI - Downloads](https://img.shields.io/pypi/dd/zoish) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zoish) 
+
 # Zoish
 
 Zoish is a package built to ease machine learning development by providing various feature-selecting modules such as:  
 - Select By Single Feature Performance
 - Recursive Feature Elimination
 - Recursive Feature Addition
 - Select By Shuffling
```

