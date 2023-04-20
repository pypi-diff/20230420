# Comparing `tmp/odoo13-addon-photovoltaic_api-13.0.1.1.0.tar.gz` & `tmp/odoo13-addon-photovoltaic_api-13.0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo13-addon-photovoltaic_api-13.0.1.1.0.tar", last modified: Tue Apr 11 10:20:00 2023, max compression
+gzip compressed data, was "odoo13-addon-photovoltaic_api-13.0.1.1.1.tar", last modified: Thu Apr 20 10:15:45 2023, max compression
```

## Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0.tar` & `odoo13-addon-photovoltaic_api-13.0.1.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.763423 odoo13-addon-photovoltaic_api-13.0.1.1.0/
--rw-r--r--   0 root         (0) root         (0)      448 2023-04-11 10:20:00.762422 odoo13-addon-photovoltaic_api-13.0.1.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.746421 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.746421 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.750421 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/
--rw-rw-rw-   0 root         (0) root         (0)      692 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.751422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/controllers/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/controllers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/controllers/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.751422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/data/
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/data/data.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.752422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/models/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.755422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/allocation.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/bank_account.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/contract.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/info.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/list_response.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/power_station.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.756422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/security/
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/security/ir.model.access.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.759422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4715 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/account.py
--rw-rw-rw-   0 root         (0) root         (0)     4970 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/allocations.py
--rw-rw-rw-   0 root         (0) root         (0)     3533 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/bank_account.py
--rw-rw-rw-   0 root         (0) root         (0)     5989 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/contracts.py
--rw-rw-rw-   0 root         (0) root         (0)     2057 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/info.py
--rw-rw-rw-   0 root         (0) root         (0)     3290 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/powerstation.py
--rw-rw-rw-   0 root         (0) root         (0)     3698 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.760422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/tests/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1640 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/tests/common.py
--rw-rw-rw-   0 root         (0) root         (0)     6052 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/tests/test_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:20:00.762422 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      448 2023-04-11 10:20:00.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1850 2023-04-11 10:20:00.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 10:20:00.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 10:20:00.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      212 2023-04-11 10:20:00.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 10:20:00.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 10:20:00.763423 odoo13-addon-photovoltaic_api-13.0.1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-04-11 10:19:37.000000 odoo13-addon-photovoltaic_api-13.0.1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.474817 odoo13-addon-photovoltaic_api-13.0.1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-20 10:15:45.474817 odoo13-addon-photovoltaic_api-13.0.1.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.458816 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.458816 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.462816 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.463817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/controllers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/controllers/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.463817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/data/
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/data/data.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.464817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/models/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.467817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/allocation.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/bank_account.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/contract.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/info.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/power_station.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.468817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.470817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4651 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     4970 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/allocations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/bank_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     5989 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/contracts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3290 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/powerstation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.471817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/tests/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/tests/test_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.473817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-20 10:15:45.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-04-20 10:15:45.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 10:15:45.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 10:15:45.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      212 2023-04-20 10:15:45.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-20 10:15:45.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 10:15:45.474817 odoo13-addon-photovoltaic_api-13.0.1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/setup.py
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/CHANGELOG.md` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 All notable changes to this project will be documented in this file. (from version 13.0.1.1.0 onwards)
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v13.0.1.1.1] - 20-04-2023
+
+### Fixed
+- Selection of contacts on signup request
+
 ## [v13.0.1.1.0] - 11-04-2023
 
 ### Fixed
 - Incorrect retrieval of account allocations
 - Count of allocations to use correct search domain
 - Naming of company users
 - Location of a user
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/__manifest__.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/__manifest__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': 'Photovoltaic API',
-    'version': '13.0.1.1.0',
+    'version': '13.0.1.1.1',
     'depends': [
         'base_rest',
         'auth_api_key',
         'auth_jwt',
         'base_rest_pydantic',
         'pydantic',
         'photovoltaic_mgmt',
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/data/data.xml` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/data/data.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/__init__.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/contract.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/contract.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/power_station.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/power_station.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/pydantic_models/user.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/user.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/security/ir.model.access.csv` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,21 +21,19 @@
     )
     def signup_request(self, **params):
         '''
         Request to create a user from a partner
         :param vat: VAT
         :return: Signup token
         '''
-        partner = self.env['res.partner'].search([('vat', '=', params.get('vat'))])
+        partner = self.env['res.partner'].search([('vat', '=', params.get('vat')), ('participant', '=', True)])
         if len(partner) < 1:
             raise MissingError('Missing error')
         elif len(partner) > 1:
             raise UserError('Bad request')
-        elif (not partner.participant):
-            raise UserError('User not participant')
             
         expiration = datetime.now() + timedelta(hours=1)
         partner.signup_prepare(expiration=expiration)
         return {
             'token': partner.signup_token,
             'email': partner.email,
             'name':  partner.name
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/allocations.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/allocations.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/bank_account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/bank_account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/contracts.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/contracts.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/info.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/info.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/powerstation.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/powerstation.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/services/user.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from odoo.addons.base_rest import restapi
 from odoo.addons.component.core import Component
 from odoo.exceptions import UserError
 
-
 from ..pydantic_models import false_to_none
 from ..pydantic_models.bank_account import BankAccountOut
 from ..pydantic_models.info import Country, PersonType, State
 from ..pydantic_models.user import UserIn, UserOut, UserShort
 
 
 class UserService(Component):
@@ -30,16 +29,15 @@
     )
     def update(self, user_in):
         duplicated_vat_partners = self.env['res.partner'].sudo().search([('vat', '=', user_in.vat)])
         if user_in.vat and len(duplicated_vat_partners) > 0 and duplicated_vat_partners[0]['id'] != self.env.user.partner_id.id:
             raise UserError('vat already exists')
 
         user_dict = user_in.dict(exclude_unset=True, exclude={'representative', 'interests'})
-
-        if (user_in.zip or user_in.state or user_in.country_id):
+        if (user_in.zip or user_in.state_id or user_in.country_id):
             user_dict['zip_id'] = None
 
         partner = self.env.user.partner_id
         is_login_vat = (partner.vat == self.env.user.login)
         partner.write(user_dict)
 
         if (partner.company_type == 'company' and partner.child_ids and user_in.representative):
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/tests/common.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/tests/common.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo/addons/photovoltaic_api/tests/test_account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/tests/test_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             'vat': VAT
         })
 
         self.assertEqual(len(self.env['res.partner'].search([('vat', '=', VAT)])), 1)
         self.assertEqual(self.env['res.partner'].search([('vat', '=', VAT)])[0].name, NAME)
 
         request = self.http('POST', '/api/account/signup_request', { 'vat': VAT }, { 'api_key': self.api_key })
-        self.assertEqual(request.status_code, 400)
+        self.assertEqual(request.status_code, 404)
 
 
     @mute_logger('odoo.addons.base_rest.http')
     def test_signup_request_correct(self):
         self.env['res.partner'].create({
             'name': NAME,
             'vat': VAT,
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.0/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt` & `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

