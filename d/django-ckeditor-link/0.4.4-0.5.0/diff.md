# Comparing `tmp/django-ckeditor-link-0.4.4.tar.gz` & `tmp/django-ckeditor-link-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ckeditor-link-0.4.4.tar", last modified: Mon Oct 17 08:50:44 2022, max compression
+gzip compressed data, was "django-ckeditor-link-0.5.0.tar", last modified: Wed Apr 19 22:05:21 2023, max compression
```

## Comparing `django-ckeditor-link-0.4.4.tar` & `django-ckeditor-link-0.5.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.182484 django-ckeditor-link-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (121)    18091 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7946 2022-10-17 08:50:44.182484 django-ckeditor-link-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7297 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.174484 django-ckeditor-link-0.4.4/ckeditor_link/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2592 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/link_model/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/link_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/link_model/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     6412 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/link_model/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/management/commands/cmsplugin2ckeditor_link.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.174484 django-ckeditor-link-0.4.4/ckeditor_link/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.174484 django-ckeditor-link-0.4.4/ckeditor_link/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.174484 django-ckeditor-link-0.4.4/ckeditor_link/static/admin/ckeditor_link/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/static/admin/ckeditor_link/css/
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/static/admin/ckeditor_link/css/link_admin.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.174484 django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.174484 django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.174484 django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/
--rw-r--r--   0 runner    (1001) docker     (121)     6536 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/
--rw-r--r--   0 runner    (1001) docker     (121)    23980 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js
--rw-r--r--   0 runner    (1001) docker     (121)    24950 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js
--rw-r--r--   0 runner    (1001) docker     (121)    14939 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js
--rw-r--r--   0 runner    (1001) docker     (121)    11226 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/plugin.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.174484 django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.174484 django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.174484 django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/
--rw-r--r--   0 runner    (1001) docker     (121)     6536 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/
--rw-r--r--   0 runner    (1001) docker     (121)    23980 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js
--rw-r--r--   0 runner    (1001) docker     (121)    24950 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js
--rw-r--r--   0 runner    (1001) docker     (121)    14939 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js
--rw-r--r--   0 runner    (1001) docker     (121)    11226 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/plugin.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3359 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/templatetags/ckeditor_link_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/settings_no_headless.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/migrations/0002_auto_20161128_1458.py
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/migrations/0003_cmsfilerlinkmodel_contriblinkmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/migrations/0004_auto_20210412_0750.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     4469 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_editor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3546 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_link_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2512 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/test_templatetag.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.178484 django-ckeditor-link-0.4.4/ckeditor_link/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/utils/django_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2965 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/ckeditor_link/tests/utils/selenium_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 08:50:44.182484 django-ckeditor-link-0.4.4/django_ckeditor_link.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7946 2022-10-17 08:50:44.000000 django-ckeditor-link-0.4.4/django_ckeditor_link.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-10-17 08:50:44.000000 django-ckeditor-link-0.4.4/django_ckeditor_link.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 08:50:44.000000 django-ckeditor-link-0.4.4/django_ckeditor_link.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 08:50:44.000000 django-ckeditor-link-0.4.4/django_ckeditor_link.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-17 08:50:44.000000 django-ckeditor-link-0.4.4/django_ckeditor_link.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-17 08:50:44.000000 django-ckeditor-link-0.4.4/django_ckeditor_link.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-10-17 08:50:44.182484 django-ckeditor-link-0.4.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1218 2022-10-17 08:50:33.000000 django-ckeditor-link-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.392096 django-ckeditor-link-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-04-19 22:05:21.396096 django-ckeditor-link-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.388096 django-ckeditor-link-0.5.0/ckeditor_link/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.388096 django-ckeditor-link-0.5.0/ckeditor_link/link_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/link_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/link_model/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/link_model/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.388096 django-ckeditor-link-0.5.0/ckeditor_link/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.388096 django-ckeditor-link-0.5.0/ckeditor_link/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/management/commands/cmsplugin2ckeditor_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.388096 django-ckeditor-link-0.5.0/ckeditor_link/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.384096 django-ckeditor-link-0.5.0/ckeditor_link/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.384096 django-ckeditor-link-0.5.0/ckeditor_link/static/admin/ckeditor_link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.388096 django-ckeditor-link-0.5.0/ckeditor_link/static/admin/ckeditor_link/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/static/admin/ckeditor_link/css/link_admin.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.384096 django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.384096 django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.388096 django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.388096 django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.388096 django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.392096 django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/
+-rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24950 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/plugin.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.388096 django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.388096 django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.388096 django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.392096 django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.392096 django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.392096 django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/
+-rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24950 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/plugin.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.392096 django-ckeditor-link-0.5.0/ckeditor_link/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/templatetags/ckeditor_link_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.392096 django-ckeditor-link-0.5.0/ckeditor_link/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/settings_no_headless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.392096 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.392096 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/migrations/0002_auto_20161128_1458.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/migrations/0003_cmsfilerlinkmodel_contriblinkmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/migrations/0004_auto_20210412_0750.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_link_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/test_templatetag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.392096 django-ckeditor-link-0.5.0/ckeditor_link/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/utils/django_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/ckeditor_link/tests/utils/selenium_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:05:21.392096 django-ckeditor-link-0.5.0/django_ckeditor_link.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-04-19 22:05:21.000000 django-ckeditor-link-0.5.0/django_ckeditor_link.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-19 22:05:21.000000 django-ckeditor-link-0.5.0/django_ckeditor_link.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 22:05:21.000000 django-ckeditor-link-0.5.0/django_ckeditor_link.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 22:05:21.000000 django-ckeditor-link-0.5.0/django_ckeditor_link.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 22:05:21.000000 django-ckeditor-link-0.5.0/django_ckeditor_link.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 22:05:21.000000 django-ckeditor-link-0.5.0/django_ckeditor_link.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 22:05:21.396096 django-ckeditor-link-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1218 2023-04-19 22:05:08.000000 django-ckeditor-link-0.5.0/setup.py
```

### Comparing `django-ckeditor-link-0.4.4/CHANGELOG.txt` & `django-ckeditor-link-0.5.0/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 ==== 0.4.5 (under development) ===
 
 - ?
 
 
+==== 0.5.0 (2023-04-19) ===
+
+- add compatibility and tests for django 4.2
+
+
 ==== 0.4.4 (2022-10-17) ===
 
 - fix broken get_link_text for foreign key links
 
 
 ==== 0.4.3 (2022-04-13) ===
```

### Comparing `django-ckeditor-link-0.4.4/LICENSE` & `django-ckeditor-link-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/PKG-INFO` & `django-ckeditor-link-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ckeditor-link
-Version: 0.4.4
+Version: 0.5.0
 Summary: Alternative link dialog for ckeditor 4, using django modeladmin forms.
 Home-page: http://github.com/bnzk/django-ckeditor-link
 Author: Ben Stähli
 Author-email: bnzk@bnzk.ch
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-ckeditor-link
 
 Build status fails sometimes - selenium and iframes and ... sleep. Passes with local tox, believe me.
 
-[![CI](https://img.shields.io/github/workflow/status/bnzk/django-ckeditor-link/CI.svg?style=flat-square&logo=github "CI")](https://github.com/bnzk/django-ckeditor-link/actions/workflows/ci.yml)
+[![CI](https://img.shields.io/github/actions/workflow/status/bnzk/django-ckeditor-link/ci.yml?style=flat-square&logo=github "CI")](https://github.com/bnzk/django-ckeditor-link/actions/workflows/ci.yml)
 [![Version](https://img.shields.io/pypi/v/django-ckeditor-link.svg?style=flat-square "Version")](https://pypi.python.org/pypi/django-ckeditor-link/)
 [![Licence](https://img.shields.io/github/license/bnzk/django-ckeditor-link.svg?style=flat-square "Licence")](https://pypi.python.org/pypi/django-ckeditor-link/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/django-ckeditor-link?style=flat-square "PyPi Downloads")](https://pypistats.org/packages/django-ckeditor-link)
 
 link plugin for ckeditor, based on django modelforms/modeladmin, allowing direct linking to your models, or to whatever your want.
 
 ### Table of contents
```

### Comparing `django-ckeditor-link-0.4.4/README.md` & `django-ckeditor-link-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # django-ckeditor-link
 
 Build status fails sometimes - selenium and iframes and ... sleep. Passes with local tox, believe me.
 
-[![CI](https://img.shields.io/github/workflow/status/bnzk/django-ckeditor-link/CI.svg?style=flat-square&logo=github "CI")](https://github.com/bnzk/django-ckeditor-link/actions/workflows/ci.yml)
+[![CI](https://img.shields.io/github/actions/workflow/status/bnzk/django-ckeditor-link/ci.yml?style=flat-square&logo=github "CI")](https://github.com/bnzk/django-ckeditor-link/actions/workflows/ci.yml)
 [![Version](https://img.shields.io/pypi/v/django-ckeditor-link.svg?style=flat-square "Version")](https://pypi.python.org/pypi/django-ckeditor-link/)
 [![Licence](https://img.shields.io/github/license/bnzk/django-ckeditor-link.svg?style=flat-square "Licence")](https://pypi.python.org/pypi/django-ckeditor-link/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/django-ckeditor-link?style=flat-square "PyPi Downloads")](https://pypistats.org/packages/django-ckeditor-link)
 
 link plugin for ckeditor, based on django modelforms/modeladmin, allowing direct linking to your models, or to whatever your want.
 
 ### Table of contents
```

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/admin.py` & `django-ckeditor-link-0.5.0/ckeditor_link/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.conf import settings
-from django.conf.urls import url
+from django.urls import path
 from django.contrib import admin
 from django.db import models
 from django.forms import widgets
 from django.http import JsonResponse
 
 
 class DjangoLinkAdmin(admin.ModelAdmin):
@@ -27,16 +27,16 @@
         return original_media + new_media
 
     def get_urls(self):
         """
         add verify url.
         """
         my_urls = [
-            url(
-                r'^verify/$',
+            path(
+                'verify/',
                 self.admin_site.admin_view(self.verify),
                 name=self._get_verify_url_name()
             ),
         ]
         return my_urls + super(DjangoLinkAdmin, self).get_urls()
 
     def _get_verify_url_name(self):
```

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/link_model/conf.py` & `django-ckeditor-link-0.5.0/ckeditor_link/link_model/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.conf import settings
 
 
 use = False
 if 'cms' in settings.INSTALLED_APPS and 'filer' in settings.INSTALLED_APPS:
     use = True
```

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/link_model/models.py` & `django-ckeditor-link-0.5.0/ckeditor_link/link_model/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from __future__ import unicode_literals
-
 from django.core.exceptions import ObjectDoesNotExist
 
 try:
     from builtins import str
 except ImportError:
     from __builtin__ import str
 
 from django.conf import settings
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from .conf import (
     CKEDITOR_LINK_TYPE_CHOICES,
     CKEDITOR_LINK_USE_CMS_FILER,
 )
 
 # dropped in favour of builtins/str, see above
```

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/management/commands/cmsplugin2ckeditor_link.py` & `django-ckeditor-link-0.5.0/ckeditor_link/management/commands/cmsplugin2ckeditor_link.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js` & `django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js` & `django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js` & `django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js` & `django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/plugin.js` & `django-ckeditor-link-0.5.0/ckeditor_link/static/ckeditor/ckeditor/plugins/djangolink/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js` & `django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/dialogs/djangolink.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js` & `django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_dialog.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js` & `django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/ckeditor_original_link_plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js` & `django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/examples-not-used/cmsplugin_example.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/plugin.js` & `django-ckeditor-link-0.5.0/ckeditor_link/static/djangocms_text_ckeditor/ckeditor/plugins/djangolink/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/templatetags/ckeditor_link_tags.py` & `django-ckeditor-link-0.5.0/ckeditor_link/templatetags/ckeditor_link_tags.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/tests/settings.py` & `django-ckeditor-link-0.5.0/ckeditor_link/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/admin.py` & `django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/admin.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/migrations/0001_initial.py` & `django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/migrations/0002_auto_20161128_1458.py` & `django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/migrations/0002_auto_20161128_1458.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/migrations/0003_cmsfilerlinkmodel_contriblinkmodel.py` & `django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/migrations/0003_cmsfilerlinkmodel_contriblinkmodel.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/migrations/0004_auto_20210412_0750.py` & `django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/migrations/0004_auto_20210412_0750.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/tests/test_app/models.py` & `django-ckeditor-link-0.5.0/ckeditor_link/tests/test_app/models.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/tests/test_editor.py` & `django-ckeditor-link-0.5.0/ckeditor_link/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/tests/test_link_model.py` & `django-ckeditor-link-0.5.0/ckeditor_link/tests/test_link_model.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/tests/test_templatetag.py` & `django-ckeditor-link-0.5.0/ckeditor_link/tests/test_templatetag.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/ckeditor_link/tests/utils/selenium_utils.py` & `django-ckeditor-link-0.5.0/ckeditor_link/tests/utils/selenium_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.conf import settings
 from django.contrib.auth.models import User
 from django.contrib.staticfiles.testing import StaticLiveServerTestCase
 from selenium.common.exceptions import NoSuchElementException
+from selenium.webdriver.common.by import By
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium import webdriver
 from selenium.webdriver.firefox.options import Options
 
 
 # compat
 import django
@@ -54,15 +55,16 @@
 
 
 class CustomWebDriver(webdriver.Firefox):
     """Our own WebDriver with some helpers added"""
 
     def find_css(self, css_selector):
         """Shortcut to find elements by CSS. Returns either a list or singleton"""
-        elems = self.find_elements_by_css_selector(css_selector)
+        # elems = self.find_elements_by_css_selector(css_selector)
+        elems = self.find_elements(By.CSS_SELECTOR, css_selector)
         found = len(elems)
         if found == 1:
             return elems[0]
         elif not elems:
             raise NoSuchElementException(css_selector)
         return elems
```

### Comparing `django-ckeditor-link-0.4.4/django_ckeditor_link.egg-info/PKG-INFO` & `django-ckeditor-link-0.5.0/django_ckeditor_link.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ckeditor-link
-Version: 0.4.4
+Version: 0.5.0
 Summary: Alternative link dialog for ckeditor 4, using django modeladmin forms.
 Home-page: http://github.com/bnzk/django-ckeditor-link
 Author: Ben Stähli
 Author-email: bnzk@bnzk.ch
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-ckeditor-link
 
 Build status fails sometimes - selenium and iframes and ... sleep. Passes with local tox, believe me.
 
-[![CI](https://img.shields.io/github/workflow/status/bnzk/django-ckeditor-link/CI.svg?style=flat-square&logo=github "CI")](https://github.com/bnzk/django-ckeditor-link/actions/workflows/ci.yml)
+[![CI](https://img.shields.io/github/actions/workflow/status/bnzk/django-ckeditor-link/ci.yml?style=flat-square&logo=github "CI")](https://github.com/bnzk/django-ckeditor-link/actions/workflows/ci.yml)
 [![Version](https://img.shields.io/pypi/v/django-ckeditor-link.svg?style=flat-square "Version")](https://pypi.python.org/pypi/django-ckeditor-link/)
 [![Licence](https://img.shields.io/github/license/bnzk/django-ckeditor-link.svg?style=flat-square "Licence")](https://pypi.python.org/pypi/django-ckeditor-link/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/django-ckeditor-link?style=flat-square "PyPi Downloads")](https://pypistats.org/packages/django-ckeditor-link)
 
 link plugin for ckeditor, based on django modelforms/modeladmin, allowing direct linking to your models, or to whatever your want.
 
 ### Table of contents
```

### Comparing `django-ckeditor-link-0.4.4/django_ckeditor_link.egg-info/SOURCES.txt` & `django-ckeditor-link-0.5.0/django_ckeditor_link.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ckeditor-link-0.4.4/setup.py` & `django-ckeditor-link-0.5.0/setup.py`

 * *Files identical despite different names*

