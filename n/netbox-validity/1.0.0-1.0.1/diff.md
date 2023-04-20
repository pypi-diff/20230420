# Comparing `tmp/netbox-validity-1.0.0.tar.gz` & `tmp/netbox-validity-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-validity-1.0.0.tar", last modified: Wed Apr 19 23:29:21 2023, max compression
+gzip compressed data, was "netbox-validity-1.0.1.tar", last modified: Thu Apr 20 18:36:48 2023, max compression
```

## Comparing `netbox-validity-1.0.0.tar` & `netbox-validity-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:29:21.504277 netbox-validity-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-04-19 23:29:21.504277 netbox-validity-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:29:21.500277 netbox-validity-1.0.0/netbox_validity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-04-19 23:29:21.000000 netbox-validity-1.0.0/netbox_validity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-19 23:29:21.000000 netbox-validity-1.0.0/netbox_validity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:29:21.000000 netbox-validity-1.0.0/netbox_validity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-19 23:29:21.000000 netbox-validity-1.0.0/netbox_validity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 23:29:21.000000 netbox-validity-1.0.0/netbox_validity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:29:21.500277 netbox-validity-1.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:29:21.504277 netbox-validity-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:29:21.500277 netbox-validity-1.0.0/validity/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:29:21.500277 netbox-validity-1.0.0/validity/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:29:21.504277 netbox-validity-1.0.0/validity/templates/validity/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/templates/validity/compliance_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/templates/validity/compliancereport.html
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/templates/validity/complianceselector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/templates/validity/compliancetest.html
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/templates/validity/compliancetestresult.html
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/templates/validity/configserializer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/templates/validity/device_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/templates/validity/gitrepo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:29:21.504277 netbox-validity-1.0.0/validity/templates/validity/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/templates/validity/inc/git_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/templates/validity/inc/path_with_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/templates/validity/inc/report_stats_row.html
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/templates/validity/nameset.html
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-19 23:29:07.000000 netbox-validity-1.0.0/validity/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.380661 netbox-validity-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-20 18:36:48.380661 netbox-validity-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.360661 netbox-validity-1.0.1/netbox_validity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-20 18:36:48.000000 netbox-validity-1.0.1/netbox_validity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-20 18:36:48.000000 netbox-validity-1.0.1/netbox_validity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:36:48.000000 netbox-validity-1.0.1/netbox_validity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-20 18:36:48.000000 netbox-validity-1.0.1/netbox_validity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 18:36:48.000000 netbox-validity-1.0.1/netbox_validity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.364661 netbox-validity-1.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 18:36:48.380661 netbox-validity-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.364661 netbox-validity-1.0.1/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.364661 netbox-validity-1.0.1/validity/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.364661 netbox-validity-1.0.1/validity/config_compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/device_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/dynamic_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.368661 netbox-validity-1.0.1/validity/config_compliance/eval/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/eval/default_nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/eval/eval_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/config_compliance/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.368661 netbox-validity-1.0.1/validity/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/forms/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/forms/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.368661 netbox-validity-1.0.1/validity/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.368661 netbox-validity-1.0.1/validity/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/management/commands/linkscripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.368661 netbox-validity-1.0.1/validity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/migrations/0002_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.368661 netbox-validity-1.0.1/validity/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/models/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.372661 netbox-validity-1.0.1/validity/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/scripts/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/scripts/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.360661 netbox-validity-1.0.1/validity/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.372661 netbox-validity-1.0.1/validity/templates/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/compliance_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/compliancereport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/complianceselector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/compliancetest.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/compliancetestresult.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/configserializer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/device_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/gitrepo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.372661 netbox-validity-1.0.1/validity/templates/validity/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/inc/git_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/inc/path_with_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/inc/report_stats_row.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templates/validity/nameset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.372661 netbox-validity-1.0.1/validity/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/templatetags/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.376661 netbox-validity-1.0.1/validity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.376661 netbox-validity-1.0.1/validity/tests/test_config_compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_config_compliance/test_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_config_compliance/test_dynamic_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_config_compliance/test_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.376661 netbox-validity-1.0.1/validity/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_models/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_models/test_git_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_models/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_models/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_models/test_vdevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.376661 netbox-validity-1.0.1/validity/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_scripts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_scripts/test_run_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.376661 netbox-validity-1.0.1/validity/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_utils/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.376661 netbox-validity-1.0.1/validity/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/utils/password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:48.380661 netbox-validity-1.0.1/validity/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-20 18:36:29.000000 netbox-validity-1.0.1/validity/views/test_result.py
```

### Comparing `netbox-validity-1.0.0/LICENSE` & `netbox-validity-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/PKG-INFO` & `netbox-validity-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 1.0.0
+Version: 1.0.1
 Summary: NetBox plugin for vendor-agnostic configuration compliance
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -72,19 +72,20 @@
 ## Why?
 Configuration compliance is one of the very common problems that arises in every company with the growth of their network. Usually companies solve this problem with some kind of scripts that do all the things at the same time: they parse configs, apply some compliance logic and push the results into some DB or third-party OSS system. Usually after the addition of several vendors (or even several software revisions of one model) these scripts become unreadable and almost no one can definitely say which rules the script checks for.
 
 Validity completely separates compliance test code from all other things like config serialization. This one encourages you to write short, clean and understandable compliance tests together with the mandatory description.
 
 
 ## Key features
+* Truly vendor-agnostic. You can easily integrate any vendor config format using [TTP](https://github.com/dmulyalin/ttp)
 * Writing compliance tests using Python expressions and [JQ](https://stedolan.github.io/jq/manual/)
 * Flexible selector system to apply the tests only to a specific subset of devices
 * Concept of **dynamic pairs**. With dynamic pair you can compare 2 different devices between each other (e.g. compare the configuration of 2 MC-LAG members).
-* **Test result explanation**. When some test fails, you can get the **explanation** of the calculation process step by step.
-* **ORM access** inside the test. You have full access to the **device** properties. For instance, you may leverage [Configuration Contexts](https://docs.netbox.dev/en/stable/features/context-data/) NetBox feature to store your desired configuration and compare it with the config collected from device.
+* **Test result explanation**. When some test fails, you can get the **explanation** of the calculation process step by step. It helps to identify the cause of the failure.
+* **ORM access** inside the test. You have full access to the **device** properties. For instance, you may leverage [Configuration Contexts](https://docs.netbox.dev/en/stable/features/context-data/) NetBox feature to store your desired configuration and compare it with the config collected from the device.
 * **Reports and webhooks**. After execution of some bunch of tests you can get the report with passed/failed statistics grouped by some Location/Site/Manufacturer/etc. Moreover, you can provision the webhook to notify an external system when compliance report is generated.
 * **Test extensibility**. You can define your own python functions or classes to reuse the code between multiple compliance tests.
 * Possibility to store all heavy text-based entities (like compliance tests or TTP Templates) in a **Git repository**
 <!--mkdocs-end-->
 
 ## Documentation
 Read the full documentation on [validity.readthedocs.io](https://validity.readthedocs.io)
```

### Comparing `netbox-validity-1.0.0/README.md` & `netbox-validity-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 ## Why?
 Configuration compliance is one of the very common problems that arises in every company with the growth of their network. Usually companies solve this problem with some kind of scripts that do all the things at the same time: they parse configs, apply some compliance logic and push the results into some DB or third-party OSS system. Usually after the addition of several vendors (or even several software revisions of one model) these scripts become unreadable and almost no one can definitely say which rules the script checks for.
 
 Validity completely separates compliance test code from all other things like config serialization. This one encourages you to write short, clean and understandable compliance tests together with the mandatory description.
 
 
 ## Key features
+* Truly vendor-agnostic. You can easily integrate any vendor config format using [TTP](https://github.com/dmulyalin/ttp)
 * Writing compliance tests using Python expressions and [JQ](https://stedolan.github.io/jq/manual/)
 * Flexible selector system to apply the tests only to a specific subset of devices
 * Concept of **dynamic pairs**. With dynamic pair you can compare 2 different devices between each other (e.g. compare the configuration of 2 MC-LAG members).
-* **Test result explanation**. When some test fails, you can get the **explanation** of the calculation process step by step.
-* **ORM access** inside the test. You have full access to the **device** properties. For instance, you may leverage [Configuration Contexts](https://docs.netbox.dev/en/stable/features/context-data/) NetBox feature to store your desired configuration and compare it with the config collected from device.
+* **Test result explanation**. When some test fails, you can get the **explanation** of the calculation process step by step. It helps to identify the cause of the failure.
+* **ORM access** inside the test. You have full access to the **device** properties. For instance, you may leverage [Configuration Contexts](https://docs.netbox.dev/en/stable/features/context-data/) NetBox feature to store your desired configuration and compare it with the config collected from the device.
 * **Reports and webhooks**. After execution of some bunch of tests you can get the report with passed/failed statistics grouped by some Location/Site/Manufacturer/etc. Moreover, you can provision the webhook to notify an external system when compliance report is generated.
 * **Test extensibility**. You can define your own python functions or classes to reuse the code between multiple compliance tests.
 * Possibility to store all heavy text-based entities (like compliance tests or TTP Templates) in a **Git repository**
 <!--mkdocs-end-->
 
 ## Documentation
 Read the full documentation on [validity.readthedocs.io](https://validity.readthedocs.io)
```

### Comparing `netbox-validity-1.0.0/netbox_validity.egg-info/PKG-INFO` & `netbox-validity-1.0.1/netbox_validity.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 1.0.0
+Version: 1.0.1
 Summary: NetBox plugin for vendor-agnostic configuration compliance
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -72,19 +72,20 @@
 ## Why?
 Configuration compliance is one of the very common problems that arises in every company with the growth of their network. Usually companies solve this problem with some kind of scripts that do all the things at the same time: they parse configs, apply some compliance logic and push the results into some DB or third-party OSS system. Usually after the addition of several vendors (or even several software revisions of one model) these scripts become unreadable and almost no one can definitely say which rules the script checks for.
 
 Validity completely separates compliance test code from all other things like config serialization. This one encourages you to write short, clean and understandable compliance tests together with the mandatory description.
 
 
 ## Key features
+* Truly vendor-agnostic. You can easily integrate any vendor config format using [TTP](https://github.com/dmulyalin/ttp)
 * Writing compliance tests using Python expressions and [JQ](https://stedolan.github.io/jq/manual/)
 * Flexible selector system to apply the tests only to a specific subset of devices
 * Concept of **dynamic pairs**. With dynamic pair you can compare 2 different devices between each other (e.g. compare the configuration of 2 MC-LAG members).
-* **Test result explanation**. When some test fails, you can get the **explanation** of the calculation process step by step.
-* **ORM access** inside the test. You have full access to the **device** properties. For instance, you may leverage [Configuration Contexts](https://docs.netbox.dev/en/stable/features/context-data/) NetBox feature to store your desired configuration and compare it with the config collected from device.
+* **Test result explanation**. When some test fails, you can get the **explanation** of the calculation process step by step. It helps to identify the cause of the failure.
+* **ORM access** inside the test. You have full access to the **device** properties. For instance, you may leverage [Configuration Contexts](https://docs.netbox.dev/en/stable/features/context-data/) NetBox feature to store your desired configuration and compare it with the config collected from the device.
 * **Reports and webhooks**. After execution of some bunch of tests you can get the report with passed/failed statistics grouped by some Location/Site/Manufacturer/etc. Moreover, you can provision the webhook to notify an external system when compliance report is generated.
 * **Test extensibility**. You can define your own python functions or classes to reuse the code between multiple compliance tests.
 * Possibility to store all heavy text-based entities (like compliance tests or TTP Templates) in a **Git repository**
 <!--mkdocs-end-->
 
 ## Documentation
 Read the full documentation on [validity.readthedocs.io](https://validity.readthedocs.io)
```

### Comparing `netbox-validity-1.0.0/pyproject.toml` & `netbox-validity-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-validity"
-version = "1.0.0"
+version = "1.0.1"
 description = "NetBox plugin for vendor-agnostic configuration compliance"
 authors = [
     {name = "Anton Miasnikov", email = "anton2008m@gmail.com"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -32,15 +32,15 @@
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 
 [tool.setuptools.packages.find]
-include = ["validity"]
+include = ["validity*"]
 
 [tool.setuptools.package-data]
 validity = ["*.html"]
 
 [tool.setuptools.dynamic.dependencies]
 file = ["requirements/base.txt"]
```

### Comparing `netbox-validity-1.0.0/validity/__init__.py` & `netbox-validity-1.0.1/validity/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class NetBoxValidityConfig(PluginConfig):
     name = "validity"
     verbose_name = "Validity: Configuration Compliance"
     description = "Vendor-agnostic framework to build your own configuration compliance rule set"
     author = "Anton Miasnikov"
     author_email = "anton2008m@gmail.com"
-    version = "1.0.0"
+    version = "1.0.1"
     base_url = "validity"
     django_apps = ["bootstrap5"]
 
     def ready(self):
         try:
             os.makedirs(settings.git_folder, exist_ok=True)
         except OSError as e:
```

### Comparing `netbox-validity-1.0.0/validity/choices.py` & `netbox-validity-1.0.1/validity/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/filtersets.py` & `netbox-validity-1.0.1/validity/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/managers.py` & `netbox-validity-1.0.1/validity/managers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/navigation.py` & `netbox-validity-1.0.1/validity/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/tables.py` & `netbox-validity-1.0.1/validity/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/templates/validity/compliance_results.html` & `netbox-validity-1.0.1/validity/templates/validity/compliance_results.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/templates/validity/compliancereport.html` & `netbox-validity-1.0.1/validity/templates/validity/compliancereport.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/templates/validity/complianceselector.html` & `netbox-validity-1.0.1/validity/templates/validity/complianceselector.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/templates/validity/compliancetest.html` & `netbox-validity-1.0.1/validity/templates/validity/compliancetest.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/templates/validity/compliancetestresult.html` & `netbox-validity-1.0.1/validity/templates/validity/compliancetestresult.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/templates/validity/configserializer.html` & `netbox-validity-1.0.1/validity/templates/validity/configserializer.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/templates/validity/device_config.html` & `netbox-validity-1.0.1/validity/templates/validity/device_config.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/templates/validity/gitrepo.html` & `netbox-validity-1.0.1/validity/templates/validity/gitrepo.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/templates/validity/nameset.html` & `netbox-validity-1.0.1/validity/templates/validity/nameset.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.0.0/validity/urls.py` & `netbox-validity-1.0.1/validity/urls.py`

 * *Files identical despite different names*

