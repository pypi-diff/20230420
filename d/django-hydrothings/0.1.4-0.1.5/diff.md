# Comparing `tmp/django-hydrothings-0.1.4.tar.gz` & `tmp/django-hydrothings-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hydrothings-0.1.4.tar", last modified: Thu Apr  6 22:45:31 2023, max compression
+gzip compressed data, was "django-hydrothings-0.1.5.tar", last modified: Wed Apr 19 23:19:55 2023, max compression
```

## Comparing `django-hydrothings-0.1.4.tar` & `django-hydrothings-0.1.5.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.244373 django-hydrothings-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-06 22:45:31.244373 django-hydrothings-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-06 22:45:31.244373 django-hydrothings-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.232373 django-hydrothings-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.236373 django-hydrothings-0.1.4/src/django_hydrothings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-06 22:45:31.000000 django-hydrothings-0.1.4/src/django_hydrothings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-06 22:45:31.000000 django-hydrothings-0.1.4/src/django_hydrothings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 22:45:31.000000 django-hydrothings-0.1.4/src/django_hydrothings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-06 22:45:31.000000 django-hydrothings-0.1.4/src/django_hydrothings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-06 22:45:31.000000 django-hydrothings-0.1.4/src/django_hydrothings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 22:45:31.000000 django-hydrothings-0.1.4/src/django_hydrothings.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.236373 django-hydrothings-0.1.4/src/hydrothings/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.236373 django-hydrothings-0.1.4/src/hydrothings/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.236373 django-hydrothings-0.1.4/src/hydrothings/backends/frostserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/frostserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/frostserver/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/frostserver/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/frostserver/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/frostserver/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.236373 django-hydrothings-0.1.4/src/hydrothings/backends/odm2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/odm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/odm2/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/odm2/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/odm2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/odm2/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/odm2/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.236373 django-hydrothings-0.1.4/src/hydrothings/backends/sensorthings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/sensorthings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/sensorthings/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/sensorthings/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/sensorthings/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/backends/sensorthings/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.236373 django-hydrothings-0.1.4/src/hydrothings/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.240373 django-hydrothings-0.1.4/src/hydrothings/components/datastreams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/datastreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/datastreams/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/datastreams/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.240373 django-hydrothings-0.1.4/src/hydrothings/components/featuresofinterest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/featuresofinterest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/featuresofinterest/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/featuresofinterest/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.240373 django-hydrothings-0.1.4/src/hydrothings/components/historicallocations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/historicallocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/historicallocations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/historicallocations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.240373 django-hydrothings-0.1.4/src/hydrothings/components/locations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/locations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/locations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.240373 django-hydrothings-0.1.4/src/hydrothings/components/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/observations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/observations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.240373 django-hydrothings-0.1.4/src/hydrothings/components/observedproperties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/observedproperties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/observedproperties/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/observedproperties/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.240373 django-hydrothings-0.1.4/src/hydrothings/components/root/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/root/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/root/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/root/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.240373 django-hydrothings-0.1.4/src/hydrothings/components/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/sensors/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/sensors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/sensors/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.240373 django-hydrothings-0.1.4/src/hydrothings/components/things/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/things/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/things/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/components/things/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.240373 django-hydrothings-0.1.4/src/hydrothings/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/extras/iso_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/src/hydrothings/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:45:31.240373 django-hydrothings-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/tests/test_allow_partial_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/tests/test_iso_interval_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/tests/test_iso_time_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/tests/test_metadata_field_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/tests/test_resolve_chained_entity_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/tests/test_sensorthings_abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-06 22:45:16.000000 django-hydrothings-0.1.4/tests/test_whitespace_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.410374 django-hydrothings-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-19 23:19:55.410374 django-hydrothings-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-19 23:19:55.410374 django-hydrothings-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.398373 django-hydrothings-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.398373 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-19 23:19:55.000000 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-19 23:19:55.000000 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:19:55.000000 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-19 23:19:55.000000 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 23:19:55.000000 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:19:55.000000 django-hydrothings-0.1.5/src/django_hydrothings.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/odm2/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/components/datastreams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/datastreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/datastreams/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/datastreams/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.402373 django-hydrothings-0.1.5/src/hydrothings/components/featuresofinterest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/featuresofinterest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/featuresofinterest/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/featuresofinterest/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/historicallocations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/historicallocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/historicallocations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/historicallocations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/locations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/locations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/observedproperties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observedproperties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observedproperties/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/observedproperties/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/root/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/root/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/root/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/root/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/sensors/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/sensors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/sensors/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/components/things/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/things/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/things/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/components/things/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.406373 django-hydrothings-0.1.5/src/hydrothings/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/extras/iso_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/src/hydrothings/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:19:55.410374 django-hydrothings-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_allow_partial_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_iso_interval_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_iso_time_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_metadata_field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_resolve_chained_entity_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_sensorthings_abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-19 23:19:40.000000 django-hydrothings-0.1.5/tests/test_whitespace_validator.py
```

### Comparing `django-hydrothings-0.1.4/LICENSE.txt` & `django-hydrothings-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/README.md` & `django-hydrothings-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/django_hydrothings.egg-info/SOURCES.txt` & `django-hydrothings-0.1.5/src/django_hydrothings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/backends/frostserver/engine.py` & `django-hydrothings-0.1.5/src/hydrothings/backends/frostserver/engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/backends/odm2/engine.py` & `django-hydrothings-0.1.5/src/hydrothings/backends/odm2/engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/backends/sensorthings/engine.py` & `django-hydrothings-0.1.5/src/hydrothings/backends/sensorthings/engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/__init__.py` & `django-hydrothings-0.1.5/src/hydrothings/components/__init__.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/datastreams/schemas.py` & `django-hydrothings-0.1.5/src/hydrothings/components/datastreams/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/datastreams/views.py` & `django-hydrothings-0.1.5/src/hydrothings/components/datastreams/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     response = request.engine.list(
         **parse_query_params(
             query_params=params.dict(),
             entity_chain=request.entity_chain
         )
     )
 
-    return entities_or_404(response)
+    return entities_or_404(response, DatastreamListResponse)
 
 
 @router.get(
     '/Datastreams({datastream_id})',
     response=generate_response_codes('get', DatastreamGetResponse),
     by_alias=True
 )
@@ -48,15 +48,15 @@
       Datastream Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/datastream/relations" target="_blank">\
       Datastream Relations</a>
     """
 
     response = request.engine.get(entity_id=datastream_id)
 
-    return entity_or_404(response, datastream_id)
+    return entity_or_404(response, datastream_id, DatastreamGetResponse)
 
 
 @router.post(
     '/Datastreams',
     response=generate_response_codes('create')
 )
 def create_datastream(request: SensorThingsRequest, response: HttpResponse, datastream: DatastreamPostBody):
```

#### html2text {}

```diff
@@ -5,27 +5,28 @@
 DatastreamPostBody, DatastreamPatchBody, DatastreamListResponse,
 DatastreamGetResponse router = Router(tags=['Datastreams']) @router.get( '/
 Datastreams', response=generate_response_codes('list', DatastreamListResponse),
 by_alias=True, url_name='list_datastream' ) def list_datastreams(request:
 SensorThingsRequest, params: QueryParams = Query(...)): """ Get a collection of
 Datastream entities. \_Datastream_Properties - \_Datastream_Relations """
 response = request.engine.list( **parse_query_params( query_params=params.dict
-(), entity_chain=request.entity_chain ) ) return entities_or_404(response)
-@router.get( '/Datastreams({datastream_id})', response=generate_response_codes
-('get', DatastreamGetResponse), by_alias=True ) def get_datastream(request:
-SensorThingsRequest, datastream_id: str): """ Get a Datastream entity. \
-Datastream_Properties - \_Datastream_Relations """ response =
-request.engine.get(entity_id=datastream_id) return entity_or_404(response,
-datastream_id) @router.post( '/Datastreams', response=generate_response_codes
-('create') ) def create_datastream(request: SensorThingsRequest, response:
-HttpResponse, datastream: DatastreamPostBody): """ Create a new Datastream
-entity. Links: \_Datastream_Properties - \_Datastream_Relations - \_Create
-Entity """ datastream_id = request.engine.create( entity_body=datastream )
-response['location'] = request.engine.get_ref( entity_id=datastream_id ) return
-201, None @router.patch( '/Datastreams({datastream_id})',
+(), entity_chain=request.entity_chain ) ) return entities_or_404(response,
+DatastreamListResponse) @router.get( '/Datastreams({datastream_id})',
+response=generate_response_codes('get', DatastreamGetResponse), by_alias=True )
+def get_datastream(request: SensorThingsRequest, datastream_id: str): """ Get a
+Datastream entity. \_Datastream_Properties - \_Datastream_Relations """
+response = request.engine.get(entity_id=datastream_id) return entity_or_404
+(response, datastream_id, DatastreamGetResponse) @router.post( '/Datastreams',
+response=generate_response_codes('create') ) def create_datastream(request:
+SensorThingsRequest, response: HttpResponse, datastream: DatastreamPostBody):
+""" Create a new Datastream entity. Links: \_Datastream_Properties - \
+Datastream_Relations - \_Create_Entity """ datastream_id =
+request.engine.create( entity_body=datastream ) response['location'] =
+request.engine.get_ref( entity_id=datastream_id ) return 201, None
+@router.patch( '/Datastreams({datastream_id})',
 response=generate_response_codes('update') ) def update_datastream(request:
 SensorThingsRequest, datastream_id: str, datastream: DatastreamPatchBody): """
 Update an existing Datastream entity. Links: \_Datastream_Properties - \
 Datastream_Relations - \_Update_Entity """ request.engine.update
 ( entity_id=datastream_id, entity_body=datastream ) return 204, None
 @router.delete( '/Datastreams({datastream_id})',
 response=generate_response_codes('delete') ) def delete_datastream(request:
```

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/featuresofinterest/schemas.py` & `django-hydrothings-0.1.5/src/hydrothings/components/featuresofinterest/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/featuresofinterest/views.py` & `django-hydrothings-0.1.5/src/hydrothings/components/featuresofinterest/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     response = request.engine.list(
         **parse_query_params(
             query_params=params.dict(),
             entity_chain=request.entity_chain
         )
     )
 
-    return entities_or_404(response)
+    return entities_or_404(response, FeatureOfInterestListResponse)
 
 
 @router.get(
     '/FeaturesOfInterest({feature_of_interest_id})',
     response=generate_response_codes('get', FeatureOfInterestGetResponse),
     by_alias=True
 )
@@ -48,15 +48,15 @@
       Feature of Interest Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/feature-of-interest/relations" target="_blank">\
       Feature of Interest Relations</a>
     """
 
     response = request.engine.get(entity_id=feature_of_interest_id)
 
-    return entity_or_404(response, feature_of_interest_id)
+    return entity_or_404(response, feature_of_interest_id, FeatureOfInterestGetResponse)
 
 
 @router.post(
     '/FeaturesOfInterest',
     response=generate_response_codes('create')
 )
 def create_feature_of_interest(
```

#### html2text {}

```diff
@@ -7,27 +7,28 @@
 (tags=['Features Of Interest']) @router.get( '/FeaturesOfInterest',
 response=generate_response_codes('list', FeatureOfInterestListResponse),
 url_name='list_feature_of_interest' ) def list_features_of_interest(request:
 SensorThingsRequest, params: QueryParams = Query(...)): """ Get a collection of
 Feature of Interest entities. \_Feature_of_Interest_Properties - \_Feature_of
 Interest_Relations """ response = request.engine.list( **parse_query_params
 ( query_params=params.dict(), entity_chain=request.entity_chain ) ) return
-entities_or_404(response) @router.get( '/FeaturesOfInterest(
-{feature_of_interest_id})', response=generate_response_codes('get',
-FeatureOfInterestGetResponse), by_alias=True ) def get_feature_of_interest
-(request, feature_of_interest_id: str): """ Get a Feature of Interest entity. \
-Feature_of_Interest_Properties - \_Feature_of_Interest_Relations """ response =
-request.engine.get(entity_id=feature_of_interest_id) return entity_or_404
-(response, feature_of_interest_id) @router.post( '/FeaturesOfInterest',
-response=generate_response_codes('create') ) def create_feature_of_interest
-( request: SensorThingsRequest, response: HttpResponse, feature_of_interest:
-FeatureOfInterestPostBody ): """ Create a new Feature of Interest entity.
-Links: \_Feature_of_Interest_Properties - \_Feature_of_Interest_Relations - \
-Create_Entity """ feature_of_interest_id = request.engine.create
-( entity_body=feature_of_interest ) response['location'] =
+entities_or_404(response, FeatureOfInterestListResponse) @router.get( '/
+FeaturesOfInterest({feature_of_interest_id})', response=generate_response_codes
+('get', FeatureOfInterestGetResponse), by_alias=True ) def
+get_feature_of_interest(request, feature_of_interest_id: str): """ Get a
+Feature of Interest entity. \_Feature_of_Interest_Properties - \_Feature_of
+Interest_Relations """ response = request.engine.get
+(entity_id=feature_of_interest_id) return entity_or_404(response,
+feature_of_interest_id, FeatureOfInterestGetResponse) @router.post( '/
+FeaturesOfInterest', response=generate_response_codes('create') ) def
+create_feature_of_interest( request: SensorThingsRequest, response:
+HttpResponse, feature_of_interest: FeatureOfInterestPostBody ): """ Create a
+new Feature of Interest entity. Links: \_Feature_of_Interest_Properties - \
+Feature_of_Interest_Relations - \_Create_Entity """ feature_of_interest_id =
+request.engine.create( entity_body=feature_of_interest ) response['location'] =
 request.engine.get_ref( entity_id=feature_of_interest_id ) return 201, None
 @router.patch( '/FeaturesOfInterest({feature_of_interest_id})',
 response=generate_response_codes('update') ) def update_feature_of_interest
 ( request: SensorThingsRequest, feature_of_interest_id: str,
 feature_of_interest: FeatureOfInterestPatchBody ): """ Update an existing
 Feature of Interest entity. Links: \_Feature_of_Interest_Properties - \_Feature
 of_Interest_Relations - \_Update_Entity """ request.engine.update
```

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/historicallocations/schemas.py` & `django-hydrothings-0.1.5/src/hydrothings/components/historicallocations/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/historicallocations/views.py` & `django-hydrothings-0.1.5/src/hydrothings/components/historicallocations/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     response = request.engine.list(
         **parse_query_params(
             query_params=params.dict(),
             entity_chain=request.entity_chain
         )
     )
 
-    return entities_or_404(response)
+    return entities_or_404(response, HistoricalLocationListResponse)
 
 
 @router.get(
     '/HistoricalLocations({historical_location_id})',
     response=generate_response_codes('get', HistoricalLocationGetResponse),
     by_alias=True
 )
@@ -49,15 +49,15 @@
       Historical Location Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/historical-location/relations" target="_blank">\
       Historical Location Relations</a>
     """
 
     response = request.engine.get(entity_id=historical_location_id)
 
-    return entity_or_404(response, historical_location_id)
+    return entity_or_404(response, historical_location_id, HistoricalLocationGetResponse)
 
 
 @router.post(
     '/HistoricalLocations',
     response=generate_response_codes('create')
 )
 def create_historical_location(
```

#### html2text {}

```diff
@@ -7,28 +7,29 @@
 (tags=['Historical Locations']) @router.get( '/HistoricalLocations',
 response=generate_response_codes('list', HistoricalLocationListResponse),
 by_alias=True, url_name='list_historical_location' ) def
 list_historical_locations(request: SensorThingsRequest, params: QueryParams =
 Query(...)): """ Get a collection of Historical Location entities. \_Historical
 Location_Properties - \_Historical_Location_Relations """ response =
 request.engine.list( **parse_query_params( query_params=params.dict(),
-entity_chain=request.entity_chain ) ) return entities_or_404(response)
-@router.get( '/HistoricalLocations({historical_location_id})',
-response=generate_response_codes('get', HistoricalLocationGetResponse),
-by_alias=True ) def get_historical_location(request: SensorThingsRequest,
-historical_location_id: str): """ Get a Historical Location entity. \
-Historical_Location_Properties - \_Historical_Location_Relations """ response =
-request.engine.get(entity_id=historical_location_id) return entity_or_404
-(response, historical_location_id) @router.post( '/HistoricalLocations',
-response=generate_response_codes('create') ) def create_historical_location
-( request: SensorThingsRequest, response: HttpResponse, historical_location:
-HistoricalLocationPostBody ): """ Create a new Historical Location entity.
-Links: \_Historical_Location_Properties - \_Historical_Location_Relations - \
-Create_Entity """ historical_location_id = request.engine.create
-( entity_body=historical_location ) response['location'] =
+entity_chain=request.entity_chain ) ) return entities_or_404(response,
+HistoricalLocationListResponse) @router.get( '/HistoricalLocations(
+{historical_location_id})', response=generate_response_codes('get',
+HistoricalLocationGetResponse), by_alias=True ) def get_historical_location
+(request: SensorThingsRequest, historical_location_id: str): """ Get a
+Historical Location entity. \_Historical_Location_Properties - \_Historical
+Location_Relations """ response = request.engine.get
+(entity_id=historical_location_id) return entity_or_404(response,
+historical_location_id, HistoricalLocationGetResponse) @router.post( '/
+HistoricalLocations', response=generate_response_codes('create') ) def
+create_historical_location( request: SensorThingsRequest, response:
+HttpResponse, historical_location: HistoricalLocationPostBody ): """ Create a
+new Historical Location entity. Links: \_Historical_Location_Properties - \
+Historical_Location_Relations - \_Create_Entity """ historical_location_id =
+request.engine.create( entity_body=historical_location ) response['location'] =
 request.engine.get_ref( entity_id=historical_location_id ) return 201, None
 @router.patch( '/HistoricalLocations({historical_location_id})',
 response=generate_response_codes('update') ) def update_historical_location
 ( request: SensorThingsRequest, historical_location_id: str,
 historical_location: HistoricalLocationPatchBody ): """ Update an existing
 Historical Location entity. Links: \_Historical_Location_Properties - \
 Historical_Location_Relations - \_Update_Entity """ request.engine.update
```

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/locations/schemas.py` & `django-hydrothings-0.1.5/src/hydrothings/components/locations/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/locations/views.py` & `django-hydrothings-0.1.5/src/hydrothings/components/locations/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     response = request.engine.list(
         **parse_query_params(
             query_params=params.dict(),
             entity_chain=request.entity_chain
         )
     )
 
-    return entities_or_404(response)
+    return entities_or_404(response, LocationListResponse)
 
 
 @router.get(
     '/Locations({location_id})',
     response=generate_response_codes('get', LocationGetResponse),
     by_alias=True
 )
@@ -48,15 +48,15 @@
       Location Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/location/relations" target="_blank">\
       Location Relations</a>
     """
 
     response = request.engine.get(entity_id=location_id)
 
-    return entity_or_404(response, location_id)
+    return entity_or_404(response, location_id, LocationGetResponse)
 
 
 @router.post(
     '/Locations',
     response=generate_response_codes('create')
 )
 def create_location(request: SensorThingsRequest, response: HttpResponse, location: LocationPostBody):
```

#### html2text {}

```diff
@@ -5,27 +5,28 @@
 LocationPostBody, LocationPatchBody, LocationListResponse, LocationGetResponse
 router = Router(tags=['Locations']) @router.get( '/Locations',
 response=generate_response_codes('list', LocationListResponse), by_alias=True,
 url_name='list_location' ) def list_locations(request: SensorThingsRequest,
 params: QueryParams = Query(...)): """ Get a collection of Location entities. \
 Location_Properties - \_Location_Relations """ response = request.engine.list
 ( **parse_query_params( query_params=params.dict(),
-entity_chain=request.entity_chain ) ) return entities_or_404(response)
-@router.get( '/Locations({location_id})', response=generate_response_codes
-('get', LocationGetResponse), by_alias=True ) def get_location(request:
-SensorThingsRequest, location_id: str): """ Get a Location entity. \_Location
-Properties - \_Location_Relations """ response = request.engine.get
-(entity_id=location_id) return entity_or_404(response, location_id)
-@router.post( '/Locations', response=generate_response_codes('create') ) def
-create_location(request: SensorThingsRequest, response: HttpResponse, location:
-LocationPostBody): """ Create a new Location entity. Links: \_Location
-Properties - \_Location_Relations - \_Create_Entity """ location_id =
-request.engine.create( entity_body=location ) response['location'] =
-request.engine.get_ref( entity_id=location_id ) return 201, None @router.patch
-( '/Locations({location_id})', response=generate_response_codes('update') ) def
+entity_chain=request.entity_chain ) ) return entities_or_404(response,
+LocationListResponse) @router.get( '/Locations({location_id})',
+response=generate_response_codes('get', LocationGetResponse), by_alias=True )
+def get_location(request: SensorThingsRequest, location_id: str): """ Get a
+Location entity. \_Location_Properties - \_Location_Relations """ response =
+request.engine.get(entity_id=location_id) return entity_or_404(response,
+location_id, LocationGetResponse) @router.post( '/Locations',
+response=generate_response_codes('create') ) def create_location(request:
+SensorThingsRequest, response: HttpResponse, location: LocationPostBody): """
+Create a new Location entity. Links: \_Location_Properties - \_Location
+Relations - \_Create_Entity """ location_id = request.engine.create
+( entity_body=location ) response['location'] = request.engine.get_ref
+( entity_id=location_id ) return 201, None @router.patch( '/Locations(
+{location_id})', response=generate_response_codes('update') ) def
 update_location(request: SensorThingsRequest, location_id: str, location:
 LocationPatchBody): """ Update an existing Location entity. Links: \_Location
 Properties - \_Location_Relations - \_Update_Entity """ request.engine.update
 ( entity_id=location_id, entity_body=location ) return 204, None @router.delete
 ( '/Locations({location_id})', response=generate_response_codes('delete') ) def
 delete_location(request: SensorThingsRequest, location_id: str): """ Delete a
 Location entity. Links: \_Delete_Entity """ request.engine.delete
```

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/observations/schemas.py` & `django-hydrothings-0.1.5/src/hydrothings/components/observations/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/observations/utils.py` & `django-hydrothings-0.1.5/src/hydrothings/components/observations/utils.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/observations/views.py` & `django-hydrothings-0.1.5/src/hydrothings/components/observations/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,17 @@
             entity_chain=request.entity_chain,
             sort_datastream=True
         )
     )
 
     if result_format == 'dataArray':
         response = convert_to_data_array(request, response)
-
-    return entities_or_404(response)
+        return entities_or_404(response, ObservationDataArrayResponse)
+    else:
+        return entities_or_404(response, ObservationListResponse)
 
 
 @router.get(
     '/Observations({observation_id})',
     response=generate_response_codes('get', ObservationGetResponse),
     by_alias=True
 )
@@ -58,15 +59,15 @@
       Observation Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/observation/relations" target="_blank">\
       Observation Relations</a>
     """
 
     response = request.engine.get(entity_id=observation_id)
 
-    return entity_or_404(response, observation_id)
+    return entity_or_404(response, observation_id, ObservationGetResponse)
 
 
 @router.post(
     '/Observations',
     response=generate_response_codes('create')
 )
 def create_observation(
```

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/observedproperties/schemas.py` & `django-hydrothings-0.1.5/src/hydrothings/components/observedproperties/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/observedproperties/views.py` & `django-hydrothings-0.1.5/src/hydrothings/components/observedproperties/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     response = request.engine.list(
         **parse_query_params(
             query_params=params.dict(),
             entity_chain=request.entity_chain
         )
     )
 
-    return entities_or_404(response)
+    return entities_or_404(response, ObservedPropertyListResponse)
 
 
 @router.get(
     '/ObservedProperties({observed_property_id})',
     response=generate_response_codes('get', ObservedPropertyGetResponse),
     by_alias=True
 )
@@ -50,15 +50,15 @@
       Observed Property Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/observed-property/relations" target="_blank">\
       Observed Property Relations</a>
     """
 
     response = request.engine.get(entity_id=observed_property_id)
 
-    return entity_or_404(response, observed_property_id)
+    return entity_or_404(response, observed_property_id, ObservedPropertyGetResponse)
 
 
 @router.post(
     '/ObservedProperties',
     response=generate_response_codes('create')
 )
 def create_observed_property(
```

#### html2text {}

```diff
@@ -7,33 +7,33 @@
 (tags=['Observed Properties']) @router.get( '/ObservedProperties',
 response=generate_response_codes('list', ObservedPropertyListResponse),
 by_alias=True, url_name='list_observed_property', exclude_none=True ) def
 list_observed_properties(request: SensorThingsRequest, params: QueryParams =
 Query(...)): """ Get a collection of Observed Property entities. \_Observed
 Property_Properties - \_Observed_Property_Relations """ response =
 request.engine.list( **parse_query_params( query_params=params.dict(),
-entity_chain=request.entity_chain ) ) return entities_or_404(response)
-@router.get( '/ObservedProperties({observed_property_id})',
-response=generate_response_codes('get', ObservedPropertyGetResponse),
-by_alias=True ) def get_observed_property(request, observed_property_id: str):
-""" Get an Observed Property entity. \_Observed_Property_Properties - \
-Observed_Property_Relations """ response = request.engine.get
-(entity_id=observed_property_id) return entity_or_404(response,
-observed_property_id) @router.post( '/ObservedProperties',
-response=generate_response_codes('create') ) def create_observed_property
-( request: SensorThingsRequest, response: HttpResponse, observed_property:
-ObservedPropertyPostBody ): """ Create a new Observed Property entity. Links: \
-Observed_Property_Properties - \_Observed_Property_Relations - \_Create_Entity
-""" observed_property_id = request.engine.create( entity_body=observed_property
-) response['location'] = request.engine.get_ref( entity_id=observed_property_id
-) return 201, None @router.patch( '/ObservedProperties(
-{observed_property_id})', response=generate_response_codes('update') ) def
-update_observed_property( request: SensorThingsRequest, observed_property_id:
-str, observed_property: ObservedPropertyPatchBody ): """ Update an existing
-Observed Property entity. Links: \_Thing_Properties - \_Thing_Relations - \
-Update_Entity """ request.engine.update( entity_id=observed_property_id,
-entity_body=observed_property ) return 204, None @router.delete( '/
+entity_chain=request.entity_chain ) ) return entities_or_404(response,
+ObservedPropertyListResponse) @router.get( '/ObservedProperties(
+{observed_property_id})', response=generate_response_codes('get',
+ObservedPropertyGetResponse), by_alias=True ) def get_observed_property
+(request, observed_property_id: str): """ Get an Observed Property entity. \
+Observed_Property_Properties - \_Observed_Property_Relations """ response =
+request.engine.get(entity_id=observed_property_id) return entity_or_404
+(response, observed_property_id, ObservedPropertyGetResponse) @router.post( '/
+ObservedProperties', response=generate_response_codes('create') ) def
+create_observed_property( request: SensorThingsRequest, response: HttpResponse,
+observed_property: ObservedPropertyPostBody ): """ Create a new Observed
+Property entity. Links: \_Observed_Property_Properties - \_Observed_Property
+Relations - \_Create_Entity """ observed_property_id = request.engine.create
+( entity_body=observed_property ) response['location'] = request.engine.get_ref
+( entity_id=observed_property_id ) return 201, None @router.patch( '/
 ObservedProperties({observed_property_id})', response=generate_response_codes
-('delete') ) def delete_observed_property(request: SensorThingsRequest,
-observed_property_id: str): """ Delete an Observed Property entity. Links: \
-Delete_Entity """ request.engine.delete( entity_id=observed_property_id )
-return 204, None
+('update') ) def update_observed_property( request: SensorThingsRequest,
+observed_property_id: str, observed_property: ObservedPropertyPatchBody ): """
+Update an existing Observed Property entity. Links: \_Thing_Properties - \
+Thing_Relations - \_Update_Entity """ request.engine.update
+( entity_id=observed_property_id, entity_body=observed_property ) return 204,
+None @router.delete( '/ObservedProperties({observed_property_id})',
+response=generate_response_codes('delete') ) def delete_observed_property
+(request: SensorThingsRequest, observed_property_id: str): """ Delete an
+Observed Property entity. Links: \_Delete_Entity """ request.engine.delete
+( entity_id=observed_property_id ) return 204, None
```

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/root/views.py` & `django-hydrothings-0.1.5/src/hydrothings/components/root/views.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/sensors/schemas.py` & `django-hydrothings-0.1.5/src/hydrothings/components/sensors/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/sensors/utils.py` & `django-hydrothings-0.1.5/src/hydrothings/components/sensors/utils.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/sensors/views.py` & `django-hydrothings-0.1.5/src/hydrothings/components/sensors/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     response = request.engine.list(
         **parse_query_params(
             query_params=params.dict(),
             entity_chain=request.entity_chain
         )
     )
-    return entities_or_404(response)
+    return entities_or_404(response, SensorListResponse)
 
 
 @router.get(
     '/Sensors({sensor_id})',
     response=generate_response_codes('get', SensorGetResponse),
     by_alias=True
 )
@@ -48,15 +48,15 @@
       Sensor Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/sensor/relations" target="_blank">\
       Sensor Relations</a>
     """
 
     response = request.engine.get(entity_id=sensor_id)
 
-    return entity_or_404(response, sensor_id)
+    return entity_or_404(response, sensor_id, SensorGetResponse)
 
 
 @router.post(
     '/Sensors',
     response=generate_response_codes('create')
 )
 def create_sensor(request: SensorThingsRequest, response: HttpResponse, sensor: SensorPostBody):
```

#### html2text {}

```diff
@@ -5,23 +5,24 @@
 SensorPostBody, SensorPatchBody, SensorListResponse, SensorGetResponse router =
 Router(tags=['Sensors']) @router.get( '/Sensors',
 response=generate_response_codes('list', SensorListResponse), by_alias=True,
 url_name='list_sensor', exclude_none=True ) def list_sensors(request, params:
 QueryParams = Query(...)): """ Get a collection of Sensor entities. \_Sensor
 Properties - \_Sensor_Relations """ response = request.engine.list
 ( **parse_query_params( query_params=params.dict(),
-entity_chain=request.entity_chain ) ) return entities_or_404(response)
-@router.get( '/Sensors({sensor_id})', response=generate_response_codes('get',
-SensorGetResponse), by_alias=True ) def get_sensor(request, sensor_id: str):
-""" Get a Sensor entity. \_Sensor_Properties - \_Sensor_Relations """ response
-= request.engine.get(entity_id=sensor_id) return entity_or_404(response,
-sensor_id) @router.post( '/Sensors', response=generate_response_codes('create')
-) def create_sensor(request: SensorThingsRequest, response: HttpResponse,
-sensor: SensorPostBody): """ Create a new Sensor entity. Links: \_Sensor
-Properties - \_Sensor_Relations - \_Create_Entity """ sensor_id =
+entity_chain=request.entity_chain ) ) return entities_or_404(response,
+SensorListResponse) @router.get( '/Sensors({sensor_id})',
+response=generate_response_codes('get', SensorGetResponse), by_alias=True ) def
+get_sensor(request, sensor_id: str): """ Get a Sensor entity. \_Sensor
+Properties - \_Sensor_Relations """ response = request.engine.get
+(entity_id=sensor_id) return entity_or_404(response, sensor_id,
+SensorGetResponse) @router.post( '/Sensors', response=generate_response_codes
+('create') ) def create_sensor(request: SensorThingsRequest, response:
+HttpResponse, sensor: SensorPostBody): """ Create a new Sensor entity. Links: \
+Sensor_Properties - \_Sensor_Relations - \_Create_Entity """ sensor_id =
 request.engine.create( entity_body=sensor ) response['location'] =
 request.engine.get_ref( entity_id=sensor_id ) return 201, None @router.patch
 ( '/Sensors({sensor_id})', response=generate_response_codes('update') ) def
 update_sensor(request: SensorThingsRequest, sensor_id: str, sensor:
 SensorPatchBody): """ Update an existing Sensor entity. Links: \_Sensor
 Properties - \_Sensor_Relations - \_Update_Entity """ request.engine.update
 ( entity_id=sensor_id, entity_body=sensor ) return 204, None @router.delete( '/
```

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/things/schemas.py` & `django-hydrothings-0.1.5/src/hydrothings/components/things/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/components/things/views.py` & `django-hydrothings-0.1.5/src/hydrothings/components/things/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     response = request.engine.list(
         **parse_query_params(
             query_params=params.dict(),
             entity_chain=request.entity_chain
         )
     )
 
-    return entities_or_404(response)
+    return entities_or_404(response, ThingListResponse)
 
 
 @router.get(
     '/Things({thing_id})',
     response=generate_response_codes('get', ThingGetResponse),
     by_alias=True
 )
@@ -49,15 +49,15 @@
       Thing Properties</a> -
     <a href="http://www.opengis.net/spec/iot_sensing/1.1/req/datamodel/thing/relations" target="_blank">\
       Thing Relations</a>
     """
 
     response = request.engine.get(entity_id=thing_id)
 
-    return entity_or_404(response, thing_id)
+    return entity_or_404(response, thing_id, ThingGetResponse)
 
 
 @router.post(
     '/Things',
     response=generate_response_codes('create')
 )
 def create_thing(request: SensorThingsRequest, response: HttpResponse, thing: ThingPostBody):
```

#### html2text {}

```diff
@@ -5,26 +5,27 @@
 ThingPatchBody, ThingListResponse, ThingGetResponse router = Router(tags=
 ['Things']) @router.get( '/Things', response=generate_response_codes('list',
 ThingListResponse), by_alias=True, url_name='list_thing', exclude_none=True )
 def list_things(request: SensorThingsRequest, params: QueryParams = Query
 (...)): """ Get a collection of Thing entities. \_Thing_Properties - \_Thing
 Relations """ response = request.engine.list( **parse_query_params
 ( query_params=params.dict(), entity_chain=request.entity_chain ) ) return
-entities_or_404(response) @router.get( '/Things({thing_id})',
-response=generate_response_codes('get', ThingGetResponse), by_alias=True ) def
-get_thing(request: SensorThingsRequest, thing_id: str): """ Get a Thing entity.
-\_Thing_Properties - \_Thing_Relations """ response = request.engine.get
-(entity_id=thing_id) return entity_or_404(response, thing_id) @router.post( '/
-Things', response=generate_response_codes('create') ) def create_thing(request:
-SensorThingsRequest, response: HttpResponse, thing: ThingPostBody): """ Create
-a new Thing entity. Links: \_Thing_Properties - \_Thing_Relations - \_Create
-Entity """ thing_id = request.engine.create( entity_body=thing ) response
-['location'] = request.engine.get_ref( entity_id=thing_id ) return 201, None
-@router.patch( '/Things({thing_id})', response=generate_response_codes
-('update') ) def update_thing(request: SensorThingsRequest, thing_id: str,
-thing: ThingPatchBody): """ Update an existing Thing entity. Links: \_Thing
-Properties - \_Thing_Relations - \_Update_Entity """ request.engine.update
+entities_or_404(response, ThingListResponse) @router.get( '/Things(
+{thing_id})', response=generate_response_codes('get', ThingGetResponse),
+by_alias=True ) def get_thing(request: SensorThingsRequest, thing_id: str): """
+Get a Thing entity. \_Thing_Properties - \_Thing_Relations """ response =
+request.engine.get(entity_id=thing_id) return entity_or_404(response, thing_id,
+ThingGetResponse) @router.post( '/Things', response=generate_response_codes
+('create') ) def create_thing(request: SensorThingsRequest, response:
+HttpResponse, thing: ThingPostBody): """ Create a new Thing entity. Links: \
+Thing_Properties - \_Thing_Relations - \_Create_Entity """ thing_id =
+request.engine.create( entity_body=thing ) response['location'] =
+request.engine.get_ref( entity_id=thing_id ) return 201, None @router.patch( '/
+Things({thing_id})', response=generate_response_codes('update') ) def
+update_thing(request: SensorThingsRequest, thing_id: str, thing:
+ThingPatchBody): """ Update an existing Thing entity. Links: \_Thing_Properties
+- \_Thing_Relations - \_Update_Entity """ request.engine.update
 ( entity_id=thing_id, entity_body=thing ) return 204, None @router.delete( '/
 Things({thing_id})', response=generate_response_codes('delete') ) def
 delete_thing(request: SensorThingsRequest, thing_id: str): """ Delete a Thing
 entity. Links: \_Delete_Entity """ request.engine.delete( entity_id=thing_id )
 return 204, None
```

### Comparing `django-hydrothings-0.1.4/src/hydrothings/engine.py` & `django-hydrothings-0.1.5/src/hydrothings/engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/extras/iso_types.py` & `django-hydrothings-0.1.5/src/hydrothings/extras/iso_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,49 @@
-from datetime import datetime
+import pytz
+from dateutil.parser import isoparse
 
 
 class ISOTime(str):
 
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         if not isinstance(v, str):
             raise TypeError('string required')
 
         try:
-            datetime.fromisoformat(v)
+            value = isoparse(v)
+            if value.tzinfo is None:
+                value = value.replace(tzinfo=pytz.UTC)
+            else:
+                value = value.astimezone(pytz.UTC)
         except TypeError:
             raise ValueError('invalid ISO time format')
 
-        return cls(v)
+        return cls(value.isoformat(sep='T', timespec='milliseconds').replace('+00:00', 'Z'))
 
 
 class ISOInterval(str):
 
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         if not isinstance(v, str):
             raise TypeError('string required')
 
-        split_v = v.split('/')
+        split_v = [
+            ISOTime.validate(dt_value) for dt_value in v.split('/')
+        ]
 
         try:
-            if len(split_v) != 2 or datetime.fromisoformat(split_v[0]) >= datetime.fromisoformat(split_v[1]):
+            if len(split_v) != 2 or isoparse(split_v[0]) >= isoparse(split_v[1]):
                 raise TypeError
         except TypeError:
             raise ValueError('invalid ISO interval format')
 
-        return cls(v)
+        return cls('/'.join(split_v))
```

### Comparing `django-hydrothings-0.1.4/src/hydrothings/main.py` & `django-hydrothings-0.1.5/src/hydrothings/main.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/middleware.py` & `django-hydrothings-0.1.5/src/hydrothings/middleware.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/schemas.py` & `django-hydrothings-0.1.5/src/hydrothings/schemas.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/settings.py` & `django-hydrothings-0.1.5/src/hydrothings/settings.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/src/hydrothings/utils.py` & `django-hydrothings-0.1.5/src/hydrothings/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import re
+import inspect
 import hydrothings.schemas as core_schemas
+from ninja import Schema
 from odata_query.grammar import ODataParser, ODataLexer
+from django.http import HttpResponse
 from pydantic import HttpUrl
 from typing import Literal, Union, List
 from requests import Response
 from hydrothings import settings
 
 
 def lookup_component(
@@ -88,30 +91,67 @@
         }
     else:
         response_codes = {}
 
     return response_codes
 
 
-def entities_or_404(response):
+def serialize_response(response, response_model):
+    """"""
+
+    if not inspect.isclass(response_model):
+        return response
+    if not issubclass(response_model, Schema):
+        return response
+
+    new_model = response_model.__new__(response_model)
+
+    fields_values = {}
+
+    for name, field in response_model.__fields__.items():
+        if name in response.keys():
+            if isinstance(response[name], list):
+                fields_values[name] = [
+                    serialize_response(fv, field.type_)
+                    for fv in response[name]
+                ]
+            elif inspect.isclass(field.type_) and issubclass(field.type_, Schema):
+                fields_values[name] = serialize_response(response[name], field.type_)
+            else:
+                fields_values[name] = response[name]
+        elif not field.required:
+            fields_values[name] = field.get_default()
+
+    object.__setattr__(new_model, '__dict__', fields_values)
+    _fields_set = set(response.keys())
+    object.__setattr__(new_model, '__fields_set__', _fields_set)
+
+    new_model._init_private_attributes()
+
+    return new_model
+
+
+def entities_or_404(response, response_model):
     """"""
 
     if isinstance(response, Response):
         return response.status_code, response.content
     else:
-        return 200, response
+        serialized_response = serialize_response(response, response_model).json(by_alias=True)
+        return HttpResponse(content=serialized_response, status=200, content_type='application/json')
 
 
-def entity_or_404(response, entity_id):
+def entity_or_404(response, entity_id, response_model):
     """"""
 
     if isinstance(response, Response):
         return response.status_code, response.content
     elif response:
-        return 200, response
+        serialized_response = serialize_response(response, response_model).json(by_alias=True)
+        return HttpResponse(content=serialized_response, status=200, content_type='application/json')
     else:
         return 404, {'message': f'Record with ID {entity_id} does not exist.'}
 
 
 def parse_query_params(
         query_params: dict,
         entity_chain: Union[List[tuple], None] = None,
```

### Comparing `django-hydrothings-0.1.4/src/hydrothings/validators.py` & `django-hydrothings-0.1.5/src/hydrothings/validators.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/tests/test_allow_partial_decorator.py` & `django-hydrothings-0.1.5/tests/test_allow_partial_decorator.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/tests/test_iso_interval_type.py` & `django-hydrothings-0.1.5/tests/test_iso_interval_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
     class IntervalModel(BaseModel):
         iso_interval: ISOInterval
 
     return IntervalModel
 
 
-@pytest.mark.parametrize('iso_interval_value', [
-    '2023-01-01T11:11:11+00:00/2023-01-02T11:11:11+00:00', '2023-01-01T11:11:11/2023-01-02T11:11:11'
+@pytest.mark.parametrize('iso_interval_value, iso_parsed_value', [
+    ['2023-01-01T11:11:11+00:00/2023-01-02T11:11:11+00:00', '2023-01-01T11:11:11.000Z/2023-01-02T11:11:11.000Z'],
+    ['2023-01-01T11:11:11/2023-01-02T11:11:11', '2023-01-01T11:11:11.000Z/2023-01-02T11:11:11.000Z']
 ])
-def test_iso_interval_valid_value(interval_model, iso_interval_value):
+def test_iso_interval_valid_value(interval_model, iso_interval_value, iso_parsed_value):
     interval_instance = interval_model(iso_interval=iso_interval_value)
-    assert interval_instance.iso_interval == iso_interval_value
+    assert interval_instance.iso_interval == iso_parsed_value
 
 
 @pytest.mark.parametrize('iso_interval_value', [
     '2023-01-01T11:11:11+00:00', '2023-01-01T11:11:11+00:00/2023-01-02T11:11:11+00:00/2023-01-03T11:11:11+00:00',
     '2023-01-02T11:11:11+00:00/2023-01-01T11:11:11+00:00', 'Jan 1, 2023/Jan 2, 2023', 123, None,
     '2023-01-01T11:11:11+00:00/2023-13-02T11:11:11+00:00', '2023-01-32T11:11:11+00:00/2023-02-02T11:11:11+00:00',
-    '2023-01-01T11:11:11+00:00|2023-01-02T11:11:11+00:00', '2023-01-01T11:11:11+00:00/2023-01-02T11:11:11',
-    '2023-01-01T11:11:11/2023-01-02T11:11:11+00:00'
+    '2023-01-01T11:11:11+00:00|2023-01-02T11:11:11+00:00'
 ])
 def test_iso_interval_invalid_value(interval_model, iso_interval_value):
     with pytest.raises(ValueError):
         interval_model(iso_interval=iso_interval_value)
```

### Comparing `django-hydrothings-0.1.4/tests/test_metadata_field_validator.py` & `django-hydrothings-0.1.5/tests/test_metadata_field_validator.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/tests/test_resolve_chained_entity_url.py` & `django-hydrothings-0.1.5/tests/test_resolve_chained_entity_url.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/tests/test_sensorthings_abstract_engine.py` & `django-hydrothings-0.1.5/tests/test_sensorthings_abstract_engine.py`

 * *Files identical despite different names*

### Comparing `django-hydrothings-0.1.4/tests/test_whitespace_validator.py` & `django-hydrothings-0.1.5/tests/test_whitespace_validator.py`

 * *Files identical despite different names*

