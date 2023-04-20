# Comparing `tmp/lohrasb-3.1.0.tar.gz` & `tmp/lohrasb-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lohrasb-3.1.0.tar", max compression
+gzip compressed data, was "lohrasb-3.2.0.tar", max compression
```

## Comparing `lohrasb-3.1.0.tar` & `lohrasb-3.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1323 2023-02-22 07:56:13.975949 lohrasb-3.1.0/LICENSE
--rw-r--r--   0        0        0    19279 2023-02-22 07:56:13.976799 lohrasb-3.1.0/README.md
--rw-r--r--   0        0        0       67 2023-02-22 07:56:13.978874 lohrasb-3.1.0/lohrasb/.env
--rw-r--r--   0        0        0     1029 2023-02-22 08:07:14.175868 lohrasb-3.1.0/lohrasb/__init__.py
--rw-r--r--   0        0        0      326 2023-02-22 07:56:13.979400 lohrasb-3.1.0/lohrasb/abstracts/estimators.py
--rw-r--r--   0        0        0      784 2023-02-22 07:56:13.979618 lohrasb-3.1.0/lohrasb/abstracts/optimizers.py
--rw-r--r--   0        0        0    70959 2023-02-22 07:56:13.980597 lohrasb-3.1.0/lohrasb/base_classes/optimizer_bases.py
--rw-r--r--   0        0        0   108910 2023-02-22 07:56:13.981561 lohrasb-3.1.0/lohrasb/best_estimator.py
--rw-r--r--   0        0        0      695 2023-02-22 07:56:13.981989 lohrasb-3.1.0/lohrasb/config.yaml
--rw-r--r--   0        0        0      405 2023-02-22 07:56:13.982658 lohrasb-3.1.0/lohrasb/decorators/decorators.py
--rw-r--r--   0        0        0        0 2023-02-22 07:56:13.982902 lohrasb-3.1.0/lohrasb/examples/__init__.py
--rw-r--r--   0        0        0    41882 2023-02-22 07:56:13.985101 lohrasb-3.1.0/lohrasb/examples/classification_gridsearch.ipynb
--rw-r--r--   0        0        0  4717043 2023-02-22 07:56:14.019938 lohrasb-3.1.0/lohrasb/examples/classification_gridsearch_interpretml_shapkernel.ipynb
--rw-r--r--   0        0        0    72699 2023-02-22 07:56:14.021850 lohrasb-3.1.0/lohrasb/examples/classification_optuna.ipynb
--rw-r--r--   0        0        0    54881 2023-02-22 07:56:14.022409 lohrasb-3.1.0/lohrasb/examples/classification_optuna_interpretml.ipynb
--rw-r--r--   0        0        0    33201 2023-02-22 07:56:14.022830 lohrasb-3.1.0/lohrasb/examples/classification_randomsearch.ipynb
--rw-r--r--   0        0        0    16972 2023-02-22 07:56:14.023326 lohrasb-3.1.0/lohrasb/examples/classification_randomsearch_multi_class.ipynb
--rw-r--r--   0        0        0    72830 2023-02-22 07:56:14.024060 lohrasb-3.1.0/lohrasb/examples/classification_ray_tunegridsearch.ipynb
--rw-r--r--   0        0        0    80165 2023-02-22 07:56:14.024494 lohrasb-3.1.0/lohrasb/examples/classification_ray_tunesearch.ipynb
--rw-r--r--   0        0        0     5517 2023-02-22 07:56:14.025082 lohrasb-3.1.0/lohrasb/examples/lohrasb.log
--rw-r--r--   0        0        0    30816 2023-02-22 07:56:14.025536 lohrasb-3.1.0/lohrasb/examples/regression_optuna.ipynb
--rw-r--r--   0        0        0   561335 2023-02-22 07:56:14.027113 lohrasb-3.1.0/lohrasb/examples/regression_optuna_interpretml.ipynb
--rw-r--r--   0        0        0    16470 2023-02-22 07:56:14.027637 lohrasb-3.1.0/lohrasb/examples/xgboost_survival_embeddings.ipynb
--rw-r--r--   0        0        0      414 2023-02-22 07:56:14.028039 lohrasb-3.1.0/lohrasb/factories/factories.py
--rw-r--r--   0        0        0        0 2023-02-22 07:56:14.028244 lohrasb-3.1.0/lohrasb/mediators/mediators.py
--rw-r--r--   0        0        0       96 2023-02-22 07:56:14.028439 lohrasb-3.1.0/lohrasb/model_conf.py
--rw-r--r--   0        0        0       95 2023-02-22 07:56:14.028615 lohrasb-3.1.0/lohrasb/project_conf.py
--rw-r--r--   0        0        0        0 2023-02-22 07:56:14.028790 lohrasb-3.1.0/lohrasb/utils/__init__.py
--rw-r--r--   0        0        0     4652 2023-02-22 07:56:14.029034 lohrasb-3.1.0/lohrasb/utils/helper_funcs.py
--rw-r--r--   0        0        0    18032 2023-02-22 07:56:14.029378 lohrasb-3.1.0/lohrasb/utils/metrics.py
--rw-r--r--   0        0        0       40 2023-02-22 08:07:14.176868 lohrasb-3.1.0/lohrasb/version.py
--rw-r--r--   0        0        0     1300 2023-02-22 08:07:14.175868 lohrasb-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    21579 1970-01-01 00:00:00.000000 lohrasb-3.1.0/setup.py
--rw-r--r--   0        0        0    20852 1970-01-01 00:00:00.000000 lohrasb-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1323 2023-02-22 07:56:13.975949 lohrasb-3.2.0/LICENSE
+-rw-r--r--   0        0        0    19279 2023-02-22 07:56:13.976799 lohrasb-3.2.0/README.md
+-rw-r--r--   0        0        0       67 2023-02-22 07:56:13.978874 lohrasb-3.2.0/lohrasb/.env
+-rw-r--r--   0        0        0     1029 2023-04-20 16:33:26.933242 lohrasb-3.2.0/lohrasb/__init__.py
+-rw-r--r--   0        0        0      326 2023-02-22 07:56:13.979400 lohrasb-3.2.0/lohrasb/abstracts/estimators.py
+-rw-r--r--   0        0        0      784 2023-02-22 07:56:13.979618 lohrasb-3.2.0/lohrasb/abstracts/optimizers.py
+-rw-r--r--   0        0        0    70959 2023-02-22 07:56:13.980597 lohrasb-3.2.0/lohrasb/base_classes/optimizer_bases.py
+-rw-r--r--   0        0        0   108910 2023-02-22 07:56:13.981561 lohrasb-3.2.0/lohrasb/best_estimator.py
+-rw-r--r--   0        0        0      695 2023-02-22 07:56:13.981989 lohrasb-3.2.0/lohrasb/config.yaml
+-rw-r--r--   0        0        0      405 2023-02-22 07:56:13.982658 lohrasb-3.2.0/lohrasb/decorators/decorators.py
+-rw-r--r--   0        0        0        0 2023-02-22 07:56:13.982902 lohrasb-3.2.0/lohrasb/examples/__init__.py
+-rw-r--r--   0        0        0    41882 2023-02-22 07:56:13.985101 lohrasb-3.2.0/lohrasb/examples/classification_gridsearch.ipynb
+-rw-r--r--   0        0        0  4717043 2023-02-22 07:56:14.019938 lohrasb-3.2.0/lohrasb/examples/classification_gridsearch_interpretml_shapkernel.ipynb
+-rw-r--r--   0        0        0    72699 2023-02-22 07:56:14.021850 lohrasb-3.2.0/lohrasb/examples/classification_optuna.ipynb
+-rw-r--r--   0        0        0    54881 2023-02-22 07:56:14.022409 lohrasb-3.2.0/lohrasb/examples/classification_optuna_interpretml.ipynb
+-rw-r--r--   0        0        0    33201 2023-02-22 07:56:14.022830 lohrasb-3.2.0/lohrasb/examples/classification_randomsearch.ipynb
+-rw-r--r--   0        0        0    16972 2023-02-22 07:56:14.023326 lohrasb-3.2.0/lohrasb/examples/classification_randomsearch_multi_class.ipynb
+-rw-r--r--   0        0        0    72830 2023-02-22 07:56:14.024060 lohrasb-3.2.0/lohrasb/examples/classification_ray_tunegridsearch.ipynb
+-rw-r--r--   0        0        0    80165 2023-02-22 07:56:14.024494 lohrasb-3.2.0/lohrasb/examples/classification_ray_tunesearch.ipynb
+-rw-r--r--   0        0        0     5517 2023-02-22 07:56:14.025082 lohrasb-3.2.0/lohrasb/examples/lohrasb.log
+-rw-r--r--   0        0        0    30816 2023-02-22 07:56:14.025536 lohrasb-3.2.0/lohrasb/examples/regression_optuna.ipynb
+-rw-r--r--   0        0        0   561335 2023-02-22 07:56:14.027113 lohrasb-3.2.0/lohrasb/examples/regression_optuna_interpretml.ipynb
+-rw-r--r--   0        0        0    16470 2023-02-22 07:56:14.027637 lohrasb-3.2.0/lohrasb/examples/xgboost_survival_embeddings.ipynb
+-rw-r--r--   0        0        0      414 2023-02-22 07:56:14.028039 lohrasb-3.2.0/lohrasb/factories/factories.py
+-rw-r--r--   0        0        0        0 2023-02-22 07:56:14.028244 lohrasb-3.2.0/lohrasb/mediators/mediators.py
+-rw-r--r--   0        0        0       96 2023-02-22 07:56:14.028439 lohrasb-3.2.0/lohrasb/model_conf.py
+-rw-r--r--   0        0        0       95 2023-02-22 07:56:14.028615 lohrasb-3.2.0/lohrasb/project_conf.py
+-rw-r--r--   0        0        0        0 2023-02-22 07:56:14.028790 lohrasb-3.2.0/lohrasb/utils/__init__.py
+-rw-r--r--   0        0        0     4652 2023-02-22 07:56:14.029034 lohrasb-3.2.0/lohrasb/utils/helper_funcs.py
+-rw-r--r--   0        0        0    18032 2023-02-22 07:56:14.029378 lohrasb-3.2.0/lohrasb/utils/metrics.py
+-rw-r--r--   0        0        0       40 2023-04-20 16:33:26.933242 lohrasb-3.2.0/lohrasb/version.py
+-rw-r--r--   0        0        0     1276 2023-04-20 16:33:26.932242 lohrasb-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0    21555 1970-01-01 00:00:00.000000 lohrasb-3.2.0/setup.py
+-rw-r--r--   0        0        0    20828 1970-01-01 00:00:00.000000 lohrasb-3.2.0/PKG-INFO
```

### Comparing `lohrasb-3.1.0/LICENSE` & `lohrasb-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/README.md` & `lohrasb-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/__init__.py` & `lohrasb-3.2.0/lohrasb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.1.0"
+__version__ = "3.2.0"
 
 import logging
 import logging.config
 import os
 from pathlib import Path, PurePath
 
 import yaml
```

### Comparing `lohrasb-3.1.0/lohrasb/abstracts/optimizers.py` & `lohrasb-3.2.0/lohrasb/abstracts/optimizers.py`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/base_classes/optimizer_bases.py` & `lohrasb-3.2.0/lohrasb/base_classes/optimizer_bases.py`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/best_estimator.py` & `lohrasb-3.2.0/lohrasb/best_estimator.py`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/config.yaml` & `lohrasb-3.2.0/lohrasb/config.yaml`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/examples/classification_gridsearch.ipynb` & `lohrasb-3.2.0/lohrasb/examples/classification_gridsearch.ipynb`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/examples/classification_gridsearch_interpretml_shapkernel.ipynb` & `lohrasb-3.2.0/lohrasb/examples/classification_gridsearch_interpretml_shapkernel.ipynb`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/examples/classification_optuna.ipynb` & `lohrasb-3.2.0/lohrasb/examples/classification_optuna.ipynb`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/examples/classification_optuna_interpretml.ipynb` & `lohrasb-3.2.0/lohrasb/examples/classification_optuna_interpretml.ipynb`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/examples/classification_randomsearch.ipynb` & `lohrasb-3.2.0/lohrasb/examples/classification_randomsearch.ipynb`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/examples/classification_randomsearch_multi_class.ipynb` & `lohrasb-3.2.0/lohrasb/examples/classification_randomsearch_multi_class.ipynb`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/examples/classification_ray_tunegridsearch.ipynb` & `lohrasb-3.2.0/lohrasb/examples/classification_ray_tunegridsearch.ipynb`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/examples/classification_ray_tunesearch.ipynb` & `lohrasb-3.2.0/lohrasb/examples/classification_ray_tunesearch.ipynb`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/examples/lohrasb.log` & `lohrasb-3.2.0/lohrasb/examples/lohrasb.log`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/examples/regression_optuna.ipynb` & `lohrasb-3.2.0/lohrasb/examples/regression_optuna.ipynb`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/examples/regression_optuna_interpretml.ipynb` & `lohrasb-3.2.0/lohrasb/examples/regression_optuna_interpretml.ipynb`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/examples/xgboost_survival_embeddings.ipynb` & `lohrasb-3.2.0/lohrasb/examples/xgboost_survival_embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/utils/helper_funcs.py` & `lohrasb-3.2.0/lohrasb/utils/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/lohrasb/utils/metrics.py` & `lohrasb-3.2.0/lohrasb/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `lohrasb-3.1.0/pyproject.toml` & `lohrasb-3.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # project configuration, use poetry
 [tool.poetry]
 name = "lohrasb"
-version = "3.1.0"
-description = "Using optuna search optimizer to estimate best tree based estimator compatible with scikit-learn"
+version = "3.2.0"
+description = "A scalable estimator optimization tool compatible with scikit-learn APIs"
 authors = ["drhosseinjavedani <h.javedani@gmail.com>"]
 homepage = "https://github.com/drhosseinjavedani/lohrasb"
 license = "BSD-3-Clause license"
 
 readme = "README.md"
 keywords = [
     "Auto ML",
```

### Comparing `lohrasb-3.1.0/setup.py` & `lohrasb-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
  'scipy>=1.5,<2.0',
  'tune-sklearn>=0.4.5,<0.5.0',
  'xgboost>=1.6.1,<2.0.0',
  'xgbse>=0.2.3,<0.3.0']
 
 setup_kwargs = {
     'name': 'lohrasb',
-    'version': '3.1.0',
-    'description': 'Using optuna search optimizer to estimate best tree based estimator compatible with scikit-learn',
+    'version': '3.2.0',
+    'description': 'A scalable estimator optimization tool compatible with scikit-learn APIs',
     'long_description': '![GitHub Repo stars](https://img.shields.io/github/stars/drhosseinjavedani/lohrasb) ![GitHub forks](https://img.shields.io/github/forks/drhosseinjavedani/lohrasb) ![GitHub language count](https://img.shields.io/github/languages/count/drhosseinjavedani/lohrasb) ![GitHub repo size](https://img.shields.io/github/repo-size/drhosseinjavedani/lohrasb) ![GitHub](https://img.shields.io/github/license/drhosseinjavedani/lohrasb)![PyPI - Downloads](https://img.shields.io/pypi/dd/lohrasb) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lohrasb) \n\n# Lohrasb\n\nLohrasb is a  tool built to ease machine learning development by tuning hyper-parameters of estimators in a scalable way. It uses [Optuna](https://optuna.readthedocs.io/en/stable/index.html), [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html), [RandomizedSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html), and [Ray tune Scikit-Learn API](https://docs.ray.io/en/latest/tune/api_docs/sklearn.html) to tune most of the estimators of sickit-learn. It is compatible with [scikit-learn](https://scikit-learn.org) pipeline, [XGBoost Survival Embeddings](https://github.com/loft-br/xgboost-survival-embeddings) and, [InterpretML](https://github.com/interpretml/interpret/).\n\n\n### Introduction\n\nBaseModel of the Lohrasb package can receive various parameters. From an estimator class to its tunning parameters and GridsearchCV, RandomizedSearchCV, or Optuna to their parameters. Samples will be split to train and validation set, and then optimization will estimate optimal related parameters using these optimizing engines.\n\n### Installation\n\nLohrasb package is available on PyPI and can be installed with pip:\n\n```sh\npip install lohrasb\n```\n\n\n### Supported estimators for this package\nLohrasb supports almost all machine learning estimators for classification and regression.\n\n### Usage\n\n- Tunning best parameters of a machine learning model using [Optuna](https://optuna.readthedocs.io/en/stable/index.html) , [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html) [RandomizedSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html), [TuneGridSearchCV, and TuneSearchCV](https://docs.ray.io/en/latest/tune/api_docs/sklearn.html) from [Ray](https://docs.ray.io/en/latest/index.html) tune Scikit-Learn API (tune.sklearn).\n\n### Factories\nFor ease of use of BestModel, some factories are available to build associated instances corresponding to each optimization engine. For example, the following factory can be used for  GridSearchCV:\n\n```\n\nobj = BaseModel().optimize_by_gridsearchcv(\n            estimator=XGBClassifier(),\n            estimator_params={\n                                "booster": ["gbtree","dart"],\n                                "eval_metric": ["auc"],\n                                "max_depth": [4, 5],\n                                "gamma": [0.1, 1.2],\n                                "subsample": [0.8],\n                            },\n            fit_params = None,\n            measure_of_accuracy=make_scorer(f1_score, greater_is_better=True),\n            # instead of measure_of_accuracy it is possible to use :  scoring="f1",\n            verbose=3,\n            n_jobs=-1,\n            random_state=42,\n            cv=KFold(2),\n        )\n```\n\n#### Example 1: Computer Hardware (Part 1: Use BestModel in sklearn pipeline)\n\n##### Import some required libraries\n```\nfrom lohrasb.best_estimator import BaseModel\nimport xgboost\nfrom optuna.pruners import HyperbandPruner\nfrom optuna.samplers._tpe.sampler import TPESampler\nfrom sklearn.model_selection import KFold,train_test_split\nimport pandas as pd\nimport numpy as np\nimport optuna\nfrom sklearn.pipeline import Pipeline\nfrom feature_engine.imputation import (\n    CategoricalImputer,\n    MeanMedianImputer\n    )\nfrom category_encoders import OrdinalEncoder\nfrom sklearn.metrics import (\n    make_scorer)\nfrom sklearn.metrics import r2_score\nfrom sklearn.linear_model import *\n\n\n```\n##### Computer Hardware [Data Set](https://archive.ics.uci.edu/ml/datasets/Computer+Hardware)\n (a regression problem)\n  \n\n```\nurldata= "https://archive.ics.uci.edu/ml/machine-learning-databases/cpu-performance/machine.data"\n# column names\ncol_names=[\n    "vendor name",\n    "Model Name",\n    "MYCT",\n    "MMIN",\n    "MMAX",\n    "CACH",\n    "CHMIN",\n    "CHMAX",\n    "PRP"\n]\n# read data\ndata = pd.read_csv(urldata,header=None,names=col_names,sep=\',\')\ndata\n```\n##### Train test split\n\n```\nX = data.loc[:, data.columns != "PRP"]\ny = data.loc[:, data.columns == "PRP"]\ny = y.values.ravel()\n\n\nX_train, X_test, y_train, y_test =train_test_split(X, y, test_size=0.33, random_state=42)\n\n```\n##### Find feature types for later use\n\n```\nint_cols =  X_train.select_dtypes(include=[\'int\']).columns.tolist()\nfloat_cols =  X_train.select_dtypes(include=[\'float\']).columns.tolist()\ncat_cols =  X_train.select_dtypes(include=[\'object\']).columns.tolist()\n```\n\n#####  Define estimator and set its arguments  \n```\nestimator = LinearRegression()\nestimator_params= {\n        "fit_intercept": [True, False],\n    }\n```\n##### Use factory\n\n```\nobj = BaseModel().optimize_by_optuna(\n            estimator=estimator,\n            estimator_params=estimator_params,\n            measure_of_accuracy="mean_absolute_error(y_true, y_pred, multioutput=\'uniform_average\')",\n            with_stratified=False,\n            test_size=.3,\n            verbose=3,\n            n_jobs=-1,\n            random_state=42,\n            # optuna params\n            # optuna study init params\n            study=optuna.create_study(\n                storage=None,\n                sampler=TPESampler(),\n                pruner=HyperbandPruner(),\n                study_name=None,\n                direction="minimize",\n                load_if_exists=False,\n                directions=None,\n            ),\n            # optuna optimization params\n            study_optimize_objective=None,\n            study_optimize_objective_n_trials=10,\n            study_optimize_objective_timeout=600,\n            study_optimize_n_jobs=-1,\n            study_optimize_catch=(),\n            study_optimize_callbacks=None,\n            study_optimize_gc_after_trial=False,\n            study_optimize_show_progress_bar=False,\n        )\n```\n#####  Build sklearn pipeline\n```\npipeline =Pipeline([\n            # int missing values imputers\n            (\'intimputer\', MeanMedianImputer(\n                imputation_method=\'median\', variables=int_cols)),\n            # category missing values imputers\n            (\'catimputer\', CategoricalImputer(variables=cat_cols)),\n            #\n            (\'catencoder\', OrdinalEncoder()),\n            # regression model \n            (\'obj\', obj),\n\n\n ])\n\n\n\n```\n##### Run Pipeline\n\n```\npipeline.fit(X_train,y_train)\ny_pred = pipeline.predict(X_test)\n```\n##### Check performance of the pipeline\n\n```\nprint(\'r2 score : \')\nprint(r2_score(y_test,y_pred))\n```\n\n##### Part 2: Use BestModel as a standalone estimator \n```\nX_train, X_test, y_train, y_test =train_test_split(X, y, test_size=0.33, random_state=42)\n```\n\n##### Transform features to make them ready for model input\n```\ntransform_pipeline =Pipeline([\n            # int missing values imputers\n            (\'intimputer\', MeanMedianImputer(\n                imputation_method=\'median\', variables=int_cols)),\n            # category missing values imputers\n            (\'catimputer\', CategoricalImputer(variables=cat_cols)),\n            #\n            (\'catencoder\', OrdinalEncoder()),\n            # classification model\n\n ])\n```\n##### Transform X_train and X_test\n\n```\nX_train=transform_pipeline.fit_transform(X_train,y_train)\nX_test=transform_pipeline.transform(X_test)\n```\n\n##### Train model and predict\n```\nobj.fit(X_train,y_train)\ny_pred = obj.predict(X_test)\n```\n\n##### Check performance of the model\n\n```\nprint(\'r2 score : \')\nprint(r2_score(y_test,y_pred))\nprint(\'mean_absolute_error : \')\nprint(mean_absolute_error(y_test,y_pred))\n\n\nprint(obj.get_best_estimator())\n\nprint(obj.best_estimator)\n\nOptunaObj = obj.get_optimized_object()\nprint(OptunaObj.trials)\n```\n\n#### Example 2: XGBoost Survival Embeddings (XGBSEKaplanNeighbors)\nFor more information refer to visit [XGBoost Survival Embeddings](https://loft-br.github.io/xgboost-survival-embeddings/examples/confidence_interval.html) page.\n\n\n##### Import some required libraries\n```\n! pip3 install torch==1.12.1\nimport sys\nsys.path.append(\'/usr/local/lib/python3.10/site-packages\')\nimport torch\nimport numpy as np\nfrom sklearn.model_selection import KFold, train_test_split\nfrom lohrasb.best_estimator import BaseModel\nfrom sklearn.pipeline import Pipeline\nfrom sklearn.metrics import make_scorer\nfrom xgbse.converters import convert_to_structured\nfrom xgbse.metrics import (\n    concordance_index,\n    approx_brier_score\n)\nfrom xgbse import (\n    XGBSEKaplanNeighbors,\n    XGBSEKaplanTree,\n    XGBSEBootstrapEstimator\n)\nfrom pycox.datasets import metabric\n\n```\n\n\n##### Read data metabric\n\n```\ndf = metabric.read_df()\ndf.head()\n```\n\n##### Define labels and train-test split \n\n```\n# splitting to X, T, E format\nX = df.drop([\'duration\', \'event\'], axis=1)\ny = convert_to_structured(df[\'duration\'], df[\'event\'])\n\n\n# splitting between train, and validation \n(X_train, X_test,\n y_train, y_test) = \\\ntrain_test_split(X, y, test_size=0.2, random_state=42)\n```\n\n\n##### Define estimator and set its arguments\n```\nestimator_params = {\n    \'n_estimators\' :[100,200]\n\n}\n\nPARAMS_TREE = {\n    \'objective\': \'survival:cox\',\n    \'eval_metric\': \'cox-nloglik\',\n    \'tree_method\': \'hist\', \n    \'max_depth\': 100, \n    \'booster\':\'dart\', \n    \'subsample\': 1.0,\n    \'min_child_weight\': 50, \n    \'colsample_bynode\': 1.0\n}\nbase_model = XGBSEKaplanTree(PARAMS_TREE)\n\nTIME_BINS = np.arange(15, 315, 15)\n```\n\n##### Define estimator and fit params\n\n```\nestimator=XGBSEBootstrapEstimator(base_model)\nfit_params = {"time_bins":TIME_BINS}\n```\n##### Define BaseModel estimator using random search CV\n\n```\nobj = BaseModel().optimize_by_randomsearchcv(\n            estimator=estimator,\n            fit_params = fit_params,\n            estimator_params=estimator_params,\n            measure_of_accuracy=make_scorer(approx_brier_score, greater_is_better=False),\n            verbose=3,\n            n_jobs=-1,\n            n_iter=2,\n            random_state=42,\n            cv=KFold(2),\n        )\n```\n\n##### Build sklearn pipeline\n\n```\npipeline =Pipeline([\n            (\'obj\', obj)\n\n ])\n```\n##### Run Pipeline\n```\npipeline.fit(X_train,y_train)\ny_pred = pipeline.predict(X_test)\n```\n\n##### Check performance of the pipeline\n\n```\nprint(f\'C-index: {concordance_index(y_test, y_pred)}\')\nprint(f\'Avg. Brier Score: {approx_brier_score(y_test, y_pred)}\')\n```\n\n#### Example 3: Using InterpretML\n\n[InterpretML](https://interpret.ml/docs/getting-started) is a package that supports training interpretable models (glassbox), as well as explaining existing ML pipelines (blackbox). In this example we will use [Shapley Additive Explanations](https://interpret.ml/docs/shap.html) of this package on [Adult Data Set](https://archive.ics.uci.edu/ml/datasets/adult) (a classification problem).\n\n##### Import some required libraries\n\n```\nimport pandas as pd\nfrom sklearn.model_selection import KFold, train_test_split\nfrom lohrasb.best_estimator import BaseModel\nfrom sklearn.pipeline import Pipeline\nfrom feature_engine.imputation import (\n    CategoricalImputer,\n    MeanMedianImputer\n    )\nfrom category_encoders import OrdinalEncoder\nfrom sklearn.metrics import (\n    classification_report,\n    confusion_matrix,\n    f1_score)\nfrom sklearn.metrics import f1_score, make_scorer\nfrom sklearn.ensemble import RandomForestClassifier\nfrom interpret import show\nfrom interpret.blackbox import ShapKernel\nimport shap\nfrom interpret import set_visualize_provider\nfrom interpret.provider import InlineProvider\nset_visualize_provider(InlineProvider())```\n```\n\n##### Read data\n```\nurldata= "https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data"\n# column names\ncol_names=["age", "workclass", "fnlwgt" , "education" ,"education-num",\n"marital-status","occupation","relationship","race","sex","capital-gain","capital-loss","hours-per-week",\n"native-country","label"\n]\n# read data\ndata = pd.read_csv(urldata,header=None,names=col_names,sep=\',\')\ndata.head()\n```\n\n##### Define labels\n```\ndata.loc[data[\'label\']==\'<=50K\',\'label\']=0\ndata.loc[data[\'label\']==\' <=50K\',\'label\']=0\n\ndata.loc[data[\'label\']==\'>50K\',\'label\']=1\ndata.loc[data[\'label\']==\' >50K\',\'label\']=1\n\ndata[\'label\']=data[\'label\'].astype(int)\n```\n\n##### Train test split\n```\n\nX = data.loc[:, data.columns != "label"]\ny = data.loc[:, data.columns == "label"]\n\nX_train, X_test, y_train, y_test =train_test_split(X, y, \\\n     test_size=0.33, stratify=y[\'label\'], random_state=42)\n\ny_train=y_train.values.ravel()\ny_test=y_test.values.ravel()\n```\n\n\n##### Find feature types for later use\n```\n\nint_cols =  X_train.select_dtypes(include=[\'int\']).columns.tolist()\nfloat_cols =  X_train.select_dtypes(include=[\'float\']).columns.tolist()\ncat_cols =  X_train.select_dtypes(include=[\'object\']).columns.tolist()\n```\n\n\n##### Define estimator and set its arguments \n```\n\nestimator = RandomForestClassifier()\nestimator_params = {\n        "max_depth": [4, 5],\n        "n_estimators":[100,200],\n        "max_features" :["sqrt", "log2"],\n\n\n    }\n    \n\nblackbox_model = BaseModel().optimize_by_gridsearchcv(\n            estimator=estimator,\n            estimator_params=estimator_params,\n            fit_params = None,\n            measure_of_accuracy=make_scorer(f1_score, greater_is_better=True),\n            verbose=3,\n            n_jobs=-1,\n            random_state=42,\n            cv=KFold(2),\n        )\n```\n\n##### Build sklearn pipeline\n\n\n```\n\npipeline =Pipeline([\n            # int missing values imputers\n            (\'intimputer\', MeanMedianImputer(\n                imputation_method=\'median\', variables=int_cols)),\n            # category missing values imputers\n            (\'catimputer\', CategoricalImputer(variables=cat_cols)),\n            #\n            (\'catencoder\', OrdinalEncoder()),\n            # classification model\n            #(\'obj\', RandomForestClassifier())\n\n ])\n```\n\n\n##### Run Pipeline\n```\n\nX_train = pipeline.fit_transform(X_train,y_train)\nX_test = pipeline.transform(X_test)\n\nblackbox_model.fit(X_train, y_train)\ny_pred = blackbox_model.predict(X_test)\n```\n\n\n##### Check performance of the pipeline\n```\n\nprint(\'F1 score : \')\nprint(f1_score(y_test,y_pred))\nprint(\'Classification report : \')\nprint(classification_report(y_test,y_pred))\nprint(\'Confusion matrix : \')\nprint(confusion_matrix(y_test,y_pred))\n```\n\n\n#####  Interpret of the pipeline and its decisions with SHAP. The visualizations provided will be for local explanations.\n\n(train set is big only we use 500 as a sample)\n```\n\nshap_kernel = ShapKernel(predict_fn=blackbox_model.predict_proba, data=shap.sample(X_train,500))\nshap_local = shap_kernel.explain_local(X_test[:20], y_test[:20])\nshow(shap_local)\n\n```\n\n#### Example 4: Explaining [Ray](https://docs.ray.io/en/latest/index.html) [Scikit-Learn API (tune.sklearn)](https://docs.ray.io/en/latest/tune/api_docs/sklearn.html)\n\n##### imports\n```\nimport pandas as pd\nfrom sklearn.model_selection import KFold, train_test_split\nfrom lohrasb.best_estimator import BaseModel\nfrom sklearn.pipeline import Pipeline\nfrom feature_engine.imputation import (\n    CategoricalImputer,\n    MeanMedianImputer\n    )\nfrom category_encoders import OrdinalEncoder\nfrom sklearn.metrics import (\n    classification_report,\n    confusion_matrix,\n    f1_score)\nfrom sklearn.metrics import f1_score, make_scorer\nfrom xgboost import *\nfrom lohrasb import logger\n\nlogger.info("Using Scikit-Learn API (tune-sklearn) for an example of classification")\n```\n##### Example: Use [Adult Data Set](https://archive.ics.uci.edu/ml/datasets/Adult) (a classification problem)\n\n```\nurldata= "https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data"\n# column names\ncol_names=["age", "workclass", "fnlwgt" , "education" ,"education-num",\n"marital-status","occupation","relationship","race","sex","capital-gain","capital-loss","hours-per-week",\n"native-country","label"\n]\n# read data\ndata = pd.read_csv(urldata,header=None,names=col_names,sep=\',\')\ndata.head()\n```\n##### Define labels\n```\ndata.loc[data[\'label\']==\'<=50K\',\'label\']=0\ndata.loc[data[\'label\']==\' <=50K\',\'label\']=0\n\ndata.loc[data[\'label\']==\'>50K\',\'label\']=1\ndata.loc[data[\'label\']==\' >50K\',\'label\']=1\n\ndata[\'label\']=data[\'label\'].astype(int)\n```\n##### Train test split\n```\nX = data.loc[:, data.columns != "label"]\ny = data.loc[:, data.columns == "label"]\n\n\nX_train, X_test, y_train, y_test =train_test_split(X, y, \\\ntest_size=0.33, stratify=y[\'label\'], random_state=42)\n```\n##### Find feature types for later use\n```\nint_cols =  X_train.select_dtypes(include=[\'int\']).columns.tolist()\nfloat_cols =  X_train.select_dtypes(include=[\'float\']).columns.tolist()\ncat_cols =  X_train.select_dtypes(include=[\'object\']).columns.tolist()\n```\n##### Define estimator and set its arguments \n```\nestimator = XGBClassifier()\nestimator_params = {\n        "booster": ["gbtree","dart"],\n        "eval_metric": ["auc"],\n        "max_depth": [4, 5],\n        "gamma": [0.1, 1.2],\n        "subsample": [0.8],\n\n    }\n\n\nobj = BaseModel().optimize_by_tunesearchcv(\n            estimator=estimator,\n            estimator_params=estimator_params,\n            fit_params = None,\n            measure_of_accuracy=make_scorer(f1_score, greater_is_better=True),\n            verbose=3,\n            random_state=44,\n            n_jobs=None,\n            cv=KFold(3),\n            early_stopping=None, \n            n_trials=10,\n            scoring=None, \n            refit=True, \n            error_score=\'raise\', \n            return_train_score=False, \n            local_dir=\'~/ray_results\', \n            name=None, \n            max_iters=1, \n            search_optimization=\'hyperopt\',\n            use_gpu=False, \n            loggers=None, \n            pipeline_auto_early_stop=True, \n            stopper=None, \n            time_budget_s=None, \n            mode=None,\n            search_kwargs=None, \n\n        )\n```\n##### Build sklearn pipeline\n\n\n```\npipeline =Pipeline([\n            # int missing values imputers\n            (\'intimputer\', MeanMedianImputer(\n                imputation_method=\'median\', variables=int_cols)),\n            # category missing values imputers\n            (\'catimputer\', CategoricalImputer(variables=cat_cols)),\n            #\n            (\'catencoder\', OrdinalEncoder()),\n            # classification model\n            (\'obj\', obj)\n\n ])\n```\n##### Run Pipeline\n```\npipeline.fit(X_train,y_train)\ny_pred = pipeline.predict(X_test)\n```\n##### Check performance of the pipeline\n```\nprint(\'F1 score : \')\nprint(f1_score(y_test,y_pred))\nprint(\'Classification report : \')\nprint(classification_report(y_test,y_pred))\nprint(\'Confusion matrix : \')\nprint(confusion_matrix(y_test,y_pred))\n```\n\n\nThere are some more examples  available in the [examples](https://github.com/drhosseinjavedani/lohrasb/tree/main/lohrasb/examples) webpage. \n\n#### License\nLicensed under the [BSD 2-Clause](https://opensource.org/licenses/BSD-2-Clause) License.',
     'author': 'drhosseinjavedani',
     'author_email': 'h.javedani@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/drhosseinjavedani/lohrasb',
     'packages': packages,
```

### Comparing `lohrasb-3.1.0/PKG-INFO` & `lohrasb-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lohrasb
-Version: 3.1.0
-Summary: Using optuna search optimizer to estimate best tree based estimator compatible with scikit-learn
+Version: 3.2.0
+Summary: A scalable estimator optimization tool compatible with scikit-learn APIs
 Home-page: https://github.com/drhosseinjavedani/lohrasb
 License: BSD-3-Clause license
 Keywords: Auto ML,Pipeline,Machine learning
 Author: drhosseinjavedani
 Author-email: h.javedani@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
```

