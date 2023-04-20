# Comparing `tmp/trubrics-1.3.3.tar.gz` & `tmp/trubrics-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trubrics-1.3.3.tar", last modified: Wed Apr  5 15:12:11 2023, max compression
+gzip compressed data, was "trubrics-1.3.4.tar", last modified: Thu Apr 20 17:33:10 2023, max compression
```

## Comparing `trubrics-1.3.3.tar` & `trubrics-1.3.4.tar`

### file list

```diff
@@ -1,76 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.513108 trubrics-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-04-05 15:11:59.000000 trubrics-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-05 15:12:11.513108 trubrics-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-04-05 15:11:59.000000 trubrics-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.501108 trubrics-1.3.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:11:59.000000 trubrics-1.3.3/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.505108 trubrics-1.3.3/examples/classification_titanic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:11:59.000000 trubrics-1.3.3/examples/classification_titanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-05 15:11:59.000000 trubrics-1.3.3/examples/classification_titanic/custom_scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-05 15:11:59.000000 trubrics-1.3.3/examples/classification_titanic/custom_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    35305 2023-04-05 15:11:59.000000 trubrics-1.3.3/examples/classification_titanic/my_first_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)    35305 2023-04-05 15:11:59.000000 trubrics-1.3.3/examples/classification_titanic/my_new_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-05 15:11:59.000000 trubrics-1.3.3/examples/classification_titanic/slicing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-05 15:11:59.000000 trubrics-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-05 15:11:59.000000 trubrics-1.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-05 15:12:11.513108 trubrics-1.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.505108 trubrics-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-05 15:11:59.000000 trubrics-1.3.3/tests/test_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.505108 trubrics-1.3.3/trubrics/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.505108 trubrics-1.3.3/trubrics/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.509108 trubrics-1.3.3/trubrics/example/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/example/app_titanic_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/example/app_titanic_gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/example/app_titanic_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/example/my_first_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/example/titanic.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/example/titanic_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/example/titanic_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/example/trubric_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.509108 trubrics-1.3.3/trubrics/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/feedback/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/feedback/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.509108 trubrics-1.3.3/trubrics/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.509108 trubrics-1.3.3/trubrics/integrations/dash/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/integrations/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/integrations/dash/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.509108 trubrics-1.3.3/trubrics/integrations/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/integrations/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/integrations/gradio/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.509108 trubrics-1.3.3/trubrics/integrations/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/integrations/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15741 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/integrations/streamlit/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/integrations/streamlit/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.513108 trubrics-1.3.3/trubrics/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/ui/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/ui/firestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/ui/trubrics_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.513108 trubrics-1.3.3/trubrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/utils/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.513108 trubrics-1.3.3/trubrics/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/validations/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.513108 trubrics-1.3.3/trubrics/validations/model/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/validations/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30071 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/validations/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/validations/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-05 15:11:59.000000 trubrics-1.3.3/trubrics/validations/validation_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:12:11.505108 trubrics-1.3.3/trubrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-05 15:12:11.000000 trubrics-1.3.3/trubrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-05 15:12:11.000000 trubrics-1.3.3/trubrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:12:11.000000 trubrics-1.3.3/trubrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-05 15:12:11.000000 trubrics-1.3.3/trubrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-05 15:12:11.000000 trubrics-1.3.3/trubrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 15:12:11.000000 trubrics-1.3.3/trubrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.468799 trubrics-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-04-20 17:33:00.000000 trubrics-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-20 17:33:10.468799 trubrics-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-04-20 17:33:00.000000 trubrics-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.460799 trubrics-1.3.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.460799 trubrics-1.3.4/examples/classification_titanic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/classification_titanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/classification_titanic/custom_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/classification_titanic/custom_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35305 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/classification_titanic/my_first_trubric.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35305 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/classification_titanic/my_new_trubric.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 17:33:00.000000 trubrics-1.3.4/examples/classification_titanic/slicing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-20 17:33:00.000000 trubrics-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-20 17:33:00.000000 trubrics-1.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-20 17:33:10.468799 trubrics-1.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.460799 trubrics-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-20 17:33:00.000000 trubrics-1.3.4/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/app_titanic_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/app_titanic_gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/app_titanic_streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/my_first_trubric.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/titanic_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/titanic_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/example/trubric_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/feedback/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/feedback/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/integrations/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/dash/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/integrations/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/gradio/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics/integrations/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/mlflow/trubrics_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.468799 trubrics-1.3.4/trubrics/integrations/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/streamlit/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/integrations/streamlit/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.468799 trubrics-1.3.4/trubrics/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/ui/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/ui/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/ui/trubrics_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.468799 trubrics-1.3.4/trubrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/utils/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.468799 trubrics-1.3.4/trubrics/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/validations/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.468799 trubrics-1.3.4/trubrics/validations/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/validations/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/validations/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/validations/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-20 17:33:00.000000 trubrics-1.3.4/trubrics/validations/validation_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:33:10.464799 trubrics-1.3.4/trubrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-20 17:33:10.000000 trubrics-1.3.4/trubrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-20 17:33:10.000000 trubrics-1.3.4/trubrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:33:10.000000 trubrics-1.3.4/trubrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-20 17:33:10.000000 trubrics-1.3.4/trubrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-20 17:33:10.000000 trubrics-1.3.4/trubrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 17:33:10.000000 trubrics-1.3.4/trubrics.egg-info/top_level.txt
```

### Comparing `trubrics-1.3.3/LICENSE` & `trubrics-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/README.md` & `trubrics-1.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,18 @@
 
 demo.launch()
 ```
 </details>
 
 ## Validate a model with the ModelValidator
 
+👇 **click here** to dive directly into our example notebook on colab
+
+[![](./assets/colab-logo.png).ipynb](https://colab.research.google.com/github/trubrics/trubrics-sdk/blob/main/examples/classification_titanic/classification_full_demo.ipynb)
+
 To close the loop on feedback issues and ensure they are not repeated, ML practitioners can build validations.
 There are three main steps to creating model validations with the trubrics-sdk:
 
 1. Initialise a `DataContext`, that wraps ML datasets and metadata into a trubrics friendly object.
 2. Build validations with the `ModelValidator`, using the `DataContext` and any ML model (scikit-learn or [any python model](https://trubrics.github.io/trubrics-sdk/models/)). The `ModelValidator` holds a number of [out-of-the-box validations](https://trubrics.github.io/trubrics-sdk/validations/) and can also be used to build [custom validations](https://trubrics.github.io/trubrics-sdk/custom_validations/) from a python function.
 3. Group validations into a `Trubric`, which is  saved as a .json file and rerun against any model / dataset.
 
@@ -143,16 +147,14 @@
 )
 trubric.save_local(path="./my_first_trubric.json")  # save trubric as a local .json file
 trubric.save_ui()  # or to the Trubrics platform
 ```
 
 The `Trubric` defines the gold standard of validations required for your project, and may be used to validate any combination of model and `DataContext`. Once saved as a .json, the trubric may be run directly from the [CLI](https://trubrics.github.io/trubrics-sdk/run_trubrics/).
 
-_See a full tutorial on the titanic dataset [here](https://trubrics.github.io/trubrics-sdk/notebooks/titanic-full-demo.html)_.
-
 
 ## Track all feedback and validations in Trubrics
 
 The Trubrics platform allows teams to collaborate on model issues and track validation changes. Please get in touch with us [here](https://trubrics.com/demo/) to gain access to Trubrics for you and your team.
 
 [![img](assets/trubrics-login.png)](https://trubrics.com/demo/)
```

### Comparing `trubrics-1.3.3/examples/classification_titanic/custom_validator.py` & `trubrics-1.3.4/examples/classification_titanic/custom_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/examples/classification_titanic/my_first_trubric.json` & `trubrics-1.3.4/examples/classification_titanic/my_first_trubric.json`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/examples/classification_titanic/my_new_trubric.json` & `trubrics-1.3.4/examples/classification_titanic/my_new_trubric.json`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/setup.cfg` & `trubrics-1.3.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [metadata]
 name = trubrics
-version = 1.3.3
+version = 1.3.4
 description = Combine data science knowledge with business user feedback to validate machine learning.
 long_description = Full documentation available at https://trubrics.github.io/trubrics-sdk/.
 
 [options]
 packages = find:
 install_requires = file: requirements.txt
 
 [options.entry_points]
 console_scripts = 
 	trubrics = trubrics.cli.main:app
+mlflow.model_evaluator = 
+	trubrics = trubrics.integrations.mlflow.trubrics_validator:TrubricsValidator
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [options.package_data]
 * = *.typed, *.csv, *.json
@@ -25,12 +27,13 @@
 [isort]
 profile = black
 
 [options.extras_require]
 streamlit = streamlit>=1.11.1,<1.18.0
 dash = dash>=2.6.2; dash-bootstrap-components>=1.2.1
 gradio = gradio>=3.8.1
+mlflow = mlflow>=2.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trubrics-1.3.3/tests/test_context.py` & `trubrics-1.3.4/tests/test_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+from pydantic import ValidationError
 
 from trubrics.context import DataContext
 from trubrics.exceptions import PandasSchemaError
 from trubrics.validations.dataclass import Validation
 
 
 def test_data_context_attributes(dummy_testing_data):
@@ -38,14 +39,19 @@
     with pytest.raises(error_type):
         DataContext(testing_data=dummy_testing_data, training_data=training_data, **kwargs)
 
 
 @pytest.mark.parametrize(
     "kwargs,error_type",
     [
-        ({"outcome": "wrong_outcome", "severity": "experiment"}, KeyError),
-        ({"outcome": "pass", "severity": "wrong_severity"}, KeyError),
+        ({"passed": "wrong_outcome", "severity": "experiment"}, ValidationError),
+        ({"passed": True, "severity": "wrong_severity"}, KeyError),
     ],
 )
 def test_validation_context_raises(kwargs, error_type):
     with pytest.raises(error_type):
-        Validation(validation_type="validate_something", validation_kwargs={"a kwarg": None}, **kwargs)
+        Validation(
+            validation_type="validate_something",
+            validation_kwargs={"a kwarg": None},
+            explanation="some docstring",
+            **kwargs
+        )
```

### Comparing `trubrics-1.3.3/trubrics/cli/main.py` & `trubrics-1.3.4/trubrics/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,15 @@
     run_context_path: str = typer.Option(
         default="titanic-example-trubric", prompt="Enter the path to your trubric run .py file. Press enter for example"
     ),
     trubric_output_file_path: str = typer.Option(
         "./my_new_trubric.json",
         prompt="Enter a local path to save your output trubric file. Press enter for default path",
     ),
+    raise_on_failure: bool = True,
 ):
     """Runs an example trubric (list of model validations) on the titanic dataset.
 
     Args:
         save_ui: whether to save validations to the UI with in app user authentication
         run_context_path: path to the trubrics run context
         trubric_output_file_path: path to save your output trubric file
@@ -230,26 +231,26 @@
         f"\nRunning trubric from file '{trubric_run_path or 'trubrics.example.trubric_run'}' with model"
         f" '{rc.model_name}' and dataset '{rc.data_context.name}'.\n"
     )
     new_trubric = rc.set_new_trubric()
     if save_ui:
         trubrics_config = load_trubrics_config().dict()
         if trubrics_config["email"] is not None:
-            new_trubric.save_ui()
+            new_trubric.save_ui(raise_on_failure=raise_on_failure)
         else:
             typer.echo(
                 typer.style(
-                    "ERROR: You must authenticate with the trubrics manager by running `trubrics init` to remotely save"
-                    " trubrics runs.",
+                    "ERROR: You must authenticate with the Trubrics platform by running `trubrics init` to remotely"
+                    " save trubrics runs.",
                     fg=typer.colors.RED,
                 )
             )
     else:
         defaults = TrubricsDefaults()
-        new_trubric.save_local(trubric_output_file_path)
+        new_trubric.save_local(trubric_output_file_path, raise_on_failure=raise_on_failure)
         rprint(
             "\n[bold orange_red1]Be sure to check out our docs to see how you can leverage the Trubrics platform."
             f"\n\n{defaults.demo_sign_up_url}[bold orange_red1]\n"
         )
 
 
 if __name__ == "__main__":
```

### Comparing `trubrics-1.3.3/trubrics/cli/run.py` & `trubrics-1.3.4/trubrics/cli/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/context.py` & `trubrics-1.3.4/trubrics/context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/example/app_titanic_streamlit.py` & `trubrics-1.3.4/trubrics/example/app_titanic_streamlit.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/example/my_first_trubric.json` & `trubrics-1.3.4/trubrics/example/my_first_trubric.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.989010989010989%*

 * *Differences: {"'validations'": "{0: {'passed': False, delete: ['outcome']}, 1: {'passed': True, delete: "*

 * *                  "['outcome']}, 2: {'passed': True, delete: ['outcome']}, 3: {'passed': True, "*

 * *                  "delete: ['outcome']}, 4: {'passed': True, delete: ['outcome']}}"}*

```diff
@@ -12,15 +12,15 @@
     ],
     "timestamp": 1676366706,
     "total_passed": 4,
     "total_passed_percent": 80.0,
     "validations": [
         {
             "explanation": "**Performance validation versus a fixed threshold value.**\n\nCompares performance of a model on any of the datasets in the DataContext to a hard coded threshold value.\n\nExample:\n```py\nfrom trubrics.validations import ModelValidator\nmodel_validator = ModelValidator(data=data_context, model=model)\nmodel_validator.validate_performance_against_threshold(\nmetric=\"recall\",\nthreshold=0.8\n)\n```\n\nArgs:\nmetric: performance metric name defined in sklearn (sklearn.metrics.SCORERS) or in a custom scorer fed in when initialising the ModelValidator object.\nthreshold: the performance threshold that the model must attain.\ndataset: the name of a dataset from the DataContext {'testing_data', 'training_data'}.\ndata_slice: the name of the data slice, specified in the slicing_functions parameter of ModelValidator.\nseverity: severity of the validation. Can be either {'error', 'warning', 'experiment'}. If None, defaults to 'error'.\n\nReturns:\nTrue for success, false otherwise. With a results dictionary giving the actual model performance calculated.\n",
-            "outcome": "fail",
+            "passed": false,
             "result": {
                 "performance": 0.7184466019417476,
                 "sample_size": 295
             },
             "severity": "warning",
             "validation_kwargs": {
                 "args": [],
@@ -29,15 +29,15 @@
                     "threshold": 0.8
                 }
             },
             "validation_type": "validate_performance_against_threshold"
         },
         {
             "explanation": "**Performance validation versus a fixed threshold value.**\n\nCompares performance of a model on any of the datasets in the DataContext to a hard coded threshold value.\n\nExample:\n```py\nfrom trubrics.validations import ModelValidator\nmodel_validator = ModelValidator(data=data_context, model=model)\nmodel_validator.validate_performance_against_threshold(\nmetric=\"recall\",\nthreshold=0.8\n)\n```\n\nArgs:\nmetric: performance metric name defined in sklearn (sklearn.metrics.SCORERS) or in a custom scorer fed in when initialising the ModelValidator object.\nthreshold: the performance threshold that the model must attain.\ndataset: the name of a dataset from the DataContext {'testing_data', 'training_data'}.\ndata_slice: the name of the data slice, specified in the slicing_functions parameter of ModelValidator.\nseverity: severity of the validation. Can be either {'error', 'warning', 'experiment'}. If None, defaults to 'error'.\n\nReturns:\nTrue for success, false otherwise. With a results dictionary giving the actual model performance calculated.\n",
-            "outcome": "pass",
+            "passed": true,
             "result": {
                 "performance": 0.7047619047619048,
                 "sample_size": 295
             },
             "severity": "error",
             "validation_kwargs": {
                 "args": [],
@@ -46,15 +46,15 @@
                     "threshold": 0.7
                 }
             },
             "validation_type": "validate_performance_against_threshold"
         },
         {
             "explanation": "**Performance validation versus a fixed threshold value.**\n\nCompares performance of a model on any of the datasets in the DataContext to a hard coded threshold value.\n\nExample:\n```py\nfrom trubrics.validations import ModelValidator\nmodel_validator = ModelValidator(data=data_context, model=model)\nmodel_validator.validate_performance_against_threshold(\nmetric=\"recall\",\nthreshold=0.8\n)\n```\n\nArgs:\nmetric: performance metric name defined in sklearn (sklearn.metrics.SCORERS) or in a custom scorer fed in when initialising the ModelValidator object.\nthreshold: the performance threshold that the model must attain.\ndataset: the name of a dataset from the DataContext {'testing_data', 'training_data'}.\ndata_slice: the name of the data slice, specified in the slicing_functions parameter of ModelValidator.\nseverity: severity of the validation. Can be either {'error', 'warning', 'experiment'}. If None, defaults to 'error'.\n\nReturns:\nTrue for success, false otherwise. With a results dictionary giving the actual model performance calculated.\n",
-            "outcome": "pass",
+            "passed": true,
             "result": {
                 "performance": 0.7115384615384616,
                 "sample_size": 295
             },
             "severity": "experiment",
             "validation_kwargs": {
                 "args": [],
@@ -63,15 +63,15 @@
                     "threshold": 0.7
                 }
             },
             "validation_type": "validate_performance_against_threshold"
         },
         {
             "explanation": "**Performance validation of testing data versus a dummy baseline model.**\n\nTrains a DummyClassifier / DummyRegressor from [sklearn](https://scikit-learn.org/stable/modules/classes.html?highlight=dummy#module-sklearn.dummy) and compares performance against the model on the test set.\n\nExample:\n```py\nfrom trubrics.validations import ModelValidator\nmodel_validator = ModelValidator(data=data_context, model=model)\nmodel_validator.validate_test_performance_against_dummy(\nmetric=\"accuracy\",\nstrategy=\"stratified\"\n)\n```\n\nArgs:\nmetric: performance metric name defined in sklearn (sklearn.metrics.SCORERS) or in a custom scorer fed in when initialising the ModelValidator object.\nstrategy: strategy of scikit-learns dummy model.\ndummy_kwargs: kwargs to be passed to dummy model.\ndata_slice: the name of the data slice, specified in the slicing_functions parameter of ModelValidator.\nseverity: severity of the validation. Can be either ['error', 'warning', 'experiment']. If None, defaults to 'error'.\n\nReturns:\nTrue for success, false otherwise. With a results dictionary giving the model's actual performance on the test set and the dummy model's performance.\n",
-            "outcome": "pass",
+            "passed": true,
             "result": {
                 "dummy_performance": 0.6508474576271186,
                 "sample_size": 295,
                 "test_performance": 0.7966101694915254
             },
             "severity": "error",
             "validation_kwargs": {
@@ -80,15 +80,15 @@
                     "metric": "accuracy"
                 }
             },
             "validation_type": "validate_test_performance_against_dummy"
         },
         {
             "explanation": "**Performance validation of testing data versus a dummy baseline model.**\n\nTrains a DummyClassifier / DummyRegressor from [sklearn](https://scikit-learn.org/stable/modules/classes.html?highlight=dummy#module-sklearn.dummy) and compares performance against the model on the test set.\n\nExample:\n```py\nfrom trubrics.validations import ModelValidator\nmodel_validator = ModelValidator(data=data_context, model=model)\nmodel_validator.validate_test_performance_against_dummy(\nmetric=\"accuracy\",\nstrategy=\"stratified\"\n)\n```\n\nArgs:\nmetric: performance metric name defined in sklearn (sklearn.metrics.SCORERS) or in a custom scorer fed in when initialising the ModelValidator object.\nstrategy: strategy of scikit-learns dummy model.\ndummy_kwargs: kwargs to be passed to dummy model.\ndata_slice: the name of the data slice, specified in the slicing_functions parameter of ModelValidator.\nseverity: severity of the validation. Can be either ['error', 'warning', 'experiment']. If None, defaults to 'error'.\n\nReturns:\nTrue for success, false otherwise. With a results dictionary giving the model's actual performance on the test set and the dummy model's performance.\n",
-            "outcome": "pass",
+            "passed": true,
             "result": {
                 "dummy_performance": 0.6508474576271186,
                 "sample_size": 295,
                 "test_performance": 0.7966101694915254
             },
             "severity": "error",
             "validation_kwargs": {
```

### Comparing `trubrics-1.3.3/trubrics/example/titanic.py` & `trubrics-1.3.4/trubrics/example/titanic.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/example/titanic_data.csv` & `trubrics-1.3.4/trubrics/example/titanic_data.csv`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/example/trubric_run.py` & `trubrics-1.3.4/trubrics/example/trubric_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,9 +19,15 @@
 
 # Note: This method of reading json is only necessary from within python package.
 # Call `Trubric.parse_file("your_trubric.json")` to read in a trubric directly.
 stream = pkg_resources.resource_stream(__name__, "my_first_trubric.json")
 trubric = Trubric.parse_obj(json.load(stream))
 
 RUN_CONTEXT = TrubricRun(
-    data_context=data_context, model_name="titanic_model", model=model, tags=["titanic-dev"], trubric=trubric
+    data_context=data_context,
+    model_name="titanic_model",
+    model_version="0.0.1",
+    model=model,
+    tags=["cli-demo"],
+    trubric=trubric,
+    failing_severity="warning",
 )
```

### Comparing `trubrics-1.3.3/trubrics/exceptions.py` & `trubrics-1.3.4/trubrics/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 class ValidationOutputError(Exception):
     """An exception signalling that the output from a validation function is invalid."""
 
 
+class TrubricValidationError(Exception):
+    """An exception signalling a validation in a Trubric run has failed."""
+
+
 class PandasSchemaError(Exception):
     """An exception signalling that two DataFrames do not have the same schema (column names & types)."""
 
 
 class UnknownValidationError(Exception):
     """An exception signalling that validation is not recognised by a given validator."""
```

### Comparing `trubrics-1.3.3/trubrics/feedback/config.py` & `trubrics-1.3.4/trubrics/feedback/config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/feedback/dataclass.py` & `trubrics-1.3.4/trubrics/feedback/dataclass.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/integrations/dash/collect.py` & `trubrics-1.3.4/trubrics/integrations/dash/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/integrations/gradio/collect.py` & `trubrics-1.3.4/trubrics/integrations/gradio/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/integrations/streamlit/collect.py` & `trubrics-1.3.4/trubrics/integrations/streamlit/collect.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def __init__(
         self,
         data: Optional[str] = None,
         model: Optional[str] = None,
         trubrics_platform_auth: Optional[str] = None,
     ):
         """
-        The FeedbackCollector allows Data Scientists to collect feedback from with their app.
+        The FeedbackCollector allows Data Scientists to collect feedback from within their app.
 
         Args:
             data: a reference to the data that was used to collect the feedback (e.g. a link to a dataset)
             model: a reference to the model that was used to collect the feedback (e.g. a link to a model)
             trubrics_platform_auth: option to save the feedback to the trubrics platform
 
                 - *None*: save feedback locally to .json
@@ -95,16 +95,16 @@
 
         Args:
             feedback_type: type of feedback to be collected
 
                 - issue: issue with a open text title and description fields
                 - thumbs: positive or negative feedback with thumbs emojis
                 - faces: a scale of 1 to 5 with face emojis
-                - custom: any custom title and description str
-            user_response: a dict of user responses to save with your feedback
+                - custom: a customisable feedback type that allows users to specify the user_response dict
+            user_response: a dict of user responses to save with your feedback for feedback_type='custom'
             path: path to save feedback local .json. Defaults to "./*timestamp*_feedback.json"
             metadata: data to save with your feedback
             tags: a list of tags for your feedback
             key: a key for each streamlit component
             open_feedback_label: label of optional text_input for "faces" or "thumbs" feedback_type
         """
         if key is None:
```

### Comparing `trubrics-1.3.3/trubrics/integrations/streamlit/experiment.py` & `trubrics-1.3.4/trubrics/integrations/streamlit/experiment.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/ui/auth.py` & `trubrics-1.3.4/trubrics/ui/auth.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/ui/firestore.py` & `trubrics-1.3.4/trubrics/ui/firestore.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/ui/trubrics_config.py` & `trubrics-1.3.4/trubrics/ui/trubrics_config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.3/trubrics/validations/dataclass.py` & `trubrics-1.3.4/trubrics/validations/dataclass.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from typing import Any, Dict, List, Optional
 
 from git import InvalidGitRepositoryError
 from git.repo import Repo
 from loguru import logger
 from pydantic import BaseModel, validator
 
+from trubrics.exceptions import TrubricValidationError
 from trubrics.ui.auth import get_trubrics_auth_token
 from trubrics.ui.firestore import add_document_to_project_subcollection
 from trubrics.ui.trubrics_config import load_trubrics_config
 
 
 def _validation_context_example():
     return {
         "example": {
             "validation_type": "validate_performance_against_threshold",
             "validation_kwargs": {"args": [], "kwargs": {"threshold": 0.8}},
-            "outcome": "fail",
+            "passed": True,
             "severity": "error",
             "result": {"performance": "0.79"},
         }
     }
 
 
 class Validation(BaseModel):
@@ -30,102 +31,109 @@
 
     Note:
         A Validation object constrains the output of validations, with the @validation_output decorator.
 
     Attributes:
         validation_type: method name of the validation.
         validation_kwargs: all args and kwargs that the validation had run with.
-        explanation: docstring explanation of the validation.
-        outcome: pass or fail output of the validation.
+        passed: pass or fail output of the validation.
         severity: severity of the validation, can be one of ["error", "warning", "experiment"], is "error" by default
         result: a dictionary of contextual elements calculated during the validation run
+        explanation: docstring explanation of the validation.
     """
 
     validation_type: str
     validation_kwargs: Dict[str, Optional[Any]]
-    explanation: str
-    outcome: str
+    passed: bool
     severity: str = "error"
     result: Optional[Dict[str, Optional[Any]]]
+    explanation: str
 
     class Config:
         extra = "forbid"
         validate_assignment = True
         schema_extra = _validation_context_example()
 
     @validator("severity")
     def severity_must_be(cls, v: str):
         severity_values = ["error", "warning", "experiment"]
         if v not in severity_values:
             raise KeyError(f"Severity must be set to: {severity_values}.")
         return v
 
-    @validator("outcome")
-    def outcome_must_be(cls, v: str):
-        outcome_values = ["pass", "fail"]
-        if v not in outcome_values:
-            raise KeyError(f"Outcome must be set to: {outcome_values}.")
-        return v
-
 
 class Trubric(BaseModel):
     """
     Dataclass for a trubric, or set of validation points. Must be serialisable to .json.
     A Trubric must contain at least metadata about the DataContext used to create the validations,
     and should contain metadata also about any model that is used.
 
     Attributes:
         name: trubric name
+        passed: has trubric passed all validations (depends on the failing_severity)
+        total_passed: number of validations that passed (depends on the failing_severity)
+        total_failed: number of validations that failed (depends on the failing_severity)
+        failing_severity: minimum severity that the trubric fails on, can be one of ["error", "warning", "experiment"].
         data_context_name: data context name (from DataContext)
         data_context_version: data context version (from DataContext)
-        validations: list of validations (defined by Validation)
         model_name: model name
         model_version: model version
         tags: list of tags for the trubric
         run_by: who the trubric was run by
         git_commit: a git commit hash from the git repo where the trubric was run
-        metadata: free textual metadata field
         timestamp: timestamp at which the trubric was run
-        total_passed: number of validations that passed
-        total_passed_percent: percentage of passed validations
+        metadata: free textual metadata field
+        validations: list of validations (defined by Validation)
     """
 
     name: str
+    passed: Optional[bool] = None
+    total_passed: Optional[int] = None
+    total_failed: Optional[int] = None
+    failing_severity: str = "error"
     data_context_name: str
     data_context_version: str
-    validations: List[Validation]
     model_name: Optional[str] = None
     model_version: Optional[str] = None
     tags: List[Optional[str]] = []
     run_by: Optional[Dict[str, str]] = None
     git_commit: Optional[str] = None
-    metadata: Optional[Dict[str, str]] = None
     timestamp: Optional[int] = None
-    total_passed: Optional[int] = None
-    total_passed_percent: Optional[float] = None
+    metadata: Optional[Dict[str, str]] = None
+    validations: List[Validation]
 
     class Config:
         extra = "forbid"
 
-    def save_local(self, path: Optional[str] = None):
-        self._set_fields_on_save()
+    @validator("failing_severity")
+    def failing_severity_must_be(cls, v: str):
+        severity_values = ["error", "warning", "experiment"]
+        if v not in severity_values:
+            raise KeyError(f"Failing severity must be set to: {severity_values}.")
+        return v
+
+    def save_local(self, path: Optional[str] = None, raise_on_failure: bool = False):
+        self.set_dynamic_fields()
         if path is None:
             path = f"./{self.name}.json"
         with open(Path(path).absolute(), "w") as file:
             file.write(self.json(indent=4))
             logger.info(f"Trubric saved to {path}.")
 
-    def save_ui(self):
+        if raise_on_failure:
+            self.raise_trubric_failure()
+
+    def save_ui(self, raise_on_failure: bool = False):
         trubrics_config = load_trubrics_config()
         auth = get_trubrics_auth_token(
             trubrics_config.firebase_auth_api_url, trubrics_config.email, trubrics_config.password.get_secret_value()
         )
 
         self.run_by = {"email": trubrics_config.email, "displayName": trubrics_config.username}
-        self._set_fields_on_save()
+        self.set_dynamic_fields()
 
         res = add_document_to_project_subcollection(
             auth,
             firestore_api_url=trubrics_config.firestore_api_url,
             project=trubrics_config.project,
             subcollection="trubrics",
             document_id=self.timestamp,
@@ -134,19 +142,39 @@
         if "error" in res:
             error_msg = f"Error in pushing trubric to the Trubrics UI: {res}"
             logger.error(error_msg)
             raise Exception(error_msg)
         else:
             logger.info("Trubric saved to the Trubrics UI.")
 
-    def _set_fields_on_save(self):
-        self.total_passed = len([a for a in self.validations if a.outcome == "pass"])
-        self.total_passed_percent = round(100 * self.total_passed / len(self.validations), 1)
+        if raise_on_failure:
+            self.raise_trubric_failure()
+
+    def set_dynamic_fields(self):
+        if self.failing_severity == "warning":
+            failing_severity = ["error", "warning"]
+        elif self.failing_severity == "experiment":
+            failing_severity = ["error", "warning", "experiment"]
+        else:
+            failing_severity = ["error"]
+        validations = [validation for validation in self.validations if validation.severity in failing_severity]
+        self.total_passed = len([a for a in validations if a.passed])
+        self.total_failed = len(validations) - self.total_passed
+        self.passed = True if self.total_failed == 0 else False
         self.timestamp = int(datetime.now().timestamp())
         try:
             self.git_commit = Repo(search_parent_directories=True).head.object.hexsha
         except InvalidGitRepositoryError:
             self.git_commit = None
             logger.warning(
                 "Current directory is not a git repository. Run `trubrics run` inside a git repository to save the"
                 " commit hash."
             )
+        return self
+
+    def raise_trubric_failure(self):
+        if not self.passed and self.total_failed:
+            raise TrubricValidationError(
+                "Trubric has failed on"
+                f" {self.total_failed} {'validations' if self.total_failed > 1 else 'validation'} with minimum"
+                f" severity='{self.failing_severity}'."
+            )
```

### Comparing `trubrics-1.3.3/trubrics/validations/model/base.py` & `trubrics-1.3.4/trubrics/validations/model/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,16 +381,16 @@
         data_slice: Optional[str] = None,
     ) -> validation_output_type:
         test_score = self._score_data_context(metric, dataset="testing_data", data_slice=data_slice)
         test_sample_size = self.data_slice_sizes[self._get_renamed_dataset("testing_data", data_slice)]
         train_score = self._score_data_context(metric, dataset="training_data", data_slice=data_slice)
         train_sample_size = self.data_slice_sizes[self._get_renamed_dataset("training_data", data_slice)]
 
-        outcome = test_score < train_score and test_score >= train_score - threshold
-        return outcome, {
+        passed = test_score < train_score and test_score >= train_score - threshold
+        return passed, {
             "train_performance": train_score,
             "test_performance": test_score,
             "train_sample_size": train_sample_size,
             "test_sample_size": test_sample_size,
         }
 
     @validation_output
```

### Comparing `trubrics-1.3.3/trubrics/validations/run.py` & `trubrics-1.3.4/trubrics/validations/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,27 +32,30 @@
     model_version: Optional[str]
     trubric: Trubric
     metadata: Optional[Dict[str, str]] = None
     tags: List[Optional[str]] = []
     custom_validator: Any = None
     custom_scorers: Optional[Dict[str, Any]] = None
     slicing_functions: Optional[Dict[str, Any]] = None
+    failing_severity: Optional[str] = None
 
     @validator("custom_validator")
     def custom_validator_inherits_validator(cls, val):
-        if issubclass(val, ModelValidator):
-            return val
-        raise TypeError("Wrong type for 'custom_validator', must be subclass of ModelValidator.")
+        if val:
+            if issubclass(val, ModelValidator):
+                return val
+            raise TypeError("Wrong type for 'custom_validator', must be subclass of ModelValidator.")
 
     @validator("custom_scorers")
     def custom_scorer_is_make_scorer(cls, val):
-        for scorer in val:
-            if not issubclass(type(val[scorer]), _BaseScorer):
-                raise TypeError("Each scorer must be subclass of scikit-learn's _BaseScorer.")
-        return val
+        if val:
+            for scorer in val:
+                if not issubclass(type(val[scorer]), _BaseScorer):
+                    raise TypeError("Each scorer must be subclass of scikit-learn's _BaseScorer.")
+            return val
 
     def generate_validations_from_trubric(self) -> Iterator[Validation]:
         if self.custom_validator is not None:
             model_validator = self.custom_validator(
                 data=self.data_context,
                 model=self.model,
                 custom_scorers=self.custom_scorers,
@@ -67,15 +70,15 @@
             )
         for validation in self.trubric.validations:
             args = validation.validation_kwargs["args"]
             kwargs = validation.validation_kwargs["kwargs"]
             try:
                 validation_result = getattr(model_validator, validation.validation_type)(*args, **kwargs)
                 new_validation = validation.copy()
-                new_validation.outcome = validation_result.outcome
+                new_validation.passed = validation_result.passed
                 new_validation.result = validation_result.result
                 yield new_validation
             except AttributeError:
                 raise UnknownValidationError(
                     f"The validation '{validation.validation_type}' does not appear to belong to a validator."
                     " Try adding the object that generated the validation to the 'custom_validator' parameter."
                 )
@@ -85,21 +88,23 @@
         validations = []
         for validation_result in all_validation_results:
             validations.append(validation_result)
 
             message_start = f"{validation_result.validation_type} [{validation_result.severity.upper()}]"
             completed_dots = f"[grey82]{(100 - len(message_start)) * '.'}[grey82]"
             message_end = (
-                f"[bold {'green' if validation_result.outcome == 'pass' else 'red'}]{validation_result.outcome.upper()}"
+                "[bold"
+                f" {'green' if validation_result.passed else 'red'}]{'PASS' if validation_result.passed else 'FAIL'}"
             )
             rprint(message_start + completed_dots + message_end)
 
         return Trubric(
             name=self.trubric.name,
+            failing_severity=self.failing_severity or self.trubric.failing_severity,
             model_name=self.model_name,
             model_version=self.model_version,
             data_context_name=self.data_context.name,
             data_context_version=self.data_context.version,
             metadata=self.metadata,
             tags=self.tags,
             validations=validations,
-        )
+        ).set_dynamic_fields()
```

### Comparing `trubrics-1.3.3/trubrics/validations/validation_output.py` & `trubrics-1.3.4/trubrics/validations/validation_output.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,19 +19,18 @@
     def inner(*args, **kwargs) -> Validation:
         output = func(*args, **kwargs)
 
         try:
             check_type("output", output, validation_output_type)
         except TypeError:
             raise ValidationOutputError(
-                f"Each validation should return an outcome and a result with type: {validation_output_type}"
+                f"Each validation should return a bool and a result with type: {validation_output_type}"
             )
 
-        outcome, result = output
-        outcome = _pass_or_fail(outcome)
+        passed, result = output
 
         if kwargs.get("severity"):
             severity = kwargs.pop("severity")
         else:
             severity = "error"
 
         if len(args) > 1:
@@ -53,15 +52,15 @@
             )
         stripped_docstring = "\n".join(" ".join(line.split()) for line in func.__doc__.split("\n"))
 
         return Validation(
             validation_type=func.__name__,
             validation_kwargs={"args": typed_args, "kwargs": typed_kwargs},
             explanation=stripped_docstring,
-            outcome=outcome,
+            passed=passed,
             severity=severity,
             result=typed_result,  # type: ignore
         )
 
     return inner
 
 
@@ -85,11 +84,7 @@
     except (OverflowError, TypeError) as e:
         if isinstance(obj, TrubricsModel):
             return False
         elif raise_error:
             raise e
         else:
             return False
-
-
-def _pass_or_fail(condition: bool) -> str:
-    return "pass" if condition else "fail"
```

### Comparing `trubrics-1.3.3/trubrics.egg-info/SOURCES.txt` & `trubrics-1.3.4/trubrics.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 trubrics/feedback/config.py
 trubrics/feedback/dataclass.py
 trubrics/integrations/__init__.py
 trubrics/integrations/dash/__init__.py
 trubrics/integrations/dash/collect.py
 trubrics/integrations/gradio/__init__.py
 trubrics/integrations/gradio/collect.py
+trubrics/integrations/mlflow/__init__.py
+trubrics/integrations/mlflow/trubrics_validator.py
 trubrics/integrations/streamlit/__init__.py
 trubrics/integrations/streamlit/collect.py
 trubrics/integrations/streamlit/experiment.py
 trubrics/ui/__init__.py
 trubrics/ui/auth.py
 trubrics/ui/firestore.py
 trubrics/ui/trubrics_config.py
```

