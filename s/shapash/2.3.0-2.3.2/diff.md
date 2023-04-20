# Comparing `tmp/shapash-2.3.0.tar.gz` & `tmp/shapash-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapash-2.3.0.tar", last modified: Wed Mar  1 13:18:10 2023, max compression
+gzip compressed data, was "shapash-2.3.2.tar", last modified: Thu Apr 20 09:46:44 2023, max compression
```

## Comparing `shapash-2.3.0.tar` & `shapash-2.3.2.tar`

### file list

```diff
@@ -1,102 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.961896 shapash-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-03-01 13:15:22.000000 shapash-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-01 13:15:22.000000 shapash-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20972 2023-03-01 13:18:10.961896 shapash-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20065 2023-03-01 13:15:22.000000 shapash-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-01 13:18:10.961896 shapash-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-03-01 13:15:22.000000 shapash-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.949896 shapash-2.3.0/shapash/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.949896 shapash-2.3.0/shapash/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/backend/acv_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/backend/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/backend/lime_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/backend/shap_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.949896 shapash-2.3.0/shapash/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)  1144733 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/data/house_prices_dataset.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/data/house_prices_labels.json
--rw-r--r--   0 runner    (1001) docker     (123)    67538 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/data/titanicdata.csv
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/data/titaniclabels.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.949896 shapash-2.3.0/shapash/decomposition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/decomposition/contributions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.953896 shapash-2.3.0/shapash/explainer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/explainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31303 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/explainer/consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/explainer/multi_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    58279 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/explainer/smart_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)   147146 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/explainer/smart_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/explainer/smart_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/explainer/smart_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.953896 shapash-2.3.0/shapash/manipulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/manipulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/manipulation/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/manipulation/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/manipulation/select_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/manipulation/summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.953896 shapash-2.3.0/shapash/report/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/base_report.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.953896 shapash-2.3.0/shapash/report/html/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/html/double_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/html/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/html/explainability.html
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/html/table_two_columns.html
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/html/univariate.html
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/project_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.945896 shapash-2.3.0/shapash/report/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.953896 shapash-2.3.0/shapash/report/template/custom/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/template/custom/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/template/custom/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/report/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.953896 shapash-2.3.0/shapash/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/style/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/style/colors.json
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/style/style_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.957896 shapash-2.3.0/shapash/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/category_encoder_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    19318 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/columntransformer_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/explanation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/load_smartpredictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/model_synoptic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.957896 shapash-2.3.0/shapash/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.957896 shapash-2.3.0/shapash/webapp/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   215609 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    88144 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/assets/jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/assets/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/assets/material-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/assets/reload.png
--rw-r--r--   0 runner    (1001) docker     (123)    29911 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/assets/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)   215609 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/assets/shapash-fond-fonce.png
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (123)   138558 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/smart_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.957896 shapash-2.3.0/shapash/webapp/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/utils/MyGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/utils/explanations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/webapp_launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-03-01 13:15:22.000000 shapash-2.3.0/shapash/webapp/webapp_launch_DVF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:10.949896 shapash-2.3.0/shapash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20972 2023-03-01 13:18:10.000000 shapash-2.3.0/shapash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-03-01 13:18:10.000000 shapash-2.3.0/shapash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 13:18:10.000000 shapash-2.3.0/shapash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 13:18:10.000000 shapash-2.3.0/shapash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-01 13:18:10.000000 shapash-2.3.0/shapash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-01 13:18:10.000000 shapash-2.3.0/shapash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.618071 shapash-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-20 09:43:34.000000 shapash-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 09:43:34.000000 shapash-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-04-20 09:46:44.618071 shapash-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20716 2023-04-20 09:43:34.000000 shapash-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-20 09:46:44.618071 shapash-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-20 09:43:34.000000 shapash-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.606071 shapash-2.3.2/shapash/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.610071 shapash-2.3.2/shapash/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/backend/acv_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/backend/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/backend/lime_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/backend/shap_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.610071 shapash-2.3.2/shapash/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/data/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.610071 shapash-2.3.2/shapash/decomposition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/decomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/decomposition/contributions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.610071 shapash-2.3.2/shapash/explainer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/explainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31311 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/explainer/consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/explainer/multi_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58279 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/explainer/smart_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147181 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/explainer/smart_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/explainer/smart_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/explainer/smart_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.610071 shapash-2.3.2/shapash/manipulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/manipulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/manipulation/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/manipulation/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/manipulation/select_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/manipulation/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.614071 shapash-2.3.2/shapash/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/base_report.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.614071 shapash-2.3.2/shapash/report/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/html/double_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/html/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/html/explainability.html
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/html/table_two_columns.html
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/html/univariate.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/project_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.602071 shapash-2.3.2/shapash/report/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.614071 shapash-2.3.2/shapash/report/template/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/template/custom/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/template/custom/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/report/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.614071 shapash-2.3.2/shapash/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/style/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/style/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/style/style_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.614071 shapash-2.3.2/shapash/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/category_encoder_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19318 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/columntransformer_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/explanation_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/load_smartpredictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/model_synoptic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.614071 shapash-2.3.2/shapash/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.618071 shapash-2.3.2/shapash/webapp/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   215609 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    88144 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/assets/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/assets/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/assets/material-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/assets/reload.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29911 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/assets/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)   215609 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/assets/shapash-fond-fonce.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)   138568 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/smart_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.618071 shapash-2.3.2/shapash/webapp/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/utils/MyGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/utils/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/webapp_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-20 09:43:34.000000 shapash-2.3.2/shapash/webapp/webapp_launch_DVF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:46:44.610071 shapash-2.3.2/shapash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-04-20 09:46:44.000000 shapash-2.3.2/shapash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-20 09:46:44.000000 shapash-2.3.2/shapash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:46:44.000000 shapash-2.3.2/shapash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:46:44.000000 shapash-2.3.2/shapash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-20 09:46:44.000000 shapash-2.3.2/shapash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 09:46:44.000000 shapash-2.3.2/shapash.egg-info/top_level.txt
```

### Comparing `shapash-2.3.0/LICENSE` & `shapash-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/PKG-INFO` & `shapash-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapash
-Version: 2.3.0
+Version: 2.3.2
 Summary: Shapash is a Python library which aims to make machine learning interpretable and understandable by everyone.
 Home-page: https://github.com/MAIF/shapash
 Author: Yann Golhen, Sebastien Bidault, Yann Lagre, Maxime Gendre
 Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0
 Keywords: shapash
 Classifier: Programming Language :: Python :: 3
@@ -56,24 +56,24 @@
 </p>
 
 ## 🎉 What's new ?
 
 
 | Version       | New Feature                                                                           | Description                                                                                                                            | Tutorial |
 |:-------------:|:-------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
-| 2.3.x         |  Additional dataset columns <br> (Demo coming soon)                                                                | In Webapp: Target and error columns added to dataset and possibility to add features outside the model for more filtering options            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/add_column_icon.png" width="50" title="add_column">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
-| 2.3.x         |  Identity card <br> (Demo coming soon)                                                                  | In Webapp: New identity card to summarize the information of the selected sample                  |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/identity_card.png" width="50" title="identity">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
-| 2.2.x         |  Picking samples <br> [New demo](https://shapash-demo.ossbymaif.fr/)                                                                | New tab in the webapp for picking samples. The graph represents the "True Values Vs Predicted Values"            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png" width="50" title="picking">](https://github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-prediction_plot.ipynb)
-| 2.2.x         |  Dataset Filter <br> [New demo](https://shapash-demo.ossbymaif.fr/)                                                                  | New tab in the webapp to filter data. And several improvements in the webapp: subtitles, labels, screen adjustments                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/webapp.png" width="50" title="webapp">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
+| 2.3.x         |  Additional dataset columns <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                | In Webapp: Target and error columns added to dataset and possibility to add features outside the model for more filtering options            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/add_column_icon.png" width="50" title="add_column">](https://github.com/MAIF/shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+| 2.3.x         |  Identity card <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                  | In Webapp: New identity card to summarize the information of the selected sample                  |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/identity_card.png" width="50" title="identity">](https://github.com/MAIF/shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+| 2.2.x         |  Picking samples <br> [Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-machine-learning-model.html)                                                                | New tab in the webapp for picking samples. The graph represents the "True Values Vs Predicted Values"            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png" width="50" title="picking">](https://github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-prediction_plot.ipynb)
+| 2.2.x         |  Dataset Filter <br>                                                              | New tab in the webapp to filter data. And several improvements in the webapp: subtitles, labels, screen adjustments                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/webapp.png" width="50" title="webapp">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
 | 2.0.x         |  Refactoring Shapash <br>                                                                   | Refactoring attributes of compile methods and init. Refactoring implementation for new backends                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/modular.png" width="50" title="modular">](https://github.com/MAIF/shapash/blob/master/tutorial/backend/tuto-backend-01.ipynb)
 | 1.7.x         |  Variabilize Colors <br>                                                                   | Giving possibility to have your own colour palette for outputs adapted to your design                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/variabilize-colors.png" width="50" title="variabilize-colors">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common02-colors.ipynb)
-| 1.6.x         |  Explainability Quality Metrics <br> [article](https://towardsdatascience.com/building-confidence-on-explainability-methods-66b9ee575514)                                                                   | To help increase confidence in explainability methods, you can evaluate the relevance of your explainability using 3 metrics: **Stability**, **Consistency** and **Compacity**                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-metrics.png" width="50" title="quality-metrics">](https://github.com/MAIF/shapash/blob/master/tutorial/explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb) 
+| 1.6.x         |  Explainability Quality Metrics <br> [Article](https://towardsdatascience.com/building-confidence-on-explainability-methods-66b9ee575514)                                                                   | To help increase confidence in explainability methods, you can evaluate the relevance of your explainability using 3 metrics: **Stability**, **Consistency** and **Compacity**                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-metrics.png" width="50" title="quality-metrics">](https://github.com/MAIF/shapash/blob/master/tutorial/explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb) 
 | 1.5.x         |  ACV Backend <br>                                                                     | A new way of estimating Shapley values using ACV. [More info about ACV here](https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-cfea30509254).                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/wheel.png" width="50" title="wheel-acv-backend">](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb)    |
-| 1.4.x         |  Groups of features <br> [demo](https://shapash-demo2.ossbymaif.fr/)                  | You can now regroup features that share common properties together. <br>This option can be useful if your model has a lot of features. |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/groups_features.gif" width="120" title="groups-features">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common01-groups_of_features.ipynb)    | 
-| 1.3.x         |  Shapash Report <br> [demo](https://shapash.readthedocs.io/en/latest/report.html)     | A standalone HTML report that constitutes a basis of an audit document.                                                                |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png" width="50" title="shapash-report">](https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-report01.ipynb)    | 
+| 1.4.x         |  Groups of features <br> [Demo](https://shapash-demo2.ossbymaif.fr/)                  | You can now regroup features that share common properties together. <br>This option can be useful if your model has a lot of features. |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/groups_features.gif" width="120" title="groups-features">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common01-groups_of_features.ipynb)    | 
+| 1.3.x         |  Shapash Report <br> [Demo](https://shapash.readthedocs.io/en/latest/report.html)     | A standalone HTML report that constitutes a basis of an audit document.                                                                |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png" width="50" title="shapash-report">](https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-report01.ipynb)    | 
 
 
 ## 🔍 Overview
 
 **Shapash** is a Python library which aims to make machine learning interpretable and understandable by everyone.
 It provides several types of visualization that display explicit labels that everyone can understand. 
 
@@ -85,14 +85,15 @@
 - [Presentation video for french speakers](https://www.youtube.com/watch?v=r1R_A9B9apk)
 - Medium:
   - [Understand your model with Shapash - Towards AI](https://pub.towardsai.net/shapash-making-ml-models-understandable-by-everyone-8f96ad469eb3) 
   - [Model auditability - Towards DS](https://towardsdatascience.com/shapash-1-3-2-announcing-new-features-for-more-auditable-ai-64a6db71c919)
   - [Group of features - Towards AI](https://pub.towardsai.net/machine-learning-6011d5d9a444)
   - [Building confidence on explainability - Towards DS](https://towardsdatascience.com/building-confidence-on-explainability-methods-66b9ee575514)
   - [Picking Examples to Understand Machine Learning Model](https://www.kdnuggets.com/2022/11/picking-examples-understand-machine-learning-model.html)
+  - [Enhancing Webapp Built-In Features for Comprehensive Machine Learning Model Interpretation](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)
 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/shapash_global.gif" width="800">
 </p>
 
 ## 🤝 Contributors
@@ -323,8 +324,12 @@
 
 <details><summary><b>Generate a report of your project</b> </summary>
 
 - [Generate a standalone HTML report of your project with generate_report](tutorial/report/tuto-shapash-report01.ipynb)
 
 </details>
 
+<details><summary><b>Analysing your model via Shapash WebApp</b> </summary>
 
+- [Add features outside of the model for more exploration options](tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+
+</details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shapash Version: 2.3.0 Summary: Shapash is a Python
+Metadata-Version: 2.1 Name: shapash Version: 2.3.2 Summary: Shapash is a Python
 library which aims to make machine learning interpretable and understandable by
 everyone. Home-page: https://github.com/MAIF/shapash Author: Yann Golhen,
 Sebastien Bidault, Yann Lagre, Maxime Gendre Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0 Keywords: shapash Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
@@ -14,63 +14,68 @@
                                   resize.png]
           [tests]  [pypi]  [downloads]  [pyversion]  [license]  [doc]
 ## ð What's new ? | Version | New Feature | Description | Tutorial | |:-----
 --------:|:--------------------------------------------------------------------
 -----------------:|:-----------------------------------------------------------
 ---------------------------------------------------------------------------:|:-
 -------:| | 2.3.x | Additional dataset columns
-(Demo coming soon) | In Webapp: Target and error columns added to dataset and
-possibility to add features outside the model for more filtering options | [
-[https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
+[New demo](https://shapash-demo.ossbymaif.fr/)
+[Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-
+interpretation-40b50157c2fb) | In Webapp: Target and error columns added to
+dataset and possibility to add features outside the model for more filtering
+options | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
 add_column_icon.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
-tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.3.x | Identity card
-(Demo coming soon) | In Webapp: New identity card to summarize the information
-of the selected sample | [[https://raw.githubusercontent.com/MAIF/shapash/
-master/docs/_static/identity_card.png]](https://github.com/MAIF/shapash/blob/
-master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.2.x |
-Picking samples
-[New demo](https://shapash-demo.ossbymaif.fr/) | New tab in the webapp for
-picking samples. The graph represents the "True Values Vs Predicted Values" | [
-[https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
-picking.png]](https://github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-
-plot06-prediction_plot.ipynb) | 2.2.x | Dataset Filter
-[New demo](https://shapash-demo.ossbymaif.fr/) | New tab in the webapp to
-filter data. And several improvements in the webapp: subtitles, labels, screen
-adjustments | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
-_static/webapp.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
-tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.0.x | Refactoring Shapash
+webapp/tuto-webapp01-additional-data.ipynb) | 2.3.x | Identity card
+[New demo](https://shapash-demo.ossbymaif.fr/)
+[Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-
+interpretation-40b50157c2fb) | In Webapp: New identity card to summarize the
+information of the selected sample | [[https://raw.githubusercontent.com/MAIF/
+shapash/master/docs/_static/identity_card.png]](https://github.com/MAIF/
+shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb) |
+2.2.x | Picking samples
+[Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-
+machine-learning-model.html) | New tab in the webapp for picking samples. The
+graph represents the "True Values Vs Predicted Values" | [[https://
+raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png]](https:
+//github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-
+prediction_plot.ipynb) | 2.2.x | Dataset Filter
+| New tab in the webapp to filter data. And several improvements in the webapp:
+subtitles, labels, screen adjustments | [[https://raw.githubusercontent.com/
+MAIF/shapash/master/docs/_static/webapp.png]](https://github.com/MAIF/shapash/
+blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.0.x |
+Refactoring Shapash
 | Refactoring attributes of compile methods and init. Refactoring
 implementation for new backends | [[https://raw.githubusercontent.com/MAIF/
 shapash/master/docs/_static/modular.png]](https://github.com/MAIF/shapash/blob/
 master/tutorial/backend/tuto-backend-01.ipynb) | 1.7.x | Variabilize Colors
 | Giving possibility to have your own colour palette for outputs adapted to
 your design | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
 _static/variabilize-colors.png]](https://github.com/MAIF/shapash/blob/master/
 tutorial/common/tuto-common02-colors.ipynb) | 1.6.x | Explainability Quality
 Metrics
-[article](https://towardsdatascience.com/building-confidence-on-explainability-
+[Article](https://towardsdatascience.com/building-confidence-on-explainability-
 methods-66b9ee575514) | To help increase confidence in explainability methods,
 you can evaluate the relevance of your explainability using 3 metrics:
 **Stability**, **Consistency** and **Compacity** | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-
 metrics.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
 explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb)
 | 1.5.x | ACV Backend
 | A new way of estimating Shapley values using ACV. [More info about ACV here]
 (https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-
 cfea30509254). | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
 _static/wheel.png]](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb) |
 | 1.4.x | Groups of features
-[demo](https://shapash-demo2.ossbymaif.fr/) | You can now regroup features that
+[Demo](https://shapash-demo2.ossbymaif.fr/) | You can now regroup features that
 share common properties together.
 This option can be useful if your model has a lot of features. | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
 groups_features.gif]](https://github.com/MAIF/shapash/blob/master/tutorial/
 common/tuto-common01-groups_of_features.ipynb) | | 1.3.x | Shapash Report
-[demo](https://shapash.readthedocs.io/en/latest/report.html) | A standalone
+[Demo](https://shapash.readthedocs.io/en/latest/report.html) | A standalone
 HTML report that constitutes a basis of an audit document. | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png]]
 (https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-
 report01.ipynb) | ## ð Overview **Shapash** is a Python library which aims
 to make machine learning interpretable and understandable by everyone. It
 provides several types of visualization that display explicit labels that
 everyone can understand. Data Scientists can understand their models easily and
@@ -85,15 +90,18 @@
 models-understandable-by-everyone-8f96ad469eb3) - [Model auditability - Towards
 DS](https://towardsdatascience.com/shapash-1-3-2-announcing-new-features-for-
 more-auditable-ai-64a6db71c919) - [Group of features - Towards AI](https://
 pub.towardsai.net/machine-learning-6011d5d9a444) - [Building confidence on
 explainability - Towards DS](https://towardsdatascience.com/building-
 confidence-on-explainability-methods-66b9ee575514) - [Picking Examples to
 Understand Machine Learning Model](https://www.kdnuggets.com/2022/11/picking-
-examples-understand-machine-learning-model.html)
+examples-understand-machine-learning-model.html) - [Enhancing Webapp Built-In
+Features for Comprehensive Machine Learning Model Interpretation](https://
+pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-
+40b50157c2fb)
      [https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
                               shapash_global.gif]
 ## ð¤ Contributors
 [https://github.com/MAIF/shapash/blob/master/docs/_static/logo_maif.png]
 [https://github.com/MAIF/shapash/blob/master/docs/_static/logo_quantmetry.png]
 [https://github.com/MAIF/shapash/blob/master/docs/_static/
 logo_societe_generale.png] [https://github.com/MAIF/shapash/blob/master/docs/
@@ -226,8 +234,10 @@
 tuto-expl03-Shapash-acv-backend.ipynb) - [Compile faster Lime and consistency
 of contributions](tutorial/explainer/tuto-expl04-Shapash-compute-Lime-
 faster.ipynb)  Evaluating the quality of your explainability  - [Building
 confidence on explainability methods using **Stability**, **Consistency** and
 **Compacity** metrics](tutorial/explainability_quality/tuto-quality01-Builing-
 confidence-explainability.ipynb)  Generate a report of your project  -
 [Generate a standalone HTML report of your project with generate_report]
-(tutorial/report/tuto-shapash-report01.ipynb)
+(tutorial/report/tuto-shapash-report01.ipynb)  Analysing your model via Shapash
+WebApp  - [Add features outside of the model for more exploration options]
+(tutorial/webapp/tuto-webapp01-additional-data.ipynb)
```

### Comparing `shapash-2.3.0/README.md` & `shapash-2.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,24 +31,24 @@
 </p>
 
 ## 🎉 What's new ?
 
 
 | Version       | New Feature                                                                           | Description                                                                                                                            | Tutorial |
 |:-------------:|:-------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
-| 2.3.x         |  Additional dataset columns <br> (Demo coming soon)                                                                | In Webapp: Target and error columns added to dataset and possibility to add features outside the model for more filtering options            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/add_column_icon.png" width="50" title="add_column">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
-| 2.3.x         |  Identity card <br> (Demo coming soon)                                                                  | In Webapp: New identity card to summarize the information of the selected sample                  |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/identity_card.png" width="50" title="identity">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
-| 2.2.x         |  Picking samples <br> [New demo](https://shapash-demo.ossbymaif.fr/)                                                                | New tab in the webapp for picking samples. The graph represents the "True Values Vs Predicted Values"            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png" width="50" title="picking">](https://github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-prediction_plot.ipynb)
-| 2.2.x         |  Dataset Filter <br> [New demo](https://shapash-demo.ossbymaif.fr/)                                                                  | New tab in the webapp to filter data. And several improvements in the webapp: subtitles, labels, screen adjustments                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/webapp.png" width="50" title="webapp">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
+| 2.3.x         |  Additional dataset columns <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                | In Webapp: Target and error columns added to dataset and possibility to add features outside the model for more filtering options            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/add_column_icon.png" width="50" title="add_column">](https://github.com/MAIF/shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+| 2.3.x         |  Identity card <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                  | In Webapp: New identity card to summarize the information of the selected sample                  |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/identity_card.png" width="50" title="identity">](https://github.com/MAIF/shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+| 2.2.x         |  Picking samples <br> [Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-machine-learning-model.html)                                                                | New tab in the webapp for picking samples. The graph represents the "True Values Vs Predicted Values"            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png" width="50" title="picking">](https://github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-prediction_plot.ipynb)
+| 2.2.x         |  Dataset Filter <br>                                                              | New tab in the webapp to filter data. And several improvements in the webapp: subtitles, labels, screen adjustments                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/webapp.png" width="50" title="webapp">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
 | 2.0.x         |  Refactoring Shapash <br>                                                                   | Refactoring attributes of compile methods and init. Refactoring implementation for new backends                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/modular.png" width="50" title="modular">](https://github.com/MAIF/shapash/blob/master/tutorial/backend/tuto-backend-01.ipynb)
 | 1.7.x         |  Variabilize Colors <br>                                                                   | Giving possibility to have your own colour palette for outputs adapted to your design                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/variabilize-colors.png" width="50" title="variabilize-colors">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common02-colors.ipynb)
-| 1.6.x         |  Explainability Quality Metrics <br> [article](https://towardsdatascience.com/building-confidence-on-explainability-methods-66b9ee575514)                                                                   | To help increase confidence in explainability methods, you can evaluate the relevance of your explainability using 3 metrics: **Stability**, **Consistency** and **Compacity**                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-metrics.png" width="50" title="quality-metrics">](https://github.com/MAIF/shapash/blob/master/tutorial/explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb) 
+| 1.6.x         |  Explainability Quality Metrics <br> [Article](https://towardsdatascience.com/building-confidence-on-explainability-methods-66b9ee575514)                                                                   | To help increase confidence in explainability methods, you can evaluate the relevance of your explainability using 3 metrics: **Stability**, **Consistency** and **Compacity**                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-metrics.png" width="50" title="quality-metrics">](https://github.com/MAIF/shapash/blob/master/tutorial/explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb) 
 | 1.5.x         |  ACV Backend <br>                                                                     | A new way of estimating Shapley values using ACV. [More info about ACV here](https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-cfea30509254).                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/wheel.png" width="50" title="wheel-acv-backend">](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb)    |
-| 1.4.x         |  Groups of features <br> [demo](https://shapash-demo2.ossbymaif.fr/)                  | You can now regroup features that share common properties together. <br>This option can be useful if your model has a lot of features. |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/groups_features.gif" width="120" title="groups-features">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common01-groups_of_features.ipynb)    | 
-| 1.3.x         |  Shapash Report <br> [demo](https://shapash.readthedocs.io/en/latest/report.html)     | A standalone HTML report that constitutes a basis of an audit document.                                                                |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png" width="50" title="shapash-report">](https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-report01.ipynb)    | 
+| 1.4.x         |  Groups of features <br> [Demo](https://shapash-demo2.ossbymaif.fr/)                  | You can now regroup features that share common properties together. <br>This option can be useful if your model has a lot of features. |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/groups_features.gif" width="120" title="groups-features">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common01-groups_of_features.ipynb)    | 
+| 1.3.x         |  Shapash Report <br> [Demo](https://shapash.readthedocs.io/en/latest/report.html)     | A standalone HTML report that constitutes a basis of an audit document.                                                                |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png" width="50" title="shapash-report">](https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-report01.ipynb)    | 
 
 
 ## 🔍 Overview
 
 **Shapash** is a Python library which aims to make machine learning interpretable and understandable by everyone.
 It provides several types of visualization that display explicit labels that everyone can understand. 
 
@@ -60,14 +60,15 @@
 - [Presentation video for french speakers](https://www.youtube.com/watch?v=r1R_A9B9apk)
 - Medium:
   - [Understand your model with Shapash - Towards AI](https://pub.towardsai.net/shapash-making-ml-models-understandable-by-everyone-8f96ad469eb3) 
   - [Model auditability - Towards DS](https://towardsdatascience.com/shapash-1-3-2-announcing-new-features-for-more-auditable-ai-64a6db71c919)
   - [Group of features - Towards AI](https://pub.towardsai.net/machine-learning-6011d5d9a444)
   - [Building confidence on explainability - Towards DS](https://towardsdatascience.com/building-confidence-on-explainability-methods-66b9ee575514)
   - [Picking Examples to Understand Machine Learning Model](https://www.kdnuggets.com/2022/11/picking-examples-understand-machine-learning-model.html)
+  - [Enhancing Webapp Built-In Features for Comprehensive Machine Learning Model Interpretation](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)
 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/shapash_global.gif" width="800">
 </p>
 
 ## 🤝 Contributors
@@ -298,8 +299,12 @@
 
 <details><summary><b>Generate a report of your project</b> </summary>
 
 - [Generate a standalone HTML report of your project with generate_report](tutorial/report/tuto-shapash-report01.ipynb)
 
 </details>
 
+<details><summary><b>Analysing your model via Shapash WebApp</b> </summary>
 
+- [Add features outside of the model for more exploration options](tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+
+</details>
```

#### html2text {}

```diff
@@ -2,63 +2,68 @@
                                   resize.png]
           [tests]  [pypi]  [downloads]  [pyversion]  [license]  [doc]
 ## ð What's new ? | Version | New Feature | Description | Tutorial | |:-----
 --------:|:--------------------------------------------------------------------
 -----------------:|:-----------------------------------------------------------
 ---------------------------------------------------------------------------:|:-
 -------:| | 2.3.x | Additional dataset columns
-(Demo coming soon) | In Webapp: Target and error columns added to dataset and
-possibility to add features outside the model for more filtering options | [
-[https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
+[New demo](https://shapash-demo.ossbymaif.fr/)
+[Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-
+interpretation-40b50157c2fb) | In Webapp: Target and error columns added to
+dataset and possibility to add features outside the model for more filtering
+options | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
 add_column_icon.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
-tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.3.x | Identity card
-(Demo coming soon) | In Webapp: New identity card to summarize the information
-of the selected sample | [[https://raw.githubusercontent.com/MAIF/shapash/
-master/docs/_static/identity_card.png]](https://github.com/MAIF/shapash/blob/
-master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.2.x |
-Picking samples
-[New demo](https://shapash-demo.ossbymaif.fr/) | New tab in the webapp for
-picking samples. The graph represents the "True Values Vs Predicted Values" | [
-[https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
-picking.png]](https://github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-
-plot06-prediction_plot.ipynb) | 2.2.x | Dataset Filter
-[New demo](https://shapash-demo.ossbymaif.fr/) | New tab in the webapp to
-filter data. And several improvements in the webapp: subtitles, labels, screen
-adjustments | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
-_static/webapp.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
-tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.0.x | Refactoring Shapash
+webapp/tuto-webapp01-additional-data.ipynb) | 2.3.x | Identity card
+[New demo](https://shapash-demo.ossbymaif.fr/)
+[Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-
+interpretation-40b50157c2fb) | In Webapp: New identity card to summarize the
+information of the selected sample | [[https://raw.githubusercontent.com/MAIF/
+shapash/master/docs/_static/identity_card.png]](https://github.com/MAIF/
+shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb) |
+2.2.x | Picking samples
+[Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-
+machine-learning-model.html) | New tab in the webapp for picking samples. The
+graph represents the "True Values Vs Predicted Values" | [[https://
+raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png]](https:
+//github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-
+prediction_plot.ipynb) | 2.2.x | Dataset Filter
+| New tab in the webapp to filter data. And several improvements in the webapp:
+subtitles, labels, screen adjustments | [[https://raw.githubusercontent.com/
+MAIF/shapash/master/docs/_static/webapp.png]](https://github.com/MAIF/shapash/
+blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.0.x |
+Refactoring Shapash
 | Refactoring attributes of compile methods and init. Refactoring
 implementation for new backends | [[https://raw.githubusercontent.com/MAIF/
 shapash/master/docs/_static/modular.png]](https://github.com/MAIF/shapash/blob/
 master/tutorial/backend/tuto-backend-01.ipynb) | 1.7.x | Variabilize Colors
 | Giving possibility to have your own colour palette for outputs adapted to
 your design | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
 _static/variabilize-colors.png]](https://github.com/MAIF/shapash/blob/master/
 tutorial/common/tuto-common02-colors.ipynb) | 1.6.x | Explainability Quality
 Metrics
-[article](https://towardsdatascience.com/building-confidence-on-explainability-
+[Article](https://towardsdatascience.com/building-confidence-on-explainability-
 methods-66b9ee575514) | To help increase confidence in explainability methods,
 you can evaluate the relevance of your explainability using 3 metrics:
 **Stability**, **Consistency** and **Compacity** | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-
 metrics.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
 explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb)
 | 1.5.x | ACV Backend
 | A new way of estimating Shapley values using ACV. [More info about ACV here]
 (https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-
 cfea30509254). | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
 _static/wheel.png]](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb) |
 | 1.4.x | Groups of features
-[demo](https://shapash-demo2.ossbymaif.fr/) | You can now regroup features that
+[Demo](https://shapash-demo2.ossbymaif.fr/) | You can now regroup features that
 share common properties together.
 This option can be useful if your model has a lot of features. | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
 groups_features.gif]](https://github.com/MAIF/shapash/blob/master/tutorial/
 common/tuto-common01-groups_of_features.ipynb) | | 1.3.x | Shapash Report
-[demo](https://shapash.readthedocs.io/en/latest/report.html) | A standalone
+[Demo](https://shapash.readthedocs.io/en/latest/report.html) | A standalone
 HTML report that constitutes a basis of an audit document. | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png]]
 (https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-
 report01.ipynb) | ## ð Overview **Shapash** is a Python library which aims
 to make machine learning interpretable and understandable by everyone. It
 provides several types of visualization that display explicit labels that
 everyone can understand. Data Scientists can understand their models easily and
@@ -73,15 +78,18 @@
 models-understandable-by-everyone-8f96ad469eb3) - [Model auditability - Towards
 DS](https://towardsdatascience.com/shapash-1-3-2-announcing-new-features-for-
 more-auditable-ai-64a6db71c919) - [Group of features - Towards AI](https://
 pub.towardsai.net/machine-learning-6011d5d9a444) - [Building confidence on
 explainability - Towards DS](https://towardsdatascience.com/building-
 confidence-on-explainability-methods-66b9ee575514) - [Picking Examples to
 Understand Machine Learning Model](https://www.kdnuggets.com/2022/11/picking-
-examples-understand-machine-learning-model.html)
+examples-understand-machine-learning-model.html) - [Enhancing Webapp Built-In
+Features for Comprehensive Machine Learning Model Interpretation](https://
+pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-
+40b50157c2fb)
      [https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
                               shapash_global.gif]
 ## ð¤ Contributors
 [https://github.com/MAIF/shapash/blob/master/docs/_static/logo_maif.png]
 [https://github.com/MAIF/shapash/blob/master/docs/_static/logo_quantmetry.png]
 [https://github.com/MAIF/shapash/blob/master/docs/_static/
 logo_societe_generale.png] [https://github.com/MAIF/shapash/blob/master/docs/
@@ -214,8 +222,10 @@
 tuto-expl03-Shapash-acv-backend.ipynb) - [Compile faster Lime and consistency
 of contributions](tutorial/explainer/tuto-expl04-Shapash-compute-Lime-
 faster.ipynb)  Evaluating the quality of your explainability  - [Building
 confidence on explainability methods using **Stability**, **Consistency** and
 **Compacity** metrics](tutorial/explainability_quality/tuto-quality01-Builing-
 confidence-explainability.ipynb)  Generate a report of your project  -
 [Generate a standalone HTML report of your project with generate_report]
-(tutorial/report/tuto-shapash-report01.ipynb)
+(tutorial/report/tuto-shapash-report01.ipynb)  Analysing your model via Shapash
+WebApp  - [Add features outside of the model for more exploration options]
+(tutorial/webapp/tuto-webapp01-additional-data.ipynb)
```

### Comparing `shapash-2.3.0/setup.py` & `shapash-2.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     exec(f.read(), version_d)
 
 
 requirements = [
     'plotly>=5.0.0',
     'matplotlib>=3.2.0',
     'numpy>1.18.0',
-    'pandas>1.0.2',
+    'pandas>1.0.2,<2.0.0',
     'shap>=0.38.1',
     'dash>=2.3.1',
     'dash-bootstrap-components>=1.1.0',
     'dash-core-components>=2.0.0',
     'dash-daq>=0.5.0',
     'dash-html-components>=2.0.0',
     'dash-renderer==1.8.3',
@@ -39,15 +39,15 @@
 extras = dict()
 
 # This list should be identical to the list in shapash/report/__init__.py
 extras['report'] = [
     'nbconvert==6.0.7',
     'papermill>=2.0.0',
     'jupyter-client<8.0.0',
-    'seaborn<=0.11.2',
+    'seaborn>=0.12.2',
     'notebook',
     'Jinja2>=2.11.0',
     'phik'
 ]
 
 extras['xgboost'] = ['xgboost>=1.0.0']
 extras['lightgbm'] = ['lightgbm>=2.3.0']
@@ -94,18 +94,14 @@
         'shapash.webapp.utils': 'shapash/webapp/utils',
         'shapash.style': 'shapash/style',
     },
     packages=['shapash', 'shapash.data', 'shapash.decomposition',
               'shapash.explainer', 'shapash.backend', 'shapash.manipulation',
               'shapash.utils', 'shapash.webapp', 'shapash.webapp.utils',
               'shapash.report', 'shapash.style'],
-    data_files=[('data', ['shapash/data/house_prices_dataset.csv']),
-                ('data', ['shapash/data/house_prices_labels.json']),
-                ('data', ['shapash/data/titanicdata.csv']),
-                ('data', ['shapash/data/titaniclabels.json']),
-                ('style', ['shapash/style/colors.json'])],
+    data_files=[('style', ['shapash/style/colors.json'])],
     include_package_data=True,
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     zip_safe=False,
 )
```

### Comparing `shapash-2.3.0/shapash/backend/__init__.py` & `shapash-2.3.2/shapash/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/backend/acv_backend.py` & `shapash-2.3.2/shapash/backend/acv_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/backend/base_backend.py` & `shapash-2.3.2/shapash/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/backend/lime_backend.py` & `shapash-2.3.2/shapash/backend/lime_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/backend/shap_backend.py` & `shapash-2.3.2/shapash/backend/shap_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/decomposition/contributions.py` & `shapash-2.3.2/shapash/decomposition/contributions.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/explainer/consistency.py` & `shapash-2.3.2/shapash/explainer/consistency.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,15 +543,15 @@
 
         # Remove constant columns
         const_cols = x.loc[:, x.apply(pd.Series.nunique) == 1]
         x = x.drop(const_cols, axis=1)
         weights = [weight.drop(const_cols, axis=1) for weight in weights]
 
         # Only keep features based on largest mean of absolute values
-        mean_contributions = np.mean(np.abs(pd.concat(weights)))
+        mean_contributions = np.mean(np.abs(pd.concat(weights)), axis=0)
         top_features = np.flip(mean_contributions.sort_values(ascending=False)[:max_features].keys())
 
         fig = self.plot_pairwise_consistency(weights, x, top_features, methods, file_name, auto_open)
 
         return fig
 
     def plot_pairwise_consistency(self, weights, x, top_features, methods, file_name, auto_open):
```

### Comparing `shapash-2.3.0/shapash/explainer/multi_decorator.py` & `shapash-2.3.2/shapash/explainer/multi_decorator.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/explainer/smart_explainer.py` & `shapash-2.3.2/shapash/explainer/smart_explainer.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/explainer/smart_plotter.py` & `shapash-2.3.2/shapash/explainer/smart_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -3190,16 +3190,17 @@
         if prediction_error is not None:
             if (self.explainer.y_target == 0).any()[0]:
                 subtitle = "Prediction Error = abs(True Values - Predicted Values)"
             else:
                 subtitle = "Prediction Error = abs(True Values - Predicted Values) / True Values"
             df_equal_bins = prediction_error.describe(percentiles=np.arange(0.1, 1, 0.1).tolist())
             equal_bins = df_equal_bins.loc[~df_equal_bins.index.isin(['count', 'mean', 'std'])].values
+            equal_bins = np.unique(equal_bins)
             self.pred_colorscale = self.tuning_colorscale(pd.DataFrame(pd.cut([val[0] for val in prediction_error.values],
-            bins=[i[0] for i in equal_bins], labels=False)))
+            bins=[i for i in equal_bins], labels=False)))
             col_scale = self.pred_colorscale
 
             y_pred = self.explainer.y_pred.loc[list_ind]
             y_target = self.explainer.y_target.loc[list_ind]
             prediction_error = np.array(prediction_error.loc[list_ind])
             # round predict
             if self.round_digit is None:
@@ -3214,21 +3215,21 @@
                 y=y_pred.values.flatten(),
                 mode='markers',
                 hovertext=hv_text,
                 hovertemplate='<b>%{hovertext}</b><br />',
                 customdata=y_pred.index.values
             )
 
-            colorpoints = pd.cut([val[0] for val in prediction_error], bins=[i[0] for i in equal_bins], labels=False)/10
+            colorpoints = pd.cut([val[0] for val in prediction_error], bins=[i for i in equal_bins], labels=False)/10
             colorbar_title = 'Prediction Error'
             fig.data[-1].marker.color = colorpoints.flatten()
             fig.data[-1].marker.coloraxis = 'coloraxis'
             fig.layout.coloraxis.colorscale = col_scale
             fig.layout.coloraxis.colorbar = {'title': {'text': colorbar_title}, "tickvals": [col_scale[0][0], col_scale[-1][0]-0.15],
-            "ticktext":[float('{:0.3f}'.format(equal_bins[0][0])), float('{:0.3f}'.format(equal_bins[-2][0]))], "tickformat": ".2s",
+            "ticktext":[float('{:0.3f}'.format(equal_bins[0])), float('{:0.3f}'.format(equal_bins[-2]))], "tickformat": ".2s",
             "yanchor": "top", "y": 1.1}
             range_axis = [min(min(y_target.values.flatten()), min(y_pred.values.flatten())), max(max(y_target.values.flatten()),
             max(y_pred.values.flatten()))]
             fig.update_xaxes(range=range_axis)
             fig.update_yaxes(range=range_axis)
             fig.update_layout(shapes=[{'type': 'line', 'yref': 'y domain', 'xref': 'x domain', 'y0': 0, 'y1': 1,
             'x0': 0, 'x1': 1, 'line': dict(color="grey", width=1, dash="dot")}])
```

### Comparing `shapash-2.3.0/shapash/explainer/smart_predictor.py` & `shapash-2.3.2/shapash/explainer/smart_predictor.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/explainer/smart_state.py` & `shapash-2.3.2/shapash/explainer/smart_state.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/manipulation/filters.py` & `shapash-2.3.2/shapash/manipulation/filters.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/manipulation/mask.py` & `shapash-2.3.2/shapash/manipulation/mask.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/manipulation/select_lines.py` & `shapash-2.3.2/shapash/manipulation/select_lines.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/manipulation/summarize.py` & `shapash-2.3.2/shapash/manipulation/summarize.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/report/__init__.py` & `shapash-2.3.2/shapash/report/__init__.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/report/base_report.ipynb` & `shapash-2.3.2/shapash/report/base_report.ipynb`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/report/common.py` & `shapash-2.3.2/shapash/report/common.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/report/data_analysis.py` & `shapash-2.3.2/shapash/report/data_analysis.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/report/generation.py` & `shapash-2.3.2/shapash/report/generation.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/report/html/dropdown.html` & `shapash-2.3.2/shapash/report/html/dropdown.html`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/report/html/explainability.html` & `shapash-2.3.2/shapash/report/html/explainability.html`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/report/html/univariate.html` & `shapash-2.3.2/shapash/report/html/univariate.html`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/report/plots.py` & `shapash-2.3.2/shapash/report/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     the number of categories is less than nb_cat_max.
     """
     df_cat_sum_hue = df_cat.groupby([col]).agg({'count': 'sum'}).reset_index()
     list_cat_to_merge = df_cat_sum_hue.sort_values('count', ascending=False)[col].to_list()[nb_cat_max - 1:]
     df_cat_other = df_cat.loc[df_cat[col].isin(list_cat_to_merge)] \
         .groupby(hue, as_index=False)[["count", "Percent"]].sum()
     df_cat_other[col] = "Other"
-    return df_cat.loc[~df_cat[col].isin(list_cat_to_merge)].append(df_cat_other)
+    return pd.concat([df_cat.loc[~df_cat[col].isin(list_cat_to_merge)],df_cat_other], axis=0)
 
 
 def generate_confusion_matrix_plot(
         y_true: Union[np.array, list],
         y_pred: Union[np.array, list],
         colors_dict: Optional[dict] = None
 ) -> plt.Figure:
```

### Comparing `shapash-2.3.0/shapash/report/project_report.py` & `shapash-2.3.2/shapash/report/project_report.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/report/template/custom/index.html.j2` & `shapash-2.3.2/shapash/report/template/custom/index.html.j2`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/report/visualisation.py` & `shapash-2.3.2/shapash/report/visualisation.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/style/colors.json` & `shapash-2.3.2/shapash/style/colors.json`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/style/style_utils.py` & `shapash-2.3.2/shapash/style/style_utils.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/utils/category_encoder_backend.py` & `shapash-2.3.2/shapash/utils/category_encoder_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/utils/check.py` & `shapash-2.3.2/shapash/utils/check.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/utils/columntransformer_backend.py` & `shapash-2.3.2/shapash/utils/columntransformer_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/utils/explanation_metrics.py` & `shapash-2.3.2/shapash/utils/explanation_metrics.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/utils/io.py` & `shapash-2.3.2/shapash/utils/io.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/utils/load_smartpredictor.py` & `shapash-2.3.2/shapash/utils/load_smartpredictor.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/utils/model.py` & `shapash-2.3.2/shapash/utils/model.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/utils/model_synoptic.py` & `shapash-2.3.2/shapash/utils/model_synoptic.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/utils/threading.py` & `shapash-2.3.2/shapash/utils/threading.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/utils/transform.py` & `shapash-2.3.2/shapash/utils/transform.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/utils/utils.py` & `shapash-2.3.2/shapash/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/webapp/assets/favicon.ico` & `shapash-2.3.2/shapash/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/webapp/assets/jquery.js` & `shapash-2.3.2/shapash/webapp/assets/jquery.js`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/webapp/assets/material-icons.css` & `shapash-2.3.2/shapash/webapp/assets/material-icons.css`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/webapp/assets/reload.png` & `shapash-2.3.2/shapash/webapp/assets/reload.png`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/webapp/assets/settings.png` & `shapash-2.3.2/shapash/webapp/assets/settings.png`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/webapp/assets/shapash-fond-fonce.png` & `shapash-2.3.2/shapash/webapp/assets/shapash-fond-fonce.png`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/webapp/assets/style.css` & `shapash-2.3.2/shapash/webapp/assets/style.css`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/webapp/smart_app.py` & `shapash-2.3.2/shapash/webapp/smart_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
         self.components['table']['dataset'] = dash_table.DataTable(
             id='dataset',
             data=self.round_dataframe.to_dict('records'),
             tooltip_data=[
                 {
                     column: {'value': str(value), 'type': 'text'}
                     for column, value in row.items()
-                } for row in self.dataframe.to_dict('rows')
+                } for row in self.dataframe.to_dict('index').values()
             ], tooltip_duration=2000,
 
             columns=[{"name": i, "id": i} for i in self.dataframe.columns],
             tooltip_header={
                 column: self.features_dict[column] for column in self.dataframe.columns
                 if column not in self.special_cols
             },
```

### Comparing `shapash-2.3.0/shapash/webapp/utils/MyGraph.py` & `shapash-2.3.2/shapash/webapp/utils/MyGraph.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/webapp/utils/explanations.py` & `shapash-2.3.2/shapash/webapp/utils/explanations.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/webapp/utils/utils.py` & `shapash-2.3.2/shapash/webapp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/webapp/webapp_launch.py` & `shapash-2.3.2/shapash/webapp/webapp_launch.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash/webapp/webapp_launch_DVF.py` & `shapash-2.3.2/shapash/webapp/webapp_launch_DVF.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.0/shapash.egg-info/PKG-INFO` & `shapash-2.3.2/shapash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapash
-Version: 2.3.0
+Version: 2.3.2
 Summary: Shapash is a Python library which aims to make machine learning interpretable and understandable by everyone.
 Home-page: https://github.com/MAIF/shapash
 Author: Yann Golhen, Sebastien Bidault, Yann Lagre, Maxime Gendre
 Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0
 Keywords: shapash
 Classifier: Programming Language :: Python :: 3
@@ -56,24 +56,24 @@
 </p>
 
 ## 🎉 What's new ?
 
 
 | Version       | New Feature                                                                           | Description                                                                                                                            | Tutorial |
 |:-------------:|:-------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
-| 2.3.x         |  Additional dataset columns <br> (Demo coming soon)                                                                | In Webapp: Target and error columns added to dataset and possibility to add features outside the model for more filtering options            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/add_column_icon.png" width="50" title="add_column">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
-| 2.3.x         |  Identity card <br> (Demo coming soon)                                                                  | In Webapp: New identity card to summarize the information of the selected sample                  |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/identity_card.png" width="50" title="identity">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
-| 2.2.x         |  Picking samples <br> [New demo](https://shapash-demo.ossbymaif.fr/)                                                                | New tab in the webapp for picking samples. The graph represents the "True Values Vs Predicted Values"            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png" width="50" title="picking">](https://github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-prediction_plot.ipynb)
-| 2.2.x         |  Dataset Filter <br> [New demo](https://shapash-demo.ossbymaif.fr/)                                                                  | New tab in the webapp to filter data. And several improvements in the webapp: subtitles, labels, screen adjustments                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/webapp.png" width="50" title="webapp">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
+| 2.3.x         |  Additional dataset columns <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                | In Webapp: Target and error columns added to dataset and possibility to add features outside the model for more filtering options            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/add_column_icon.png" width="50" title="add_column">](https://github.com/MAIF/shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+| 2.3.x         |  Identity card <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                  | In Webapp: New identity card to summarize the information of the selected sample                  |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/identity_card.png" width="50" title="identity">](https://github.com/MAIF/shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+| 2.2.x         |  Picking samples <br> [Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-machine-learning-model.html)                                                                | New tab in the webapp for picking samples. The graph represents the "True Values Vs Predicted Values"            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png" width="50" title="picking">](https://github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-prediction_plot.ipynb)
+| 2.2.x         |  Dataset Filter <br>                                                              | New tab in the webapp to filter data. And several improvements in the webapp: subtitles, labels, screen adjustments                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/webapp.png" width="50" title="webapp">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
 | 2.0.x         |  Refactoring Shapash <br>                                                                   | Refactoring attributes of compile methods and init. Refactoring implementation for new backends                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/modular.png" width="50" title="modular">](https://github.com/MAIF/shapash/blob/master/tutorial/backend/tuto-backend-01.ipynb)
 | 1.7.x         |  Variabilize Colors <br>                                                                   | Giving possibility to have your own colour palette for outputs adapted to your design                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/variabilize-colors.png" width="50" title="variabilize-colors">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common02-colors.ipynb)
-| 1.6.x         |  Explainability Quality Metrics <br> [article](https://towardsdatascience.com/building-confidence-on-explainability-methods-66b9ee575514)                                                                   | To help increase confidence in explainability methods, you can evaluate the relevance of your explainability using 3 metrics: **Stability**, **Consistency** and **Compacity**                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-metrics.png" width="50" title="quality-metrics">](https://github.com/MAIF/shapash/blob/master/tutorial/explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb) 
+| 1.6.x         |  Explainability Quality Metrics <br> [Article](https://towardsdatascience.com/building-confidence-on-explainability-methods-66b9ee575514)                                                                   | To help increase confidence in explainability methods, you can evaluate the relevance of your explainability using 3 metrics: **Stability**, **Consistency** and **Compacity**                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-metrics.png" width="50" title="quality-metrics">](https://github.com/MAIF/shapash/blob/master/tutorial/explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb) 
 | 1.5.x         |  ACV Backend <br>                                                                     | A new way of estimating Shapley values using ACV. [More info about ACV here](https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-cfea30509254).                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/wheel.png" width="50" title="wheel-acv-backend">](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb)    |
-| 1.4.x         |  Groups of features <br> [demo](https://shapash-demo2.ossbymaif.fr/)                  | You can now regroup features that share common properties together. <br>This option can be useful if your model has a lot of features. |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/groups_features.gif" width="120" title="groups-features">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common01-groups_of_features.ipynb)    | 
-| 1.3.x         |  Shapash Report <br> [demo](https://shapash.readthedocs.io/en/latest/report.html)     | A standalone HTML report that constitutes a basis of an audit document.                                                                |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png" width="50" title="shapash-report">](https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-report01.ipynb)    | 
+| 1.4.x         |  Groups of features <br> [Demo](https://shapash-demo2.ossbymaif.fr/)                  | You can now regroup features that share common properties together. <br>This option can be useful if your model has a lot of features. |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/groups_features.gif" width="120" title="groups-features">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common01-groups_of_features.ipynb)    | 
+| 1.3.x         |  Shapash Report <br> [Demo](https://shapash.readthedocs.io/en/latest/report.html)     | A standalone HTML report that constitutes a basis of an audit document.                                                                |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png" width="50" title="shapash-report">](https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-report01.ipynb)    | 
 
 
 ## 🔍 Overview
 
 **Shapash** is a Python library which aims to make machine learning interpretable and understandable by everyone.
 It provides several types of visualization that display explicit labels that everyone can understand. 
 
@@ -85,14 +85,15 @@
 - [Presentation video for french speakers](https://www.youtube.com/watch?v=r1R_A9B9apk)
 - Medium:
   - [Understand your model with Shapash - Towards AI](https://pub.towardsai.net/shapash-making-ml-models-understandable-by-everyone-8f96ad469eb3) 
   - [Model auditability - Towards DS](https://towardsdatascience.com/shapash-1-3-2-announcing-new-features-for-more-auditable-ai-64a6db71c919)
   - [Group of features - Towards AI](https://pub.towardsai.net/machine-learning-6011d5d9a444)
   - [Building confidence on explainability - Towards DS](https://towardsdatascience.com/building-confidence-on-explainability-methods-66b9ee575514)
   - [Picking Examples to Understand Machine Learning Model](https://www.kdnuggets.com/2022/11/picking-examples-understand-machine-learning-model.html)
+  - [Enhancing Webapp Built-In Features for Comprehensive Machine Learning Model Interpretation](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)
 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/shapash_global.gif" width="800">
 </p>
 
 ## 🤝 Contributors
@@ -323,8 +324,12 @@
 
 <details><summary><b>Generate a report of your project</b> </summary>
 
 - [Generate a standalone HTML report of your project with generate_report](tutorial/report/tuto-shapash-report01.ipynb)
 
 </details>
 
+<details><summary><b>Analysing your model via Shapash WebApp</b> </summary>
 
+- [Add features outside of the model for more exploration options](tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+
+</details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shapash Version: 2.3.0 Summary: Shapash is a Python
+Metadata-Version: 2.1 Name: shapash Version: 2.3.2 Summary: Shapash is a Python
 library which aims to make machine learning interpretable and understandable by
 everyone. Home-page: https://github.com/MAIF/shapash Author: Yann Golhen,
 Sebastien Bidault, Yann Lagre, Maxime Gendre Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0 Keywords: shapash Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
@@ -14,63 +14,68 @@
                                   resize.png]
           [tests]  [pypi]  [downloads]  [pyversion]  [license]  [doc]
 ## ð What's new ? | Version | New Feature | Description | Tutorial | |:-----
 --------:|:--------------------------------------------------------------------
 -----------------:|:-----------------------------------------------------------
 ---------------------------------------------------------------------------:|:-
 -------:| | 2.3.x | Additional dataset columns
-(Demo coming soon) | In Webapp: Target and error columns added to dataset and
-possibility to add features outside the model for more filtering options | [
-[https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
+[New demo](https://shapash-demo.ossbymaif.fr/)
+[Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-
+interpretation-40b50157c2fb) | In Webapp: Target and error columns added to
+dataset and possibility to add features outside the model for more filtering
+options | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
 add_column_icon.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
-tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.3.x | Identity card
-(Demo coming soon) | In Webapp: New identity card to summarize the information
-of the selected sample | [[https://raw.githubusercontent.com/MAIF/shapash/
-master/docs/_static/identity_card.png]](https://github.com/MAIF/shapash/blob/
-master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.2.x |
-Picking samples
-[New demo](https://shapash-demo.ossbymaif.fr/) | New tab in the webapp for
-picking samples. The graph represents the "True Values Vs Predicted Values" | [
-[https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
-picking.png]](https://github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-
-plot06-prediction_plot.ipynb) | 2.2.x | Dataset Filter
-[New demo](https://shapash-demo.ossbymaif.fr/) | New tab in the webapp to
-filter data. And several improvements in the webapp: subtitles, labels, screen
-adjustments | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
-_static/webapp.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
-tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.0.x | Refactoring Shapash
+webapp/tuto-webapp01-additional-data.ipynb) | 2.3.x | Identity card
+[New demo](https://shapash-demo.ossbymaif.fr/)
+[Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-
+interpretation-40b50157c2fb) | In Webapp: New identity card to summarize the
+information of the selected sample | [[https://raw.githubusercontent.com/MAIF/
+shapash/master/docs/_static/identity_card.png]](https://github.com/MAIF/
+shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb) |
+2.2.x | Picking samples
+[Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-
+machine-learning-model.html) | New tab in the webapp for picking samples. The
+graph represents the "True Values Vs Predicted Values" | [[https://
+raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png]](https:
+//github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-
+prediction_plot.ipynb) | 2.2.x | Dataset Filter
+| New tab in the webapp to filter data. And several improvements in the webapp:
+subtitles, labels, screen adjustments | [[https://raw.githubusercontent.com/
+MAIF/shapash/master/docs/_static/webapp.png]](https://github.com/MAIF/shapash/
+blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.0.x |
+Refactoring Shapash
 | Refactoring attributes of compile methods and init. Refactoring
 implementation for new backends | [[https://raw.githubusercontent.com/MAIF/
 shapash/master/docs/_static/modular.png]](https://github.com/MAIF/shapash/blob/
 master/tutorial/backend/tuto-backend-01.ipynb) | 1.7.x | Variabilize Colors
 | Giving possibility to have your own colour palette for outputs adapted to
 your design | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
 _static/variabilize-colors.png]](https://github.com/MAIF/shapash/blob/master/
 tutorial/common/tuto-common02-colors.ipynb) | 1.6.x | Explainability Quality
 Metrics
-[article](https://towardsdatascience.com/building-confidence-on-explainability-
+[Article](https://towardsdatascience.com/building-confidence-on-explainability-
 methods-66b9ee575514) | To help increase confidence in explainability methods,
 you can evaluate the relevance of your explainability using 3 metrics:
 **Stability**, **Consistency** and **Compacity** | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-
 metrics.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
 explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb)
 | 1.5.x | ACV Backend
 | A new way of estimating Shapley values using ACV. [More info about ACV here]
 (https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-
 cfea30509254). | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
 _static/wheel.png]](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb) |
 | 1.4.x | Groups of features
-[demo](https://shapash-demo2.ossbymaif.fr/) | You can now regroup features that
+[Demo](https://shapash-demo2.ossbymaif.fr/) | You can now regroup features that
 share common properties together.
 This option can be useful if your model has a lot of features. | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
 groups_features.gif]](https://github.com/MAIF/shapash/blob/master/tutorial/
 common/tuto-common01-groups_of_features.ipynb) | | 1.3.x | Shapash Report
-[demo](https://shapash.readthedocs.io/en/latest/report.html) | A standalone
+[Demo](https://shapash.readthedocs.io/en/latest/report.html) | A standalone
 HTML report that constitutes a basis of an audit document. | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png]]
 (https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-
 report01.ipynb) | ## ð Overview **Shapash** is a Python library which aims
 to make machine learning interpretable and understandable by everyone. It
 provides several types of visualization that display explicit labels that
 everyone can understand. Data Scientists can understand their models easily and
@@ -85,15 +90,18 @@
 models-understandable-by-everyone-8f96ad469eb3) - [Model auditability - Towards
 DS](https://towardsdatascience.com/shapash-1-3-2-announcing-new-features-for-
 more-auditable-ai-64a6db71c919) - [Group of features - Towards AI](https://
 pub.towardsai.net/machine-learning-6011d5d9a444) - [Building confidence on
 explainability - Towards DS](https://towardsdatascience.com/building-
 confidence-on-explainability-methods-66b9ee575514) - [Picking Examples to
 Understand Machine Learning Model](https://www.kdnuggets.com/2022/11/picking-
-examples-understand-machine-learning-model.html)
+examples-understand-machine-learning-model.html) - [Enhancing Webapp Built-In
+Features for Comprehensive Machine Learning Model Interpretation](https://
+pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-
+40b50157c2fb)
      [https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
                               shapash_global.gif]
 ## ð¤ Contributors
 [https://github.com/MAIF/shapash/blob/master/docs/_static/logo_maif.png]
 [https://github.com/MAIF/shapash/blob/master/docs/_static/logo_quantmetry.png]
 [https://github.com/MAIF/shapash/blob/master/docs/_static/
 logo_societe_generale.png] [https://github.com/MAIF/shapash/blob/master/docs/
@@ -226,8 +234,10 @@
 tuto-expl03-Shapash-acv-backend.ipynb) - [Compile faster Lime and consistency
 of contributions](tutorial/explainer/tuto-expl04-Shapash-compute-Lime-
 faster.ipynb)  Evaluating the quality of your explainability  - [Building
 confidence on explainability methods using **Stability**, **Consistency** and
 **Compacity** metrics](tutorial/explainability_quality/tuto-quality01-Builing-
 confidence-explainability.ipynb)  Generate a report of your project  -
 [Generate a standalone HTML report of your project with generate_report]
-(tutorial/report/tuto-shapash-report01.ipynb)
+(tutorial/report/tuto-shapash-report01.ipynb)  Analysing your model via Shapash
+WebApp  - [Add features outside of the model for more exploration options]
+(tutorial/webapp/tuto-webapp01-additional-data.ipynb)
```

### Comparing `shapash-2.3.0/shapash.egg-info/SOURCES.txt` & `shapash-2.3.2/shapash.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -14,18 +14,14 @@
 shapash/backend/__init__.py
 shapash/backend/acv_backend.py
 shapash/backend/base_backend.py
 shapash/backend/lime_backend.py
 shapash/backend/shap_backend.py
 shapash/data/__init__.py
 shapash/data/data_loader.py
-shapash/data/house_prices_dataset.csv
-shapash/data/house_prices_labels.json
-shapash/data/titanicdata.csv
-shapash/data/titaniclabels.json
 shapash/decomposition/__init__.py
 shapash/decomposition/contributions.py
 shapash/explainer/__init__.py
 shapash/explainer/consistency.py
 shapash/explainer/multi_decorator.py
 shapash/explainer/smart_explainer.py
 shapash/explainer/smart_plotter.py
```

### Comparing `shapash-2.3.0/shapash.egg-info/requires.txt` & `shapash-2.3.2/shapash.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 plotly>=5.0.0
 matplotlib>=3.2.0
 numpy>1.18.0
-pandas>1.0.2
+pandas<2.0.0,>1.0.2
 shap>=0.38.1
 dash>=2.3.1
 dash-bootstrap-components>=1.1.0
 dash-core-components>=2.0.0
 dash-daq>=0.5.0
 dash-html-components>=2.0.0
 dash-renderer==1.8.3
@@ -28,14 +28,14 @@
 [lime]
 lime>=0.2.0.0
 
 [report]
 nbconvert==6.0.7
 papermill>=2.0.0
 jupyter-client<8.0.0
-seaborn<=0.11.2
+seaborn>=0.12.2
 notebook
 Jinja2>=2.11.0
 phik
 
 [xgboost]
 xgboost>=1.0.0
```

