# Comparing `tmp/invenio-config-tugraz-0.9.0.tar.gz` & `tmp/invenio-config-tugraz-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-config-tugraz-0.9.0.tar", last modified: Mon May 30 11:39:47 2022, max compression
+gzip compressed data, was "dist/invenio-config-tugraz-0.9.1.tar", last modified: Mon May 30 12:20:39 2022, max compression
```

## Comparing `invenio-config-tugraz-0.9.0.tar` & `invenio-config-tugraz-0.9.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3578 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4609 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7469 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10379 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7011 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2558 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/base_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11517 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/ext.py
--rw-r--r--   0 runner    (1001) docker     (121)     8473 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/generators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/rdm_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/restrictions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/restrictions/access_right/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/restrictions/access_right/access_right.csv
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/restrictions/access_right/access_right_limit.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/
--rw-r--r--   0 runner    (1001) docker     (121)    76674 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_General_Data_Protection_Rights_de.pdf
--rw-r--r--   0 runner    (1001) docker     (121)    24763 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_General_Data_Protection_Rights_en.pdf
--rw-r--r--   0 runner    (1001) docker     (121)   277617 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_01_de.pdf
--rw-r--r--   0 runner    (1001) docker     (121)   308633 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_01_en.pdf
--rw-r--r--   0 runner    (1001) docker     (121)   244668 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_02_de.pdf
--rw-r--r--   0 runner    (1001) docker     (121)   281137 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_02_en.pdf
--rw-r--r--   0 runner    (1001) docker     (121)   112443 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_Terms_And_Conditions_de.pdf
--rw-r--r--   0 runner    (1001) docker     (121)    24939 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_Terms_And_Conditions_en.pdf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/templates/security/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/templates/security/email/
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/templates/security/email/welcome.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/translations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/translations/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/translations/de/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4609 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/invenio_config_tugraz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      853 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 11:39:47.000000 invenio-config-tugraz-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     5095 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-05-30 11:39:36.000000 invenio-config-tugraz-0.9.0/tests/test_invenio_config_tugraz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3578 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     7469 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10379 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7011 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2558 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/base_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11517 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/ext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8473 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/generators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/rdm_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/restrictions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/restrictions/access_right/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/restrictions/access_right/access_right.csv
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/restrictions/access_right/access_right_limit.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/
+-rw-r--r--   0 runner    (1001) docker     (121)    76674 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_General_Data_Protection_Rights_de.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)    24763 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_General_Data_Protection_Rights_en.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)   277617 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_01_de.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)   308633 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_01_en.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)   244668 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_02_de.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)   281137 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_02_en.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)   112443 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_Terms_And_Conditions_de.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)    24939 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_Terms_And_Conditions_en.pdf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/templates/security/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/templates/security/email/
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/templates/security/email/welcome.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/translations/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/translations/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/translations/de/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/invenio_config_tugraz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      853 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 12:20:39.000000 invenio-config-tugraz-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     5095 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2022-05-30 12:20:34.000000 invenio-config-tugraz-0.9.1/tests/test_invenio_config_tugraz.py
```

### Comparing `invenio-config-tugraz-0.9.0/.editorconfig` & `invenio-config-tugraz-0.9.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/.tx/config` & `invenio-config-tugraz-0.9.1/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/CHANGES.rst` & `invenio-config-tugraz-0.9.1/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
     invenio-config-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
+Version 0.9.1 (released 2022-05-30)
+
+- ci(publish): ping babel version (#99)
+
 Version 0.9.0 (released 2022-05-30)
 
 - config: adds new introduced configs v9
 - dep: compatible to v9 rdm
 - config: add deposit form quota variable (#91)
 - migrate setup py to cfg (#94)
 - fix: update email welcome template with SITE_UI_URL (#93)
```

### Comparing `invenio-config-tugraz-0.9.0/CONTRIBUTING.rst` & `invenio-config-tugraz-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/LICENSE` & `invenio-config-tugraz-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/MANIFEST.in` & `invenio-config-tugraz-0.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/PKG-INFO` & `invenio-config-tugraz-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tugraz
-Version: 0.9.0
+Version: 0.9.1
 Summary: "Invenio module that adds tugraz configs."
 Home-page: https://github.com/tu-graz-library/invenio-config-tugraz
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
 Description: ..
             Copyright (C) 2020-2021 Graz University of Technology.
@@ -57,14 +57,18 @@
         
             invenio-config-tugraz is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
+        Version 0.9.1 (released 2022-05-30)
+        
+        - ci(publish): ping babel version (#99)
+        
         Version 0.9.0 (released 2022-05-30)
         
         - config: adds new introduced configs v9
         - dep: compatible to v9 rdm
         - config: add deposit form quota variable (#91)
         - migrate setup py to cfg (#94)
         - fix: update email welcome template with SITE_UI_URL (#93)
```

### Comparing `invenio-config-tugraz-0.9.0/README.rst` & `invenio-config-tugraz-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/babel.ini` & `invenio-config-tugraz-0.9.1/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/docs/Makefile` & `invenio-config-tugraz-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/docs/conf.py` & `invenio-config-tugraz-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/docs/index.rst` & `invenio-config-tugraz-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/docs/make.bat` & `invenio-config-tugraz-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/base_permissions.py` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/base_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/config.py` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/config.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/ext.py` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/generators.py` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/rdm_permissions.py` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/rdm_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_General_Data_Protection_Rights_de.pdf` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_General_Data_Protection_Rights_de.pdf`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_General_Data_Protection_Rights_en.pdf` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_General_Data_Protection_Rights_en.pdf`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_01_de.pdf` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_01_de.pdf`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_01_en.pdf` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_01_en.pdf`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_02_de.pdf` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_02_de.pdf`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_02_en.pdf` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_Guide_02_en.pdf`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_Terms_And_Conditions_de.pdf` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_Terms_And_Conditions_de.pdf`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/static/documents/TUGraz_Repository_Terms_And_Conditions_en.pdf` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/static/documents/TUGraz_Repository_Terms_And_Conditions_en.pdf`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/templates/security/email/welcome.txt` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/templates/security/email/welcome.txt`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/translations/de/LC_MESSAGES/messages.mo` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/translations/de/LC_MESSAGES/messages.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -3,19 +3,19 @@
 "Project-Id-Version: invenio-config-tugraz 0.5.5\n"
 "Report-Msgid-Bugs-To: mojib.wali@tugraz.at\n"
 "POT-Creation-Date: 2021-04-27 15:30+0200\n"
 "PO-Revision-Date: 2021-04-22 11:57+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.1\n"
+"Generated-By: Babel 2.9.1\n"
 
 msgid "Best regards,"
 msgstr "Mit freundlichen Grüßen,"
 
 msgid "Data Protection Rights"
 msgstr "Datenschutzerklärung"
```

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/translations/de/LC_MESSAGES/messages.po` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/translations/messages.pot` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz/views.py` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz/views.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz.egg-info/PKG-INFO` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tugraz
-Version: 0.9.0
+Version: 0.9.1
 Summary: "Invenio module that adds tugraz configs."
 Home-page: https://github.com/tu-graz-library/invenio-config-tugraz
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
 Description: ..
             Copyright (C) 2020-2021 Graz University of Technology.
@@ -57,14 +57,18 @@
         
             invenio-config-tugraz is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
+        Version 0.9.1 (released 2022-05-30)
+        
+        - ci(publish): ping babel version (#99)
+        
         Version 0.9.0 (released 2022-05-30)
         
         - config: adds new introduced configs v9
         - dep: compatible to v9 rdm
         - config: add deposit form quota variable (#91)
         - migrate setup py to cfg (#94)
         - fix: update email welcome template with SITE_UI_URL (#93)
```

### Comparing `invenio-config-tugraz-0.9.0/invenio_config_tugraz.egg-info/SOURCES.txt` & `invenio-config-tugraz-0.9.1/invenio_config_tugraz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/run-tests.sh` & `invenio-config-tugraz-0.9.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/setup.cfg` & `invenio-config-tugraz-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/tests/conftest.py` & `invenio-config-tugraz-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/tests/test_generators.py` & `invenio-config-tugraz-0.9.1/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tugraz-0.9.0/tests/test_invenio_config_tugraz.py` & `invenio-config-tugraz-0.9.1/tests/test_invenio_config_tugraz.py`

 * *Files identical despite different names*

