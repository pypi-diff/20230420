# Comparing `tmp/datasette-dashboards-0.4.0.tar.gz` & `tmp/datasette_dashboards-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-dashboards-0.4.0.tar", last modified: Thu Mar 30 12:37:45 2023, max compression
+gzip compressed data, was "datasette_dashboards-0.5.0.tar", max compression
```

## Comparing `datasette-dashboards-0.4.0.tar` & `datasette_dashboards-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:37:45.666081 datasette-dashboards-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-30 12:37:33.000000 datasette-dashboards-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12033 2023-03-30 12:37:45.666081 datasette-dashboards-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-03-30 12:37:33.000000 datasette-dashboards-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:37:45.662081 datasette-dashboards-0.4.0/datasette_dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-03-30 12:37:33.000000 datasette-dashboards-0.4.0/datasette_dashboards/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:37:45.666081 datasette-dashboards-0.4.0/datasette_dashboards/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-03-30 12:37:33.000000 datasette-dashboards-0.4.0/datasette_dashboards/static/dashboards.css
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-03-30 12:37:33.000000 datasette-dashboards-0.4.0/datasette_dashboards/static/dashboards.js
--rw-r--r--   0 runner    (1001) docker     (123)    64383 2023-03-30 12:37:33.000000 datasette-dashboards-0.4.0/datasette_dashboards/static/vega-embed.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   244624 2023-03-30 12:37:33.000000 datasette-dashboards-0.4.0/datasette_dashboards/static/vega-lite.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   510672 2023-03-30 12:37:33.000000 datasette-dashboards-0.4.0/datasette_dashboards/static/vega.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:37:45.666081 datasette-dashboards-0.4.0/datasette_dashboards/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-03-30 12:37:33.000000 datasette-dashboards-0.4.0/datasette_dashboards/templates/dashboard_chart.html
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-30 12:37:33.000000 datasette-dashboards-0.4.0/datasette_dashboards/templates/dashboard_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-03-30 12:37:33.000000 datasette-dashboards-0.4.0/datasette_dashboards/templates/dashboard_view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:37:45.662081 datasette-dashboards-0.4.0/datasette_dashboards.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12033 2023-03-30 12:37:45.000000 datasette-dashboards-0.4.0/datasette_dashboards.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-30 12:37:45.000000 datasette-dashboards-0.4.0/datasette_dashboards.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 12:37:45.000000 datasette-dashboards-0.4.0/datasette_dashboards.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-30 12:37:45.000000 datasette-dashboards-0.4.0/datasette_dashboards.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-30 12:37:45.000000 datasette-dashboards-0.4.0/datasette_dashboards.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-30 12:37:45.000000 datasette-dashboards-0.4.0/datasette_dashboards.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 12:37:45.666081 datasette-dashboards-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-30 12:37:33.000000 datasette-dashboards-0.4.0/setup.py
+-rw-r--r--   0        0        0    11357 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/LICENSE
+-rw-r--r--   0        0        0    11575 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/README.md
+-rw-r--r--   0        0        0     7837 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/datasette_dashboards/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/datasette_dashboards/py.typed
+-rw-r--r--   0        0        0     1358 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/datasette_dashboards/static/dashboards.css
+-rw-r--r--   0        0        0     6417 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/datasette_dashboards/static/dashboards.js
+-rw-r--r--   0        0        0    64383 2023-04-20 16:51:57.819826 datasette_dashboards-0.5.0/datasette_dashboards/static/vega-embed.min.js
+-rw-r--r--   0        0        0   244624 2023-04-20 16:51:57.823827 datasette_dashboards-0.5.0/datasette_dashboards/static/vega-lite.min.js
+-rw-r--r--   0        0        0   510672 2023-04-20 16:51:57.823827 datasette_dashboards-0.5.0/datasette_dashboards/static/vega.min.js
+-rw-r--r--   0        0        0     2270 2023-04-20 16:51:57.823827 datasette_dashboards-0.5.0/datasette_dashboards/templates/dashboard_chart.html
+-rw-r--r--   0        0        0      617 2023-04-20 16:51:57.823827 datasette_dashboards-0.5.0/datasette_dashboards/templates/dashboard_list.html
+-rw-r--r--   0        0        0     4925 2023-04-20 16:51:57.823827 datasette_dashboards-0.5.0/datasette_dashboards/templates/dashboard_view.html
+-rw-r--r--   0        0        0     1427 2023-04-20 16:51:57.835827 datasette_dashboards-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    12419 1970-01-01 00:00:00.000000 datasette_dashboards-0.5.0/PKG-INFO
```

### Comparing `datasette-dashboards-0.4.0/LICENSE` & `datasette_dashboards-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-dashboards-0.4.0/PKG-INFO` & `datasette_dashboards-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: datasette-dashboards
-Version: 0.4.0
-Summary: Datasette plugin providing data dashboards from metadata
-Home-page: https://github.com/rclement/datasette-dashboards
-Author: Romain Clement
-License: Apache License, Version 2.0
-Project-URL: Changelog, https://github.com/rclement/datasette-dashboards/blob/master/CHANGELOG.md
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # datasette-dashboards
 
 > Datasette plugin providing data dashboards from metadata
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-dashboards.svg)](https://pypi.org/project/datasette-dashboards/)
 [![CI/CD](https://github.com/rclement/datasette-dashboards/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/rclement/datasette-dashboards/actions/workflows/ci-cd.yml)
 [![Coverage Status](https://img.shields.io/codecov/c/github/rclement/datasette-dashboards)](https://codecov.io/gh/rclement/datasette-dashboards)
@@ -280,16 +267,16 @@
 
 ## Development
 
 To set up this plugin locally, first checkout the code.
 Then create a new virtual environment and the required dependencies:
 
 ```bash
-pipenv install -d
-pipenv shell
+poetry install
+poetry shell
 ```
 
 To run the tests:
 
 ```bash
 pytest
 ```
```

### Comparing `datasette-dashboards-0.4.0/README.md` & `datasette_dashboards-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: datasette-dashboards
+Version: 0.5.0
+Summary: Datasette plugin providing data dashboards from metadata
+Home-page: https://github.com/rclement/datasette-dashboards
+License: Apache License, Version 2.0
+Author: Romain Clement
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: datasette
+Requires-Dist: datasette-leaflet
+Requires-Dist: datasette-render-markdown
+Project-URL: Changelog, https://github.com/rclement/datasette-dashboards/blob/master/CHANGELOG.md
+Project-URL: Repository, https://github.com/rclement/datasette-dashboards
+Description-Content-Type: text/markdown
+
 # datasette-dashboards
 
 > Datasette plugin providing data dashboards from metadata
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-dashboards.svg)](https://pypi.org/project/datasette-dashboards/)
 [![CI/CD](https://github.com/rclement/datasette-dashboards/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/rclement/datasette-dashboards/actions/workflows/ci-cd.yml)
 [![Coverage Status](https://img.shields.io/codecov/c/github/rclement/datasette-dashboards)](https://codecov.io/gh/rclement/datasette-dashboards)
@@ -267,16 +287,16 @@
 
 ## Development
 
 To set up this plugin locally, first checkout the code.
 Then create a new virtual environment and the required dependencies:
 
 ```bash
-pipenv install -d
-pipenv shell
+poetry install
+poetry shell
 ```
 
 To run the tests:
 
 ```bash
 pytest
 ```
@@ -293,7 +313,8 @@
 ```
 
 ## License
 
 Licensed under Apache License, Version 2.0
 
 Copyright (c) 2021 - present Romain Clement
+
```

### Comparing `datasette-dashboards-0.4.0/datasette_dashboards/__init__.py` & `datasette_dashboards-0.5.0/datasette_dashboards/__init__.py`

 * *Files identical despite different names*

### Comparing `datasette-dashboards-0.4.0/datasette_dashboards/static/dashboards.css` & `datasette_dashboards-0.5.0/datasette_dashboards/static/dashboards.css`

 * *Files identical despite different names*

### Comparing `datasette-dashboards-0.4.0/datasette_dashboards/static/dashboards.js` & `datasette_dashboards-0.5.0/datasette_dashboards/static/dashboards.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -207,8 +207,10 @@
 }
 
 function autorefresh(minutes) {
     const timeout = Math.round(minutes * 60 * 1000)
     window.setTimeout(function() {
         window.location.reload()
     }, timeout)
-}
+}
+
+vega.setRandom(vega.randomLCG(0))
```

### Comparing `datasette-dashboards-0.4.0/datasette_dashboards/static/vega-embed.min.js` & `datasette_dashboards-0.5.0/datasette_dashboards/static/vega-embed.min.js`

 * *Files identical despite different names*

### Comparing `datasette-dashboards-0.4.0/datasette_dashboards/static/vega-lite.min.js` & `datasette_dashboards-0.5.0/datasette_dashboards/static/vega-lite.min.js`

 * *Files identical despite different names*

### Comparing `datasette-dashboards-0.4.0/datasette_dashboards/static/vega.min.js` & `datasette_dashboards-0.5.0/datasette_dashboards/static/vega.min.js`

 * *Files identical despite different names*

### Comparing `datasette-dashboards-0.4.0/datasette_dashboards/templates/dashboard_chart.html` & `datasette_dashboards-0.5.0/datasette_dashboards/templates/dashboard_chart.html`

 * *Files identical despite different names*

### Comparing `datasette-dashboards-0.4.0/datasette_dashboards/templates/dashboard_list.html` & `datasette_dashboards-0.5.0/datasette_dashboards/templates/dashboard_list.html`

 * *Files identical despite different names*

### Comparing `datasette-dashboards-0.4.0/datasette_dashboards/templates/dashboard_view.html` & `datasette_dashboards-0.5.0/datasette_dashboards/templates/dashboard_view.html`

 * *Files identical despite different names*

