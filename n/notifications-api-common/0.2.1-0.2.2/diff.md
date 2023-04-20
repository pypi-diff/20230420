# Comparing `tmp/notifications-api-common-0.2.1.tar.gz` & `tmp/notifications-api-common-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notifications-api-common-0.2.1.tar", last modified: Tue Feb  7 14:18:23 2023, max compression
+gzip compressed data, was "notifications-api-common-0.2.2.tar", last modified: Thu Apr 20 10:44:45 2023, max compression
```

## Comparing `notifications-api-common-0.2.1.tar` & `notifications-api-common-0.2.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.034564 notifications-api-common-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-02-07 14:18:23.034564 notifications-api-common-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.030564 notifications-api-common-0.2.1/notifications_api_common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.030564 notifications-api-common-0.2.1/notifications_api_common/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/autoretry.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/kanalen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.026564 notifications-api-common-0.2.1/notifications_api_common/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.026564 notifications-api-common-0.2.1/notifications_api_common/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.030564 notifications-api-common-0.2.1/notifications_api_common/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.026564 notifications-api-common-0.2.1/notifications_api_common/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.030564 notifications-api-common-0.2.1/notifications_api_common/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.030564 notifications-api-common-0.2.1/notifications_api_common/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.030564 notifications-api-common-0.2.1/notifications_api_common/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/management/commands/register_kanalen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.034564 notifications-api-common-0.2.1/notifications_api_common/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/migrations/0002_notificationsconfig_notifications_api_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/migrations/0003_migrate_api_root.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/migrations/0004_remove_notificationsconfig_api_root.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/migrations/0005_auto_20220810_0950.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/migrations/0006_auto_20221018_1406.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/migrations/0006_auto_20221213_0214.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/migrations/0007_auto_20221206_0414.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/migrations/0008_merge_0006_auto_20221213_0214_0007_auto_20221206_0414.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.026564 notifications-api-common-0.2.1/notifications_api_common/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.034564 notifications-api-common-0.2.1/notifications_api_common/templates/notifications_api_common/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/templates/notifications_api_common/kanalen.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.034564 notifications-api-common-0.2.1/notifications_api_common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/notifications_api_common/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.030564 notifications-api-common-0.2.1/notifications_api_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-02-07 14:18:23.000000 notifications-api-common-0.2.1/notifications_api_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-02-07 14:18:23.000000 notifications-api-common-0.2.1/notifications_api_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 14:18:23.000000 notifications-api-common-0.2.1/notifications_api_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 14:18:23.000000 notifications-api-common-0.2.1/notifications_api_common.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-07 14:18:23.000000 notifications-api-common-0.2.1/notifications_api_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-07 14:18:23.000000 notifications-api-common-0.2.1/notifications_api_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-02-07 14:18:23.034564 notifications-api-common-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:18:23.034564 notifications-api-common-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/tests/test_kanaal_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/tests/test_register_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-02-07 14:18:15.000000 notifications-api-common-0.2.1/tests/test_send_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.988062 notifications-api-common-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-20 10:44:45.988062 notifications-api-common-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.984063 notifications-api-common-0.2.2/notifications_api_common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.984063 notifications-api-common-0.2.2/notifications_api_common/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/autoretry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/kanalen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.980063 notifications-api-common-0.2.2/notifications_api_common/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.980063 notifications-api-common-0.2.2/notifications_api_common/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.984063 notifications-api-common-0.2.2/notifications_api_common/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.980063 notifications-api-common-0.2.2/notifications_api_common/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.984063 notifications-api-common-0.2.2/notifications_api_common/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.988062 notifications-api-common-0.2.2/notifications_api_common/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.988062 notifications-api-common-0.2.2/notifications_api_common/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/management/commands/register_kanalen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.988062 notifications-api-common-0.2.2/notifications_api_common/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/migrations/0002_notificationsconfig_notifications_api_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/migrations/0003_migrate_api_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/migrations/0004_remove_notificationsconfig_api_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/migrations/0005_auto_20220810_0950.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/migrations/0006_auto_20221018_1406.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/migrations/0006_auto_20221213_0214.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/migrations/0007_auto_20221206_0414.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/migrations/0008_merge_0006_auto_20221213_0214_0007_auto_20221206_0414.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.980063 notifications-api-common-0.2.2/notifications_api_common/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.988062 notifications-api-common-0.2.2/notifications_api_common/templates/notifications_api_common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/templates/notifications_api_common/kanalen.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.988062 notifications-api-common-0.2.2/notifications_api_common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/notifications_api_common/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.984063 notifications-api-common-0.2.2/notifications_api_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-20 10:44:45.000000 notifications-api-common-0.2.2/notifications_api_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-20 10:44:45.000000 notifications-api-common-0.2.2/notifications_api_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:44:45.000000 notifications-api-common-0.2.2/notifications_api_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:44:45.000000 notifications-api-common-0.2.2/notifications_api_common.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 10:44:45.000000 notifications-api-common-0.2.2/notifications_api_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 10:44:45.000000 notifications-api-common-0.2.2/notifications_api_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-20 10:44:45.988062 notifications-api-common-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:44:45.988062 notifications-api-common-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/tests/test_kanaal_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/tests/test_register_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-20 10:44:38.000000 notifications-api-common-0.2.2/tests/test_send_message.py
```

### Comparing `notifications-api-common-0.2.1/CHANGELOG.rst` & `notifications-api-common-0.2.2/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+0.2.2 (2023-04-20)
+------------------
+
+Fixed a crash in migrations during fresh installs when using the latest zgw-consumers.
+
 0.2.1 (2023-02-07)
 ------------------
 
 Fixed automatic retry for assured delivery introduced in 0.2.0
 
 * After automatic retries are exhausted failed notifications with 50x HTTP statuses
   will be shown in the admin interface.
```

### Comparing `notifications-api-common-0.2.1/LICENSE` & `notifications-api-common-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/PKG-INFO` & `notifications-api-common-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notifications-api-common
-Version: 0.2.1
+Version: 0.2.2
 Summary: Re-usable integration layer for the Common Ground Notifications API specification.
 Home-page: https://github.com/maykinmedia/notifications-api-common
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Project-URL: Changelog, https://github.com/maykinmedia/notifications-api-common/blob/main/CHANGELOG.rst
 Project-URL: Bug Tracker, https://github.com/maykinmedia/notifications-api-common/issues
@@ -30,15 +30,15 @@
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 notifications-api-common
 ========================
 
-:Version: 0.2.1
+:Version: 0.2.2
 :Source: https://github.com/maykinmedia/notifications-api-common
 :Keywords: notifications, REST, API, Common Ground, ZGW
 :PythonVersion: 3.9
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `notifications-api-common-0.2.1/README.rst` & `notifications-api-common-0.2.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 notifications-api-common
 ========================
 
-:Version: 0.2.1
+:Version: 0.2.2
 :Source: https://github.com/maykinmedia/notifications-api-common
 :Keywords: notifications, REST, API, Common Ground, ZGW
 :PythonVersion: 3.9
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `notifications-api-common-0.2.1/notifications_api_common/admin.py` & `notifications-api-common-0.2.2/notifications_api_common/admin.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/api/serializers.py` & `notifications-api-common-0.2.2/notifications_api_common/api/serializers.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/autoretry.py` & `notifications-api-common-0.2.2/notifications_api_common/autoretry.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/kanalen.py` & `notifications-api-common-0.2.2/notifications_api_common/kanalen.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/locale/en/LC_MESSAGES/django.mo` & `notifications-api-common-0.2.2/notifications_api_common/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/locale/en/LC_MESSAGES/django.po` & `notifications-api-common-0.2.2/notifications_api_common/locale/en/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: 0.2.1\n"
+"Project-Id-Version: 0.2.2\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-12-14 13:45+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
```

### Comparing `notifications-api-common-0.2.1/notifications_api_common/locale/nl/LC_MESSAGES/django.mo` & `notifications-api-common-0.2.2/notifications_api_common/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/locale/nl/LC_MESSAGES/django.po` & `notifications-api-common-0.2.2/notifications_api_common/locale/nl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: 0.2.1\n"
+"Project-Id-Version: 0.2.2\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-12-14 13:45+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
```

### Comparing `notifications-api-common-0.2.1/notifications_api_common/management/commands/register_kanalen.py` & `notifications-api-common-0.2.2/notifications_api_common/management/commands/register_kanalen.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/migrations/0001_initial.py` & `notifications-api-common-0.2.2/notifications_api_common/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/migrations/0002_notificationsconfig_notifications_api_service.py` & `notifications-api-common-0.2.2/notifications_api_common/migrations/0002_notificationsconfig_notifications_api_service.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/migrations/0005_auto_20220810_0950.py` & `notifications-api-common-0.2.2/notifications_api_common/migrations/0005_auto_20220810_0950.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/migrations/0006_auto_20221018_1406.py` & `notifications-api-common-0.2.2/notifications_api_common/migrations/0006_auto_20221018_1406.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/migrations/0006_auto_20221213_0214.py` & `notifications-api-common-0.2.2/notifications_api_common/migrations/0006_auto_20221213_0214.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/migrations/0007_auto_20221206_0414.py` & `notifications-api-common-0.2.2/notifications_api_common/migrations/0007_auto_20221206_0414.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/models.py` & `notifications-api-common-0.2.2/notifications_api_common/models.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/tasks.py` & `notifications-api-common-0.2.2/notifications_api_common/tasks.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/templates/notifications_api_common/kanalen.html` & `notifications-api-common-0.2.2/notifications_api_common/templates/notifications_api_common/kanalen.html`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/utils.py` & `notifications-api-common-0.2.2/notifications_api_common/utils.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/validators.py` & `notifications-api-common-0.2.2/notifications_api_common/validators.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common/viewsets.py` & `notifications-api-common-0.2.2/notifications_api_common/viewsets.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/notifications_api_common.egg-info/PKG-INFO` & `notifications-api-common-0.2.2/notifications_api_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notifications-api-common
-Version: 0.2.1
+Version: 0.2.2
 Summary: Re-usable integration layer for the Common Ground Notifications API specification.
 Home-page: https://github.com/maykinmedia/notifications-api-common
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Project-URL: Changelog, https://github.com/maykinmedia/notifications-api-common/blob/main/CHANGELOG.rst
 Project-URL: Bug Tracker, https://github.com/maykinmedia/notifications-api-common/issues
@@ -30,15 +30,15 @@
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 notifications-api-common
 ========================
 
-:Version: 0.2.1
+:Version: 0.2.2
 :Source: https://github.com/maykinmedia/notifications-api-common
 :Keywords: notifications, REST, API, Common Ground, ZGW
 :PythonVersion: 3.9
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `notifications-api-common-0.2.1/notifications_api_common.egg-info/SOURCES.txt` & `notifications-api-common-0.2.2/notifications_api_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/setup.cfg` & `notifications-api-common-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = notifications-api-common
-version = 0.2.1
+version = 0.2.2
 description = Re-usable integration layer for the Common Ground Notifications API specification.
 long_description = file: README.rst
 url = https://github.com/maykinmedia/notifications-api-common
 project_urls = 
 	Changelog = https://github.com/maykinmedia/notifications-api-common/blob/main/CHANGELOG.rst
 	Bug Tracker = https://github.com/maykinmedia/notifications-api-common/issues
 	Source Code = https://github.com/maykinmedia/notifications-api-common
```

### Comparing `notifications-api-common-0.2.1/tests/test_kanaal_documentation.py` & `notifications-api-common-0.2.2/tests/test_kanaal_documentation.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/tests/test_register_webhook.py` & `notifications-api-common-0.2.2/tests/test_register_webhook.py`

 * *Files identical despite different names*

### Comparing `notifications-api-common-0.2.1/tests/test_send_message.py` & `notifications-api-common-0.2.2/tests/test_send_message.py`

 * *Files identical despite different names*

