# Comparing `tmp/oarepo-model-builder-requests-3.1.1.tar.gz` & `tmp/oarepo-model-builder-requests-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-requests-3.1.1.tar", last modified: Wed Feb 15 14:37:20 2023, max compression
+gzip compressed data, was "oarepo-model-builder-requests-3.1.2.tar", last modified: Thu Apr 20 14:34:14 2023, max compression
```

## Comparing `oarepo-model-builder-requests-3.1.1.tar` & `oarepo-model-builder-requests-3.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:37:20.986697 oarepo-model-builder-requests-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-02-15 14:37:20.986697 oarepo-model-builder-requests-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:37:20.974696 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:37:20.978696 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/invenio_requests_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/invenio_requests_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/invenio_requests_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/invenio_requests_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/invenio_requests_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/invenio_requests_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/invenio_requests_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:37:20.982697 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_actions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_resolvers.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_views.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:37:20.982697 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/model_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/model_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/model_preprocessors/invenio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:37:20.982697 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/tests/invenio_requests_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/tests/invenio_requests_test_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:37:20.982697 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:37:20.982697 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:37:20.974696 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-02-15 14:37:20.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-02-15 14:37:20.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 14:37:20.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-02-15 14:37:20.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-15 14:37:20.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-15 14:37:20.000000 oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-02-15 14:37:20.986697 oarepo-model-builder-requests-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 14:37:20.986697 oarepo-model-builder-requests-3.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-02-15 14:34:11.000000 oarepo-model-builder-requests-3.1.1/tests/test_custom_action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.950141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_actions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_resolvers.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_views.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/model_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/model_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/model_preprocessors/invenio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/invenio_requests_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/invenio_requests_test_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.950141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-20 14:34:14.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-20 14:34:14.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:34:14.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-20 14:34:14.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 14:34:14.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 14:34:14.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-20 14:34:14.958141 oarepo-model-builder-requests-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/tests/test_custom_action.py
```

### Comparing `oarepo-model-builder-requests-3.1.1/LICENSE` & `oarepo-model-builder-requests-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.1/PKG-INFO` & `oarepo-model-builder-requests-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-requests
-Version: 3.1.1
+Version: 3.1.2
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder requests
 Plugin for oarepo-model-builder to allow specifying requests 
 tied to the base model, based on invenio requests. <br>
```

### Comparing `oarepo-model-builder-requests-3.1.1/README.md` & `oarepo-model-builder-requests-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/invenio_requests_builder.py` & `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_actions.py.jinja2` & `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_actions.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_config.py.jinja2` & `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2` & `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/model_preprocessors/invenio.py` & `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/model_preprocessors/invenio.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2` & `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2` & `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     request_record_input_data,
 ):
     receiver_user = users[1]
     sender_identity = identity_simple
     receiver_identity = identity_simple_2
     request_types = app.extensions["invenio-requests"].request_type_registry
     for request_type in request_types:
+        if request_type.__module__ != "{{ current_model.requests_types }}":
+            continue
         request = submit_request(
             sender_identity,
             data=request_record_input_data,
             topic=example_{{ current_model.record_prefix_snake }},
             request_type=request_type,
             receiver=receiver_user,
         )
```

### Comparing `oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests/validation/__init__.py` & `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests.egg-info/PKG-INFO` & `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-requests
-Version: 3.1.1
+Version: 3.1.2
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder requests
 Plugin for oarepo-model-builder to allow specifying requests 
 tied to the base model, based on invenio requests. <br>
```

### Comparing `oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests.egg-info/SOURCES.txt` & `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.1/oarepo_model_builder_requests.egg-info/entry_points.txt` & `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.1/setup.cfg` & `oarepo-model-builder-requests-3.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-requests
-version = 3.1.1
+version = 3.1.2
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

### Comparing `oarepo-model-builder-requests-3.1.1/tests/test_custom_action.py` & `oarepo-model-builder-requests-3.1.2/tests/test_custom_action.py`

 * *Files identical despite different names*

