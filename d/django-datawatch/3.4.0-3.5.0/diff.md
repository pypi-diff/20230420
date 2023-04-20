# Comparing `tmp/django-datawatch-3.4.0.tar.gz` & `tmp/django-datawatch-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-datawatch-3.4.0.tar", last modified: Wed Apr 19 16:22:20 2023, max compression
+gzip compressed data, was "django-datawatch-3.5.0.tar", last modified: Thu Apr 20 14:56:55 2023, max compression
```

## Comparing `django-datawatch-3.4.0.tar` & `django-datawatch-3.5.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.619444 django-datawatch-3.4.0/django_datawatch/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/backends/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/backends/synchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/common/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/datawatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.619444 django-datawatch-3.4.0/django_datawatch/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.619444 django-datawatch-3.4.0/django_datawatch/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/management/commands/datawatch_clean_up.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/management/commands/datawatch_list_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/management/commands/datawatch_refresh_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/management/commands/datawatch_run_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/migrations/0002_auto_20180807_1508.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/migrations/0003_resultstatushistory.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/querysets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.619444 django-datawatch-3.4.0/django_datawatch/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/templatetags/class_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tests/test_base_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tests/test_post_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/tests/test_trigger_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/django_datawatch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:22:20.623444 django-datawatch-3.4.0/django_datawatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-19 16:22:20.000000 django-datawatch-3.4.0/django_datawatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-19 16:22:20.000000 django-datawatch-3.4.0/django_datawatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:22:20.000000 django-datawatch-3.4.0/django_datawatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-19 16:22:20.000000 django-datawatch-3.4.0/django_datawatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 16:22:20.000000 django-datawatch-3.4.0/django_datawatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-19 16:22:20.627444 django-datawatch-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-19 16:22:17.000000 django-datawatch-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.706883 django-datawatch-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-04-20 14:56:55.706883 django-datawatch-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.698883 django-datawatch-3.5.0/django_datawatch/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.702883 django-datawatch-3.5.0/django_datawatch/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/backends/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/backends/synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.702883 django-datawatch-3.5.0/django_datawatch/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/common/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/datawatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.686883 django-datawatch-3.5.0/django_datawatch/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.686883 django-datawatch-3.5.0/django_datawatch/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.702883 django-datawatch-3.5.0/django_datawatch/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.702883 django-datawatch-3.5.0/django_datawatch/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.702883 django-datawatch-3.5.0/django_datawatch/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/management/commands/datawatch_clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/management/commands/datawatch_list_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/management/commands/datawatch_refresh_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/management/commands/datawatch_run_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.702883 django-datawatch-3.5.0/django_datawatch/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/migrations/0002_auto_20180807_1508.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/migrations/0003_resultstatushistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/querysets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.686883 django-datawatch-3.5.0/django_datawatch/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.706883 django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.706883 django-datawatch-3.5.0/django_datawatch/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/templatetags/class_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.706883 django-datawatch-3.5.0/django_datawatch/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tests/test_base_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tests/test_post_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tests/test_trigger_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.698883 django-datawatch-3.5.0/django_datawatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-04-20 14:56:55.000000 django-datawatch-3.5.0/django_datawatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-20 14:56:55.000000 django-datawatch-3.5.0/django_datawatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:56:55.000000 django-datawatch-3.5.0/django_datawatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 14:56:55.000000 django-datawatch-3.5.0/django_datawatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 14:56:55.000000 django-datawatch-3.5.0/django_datawatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-20 14:56:55.706883 django-datawatch-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/setup.py
```

### Comparing `django-datawatch-3.4.0/LICENSE` & `django-datawatch-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/PKG-INFO` & `django-datawatch-3.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: django-datawatch
-Version: 3.4.0
+Version: 3.5.0
 Summary: Django Datawatch runs automated data checks in your Django installation
 Home-page: https://github.com/RegioHelden/django-datawatch
 Download-URL: 
 Author: Jens Nistler <opensource@jensnistler.de>, Bogdan Radko <bogdan.radko@regiohelden.de>
 Author-email: opensource@regiohelden.de
 License: MIT
 Keywords: django,monitoring,datawatch,check,checks
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -206,83 +207,83 @@
 Datawatch supported setting a specific queue in release < 0.4.0
 
 With the switch to celery 4, you should use task routing to define the queue for your tasks, see http://docs.celeryproject.org/en/latest/userguide/routing.html
 
 # CONTRIBUTE
 
 ## Dev environment
-- docker (at least 17.12.0+)
-- docker-compose (at least 1.18.0)
+- [Docker](https://docs.docker.com/) (19.03.0 or later)
+- [Compose plugin for Docker](https://docs.docker.com/compose/install/linux/)
 
 Please make sure that no other container is using port 8000 as this is the one you're install gets exposed to:
 http://localhost:8000/
 
 ## Setup
 
 We've included an example app to show how django_datawatch works.
 Start by launching the included docker container.
 ```bash
-docker-compose up -d
+docker compose up -d
 ```
 
 Then setup the example app environment.
 ```bash
-docker-compose run --rm app migrate
-docker-compose run --rm app loaddata example
+docker compose run --rm app migrate
+docker compose run --rm app loaddata example
 ```
 The installed superuser is "example" with password "datawatch".
 
 ## Run checks
 
 Open http://localhost:8000/, log in and then go back to http://localhost:8000/.
 You'll be prompted with an empty dashboard. That's because we didn't run any checks yet.
 Let's enqueue an update.
 ```bash
-docker-compose run --rm app datawatch_run_checks --force
+docker compose run --rm app datawatch_run_checks --force
 ```
 
 The checks for the example app are run synchronously and should be updated immediately.
 If you decide to switch to the celery backend, you should now start a celery worker to process the checks.
 ```bash
-docker-compose run --rm --entrypoint celery app -A example worker -l DEBUG
+docker compose run --rm --entrypoint celery app -A example worker -l DEBUG
 ```
 
 To execute the celery beat scheduler which runs the datawatch scheduler every minute, just run:
 ```bash
-docker-compose run --rm --entrypoint celery app -A example  beat --scheduler django_celery_beat.schedulers:DatabaseScheduler
+docker compose run --rm --entrypoint celery app -A example  beat --scheduler django_celery_beat.schedulers:DatabaseScheduler
 ```
 
 You will see some failed check now after you refreshed the dashboard view.
 
 ![Django Datawatch dashboard](http://static.jensnistler.de/django_datawatch.png "Django Datawatch dashboard")
 
 ## Run the tests
 ```bash
-docker-compose run --rm app test
+docker compose run --rm app test
 ```
 
 ## Requirements upgrades
 
 Check for upgradeable packages by running 
 ```bash
-docker-compose up -d
-docker-compose exec app pip-check
+docker compose up -d
+docker compose exec app pip-check
 ```
 
 ## Translations
 
 Collect and compile translations for all registered locales
 
 ```bash
-docker-compose run --rm app makemessages --no-location --all
-docker-compose run --rm app compilemessages
+docker compose run --rm app makemessages --no-location --all
+docker compose run --rm app compilemessages
 ```
 
 ## Making a new release
 
 [bumpversion](https://github.com/peritus/bumpversion) is used to manage releases.
 
 Add your changes to the [CHANGELOG](./CHANGELOG.rst), run
 ```bash
-docker-compose exec app bumpversion <major|minor|patch>
+docker compose exec app bumpversion <major|minor|patch>
 ```
 then push (including tags).
```

### Comparing `django-datawatch-3.4.0/README.md` & `django-datawatch-3.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -180,83 +180,83 @@
 Datawatch supported setting a specific queue in release < 0.4.0
 
 With the switch to celery 4, you should use task routing to define the queue for your tasks, see http://docs.celeryproject.org/en/latest/userguide/routing.html
 
 # CONTRIBUTE
 
 ## Dev environment
-- docker (at least 17.12.0+)
-- docker-compose (at least 1.18.0)
+- [Docker](https://docs.docker.com/) (19.03.0 or later)
+- [Compose plugin for Docker](https://docs.docker.com/compose/install/linux/)
 
 Please make sure that no other container is using port 8000 as this is the one you're install gets exposed to:
 http://localhost:8000/
 
 ## Setup
 
 We've included an example app to show how django_datawatch works.
 Start by launching the included docker container.
 ```bash
-docker-compose up -d
+docker compose up -d
 ```
 
 Then setup the example app environment.
 ```bash
-docker-compose run --rm app migrate
-docker-compose run --rm app loaddata example
+docker compose run --rm app migrate
+docker compose run --rm app loaddata example
 ```
 The installed superuser is "example" with password "datawatch".
 
 ## Run checks
 
 Open http://localhost:8000/, log in and then go back to http://localhost:8000/.
 You'll be prompted with an empty dashboard. That's because we didn't run any checks yet.
 Let's enqueue an update.
 ```bash
-docker-compose run --rm app datawatch_run_checks --force
+docker compose run --rm app datawatch_run_checks --force
 ```
 
 The checks for the example app are run synchronously and should be updated immediately.
 If you decide to switch to the celery backend, you should now start a celery worker to process the checks.
 ```bash
-docker-compose run --rm --entrypoint celery app -A example worker -l DEBUG
+docker compose run --rm --entrypoint celery app -A example worker -l DEBUG
 ```
 
 To execute the celery beat scheduler which runs the datawatch scheduler every minute, just run:
 ```bash
-docker-compose run --rm --entrypoint celery app -A example  beat --scheduler django_celery_beat.schedulers:DatabaseScheduler
+docker compose run --rm --entrypoint celery app -A example  beat --scheduler django_celery_beat.schedulers:DatabaseScheduler
 ```
 
 You will see some failed check now after you refreshed the dashboard view.
 
 ![Django Datawatch dashboard](http://static.jensnistler.de/django_datawatch.png "Django Datawatch dashboard")
 
 ## Run the tests
 ```bash
-docker-compose run --rm app test
+docker compose run --rm app test
 ```
 
 ## Requirements upgrades
 
 Check for upgradeable packages by running 
 ```bash
-docker-compose up -d
-docker-compose exec app pip-check
+docker compose up -d
+docker compose exec app pip-check
 ```
 
 ## Translations
 
 Collect and compile translations for all registered locales
 
 ```bash
-docker-compose run --rm app makemessages --no-location --all
-docker-compose run --rm app compilemessages
+docker compose run --rm app makemessages --no-location --all
+docker compose run --rm app compilemessages
 ```
 
 ## Making a new release
 
 [bumpversion](https://github.com/peritus/bumpversion) is used to manage releases.
 
 Add your changes to the [CHANGELOG](./CHANGELOG.rst), run
 ```bash
-docker-compose exec app bumpversion <major|minor|patch>
+docker compose exec app bumpversion <major|minor|patch>
 ```
 then push (including tags).
```

### Comparing `django-datawatch-3.4.0/django_datawatch/admin.py` & `django-datawatch-3.5.0/django_datawatch/admin.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/backends/celery.py` & `django-datawatch-3.5.0/django_datawatch/backends/celery.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/backends/synchronous.py` & `django-datawatch-3.5.0/django_datawatch/backends/synchronous.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/base.py` & `django-datawatch-3.5.0/django_datawatch/base.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/common/views.py` & `django-datawatch-3.5.0/django_datawatch/common/views.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/datawatch.py` & `django-datawatch-3.5.0/django_datawatch/datawatch.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/forms.py` & `django-datawatch-3.5.0/django_datawatch/forms.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/locale/de/LC_MESSAGES/django.mo` & `django-datawatch-3.5.0/django_datawatch/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/locale/de/LC_MESSAGES/django.po` & `django-datawatch-3.5.0/django_datawatch/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/management/commands/datawatch_refresh_results.py` & `django-datawatch-3.5.0/django_datawatch/management/commands/datawatch_refresh_results.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/management/commands/datawatch_run_checks.py` & `django-datawatch-3.5.0/django_datawatch/management/commands/datawatch_run_checks.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/migrations/0001_initial.py` & `django-datawatch-3.5.0/django_datawatch/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/migrations/0002_auto_20180807_1508.py` & `django-datawatch-3.5.0/django_datawatch/migrations/0002_auto_20180807_1508.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/migrations/0003_resultstatushistory.py` & `django-datawatch-3.5.0/django_datawatch/migrations/0003_resultstatushistory.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/models.py` & `django-datawatch-3.5.0/django_datawatch/models.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/querysets.py` & `django-datawatch-3.5.0/django_datawatch/querysets.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/tasks.py` & `django-datawatch-3.5.0/django_datawatch/tasks.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/base.html` & `django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/base.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 {% load i18n %}
 
 <!DOCTYPE html>
 <html>
+
 <head lang="en">
     <meta charset="UTF-8">
     <title>Django Datawatch</title>
-    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
+    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous">
 </head>
+
 <body>
-    <nav class="navbar navbar-default">
+    <nav class="navbar navbar-expand-lg bg-light">
         <div class="container-fluid">
-            <div class="navbar-header">
-                <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar"
-                        aria-expanded="false" aria-controls="navbar">
-                    <span class="sr-only">Toggle navigation</span>
-                    <span class="icon-bar"></span>
-                    <span class="icon-bar"></span>
-                    <span class="icon-bar"></span>
-                </button>
-                <a class="navbar-brand" href="{% url "django_datawatch_index" %}">Django Datawatch</a>
-            </div>
-            <div id="navbar" class="navbar-collapse collapse">
-                <ul class="nav navbar-nav">
-                    <li class="active"><a href="{% url "django_datawatch_index" %}">{% trans "Home" %}</a></li>
+            <a class="navbar-brand" href="{% url "django_datawatch_index" %}">Django Datawatch</a>
+            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
+                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
+                <span class="navbar-toggler-icon"></span>
+            </button>
+            <div class="collapse navbar-collapse" id="navbarNav">
+                <ul class="navbar-nav">
+                    <li class="nav-item">
+                        <a class="nav-link active" aria-current="page" href="{% url "django_datawatch_index" %}">{% trans "Home" %}</a>
+                    </li>
                 </ul>
             </div>
         </div>
     </nav>
 
-    <div class="container">
+    <div class="container mt-2">
         {% if messages %}
             {% for message in messages %}
-                <div id="messageframework" class="alert alert-block {% if 'debug' in message.tags or 'info' in message.tags %}alert-info{% elif 'success' in message.tags %}alert-success{% elif 'error' in message.tags %}alert-danger{% elif 'warning' in message.tags %}alert-warning{% endif %}">
-                    <strong>
-                        {% if 'debug' in message.tags %}
-                            {% trans 'DEBUG' %}
-                        {% elif 'info' in message.tags %}
-                            {% trans 'Info' %}
-                        {% elif 'success' in message.tags %}
-                            {% trans 'Success' %}
-                        {% elif 'error' in message.tags %}
-                            {% trans 'Error' %}
-                        {% else %}
-                            {% trans 'Warning' %}
-                        {% endif %}
-                    </strong>
-                    <p>
+                <div class="card mb-4 {% if 'debug' in message.tags or 'info' in message.tags %}text-bg-info{% elif 'success' in message.tags %}text-bg-success{% elif 'error' in message.tags %}text-bg-danger{% elif 'warning' in message.tags %}text-bg-warning{% endif %}">
+                    <div class="card-header">
+                        <h5 class="card-title pt-2">
+                            {% if 'debug' in message.tags %}
+                                {% trans 'DEBUG' %}
+                            {% elif 'info' in message.tags %}
+                                {% trans 'Info' %}
+                            {% elif 'success' in message.tags %}
+                                {% trans 'Success' %}
+                            {% elif 'error' in message.tags %}
+                                {% trans 'Error' %}
+                            {% else %}
+                                {% trans 'Warning' %}
+                            {% endif %}
+                        </h5>
+                    </div>
+                    <div class="card-body">
                         {% if 'safe' in message.tags %}
                             {{ message|safe }}
                         {% else %}
                             {{ message }}
                         {% endif %}
-                    </p>
+                    </div>
                 </div>
             {% endfor %}
         {% endif %}
 
         {% block django_datawatch %}{% endblock %}
     </div>
+
+    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-kenU1KFdBIe4zVF0s0G1M5b4hcpxyD9F7jL+jjXkk+Q2h455rYXK/7HAuoJl+0I4" crossorigin="anonymous"></script>
 </body>
-</html>
+
+</html>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% load i18n %}
- Toggle navigation
  %}">Django Datawatch
+
     *  %}">{% trans "Home" %}
 {% if messages %} {% for message in messages %}
-{% if 'debug' in message.tags %} {% trans 'DEBUG' %} {% elif 'info' in
+** {% if 'debug' in message.tags %} {% trans 'DEBUG' %} {% elif 'info' in
 message.tags %} {% trans 'Info' %} {% elif 'success' in message.tags %} {%
 trans 'Success' %} {% elif 'error' in message.tags %} {% trans 'Error' %} {%
-else %} {% trans 'Warning' %} {% endif %}
+else %} {% trans 'Warning' %} {% endif %} **
 {% if 'safe' in message.tags %} {{ message|safe }} {% else %} {{ message }} {%
 endif %}
 {% endfor %} {% endif %} {% block django_datawatch %}{% endblock %}
```

### Comparing `django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/dashboard.html` & `django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/dashboard.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 {% extends "django_datawatch/base.html" %}
 {% load i18n %}
-{% load bootstrap3 %}
+{% load django_bootstrap5 %}
 
 {% block django_datawatch %}
-    <div class="row">
-        <div class="col-md-12">
-            <div class="panel panel-default">
-                <div class="panel-heading">
-                    <h3 class="panel-title">{% trans "Filter" %}</h3>
-                </div>
-                <div class="panel-body">
-                    <form method="get" class="form-horizontal">
-                        {% bootstrap_form form layout='horizontal' %}
-                        {% buttons %}
-                            <div class="col-sm-offset-2 col-sm-10">
-                                {% trans "Filter" as trans_filter %}
-                                {% bootstrap_button trans_filter button_type="submit" button_class="btn-primary" %}
-                            </div>
-                        {% endbuttons %}
-                    </form>
-                </div>
+    <div class="card mb-4">
+        <div class="card-body">
+            <h5 class="card-title">{% trans "Filter" %}</h5>
+            <div>
+                <form method="get" class="form-horizontal">
+                    {% bootstrap_form form layout='horizontal' %}
+                    <div class="offset-md-2 col-md-10">
+                        {% trans "Filter" as trans_filter %}
+                        {% bootstrap_button trans_filter button_type="submit" button_class="btn-primary" %}
+                    </div>
+                </form>
             </div>
         </div>
     </div>
 
     {% regroup results by get_status_display as status_list %}
-    <div class="row">
+    <div class="row mb-4">
         {% if not status_list %}
             <div class="col-md-12">
                 <div class="alert alert-info text-center">
                     <h3>{% trans "There is nothing to see here. Everything is fine!" %}</h3>
                 </div>
             </div>
         {% else %}
@@ -48,15 +42,15 @@
             {% endfor %}
         {% endif %}
     </div>
 
     <div class="row">
         <div class="col-md-12">
             {% for status in status_list %}
-                <h1 id="status-{{ status.grouper|slugify }}">{{ status.grouper }}</h1>
+                <h3 id="status-{{ status.grouper|slugify }}">{{ status.grouper }}</h3>
 
                 <table class="table table-bordered">
                     {% for result in status.list %}
                         <tr>
                             <td style="width: 20%;">
                                 <span class="label label-{% if result.status == result.STATUS.critical %}danger{% elif result.status == result.STATUS.warning %}warning{% elif result.status == result.STATUS.ok %}success{% endif %}">{{ result.get_status_display }}</span>
                                 {% if result.is_acknowledged %}
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-{% extends "django_datawatch/base.html" %} {% load i18n %} {% load bootstrap3
-%} {% block django_datawatch %}
-**** {% trans "Filter" %} ****
-{% bootstrap_form form layout='horizontal' %} {% buttons %}
+{% extends "django_datawatch/base.html" %} {% load i18n %} {% load
+django_bootstrap5 %} {% block django_datawatch %}
+** {% trans "Filter" %} **
+{% bootstrap_form form layout='horizontal' %}
 {% trans "Filter" as trans_filter %} {% bootstrap_button trans_filter
 button_type="submit" button_class="btn-primary" %}
-{% endbuttons %}
 {% regroup results by get_status_display as status_list %}
 {% if not status_list %}
 **** {% trans "There is nothing to see here. Everything is fine!" %} ****
 {% else %} {% widthratio 12 status_list|length 1 as size %} {% for status in
 status_list %} {% for status_definition in results.get_stats %} {% if
 status.grouper == status_definition.status_name %}
 {{_status_definition.status_name_}}
 ****_{{_status_definition.amount_}}_****
 {% endif %} {% endfor %} {% endfor %} {% endif %}
 {% for status in status_list %}
-****** {{ status.grouper }} ******
+**** {{ status.grouper }} ****
 {{ result.get_status_display }} {%                                      {
 if result.is_acknowledged %}         pk=result.pk %}"> {                {
 {% blocktrans with                  {                                   result.payload_description|linebreaksbr
 date=result.acknowledged_until|date result.get_check_instance.get_title }} {
 %}Acknowledged until {{ date }}{%   }}                                  {
 endblocktrans %} {% endif %}                                            result.get_formatted_data|linebreaksbr
                                                                         }}
```

### Comparing `django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/detail.html` & `django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/detail.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 {% extends "django_datawatch/base.html" %}
 {% load i18n class_name %}
 
 {% block django_datawatch %}
     {% with check_instance=result.get_check_instance %}
         <div class="row">
             <div class="col-md-12">
-                <div class="panel {% if result.status == result.STATUS.critical %}panel-danger{% elif result.status == result.STATUS.warning %}panel-warning{% elif result.status == result.STATUS.ok %}panel-success{% else %}panel-default{% endif %}">
-                    <div class="panel-heading">
-                        <div class="panel-title">
-                            <h3>{{ result.get_status_display }} - {{ check_instance.get_title }}</h3>
-                        </div>
+                <div class="card">
+                    <div class="card-header {% if result.status == result.STATUS.critical %}text-bg-danger{% elif result.status == result.STATUS.warning %}text-bg-warning{% elif result.status == result.STATUS.ok %}text-bg-success{% else %}panel-default{% endif %}">
+                        <h5 class="card-title pt-2">{{ result.get_status_display }} - {{ check_instance.get_title }}</h5>
                     </div>
-                    <div class="panel-body">
+                    <div class="card-body">
                         <div class="row">
                             <div class="col-md-8">
                                 <h3>{{ result.payload_description }}</h3>
                             </div>
-                            <div class="col-md-4 text-right">
+                            <div class="col-md-4 text-end">
                                 {% if perms.django_datawatch.acknowledge %}
                                     <a href="{% url "django_datawatch_result_acknowledge" pk=result.pk %}">{% trans "Acknowledge" %}</a><br>
                                 {% endif %}
                                 {% if perms.django_datawatch.config and check_instance.get_form_class %}
                                     <a href="{% url "django_datawatch_result_config" pk=result.pk %}">{% trans "Change config" %}</a><br>
                                 {% endif %}
                                 {% if perms.django_datawatch.refresh %}
@@ -128,17 +126,16 @@
                                         <p>
                                             <strong>{% trans "Reason:" %}</strong> {{ result.acknowledged_reason }}
                                         </p>
                                     </div>
                                 </div>
                             </div>
                         {% endif %}
-                        <div class="row">
+                        <div class="row mt-4">
                             <div class="col-md-12">
-                                <hr>
                                 {% block django_datawatch_check %}{% endblock %}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "django_datawatch/base.html" %} {% load i18n class_name %} {% block
 django_datawatch %} {% with check_instance=result.get_check_instance %}
-**** {{ result.get_status_display }} - {{ check_instance.get_title }} ****
+** {{ result.get_status_display }} - {{ check_instance.get_title }} **
 **** {{ result.payload_description }} ****
 {% if perms.django_datawatch.acknowledge %}
  pk=result.pk %}">{% trans "Acknowledge" %}
 
 {% endif %} {% if perms.django_datawatch.config and
 check_instance.get_form_class %}
  pk=result.pk %}">{% trans "Change config" %}
@@ -42,10 +42,9 @@
                                     trans "Not set" %} {% endif %}
 {% endif %} {% if result.is_acknowledged %}
 {% blocktrans with date=result.acknowledged_until|date
 user=result.acknowledged_by %}Acknowledged until {{ date }} by {{ user }}{%
 endblocktrans %}
 {% trans "Reason:" %} {{ result.acknowledged_reason }}
 {% endif %}
-===============================================================================
 {% block django_datawatch_check %}{% endblock %}
 {% endwith %} {% endblock %}
```

### Comparing `django-datawatch-3.4.0/django_datawatch/templates/django_datawatch/form.html` & `django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/form.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 {% extends "django_datawatch/base.html" %}
 {% load i18n %}
-{% load bootstrap3 %}
+{% load django_bootstrap5 %}
 
 {% block django_datawatch %}
-    <div class="row">
-        <div class="col-md-12">
-            <div class="panel panel-default">
-                <div class="panel-heading">
-                    <h3 class="panel-title">{% trans "Filter" %}</h3>
-                </div>
-                <div class="panel-body">
+    <div class="container mt-2 mb-4">
+        <div class="card">
+            <div class="card-body">
+                <div>
                     <form method="post" class="form-horizontal">
                         {% csrf_token %}
                         {% bootstrap_form form layout='horizontal' %}
-                        {% buttons %}
-                            <div class="col-sm-offset-2 col-sm-10">
-                                {% bootstrap_button action button_type="submit" button_class="btn-primary" %}
-                                &#160;
-                                <a href="javascript:history.back();">{% trans "Cancel" %}</a>
-                            </div>
-                        {% endbuttons %}
+                        <div class="offset-md-2 col-md-10">
+                            {% bootstrap_button action button_type="submit" button_class="btn-primary" %}
+                            &#160;
+                            <a href="javascript:history.back();">{% trans "Cancel" %}</a>
+                        </div>
                     </form>
                 </div>
             </div>
         </div>
     </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,6 @@
-{% extends "django_datawatch/base.html" %} {% load i18n %} {% load bootstrap3
-%} {% block django_datawatch %}
-**** {% trans "Filter" %} ****
-{% csrf_token %} {% bootstrap_form form layout='horizontal' %} {% buttons %}
+{% extends "django_datawatch/base.html" %} {% load i18n %} {% load
+django_bootstrap5 %} {% block django_datawatch %}
+{% csrf_token %} {% bootstrap_form form layout='horizontal' %}
 {% bootstrap_button action button_type="submit" button_class="btn-primary" %}  
 {%_trans_"Cancel"_%}
-{% endbuttons %}
 {% endblock %}
```

### Comparing `django-datawatch-3.4.0/django_datawatch/tests/test_base_check.py` & `django-datawatch-3.5.0/django_datawatch/tests/test_base_check.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/tests/test_integration.py` & `django-datawatch-3.5.0/django_datawatch/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/tests/test_post_delete.py` & `django-datawatch-3.5.0/django_datawatch/tests/test_post_delete.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/tests/test_scheduler.py` & `django-datawatch-3.5.0/django_datawatch/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/tests/test_trigger_update.py` & `django-datawatch-3.5.0/django_datawatch/tests/test_trigger_update.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/urls.py` & `django-datawatch-3.5.0/django_datawatch/urls.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch/views.py` & `django-datawatch-3.5.0/django_datawatch/views.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/django_datawatch.egg-info/PKG-INFO` & `django-datawatch-3.5.0/django_datawatch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: django-datawatch
-Version: 3.4.0
+Version: 3.5.0
 Summary: Django Datawatch runs automated data checks in your Django installation
 Home-page: https://github.com/RegioHelden/django-datawatch
 Download-URL: 
 Author: Jens Nistler <opensource@jensnistler.de>, Bogdan Radko <bogdan.radko@regiohelden.de>
 Author-email: opensource@regiohelden.de
 License: MIT
 Keywords: django,monitoring,datawatch,check,checks
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -206,83 +207,83 @@
 Datawatch supported setting a specific queue in release < 0.4.0
 
 With the switch to celery 4, you should use task routing to define the queue for your tasks, see http://docs.celeryproject.org/en/latest/userguide/routing.html
 
 # CONTRIBUTE
 
 ## Dev environment
-- docker (at least 17.12.0+)
-- docker-compose (at least 1.18.0)
+- [Docker](https://docs.docker.com/) (19.03.0 or later)
+- [Compose plugin for Docker](https://docs.docker.com/compose/install/linux/)
 
 Please make sure that no other container is using port 8000 as this is the one you're install gets exposed to:
 http://localhost:8000/
 
 ## Setup
 
 We've included an example app to show how django_datawatch works.
 Start by launching the included docker container.
 ```bash
-docker-compose up -d
+docker compose up -d
 ```
 
 Then setup the example app environment.
 ```bash
-docker-compose run --rm app migrate
-docker-compose run --rm app loaddata example
+docker compose run --rm app migrate
+docker compose run --rm app loaddata example
 ```
 The installed superuser is "example" with password "datawatch".
 
 ## Run checks
 
 Open http://localhost:8000/, log in and then go back to http://localhost:8000/.
 You'll be prompted with an empty dashboard. That's because we didn't run any checks yet.
 Let's enqueue an update.
 ```bash
-docker-compose run --rm app datawatch_run_checks --force
+docker compose run --rm app datawatch_run_checks --force
 ```
 
 The checks for the example app are run synchronously and should be updated immediately.
 If you decide to switch to the celery backend, you should now start a celery worker to process the checks.
 ```bash
-docker-compose run --rm --entrypoint celery app -A example worker -l DEBUG
+docker compose run --rm --entrypoint celery app -A example worker -l DEBUG
 ```
 
 To execute the celery beat scheduler which runs the datawatch scheduler every minute, just run:
 ```bash
-docker-compose run --rm --entrypoint celery app -A example  beat --scheduler django_celery_beat.schedulers:DatabaseScheduler
+docker compose run --rm --entrypoint celery app -A example  beat --scheduler django_celery_beat.schedulers:DatabaseScheduler
 ```
 
 You will see some failed check now after you refreshed the dashboard view.
 
 ![Django Datawatch dashboard](http://static.jensnistler.de/django_datawatch.png "Django Datawatch dashboard")
 
 ## Run the tests
 ```bash
-docker-compose run --rm app test
+docker compose run --rm app test
 ```
 
 ## Requirements upgrades
 
 Check for upgradeable packages by running 
 ```bash
-docker-compose up -d
-docker-compose exec app pip-check
+docker compose up -d
+docker compose exec app pip-check
 ```
 
 ## Translations
 
 Collect and compile translations for all registered locales
 
 ```bash
-docker-compose run --rm app makemessages --no-location --all
-docker-compose run --rm app compilemessages
+docker compose run --rm app makemessages --no-location --all
+docker compose run --rm app compilemessages
 ```
 
 ## Making a new release
 
 [bumpversion](https://github.com/peritus/bumpversion) is used to manage releases.
 
 Add your changes to the [CHANGELOG](./CHANGELOG.rst), run
 ```bash
-docker-compose exec app bumpversion <major|minor|patch>
+docker compose exec app bumpversion <major|minor|patch>
 ```
 then push (including tags).
```

### Comparing `django-datawatch-3.4.0/django_datawatch.egg-info/SOURCES.txt` & `django-datawatch-3.5.0/django_datawatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.4.0/setup.py` & `django-datawatch-3.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,15 @@
     description='Django Datawatch runs automated data checks in your Django installation',
     author='Jens Nistler <opensource@jensnistler.de>, Bogdan Radko <bogdan.radko@regiohelden.de>',
     author_email='opensource@regiohelden.de',
     long_description=long_description(),
     long_description_content_type='text/markdown',
     install_requires=[
         'celery>=5.0.0',
-        'Django>=3.2,<4.2',
-        'django-bootstrap3>=21.1',
+        'Django>=3.2,<5.0',
         'django-extensions>=3.0.0',
         'django-model-utils>=4.2.0',
         'python-dateutil>=2.8.0',
     ],
     license='MIT',
     url='https://github.com/RegioHelden/django-datawatch',
     download_url='',
@@ -47,14 +46,15 @@
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

