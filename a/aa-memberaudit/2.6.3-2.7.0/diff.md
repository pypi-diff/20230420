# Comparing `tmp/aa_memberaudit-2.6.3.tar.gz` & `tmp/aa_memberaudit-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_memberaudit-2.6.3.tar", last modified: Sun Apr 16 16:38:10 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aa_memberaudit-2.6.3.tar` & `aa_memberaudit-2.7.0.tar`

### file list

```diff
@@ -1,278 +1,233 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.703024 aa_memberaudit-2.6.3/
--rw-rw-rw-   0 root         (0) root         (0)    25180 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1070 2020-12-07 16:50:18.000000 aa_memberaudit-2.6.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-03-27 13:03:22.000000 aa_memberaudit-2.6.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6841 2023-04-16 16:38:10.703024 aa_memberaudit-2.6.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5719 2023-03-23 15:22:24.000000 aa_memberaudit-2.6.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.527024 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6841 2023-04-16 16:38:10.000000 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11185 2023-04-16 16:38:10.000000 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:38:10.000000 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:38:10.000000 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2023-04-16 16:38:10.000000 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 16:38:10.000000 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.543024 aa_memberaudit-2.6.3/memberaudit/
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22972 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     4486 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1223 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.3/memberaudit/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-03-22 20:38:17.000000 aa_memberaudit-2.6.3/memberaudit/checks.py
--rw-rw-rw-   0 root         (0) root         (0)     1354 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.3/memberaudit/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.547024 aa_memberaudit-2.6.3/memberaudit/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11673 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/core/data_exporters.py
--rw-rw-rw-   0 root         (0) root         (0)    19049 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.3/memberaudit/core/eft_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5305 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.3/memberaudit/core/fittings.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2022-09-03 21:36:22.000000 aa_memberaudit-2.6.3/memberaudit/core/skill_plans.py
--rw-rw-rw-   0 root         (0) root         (0)     5342 2022-09-02 18:40:08.000000 aa_memberaudit-2.6.3/memberaudit/core/skills.py
--rw-rw-rw-   0 root         (0) root         (0)     3150 2022-07-14 11:30:46.000000 aa_memberaudit-2.6.3/memberaudit/core/xml_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     2336 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     3636 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     2257 2023-02-24 17:52:57.000000 aa_memberaudit-2.6.3/memberaudit/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.551024 aa_memberaudit-2.6.3/memberaudit/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    40294 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.551024 aa_memberaudit-2.6.3/memberaudit/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    40291 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.551024 aa_memberaudit-2.6.3/memberaudit/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    40291 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/ko/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.551024 aa_memberaudit-2.6.3/memberaudit/locale/ko/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    40284 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.551024 aa_memberaudit-2.6.3/memberaudit/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    40433 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.551024 aa_memberaudit-2.6.3/memberaudit/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    40284 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.559024 aa_memberaudit-2.6.3/memberaudit/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      102 2020-11-24 21:31:34.000000 aa_memberaudit-2.6.3/memberaudit/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1424 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_data_export.py
--rw-rw-rw-   0 root         (0) root         (0)     1357 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_load_eve.py
--rw-rw-rw-   0 root         (0) root         (0)     3832 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_reset_characters.py
--rw-rw-rw-   0 root         (0) root         (0)      723 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_stats.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_update_characters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.563024 aa_memberaudit-2.6.3/memberaudit/managers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/managers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13007 2023-02-24 14:11:29.000000 aa_memberaudit-2.6.3/memberaudit/managers/character.py
--rw-rw-rw-   0 root         (0) root         (0)    21180 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/managers/general.py
--rw-rw-rw-   0 root         (0) root         (0)    48369 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/managers/sections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.567024 aa_memberaudit-2.6.3/memberaudit/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    65995 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.3/memberaudit/migrations/0001_initial_new.py
--rw-rw-rw-   0 root         (0) root         (0)     3444 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.3/memberaudit/migrations/0002_add_mining_ledger.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.3/memberaudit/migrations/0003_add_notify_permission.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.3/memberaudit/migrations/0004_character_is_disabled.py
--rw-rw-rw-   0 root         (0) root         (0)     3819 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/migrations/0005_add_fw_stats.py
--rw-rw-rw-   0 root         (0) root         (0)     5969 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/migrations/0006_add_localizations.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.567024 aa_memberaudit-2.6.3/memberaudit/models/
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    53374 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/models/character.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2021-01-17 22:43:01.000000 aa_memberaudit-2.6.3/memberaudit/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    14766 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/models/general.py
--rw-rw-rw-   0 root         (0) root         (0)    39924 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.3/memberaudit/models/sections.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2022-06-17 10:57:57.000000 aa_memberaudit-2.6.3/memberaudit/providers.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2022-03-05 14:47:06.000000 aa_memberaudit-2.6.3/memberaudit/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.591024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-02-24 14:11:29.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/admin.css
--rw-rw-rw-   0 root         (0) root         (0)      174 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/character_finder.css
--rw-rw-rw-   0 root         (0) root         (0)     5638 2022-10-13 18:45:54.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/character_viewer.css
--rw-rw-rw-   0 root         (0) root         (0)     2540 2021-01-29 15:59:17.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/character_viewer.min.css
--rw-rw-rw-   0 root         (0) root         (0)       94 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/data_export.css
--rw-rw-rw-   0 root         (0) root         (0)     1538 2021-05-04 21:32:43.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/global.css
--rw-rw-rw-   0 root         (0) root         (0)      646 2021-01-29 15:59:17.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/global.min.css
--rw-rw-rw-   0 root         (0) root         (0)     4331 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/launcher.css
--rw-rw-rw-   0 root         (0) root         (0)     2765 2021-01-29 15:59:17.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/launcher.min.css
--rw-rw-rw-   0 root         (0) root         (0)     1363 2021-02-16 17:03:36.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/memberaudit.css
--rw-rw-rw-   0 root         (0) root         (0)      617 2021-02-16 17:03:36.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/memberaudit.min.css
--rw-rw-rw-   0 root         (0) root         (0)      611 2021-02-17 10:40:00.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/reports.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.607024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/
--rw-rw-rw-   0 root         (0) root         (0)    43262 2020-10-26 16:42:17.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
--rw-rw-rw-   0 root         (0) root         (0)    43381 2020-10-26 16:42:17.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
--rw-rw-rw-   0 root         (0) root         (0)     1862 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/charisma.png
--rw-rw-rw-   0 root         (0) root         (0)      694 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/eve-prism.png
--rw-rw-rw-   0 root         (0) root         (0)      220 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/evelogo.png
--rw-rw-rw-   0 root         (0) root         (0)      595 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/evesearch.png
--rw-rw-rw-   0 root         (0) root         (0)     1966 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/intelligence.png
--rw-rw-rw-   0 root         (0) root         (0)     1809 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/memory.png
--rw-rw-rw-   0 root         (0) root         (0)     1803 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/perception.png
--rw-rw-rw-   0 root         (0) root         (0)     1782 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/willpower.png
--rw-rw-rw-   0 root         (0) root         (0)      259 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/zkillboard.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.615024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/
--rw-rw-rw-   0 root         (0) root         (0)     5573 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-rw-rw-   0 root         (0) root         (0)     3908 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
--rw-rw-rw-   0 root         (0) root         (0)     2529 2022-04-01 19:48:30.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
--rw-rw-rw-   0 root         (0) root         (0)      384 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-rw-rw-   0 root         (0) root         (0)      384 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.615024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/moment/
--rw-rw-rw-   0 root         (0) root         (0)    69950 2020-10-28 14:46:25.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/moment/moment.min.js
--rw-rw-rw-   0 root         (0) root         (0)   881821 2023-02-16 19:01:05.000000 aa_memberaudit-2.6.3/memberaudit/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)    39964 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/templates/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.619024 aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/character/
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.619024 aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/skillset/
--rw-rw-rw-   0 root         (0) root         (0)      488 2022-09-02 18:40:08.000000 aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/skillset/change_list.html
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.623024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/
--rw-rw-rw-   0 root         (0) root         (0)      367 2020-12-07 00:53:01.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/base.html
--rw-rw-rw-   0 root         (0) root         (0)     4711 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/character_finder.html
--rw-rw-rw-   0 root         (0) root         (0)    27476 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/character_viewer.html
--rw-rw-rw-   0 root         (0) root         (0)     2909 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/data_export.html
--rw-rw-rw-   0 root         (0) root         (0)     8515 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/launcher.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.631024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/
--rw-rw-rw-   0 root         (0) root         (0)     1238 2021-01-29 15:52:00.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
--rw-rw-rw-   0 root         (0) root         (0)     4307 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
--rw-rw-rw-   0 root         (0) root         (0)     1713 2021-02-18 07:41:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1246 2020-11-01 21:48:51.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
--rw-rw-rw-   0 root         (0) root         (0)     8075 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
--rw-rw-rw-   0 root         (0) root         (0)      658 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
--rw-rw-rw-   0 root         (0) root         (0)     1375 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
--rw-rw-rw-   0 root         (0) root         (0)     3880 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.635024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.635024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/
--rw-rw-rw-   0 root         (0) root         (0)     9001 2022-07-22 18:45:02.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
--rw-rw-rw-   0 root         (0) root         (0)     1451 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.647024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/
--rw-rw-rw-   0 root         (0) root         (0)     1218 2021-01-29 15:52:00.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
--rw-rw-rw-   0 root         (0) root         (0)     2604 2021-02-23 15:40:36.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
--rw-rw-rw-   0 root         (0) root         (0)      808 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
--rw-rw-rw-   0 root         (0) root         (0)      919 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
--rw-rw-rw-   0 root         (0) root         (0)      543 2020-11-09 19:29:14.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
--rw-rw-rw-   0 root         (0) root         (0)      894 2020-12-14 23:31:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
--rw-rw-rw-   0 root         (0) root         (0)      488 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
--rw-rw-rw-   0 root         (0) root         (0)     2786 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
--rw-rw-rw-   0 root         (0) root         (0)      678 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
--rw-rw-rw-   0 root         (0) root         (0)      148 2020-11-09 19:29:14.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
--rw-rw-rw-   0 root         (0) root         (0)      572 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
--rw-rw-rw-   0 root         (0) root         (0)     2841 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
--rw-rw-rw-   0 root         (0) root         (0)      741 2022-10-13 17:41:55.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
--rw-rw-rw-   0 root         (0) root         (0)      626 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
--rw-rw-rw-   0 root         (0) root         (0)      554 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
--rw-rw-rw-   0 root         (0) root         (0)     2674 2022-01-23 15:08:18.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.651024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.651024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
--rw-rw-rw-   0 root         (0) root         (0)      691 2021-02-16 15:13:05.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
--rw-rw-rw-   0 root         (0) root         (0)      709 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/solar_system.html
--rw-rw-rw-   0 root         (0) root         (0)     9420 2022-04-01 19:56:47.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/reports.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.651024 aa_memberaudit-2.6.3/memberaudit/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      330 2021-01-05 22:10:38.000000 aa_memberaudit-2.6.3/memberaudit/templatetags/memberaudit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.659024 aa_memberaudit-2.6.3/memberaudit/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.659024 aa_memberaudit-2.6.3/memberaudit/tests/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6340 2022-07-14 11:30:46.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/test_core_xml_converter.py
--rw-rw-rw-   0 root         (0) root         (0)    12708 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/test_data_exporters.py
--rw-rw-rw-   0 root         (0) root         (0)    20438 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/test_eft_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4627 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/test_fittings.py
--rw-rw-rw-   0 root         (0) root         (0)     4082 2022-09-03 21:36:22.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/test_skill_plans.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2022-09-02 18:40:08.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/test_skills.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.663024 aa_memberaudit-2.6.3/memberaudit/tests/managers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/tests/managers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18357 2023-02-24 14:11:29.000000 aa_memberaudit-2.6.3/memberaudit/tests/managers/test_character.py
--rw-rw-rw-   0 root         (0) root         (0)    39823 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/managers/test_general.py
--rw-rw-rw-   0 root         (0) root         (0)     3382 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/managers/test_sections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.667024 aa_memberaudit-2.6.3/memberaudit/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    34701 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_1.py
--rw-rw-rw-   0 root         (0) root         (0)    35834 2023-02-16 19:01:05.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_2.py
--rw-rw-rw-   0 root         (0) root         (0)    40698 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_3.py
--rw-rw-rw-   0 root         (0) root         (0)    28275 2023-03-22 21:45:48.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_4.py
--rw-rw-rw-   0 root         (0) root         (0)    10448 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/test_general.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/test_sections.py
--rw-rw-rw-   0 root         (0) root         (0)     1048 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11633 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2023-02-24 17:52:57.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_checks.py
--rw-rw-rw-   0 root         (0) root         (0)     3425 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     4062 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2022-08-07 14:05:02.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_factories.py
--rw-rw-rw-   0 root         (0) root         (0)     3516 2022-09-03 16:21:19.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_forms.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2023-02-24 17:52:57.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    12216 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2022-03-05 14:47:06.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_signals.py
--rw-rw-rw-   0 root         (0) root         (0)    36109 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_templatetags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.679024 aa_memberaudit-2.6.3/memberaudit/tests/testdata/
--rw-rw-rw-   0 root         (0) root         (0)      267 2020-10-22 17:18:30.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4277 2022-10-12 21:43:27.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/create_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)     4350 2022-02-10 22:57:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/entities.json
--rw-rw-rw-   0 root         (0) root         (0)     4703 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/esi_client_stub.py
--rw-rw-rw-   0 root         (0) root         (0)    40192 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/esi_testdata.json
--rw-rw-rw-   0 root         (0) root         (0)  1159197 2022-10-12 21:43:27.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/eveuniverse.json
--rw-rw-rw-   0 root         (0) root         (0)    11769 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.691024 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/
--rw-rw-rw-   0 root         (0) root         (0)      799 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_archon.txt
--rw-rw-rw-   0 root         (0) root         (0)      889 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
--rw-rw-rw-   0 root         (0) root         (0)      231 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_empty.txt
--rw-rw-rw-   0 root         (0) root         (0)      503 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
--rw-rw-rw-   0 root         (0) root         (0)      193 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
--rw-rw-rw-   0 root         (0) root         (0)      377 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
--rw-rw-rw-   0 root         (0) root         (0)       96 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
--rw-rw-rw-   0 root         (0) root         (0)      583 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_svipul.txt
--rw-rw-rw-   0 root         (0) root         (0)      432 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
--rw-rw-rw-   0 root         (0) root         (0)      700 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_tengu.txt
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_tristan.txt
--rw-rw-rw-   0 root         (0) root         (0)      332 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
--rw-rw-rw-   0 root         (0) root         (0)      410 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
--rw-rw-rw-   0 root         (0) root         (0)      460 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
--rw-rw-rw-   0 root         (0) root         (0)     3908 2022-01-20 23:34:01.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/generate_character.py
--rw-rw-rw-   0 root         (0) root         (0)     3859 2022-01-20 23:34:01.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/generate_doctrines.py
--rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/load_entities.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2020-10-22 17:18:30.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/load_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)     1188 2022-02-10 21:29:55.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/load_locations.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/pilot_esi_error_handling.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/profiler_toolbox.py
--rw-rw-rw-   0 root         (0) root         (0)     3494 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.699024 aa_memberaudit-2.6.3/memberaudit/tests/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7809 2022-09-03 16:21:19.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     7079 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_character_finder.py
--rw-rw-rw-   0 root         (0) root         (0)    32680 2023-03-22 21:45:48.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_character_viewer_1.py
--rw-rw-rw-   0 root         (0) root         (0)    22475 2022-10-13 12:47:37.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_character_viewer_2.py
--rw-rw-rw-   0 root         (0) root         (0)    14577 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_characters.py
--rw-rw-rw-   0 root         (0) root         (0)     4091 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_data_export.py
--rw-rw-rw-   0 root         (0) root         (0)    16230 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_reports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.699024 aa_memberaudit-2.6.3/memberaudit/tools/
--rw-rw-rw-   0 root         (0) root         (0)     3051 2022-10-21 18:07:26.000000 aa_memberaudit-2.6.3/memberaudit/tools/drop_tables.sql
--rw-rw-rw-   0 root         (0) root         (0)      329 2020-12-16 22:00:54.000000 aa_memberaudit-2.6.3/memberaudit/tools/total_size.sql
--rw-rw-rw-   0 root         (0) root         (0)     7031 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.703024 aa_memberaudit-2.6.3/memberaudit/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/views/_common.py
--rw-rw-rw-   0 root         (0) root         (0)     4636 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/admin.py
--rw-rw-rw-   0 root         (0) root         (0)    12529 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/character_finder.py
--rw-rw-rw-   0 root         (0) root         (0)    25505 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/character_viewer_1.py
--rw-rw-rw-   0 root         (0) root         (0)    22528 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/character_viewer_2.py
--rw-rw-rw-   0 root         (0) root         (0)     7909 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/characters.py
--rw-rw-rw-   0 root         (0) root         (0)     2231 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/data_export.py
--rw-rw-rw-   0 root         (0) root         (0)    13100 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/reports.py
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1748 2023-04-16 16:38:10.707024 aa_memberaudit-2.6.3/setup.cfg
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/__init__.py
+-rw-r--r--   0        0        0    22972 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/admin.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/app_settings.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/apps.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/auth_hooks.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/checks.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/constants.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/decorators.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/forms.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/helpers.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/providers.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/signals.py
+-rw-r--r--   0        0        0   881821 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/swagger.json
+-rw-r--r--   0        0        0    40138 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tasks.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/__init__.py
+-rw-r--r--   0        0        0    11673 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/data_exporters.py
+-rw-r--r--   0        0        0    19049 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/eft_parser.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/fittings.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/skill_plans.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/skills.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/core/xml_converter.py
+-rw-r--r--   0        0        0    40885 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/django.pot
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40935 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    40291 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40932 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40885 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40885 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40925 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40885 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41080 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41163 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40925 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/management/commands/__init__.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_data_export.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_load_eve.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_reset_characters.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_stats.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_update_characters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/managers/__init__.py
+-rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/managers/character.py
+-rw-r--r--   0        0        0    21235 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/managers/general.py
+-rw-r--r--   0        0        0    48513 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/managers/sections.py
+-rw-r--r--   0        0        0    65995 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0002_add_mining_ledger.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0003_add_notify_permission.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0004_character_is_disabled.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0005_add_fw_stats.py
+-rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0006_add_localizations.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/0007_add_localization_2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/migrations/__init__.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/models/__init__.py
+-rw-r--r--   0        0        0    54096 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/models/character.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/models/constants.py
+-rw-r--r--   0        0        0    15409 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/models/general.py
+-rw-r--r--   0        0        0    40017 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/models/sections.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/admin.css
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/character_finder.css
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/character_viewer.css
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/character_viewer.min.css
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/data_export.css
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/global.css
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/global.min.css
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/launcher.css
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/launcher.min.css
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/memberaudit.css
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/memberaudit.min.css
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/reports.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/charisma.png
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/eve-prism.png
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/evelogo.png
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/evesearch.png
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/intelligence.png
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/memory.png
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/perception.png
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/willpower.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/zkillboard.png
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
+-rw-r--r--   0        0        0    69950 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/moment/moment.min.js
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/admin/memberaudit/skillset/change_list.html
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/base.html
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/character_finder.html
+-rw-r--r--   0        0        0    27476 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/character_viewer.html
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/data_export.html
+-rw-r--r--   0        0        0     8515 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/launcher.html
+-rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/reports.html
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/menu.html
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/solar_system.html
+-rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templatetags/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/templatetags/memberaudit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/__init__.py
+-rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_admin.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_checks.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_commands.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_decorators.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_factories.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_forms.py
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_helpers.py
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_integration.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_signals.py
+-rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_tasks.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/test_templatetags.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/__init__.py
+-rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/test_core_xml_converter.py
+-rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/test_data_exporters.py
+-rw-r--r--   0        0        0    20438 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/test_eft_parser.py
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/test_fittings.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/test_skill_plans.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/core/test_skills.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/managers/__init__.py
+-rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/managers/test_character.py
+-rw-r--r--   0        0        0    41576 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/managers/test_general.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/managers/test_sections.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/__init__.py
+-rw-r--r--   0        0        0    36061 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_1.py
+-rw-r--r--   0        0        0    35834 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_2.py
+-rw-r--r--   0        0        0    40698 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_3.py
+-rw-r--r--   0        0        0    28275 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_4.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_5.py
+-rw-r--r--   0        0        0    10448 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_general.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/test_sections.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/models/utils.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/entities.json
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/esi_client_stub.py
+-rw-r--r--   0        0        0    40192 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/esi_testdata.json
+-rw-r--r--   0        0        0  1159197 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0    12618 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/factories.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/generate_character.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/generate_doctrines.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/load_entities.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/load_locations.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/pilot_esi_error_handling.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/profiler_toolbox.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_archon.txt
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_empty.txt
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_svipul.txt
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_tengu.txt
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_tristan.txt
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/__init__.py
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_admin.py
+-rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_character_finder.py
+-rw-r--r--   0        0        0    32680 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_character_viewer_1.py
+-rw-r--r--   0        0        0    22475 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_character_viewer_2.py
+-rw-r--r--   0        0        0    14577 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_characters.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_data_export.py
+-rw-r--r--   0        0        0    16230 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tests/views/test_reports.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tools/drop_tables.sql
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/tools/total_size.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/__init__.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/_common.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/admin.py
+-rw-r--r--   0        0        0    12529 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/character_finder.py
+-rw-r--r--   0        0        0    25497 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/character_viewer_1.py
+-rw-r--r--   0        0        0    22528 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/character_viewer_2.py
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/characters.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/data_export.py
+-rw-r--r--   0        0        0    13100 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/memberaudit/views/reports.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/LICENSE
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/README.md
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 aa_memberaudit-2.7.0/PKG-INFO
```

### Comparing `aa_memberaudit-2.6.3/LICENSE` & `aa_memberaudit-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/PKG-INFO` & `aa_memberaudit-2.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Metadata-Version: 2.1
-Name: aa_memberaudit
-Version: 2.6.3
+Name: aa-memberaudit
+Version: 2.7.0
 Summary: An Alliance Auth app that provides full access to Eve characters and related reports for auditing, vetting and monitoring.
-Home-page: https://gitlab.com/ErikKalkoken/aa-memberaudit
-Author: Erik Kalkoken
-Author-email: kalkoken87@gmail.com
-License: MIT
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-memberaudit
+Project-URL: Documentation, https://aa-memberaudit.readthedocs.io/en/latest/
+Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-memberaudit
+Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-memberaudit/-/blob/master/CHANGELOG.md
+Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-memberaudit/-/issues
+Author-email: Erik Kalkoken <kalkoken87@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
 Keywords: allianceauth,eveonline,memberaudit
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.8
+Requires-Python: >=3.8
+Requires-Dist: allianceauth-app-utils>=1.16.1
+Requires-Dist: allianceauth>=3
+Requires-Dist: bleach
+Requires-Dist: dj-datatables-view
+Requires-Dist: django-eveuniverse>=0.19
+Requires-Dist: humanize
+Requires-Dist: unidecode
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Member Audit
 
 An Alliance Auth app that provides full access to Eve characters and related reports for auditing, vetting and monitoring.
 
 [![release](https://img.shields.io/pypi/v/aa-memberaudit?label=release)](https://pypi.org/project/aa-memberaudit/)
 [![python](https://img.shields.io/pypi/pyversions/aa-memberaudit)](https://pypi.org/project/aa-memberaudit/)
```

### Comparing `aa_memberaudit-2.6.3/README.md` & `aa_memberaudit-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/admin.py` & `aa_memberaudit-2.7.0/memberaudit/admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/app_settings.py` & `aa_memberaudit-2.7.0/memberaudit/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/auth_hooks.py` & `aa_memberaudit-2.7.0/memberaudit/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/checks.py` & `aa_memberaudit-2.7.0/memberaudit/checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/constants.py` & `aa_memberaudit-2.7.0/memberaudit/constants.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/core/data_exporters.py` & `aa_memberaudit-2.7.0/memberaudit/core/data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/core/eft_parser.py` & `aa_memberaudit-2.7.0/memberaudit/core/eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/core/fittings.py` & `aa_memberaudit-2.7.0/memberaudit/core/fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/core/skill_plans.py` & `aa_memberaudit-2.7.0/memberaudit/core/skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/core/skills.py` & `aa_memberaudit-2.7.0/memberaudit/core/skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/core/xml_converter.py` & `aa_memberaudit-2.7.0/memberaudit/core/xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/decorators.py` & `aa_memberaudit-2.7.0/memberaudit/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/forms.py` & `aa_memberaudit-2.7.0/memberaudit/forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/helpers.py` & `aa_memberaudit-2.7.0/memberaudit/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,39 +18,39 @@
     prop_name: str, dct: dict, Model: type
 ) -> Optional[models.Model]:
     """Gets or creates a new eveuniverse object from a dictionary entry.
 
     return the object on success or None
     """
     if dct.get(prop_name):
-        obj, _ = Model.objects.get_or_create_esi(id=dct.get(prop_name))
+        obj, _ = Model.objects.get_or_create_esi(id=dct.get(prop_name))  # type: ignore
     else:
         obj = None
 
     return obj
 
 
 def get_or_create_or_none(
     prop_name: str, dct: dict, Model: type
 ) -> Optional[models.Model]:
     """Get or creates a Django object from a dictionary entry or returns None."""
     if dct.get(prop_name):
-        obj, _ = Model.objects.get_or_create(id=dct.get(prop_name))
+        obj, _ = Model.objects.get_or_create(id=dct.get(prop_name))  # type: ignore
         return obj
     return None
 
 
 def get_or_none(prop_name: str, dct: dict, Model: type) -> Optional[models.Model]:
     """Gets a new Django object from a dictionary entry
     or returns None if it does not exist."""
     id = dct.get(prop_name)
     if id:
         try:
-            return Model.objects.get(id=id)
-        except Model.DoesNotExist:
+            return Model.objects.get(id=id)  # type: ignore
+        except Model.DoesNotExist:  # type: ignore
             pass
     return None
 
 
 def filter_groups_available_to_user(
     groups_qs: models.QuerySet, user: User
 ) -> models.QuerySet:
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/locale/de/LC_MESSAGES/django.po` & `aa_memberaudit-2.7.0/memberaudit/locale/en/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-16 17:58+0200\n"
-"PO-Revision-Date: 2020-12-07 21:40+0000\n"
-"Language-Team: German (https://app.transifex.com/kalkoken-apps/teams/107978/de/)\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:72
 msgid "Restricted to states"
 msgstr ""
 
 #: admin.py:133 admin.py:311
@@ -275,16 +276,15 @@
 msgstr ""
 
 #: models/general.py:268
 msgid "is doctrine"
 msgstr ""
 
 #: models/general.py:270
-msgid ""
-"This enables a skill set group to show up correctly in doctrine reports"
+msgid "This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
 #: models/general.py:276
 msgid "is active"
 msgstr ""
 
 #: models/general.py:277
@@ -337,16 +337,15 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:414
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
-#: templates/memberaudit/reports.html:80
-#: templates/memberaudit/reports.html:145
+#: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
 #: models/general.py:415
 msgid "Mailing List"
 msgstr ""
@@ -837,17 +836,20 @@
 msgid "Export file age"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
 "\n"
-"                    Export files contain the complete data of all <strong>%(amount_of_characters)s</strong>\n"
-"                    characters known to Member Audit. They are in CSV format and zipped.\n"
-"                    Existing export files can updated after %(minutes_until_next_update)s minutes.\n"
+"                    Export files contain the complete data of all "
+"<strong>%(amount_of_characters)s</strong>\n"
+"                    characters known to Member Audit. They are in CSV format "
+"and zipped.\n"
+"                    Existing export files can updated after "
+"%(minutes_until_next_update)s minutes.\n"
 "                "
 msgstr ""
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr ""
 
@@ -1559,16 +1561,15 @@
 
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
 msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70
-#: templates/memberaudit/reports.html:209
+#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
 msgid "State"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:15
 msgid "Is Main?"
 msgstr ""
 
@@ -1578,16 +1579,15 @@
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:11
 #: templates/memberaudit/reports.html:85
 msgid "Registered?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:12
-#: templates/memberaudit/reports.html:90
-#: templates/memberaudit/reports.html:150
+#: templates/memberaudit/reports.html:90 templates/memberaudit/reports.html:150
 msgid "Compliant?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:13
 msgid "Total Chars"
 msgstr ""
 
@@ -1649,16 +1649,16 @@
 
 #: views/character_viewer_2.py:616
 msgid "Sell"
 msgstr ""
 
 #: views/characters.py:119
 msgid ""
-"has been registered. Note that it can take a minute until all character data"
-" is visible."
+"has been registered. Note that it can take a minute until all character data "
+"is visible."
 msgstr ""
 
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr ""
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/locale/en/LC_MESSAGES/django.po` & `aa_memberaudit-2.7.0/memberaudit/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,453 +4,487 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-16 17:58+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-19 22:04+0200\n"
+"PO-Revision-Date: 2020-12-07 21:40+0000\n"
+"Language-Team: Russian (https://app.transifex.com/kalkoken-apps/teams/107978/"
+"ru/)\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
+"(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
-#: admin.py:72
+#: admin.py:73
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:133 admin.py:311
+#: admin.py:134 admin.py:312
 msgid "update status"
 msgstr ""
 
-#: admin.py:159 admin.py:288
+#: admin.py:160 admin.py:289
 msgid "state"
 msgstr ""
 
-#: admin.py:185
+#: admin.py:186
 msgid "No main"
 msgstr ""
 
-#: admin.py:267
+#: admin.py:268 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:271
+#: admin.py:272
 msgid "enabled"
 msgstr ""
 
-#: admin.py:277
+#: admin.py:278
 msgid "main"
 msgstr ""
 
-#: admin.py:298
+#: admin.py:299
 msgid "organization"
 msgstr ""
 
-#: admin.py:323
+#: admin.py:324
 msgid "created"
 msgstr ""
 
-#: admin.py:327
+#: admin.py:328
 msgid "last update"
 msgstr ""
 
-#: admin.py:351
+#: admin.py:352
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:362
+#: admin.py:363
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:371
+#: admin.py:372
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:376
+#: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:383
+#: admin.py:384
 #, python-format
 msgid "Started updating character: %s. "
 msgstr ""
 
-#: admin.py:386
+#: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:395
+#: admin.py:396
 #, python-format
 msgid "Started updating assets for character: %s."
 msgstr ""
 
-#: admin.py:401 admin.py:428
+#: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:420
+#: admin.py:421
 #, python-format
 msgid "Started updating %s for character: %s. "
 msgstr ""
 
-#: admin.py:445
+#: admin.py:446
 #, python-format
 msgid "Started updating %s for character: %s."
 msgstr ""
 
-#: admin.py:450
+#: admin.py:451
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:454
+#: admin.py:455
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:456
+#: admin.py:457
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:460
+#: admin.py:461
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:492 models/general.py:259 models/general.py:294
+#: admin.py:493 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:496
+#: admin.py:497
 msgid "solar system"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:501
 msgid "type"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:505
 msgid "group"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:509
 msgid "updated at"
 msgstr ""
 
-#: admin.py:569
+#: admin.py:570
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
 
-#: models/character.py:67
+#: models/character.py:69
 msgid "assets"
 msgstr ""
 
-#: models/character.py:69
+#: models/character.py:71
 msgid "contacts"
 msgstr ""
 
-#: models/character.py:70
+#: models/character.py:72
 msgid "contracts"
 msgstr ""
 
-#: models/character.py:71
+#: models/character.py:73
 msgid "corporation history"
 msgstr ""
 
-#: models/character.py:72
+#: models/character.py:74
 msgid "faction warfare statistics"
 msgstr ""
 
-#: models/character.py:73
+#: models/character.py:75
 msgid "implants"
 msgstr ""
 
-#: models/character.py:74
+#: models/character.py:76
 msgid "jump clones"
 msgstr ""
 
-#: models/character.py:75
+#: models/character.py:77 models/general.py:185
 msgid "location"
 msgstr ""
 
-#: models/character.py:76
+#: models/character.py:78
 msgid "loyalty"
 msgstr ""
 
-#: models/character.py:77
+#: models/character.py:79
 msgid "mails"
 msgstr ""
 
-#: models/character.py:78
+#: models/character.py:80
 msgid "mining ledger"
 msgstr ""
 
-#: models/character.py:79
+#: models/character.py:81
 msgid "online status"
 msgstr ""
 
-#: models/character.py:80
+#: models/character.py:82
 msgid "ship"
 msgstr ""
 
-#: models/character.py:81 models/general.py:335
+#: models/character.py:83 models/general.py:353 models/general.py:386
 msgid "skills"
 msgstr ""
 
-#: models/character.py:82
+#: models/character.py:84
 msgid "skill queue"
 msgstr ""
 
-#: models/character.py:83 models/general.py:263
+#: models/character.py:85 models/general.py:271 models/general.py:340
 msgid "skill sets"
 msgstr ""
 
-#: models/character.py:84
+#: models/character.py:86
 msgid "wallet balance"
 msgstr ""
 
-#: models/character.py:85
+#: models/character.py:87
 msgid "wallet journal"
 msgstr ""
 
-#: models/character.py:86
+#: models/character.py:88
 msgid "wallet transactions"
 msgstr ""
 
-#: models/character.py:87
+#: models/character.py:89
 msgid "attributes"
 msgstr ""
 
-#: models/character.py:139
+#: models/character.py:141
 msgid "ok"
 msgstr ""
 
-#: models/character.py:140 models/sections.py:233
+#: models/character.py:142 models/sections.py:234
 msgid "in progress"
 msgstr ""
 
-#: models/character.py:141
+#: models/character.py:143
 msgid "incomplete"
 msgstr ""
 
-#: models/character.py:142
+#: models/character.py:144
 msgid "error"
 msgstr ""
 
-#: models/character.py:143
+#: models/character.py:145
 msgid "disabled"
 msgstr ""
 
-#: models/character.py:150
+#: models/character.py:152
 msgid "eve character"
 msgstr ""
 
-#: models/character.py:154
+#: models/character.py:156
 msgid "created at"
 msgstr ""
 
-#: models/character.py:158
+#: models/character.py:160
 msgid "is shared"
 msgstr ""
 
-#: models/character.py:163
+#: models/character.py:165
 msgid "is disabled"
 msgstr ""
 
-#: models/character.py:167
+#: models/character.py:169
 msgid "mailing lists"
 msgstr ""
 
-#: models/general.py:261 models/general.py:296
+#: models/character.py:177
+msgid "characters"
+msgstr ""
+
+#: models/character.py:1294 models/character.py:1295
+msgid "character update status"
+msgstr ""
+
+#: models/general.py:116
+msgid "compliance group designation"
+msgstr ""
+
+#: models/general.py:117
+msgid "compliance group designations"
+msgstr ""
+
+#: models/general.py:186
+msgid "locations"
+msgstr ""
+
+#: models/general.py:269 models/general.py:309
 msgid "description"
 msgstr ""
 
-#: models/general.py:268
+#: models/general.py:276
 msgid "is doctrine"
 msgstr ""
 
-#: models/general.py:270
+#: models/general.py:278
 msgid "This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
-#: models/general.py:276
+#: models/general.py:284
 msgid "is active"
 msgstr ""
 
-#: models/general.py:277
+#: models/general.py:285
 msgid "Whether this skill set group is in active use"
 msgstr ""
 
-#: models/general.py:285
+#: models/general.py:290
+msgid "skill set group"
+msgstr ""
+
+#: models/general.py:291
+msgid "skill set groups"
+msgstr ""
+
+#: models/general.py:298
 msgid "Doctrine: "
 msgstr ""
 
-#: models/general.py:304
+#: models/general.py:317
 msgid "ship type"
 msgstr ""
 
-#: models/general.py:307
+#: models/general.py:320
 msgid ""
 "Ship type is used for visual presentation only. All skill requirements must "
 "be explicitly defined."
 msgstr ""
 
-#: models/general.py:315
+#: models/general.py:328
 msgid "is visible"
 msgstr ""
 
-#: models/general.py:317
+#: models/general.py:330
 msgid ""
 "Non visible skill sets are not shown to users on their character sheet and "
 "used for audit purposes only."
 msgstr ""
 
-#: models/general.py:340
+#: models/general.py:339
+msgid "skill set"
+msgstr ""
+
+#: models/general.py:358 models/general.py:385
 msgid "skill"
 msgstr ""
 
-#: models/general.py:349
+#: models/general.py:367
 msgid "required level"
 msgstr ""
 
-#: models/general.py:356
+#: models/general.py:374
 msgid "recommended level"
 msgstr ""
 
-#: models/general.py:412 templates/memberaudit/reports.html:75
+#: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:413
+#: models/general.py:434
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
-#: models/general.py:414
+#: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
 #: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
-#: models/general.py:415
+#: models/general.py:436
 msgid "Mailing List"
 msgstr ""
 
-#: models/general.py:416
+#: models/general.py:437
 msgid "Unknown"
 msgstr ""
 
-#: models/sections.py:146
+#: models/sections.py:147
 msgid "excellent standing"
 msgstr ""
 
-#: models/sections.py:147
+#: models/sections.py:148
 msgid "good standing"
 msgstr ""
 
-#: models/sections.py:148
+#: models/sections.py:149
 msgid "neutral standing"
 msgstr ""
 
-#: models/sections.py:149
+#: models/sections.py:150
 msgid "bad standing"
 msgstr ""
 
-#: models/sections.py:150
+#: models/sections.py:151
 msgid "terrible standing"
 msgstr ""
 
-#: models/sections.py:204
+#: models/sections.py:205
 msgid "alliance"
 msgstr ""
 
-#: models/sections.py:205
+#: models/sections.py:206
 msgid "corporation"
 msgstr ""
 
-#: models/sections.py:206
+#: models/sections.py:207
 msgid "private"
 msgstr ""
 
-#: models/sections.py:207
+#: models/sections.py:208
 msgid "public"
 msgstr ""
 
-#: models/sections.py:227
+#: models/sections.py:228
 msgid "canceled"
 msgstr ""
 
-#: models/sections.py:228
+#: models/sections.py:229
 msgid "deleted"
 msgstr ""
 
-#: models/sections.py:229
+#: models/sections.py:230
 msgid "failed"
 msgstr ""
 
-#: models/sections.py:230
+#: models/sections.py:231
 msgid "finished"
 msgstr ""
 
-#: models/sections.py:231
+#: models/sections.py:232
 msgid "finished contractor"
 msgstr ""
 
-#: models/sections.py:232
+#: models/sections.py:233
 msgid "finished issuer"
 msgstr ""
 
-#: models/sections.py:234
+#: models/sections.py:235
 msgid "outstanding"
 msgstr ""
 
-#: models/sections.py:235
+#: models/sections.py:236
 msgid "rejected"
 msgstr ""
 
-#: models/sections.py:236
+#: models/sections.py:237
 msgid "reversed"
 msgstr ""
 
-#: models/sections.py:257
+#: models/sections.py:258
 msgid "auction"
 msgstr ""
 
-#: models/sections.py:258
+#: models/sections.py:259
 msgid "courier"
 msgstr ""
 
-#: models/sections.py:259
+#: models/sections.py:260
 msgid "item exchange"
 msgstr ""
 
-#: models/sections.py:260
+#: models/sections.py:261
 msgid "loan"
 msgstr ""
 
-#: models/sections.py:261
+#: models/sections.py:262
 msgid "unknown"
 msgstr ""
 
-#: models/sections.py:419
+#: models/sections.py:421
 msgid "[Multiple Items]"
 msgstr ""
 
 #: models/sections.py:520
 msgid "male"
 msgstr ""
 
@@ -1516,15 +1550,15 @@
 msgid "Character Finder"
 msgstr ""
 
 #: templates/memberaudit/partials/menu.html:50 views/reports.py:39
 msgid "Reports"
 msgstr ""
 
-#: templates/memberaudit/partials/menu.html:58 views/data_export.py:25
+#: templates/memberaudit/partials/menu.html:58 views/data_export.py:24
 msgid "Data Export"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:3
 msgid "Color code:"
 msgstr ""
 
@@ -1668,13 +1702,13 @@
 msgstr ""
 
 #: views/characters.py:156
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
-#: views/data_export.py:55
+#: views/data_export.py:53
 #, python-format
 msgid ""
 "Data export for topic <strong>%s</strong> has been started. This can take a "
 "couple of minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/locale/es/LC_MESSAGES/django.po` & `aa_memberaudit-2.7.0/memberaudit/locale/django.pot`

 * *Files 4% similar despite different names*

```diff
@@ -4,453 +4,484 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-16 17:58+0200\n"
+"POT-Creation-Date: 2023-04-19 22:04+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin.py:72
+#: admin.py:73
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:133 admin.py:311
+#: admin.py:134 admin.py:312
 msgid "update status"
 msgstr ""
 
-#: admin.py:159 admin.py:288
+#: admin.py:160 admin.py:289
 msgid "state"
 msgstr ""
 
-#: admin.py:185
+#: admin.py:186
 msgid "No main"
 msgstr ""
 
-#: admin.py:267
+#: admin.py:268 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:271
+#: admin.py:272
 msgid "enabled"
 msgstr ""
 
-#: admin.py:277
+#: admin.py:278
 msgid "main"
 msgstr ""
 
-#: admin.py:298
+#: admin.py:299
 msgid "organization"
 msgstr ""
 
-#: admin.py:323
+#: admin.py:324
 msgid "created"
 msgstr ""
 
-#: admin.py:327
+#: admin.py:328
 msgid "last update"
 msgstr ""
 
-#: admin.py:351
+#: admin.py:352
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:362
+#: admin.py:363
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:371
+#: admin.py:372
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:376
+#: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:383
+#: admin.py:384
 #, python-format
 msgid "Started updating character: %s. "
 msgstr ""
 
-#: admin.py:386
+#: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:395
+#: admin.py:396
 #, python-format
 msgid "Started updating assets for character: %s."
 msgstr ""
 
-#: admin.py:401 admin.py:428
+#: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:420
+#: admin.py:421
 #, python-format
 msgid "Started updating %s for character: %s. "
 msgstr ""
 
-#: admin.py:445
+#: admin.py:446
 #, python-format
 msgid "Started updating %s for character: %s."
 msgstr ""
 
-#: admin.py:450
+#: admin.py:451
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:454
+#: admin.py:455
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:456
+#: admin.py:457
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:460
+#: admin.py:461
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:492 models/general.py:259 models/general.py:294
+#: admin.py:493 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:496
+#: admin.py:497
 msgid "solar system"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:501
 msgid "type"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:505
 msgid "group"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:509
 msgid "updated at"
 msgstr ""
 
-#: admin.py:569
+#: admin.py:570
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
 
-#: models/character.py:67
+#: models/character.py:69
 msgid "assets"
 msgstr ""
 
-#: models/character.py:69
+#: models/character.py:71
 msgid "contacts"
 msgstr ""
 
-#: models/character.py:70
+#: models/character.py:72
 msgid "contracts"
 msgstr ""
 
-#: models/character.py:71
+#: models/character.py:73
 msgid "corporation history"
 msgstr ""
 
-#: models/character.py:72
+#: models/character.py:74
 msgid "faction warfare statistics"
 msgstr ""
 
-#: models/character.py:73
+#: models/character.py:75
 msgid "implants"
 msgstr ""
 
-#: models/character.py:74
+#: models/character.py:76
 msgid "jump clones"
 msgstr ""
 
-#: models/character.py:75
+#: models/character.py:77 models/general.py:185
 msgid "location"
 msgstr ""
 
-#: models/character.py:76
+#: models/character.py:78
 msgid "loyalty"
 msgstr ""
 
-#: models/character.py:77
+#: models/character.py:79
 msgid "mails"
 msgstr ""
 
-#: models/character.py:78
+#: models/character.py:80
 msgid "mining ledger"
 msgstr ""
 
-#: models/character.py:79
+#: models/character.py:81
 msgid "online status"
 msgstr ""
 
-#: models/character.py:80
+#: models/character.py:82
 msgid "ship"
 msgstr ""
 
-#: models/character.py:81 models/general.py:335
+#: models/character.py:83 models/general.py:353 models/general.py:386
 msgid "skills"
 msgstr ""
 
-#: models/character.py:82
+#: models/character.py:84
 msgid "skill queue"
 msgstr ""
 
-#: models/character.py:83 models/general.py:263
+#: models/character.py:85 models/general.py:271 models/general.py:340
 msgid "skill sets"
 msgstr ""
 
-#: models/character.py:84
+#: models/character.py:86
 msgid "wallet balance"
 msgstr ""
 
-#: models/character.py:85
+#: models/character.py:87
 msgid "wallet journal"
 msgstr ""
 
-#: models/character.py:86
+#: models/character.py:88
 msgid "wallet transactions"
 msgstr ""
 
-#: models/character.py:87
+#: models/character.py:89
 msgid "attributes"
 msgstr ""
 
-#: models/character.py:139
+#: models/character.py:141
 msgid "ok"
 msgstr ""
 
-#: models/character.py:140 models/sections.py:233
+#: models/character.py:142 models/sections.py:234
 msgid "in progress"
 msgstr ""
 
-#: models/character.py:141
+#: models/character.py:143
 msgid "incomplete"
 msgstr ""
 
-#: models/character.py:142
+#: models/character.py:144
 msgid "error"
 msgstr ""
 
-#: models/character.py:143
+#: models/character.py:145
 msgid "disabled"
 msgstr ""
 
-#: models/character.py:150
+#: models/character.py:152
 msgid "eve character"
 msgstr ""
 
-#: models/character.py:154
+#: models/character.py:156
 msgid "created at"
 msgstr ""
 
-#: models/character.py:158
+#: models/character.py:160
 msgid "is shared"
 msgstr ""
 
-#: models/character.py:163
+#: models/character.py:165
 msgid "is disabled"
 msgstr ""
 
-#: models/character.py:167
+#: models/character.py:169
 msgid "mailing lists"
 msgstr ""
 
-#: models/general.py:261 models/general.py:296
+#: models/character.py:177
+msgid "characters"
+msgstr ""
+
+#: models/character.py:1294 models/character.py:1295
+msgid "character update status"
+msgstr ""
+
+#: models/general.py:116
+msgid "compliance group designation"
+msgstr ""
+
+#: models/general.py:117
+msgid "compliance group designations"
+msgstr ""
+
+#: models/general.py:186
+msgid "locations"
+msgstr ""
+
+#: models/general.py:269 models/general.py:309
 msgid "description"
 msgstr ""
 
-#: models/general.py:268
+#: models/general.py:276
 msgid "is doctrine"
 msgstr ""
 
-#: models/general.py:270
+#: models/general.py:278
 msgid "This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
-#: models/general.py:276
+#: models/general.py:284
 msgid "is active"
 msgstr ""
 
-#: models/general.py:277
+#: models/general.py:285
 msgid "Whether this skill set group is in active use"
 msgstr ""
 
-#: models/general.py:285
+#: models/general.py:290
+msgid "skill set group"
+msgstr ""
+
+#: models/general.py:291
+msgid "skill set groups"
+msgstr ""
+
+#: models/general.py:298
 msgid "Doctrine: "
 msgstr ""
 
-#: models/general.py:304
+#: models/general.py:317
 msgid "ship type"
 msgstr ""
 
-#: models/general.py:307
+#: models/general.py:320
 msgid ""
 "Ship type is used for visual presentation only. All skill requirements must "
 "be explicitly defined."
 msgstr ""
 
-#: models/general.py:315
+#: models/general.py:328
 msgid "is visible"
 msgstr ""
 
-#: models/general.py:317
+#: models/general.py:330
 msgid ""
 "Non visible skill sets are not shown to users on their character sheet and "
 "used for audit purposes only."
 msgstr ""
 
-#: models/general.py:340
+#: models/general.py:339
+msgid "skill set"
+msgstr ""
+
+#: models/general.py:358 models/general.py:385
 msgid "skill"
 msgstr ""
 
-#: models/general.py:349
+#: models/general.py:367
 msgid "required level"
 msgstr ""
 
-#: models/general.py:356
+#: models/general.py:374
 msgid "recommended level"
 msgstr ""
 
-#: models/general.py:412 templates/memberaudit/reports.html:75
+#: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:413
+#: models/general.py:434
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
-#: models/general.py:414
+#: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
 #: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
-#: models/general.py:415
+#: models/general.py:436
 msgid "Mailing List"
 msgstr ""
 
-#: models/general.py:416
+#: models/general.py:437
 msgid "Unknown"
 msgstr ""
 
-#: models/sections.py:146
+#: models/sections.py:147
 msgid "excellent standing"
 msgstr ""
 
-#: models/sections.py:147
+#: models/sections.py:148
 msgid "good standing"
 msgstr ""
 
-#: models/sections.py:148
+#: models/sections.py:149
 msgid "neutral standing"
 msgstr ""
 
-#: models/sections.py:149
+#: models/sections.py:150
 msgid "bad standing"
 msgstr ""
 
-#: models/sections.py:150
+#: models/sections.py:151
 msgid "terrible standing"
 msgstr ""
 
-#: models/sections.py:204
+#: models/sections.py:205
 msgid "alliance"
 msgstr ""
 
-#: models/sections.py:205
+#: models/sections.py:206
 msgid "corporation"
 msgstr ""
 
-#: models/sections.py:206
+#: models/sections.py:207
 msgid "private"
 msgstr ""
 
-#: models/sections.py:207
+#: models/sections.py:208
 msgid "public"
 msgstr ""
 
-#: models/sections.py:227
+#: models/sections.py:228
 msgid "canceled"
 msgstr ""
 
-#: models/sections.py:228
+#: models/sections.py:229
 msgid "deleted"
 msgstr ""
 
-#: models/sections.py:229
+#: models/sections.py:230
 msgid "failed"
 msgstr ""
 
-#: models/sections.py:230
+#: models/sections.py:231
 msgid "finished"
 msgstr ""
 
-#: models/sections.py:231
+#: models/sections.py:232
 msgid "finished contractor"
 msgstr ""
 
-#: models/sections.py:232
+#: models/sections.py:233
 msgid "finished issuer"
 msgstr ""
 
-#: models/sections.py:234
+#: models/sections.py:235
 msgid "outstanding"
 msgstr ""
 
-#: models/sections.py:235
+#: models/sections.py:236
 msgid "rejected"
 msgstr ""
 
-#: models/sections.py:236
+#: models/sections.py:237
 msgid "reversed"
 msgstr ""
 
-#: models/sections.py:257
+#: models/sections.py:258
 msgid "auction"
 msgstr ""
 
-#: models/sections.py:258
+#: models/sections.py:259
 msgid "courier"
 msgstr ""
 
-#: models/sections.py:259
+#: models/sections.py:260
 msgid "item exchange"
 msgstr ""
 
-#: models/sections.py:260
+#: models/sections.py:261
 msgid "loan"
 msgstr ""
 
-#: models/sections.py:261
+#: models/sections.py:262
 msgid "unknown"
 msgstr ""
 
-#: models/sections.py:419
+#: models/sections.py:421
 msgid "[Multiple Items]"
 msgstr ""
 
 #: models/sections.py:520
 msgid "male"
 msgstr ""
 
@@ -1516,15 +1547,15 @@
 msgid "Character Finder"
 msgstr ""
 
 #: templates/memberaudit/partials/menu.html:50 views/reports.py:39
 msgid "Reports"
 msgstr ""
 
-#: templates/memberaudit/partials/menu.html:58 views/data_export.py:25
+#: templates/memberaudit/partials/menu.html:58 views/data_export.py:24
 msgid "Data Export"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:3
 msgid "Color code:"
 msgstr ""
 
@@ -1668,13 +1699,13 @@
 msgstr ""
 
 #: views/characters.py:156
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
-#: views/data_export.py:55
+#: views/data_export.py:53
 #, python-format
 msgid ""
 "Data export for topic <strong>%s</strong> has been started. This can take a "
 "couple of minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/locale/ko/LC_MESSAGES/django.po` & `aa_memberaudit-2.7.0/memberaudit/locale/de/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,453 +4,485 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-16 17:58+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-19 22:04+0200\n"
+"PO-Revision-Date: 2020-12-07 21:40+0000\n"
+"Language-Team: German (https://app.transifex.com/kalkoken-apps/teams/107978/"
+"de/)\n"
+"Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin.py:72
+#: admin.py:73
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:133 admin.py:311
+#: admin.py:134 admin.py:312
 msgid "update status"
 msgstr ""
 
-#: admin.py:159 admin.py:288
+#: admin.py:160 admin.py:289
 msgid "state"
 msgstr ""
 
-#: admin.py:185
+#: admin.py:186
 msgid "No main"
 msgstr ""
 
-#: admin.py:267
+#: admin.py:268 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:271
+#: admin.py:272
 msgid "enabled"
 msgstr ""
 
-#: admin.py:277
+#: admin.py:278
 msgid "main"
 msgstr ""
 
-#: admin.py:298
+#: admin.py:299
 msgid "organization"
 msgstr ""
 
-#: admin.py:323
+#: admin.py:324
 msgid "created"
 msgstr ""
 
-#: admin.py:327
+#: admin.py:328
 msgid "last update"
 msgstr ""
 
-#: admin.py:351
+#: admin.py:352
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:362
+#: admin.py:363
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:371
+#: admin.py:372
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:376
+#: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:383
+#: admin.py:384
 #, python-format
 msgid "Started updating character: %s. "
 msgstr ""
 
-#: admin.py:386
+#: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:395
+#: admin.py:396
 #, python-format
 msgid "Started updating assets for character: %s."
 msgstr ""
 
-#: admin.py:401 admin.py:428
+#: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:420
+#: admin.py:421
 #, python-format
 msgid "Started updating %s for character: %s. "
 msgstr ""
 
-#: admin.py:445
+#: admin.py:446
 #, python-format
 msgid "Started updating %s for character: %s."
 msgstr ""
 
-#: admin.py:450
+#: admin.py:451
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:454
+#: admin.py:455
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:456
+#: admin.py:457
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:460
+#: admin.py:461
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:492 models/general.py:259 models/general.py:294
+#: admin.py:493 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:496
+#: admin.py:497
 msgid "solar system"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:501
 msgid "type"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:505
 msgid "group"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:509
 msgid "updated at"
 msgstr ""
 
-#: admin.py:569
+#: admin.py:570
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
 
-#: models/character.py:67
+#: models/character.py:69
 msgid "assets"
 msgstr ""
 
-#: models/character.py:69
+#: models/character.py:71
 msgid "contacts"
 msgstr ""
 
-#: models/character.py:70
+#: models/character.py:72
 msgid "contracts"
 msgstr ""
 
-#: models/character.py:71
+#: models/character.py:73
 msgid "corporation history"
 msgstr ""
 
-#: models/character.py:72
+#: models/character.py:74
 msgid "faction warfare statistics"
 msgstr ""
 
-#: models/character.py:73
+#: models/character.py:75
 msgid "implants"
 msgstr ""
 
-#: models/character.py:74
+#: models/character.py:76
 msgid "jump clones"
 msgstr ""
 
-#: models/character.py:75
+#: models/character.py:77 models/general.py:185
 msgid "location"
 msgstr ""
 
-#: models/character.py:76
+#: models/character.py:78
 msgid "loyalty"
 msgstr ""
 
-#: models/character.py:77
+#: models/character.py:79
 msgid "mails"
 msgstr ""
 
-#: models/character.py:78
+#: models/character.py:80
 msgid "mining ledger"
 msgstr ""
 
-#: models/character.py:79
+#: models/character.py:81
 msgid "online status"
 msgstr ""
 
-#: models/character.py:80
+#: models/character.py:82
 msgid "ship"
 msgstr ""
 
-#: models/character.py:81 models/general.py:335
+#: models/character.py:83 models/general.py:353 models/general.py:386
 msgid "skills"
 msgstr ""
 
-#: models/character.py:82
+#: models/character.py:84
 msgid "skill queue"
 msgstr ""
 
-#: models/character.py:83 models/general.py:263
+#: models/character.py:85 models/general.py:271 models/general.py:340
 msgid "skill sets"
 msgstr ""
 
-#: models/character.py:84
+#: models/character.py:86
 msgid "wallet balance"
 msgstr ""
 
-#: models/character.py:85
+#: models/character.py:87
 msgid "wallet journal"
 msgstr ""
 
-#: models/character.py:86
+#: models/character.py:88
 msgid "wallet transactions"
 msgstr ""
 
-#: models/character.py:87
+#: models/character.py:89
 msgid "attributes"
 msgstr ""
 
-#: models/character.py:139
+#: models/character.py:141
 msgid "ok"
 msgstr ""
 
-#: models/character.py:140 models/sections.py:233
+#: models/character.py:142 models/sections.py:234
 msgid "in progress"
 msgstr ""
 
-#: models/character.py:141
+#: models/character.py:143
 msgid "incomplete"
 msgstr ""
 
-#: models/character.py:142
+#: models/character.py:144
 msgid "error"
 msgstr ""
 
-#: models/character.py:143
+#: models/character.py:145
 msgid "disabled"
 msgstr ""
 
-#: models/character.py:150
+#: models/character.py:152
 msgid "eve character"
 msgstr ""
 
-#: models/character.py:154
+#: models/character.py:156
 msgid "created at"
 msgstr ""
 
-#: models/character.py:158
+#: models/character.py:160
 msgid "is shared"
 msgstr ""
 
-#: models/character.py:163
+#: models/character.py:165
 msgid "is disabled"
 msgstr ""
 
-#: models/character.py:167
+#: models/character.py:169
 msgid "mailing lists"
 msgstr ""
 
-#: models/general.py:261 models/general.py:296
+#: models/character.py:177
+msgid "characters"
+msgstr ""
+
+#: models/character.py:1294 models/character.py:1295
+msgid "character update status"
+msgstr ""
+
+#: models/general.py:116
+msgid "compliance group designation"
+msgstr ""
+
+#: models/general.py:117
+msgid "compliance group designations"
+msgstr ""
+
+#: models/general.py:186
+msgid "locations"
+msgstr ""
+
+#: models/general.py:269 models/general.py:309
 msgid "description"
 msgstr ""
 
-#: models/general.py:268
+#: models/general.py:276
 msgid "is doctrine"
 msgstr ""
 
-#: models/general.py:270
+#: models/general.py:278
 msgid "This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
-#: models/general.py:276
+#: models/general.py:284
 msgid "is active"
 msgstr ""
 
-#: models/general.py:277
+#: models/general.py:285
 msgid "Whether this skill set group is in active use"
 msgstr ""
 
-#: models/general.py:285
+#: models/general.py:290
+msgid "skill set group"
+msgstr ""
+
+#: models/general.py:291
+msgid "skill set groups"
+msgstr ""
+
+#: models/general.py:298
 msgid "Doctrine: "
 msgstr ""
 
-#: models/general.py:304
+#: models/general.py:317
 msgid "ship type"
 msgstr ""
 
-#: models/general.py:307
+#: models/general.py:320
 msgid ""
 "Ship type is used for visual presentation only. All skill requirements must "
 "be explicitly defined."
 msgstr ""
 
-#: models/general.py:315
+#: models/general.py:328
 msgid "is visible"
 msgstr ""
 
-#: models/general.py:317
+#: models/general.py:330
 msgid ""
 "Non visible skill sets are not shown to users on their character sheet and "
 "used for audit purposes only."
 msgstr ""
 
-#: models/general.py:340
+#: models/general.py:339
+msgid "skill set"
+msgstr ""
+
+#: models/general.py:358 models/general.py:385
 msgid "skill"
 msgstr ""
 
-#: models/general.py:349
+#: models/general.py:367
 msgid "required level"
 msgstr ""
 
-#: models/general.py:356
+#: models/general.py:374
 msgid "recommended level"
 msgstr ""
 
-#: models/general.py:412 templates/memberaudit/reports.html:75
+#: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:413
+#: models/general.py:434
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
-#: models/general.py:414
+#: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
 #: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
-#: models/general.py:415
+#: models/general.py:436
 msgid "Mailing List"
 msgstr ""
 
-#: models/general.py:416
+#: models/general.py:437
 msgid "Unknown"
 msgstr ""
 
-#: models/sections.py:146
+#: models/sections.py:147
 msgid "excellent standing"
 msgstr ""
 
-#: models/sections.py:147
+#: models/sections.py:148
 msgid "good standing"
 msgstr ""
 
-#: models/sections.py:148
+#: models/sections.py:149
 msgid "neutral standing"
 msgstr ""
 
-#: models/sections.py:149
+#: models/sections.py:150
 msgid "bad standing"
 msgstr ""
 
-#: models/sections.py:150
+#: models/sections.py:151
 msgid "terrible standing"
 msgstr ""
 
-#: models/sections.py:204
+#: models/sections.py:205
 msgid "alliance"
 msgstr ""
 
-#: models/sections.py:205
+#: models/sections.py:206
 msgid "corporation"
 msgstr ""
 
-#: models/sections.py:206
+#: models/sections.py:207
 msgid "private"
 msgstr ""
 
-#: models/sections.py:207
+#: models/sections.py:208
 msgid "public"
 msgstr ""
 
-#: models/sections.py:227
+#: models/sections.py:228
 msgid "canceled"
 msgstr ""
 
-#: models/sections.py:228
+#: models/sections.py:229
 msgid "deleted"
 msgstr ""
 
-#: models/sections.py:229
+#: models/sections.py:230
 msgid "failed"
 msgstr ""
 
-#: models/sections.py:230
+#: models/sections.py:231
 msgid "finished"
 msgstr ""
 
-#: models/sections.py:231
+#: models/sections.py:232
 msgid "finished contractor"
 msgstr ""
 
-#: models/sections.py:232
+#: models/sections.py:233
 msgid "finished issuer"
 msgstr ""
 
-#: models/sections.py:234
+#: models/sections.py:235
 msgid "outstanding"
 msgstr ""
 
-#: models/sections.py:235
+#: models/sections.py:236
 msgid "rejected"
 msgstr ""
 
-#: models/sections.py:236
+#: models/sections.py:237
 msgid "reversed"
 msgstr ""
 
-#: models/sections.py:257
+#: models/sections.py:258
 msgid "auction"
 msgstr ""
 
-#: models/sections.py:258
+#: models/sections.py:259
 msgid "courier"
 msgstr ""
 
-#: models/sections.py:259
+#: models/sections.py:260
 msgid "item exchange"
 msgstr ""
 
-#: models/sections.py:260
+#: models/sections.py:261
 msgid "loan"
 msgstr ""
 
-#: models/sections.py:261
+#: models/sections.py:262
 msgid "unknown"
 msgstr ""
 
-#: models/sections.py:419
+#: models/sections.py:421
 msgid "[Multiple Items]"
 msgstr ""
 
 #: models/sections.py:520
 msgid "male"
 msgstr ""
 
@@ -1516,15 +1548,15 @@
 msgid "Character Finder"
 msgstr ""
 
 #: templates/memberaudit/partials/menu.html:50 views/reports.py:39
 msgid "Reports"
 msgstr ""
 
-#: templates/memberaudit/partials/menu.html:58 views/data_export.py:25
+#: templates/memberaudit/partials/menu.html:58 views/data_export.py:24
 msgid "Data Export"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:3
 msgid "Color code:"
 msgstr ""
 
@@ -1668,13 +1700,13 @@
 msgstr ""
 
 #: views/characters.py:156
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
-#: views/data_export.py:55
+#: views/data_export.py:53
 #, python-format
 msgid ""
 "Data export for topic <strong>%s</strong> has been started. This can take a "
 "couple of minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/locale/ru/LC_MESSAGES/django.po` & `aa_memberaudit-2.7.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,454 +4,484 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-16 17:58+0200\n"
-"PO-Revision-Date: 2020-12-07 21:40+0000\n"
-"Language-Team: Russian (https://app.transifex.com/kalkoken-apps/teams/107978/ru/)\n"
+"POT-Creation-Date: 2023-04-19 22:04+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ru\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 
-#: admin.py:72
+#: admin.py:73
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:133 admin.py:311
+#: admin.py:134 admin.py:312
 msgid "update status"
 msgstr ""
 
-#: admin.py:159 admin.py:288
+#: admin.py:160 admin.py:289
 msgid "state"
 msgstr ""
 
-#: admin.py:185
+#: admin.py:186
 msgid "No main"
 msgstr ""
 
-#: admin.py:267
+#: admin.py:268 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:271
+#: admin.py:272
 msgid "enabled"
 msgstr ""
 
-#: admin.py:277
+#: admin.py:278
 msgid "main"
 msgstr ""
 
-#: admin.py:298
+#: admin.py:299
 msgid "organization"
 msgstr ""
 
-#: admin.py:323
+#: admin.py:324
 msgid "created"
 msgstr ""
 
-#: admin.py:327
+#: admin.py:328
 msgid "last update"
 msgstr ""
 
-#: admin.py:351
+#: admin.py:352
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:362
+#: admin.py:363
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:371
+#: admin.py:372
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:376
+#: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:383
+#: admin.py:384
 #, python-format
 msgid "Started updating character: %s. "
 msgstr ""
 
-#: admin.py:386
+#: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:395
+#: admin.py:396
 #, python-format
 msgid "Started updating assets for character: %s."
 msgstr ""
 
-#: admin.py:401 admin.py:428
+#: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:420
+#: admin.py:421
 #, python-format
 msgid "Started updating %s for character: %s. "
 msgstr ""
 
-#: admin.py:445
+#: admin.py:446
 #, python-format
 msgid "Started updating %s for character: %s."
 msgstr ""
 
-#: admin.py:450
+#: admin.py:451
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:454
+#: admin.py:455
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:456
+#: admin.py:457
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:460
+#: admin.py:461
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:492 models/general.py:259 models/general.py:294
+#: admin.py:493 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:496
+#: admin.py:497
 msgid "solar system"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:501
 msgid "type"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:505
 msgid "group"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:509
 msgid "updated at"
 msgstr ""
 
-#: admin.py:569
+#: admin.py:570
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
 
-#: models/character.py:67
+#: models/character.py:69
 msgid "assets"
 msgstr ""
 
-#: models/character.py:69
+#: models/character.py:71
 msgid "contacts"
 msgstr ""
 
-#: models/character.py:70
+#: models/character.py:72
 msgid "contracts"
 msgstr ""
 
-#: models/character.py:71
+#: models/character.py:73
 msgid "corporation history"
 msgstr ""
 
-#: models/character.py:72
+#: models/character.py:74
 msgid "faction warfare statistics"
 msgstr ""
 
-#: models/character.py:73
+#: models/character.py:75
 msgid "implants"
 msgstr ""
 
-#: models/character.py:74
+#: models/character.py:76
 msgid "jump clones"
 msgstr ""
 
-#: models/character.py:75
+#: models/character.py:77 models/general.py:185
 msgid "location"
 msgstr ""
 
-#: models/character.py:76
+#: models/character.py:78
 msgid "loyalty"
 msgstr ""
 
-#: models/character.py:77
+#: models/character.py:79
 msgid "mails"
 msgstr ""
 
-#: models/character.py:78
+#: models/character.py:80
 msgid "mining ledger"
 msgstr ""
 
-#: models/character.py:79
+#: models/character.py:81
 msgid "online status"
 msgstr ""
 
-#: models/character.py:80
+#: models/character.py:82
 msgid "ship"
 msgstr ""
 
-#: models/character.py:81 models/general.py:335
+#: models/character.py:83 models/general.py:353 models/general.py:386
 msgid "skills"
 msgstr ""
 
-#: models/character.py:82
+#: models/character.py:84
 msgid "skill queue"
 msgstr ""
 
-#: models/character.py:83 models/general.py:263
+#: models/character.py:85 models/general.py:271 models/general.py:340
 msgid "skill sets"
 msgstr ""
 
-#: models/character.py:84
+#: models/character.py:86
 msgid "wallet balance"
 msgstr ""
 
-#: models/character.py:85
+#: models/character.py:87
 msgid "wallet journal"
 msgstr ""
 
-#: models/character.py:86
+#: models/character.py:88
 msgid "wallet transactions"
 msgstr ""
 
-#: models/character.py:87
+#: models/character.py:89
 msgid "attributes"
 msgstr ""
 
-#: models/character.py:139
+#: models/character.py:141
 msgid "ok"
 msgstr ""
 
-#: models/character.py:140 models/sections.py:233
+#: models/character.py:142 models/sections.py:234
 msgid "in progress"
 msgstr ""
 
-#: models/character.py:141
+#: models/character.py:143
 msgid "incomplete"
 msgstr ""
 
-#: models/character.py:142
+#: models/character.py:144
 msgid "error"
 msgstr ""
 
-#: models/character.py:143
+#: models/character.py:145
 msgid "disabled"
 msgstr ""
 
-#: models/character.py:150
+#: models/character.py:152
 msgid "eve character"
 msgstr ""
 
-#: models/character.py:154
+#: models/character.py:156
 msgid "created at"
 msgstr ""
 
-#: models/character.py:158
+#: models/character.py:160
 msgid "is shared"
 msgstr ""
 
-#: models/character.py:163
+#: models/character.py:165
 msgid "is disabled"
 msgstr ""
 
-#: models/character.py:167
+#: models/character.py:169
 msgid "mailing lists"
 msgstr ""
 
-#: models/general.py:261 models/general.py:296
+#: models/character.py:177
+msgid "characters"
+msgstr ""
+
+#: models/character.py:1294 models/character.py:1295
+msgid "character update status"
+msgstr ""
+
+#: models/general.py:116
+msgid "compliance group designation"
+msgstr ""
+
+#: models/general.py:117
+msgid "compliance group designations"
+msgstr ""
+
+#: models/general.py:186
+msgid "locations"
+msgstr ""
+
+#: models/general.py:269 models/general.py:309
 msgid "description"
 msgstr ""
 
-#: models/general.py:268
+#: models/general.py:276
 msgid "is doctrine"
 msgstr ""
 
-#: models/general.py:270
-msgid ""
-"This enables a skill set group to show up correctly in doctrine reports"
+#: models/general.py:278
+msgid "This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
-#: models/general.py:276
+#: models/general.py:284
 msgid "is active"
 msgstr ""
 
-#: models/general.py:277
+#: models/general.py:285
 msgid "Whether this skill set group is in active use"
 msgstr ""
 
-#: models/general.py:285
+#: models/general.py:290
+msgid "skill set group"
+msgstr ""
+
+#: models/general.py:291
+msgid "skill set groups"
+msgstr ""
+
+#: models/general.py:298
 msgid "Doctrine: "
 msgstr ""
 
-#: models/general.py:304
+#: models/general.py:317
 msgid "ship type"
 msgstr ""
 
-#: models/general.py:307
+#: models/general.py:320
 msgid ""
 "Ship type is used for visual presentation only. All skill requirements must "
 "be explicitly defined."
 msgstr ""
 
-#: models/general.py:315
+#: models/general.py:328
 msgid "is visible"
 msgstr ""
 
-#: models/general.py:317
+#: models/general.py:330
 msgid ""
 "Non visible skill sets are not shown to users on their character sheet and "
 "used for audit purposes only."
 msgstr ""
 
-#: models/general.py:340
+#: models/general.py:339
+msgid "skill set"
+msgstr ""
+
+#: models/general.py:358 models/general.py:385
 msgid "skill"
 msgstr ""
 
-#: models/general.py:349
+#: models/general.py:367
 msgid "required level"
 msgstr ""
 
-#: models/general.py:356
+#: models/general.py:374
 msgid "recommended level"
 msgstr ""
 
-#: models/general.py:412 templates/memberaudit/reports.html:75
+#: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:413
+#: models/general.py:434
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
-#: models/general.py:414
+#: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
-#: templates/memberaudit/reports.html:80
-#: templates/memberaudit/reports.html:145
+#: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
-#: models/general.py:415
+#: models/general.py:436
 msgid "Mailing List"
 msgstr ""
 
-#: models/general.py:416
+#: models/general.py:437
 msgid "Unknown"
 msgstr ""
 
-#: models/sections.py:146
+#: models/sections.py:147
 msgid "excellent standing"
 msgstr ""
 
-#: models/sections.py:147
+#: models/sections.py:148
 msgid "good standing"
 msgstr ""
 
-#: models/sections.py:148
+#: models/sections.py:149
 msgid "neutral standing"
 msgstr ""
 
-#: models/sections.py:149
+#: models/sections.py:150
 msgid "bad standing"
 msgstr ""
 
-#: models/sections.py:150
+#: models/sections.py:151
 msgid "terrible standing"
 msgstr ""
 
-#: models/sections.py:204
+#: models/sections.py:205
 msgid "alliance"
 msgstr ""
 
-#: models/sections.py:205
+#: models/sections.py:206
 msgid "corporation"
 msgstr ""
 
-#: models/sections.py:206
+#: models/sections.py:207
 msgid "private"
 msgstr ""
 
-#: models/sections.py:207
+#: models/sections.py:208
 msgid "public"
 msgstr ""
 
-#: models/sections.py:227
+#: models/sections.py:228
 msgid "canceled"
 msgstr ""
 
-#: models/sections.py:228
+#: models/sections.py:229
 msgid "deleted"
 msgstr ""
 
-#: models/sections.py:229
+#: models/sections.py:230
 msgid "failed"
 msgstr ""
 
-#: models/sections.py:230
+#: models/sections.py:231
 msgid "finished"
 msgstr ""
 
-#: models/sections.py:231
+#: models/sections.py:232
 msgid "finished contractor"
 msgstr ""
 
-#: models/sections.py:232
+#: models/sections.py:233
 msgid "finished issuer"
 msgstr ""
 
-#: models/sections.py:234
+#: models/sections.py:235
 msgid "outstanding"
 msgstr ""
 
-#: models/sections.py:235
+#: models/sections.py:236
 msgid "rejected"
 msgstr ""
 
-#: models/sections.py:236
+#: models/sections.py:237
 msgid "reversed"
 msgstr ""
 
-#: models/sections.py:257
+#: models/sections.py:258
 msgid "auction"
 msgstr ""
 
-#: models/sections.py:258
+#: models/sections.py:259
 msgid "courier"
 msgstr ""
 
-#: models/sections.py:259
+#: models/sections.py:260
 msgid "item exchange"
 msgstr ""
 
-#: models/sections.py:260
+#: models/sections.py:261
 msgid "loan"
 msgstr ""
 
-#: models/sections.py:261
+#: models/sections.py:262
 msgid "unknown"
 msgstr ""
 
-#: models/sections.py:419
+#: models/sections.py:421
 msgid "[Multiple Items]"
 msgstr ""
 
 #: models/sections.py:520
 msgid "male"
 msgstr ""
 
@@ -837,17 +867,20 @@
 msgid "Export file age"
 msgstr ""
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
 "\n"
-"                    Export files contain the complete data of all <strong>%(amount_of_characters)s</strong>\n"
-"                    characters known to Member Audit. They are in CSV format and zipped.\n"
-"                    Existing export files can updated after %(minutes_until_next_update)s minutes.\n"
+"                    Export files contain the complete data of all "
+"<strong>%(amount_of_characters)s</strong>\n"
+"                    characters known to Member Audit. They are in CSV format "
+"and zipped.\n"
+"                    Existing export files can updated after "
+"%(minutes_until_next_update)s minutes.\n"
 "                "
 msgstr ""
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr ""
 
@@ -1514,15 +1547,15 @@
 msgid "Character Finder"
 msgstr ""
 
 #: templates/memberaudit/partials/menu.html:50 views/reports.py:39
 msgid "Reports"
 msgstr ""
 
-#: templates/memberaudit/partials/menu.html:58 views/data_export.py:25
+#: templates/memberaudit/partials/menu.html:58 views/data_export.py:24
 msgid "Data Export"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:3
 msgid "Color code:"
 msgstr ""
 
@@ -1559,16 +1592,15 @@
 
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
 msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70
-#: templates/memberaudit/reports.html:209
+#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
 msgid "State"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:15
 msgid "Is Main?"
 msgstr ""
 
@@ -1578,16 +1610,15 @@
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:11
 #: templates/memberaudit/reports.html:85
 msgid "Registered?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:12
-#: templates/memberaudit/reports.html:90
-#: templates/memberaudit/reports.html:150
+#: templates/memberaudit/reports.html:90 templates/memberaudit/reports.html:150
 msgid "Compliant?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:13
 msgid "Total Chars"
 msgstr ""
 
@@ -1649,16 +1680,16 @@
 
 #: views/character_viewer_2.py:616
 msgid "Sell"
 msgstr ""
 
 #: views/characters.py:119
 msgid ""
-"has been registered. Note that it can take a minute until all character data"
-" is visible."
+"has been registered. Note that it can take a minute until all character data "
+"is visible."
 msgstr ""
 
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr ""
 
@@ -1668,13 +1699,13 @@
 msgstr ""
 
 #: views/characters.py:156
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
-#: views/data_export.py:55
+#: views/data_export.py:53
 #, python-format
 msgid ""
 "Data export for topic <strong>%s</strong> has been started. This can take a "
 "couple of minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_memberaudit-2.7.0/memberaudit/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,453 +4,484 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-16 17:58+0200\n"
+"POT-Creation-Date: 2023-04-19 22:04+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: admin.py:72
+#: admin.py:73
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:133 admin.py:311
+#: admin.py:134 admin.py:312
 msgid "update status"
 msgstr ""
 
-#: admin.py:159 admin.py:288
+#: admin.py:160 admin.py:289
 msgid "state"
 msgstr ""
 
-#: admin.py:185
+#: admin.py:186
 msgid "No main"
 msgstr ""
 
-#: admin.py:267
+#: admin.py:268 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:271
+#: admin.py:272
 msgid "enabled"
 msgstr ""
 
-#: admin.py:277
+#: admin.py:278
 msgid "main"
 msgstr ""
 
-#: admin.py:298
+#: admin.py:299
 msgid "organization"
 msgstr ""
 
-#: admin.py:323
+#: admin.py:324
 msgid "created"
 msgstr ""
 
-#: admin.py:327
+#: admin.py:328
 msgid "last update"
 msgstr ""
 
-#: admin.py:351
+#: admin.py:352
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:362
+#: admin.py:363
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:371
+#: admin.py:372
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:376
+#: admin.py:377
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:383
+#: admin.py:384
 #, python-format
 msgid "Started updating character: %s. "
 msgstr ""
 
-#: admin.py:386
+#: admin.py:387
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:395
+#: admin.py:396
 #, python-format
 msgid "Started updating assets for character: %s."
 msgstr ""
 
-#: admin.py:401 admin.py:428
+#: admin.py:402 admin.py:429
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:420
+#: admin.py:421
 #, python-format
 msgid "Started updating %s for character: %s. "
 msgstr ""
 
-#: admin.py:445
+#: admin.py:446
 #, python-format
 msgid "Started updating %s for character: %s."
 msgstr ""
 
-#: admin.py:450
+#: admin.py:451
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:454
+#: admin.py:455
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:456
+#: admin.py:457
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:460
+#: admin.py:461
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:492 models/general.py:259 models/general.py:294
+#: admin.py:493 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:496
+#: admin.py:497
 msgid "solar system"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:501
 msgid "type"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:505
 msgid "group"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:509
 msgid "updated at"
 msgstr ""
 
-#: admin.py:569
+#: admin.py:570
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
 
-#: models/character.py:67
+#: models/character.py:69
 msgid "assets"
 msgstr ""
 
-#: models/character.py:69
+#: models/character.py:71
 msgid "contacts"
 msgstr ""
 
-#: models/character.py:70
+#: models/character.py:72
 msgid "contracts"
 msgstr ""
 
-#: models/character.py:71
+#: models/character.py:73
 msgid "corporation history"
 msgstr ""
 
-#: models/character.py:72
+#: models/character.py:74
 msgid "faction warfare statistics"
 msgstr ""
 
-#: models/character.py:73
+#: models/character.py:75
 msgid "implants"
 msgstr ""
 
-#: models/character.py:74
+#: models/character.py:76
 msgid "jump clones"
 msgstr ""
 
-#: models/character.py:75
+#: models/character.py:77 models/general.py:185
 msgid "location"
 msgstr ""
 
-#: models/character.py:76
+#: models/character.py:78
 msgid "loyalty"
 msgstr ""
 
-#: models/character.py:77
+#: models/character.py:79
 msgid "mails"
 msgstr ""
 
-#: models/character.py:78
+#: models/character.py:80
 msgid "mining ledger"
 msgstr ""
 
-#: models/character.py:79
+#: models/character.py:81
 msgid "online status"
 msgstr ""
 
-#: models/character.py:80
+#: models/character.py:82
 msgid "ship"
 msgstr ""
 
-#: models/character.py:81 models/general.py:335
+#: models/character.py:83 models/general.py:353 models/general.py:386
 msgid "skills"
 msgstr ""
 
-#: models/character.py:82
+#: models/character.py:84
 msgid "skill queue"
 msgstr ""
 
-#: models/character.py:83 models/general.py:263
+#: models/character.py:85 models/general.py:271 models/general.py:340
 msgid "skill sets"
 msgstr ""
 
-#: models/character.py:84
+#: models/character.py:86
 msgid "wallet balance"
 msgstr ""
 
-#: models/character.py:85
+#: models/character.py:87
 msgid "wallet journal"
 msgstr ""
 
-#: models/character.py:86
+#: models/character.py:88
 msgid "wallet transactions"
 msgstr ""
 
-#: models/character.py:87
+#: models/character.py:89
 msgid "attributes"
 msgstr ""
 
-#: models/character.py:139
+#: models/character.py:141
 msgid "ok"
 msgstr ""
 
-#: models/character.py:140 models/sections.py:233
+#: models/character.py:142 models/sections.py:234
 msgid "in progress"
 msgstr ""
 
-#: models/character.py:141
+#: models/character.py:143
 msgid "incomplete"
 msgstr ""
 
-#: models/character.py:142
+#: models/character.py:144
 msgid "error"
 msgstr ""
 
-#: models/character.py:143
+#: models/character.py:145
 msgid "disabled"
 msgstr ""
 
-#: models/character.py:150
+#: models/character.py:152
 msgid "eve character"
 msgstr ""
 
-#: models/character.py:154
+#: models/character.py:156
 msgid "created at"
 msgstr ""
 
-#: models/character.py:158
+#: models/character.py:160
 msgid "is shared"
 msgstr ""
 
-#: models/character.py:163
+#: models/character.py:165
 msgid "is disabled"
 msgstr ""
 
-#: models/character.py:167
+#: models/character.py:169
 msgid "mailing lists"
 msgstr ""
 
-#: models/general.py:261 models/general.py:296
+#: models/character.py:177
+msgid "characters"
+msgstr ""
+
+#: models/character.py:1294 models/character.py:1295
+msgid "character update status"
+msgstr ""
+
+#: models/general.py:116
+msgid "compliance group designation"
+msgstr ""
+
+#: models/general.py:117
+msgid "compliance group designations"
+msgstr ""
+
+#: models/general.py:186
+msgid "locations"
+msgstr ""
+
+#: models/general.py:269 models/general.py:309
 msgid "description"
 msgstr ""
 
-#: models/general.py:268
+#: models/general.py:276
 msgid "is doctrine"
 msgstr ""
 
-#: models/general.py:270
+#: models/general.py:278
 msgid "This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
-#: models/general.py:276
+#: models/general.py:284
 msgid "is active"
 msgstr ""
 
-#: models/general.py:277
+#: models/general.py:285
 msgid "Whether this skill set group is in active use"
 msgstr ""
 
-#: models/general.py:285
+#: models/general.py:290
+msgid "skill set group"
+msgstr ""
+
+#: models/general.py:291
+msgid "skill set groups"
+msgstr ""
+
+#: models/general.py:298
 msgid "Doctrine: "
 msgstr ""
 
-#: models/general.py:304
+#: models/general.py:317
 msgid "ship type"
 msgstr ""
 
-#: models/general.py:307
+#: models/general.py:320
 msgid ""
 "Ship type is used for visual presentation only. All skill requirements must "
 "be explicitly defined."
 msgstr ""
 
-#: models/general.py:315
+#: models/general.py:328
 msgid "is visible"
 msgstr ""
 
-#: models/general.py:317
+#: models/general.py:330
 msgid ""
 "Non visible skill sets are not shown to users on their character sheet and "
 "used for audit purposes only."
 msgstr ""
 
-#: models/general.py:340
+#: models/general.py:339
+msgid "skill set"
+msgstr ""
+
+#: models/general.py:358 models/general.py:385
 msgid "skill"
 msgstr ""
 
-#: models/general.py:349
+#: models/general.py:367
 msgid "required level"
 msgstr ""
 
-#: models/general.py:356
+#: models/general.py:374
 msgid "recommended level"
 msgstr ""
 
-#: models/general.py:412 templates/memberaudit/reports.html:75
+#: models/general.py:433 templates/memberaudit/reports.html:75
 #: templates/memberaudit/reports.html:140
 #: templates/memberaudit/reports.html:214
 msgid "Alliance"
 msgstr ""
 
-#: models/general.py:413
+#: models/general.py:434
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
-#: models/general.py:414
+#: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
 #: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
-#: models/general.py:415
+#: models/general.py:436
 msgid "Mailing List"
 msgstr ""
 
-#: models/general.py:416
+#: models/general.py:437
 msgid "Unknown"
 msgstr ""
 
-#: models/sections.py:146
+#: models/sections.py:147
 msgid "excellent standing"
 msgstr ""
 
-#: models/sections.py:147
+#: models/sections.py:148
 msgid "good standing"
 msgstr ""
 
-#: models/sections.py:148
+#: models/sections.py:149
 msgid "neutral standing"
 msgstr ""
 
-#: models/sections.py:149
+#: models/sections.py:150
 msgid "bad standing"
 msgstr ""
 
-#: models/sections.py:150
+#: models/sections.py:151
 msgid "terrible standing"
 msgstr ""
 
-#: models/sections.py:204
+#: models/sections.py:205
 msgid "alliance"
 msgstr ""
 
-#: models/sections.py:205
+#: models/sections.py:206
 msgid "corporation"
 msgstr ""
 
-#: models/sections.py:206
+#: models/sections.py:207
 msgid "private"
 msgstr ""
 
-#: models/sections.py:207
+#: models/sections.py:208
 msgid "public"
 msgstr ""
 
-#: models/sections.py:227
+#: models/sections.py:228
 msgid "canceled"
 msgstr ""
 
-#: models/sections.py:228
+#: models/sections.py:229
 msgid "deleted"
 msgstr ""
 
-#: models/sections.py:229
+#: models/sections.py:230
 msgid "failed"
 msgstr ""
 
-#: models/sections.py:230
+#: models/sections.py:231
 msgid "finished"
 msgstr ""
 
-#: models/sections.py:231
+#: models/sections.py:232
 msgid "finished contractor"
 msgstr ""
 
-#: models/sections.py:232
+#: models/sections.py:233
 msgid "finished issuer"
 msgstr ""
 
-#: models/sections.py:234
+#: models/sections.py:235
 msgid "outstanding"
 msgstr ""
 
-#: models/sections.py:235
+#: models/sections.py:236
 msgid "rejected"
 msgstr ""
 
-#: models/sections.py:236
+#: models/sections.py:237
 msgid "reversed"
 msgstr ""
 
-#: models/sections.py:257
+#: models/sections.py:258
 msgid "auction"
 msgstr ""
 
-#: models/sections.py:258
+#: models/sections.py:259
 msgid "courier"
 msgstr ""
 
-#: models/sections.py:259
+#: models/sections.py:260
 msgid "item exchange"
 msgstr ""
 
-#: models/sections.py:260
+#: models/sections.py:261
 msgid "loan"
 msgstr ""
 
-#: models/sections.py:261
+#: models/sections.py:262
 msgid "unknown"
 msgstr ""
 
-#: models/sections.py:419
+#: models/sections.py:421
 msgid "[Multiple Items]"
 msgstr ""
 
 #: models/sections.py:520
 msgid "male"
 msgstr ""
 
@@ -1516,15 +1547,15 @@
 msgid "Character Finder"
 msgstr ""
 
 #: templates/memberaudit/partials/menu.html:50 views/reports.py:39
 msgid "Reports"
 msgstr ""
 
-#: templates/memberaudit/partials/menu.html:58 views/data_export.py:25
+#: templates/memberaudit/partials/menu.html:58 views/data_export.py:24
 msgid "Data Export"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/_compliance_color_code.html:3
 msgid "Color code:"
 msgstr ""
 
@@ -1668,13 +1699,13 @@
 msgstr ""
 
 #: views/characters.py:156
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
-#: views/data_export.py:55
+#: views/data_export.py:53
 #, python-format
 msgid ""
 "Data export for topic <strong>%s</strong> has been started. This can take a "
 "couple of minutes. You will get a notification once it is completed."
 msgstr ""
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_data_export.py` & `aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_load_eve.py` & `aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_reset_characters.py` & `aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_reset_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_stats.py` & `aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_update_characters.py` & `aa_memberaudit-2.7.0/memberaudit/management/commands/memberaudit_update_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/managers/character.py` & `aa_memberaudit-2.7.0/memberaudit/managers/character.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,36 +210,36 @@
 
                 # calc totals
                 qs = qs_base.filter(section__in=sections)
                 try:
                     first = qs.order_by("started_at").first()
                     last = qs.order_by("finished_at").last()
                     started_at = first.started_at
-                    finshed_at = last.finished_at
-                    duration = round((finshed_at - started_at).total_seconds(), 1)
+                    finished_at = last.finished_at
+                    duration = round((finished_at - started_at).total_seconds(), 1)
                 except (KeyError, AttributeError):
                     first = None
                     last = None
                     duration = None
                     started_at = None
-                    finshed_at = None
+                    finished_at = None
 
                 available_time = (
                     settings[f"MEMBERAUDIT_UPDATE_STALE_RING_{ring}"]
                     - settings["MEMBERAUDIT_UPDATE_STALE_OFFSET"]
                 ) * 60
                 throughput = (
                     floor(all_characters_count / duration * 3600) if duration else None
                 )
                 within_boundaries = duration < available_time if duration else None
                 update_stats[f"ring_{ring}"] = {
                     "total": {
                         "duration": duration,
                         "started_at": started_at,
-                        "finshed_at": finshed_at,
+                        "finished_at": finished_at,
                         "root_task_id": root_task_ids.get(ring),
                         "throughput_est": throughput,
                         "available_time": available_time,
                         "within_available_time": within_boundaries,
                     },
                     "max": {},
                     "sections": {},
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/managers/general.py` & `aa_memberaudit-2.7.0/memberaudit/managers/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime as dt
-from typing import Iterable, List, Tuple
+from typing import Iterable, List, Optional, Tuple
 
 from bravado.exception import HTTPForbidden, HTTPUnauthorized
 from celery_once import AlreadyQueued
 
 from django.contrib.auth.models import Group, User
 from django.db import models, transaction
 from django.db.models import Q
@@ -211,28 +211,26 @@
             "%s: Creating empty location for ID not matching any known pattern:", id
         )
         return self.get_or_create(id=id)
 
     def _station_update_or_create_dict(
         self, id: int, station: dict
     ) -> Tuple[models.Model, bool]:
-        if station.get("system_id"):
-            eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
-                id=station.get("system_id")
-            )
+        if system_id := station.get("system_id"):
+            eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(id=system_id)
         else:
             eve_solar_system = None
 
-        if station.get("type_id"):
-            eve_type, _ = EveType.objects.get_or_create_esi(id=station.get("type_id"))
+        if type_id := station.get("type_id"):
+            eve_type, _ = EveType.objects.get_or_create_esi(id=type_id)
         else:
             eve_type = None
 
-        if station.get("owner"):
-            owner, _ = EveEntity.objects.get_or_create_esi(id=station.get("owner"))
+        if owner_id := station.get("owner"):
+            owner, _ = EveEntity.objects.get_or_create_esi(id=owner_id)
         else:
             owner = None
 
         return self.update_or_create(
             id=id,
             defaults={
                 "name": station.get("name", ""),
@@ -274,28 +272,28 @@
         else:
             return self._structure_update_or_create_dict(id=id, structure=structure)
 
     def _structure_update_or_create_dict(
         self, id: int, structure: dict
     ) -> Tuple[models.Model, bool]:
         """creates a new Location object from a structure dict"""
-        if structure.get("solar_system_id"):
+        if solar_system_id := structure.get("solar_system_id"):
             eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
-                id=structure.get("solar_system_id")
+                id=solar_system_id
             )
         else:
             eve_solar_system = None
 
-        if structure.get("type_id"):
-            eve_type, _ = EveType.objects.get_or_create_esi(id=structure.get("type_id"))
+        if type_id := structure.get("type_id"):
+            eve_type, _ = EveType.objects.get_or_create_esi(id=type_id)
         else:
             eve_type = None
 
-        if structure.get("owner_id"):
-            owner, _ = EveEntity.objects.get_or_create_esi(id=structure.get("owner_id"))
+        if owner_id := structure.get("owner_id"):
+            owner, _ = EveEntity.objects.get_or_create_esi(id=owner_id)
         else:
             owner = None
 
         return self.update_or_create(
             id=id,
             defaults={
                 "name": structure.get("name", ""),
@@ -304,36 +302,36 @@
                 "owner": owner,
             },
         )
 
 
 class MailEntityManager(models.Manager):
     def get_or_create_esi(
-        self, id: int, category: str = None
+        self, id: int, category: Optional[str] = None
     ) -> Tuple[models.Model, bool]:
         return self._get_or_create_esi(id=id, category=category, update_async=False)
 
     def get_or_create_esi_async(
-        self, id: int, category: str = None
+        self, id: int, category: Optional[str] = None
     ) -> Tuple[models.Model, bool]:
         return self._get_or_create_esi(id=id, category=category, update_async=True)
 
     def _get_or_create_esi(
-        self, id: int, category: str, update_async: bool
+        self, id: int, category: Optional[str], update_async: bool
     ) -> Tuple[models.Model, bool]:
         id = int(id)
         try:
             return self.get(id=id), False
         except self.model.DoesNotExist:
             if update_async:
                 return self.update_or_create_esi_async(id=id, category=category)
             return self.update_or_create_esi(id=id, category=category)
 
     def update_or_create_esi(
-        self, id: int, category: str = None
+        self, id: int, category: Optional[str] = None
     ) -> Tuple[models.Model, bool]:
         """will try to update or create a new object from ESI
 
         Mailing lists can not be resolved from ESI
         and will therefore be created without name
 
         Trying to resolve a mailing list from ESI will result in an ESI error,
@@ -365,15 +363,15 @@
                 return self.update_or_create(
                     id=id,
                     defaults={"category": self.model.Category.MAILING_LIST},
                 )
             return self.update_or_create_from_eve_entity_id(id=id)
 
     def update_or_create_esi_async(
-        self, id: int, category: str = None
+        self, id: int, category: Optional[str] = None
     ) -> Tuple[models.Model, bool]:
         """Same as update_or_create_esi, but will create and return an empty object and delegate the ID resolution to a task (if needed),
         which will automatically retry on many common error conditions
         """
         id = int(id)
         try:
             obj = self.get(id=id)
@@ -471,15 +469,15 @@
         return new_mailing_lists
 
 
 class SkillSetManager(models.Manager):
     def update_or_create_from_fitting(
         self,
         fitting: Fitting,
-        user: User = None,
+        user: Optional[User] = None,
         skill_set_group=None,
         skill_set_name=None,
     ) -> Tuple[models.Model, bool]:
         """Update or create a skill set from a fitting."""
         if not skill_set_name:
             skill_set_name = fitting.name
         return self.update_or_create_from_skills(
@@ -488,15 +486,15 @@
             source=f"EFT fitting '{fitting.name}'",
             user=user,
             skill_set_group=skill_set_group,
             ship_type=fitting.ship_type,
         )
 
     def update_or_create_from_skill_plan(
-        self, skill_plan: SkillPlan, user: User = None, skill_set_group=None
+        self, skill_plan: SkillPlan, user: Optional[User] = None, skill_set_group=None
     ) -> Tuple[models.Model, bool]:
         """Update or create a skill set from a fitting."""
 
         return self.update_or_create_from_skills(
             name=skill_plan.name,
             skills=skill_plan.skills,
             source="imported skill plan",
@@ -505,17 +503,17 @@
         )
 
     def update_or_create_from_skills(
         self,
         name: str,
         skills: List[Skill],
         source: str,
-        user: User = None,
+        user: Optional[User] = None,
         skill_set_group=None,
-        ship_type: EveType = None,
+        ship_type: Optional[EveType] = None,
     ) -> Tuple[models.Model, bool]:
         """Update or create a skill set from skills."""
         from ..models import SkillSetSkill
 
         description = (
             f"Generated from {source} "
             f"by {user if user else '?'} "
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/managers/sections.py` & `aa_memberaudit-2.7.0/memberaudit/managers/sections.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,21 +97,25 @@
                 "%s: Removing %s obsolete contacts", character, len(obsolete_ids)
             )
             self.filter(character=character, eve_entity_id__in=obsolete_ids).delete()
 
         create_ids = incoming_ids.difference(existing_ids)
         if create_ids:
             self._create_new_contacts(
-                character=character, contacts_list=contacts_list, contact_ids=create_ids
+                character=character,
+                contacts_list=contacts_list,
+                contact_ids=list(create_ids),
             )
 
         update_ids = incoming_ids.difference(create_ids)
         if update_ids:
             self._update_existing_contacts(
-                character=character, contacts_list=contacts_list, contact_ids=update_ids
+                character=character,
+                contacts_list=contacts_list,
+                contact_ids=list(update_ids),
             )
 
         if not obsolete_ids and not create_ids and not update_ids:
             logger.info("%s: Contacts have not changed", character)
 
     def _create_new_contacts(
         self, character: models.Model, contacts_list: dict, contact_ids: list
@@ -898,17 +902,18 @@
 CharacterMiningLedgerEntryManager = CharacterMiningLedgerEntryManagerBase.from_queryset(
     CharacterMiningLedgerEntryQueryset
 )
 
 
 class CharacterShipManager(models.Manager):
     def update_for_character(self, character: models.Model, ship_info: dict):
-        eve_type, _ = EveType.objects.get_or_create_esi(
-            id=ship_info.get("ship_type_id")
-        )
+        ship_type_id = ship_info.get("ship_type_id")
+        if not ship_type_id:
+            return
+        eve_type, _ = EveType.objects.get_or_create_esi(id=ship_type_id)
         self.update_or_create(
             character=character,
             defaults={
                 "eve_type": eve_type,
                 "name": ship_info["ship_name"],
             },
         )
@@ -973,30 +978,30 @@
                 self._update_from_dict(
                     character=character, skills_list=skills_list, update_ids=update_ids
                 )
 
         if not obsolete_ids and not create_ids and not update_ids:
             logger.info("%s: Skills have not changed", character)
 
-    def _create_from_dict(self, character, skills_list: dict, create_ids: list):
+    def _create_from_dict(self, character, skills_list: dict, create_ids: set):
         logger.info("%s: Storing %s new skills", character, len(create_ids))
         skills = [
             self.model(
                 character=character,
                 eve_type=EveType.objects.get(id=skill_info.get("skill_id")),
                 active_skill_level=skill_info.get("active_skill_level"),
                 skillpoints_in_skill=skill_info.get("skillpoints_in_skill"),
                 trained_skill_level=skill_info.get("trained_skill_level"),
             )
             for skill_id, skill_info in skills_list.items()
             if skill_id in create_ids
         ]
         self.bulk_create(skills, batch_size=MEMBERAUDIT_BULK_METHODS_BATCH_SIZE)
 
-    def _update_from_dict(self, character, skills_list: dict, update_ids: list):
+    def _update_from_dict(self, character, skills_list: dict, update_ids: set):
         logger.info("%s: Updating %s skills", character, len(update_ids))
         update_pks = list(
             self.filter(character=character, eve_type_id__in=update_ids).values_list(
                 "pk", flat=True
             )
         )
         skills = self.in_bulk(update_pks)
@@ -1151,15 +1156,15 @@
             self.filter(character=character, date__lt=cutoff_datetime).delete()
 
         incoming_location_ids = {
             row.get("location_id") for row in transaction_list.values()
         }
         character._preload_all_locations(token, incoming_location_ids)
         type_ids = {row.get("type_id") for row in transaction_list.values()}
-        EveType.objects.bulk_get_or_create_esi(ids=type_ids)
+        EveType.objects.bulk_get_or_create_esi(ids=list(type_ids))
 
         with transaction.atomic():
             incoming_ids = set(transaction_list.keys())
             existing_ids = set(self.values_list("transaction_id", flat=True))
             create_ids = incoming_ids.difference(existing_ids)
             if not create_ids:
                 logger.info("%s: No new wallet transcations", character)
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/migrations/0001_initial_new.py` & `aa_memberaudit-2.7.0/memberaudit/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/migrations/0002_add_mining_ledger.py` & `aa_memberaudit-2.7.0/memberaudit/migrations/0002_add_mining_ledger.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/migrations/0003_add_notify_permission.py` & `aa_memberaudit-2.7.0/memberaudit/migrations/0003_add_notify_permission.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/migrations/0004_character_is_disabled.py` & `aa_memberaudit-2.7.0/memberaudit/migrations/0004_character_is_disabled.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/migrations/0005_add_fw_stats.py` & `aa_memberaudit-2.7.0/memberaudit/migrations/0005_add_fw_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/migrations/0006_add_localizations.py` & `aa_memberaudit-2.7.0/memberaudit/migrations/0006_add_localizations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/models/__init__.py` & `aa_memberaudit-2.7.0/memberaudit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/models/character.py` & `aa_memberaudit-2.7.0/memberaudit/models/character.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,16 @@
         "MailEntity", related_name="characters", verbose_name=_("mailing lists")
     )
 
     objects = CharacterManager()
 
     class Meta:
         default_permissions = ()
+        verbose_name = _("character")
+        verbose_name_plural = _("characters")
 
     def __str__(self) -> str:
         return f"{self.eve_character.character_name} (PK:{self.pk})"
 
     def __repr__(self) -> str:
         return f"Character(pk={self.pk}, eve_character='{self.eve_character}')"
 
@@ -241,35 +243,34 @@
         try:
             if self.user == user:  # shortcut for better performance
                 return True
         except AttributeError:
             pass
         return Character.objects.user_has_access(user).filter(pk=self.pk).exists()
 
-    def is_update_status_ok(self) -> bool:
+    def is_update_status_ok(self) -> Optional[bool]:
         """returns status of last update
 
         Returns:
         - True: If update was complete and without errors
         - False if there where any errors
         - None: if last update is incomplete
         """
         errors_count = self.update_status_set.filter(is_success=False).count()
         ok_count = self.update_status_set.filter(is_success=True).count()
         if errors_count > 0:
             return False
-        elif ok_count == len(Character.UpdateSection.choices):
+        if ok_count == len(Character.UpdateSection.choices):
             return True
-        else:
-            return None
+        return None
 
     @classmethod
     def update_section_time_until_stale(cls, section: str) -> dt.timedelta:
         """time until given update section is considered stale"""
-        ring = cls.UPDATE_SECTION_RINGS_MAP[section]
+        ring = cls.UPDATE_SECTION_RINGS_MAP[cls.UpdateSection(section)]
         if ring == 1:
             minutes = MEMBERAUDIT_UPDATE_STALE_RING_1
         elif ring == 2:
             minutes = MEMBERAUDIT_UPDATE_STALE_RING_2
         else:
             minutes = MEMBERAUDIT_UPDATE_STALE_RING_3
 
@@ -298,60 +299,65 @@
         except (CharacterUpdateStatus.DoesNotExist, ObjectDoesNotExist, AttributeError):
             return True
 
         deadline = now() - self.update_section_time_until_stale(section)
         return update_status.started_at < deadline
 
     def has_section_changed(
-        self, section: str, content: str, hash_num: int = 1
+        self, section: str, content: Any, hash_num: int = 1
     ) -> bool:
         """returns False if the content hash for this section has not changed, else True"""
         try:
-            section = self.update_status_set.get(section=section)
+            section_obj: CharacterUpdateStatus = self.update_status_set.get(
+                section=section
+            )
         except CharacterUpdateStatus.DoesNotExist:
             return True
-        else:
-            return section.has_changed(content=content, hash_num=hash_num)
+        return section_obj.has_changed(content=content, hash_num=hash_num)
 
     def update_section_content_hash(
-        self, section: str, content: str, hash_num: int = 1
-    ) -> bool:
+        self, section: str, content: Any, hash_num: int = 1
+    ) -> None:
         try:
-            section = self.update_status_set.get(section=section)
+            section_obj: CharacterUpdateStatus = self.update_status_set.get(
+                section=section
+            )
         except CharacterUpdateStatus.DoesNotExist:
-            section, _ = CharacterUpdateStatus.objects.get_or_create(
+            section_obj, _ = CharacterUpdateStatus.objects.get_or_create(
                 character=self, section=section
             )
-
-        section.update_content_hash(content=content, hash_num=hash_num)
+        section_obj.update_content_hash(content=content, hash_num=hash_num)
 
     def reset_update_section(
-        self, section: str, root_task_id: str = None, parent_task_id: str = None
+        self,
+        section: str,
+        root_task_id: Optional[str] = None,
+        parent_task_id: Optional[str] = None,
     ) -> "CharacterUpdateStatus":
         """resets status of given update section and returns it"""
         try:
-            section = self.update_status_set.get(section=section)
+            section_onj: CharacterUpdateStatus = self.update_status_set.get(
+                section=section
+            )
         except CharacterUpdateStatus.DoesNotExist:
-            section, _ = CharacterUpdateStatus.objects.get_or_create(
+            section_onj, _ = CharacterUpdateStatus.objects.get_or_create(
                 character=self, section=section
             )
-
-        section.reset(root_task_id, parent_task_id)
-        return section
+        section_onj.reset(root_task_id, parent_task_id)
+        return section_onj
 
     def is_section_updating(self, section: str) -> bool:
         """returns True if section is currently updating, or does not exist, else False"""
         try:
-            section = self.update_status_set.get(section=section)
+            section_obj = self.update_status_set.get(section=section)
         except CharacterUpdateStatus.DoesNotExist:
             return True
+        return section_obj.is_updating
 
-        return section.is_updating
-
-    def _preload_all_locations(self, token: Token, incoming_ids: set) -> list:
+    def _preload_all_locations(self, token: Token, incoming_ids: set) -> set:
         """loads location objects specified by given set
 
         returns list of existing location IDs after preload
         """
         existing_ids = set(Location.objects.values_list("id", flat=True))
         missing_ids = incoming_ids.difference(existing_ids)
         if missing_ids:
@@ -363,15 +369,14 @@
                     Location.objects.get_or_create_esi_async(
                         id=location_id, token=token
                     )
                 except ValueError:
                     pass
                 else:
                     existing_ids.add(location_id)
-
         return existing_ids
 
     def fetch_token(self, scopes=None) -> Token:
         """returns valid token for character
 
         Args:
         - scopes: Optionally provide the required scopes.
@@ -396,17 +401,18 @@
             title = f"{__title__}: Invalid or missing token for {self.eve_character}"
             message = (
                 f"{MEMBERAUDIT_APP_NAME} could not find a valid token for your "
                 f"character {self.eve_character}.\n"
                 f"Please re-add that character to {MEMBERAUDIT_APP_NAME} "
                 "at your earliest convenience to update your token."
             )
-            notify_throttled(
-                message_id=message_id, user=self.user, title=title, message=message
-            )
+            if self.user:
+                notify_throttled(
+                    message_id=message_id, user=self.user, title=title, message=message
+                )
             raise TokenError(f"Could not find a matching token for {self}")
         return token
 
     @fetch_token_for_character("esi-assets.read_assets.v1")
     def assets_build_list_from_esi(
         self, token: Token, force_update=False
     ) -> Optional[list]:
@@ -450,29 +456,32 @@
         else:
             logger.info("%s: Assets did not change", self)
             return None
 
     @fetch_token_for_character("esi-universe.read_structures.v1")
     def assets_preload_objects(self, token: Token, asset_list: list) -> None:
         """preloads objects needed to build the asset tree"""
+        if not asset_list:
+            return
         logger.info("%s: Preloading objects for asset tree", self)
         required_ids = {x["type_id"] for x in asset_list if "type_id" in x}
         existing_ids = set(EveType.objects.values_list("id", flat=True))
         missing_ids = required_ids.difference(existing_ids)
         if missing_ids:
             logger.info("%s: Loading %s missing types from ESI", self, len(missing_ids))
-            EveType.objects.bulk_get_or_create_esi(ids=missing_ids)
+            EveType.objects.bulk_get_or_create_esi(ids=list(missing_ids))
 
         assets_flat = {int(x["item_id"]): x for x in asset_list}
         incoming_location_ids = {
             x["location_id"]
             for x in assets_flat.values()
             if "location_id" in x and x["location_id"] not in assets_flat
         }
-        self._preload_all_locations(token=token, incoming_ids=incoming_location_ids)
+        if incoming_location_ids:
+            self._preload_all_locations(token=token, incoming_ids=incoming_location_ids)
 
     def update_character_details(self, force_update: bool = False):
         """syncs the character details for the given character"""
         from .sections import CharacterDetails
 
         logger.info("%s: Fetching character details from ESI", self)
         details = esi.client.Character.get_characters_character_id(
@@ -551,15 +560,18 @@
                 obj["start_location_id"]
                 for contract_id, obj in contracts_list.items()
                 if contract_id not in existing_ids
             }
             incoming_location_ids |= {
                 obj["end_location_id"] for obj in contracts_list.values()
             }
-            self._preload_all_locations(token=token, incoming_ids=incoming_location_ids)
+            if incoming_location_ids:
+                self._preload_all_locations(
+                    token=token, incoming_ids=incoming_location_ids
+                )
             self.contracts.update_for_character(self, contracts_list)
             self.update_section_content_hash(
                 section=self.UpdateSection.CONTRACTS, content=contracts_list
             )
         else:
             logger.info("%s: Contracts have not changed", self)
 
@@ -759,15 +771,16 @@
             # fetch related objects ahead of transaction
             if jump_clones_list:
                 incoming_location_ids = {
                     record["location_id"]
                     for record in jump_clones_info["jump_clones"]
                     if "location_id" in record
                 }
-                self._preload_all_locations(token, incoming_location_ids)
+                if incoming_location_ids:
+                    self._preload_all_locations(token, incoming_location_ids)
 
                 for jump_clone_info in jump_clones_list:
                     if jump_clone_info.get("implants"):
                         EveType.objects.bulk_get_or_create_esi(
                             ids=jump_clone_info.get("implants", [])
                         )
 
@@ -1079,15 +1092,15 @@
         return skills_list
 
     def _preload_types(self, skills_list: dict):
         if skills_list:
             incoming_ids = set(skills_list.keys())
             existing_ids = set(self.skills.values_list("eve_type_id", flat=True))
             new_ids = incoming_ids.difference(existing_ids)
-            EveType.objects.bulk_get_or_create_esi(ids=new_ids)
+            EveType.objects.bulk_get_or_create_esi(ids=list(new_ids))
 
     @fetch_token_for_character("esi-wallet.read_character_wallet.v1")
     def update_wallet_balance(self, token):
         """syncs the character's wallet balance"""
         from .sections import CharacterWalletBalance
 
         logger.info("%s: Fetching wallet balance from ESI", self)
@@ -1135,15 +1148,15 @@
         self.wallet_transactions.update_for_character(
             character=self,
             cutoff_datetime=data_retention_cutoff(),
             transactions=transactions,
             token=token,
         )
 
-    def _store_list_to_disk(self, lst: list, name: str):
+    def _store_list_to_disk(self, lst: Any, name: str):
         """stores the given list as JSON file to disk. For debugging
 
         Will store under memberaudit_logs/{DATE}/{CHARACTER_PK}_{NAME}.json
         """
         today_str = now().strftime("%Y%m%d")
         now_str = now().strftime("%Y%m%d%H%M")
         path = f"memberaudit_log/{today_str}"
@@ -1274,14 +1287,16 @@
         default_permissions = ()
         constraints = [
             models.UniqueConstraint(
                 fields=["character", "section"],
                 name="functional_pk_charactersyncstatus",
             )
         ]
+        verbose_name = _("character update status")
+        verbose_name_plural = _("character update status")
 
     def __str__(self) -> str:
         return f"{self.character}-{self.section}"
 
     @property
     def is_updating(self) -> bool:
         if not self.started_at and not self.finished_at:
@@ -1314,15 +1329,17 @@
 
     @staticmethod
     def _calculate_hash(content: Any) -> str:
         return hashlib.md5(
             json.dumps(content, cls=DjangoJSONEncoder).encode("utf-8")
         ).hexdigest()
 
-    def reset(self, root_task_id: str = None, parent_task_id: str = None) -> None:
+    def reset(
+        self, root_task_id: Optional[str] = None, parent_task_id: Optional[str] = None
+    ) -> None:
         """resets this update status"""
         self.is_success = None
         self.last_error_message = ""
         self.started_at = now()
         self.finished_at = None
         self.root_task_id = root_task_id if root_task_id else ""
         self.parent_task_id = parent_task_id if root_task_id else ""
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/models/general.py` & `aa_memberaudit-2.7.0/memberaudit/models/general.py`

 * *Files 13% similar despite different names*

```diff
@@ -107,14 +107,19 @@
     Note that compliance groups are fully managed by the app.
     """
 
     group = models.OneToOneField(Group, on_delete=models.CASCADE)
 
     objects = ComplianceGroupDesignationManager()
 
+    class Meta:
+        default_permissions = ()
+        verbose_name = _("compliance group designation")
+        verbose_name_plural = _("compliance group designations")
+
     def __str__(self) -> str:
         return str(self.group)
 
     def save(self, *args, **kwargs) -> None:
         self._ensure_internal_group()
         super().save(*args, **kwargs)
 
@@ -173,14 +178,16 @@
     )
     updated_at = models.DateTimeField(auto_now=True)
 
     objects = LocationManager()
 
     class Meta:
         default_permissions = ()
+        verbose_name = _("location")
+        verbose_name_plural = _("locations")
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return "{}(id={}, name='{}')".format(
             self.__class__.__name__, self.id, self.name
@@ -274,14 +281,19 @@
     is_active = models.BooleanField(
         default=True,
         db_index=True,
         verbose_name=_("is active"),
         help_text=_("Whether this skill set group is in active use"),
     )
 
+    class Meta:
+        default_permissions = ()
+        verbose_name = _("skill set group")
+        verbose_name_plural = _("skill set groups")
+
     def __str__(self) -> str:
         return str(self.name)
 
     @property
     def name_plus(self) -> str:
         return "{}{}".format(_("Doctrine: ") if self.is_doctrine else "", self.name)
 
@@ -318,14 +330,19 @@
             "Non visible skill sets are not shown to users "
             "on their character sheet and used for audit purposes only."
         ),
     )
 
     objects = SkillSetManager()
 
+    class Meta:
+        default_permissions = ()
+        verbose_name = _("skill set")
+        verbose_name_plural = _("skill sets")
+
     def __str__(self) -> str:
         return str(self.name)
 
 
 class SkillSetSkill(models.Model):
     """A specific skill within a skill set."""
 
@@ -360,14 +377,17 @@
     class Meta:
         constraints = [
             models.UniqueConstraint(
                 fields=["skill_set", "eve_type"],
                 name="functional_pk_skillsetskill",
             )
         ]
+        default_permissions = ()
+        verbose_name = _("skill")
+        verbose_name_plural = _("skills")
 
     def __str__(self) -> str:
         if self.recommended_level:
             recommended_level_str = (
                 " / " + MAP_ARABIC_TO_ROMAN_NUMBERS[self.recommended_level]
             )
         else:
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/models/sections.py` & `aa_memberaudit-2.7.0/memberaudit/models/sections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Character sections models
 """
+from typing import Optional
 
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
 from django.utils.html import strip_tags
 from django.utils.safestring import mark_safe
 from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
@@ -172,28 +173,28 @@
             )
         ]
 
     def __str__(self) -> str:
         return f"{self.character}-{self.eve_entity.name}"
 
     @property
-    def standing_level(self) -> int:
+    def standing_level(self) -> str:
         if self.standing > 5:
             return self.STANDING_EXCELLENT
 
         if 5 >= self.standing > 0:
             return self.STANDING_GOOD
 
         if self.standing == 0:
             return self.STANDING_NEUTRAL
 
         if 0 > self.standing >= -5:
             return self.STANDING_BAD
 
-        if self.standing < -5:
+        else:
             return self.STANDING_TERRIBLE
 
 
 class CharacterContract(models.Model):
     """An Eve Online contract belonging to a Character"""
 
     AVAILABILITY_ALLIANCE = "AL"
@@ -395,37 +396,36 @@
 
     @property
     def has_expired(self) -> bool:
         """returns true if this contract is expired"""
         return self.date_expired < now()
 
     @property
-    def hours_issued_2_completed(self) -> float:
-        if self.date_completed:
-            td = self.date_completed - self.date_issued
-            return td.days * 24 + (td.seconds / 3600)
-        else:
+    def hours_issued_2_completed(self) -> Optional[float]:
+        if not self.date_completed:
             return None
+        td = self.date_completed - self.date_issued
+        return td.days * 24 + (td.seconds / 3600)
 
     def summary(self) -> str:
         """return summary text for this contract"""
         if self.contract_type == CharacterContract.TYPE_COURIER:
-            summary = (
+            if not self.start_location or not self.end_location:
+                return ""
+            return (
                 f"{self.start_location.eve_solar_system} >> "
                 f"{self.end_location.eve_solar_system} "
                 f"({self.volume:.0f} m3)"
             )
-        else:
-            if self.items.filter(is_included=True).count() > 1:
-                summary = _("[Multiple Items]")
-            else:
-                first_item = self.items.first()
-                summary = first_item.eve_type.name if first_item else "(no items)"
 
-        return summary
+        if self.items.filter(is_included=True).count() > 1:
+            return _("[Multiple Items]")
+
+        first_item = self.items.first()
+        return first_item.eve_type.name if first_item else "(no items)"
 
 
 class CharacterContractBid(models.Model):
     contract = models.ForeignKey(
         CharacterContract, on_delete=models.CASCADE, related_name="bids"
     )
     bid_id = models.PositiveIntegerField(db_index=True)
@@ -582,51 +582,51 @@
         return mark_safe(eve_xml_to_html(self.description, add_default_style=True))
 
 
 class CharacterFwStats(models.Model):
     """Faction Warfare statistics of a character"""
 
     RANKS = {
-        EveFactionId.AMARR_EMPIRE: (
+        EveFactionId.AMARR_EMPIRE.value: (
             _("Paladin Crusader"),
             _("Templar Lieutenant"),
             _("Cardinal Lieutenant"),
             _("Arch Lieutenant"),
             _("Imperial Major"),
             _("Marshal Commander"),
             _("Imperator Commander"),
             _("Tribunus Colonel"),
             _("Legatus Commodore"),
             _("Divine Commodore"),
         ),
-        EveFactionId.CALDARI_STATE: (
+        EveFactionId.CALDARI_STATE.value: (
             _("Protectorate Ensign"),
             _("Second Lieutenant"),
             _("First Lieutenant"),
             _("Captain"),
             _("Major"),
             _("Lieutenant Colonel"),
             _("Colonel"),
             _("Wing Commander"),
             _("Strike Commander"),
             _("Brigadier General"),
         ),
-        EveFactionId.GALLENTE_FEDERATION: (
+        EveFactionId.GALLENTE_FEDERATION.value: (
             _("Federation Minuteman"),
             _("Defender Lieutenant"),
             _("Guardian Lieutenant"),
             _("Lieutenant Sentinel"),
             _("Shield Commander"),
             _("Aegis Commander"),
             _("Vice Commander"),
             _("Major General"),
             _("Lieutenant General"),
             _("Luminaire General"),
         ),
-        EveFactionId.MINMATAR_REPUBLIC: (
+        EveFactionId.MINMATAR_REPUBLIC.value: (
             _("Nation Warrior"),
             _("Spike Lieutenant"),
             _("Spear Lieutenant"),
             _("Venge Captain"),
             _("Lance Commander"),
             _("Blade Commander"),
             _("Talon Commander"),
@@ -659,21 +659,21 @@
         default_permissions = ()
 
     def __str__(self) -> str:
         return str(self.character)
 
     def current_rank_name(self) -> str:
         """Name of current rank or empty string when not enlisted."""
-        if not self.faction:
+        if not self.faction_id or not self.current_rank:
             return ""
         return self.rank_name_generic(self.faction_id, self.current_rank)
 
     def highest_rank_name(self) -> str:
         """Name of highest rank or empty string when not enlisted."""
-        if not self.faction:
+        if not self.faction_id or not self.current_rank:
             return ""
         return self.rank_name_generic(self.faction_id, self.current_rank)
 
     @classmethod
     def rank_name_generic(cls, faction_id: int, rank_id: int) -> str:
         """Name of requested rank.
 
@@ -1034,15 +1034,15 @@
 
     def __str__(self) -> str:
         return f"{self.character}-{self.queue_position}"
 
     @property
     def is_active(self) -> bool:
         """Returns true when this skill is currently being trained"""
-        return self.finish_date and self.queue_position == 0
+        return bool(self.finish_date) and self.queue_position == 0
 
 
 class CharacterSkillSetCheck(models.Model):
     character = models.ForeignKey(
         Character, on_delete=models.CASCADE, related_name="skill_set_checks"
     )
     skill_set = models.ForeignKey("SkillSet", on_delete=models.CASCADE)
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/character_viewer.css` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/character_viewer.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/character_viewer.min.css` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/character_viewer.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/global.css` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/global.min.css` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/global.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/launcher.css` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/launcher.min.css` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/launcher.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/memberaudit.css` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/memberaudit.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/memberaudit.min.css` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/memberaudit.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/reports.css` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/css/reports.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/charisma.png` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/charisma.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/eve-prism.png` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/eve-prism.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/evesearch.png` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/evesearch.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/intelligence.png` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/intelligence.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/memory.png` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/memory.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/perception.png` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/perception.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/willpower.png` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/images/willpower.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/moment/moment.min.js` & `aa_memberaudit-2.7.0/memberaudit/static/memberaudit/vendor/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/swagger.json` & `aa_memberaudit-2.7.0/memberaudit/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tasks.py` & `aa_memberaudit-2.7.0/memberaudit/tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -268,16 +268,16 @@
     }
 )
 def update_character_section(
     self,
     character_pk: int,
     section: str,
     force_update: bool = False,
-    root_task_id: str = None,
-    parent_task_id: str = None,
+    root_task_id: Optional[str] = None,
+    parent_task_id: Optional[str] = None,
     **kwargs,
 ) -> None:
     """Task that updates the section of a character"""
     fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
@@ -301,15 +301,15 @@
 def _character_update_with_error_logging(
     self, character: Character, section: str, method: object, *args, **kwargs
 ):
     """Facilitate catching and logging of exceptions potentially occurring
     during a character update.
     """
     try:
-        return method(*args, **kwargs)
+        return method(*args, **kwargs)  # type: ignore
     except Exception as ex:
         error_message = f"{type(ex).__name__}: {str(ex)}"
         logger.error(
             "%s: %s: Error ocurred: %s",
             character,
             Character.UpdateSection.display_name(section),
             error_message,
@@ -362,16 +362,16 @@
         **{"once": {"keys": ["character_pk", "force_update"]}},
     }
 )
 def update_character_assets(
     self,
     character_pk: int,
     force_update: bool = False,
-    root_task_id: str = None,
-    parent_task_id: str = None,
+    root_task_id: Optional[str] = None,
+    parent_task_id: Optional[str] = None,
 ) -> None:
     """Main tasks for updating the character's assets"""
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     logger.info(
         "%s: Updating %s",
@@ -604,16 +604,16 @@
         **{"once": {"keys": ["character_pk", "force_update"]}},
     }
 )
 def update_character_mails(
     self,
     character_pk: int,
     force_update: bool = False,
-    root_task_id: str = None,
-    parent_task_id: str = None,
+    root_task_id: Optional[str] = None,
+    parent_task_id: Optional[str] = None,
 ) -> None:
     """Main task for updating mails of a character"""
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     section = Character.UpdateSection.MAILS
     logger.info(
@@ -736,16 +736,16 @@
         **{"once": {"keys": ["character_pk", "force_update"]}},
     }
 )
 def update_character_contacts(
     self,
     character_pk: int,
     force_update: bool = False,
-    root_task_id: str = None,
-    parent_task_id: str = None,
+    root_task_id: Optional[str] = None,
+    parent_task_id: Optional[str] = None,
 ) -> None:
     """Main task for updating contacts of a character"""
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     section = Character.UpdateSection.CONTACTS
     character.reset_update_section(
@@ -810,16 +810,16 @@
         **{"once": {"keys": ["character_pk", "force_update"]}},
     }
 )
 def update_character_contracts(
     self,
     character_pk: int,
     force_update: bool = False,
-    root_task_id: str = None,
-    parent_task_id: str = None,
+    root_task_id: Optional[str] = None,
+    parent_task_id: Optional[str] = None,
 ) -> None:
     """Main task for updating contracts of a character"""
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     section = Character.UpdateSection.CONTRACTS
     character.reset_update_section(
@@ -838,15 +838,15 @@
         update_unresolved_eve_entities.si().set(priority=priority),
     ).delay()
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
 def update_character_contract_headers(
     self, character_pk: int, force_update: bool = False
-) -> bool:
+):
     fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     _character_update_with_error_logging(
         self,
         character,
@@ -937,15 +937,18 @@
 
 
 # special tasks for updating wallet
 
 
 @shared_task(**{**TASK_DEFAULTS_BIND_ONCE, **{"once": {"keys": ["character_pk"]}}})
 def update_character_wallet_journal(
-    self, character_pk: int, root_task_id: str = None, parent_task_id: str = None
+    self,
+    character_pk: int,
+    root_task_id: Optional[str] = None,
+    parent_task_id: Optional[str] = None,
 ) -> None:
     """Main task for updating wallet journal of a character"""
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     section = Character.UpdateSection.WALLET_JOURNAL
     character.reset_update_section(
@@ -1025,15 +1028,15 @@
         )
         raise self.retry(countdown=ex.retry_in) from ex
 
 
 @shared_task(
     **{**TASK_DEFAULTS_ONCE, **{"once": {"keys": ["id"]}, "max_retries": None}}
 )
-def update_mail_entity_esi(id: int, category: str = None):
+def update_mail_entity_esi(id: int, category: Optional[str] = None):
     """Updates a mail entity object from ESI
     and retries later if the ESI error limit has already been reached
     """
     MailEntity.objects.update_or_create_esi(id=id, category=category)
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
@@ -1071,46 +1074,46 @@
     """Delete a member audit character"""
     character = Character.objects.get(pk=character_pk)
     logger.info("%s: Deleting character", character)
     character.delete()
 
 
 @shared_task(**TASK_DEFAULTS_BIND)
-def export_data(self, user_pk: int = None) -> None:
+def export_data(self, user_pk: Optional[int] = None) -> None:
     """Export data to files."""
     priority = _get_task_priority(self) or MEMBERAUDIT_TASKS_LOW_PRIORITY
     tasks = [
         _export_data_for_topic.si(topic).set(priority=priority)
         for topic in data_exporters.DataExporter.topics
     ]
     if user_pk:
         tasks.append(_export_data_inform_user.si(user_pk))
     chain(tasks).delay()
 
 
 @shared_task(**TASK_DEFAULTS_BIND)
-def export_data_for_topic(self, topic: str, user_pk: int) -> str:
+def export_data_for_topic(self, topic: str, user_pk: int):
     priority = _get_task_priority(self) or MEMBERAUDIT_TASKS_LOW_PRIORITY
     chain(
         _export_data_for_topic.si(topic).set(priority=priority),
         _export_data_inform_user.si(user_pk, topic).set(priority=priority),
     ).delay()
 
 
 @shared_task(**TASK_DEFAULTS_ONCE)
-def _export_data_for_topic(topic: str, destination_folder: str = None) -> str:
+def _export_data_for_topic(topic: str, destination_folder: Optional[str] = None) -> str:
     """Export data for given topic into a zipped file in destination."""
     file_path = data_exporters.export_topic_to_archive(
         topic=topic, destination_folder=destination_folder
     )
     return str(file_path)
 
 
 @shared_task(**TASK_DEFAULTS)
-def _export_data_inform_user(user_pk: int, topic: str = None):
+def _export_data_inform_user(user_pk: int, topic: Optional[str] = None):
     user = User.objects.get(pk=user_pk)
     if topic:
         title = f"{__title__}: Data export for {topic} completed"
         message = f"Data export has been completed for topic {topic}."
     else:
         title = f"{__title__}: Full data export completed"
         message = (
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html` & `aa_memberaudit-2.7.0/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/skillset/import_skills.html` & `aa_memberaudit-2.7.0/memberaudit/templates/admin/memberaudit/skillset/import_skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/character_finder.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/character_finder.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/character_viewer.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/data_export.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/data_export.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/launcher.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/launcher.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/contract.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/contract.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/mail.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/mail.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/overview.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/overview.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/menu.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/solar_system.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/partials/solar_system.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/reports.html` & `aa_memberaudit-2.7.0/memberaudit/templates/memberaudit/reports.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/core/test_core_xml_converter.py` & `aa_memberaudit-2.7.0/memberaudit/tests/core/test_core_xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/core/test_data_exporters.py` & `aa_memberaudit-2.7.0/memberaudit/tests/core/test_data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/core/test_eft_parser.py` & `aa_memberaudit-2.7.0/memberaudit/tests/core/test_eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/core/test_fittings.py` & `aa_memberaudit-2.7.0/memberaudit/tests/core/test_fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/core/test_skill_plans.py` & `aa_memberaudit-2.7.0/memberaudit/tests/core/test_skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/core/test_skills.py` & `aa_memberaudit-2.7.0/memberaudit/tests/core/test_skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/managers/test_character.py` & `aa_memberaudit-2.7.0/memberaudit/tests/managers/test_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/managers/test_general.py` & `aa_memberaudit-2.7.0/memberaudit/tests/managers/test_general.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import datetime as dt
 from unittest.mock import MagicMock, patch
 
 from bravado.exception import HTTPForbidden, HTTPNotFound, HTTPUnauthorized
 from celery_once import AlreadyQueued
 
 from django.core.cache import cache
-from django.test import TestCase, override_settings
+from django.test import override_settings
 from django.utils.timezone import now
 from eveuniverse.models import EveEntity, EveSolarSystem, EveType
 
 from allianceauth.eveonline.models import EveCorporationInfo
 from allianceauth.notifications.models import Notification
 from app_utils.esi import EsiStatus, fetch_esi_status
-from app_utils.esi_testing import BravadoResponseStub
+from app_utils.esi_testing import BravadoOperationStub, BravadoResponseStub
 from app_utils.testing import (
     NoSocketsTestCase,
     create_authgroup,
     create_state,
     create_user_from_evecharacter,
 )
 
@@ -34,61 +34,72 @@
     create_skill,
     create_skill_plan,
     create_skill_set_group,
 )
 from ..testdata.load_entities import load_entities
 from ..testdata.load_eveuniverse import load_eveuniverse
 from ..utils import (
+    NoSocketsTestCaseFixtures,
     add_auth_character_to_user,
     add_memberaudit_character_to_user,
     create_memberaudit_character,
 )
 
 MANAGERS_PATH = "memberaudit.managers.general"
 TASKS_PATH = "memberaudit.tasks"
 
 
+@patch(
+    "allianceauth.authentication.models.notify", lambda *args, **kwargs: None
+)  # state changes trigger notify
+@patch(MANAGERS_PATH + ".notify", spec=True)
 class TestComplianceGroupDesignation(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
 
-    def test_should_add_group_to_compliant_user_and_notify(self):
+    def test_should_add_group_to_compliant_user_and_notify(self, mock_notify):
         # given
         compliance_group = create_compliance_group()
         other_group = create_authgroup(internal=True)
         user, _ = create_user_from_evecharacter(
             1001, permissions=["memberaudit.basic_access"]
         )
         add_memberaudit_character_to_user(user, 1001)
         # when
         ComplianceGroupDesignation.objects.update_user(user)
         # then
         self.assertIn(compliance_group, user.groups.all())
         self.assertNotIn(other_group, user.groups.all())
-        self.assertTrue(
-            user.notification_set.filter(level=Notification.Level.SUCCESS).exists()
-        )
+        self.assertEqual(mock_notify.call_count, 1)
+        args, kwargs = mock_notify.call_args
+        self.assertEqual(kwargs["level"], Notification.Level.SUCCESS)
+        self.assertEqual(args[0], user)
 
-    def test_should_add_state_group_to_compliant_user_when_state_matches(self):
+    def test_should_add_state_group_to_compliant_user_when_state_matches(
+        self, mock_notify
+    ):
         # given
         member_corporation = EveCorporationInfo.objects.get(corporation_id=2001)
         my_state = create_state(member_corporations=[member_corporation], priority=200)
         compliance_group = create_compliance_group(states=[my_state])
+
         user, _ = create_user_from_evecharacter(
             1001, permissions=["memberaudit.basic_access"]
         )
         add_memberaudit_character_to_user(user, 1001)
         # when
         ComplianceGroupDesignation.objects.update_user(user)
         # then
         self.assertIn(compliance_group, user.groups.all())
 
-    def test_should_not_add_state_group_to_compliant_user_when_state_not_matches(self):
+    def test_should_not_add_state_group_to_compliant_user_when_state_not_matches(
+        self, mock_notify
+    ):
         # given
         my_state = create_state(priority=200)
         compliance_group = create_compliance_group(states=[my_state])
         user, _ = create_user_from_evecharacter(
             1001, permissions=["memberaudit.basic_access"]
         )
         add_memberaudit_character_to_user(user, 1001)
@@ -108,46 +119,46 @@
     #     )
     #     add_memberaudit_character_to_user(user, 1001)
     #     # when
     #     ComplianceGroupDesignation.objects.update_user(user)
     #     # then
     #     self.assertIn(compliance_group, user.groups.all())
 
-    def test_should_add_multiple_groups_to_compliant_user(self):
+    def test_should_add_multiple_groups_to_compliant_user(self, mock_notify):
         # given
         compliance_group_1 = create_compliance_group()
         compliance_group_2 = create_compliance_group()
         user, _ = create_user_from_evecharacter(
             1001, permissions=["memberaudit.basic_access"]
         )
         add_memberaudit_character_to_user(user, 1001)
         # when
         ComplianceGroupDesignation.objects.update_user(user)
         # then
         self.assertIn(compliance_group_1, user.groups.all())
         self.assertIn(compliance_group_2, user.groups.all())
 
-    def test_should_remove_group_from_non_compliant_user_and_notify(self):
+    def test_should_remove_group_from_non_compliant_user_and_notify(self, mock_notify):
         # given
         compliance_group = create_compliance_group()
         other_group = create_authgroup(internal=True)
         user, _ = create_user_from_evecharacter(
             1001, permissions=["memberaudit.basic_access"]
         )
         user.groups.add(compliance_group, other_group)
         # when
         ComplianceGroupDesignation.objects.update_user(user)
         # then
         self.assertNotIn(compliance_group, user.groups.all())
         self.assertIn(other_group, user.groups.all())
-        self.assertTrue(
-            user.notification_set.filter(level=Notification.Level.WARNING).exists()
-        )
+        args, kwargs = mock_notify.call_args
+        self.assertEqual(kwargs["level"], Notification.Level.WARNING)
+        self.assertEqual(args[0], user)
 
-    def test_should_remove_multiple_groups_from_non_compliant_user(self):
+    def test_should_remove_multiple_groups_from_non_compliant_user(self, mock_notify):
         # given
         compliance_group_1 = create_compliance_group()
         compliance_group_2 = create_compliance_group()
         other_group = create_authgroup(internal=True)
         user, _ = create_user_from_evecharacter(
             1001, permissions=["memberaudit.basic_access"]
         )
@@ -156,41 +167,41 @@
         ComplianceGroupDesignation.objects.update_user(user)
         # then
         self.assertNotIn(compliance_group_1, user.groups.all())
         self.assertNotIn(compliance_group_2, user.groups.all())
         self.assertIn(other_group, user.groups.all())
 
     def test_user_with_one_registered_and_one_unregistered_characater_is_not_compliant(
-        self,
+        self, mock_notify
     ):
         # given
         compliance_group = create_compliance_group()
         user, _ = create_user_from_evecharacter(
             1001, permissions=["memberaudit.basic_access"]
         )
         add_memberaudit_character_to_user(user, 1001)
         add_auth_character_to_user(user, 1002)
         user.groups.add(compliance_group)
         # when
         ComplianceGroupDesignation.objects.update_user(user)
         # then
         self.assertNotIn(compliance_group, user.groups.all())
 
-    def test_user_without_basic_permission_is_not_compliant(self):
+    def test_user_without_basic_permission_is_not_compliant(self, mock_notify):
         # given
         compliance_group = create_compliance_group()
         user, _ = create_user_from_evecharacter(1001)
         add_memberaudit_character_to_user(user, 1001)
         user.groups.add(compliance_group)
         # when
         ComplianceGroupDesignation.objects.update_user(user)
         # then
         self.assertNotIn(compliance_group, user.groups.all())
 
-    def test_should_add_missing_groups_if_user_remains_compliant(self):
+    def test_should_add_missing_groups_if_user_remains_compliant(self, mock_notify):
         # given
         compliance_group_1 = create_compliance_group()
         compliance_group_2 = create_compliance_group()
         other_group = create_authgroup(internal=True)
         user, _ = create_user_from_evecharacter(
             1001, permissions=["memberaudit.basic_access"]
         )
@@ -219,26 +230,26 @@
 
         obj, created = MailEntity.objects.get_or_create_esi(id=1234)
 
         self.assertFalse(created)
         self.assertEqual(obj.category, MailEntity.Category.CHARACTER)
         self.assertEqual(obj.name, "John Doe")
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
+    @patch(MANAGERS_PATH + ".fetch_esi_status", spec=True)
     def test_get_or_create_esi_2(self, mock_fetch_esi_status):
         """When entity does not exist, create it from ESI / existing EveEntity"""
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
 
         obj, created = MailEntity.objects.get_or_create_esi(id=1001)
 
         self.assertTrue(created)
         self.assertEqual(obj.category, MailEntity.Category.CHARACTER)
         self.assertEqual(obj.name, "Bruce Wayne")
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
+    @patch(MANAGERS_PATH + ".fetch_esi_status", spec=True)
     def test_update_or_create_esi_1(self, mock_fetch_esi_status):
         """When entity does not exist, create it from ESI / existing EveEntity"""
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
 
         obj, created = MailEntity.objects.update_or_create_esi(id=1001)
 
         self.assertTrue(created)
@@ -271,15 +282,17 @@
         # method must not create an EveEntity object for the mailing list
         self.assertFalse(EveEntity.objects.filter(id=9001).exists())
 
     @patch(MANAGERS_PATH + ".fetch_esi_status", MagicMock(return_value=MagicMock()))
     def test_update_or_create_esi_4(self):
         """When entity does not exist and is a mailing list, then create it."""
         # when
-        with patch(MANAGERS_PATH + ".EveEntity.objects.get_or_create_esi") as m:
+        with patch(
+            MANAGERS_PATH + ".EveEntity.objects.get_or_create_esi", spec=True
+        ) as m:
             m.return_value = None, False
             obj, created = MailEntity.objects.update_or_create_esi(id=9001)
         # when
         self.assertTrue(created)
         self.assertEqual(obj.id, 9001)
         self.assertEqual(obj.category, MailEntity.Category.MAILING_LIST)
 
@@ -396,16 +409,16 @@
 
         MailEntity.objects.bulk_update_names([obj_1001], keep_names=True)
 
         self.assertEqual(obj_1001.name, "John Doe")
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-@patch(MANAGERS_PATH + ".fetch_esi_status")
-class TestMailEntityManagerAsync(TestCase):
+@patch(MANAGERS_PATH + ".fetch_esi_status", spec=True)
+class TestMailEntityManagerAsync(NoSocketsTestCaseFixtures):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
 
     def test_get_or_create_esi_async_1(self, mock_fetch_esi_status):
         """When entity already exists, return it"""
@@ -520,27 +533,27 @@
 @patch(MANAGERS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 class TestMailEntityManagerAsync2(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
 
-    @patch(TASKS_PATH + ".update_mail_entity_esi")
+    @patch(TASKS_PATH + ".update_mail_entity_esi", spec=True)
     def test_should_create_new_object_and_try_to_resolve(
         self, mock_task_update_mail_entity_esi
     ):
         # when
         obj, created = MailEntity.objects.update_or_create_esi_async(1001)
         # then
         self.assertTrue(created)
         self.assertEqual(obj.category, MailEntity.Category.UNKNOWN)
         self.assertEqual(obj.name, "")
         self.assertTrue(mock_task_update_mail_entity_esi.apply_async.called)
 
-    @patch("memberaudit.tasks.update_mail_entity_esi")
+    @patch("memberaudit.tasks.update_mail_entity_esi", spec=True)
     def test_should_create_new_object_and_try_to_resolve_and_ignore_already_queued(
         self, mock_task_update_mail_entity_esi
     ):
         # given
         mock_task_update_mail_entity_esi.apply_async.side_effect = AlreadyQueued(10)
         # when
         obj, created = MailEntity.objects.update_or_create_esi_async(1001)
@@ -548,15 +561,16 @@
         self.assertTrue(created)
         self.assertEqual(obj.category, MailEntity.Category.UNKNOWN)
         self.assertEqual(obj.name, "")
         self.assertTrue(mock_task_update_mail_entity_esi.apply_async.called)
 
 
 @patch(MANAGERS_PATH + ".esi")
-class TestLocationManager(NoSocketsTestCase):
+@patch(MANAGERS_PATH + ".fetch_esi_status", spec=True)
+class TestLocationManagerStructures(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         cls.jita = EveSolarSystem.objects.get(id=30000142)
         cls.amamake = EveSolarSystem.objects.get(id=30002537)
@@ -566,32 +580,52 @@
         cls.corporation_2001 = EveEntity.objects.get(id=2001)
         cls.corporation_2002 = EveEntity.objects.get(id=2002)
         cls.character = create_memberaudit_character(1001)
         cls.token = (
             cls.character.eve_character.character_ownership.user.token_set.first()
         )
 
-    # Structures
-
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
     def test_can_create_structure(self, mock_fetch_esi_status, mock_esi):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client = esi_client_stub
 
         obj, created = Location.objects.update_or_create_esi(
             id=1000000000001, token=self.token
         )
         self.assertTrue(created)
         self.assertEqual(obj.id, 1000000000001)
         self.assertEqual(obj.name, "Amamake - Test Structure Alpha")
         self.assertEqual(obj.eve_solar_system, self.amamake)
         self.assertEqual(obj.eve_type, self.astrahus)
         self.assertEqual(obj.owner, self.corporation_2001)
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
+    def test_can_handle_incomplete_data_from_esi(self, mock_fetch_esi_status, mock_esi):
+        # given
+        mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
+        mock_esi.client.Universe.get_universe_structures_structure_id.return_value = (
+            BravadoOperationStub(
+                {
+                    "owner_id": None,
+                    "name": "Incomplete data",
+                    "solar_system_id": 30002537,
+                }
+            )
+        )
+        # when
+        obj, created = Location.objects.update_or_create_esi(
+            id=1000000000666, token=self.token
+        )
+        # then
+        self.assertTrue(created)
+        self.assertEqual(obj.id, 1000000000666)
+        self.assertEqual(obj.name, "Incomplete data")
+        self.assertEqual(obj.eve_solar_system, self.amamake)
+        self.assertIsNone(obj.eve_type)
+        self.assertIsNone(obj.owner)
+
     def test_can_update_structure(self, mock_fetch_esi_status, mock_esi):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client = esi_client_stub
 
         obj, _ = Location.objects.update_or_create_esi(
             id=1000000000001, token=self.token
         )
@@ -606,15 +640,14 @@
         self.assertFalse(created)
         self.assertEqual(obj.id, 1000000000001)
         self.assertEqual(obj.name, "Amamake - Test Structure Alpha")
         self.assertEqual(obj.eve_solar_system, self.amamake)
         self.assertEqual(obj.eve_type, self.astrahus)
         self.assertEqual(obj.owner, self.corporation_2001)
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
     def test_does_not_update_existing_location_during_grace_period(
         self, mock_fetch_esi_status, mock_esi
     ):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client = esi_client_stub
 
         obj_existing = Location.objects.create(
@@ -626,26 +659,24 @@
         )
         obj, created = Location.objects.get_or_create_esi(
             id=1000000000001, token=self.token
         )
         self.assertFalse(created)
         self.assertEqual(obj, obj_existing)
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
     def test_always_update_existing_empty_locations_after_grace_period_1(
         self, mock_fetch_esi_status, mock_esi
     ):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client = esi_client_stub
 
         Location.objects.create(id=1000000000001)
         obj, _ = Location.objects.get_or_create_esi(id=1000000000001, token=self.token)
         self.assertIsNone(obj.eve_solar_system)
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
     def test_always_update_existing_empty_locations_after_grace_period_2(
         self, mock_fetch_esi_status, mock_esi
     ):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client = esi_client_stub
 
         mocked_update_at = now() - dt.timedelta(minutes=6)
@@ -654,15 +685,14 @@
         ):
             Location.objects.create(id=1000000000001)
             obj, _ = Location.objects.get_or_create_esi(
                 id=1000000000001, token=self.token
             )
         self.assertEqual(obj.eve_solar_system, self.amamake)
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
     @patch(MANAGERS_PATH + ".MEMBERAUDIT_LOCATION_STALE_HOURS", 24)
     def test_always_update_existing_locations_which_are_stale(
         self, mock_fetch_esi_status, mock_esi
     ):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client = esi_client_stub
 
@@ -679,91 +709,84 @@
             )
         obj, created = Location.objects.get_or_create_esi(
             id=1000000000001, token=self.token
         )
         self.assertFalse(created)
         self.assertEqual(obj.eve_solar_system, self.amamake)
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
     def test_propagates_http_error_on_structure_create(
         self, mock_fetch_esi_status, mock_esi
     ):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client = esi_client_stub
 
         with self.assertRaises(HTTPNotFound):
             Location.objects.update_or_create_esi(id=1000000000099, token=self.token)
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
     def test_always_creates_empty_location_for_invalid_ids(
         self, mock_fetch_esi_status, mock_esi
     ):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client = esi_client_stub
 
         obj, created = Location.objects.update_or_create_esi(
             id=80000000, token=self.token
         )
         self.assertTrue(created)
         self.assertTrue(obj.is_empty)
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
     def test_propagates_exceptions_on_structure_create(
         self, mock_fetch_esi_status, mock_esi
     ):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client.Universe.get_universe_structures_structure_id.side_effect = (
             RuntimeError
         )
 
         with self.assertRaises(RuntimeError):
             Location.objects.update_or_create_esi(id=1000000000099, token=self.token)
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
     def test_can_create_empty_location_on_access_error_1(
         self, mock_fetch_esi_status, mock_esi
     ):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client.Universe.get_universe_structures_structure_id.side_effect = (
             HTTPForbidden(response=BravadoResponseStub(403, "Test exception"))
         )
 
         obj, created = Location.objects.update_or_create_esi(
             id=1000000000099, token=self.token
         )
         self.assertTrue(created)
         self.assertEqual(obj.id, 1000000000099)
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
     def test_can_create_empty_location_on_access_error_2(
         self, mock_fetch_esi_status, mock_esi
     ):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client.Universe.get_universe_structures_structure_id.side_effect = (
             HTTPUnauthorized(response=BravadoResponseStub(401, "Test exception"))
         )
 
         obj, created = Location.objects.update_or_create_esi(
             id=1000000000099, token=self.token
         )
         self.assertTrue(created)
         self.assertEqual(obj.id, 1000000000099)
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
     def test_does_not_creates_empty_location_on_access_errors_if_requested(
         self, mock_fetch_esi_status, mock_esi
     ):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client.Universe.get_universe_structures_structure_id.side_effect = (
             RuntimeError
         )
         with self.assertRaises(RuntimeError):
             Location.objects.update_or_create_esi(id=1000000000099, token=self.token)
 
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
     def test_records_esi_error_on_access_error(self, mock_fetch_esi_status, mock_esi):
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client.Universe.get_universe_structures_structure_id.side_effect = (
             HTTPForbidden(
                 response=BravadoResponseStub(
                     403,
                     "Test exception",
@@ -776,15 +799,35 @@
         )
 
         obj, created = Location.objects.update_or_create_esi(
             id=1000000000099, token=self.token
         )
         self.assertTrue(created)
 
-    # Stations
+
+@patch(MANAGERS_PATH + ".esi")
+class TestLocationManagerOther(NoSocketsTestCase):
+    @classmethod
+    def setUpClass(cls) -> None:
+        super().setUpClass()
+        load_eveuniverse()
+        load_entities()
+        cls.jita = EveSolarSystem.objects.get(id=30000142)
+        cls.amamake = EveSolarSystem.objects.get(id=30002537)
+        cls.astrahus = EveType.objects.get(id=35832)
+        cls.athanor = EveType.objects.get(id=35835)
+        cls.jita_trade_hub = EveType.objects.get(id=52678)
+        cls.corporation_2001 = EveEntity.objects.get(id=2001)
+        cls.corporation_2002 = EveEntity.objects.get(id=2002)
+        cls.character = create_memberaudit_character(1001)
+        cls.token = (
+            cls.character.eve_character.character_ownership.user.token_set.first()
+        )
+
+    # stations
 
     def test_can_create_station(self, mock_esi):
         mock_esi.client = esi_client_stub
 
         obj, created = Location.objects.update_or_create_esi(
             id=60003760, token=self.token
         )
@@ -850,15 +893,15 @@
         self.assertEqual(obj.id, 2004)
         self.assertEqual(obj.name, "ASSET SAFETY")
         self.assertIsNone(obj.eve_solar_system)
         self.assertIsNone(obj.owner)
         self.assertEqual(obj.eve_type, EveType.objects.get(id=60))
 
 
-class TestLocationManagerAsync(TestCase):
+class TestLocationManagerAsync(NoSocketsTestCaseFixtures):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         cls.jita = EveSolarSystem.objects.get(id=30000142)
         cls.amamake = EveSolarSystem.objects.get(id=30002537)
@@ -875,15 +918,15 @@
     def setUp(self) -> None:
         cache.clear()
 
     @override_settings(
         CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True
     )
     @patch(MANAGERS_PATH + ".esi")
-    @patch(MANAGERS_PATH + ".fetch_esi_status")
+    @patch(MANAGERS_PATH + ".fetch_esi_status", spec=True)
     def test_can_create_structure_async(self, mock_fetch_esi_status, mock_esi):
         # given
         mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
         mock_esi.client = esi_client_stub
         # when
         obj, created = Location.objects.update_or_create_esi_async(
             id=1000000000001, token=self.token
@@ -897,15 +940,15 @@
         self.assertEqual(obj.name, "Amamake - Test Structure Alpha")
         self.assertEqual(obj.eve_solar_system, self.amamake)
         self.assertEqual(obj.eve_type, self.astrahus)
         self.assertEqual(obj.owner, self.corporation_2001)
         self.assertTrue(mock_fetch_esi_status.called)  # proofs task was called
 
     @patch(MANAGERS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
-    @patch(TASKS_PATH + ".update_structure_esi")
+    @patch(TASKS_PATH + ".update_structure_esi", spec=True)
     def test_should_create_location_and_ignore_already_queued(
         self, mock_task_update_structure_esi
     ):
         # given
         mock_task_update_structure_esi.apply_async.side_effect = AlreadyQueued(10)
         # when
         obj, created = Location.objects.update_or_create_esi_async(
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_1.py` & `aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,26 @@
 
 class TestCharacter(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
 
+    def test_user_should_produce_str(self):
+        # given
+        character_1001 = create_memberaudit_character(1001)
+        # when/then
+        self.assertTrue(str(character_1001))
+
+    def test_user_should_produce_repr(self):
+        # given
+        character_1001 = create_memberaudit_character(1001)
+        # when/then
+        self.assertTrue(repr(character_1001))
+
     def test_user_should_return_user_when_not_orphan(self):
         # given
         character_1001 = create_memberaudit_character(1001)
         user = character_1001.eve_character.character_ownership.user
         # when/then
         self.assertEqual(character_1001.user, user)
 
@@ -447,14 +459,251 @@
         # when
         result = str(self.character_1001.ship)
         # then
         self.assertIn("Bruce Wayne", result)
         self.assertIn("Merlin", result)
 
 
+class TestCharacterUpdateSkillSets(NoSocketsTestCase):
+    @classmethod
+    def setUpClass(cls) -> None:
+        super().setUpClass()
+        load_eveuniverse()
+        load_entities()
+        load_locations()
+        cls.character = create_memberaudit_character(1001)
+        cls.skill_type_1 = EveType.objects.get(id=24311)
+        cls.skill_type_2 = EveType.objects.get(id=24312)
+
+    def test_has_all_skills(self):
+        CharacterSkill.objects.create(
+            character=self.character,
+            eve_type=self.skill_type_1,
+            active_skill_level=5,
+            skillpoints_in_skill=10,
+            trained_skill_level=5,
+        )
+        CharacterSkill.objects.create(
+            character=self.character,
+            eve_type=self.skill_type_2,
+            active_skill_level=5,
+            skillpoints_in_skill=10,
+            trained_skill_level=5,
+        )
+        skill_set = SkillSet.objects.create(name="Ship 1")
+        SkillSetSkill.objects.create(
+            skill_set=skill_set, eve_type=self.skill_type_1, required_level=5
+        )
+        SkillSetSkill.objects.create(
+            skill_set=skill_set, eve_type=self.skill_type_2, required_level=3
+        )
+        skill_set_group = SkillSetGroup.objects.create(name="Dummy")
+        skill_set_group.skill_sets.add(skill_set)
+
+        self.character.update_skill_sets()
+
+        self.assertEqual(self.character.skill_set_checks.count(), 1)
+        first = self.character.skill_set_checks.first()
+        self.assertEqual(first.skill_set.pk, skill_set.pk)
+        self.assertEqual(first.failed_required_skills.count(), 0)
+
+    def test_one_skill_below(self):
+        CharacterSkill.objects.create(
+            character=self.character,
+            eve_type=self.skill_type_1,
+            active_skill_level=5,
+            skillpoints_in_skill=10,
+            trained_skill_level=5,
+        )
+        CharacterSkill.objects.create(
+            character=self.character,
+            eve_type=self.skill_type_2,
+            active_skill_level=2,
+            skillpoints_in_skill=10,
+            trained_skill_level=5,
+        )
+        skill_set = SkillSet.objects.create(name="Ship 1")
+        SkillSetSkill.objects.create(
+            skill_set=skill_set, eve_type=self.skill_type_1, required_level=5
+        )
+        skill_2 = SkillSetSkill.objects.create(
+            skill_set=skill_set, eve_type=self.skill_type_2, required_level=3
+        )
+        skill_set_group = SkillSetGroup.objects.create(name="Dummy")
+        skill_set_group.skill_sets.add(skill_set)
+
+        self.character.update_skill_sets()
+
+        self.assertEqual(self.character.skill_set_checks.count(), 1)
+        first = self.character.skill_set_checks.first()
+        self.assertEqual(first.skill_set.pk, skill_set.pk)
+        self.assertEqual(
+            {obj.pk for obj in first.failed_required_skills.all()}, {skill_2.pk}
+        )
+
+    def test_misses_one_skill(self):
+        CharacterSkill.objects.create(
+            character=self.character,
+            eve_type=self.skill_type_1,
+            active_skill_level=5,
+            skillpoints_in_skill=10,
+            trained_skill_level=5,
+        )
+        skill_set = SkillSet.objects.create(name="Ship 1")
+        SkillSetSkill.objects.create(
+            skill_set=skill_set, eve_type=self.skill_type_1, required_level=5
+        )
+        skill_2 = SkillSetSkill.objects.create(
+            skill_set=skill_set, eve_type=self.skill_type_2, required_level=3
+        )
+        skill_set_group = SkillSetGroup.objects.create(name="Dummy")
+        skill_set_group.skill_sets.add(skill_set)
+
+        self.character.update_skill_sets()
+
+        self.assertEqual(self.character.skill_set_checks.count(), 1)
+        first = self.character.skill_set_checks.first()
+        self.assertEqual(first.skill_set.pk, skill_set.pk)
+        self.assertEqual(
+            {obj.pk for obj in first.failed_required_skills.all()}, {skill_2.pk}
+        )
+
+    def test_passed_required_and_misses_recommendend_skill(self):
+        CharacterSkill.objects.create(
+            character=self.character,
+            eve_type=self.skill_type_1,
+            active_skill_level=4,
+            skillpoints_in_skill=10,
+            trained_skill_level=4,
+        )
+        skill_set = SkillSet.objects.create(name="Ship 1")
+        skill_1 = SkillSetSkill.objects.create(
+            skill_set=skill_set,
+            eve_type=self.skill_type_1,
+            required_level=3,
+            recommended_level=5,
+        )
+        self.character.update_skill_sets()
+
+        self.assertEqual(self.character.skill_set_checks.count(), 1)
+        first = self.character.skill_set_checks.first()
+        self.assertEqual(first.skill_set.pk, skill_set.pk)
+        self.assertEqual({obj.pk for obj in first.failed_required_skills.all()}, set())
+        self.assertEqual(
+            {obj.pk for obj in first.failed_recommended_skills.all()}, {skill_1.pk}
+        )
+
+    def test_misses_recommendend_skill_only(self):
+        CharacterSkill.objects.create(
+            character=self.character,
+            eve_type=self.skill_type_1,
+            active_skill_level=4,
+            skillpoints_in_skill=10,
+            trained_skill_level=4,
+        )
+        skill_set = SkillSet.objects.create(name="Ship 1")
+        skill_1 = SkillSetSkill.objects.create(
+            skill_set=skill_set,
+            eve_type=self.skill_type_1,
+            recommended_level=5,
+        )
+        self.character.update_skill_sets()
+
+        self.assertEqual(self.character.skill_set_checks.count(), 1)
+        first = self.character.skill_set_checks.first()
+        self.assertEqual(first.skill_set.pk, skill_set.pk)
+        self.assertEqual({obj.pk for obj in first.failed_required_skills.all()}, set())
+        self.assertEqual(
+            {obj.pk for obj in first.failed_recommended_skills.all()}, {skill_1.pk}
+        )
+
+    def test_misses_all_skills(self):
+        skill_set = SkillSet.objects.create(name="Ship 1")
+        skill_1 = SkillSetSkill.objects.create(
+            skill_set=skill_set, eve_type=self.skill_type_1, required_level=5
+        )
+        skill_2 = SkillSetSkill.objects.create(
+            skill_set=skill_set, eve_type=self.skill_type_2, required_level=3
+        )
+        skill_set_group = SkillSetGroup.objects.create(name="Dummy")
+        skill_set_group.skill_sets.add(skill_set)
+
+        self.character.update_skill_sets()
+
+        self.assertEqual(self.character.skill_set_checks.count(), 1)
+        first = self.character.skill_set_checks.first()
+        self.assertEqual(first.skill_set.pk, skill_set.pk)
+        self.assertEqual(
+            {obj.pk for obj in first.failed_required_skills.all()},
+            {skill_1.pk, skill_2.pk},
+        )
+
+    def test_does_not_require_doctrine_definition(self):
+        skill_set = SkillSet.objects.create(name="Ship 1")
+        skill_1 = SkillSetSkill.objects.create(
+            skill_set=skill_set, eve_type=self.skill_type_1, required_level=5
+        )
+        skill_2 = SkillSetSkill.objects.create(
+            skill_set=skill_set, eve_type=self.skill_type_2, required_level=3
+        )
+
+        self.character.update_skill_sets()
+
+        self.assertEqual(self.character.skill_set_checks.count(), 1)
+        first = self.character.skill_set_checks.first()
+        self.assertEqual(first.skill_set.pk, skill_set.pk)
+        self.assertEqual(
+            {obj.pk for obj in first.failed_required_skills.all()},
+            {skill_1.pk, skill_2.pk},
+        )
+
+
+class TestCharacterWalletJournalEntry(NoSocketsTestCase):
+    def test_match_context_type_id(self):
+        self.assertEqual(
+            CharacterWalletJournalEntry.match_context_type_id("character_id"),
+            CharacterWalletJournalEntry.CONTEXT_ID_TYPE_CHARACTER_ID,
+        )
+        self.assertEqual(
+            CharacterWalletJournalEntry.match_context_type_id("contract_id"),
+            CharacterWalletJournalEntry.CONTEXT_ID_TYPE_CONTRACT_ID,
+        )
+        self.assertEqual(
+            CharacterWalletJournalEntry.match_context_type_id(None),
+            CharacterWalletJournalEntry.CONTEXT_ID_TYPE_UNDEFINED,
+        )
+
+
+class TestCharacterUpdateStatusOk(NoSocketsTestCase):
+    @classmethod
+    def setUpClass(cls) -> None:
+        super().setUpClass()
+        load_entities()
+        cls.character = create_memberaudit_character(1001)
+
+    def test_should_return_none_when_not_all_sections_exist(self):
+        # when/then
+        self.assertIsNone(self.character.is_update_status_ok())
+
+    def test_should_return_false_when_a_section_has_errors(self):
+        # given
+        create_character_update_status(character=self.character, is_success=False)
+        # when/then
+        self.assertFalse(self.character.is_update_status_ok())
+
+    def test_should_return_true_when_all_sections_exist_and_have_no_error(self):
+        # given
+        for section in Character.UpdateSection:
+            create_character_update_status(
+                character=self.character, is_success=True, section=section.value
+            )
+        # when/then
+        self.assertTrue(self.character.is_update_status_ok())
+
+
 class TestCharacterUpdateSection(NoSocketsTestCase):
     def test_method_name(self):
         result = Character.UpdateSection.method_name(
             Character.UpdateSection.CORPORATION_HISTORY
         )
         self.assertEqual(result, "update_corporation_history")
 
@@ -723,217 +972,7 @@
                 character=self.character, section=self.section, is_success=True
             )
         self.assertTrue(self.character.is_update_section_stale(self.section))
 
     def test_does_not_exist(self):
         """When section does not exist, then return True"""
         self.assertTrue(self.character.is_update_section_stale(self.section))
-
-
-class TestCharacterUpdateSkillSets(NoSocketsTestCase):
-    @classmethod
-    def setUpClass(cls) -> None:
-        super().setUpClass()
-        load_eveuniverse()
-        load_entities()
-        load_locations()
-        cls.character = create_memberaudit_character(1001)
-        cls.skill_type_1 = EveType.objects.get(id=24311)
-        cls.skill_type_2 = EveType.objects.get(id=24312)
-
-    def test_has_all_skills(self):
-        CharacterSkill.objects.create(
-            character=self.character,
-            eve_type=self.skill_type_1,
-            active_skill_level=5,
-            skillpoints_in_skill=10,
-            trained_skill_level=5,
-        )
-        CharacterSkill.objects.create(
-            character=self.character,
-            eve_type=self.skill_type_2,
-            active_skill_level=5,
-            skillpoints_in_skill=10,
-            trained_skill_level=5,
-        )
-        skill_set = SkillSet.objects.create(name="Ship 1")
-        SkillSetSkill.objects.create(
-            skill_set=skill_set, eve_type=self.skill_type_1, required_level=5
-        )
-        SkillSetSkill.objects.create(
-            skill_set=skill_set, eve_type=self.skill_type_2, required_level=3
-        )
-        skill_set_group = SkillSetGroup.objects.create(name="Dummy")
-        skill_set_group.skill_sets.add(skill_set)
-
-        self.character.update_skill_sets()
-
-        self.assertEqual(self.character.skill_set_checks.count(), 1)
-        first = self.character.skill_set_checks.first()
-        self.assertEqual(first.skill_set.pk, skill_set.pk)
-        self.assertEqual(first.failed_required_skills.count(), 0)
-
-    def test_one_skill_below(self):
-        CharacterSkill.objects.create(
-            character=self.character,
-            eve_type=self.skill_type_1,
-            active_skill_level=5,
-            skillpoints_in_skill=10,
-            trained_skill_level=5,
-        )
-        CharacterSkill.objects.create(
-            character=self.character,
-            eve_type=self.skill_type_2,
-            active_skill_level=2,
-            skillpoints_in_skill=10,
-            trained_skill_level=5,
-        )
-        skill_set = SkillSet.objects.create(name="Ship 1")
-        SkillSetSkill.objects.create(
-            skill_set=skill_set, eve_type=self.skill_type_1, required_level=5
-        )
-        skill_2 = SkillSetSkill.objects.create(
-            skill_set=skill_set, eve_type=self.skill_type_2, required_level=3
-        )
-        skill_set_group = SkillSetGroup.objects.create(name="Dummy")
-        skill_set_group.skill_sets.add(skill_set)
-
-        self.character.update_skill_sets()
-
-        self.assertEqual(self.character.skill_set_checks.count(), 1)
-        first = self.character.skill_set_checks.first()
-        self.assertEqual(first.skill_set.pk, skill_set.pk)
-        self.assertEqual(
-            {obj.pk for obj in first.failed_required_skills.all()}, {skill_2.pk}
-        )
-
-    def test_misses_one_skill(self):
-        CharacterSkill.objects.create(
-            character=self.character,
-            eve_type=self.skill_type_1,
-            active_skill_level=5,
-            skillpoints_in_skill=10,
-            trained_skill_level=5,
-        )
-        skill_set = SkillSet.objects.create(name="Ship 1")
-        SkillSetSkill.objects.create(
-            skill_set=skill_set, eve_type=self.skill_type_1, required_level=5
-        )
-        skill_2 = SkillSetSkill.objects.create(
-            skill_set=skill_set, eve_type=self.skill_type_2, required_level=3
-        )
-        skill_set_group = SkillSetGroup.objects.create(name="Dummy")
-        skill_set_group.skill_sets.add(skill_set)
-
-        self.character.update_skill_sets()
-
-        self.assertEqual(self.character.skill_set_checks.count(), 1)
-        first = self.character.skill_set_checks.first()
-        self.assertEqual(first.skill_set.pk, skill_set.pk)
-        self.assertEqual(
-            {obj.pk for obj in first.failed_required_skills.all()}, {skill_2.pk}
-        )
-
-    def test_passed_required_and_misses_recommendend_skill(self):
-        CharacterSkill.objects.create(
-            character=self.character,
-            eve_type=self.skill_type_1,
-            active_skill_level=4,
-            skillpoints_in_skill=10,
-            trained_skill_level=4,
-        )
-        skill_set = SkillSet.objects.create(name="Ship 1")
-        skill_1 = SkillSetSkill.objects.create(
-            skill_set=skill_set,
-            eve_type=self.skill_type_1,
-            required_level=3,
-            recommended_level=5,
-        )
-        self.character.update_skill_sets()
-
-        self.assertEqual(self.character.skill_set_checks.count(), 1)
-        first = self.character.skill_set_checks.first()
-        self.assertEqual(first.skill_set.pk, skill_set.pk)
-        self.assertEqual({obj.pk for obj in first.failed_required_skills.all()}, set())
-        self.assertEqual(
-            {obj.pk for obj in first.failed_recommended_skills.all()}, {skill_1.pk}
-        )
-
-    def test_misses_recommendend_skill_only(self):
-        CharacterSkill.objects.create(
-            character=self.character,
-            eve_type=self.skill_type_1,
-            active_skill_level=4,
-            skillpoints_in_skill=10,
-            trained_skill_level=4,
-        )
-        skill_set = SkillSet.objects.create(name="Ship 1")
-        skill_1 = SkillSetSkill.objects.create(
-            skill_set=skill_set,
-            eve_type=self.skill_type_1,
-            recommended_level=5,
-        )
-        self.character.update_skill_sets()
-
-        self.assertEqual(self.character.skill_set_checks.count(), 1)
-        first = self.character.skill_set_checks.first()
-        self.assertEqual(first.skill_set.pk, skill_set.pk)
-        self.assertEqual({obj.pk for obj in first.failed_required_skills.all()}, set())
-        self.assertEqual(
-            {obj.pk for obj in first.failed_recommended_skills.all()}, {skill_1.pk}
-        )
-
-    def test_misses_all_skills(self):
-        skill_set = SkillSet.objects.create(name="Ship 1")
-        skill_1 = SkillSetSkill.objects.create(
-            skill_set=skill_set, eve_type=self.skill_type_1, required_level=5
-        )
-        skill_2 = SkillSetSkill.objects.create(
-            skill_set=skill_set, eve_type=self.skill_type_2, required_level=3
-        )
-        skill_set_group = SkillSetGroup.objects.create(name="Dummy")
-        skill_set_group.skill_sets.add(skill_set)
-
-        self.character.update_skill_sets()
-
-        self.assertEqual(self.character.skill_set_checks.count(), 1)
-        first = self.character.skill_set_checks.first()
-        self.assertEqual(first.skill_set.pk, skill_set.pk)
-        self.assertEqual(
-            {obj.pk for obj in first.failed_required_skills.all()},
-            {skill_1.pk, skill_2.pk},
-        )
-
-    def test_does_not_require_doctrine_definition(self):
-        skill_set = SkillSet.objects.create(name="Ship 1")
-        skill_1 = SkillSetSkill.objects.create(
-            skill_set=skill_set, eve_type=self.skill_type_1, required_level=5
-        )
-        skill_2 = SkillSetSkill.objects.create(
-            skill_set=skill_set, eve_type=self.skill_type_2, required_level=3
-        )
-
-        self.character.update_skill_sets()
-
-        self.assertEqual(self.character.skill_set_checks.count(), 1)
-        first = self.character.skill_set_checks.first()
-        self.assertEqual(first.skill_set.pk, skill_set.pk)
-        self.assertEqual(
-            {obj.pk for obj in first.failed_required_skills.all()},
-            {skill_1.pk, skill_2.pk},
-        )
-
-
-class TestCharacterWalletJournalEntry(NoSocketsTestCase):
-    def test_match_context_type_id(self):
-        self.assertEqual(
-            CharacterWalletJournalEntry.match_context_type_id("character_id"),
-            CharacterWalletJournalEntry.CONTEXT_ID_TYPE_CHARACTER_ID,
-        )
-        self.assertEqual(
-            CharacterWalletJournalEntry.match_context_type_id("contract_id"),
-            CharacterWalletJournalEntry.CONTEXT_ID_TYPE_CONTRACT_ID,
-        )
-        self.assertEqual(
-            CharacterWalletJournalEntry.match_context_type_id(None),
-            CharacterWalletJournalEntry.CONTEXT_ID_TYPE_UNDEFINED,
-        )
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_2.py` & `aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_3.py` & `aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_4.py` & `aa_memberaudit-2.7.0/memberaudit/tests/models/test_character_4.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/models/test_general.py` & `aa_memberaudit-2.7.0/memberaudit/tests/models/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/models/test_sections.py` & `aa_memberaudit-2.7.0/memberaudit/tests/models/test_sections.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from typing import NamedTuple
+
 from django.test import TestCase
+from eveuniverse.models import EveEntity
 
 from memberaudit.constants import EveFactionId
-from memberaudit.models import CharacterFwStats
+from memberaudit.models import CharacterContact, CharacterFwStats
 
-from ..testdata.factories import create_fw_stats
+from ..testdata.factories import create_character_contact, create_fw_stats
 from ..utils import create_memberaudit_character, load_entities, load_eveuniverse
 
 
 class TestCharacterFwStatsRankNameGeneric(TestCase):
     def test_should_return_rank_name_when_found(self):
         # when
         result = CharacterFwStats.rank_name_generic(EveFactionId.CALDARI_STATE, 4)
@@ -40,7 +43,41 @@
         self.assertEqual(obj.current_rank_name(), "Major")
 
     def test_should_return_rank_name_when_not_found(self):
         # given
         obj = create_fw_stats(character=self.character, faction=None)
         # when/then
         self.assertEqual(obj.current_rank_name(), "")
+
+
+class TestCharacterContactStandingLevel(TestCase):
+    @classmethod
+    def setUpClass(cls) -> None:
+        super().setUpClass()
+        load_eveuniverse()
+        load_entities()
+
+    class MyTestCase(NamedTuple):
+        standing: float
+        expected_result: str
+
+    def test_should_determine_correct_standing(self):
+        # given
+        character = create_memberaudit_character(1001)
+        contact_character = EveEntity.objects.get(id=1101)
+
+        test_cases = [
+            self.MyTestCase(9.9, CharacterContact.STANDING_EXCELLENT),
+            self.MyTestCase(4.9, CharacterContact.STANDING_GOOD),
+            self.MyTestCase(0.0, CharacterContact.STANDING_NEUTRAL),
+            self.MyTestCase(-4.9, CharacterContact.STANDING_BAD),
+            self.MyTestCase(-9.9, CharacterContact.STANDING_TERRIBLE),
+        ]
+        for test_case in test_cases:
+            with self.subTest(standing=test_case.standing):
+                contact = create_character_contact(
+                    character=character,
+                    eve_entity=contact_character,
+                    standing=test_case.standing,
+                )
+                self.assertEqual(contact.standing_level, test_case.expected_result)
+                contact.delete()
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/models/utils.py` & `aa_memberaudit-2.7.0/memberaudit/tests/models/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/test_admin.py` & `aa_memberaudit-2.7.0/memberaudit/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/test_auth_hooks.py` & `aa_memberaudit-2.7.0/memberaudit/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/test_checks.py` & `aa_memberaudit-2.7.0/memberaudit/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/test_commands.py` & `aa_memberaudit-2.7.0/memberaudit/tests/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import tempfile
 from io import StringIO
 from pathlib import Path
+from unittest import skip
 
 from django.core.management import call_command
 
 from app_utils.testing import NoSocketsTestCase
 
 from ..models import Character
 from .testdata.factories import (
@@ -19,14 +20,15 @@
     create_user_from_evecharacter_with_access,
 )
 
 PACKAGE_PATH = "memberaudit.management.commands"
 DATA_EXPORTERS_PATH = "memberaudit.core.data_exporters"
 
 
+@skip("Maria DB breaks")
 class TestResetCharacters(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_entities()
         Character.objects.all().delete()
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/test_decorators.py` & `aa_memberaudit-2.7.0/memberaudit/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/test_factories.py` & `aa_memberaudit-2.7.0/memberaudit/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/test_forms.py` & `aa_memberaudit-2.7.0/memberaudit/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/test_helpers.py` & `aa_memberaudit-2.7.0/memberaudit/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/test_integration.py` & `aa_memberaudit-2.7.0/memberaudit/tests/test_integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,31 +25,35 @@
 from .testdata.esi_client_stub import esi_client_stub
 from .testdata.load_entities import load_entities
 from .testdata.load_eveuniverse import load_eveuniverse
 from .testdata.load_locations import load_locations
 from .utils import (
     add_auth_character_to_user,
     add_memberaudit_character_to_user,
+    clear_celery_once_locks,
     create_memberaudit_character,
     create_user_from_evecharacter_with_access,
 )
 
 MANAGERS_PATH = "memberaudit.managers"
 MODELS_PATH = "memberaudit.models"
 TASKS_PATH = "memberaudit.tasks"
 
 
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 class TestUILauncher(WebTest):
+    fixtures = ["disable_analytics.json"]
+
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         load_locations()
+        clear_celery_once_locks()
 
     def setUp(self) -> None:
         self.user, _ = create_user_from_evecharacter_with_access(1002)
 
     def test_open_character_viewer(self):
         """
         given user has character registered
@@ -112,19 +116,18 @@
         self.assertEqual(launcher.status_code, 200)
 
         # check update went through
         character_1001 = character_ownership_1001.character.memberaudit_character
         self.assertTrue(character_1001.is_update_status_ok())
 
         # check added character is now visible in launcher
+        a_tags = launcher.html.find_all("a", href=True)
+        viewer_url = reverse("memberaudit:character_viewer", args=[character_1001.pk])
         character_1001_links = [
-            x["href"]
-            for x in launcher.html.find_all("a", href=True)
-            if x["href"]
-            == reverse("memberaudit:character_viewer", args=[character_1001.pk])
+            a_tag["href"] for a_tag in a_tags if a_tag["href"] == viewer_url
         ]
         self.assertGreater(len(character_1001_links), 0)
 
     def test_share_character_1(self):
         """
         when user has share permission
         then he can share his characters
@@ -137,19 +140,18 @@
 
         # login & open launcher page
         self.app.set_user(self.user)
         launcher = self.app.get(reverse("memberaudit:launcher"))
         self.assertEqual(launcher.status_code, 200)
 
         # check for share button
+        share_url = reverse("memberaudit:share_character", args=[character_1001.pk])
+        a_tags = launcher.html.find_all("a", href=True)
         character_1001_links = [
-            x["href"]
-            for x in launcher.html.find_all("a", href=True)
-            if x["href"]
-            == reverse("memberaudit:share_character", args=[character_1001.pk])
+            a_tag["href"] for a_tag in a_tags if a_tag["href"] == share_url
         ]
         self.assertGreater(len(character_1001_links), 0)
 
     def test_share_character_2(self):
         """
         when user does not have share permission
         then he can not share his characters
@@ -159,24 +161,25 @@
 
         # login & open launcher page
         self.app.set_user(self.user)
         launcher = self.app.get(reverse("memberaudit:launcher"))
         self.assertEqual(launcher.status_code, 200)
 
         # check for share button
+        share_url = reverse("memberaudit:share_character", args=[character_1001.pk])
+        a_tags = launcher.html.find_all("a", href=True)
         character_1001_links = [
-            x["href"]
-            for x in launcher.html.find_all("a", href=True)
-            if x["href"]
-            == reverse("memberaudit:share_character", args=[character_1001.pk])
+            a_tag["href"] for a_tag in a_tags if a_tag["href"] == share_url
         ]
         self.assertEqual(len(character_1001_links), 0)
 
 
 class TestUICharacterViewer(WebTest):
+    fixtures = ["disable_analytics.json"]
+
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         load_locations()
         cls.character = create_memberaudit_character(1001)
@@ -329,20 +332,23 @@
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(TASKS_PATH + ".MEMBERAUDIT_LOG_UPDATE_STATS", False)
 @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
 @patch(MODELS_PATH + ".character.esi")
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 class TestTasksE2E(TestCase):
+    fixtures = ["disable_analytics.json"]
+
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         load_locations()
+        clear_celery_once_locks()
 
     def test_should_update_all_characters(self, mock_esi):
         # given
         mock_esi.client = esi_client_stub
         character_1001 = create_memberaudit_character(1001)
         # when
         tasks.update_all_characters()
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/test_signals.py` & `aa_memberaudit-2.7.0/memberaudit/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/test_tasks.py` & `aa_memberaudit-2.7.0/memberaudit/tests/test_tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,92 +1,71 @@
 import datetime as dt
 from unittest import skip
 from unittest.mock import MagicMock, patch
 
-from bravado.exception import HTTPInternalServerError
 from celery.exceptions import Retry as CeleryRetry
 
-from django.test import TestCase, override_settings
+from django.test import override_settings
 from django.utils.timezone import now
 from esi.models import Token
 from eveuniverse.models import EveSolarSystem, EveType
 from eveuniverse.tests.testdata.factories import create_eve_entity
 
 from allianceauth.eveonline.models import EveCharacter
-from allianceauth.utils.cache import get_redis_client
 from app_utils.esi import (
     EsiDailyDowntime,
     EsiErrorLimitExceeded,
     EsiOffline,
     EsiStatus,
     fetch_esi_status,
 )
-from app_utils.esi_testing import BravadoResponseStub
+from app_utils.esi_testing import build_http_error
 from app_utils.testing import (
+    NoSocketsTestCase,
     create_authgroup,
     create_user_from_evecharacter,
     generate_invalid_pk,
 )
 
+from memberaudit import tasks
 from memberaudit.models import (
     Character,
     CharacterAsset,
     CharacterUpdateStatus,
     Location,
 )
-from memberaudit.tasks import (
-    _export_data_for_topic,
-    delete_character,
-    export_data,
-    run_regular_updates,
-    update_all_characters,
-    update_character,
-    update_character_assets,
-    update_character_contacts,
-    update_character_contracts,
-    update_character_mails,
-    update_character_wallet_journal,
-    update_characters_skill_checks,
-    update_compliance_groups_for_user,
-    update_mail_entity_esi,
-    update_market_prices,
-    update_structure_esi,
-    update_unresolved_eve_entities,
-)
 
 from .testdata.esi_client_stub import esi_client_error_stub, esi_client_stub
 from .testdata.factories import create_character, create_compliance_group_designation
 from .testdata.load_entities import load_entities
 from .testdata.load_eveuniverse import load_eveuniverse
 from .testdata.load_locations import load_locations
-from .utils import create_memberaudit_character
+from .utils import clear_celery_once_locks, create_memberaudit_character
 
 MODELS_PATH = "memberaudit.models"
 MANAGERS_PATH = "memberaudit.managers"
 TASKS_PATH = "memberaudit.tasks"
 
 
-def clear_celery_once_locks():
-    r = get_redis_client()
-    if keys := r.keys(":?:qo_memberaudit.*"):
-        r.delete(*keys)
+class TestCaseTasks(NoSocketsTestCase):
+    fixtures = ["disable_analytics.json"]
 
 
-@patch(TASKS_PATH + ".update_compliance_groups_for_all")
-@patch(TASKS_PATH + ".update_all_characters")
-@patch(TASKS_PATH + ".update_market_prices")
-class TestRegularUpdates(TestCase):
+@patch(TASKS_PATH + ".update_compliance_groups_for_all", spec=True)
+@patch(TASKS_PATH + ".update_all_characters", spec=True)
+@patch(TASKS_PATH + ".update_market_prices", spec=True)
+class TestRegularUpdates(TestCaseTasks):
     def test_should_run_update_for_all_except_compliance_groups(
         self,
         mock_update_market_prices,
         mock_update_all_characters,
         mock_update_compliance_groups_for_all,
     ):
         # when
-        run_regular_updates()
+        tasks.run_regular_updates()
         # then
         self.assertTrue(mock_update_market_prices.apply_async.called)
         self.assertTrue(mock_update_all_characters.apply_async.called)
         self.assertFalse(mock_update_compliance_groups_for_all.apply_async.called)
 
     def test_should_run_update_for_all_incl_compliance_groups(
         self,
@@ -94,33 +73,33 @@
         mock_update_all_characters,
         mock_update_compliance_groups_for_all,
     ):
         # given
         group = create_authgroup(internal=False)
         create_compliance_group_designation(group)
         # when
-        run_regular_updates()
+        tasks.run_regular_updates()
         # then
         self.assertTrue(mock_update_market_prices.apply_async.called)
         self.assertTrue(mock_update_all_characters.apply_async.called)
         self.assertTrue(mock_update_compliance_groups_for_all.apply_async.called)
 
 
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
-class TestOtherTasks(TestCase):
-    @patch(TASKS_PATH + ".EveMarketPrice.objects.update_from_esi")
+class TestOtherTasks(TestCaseTasks):
+    @patch(TASKS_PATH + ".EveMarketPrice.objects.update_from_esi", spec=True)
     def test_update_market_prices(self, mock_update_from_esi):
-        update_market_prices()
+        tasks.update_market_prices()
         self.assertTrue(mock_update_from_esi.called)
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True)  # need to ignore exceptions
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MODELS_PATH + ".character.esi")
-class TestUpdateCharacterAssets(TestCase):
+class TestUpdateCharacterAssets(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         load_locations()
         cls.character_1001 = create_memberaudit_character(1001)
@@ -133,15 +112,15 @@
         cls.amamake = EveSolarSystem.objects.get(id=30002537)
         cls.structure_1 = Location.objects.get(id=1000000000001)
 
     def test_update_assets_1(self, mock_esi):
         """can create assets from scratch"""
         mock_esi.client = esi_client_stub
 
-        update_character_assets(self.character_1001.pk)
+        tasks.update_character_assets(self.character_1001.pk)
         self.assertSetEqual(
             set(self.character_1001.assets.values_list("item_id", flat=True)),
             {
                 1100000000001,
                 1100000000002,
                 1100000000003,
                 1100000000004,
@@ -203,15 +182,15 @@
             location=self.jita_44,
             eve_type=EveType.objects.get(id=20185),
             is_singleton=False,
             name="Trucker",
             quantity=1,
         )
 
-        update_character_assets(self.character_1001.pk)
+        tasks.update_character_assets(self.character_1001.pk)
         self.assertSetEqual(
             set(self.character_1001.assets.values_list("item_id", flat=True)),
             {
                 1100000000001,
                 1100000000002,
                 1100000000003,
                 1100000000004,
@@ -231,15 +210,15 @@
             location=self.jita_44,
             eve_type=EveType.objects.get(id=20185),
             is_singleton=True,
             name="Parent Item 1",
             quantity=10,
         )
 
-        update_character_assets(self.character_1001.pk)
+        tasks.update_character_assets(self.character_1001.pk)
         self.assertSetEqual(
             set(self.character_1001.assets.values_list("item_id", flat=True)),
             {
                 1100000000001,
                 1100000000002,
                 1100000000003,
                 1100000000004,
@@ -275,15 +254,15 @@
             parent=parent_asset,
             eve_type=EveType.objects.get(id=19540),
             is_singleton=True,
             is_blueprint_copy=False,
             quantity=1,
         )
 
-        update_character_assets(self.character_1001.pk)
+        tasks.update_character_assets(self.character_1001.pk)
         self.assertSetEqual(
             set(self.character_1001.assets.values_list("item_id", flat=True)),
             {
                 1100000000001,
                 1100000000002,
                 1100000000003,
                 1100000000004,
@@ -294,151 +273,152 @@
             },
         )
 
     def test_update_assets_5(self, mock_esi):
         """when update succeeded then report update success"""
         mock_esi.client = esi_client_stub
 
-        update_character_assets(self.character_1001.pk)
+        tasks.update_character_assets(self.character_1001.pk)
 
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.ASSETS
         )
         self.assertTrue(status.is_success)
         self.assertFalse(status.last_error_message)
 
     def test_update_assets_6(self, mock_esi):
         """when update failed then report the error"""
+        # given
+        exception = build_http_error(500, "Test exception")
         mock_esi.client.Assets.get_characters_character_id_assets.side_effect = (
-            HTTPInternalServerError(response=BravadoResponseStub(500, "Test exception"))
+            exception
         )
-
+        # when
         with self.assertRaises(OSError):
-            update_character_assets(self.character_1001.pk)
-
+            tasks.update_character_assets(self.character_1001.pk)
+        # then
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.ASSETS
         )
         self.assertFalse(status.is_success)
         self.assertEqual(
             status.last_error_message, "HTTPInternalServerError: 500 Test exception"
         )
 
     def test_update_assets_7(self, mock_esi):
         """when preload objects failed then report the error"""
         mock_esi.client = esi_client_stub
 
-        with patch(MODELS_PATH + ".character.Location") as m:
-            m.objects.get_or_create_esi_async.side_effect = HTTPInternalServerError(
-                response=BravadoResponseStub(500, "Test exception")
-            )
+        with patch(MODELS_PATH + ".character.Location", spec=True) as m:
+            exception = build_http_error(500, "Test exception")
+            m.objects.get_or_create_esi_async.side_effect = exception
             with self.assertRaises(OSError):
-                update_character_assets(self.character_1001.pk)
+                tasks.update_character_assets(self.character_1001.pk)
 
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.ASSETS
         )
         self.assertFalse(status.is_success)
         self.assertEqual(
             status.last_error_message, "HTTPInternalServerError: 500 Test exception"
         )
 
     def test_update_assets_8(self, mock_esi):
         """when building the asset tree failed then report the error"""
         mock_esi.client = esi_client_stub
 
         with patch(MODELS_PATH + ".character.logger") as m:
-            m.info.side_effect = HTTPInternalServerError(
-                response=BravadoResponseStub(500, "Test exception")
-            )
+            exception = build_http_error(500, "Test exception")
+            m.info.side_effect = exception
             with self.assertRaises(OSError):
-                update_character_assets(self.character_1001.pk)
+                tasks.update_character_assets(self.character_1001.pk)
 
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.ASSETS
         )
         self.assertFalse(status.is_success)
         self.assertEqual(
             status.last_error_message, "HTTPInternalServerError: 500 Test exception"
         )
 
     def test_update_assets_9(self, mock_esi):
         """when info from ESI has not change, then don't re-create asset tree"""
         mock_esi.client = esi_client_stub
 
         self.character_1001.reset_update_section(Character.UpdateSection.ASSETS)
-        update_character_assets(self.character_1001.pk)
+        tasks.update_character_assets(self.character_1001.pk)
         asset = self.character_1001.assets.get(item_id=1100000000001)
         asset.name = "New Name"
         asset.save()
-        update_character_assets(self.character_1001.pk)
+        tasks.update_character_assets(self.character_1001.pk)
 
         asset = self.character_1001.assets.get(item_id=1100000000001)
         self.assertEqual(asset.name, "New Name")
 
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.ASSETS
         )
         self.assertTrue(status.is_success)
 
     def test_update_assets_10(self, mock_esi):
         """when info from ESI has not change and update is forced, then re-create asset tree"""
         mock_esi.client = esi_client_stub
 
         self.character_1001.reset_update_section(Character.UpdateSection.ASSETS)
-        update_character_assets(self.character_1001.pk)
+        tasks.update_character_assets(self.character_1001.pk)
         asset = self.character_1001.assets.get(item_id=1100000000001)
         asset.name = "New Name"
         asset.save()
-        update_character_assets(self.character_1001.pk, force_update=True)
+        tasks.update_character_assets(self.character_1001.pk, force_update=True)
 
         asset = self.character_1001.assets.get(item_id=1100000000001)
         self.assertEqual(asset.name, "Parent Item 1")
 
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.ASSETS
         )
         self.assertTrue(status.is_success)
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MODELS_PATH + ".character.esi")
-class TestUpdateCharacterMails(TestCase):
+class TestUpdateCharacterMails(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         cls.character_1001 = create_memberaudit_character(1001)
         cls.token = (
             cls.character_1001.eve_character.character_ownership.user.token_set.first()
         )
 
     def test_update_ok(self, mock_esi):
         """when update succeeded then report update success"""
         mock_esi.client = esi_client_stub
 
-        update_character_mails(self.character_1001.pk)
+        tasks.update_character_mails(self.character_1001.pk)
 
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.MAILS
         )
         self.assertTrue(status.is_success)
         self.assertFalse(status.last_error_message)
 
     def test_detect_error(self, mock_esi):
         """when update failed then report the error"""
+        exception = build_http_error(500, "Test exception")
         mock_esi.client.Mail.get_characters_character_id_mail_lists.side_effect = (
-            HTTPInternalServerError(response=BravadoResponseStub(500, "Test exception"))
+            exception
         )
 
         try:
-            update_character_mails(self.character_1001.pk)
+            tasks.update_character_mails(self.character_1001.pk)
         except Exception:
             status = self.character_1001.update_status_set.get(
                 section=Character.UpdateSection.MAILS
             )
             self.assertFalse(status.is_success)
             self.assertEqual(
                 status.last_error_message, "HTTPInternalServerError: 500 Test exception"
@@ -447,45 +427,46 @@
             self.assertTrue(False)  # Hack to ensure the test fails when it gets here
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MODELS_PATH + ".character.esi")
-class TestUpdateCharacterContacts(TestCase):
+class TestUpdateCharacterContacts(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         cls.character_1001 = create_memberaudit_character(1001)
         cls.token = (
             cls.character_1001.eve_character.character_ownership.user.token_set.first()
         )
 
     def test_update_ok(self, mock_esi):
         """when update succeeded then report update success"""
         mock_esi.client = esi_client_stub
 
-        update_character_contacts(self.character_1001.pk)
+        tasks.update_character_contacts(self.character_1001.pk)
 
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.CONTACTS
         )
         self.assertTrue(status.is_success)
         self.assertFalse(status.last_error_message)
 
     def test_detect_error(self, mock_esi):
         """when update failed then report the error"""
-        mock_esi.client.Contacts.get_characters_character_id_contacts_labels.side_effect = HTTPInternalServerError(
-            response=BravadoResponseStub(500, "Test exception")
+        exception = build_http_error(500, "Test exception")
+        mock_esi.client.Contacts.get_characters_character_id_contacts_labels.side_effect = (
+            exception
         )
 
         try:
-            update_character_contacts(self.character_1001.pk)
+            tasks.update_character_contacts(self.character_1001.pk)
         except Exception:
             status = self.character_1001.update_status_set.get(
                 section=Character.UpdateSection.CONTACTS
             )
             self.assertFalse(status.is_success)
             self.assertEqual(
                 status.last_error_message, "HTTPInternalServerError: 500 Test exception"
@@ -494,15 +475,15 @@
             self.assertTrue(False)  # Hack to ensure the test fails when it gets here
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MODELS_PATH + ".character.esi")
-class TestUpdateCharacterContracts(TestCase):
+class TestUpdateCharacterContracts(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         load_locations()
         cls.character_1001 = create_memberaudit_character(1001)
@@ -510,30 +491,31 @@
             cls.character_1001.eve_character.character_ownership.user.token_set.first()
         )
 
     def test_update_ok(self, mock_esi):
         """when update succeeded then report update success"""
         mock_esi.client = esi_client_stub
 
-        update_character_contracts(self.character_1001.pk)
+        tasks.update_character_contracts(self.character_1001.pk)
 
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.CONTRACTS
         )
         self.assertTrue(status.is_success)
         self.assertFalse(status.last_error_message)
 
     def test_detect_error(self, mock_esi):
         """when update failed then report the error"""
+        exception = build_http_error(500, "Test exception")
         mock_esi.client.Contracts.get_characters_character_id_contracts.side_effect = (
-            HTTPInternalServerError(response=BravadoResponseStub(500, "Test exception"))
+            exception
         )
 
         try:
-            update_character_contracts(self.character_1001.pk)
+            tasks.update_character_contracts(self.character_1001.pk)
         except Exception:
             status = self.character_1001.update_status_set.get(
                 section=Character.UpdateSection.CONTRACTS
             )
             self.assertFalse(status.is_success)
             self.assertEqual(
                 status.last_error_message, "HTTPInternalServerError: 500 Test exception"
@@ -542,45 +524,46 @@
             self.assertTrue(False)  # Hack to ensure the test fails when it gets here
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MODELS_PATH + ".character.esi")
-class TestUpdateCharacterWalletJournal(TestCase):
+class TestUpdateCharacterWalletJournal(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         cls.character_1001 = create_memberaudit_character(1001)
         cls.token = (
             cls.character_1001.eve_character.character_ownership.user.token_set.first()
         )
 
     def test_update_ok(self, mock_esi):
         """when update succeeded then report update success"""
         mock_esi.client = esi_client_stub
 
-        update_character_wallet_journal(self.character_1001.pk)
+        tasks.update_character_wallet_journal(self.character_1001.pk)
 
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.WALLET_JOURNAL
         )
         self.assertTrue(status.is_success)
         self.assertFalse(status.last_error_message)
 
     def test_detect_error(self, mock_esi):
         """when update failed then report the error"""
-        mock_esi.client.Wallet.get_characters_character_id_wallet_journal.side_effect = HTTPInternalServerError(
-            response=BravadoResponseStub(500, "Test exception")
+        exception = build_http_error(500, "Test exception")
+        mock_esi.client.Wallet.get_characters_character_id_wallet_journal.side_effect = (
+            exception
         )
 
         try:
-            update_character_wallet_journal(self.character_1001.pk)
+            tasks.update_character_wallet_journal(self.character_1001.pk)
         except Exception:
             status = self.character_1001.update_status_set.get(
                 section=Character.UpdateSection.WALLET_JOURNAL
             )
             self.assertFalse(status.is_success)
             self.assertEqual(
                 status.last_error_message, "HTTPInternalServerError: 500 Test exception"
@@ -590,15 +573,15 @@
 
 
 @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MODELS_PATH + ".character.esi")
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-class TestUpdateCharacter(TestCase):
+class TestUpdateCharacter(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         load_locations()
 
@@ -607,69 +590,69 @@
         clear_celery_once_locks()
 
     @skip  # temporary disabled because it does not work in tox
     def test_should_update_normally(self, mock_esi):
         """can update from scratch"""
         mock_esi.client = esi_client_stub
 
-        result = update_character(self.character_1001.pk)
+        result = tasks.update_character(self.character_1001.pk)
         self.assertTrue(result)
         self.assertTrue(self.character_1001.is_update_status_ok())
 
     def test_should_report_errors_during_updates(self, mock_esi):
         mock_esi.client = esi_client_error_stub
 
         with self.assertRaises(OSError):  # raised when trying to fetch attributes
-            update_character(self.character_1001.pk)
+            tasks.update_character(self.character_1001.pk)
 
         self.assertFalse(self.character_1001.is_update_status_ok())
 
         status = self.character_1001.update_status_set.get(
             character=self.character_1001,
             section=Character.UpdateSection.ATTRIBUTES,
         )
         self.assertFalse(status.is_success)
         self.assertEqual(
             status.last_error_message, "HTTPInternalServerError: 500 Test exception"
         )
         self.assertTrue(status.finished_at)
 
-    @patch(TASKS_PATH + ".Character.update_loyalty")
+    @patch(TASKS_PATH + ".Character.update_loyalty", spec=True)
     def test_should_update_stale_sections_only_1(self, update_loyalty, mock_esi):
         """normal section"""
         mock_esi.client = esi_client_stub
         CharacterUpdateStatus.objects.create(
             character=self.character_1001,
             section=Character.UpdateSection.LOYALTY,
             is_success=True,
             started_at=now() - dt.timedelta(seconds=30),
             finished_at=now(),
         )
 
-        update_character(self.character_1001.pk)
+        tasks.update_character(self.character_1001.pk)
 
         self.assertFalse(update_loyalty.called)
 
-    @patch(TASKS_PATH + ".update_character_mails")
+    @patch(TASKS_PATH + ".update_character_mails", spec=True)
     def test_should_update_stale_sections_only_2(
-        self, update_character_mails, mock_esi
+        self, mock_update_character_mails, mock_esi
     ):
         """special section"""
         mock_esi.client = esi_client_stub
         CharacterUpdateStatus.objects.create(
             character=self.character_1001,
             section=Character.UpdateSection.MAILS,
             is_success=True,
             started_at=now() - dt.timedelta(seconds=30),
             finished_at=now(),
         )
 
-        update_character(self.character_1001.pk)
+        tasks.update_character(self.character_1001.pk)
 
-        self.assertFalse(update_character_mails.apply_async.called)
+        self.assertFalse(mock_update_character_mails.apply_async.called)
 
     @patch(TASKS_PATH + ".Character.update_skills", spec=True)
     def test_should_update_stale_sections_only_3(self, mock_update_skills, mock_esi):
         """When generic section has recently been updated and force_update is called
         then update again
         """
         mock_esi.client = esi_client_stub
@@ -677,15 +660,15 @@
             character=self.character_1001,
             section=Character.UpdateSection.SKILLS,
             is_success=True,
             started_at=now() - dt.timedelta(seconds=30),
             finished_at=now(),
         )
 
-        update_character(self.character_1001.pk, force_update=True)
+        tasks.update_character(self.character_1001.pk, force_update=True)
 
         self.assertTrue(mock_update_skills.called)
 
     def test_no_update_required(self, mock_esi):
         """Do not update anything when not required"""
         mock_esi.client = esi_client_stub
         for section in Character.UpdateSection.values:
@@ -693,183 +676,197 @@
                 character=self.character_1001,
                 section=section,
                 is_success=True,
                 started_at=now() - dt.timedelta(seconds=30),
                 finished_at=now(),
             )
 
-        result = update_character(self.character_1001.pk)
+        result = tasks.update_character(self.character_1001.pk)
         self.assertFalse(result)
 
     def test_update_forced(self, mock_esi):
         """Can do forced update"""
         mock_esi.client = esi_client_stub
 
-        result = update_character(self.character_1001.pk, force_update=True)
+        result = tasks.update_character(self.character_1001.pk, force_update=True)
         self.assertTrue(result)
         self.assertTrue(self.character_1001.is_update_status_ok())
 
+    def test_skip_update_for_orphans(self, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        character = create_character(EveCharacter.objects.get(character_id=1121))
+        # when
+        result = tasks.update_character(character.pk)
+        # then
+        self.assertFalse(result)
+        self.assertIsNone(character.is_update_status_ok())
+
 
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
-@patch(TASKS_PATH + ".Location.objects.structure_update_or_create_esi")
-class TestUpdateStructureEsi(TestCase):
+@patch(TASKS_PATH + ".Location.objects.structure_update_or_create_esi", spec=True)
+class TestUpdateStructureEsi(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
         cls.character = create_memberaudit_character(1001)
         cls.token = (
             cls.character.eve_character.character_ownership.user.token_set.first()
         )
 
     def test_normal(self, mock_structure_update_or_create_esi):
         """When ESI status is ok, then create MailEntity"""
         mock_structure_update_or_create_esi.return_value = None
         try:
-            update_structure_esi(id=1000000000001, token_pk=self.token.pk)
+            tasks.update_structure_esi(id=1000000000001, token_pk=self.token.pk)
         except Exception as ex:
             self.fail(f"Unexpected exception occurred: {ex}")
 
     def test_invalid_token(self, mock_structure_update_or_create_esi):
         """When called with invalid token, raise exception"""
         mock_structure_update_or_create_esi.side_effect = EsiOffline
 
         with self.assertRaises(Token.DoesNotExist):
-            update_structure_esi(id=1000000000001, token_pk=generate_invalid_pk(Token))
+            tasks.update_structure_esi(
+                id=1000000000001, token_pk=generate_invalid_pk(Token)
+            )
 
     def test_esi_status_1(self, mock_structure_update_or_create_esi):
         """When ESI is offline, then retry"""
         mock_structure_update_or_create_esi.side_effect = EsiOffline
 
         with self.assertRaises(CeleryRetry):
-            update_structure_esi(id=1000000000001, token_pk=self.token.pk)
+            tasks.update_structure_esi(id=1000000000001, token_pk=self.token.pk)
 
     def test_esi_status_2(self, mock_structure_update_or_create_esi):
         """When ESI error limit reached, then retry"""
         mock_structure_update_or_create_esi.side_effect = EsiErrorLimitExceeded(5)
 
         with self.assertRaises(CeleryRetry):
-            update_structure_esi(id=1000000000001, token_pk=self.token.pk)
+            tasks.update_structure_esi(id=1000000000001, token_pk=self.token.pk)
 
 
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
-@patch(TASKS_PATH + ".MailEntity.objects.update_or_create_esi")
-class TestUpdateMailEntityEsi(TestCase):
+@patch(TASKS_PATH + ".MailEntity.objects.update_or_create_esi", spec=True)
+class TestUpdateMailEntityEsi(TestCaseTasks):
     def test_normal(self, mock_update_or_create_esi):
         """When ESI status is ok, then create MailEntity"""
         mock_update_or_create_esi.return_value = None
         try:
-            update_mail_entity_esi(1001)
+            tasks.update_mail_entity_esi(1001)
         except Exception:
             self.fail("Unexpected exception occurred")
 
     def test_esi_status_1(self, mock_update_or_create_esi):
         """When ESI is offline, then abort"""
         mock_update_or_create_esi.side_effect = EsiOffline
 
         with self.assertRaises(EsiOffline):
-            update_mail_entity_esi(1001)
+            tasks.update_mail_entity_esi(1001)
 
     def test_esi_status_2(self, mock_update_or_create_esi):
         """When ESI error limit reached, then abort"""
         mock_update_or_create_esi.side_effect = EsiErrorLimitExceeded(5)
 
         with self.assertRaises(EsiErrorLimitExceeded):
-            update_mail_entity_esi(1001)
+            tasks.update_mail_entity_esi(1001)
 
 
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-class TestUpdateCharactersDoctrines(TestCase):
+class TestUpdateCharactersDoctrines(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
 
     def setUp(self) -> None:
         self.character_1001 = create_memberaudit_character(1001)
 
     @patch(MODELS_PATH + ".character.Character.update_skill_sets")
     def test_normal(self, mock_update_skill_sets):
-        update_characters_skill_checks()
+        tasks.update_characters_skill_checks()
         self.assertTrue(mock_update_skill_sets.called)
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-class TestDeleteCharacter(TestCase):
+class TestDeleteCharacter(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
 
     def test_should_delete_a_character(self):
         # given
         character_1001 = create_memberaudit_character(1001)
         # when
-        delete_character.delay(character_1001.pk)
+        tasks.delete_character.delay(character_1001.pk)
         # then
         self.assertFalse(Character.objects.filter(pk=character_1001.pk).exists())
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-class TestExportData(TestCase):
+class TestExportData(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
         cls.character = create_memberaudit_character(1001)
 
-    @patch(TASKS_PATH + ".data_exporters.export_topic_to_archive")
+    @patch(TASKS_PATH + ".data_exporters.export_topic_to_archive", spec=True)
     def test_should_export_all_topics(self, mock_export_topic_to_file):
         # when
-        export_data()
+        tasks.export_data()
         # then
         called_topics = [
             call[1]["topic"] for call in mock_export_topic_to_file.call_args_list
         ]
         self.assertEqual(len(called_topics), 3)
         self.assertSetEqual(
             set(called_topics), {"contract", "contract-item", "wallet-journal"}
         )
 
-    @patch(TASKS_PATH + ".data_exporters.export_topic_to_archive")
+    @patch(TASKS_PATH + ".data_exporters.export_topic_to_archive", spec=True)
     def test_should_export_wallet_journal(self, mock_export_topic_to_file):
+        # given
+        user = self.character.user
         # when
-        _export_data_for_topic(topic="abc")
+        tasks.export_data_for_topic(topic="abc", user_pk=user.pk)
         # then
         self.assertTrue(mock_export_topic_to_file.called)
         _, kwargs = mock_export_topic_to_file.call_args
         self.assertEqual(kwargs["topic"], "abc")
 
 
-class TestUpdateComplianceGroupDesignations(TestCase):
+class TestUpdateComplianceGroupDesignations(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
 
-    @patch(TASKS_PATH + ".ComplianceGroupDesignation.objects.update_user")
+    @patch(TASKS_PATH + ".ComplianceGroupDesignation.objects.update_user", spec=True)
     def test_should_update_for_user(self, mock_update_user):
         # given
         user, _ = create_user_from_evecharacter(
             1001,
             permissions=["memberaudit.basic_access"],
             scopes=Character.get_esi_scopes(),
         )
         # when
-        update_compliance_groups_for_user(user.pk)
+        tasks.update_compliance_groups_for_user(user.pk)
         # then
         self.assertTrue(mock_update_user.called)
 
 
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
-@patch(TASKS_PATH + ".update_character")
-class TestUpdateAllCharacters(TestCase):
+@patch(TASKS_PATH + ".update_character", spec=True)
+class TestUpdateAllCharacters(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         load_locations()
 
@@ -877,81 +874,93 @@
         # given
         character_1001 = create_memberaudit_character(1001)
         character_1002 = create_memberaudit_character(1002)
         character_1003 = create_memberaudit_character(1003)
         character_1003.is_disabled = True
         character_1003.save()
         # when
-        update_all_characters()
+        tasks.update_all_characters()
         # then
         self.assertTrue(mock_update_character.apply_async.called)
         called_pks = {
             o[1]["kwargs"]["character_pk"]
             for o in mock_update_character.apply_async.call_args_list
         }
         self.assertSetEqual(called_pks, {character_1001.pk, character_1002.pk})
 
     def test_should_disable_orphaned_characters(self, mock_update_character):
         # given
         character_1001 = create_memberaudit_character(1001)
         eve_character_1002 = EveCharacter.objects.get(character_id=1002)
         character_1002 = create_character(eve_character_1002)
         # when
-        update_all_characters()
+        tasks.update_all_characters()
         # then
         character_1001.refresh_from_db()
         self.assertFalse(character_1001.is_disabled)
         character_1002.refresh_from_db()
         self.assertTrue(character_1002.is_disabled)
 
 
-@patch(TASKS_PATH + ".fetch_esi_status")
-class TestAbortMainTaskDuringDailyDowntime(TestCase):
-    @patch(TASKS_PATH + ".update_character")
+@patch(TASKS_PATH + ".fetch_esi_status", spec=True)
+class TestAbortMainTaskDuringDailyDowntime(TestCaseTasks):
+    @patch(TASKS_PATH + ".update_character", spec=True)
     def test_should_abort_update_all_characters(
         self, mock_update_character, mock_fetch_esi_status
     ):
         # given
         mock_fetch_esi_status.return_value.raise_for_status.side_effect = (
             EsiDailyDowntime
         )
         # when/then
-        update_all_characters()
+        tasks.update_all_characters()
         # then
         self.assertFalse(mock_update_character.apply_async.called)
 
     @patch(TASKS_PATH + ".EveMarketPrice.objects.update_from_esi")
     def test_should_abort_update_market_prices(
         self, mock_update_from_esi, mock_fetch_esi_status
     ):
         # given
         mock_fetch_esi_status.return_value.raise_for_status.side_effect = (
             EsiDailyDowntime
         )
         # when/then
-        update_market_prices()
+        tasks.update_market_prices()
         # then
         self.assertFalse(mock_update_from_esi.called)
 
 
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
-@patch(TASKS_PATH + ".EveEntity.objects.update_from_esi_by_id")
-class TestUpdateUnresolvedEveEntities(TestCase):
+@patch(TASKS_PATH + ".EveEntity.objects.update_from_esi_by_id", spec=True)
+class TestUpdateUnresolvedEveEntities(TestCaseTasks):
     def test_should_not_attempt_to_update_when_no_unresolved_entities(
         self, mock_update_from_esi_by_id
     ):
         # given
         create_eve_entity(id=1, name="alpha")
         # when
-        update_unresolved_eve_entities()
+        tasks.update_unresolved_eve_entities()
         # then
         self.assertFalse(mock_update_from_esi_by_id.called)
 
     def test_should_update_unresolved_entities(self, mock_update_from_esi_by_id):
         # given
         create_eve_entity(id=1)
         # when
-        update_unresolved_eve_entities()
+        tasks.update_unresolved_eve_entities()
         # then
         self.assertTrue(mock_update_from_esi_by_id.called)
         args, _ = mock_update_from_esi_by_id.call_args
         self.assertEqual(list(args[0]), [1])
+
+
+@patch(TASKS_PATH + ".check_character_consistency", spec=True)
+class TestCheckCharacterConsistency(TestCaseTasks):
+    def test_should_run_checks(self, mock_check_character_consistency):
+        # given
+        load_entities()
+        character = create_memberaudit_character(1001)
+        # when
+        tasks.check_character_consistency(character.pk)
+        # then
+        self.assertTrue(mock_check_character_consistency.called)
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/test_templatetags.py` & `aa_memberaudit-2.7.0/memberaudit/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/create_eveuniverse.py` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/entities.json` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/esi_client_stub.py` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/esi_testdata.json` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/esi_testdata.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/eveuniverse.json` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/factories.py` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 import random
 from itertools import count
 from pathlib import Path
 from typing import Iterable
 
 from django.contrib.auth.models import Group, User
 from django.utils.timezone import now
-from eveuniverse.models import EveSolarSystem, EveType
+from eveuniverse.models import EveEntity, EveSolarSystem, EveType
 
 from allianceauth.authentication.models import State
 from app_utils.testing import create_authgroup
 
 from memberaudit.constants import EveCategoryId
 from memberaudit.core.fittings import Fitting, Item, Module
 from memberaudit.core.skill_plans import SkillPlan
 from memberaudit.core.skills import Skill
 from memberaudit.models import (
     Character,
+    CharacterContact,
     CharacterContract,
+    CharacterContractBid,
     CharacterContractItem,
     CharacterFwStats,
     CharacterMail,
     CharacterMailLabel,
     CharacterMiningLedgerEntry,
     CharacterOnlineStatus,
     CharacterUpdateStatus,
@@ -129,14 +131,28 @@
         "started_at": now() - dt.timedelta(minutes=5),
         "finished_at": now(),
     }
     params.update(kwargs)
     return CharacterUpdateStatus.objects.create(**params)
 
 
+def create_character_contact(
+    character: Character, eve_entity: EveEntity, **kwargs
+) -> CharacterContact:
+    params = {
+        "character": character,
+        "eve_entity": eve_entity,
+        "is_blocked": False,
+        "is_watched": False,
+        "standing": 0.0,
+    }
+    params.update(kwargs)
+    return CharacterContact.objects.create(**params)
+
+
 def create_character_contract(character: Character, **kwargs) -> CharacterContract:
     date_issued = now() if "date_issued" not in kwargs else kwargs["date_issued"]
     params = {
         "character": character,
         "contract_id": next_number("contract_id"),
         "availability": CharacterContract.AVAILABILITY_PERSONAL,
         "contract_type": CharacterContract.TYPE_ITEM_EXCHANGE,
@@ -164,14 +180,28 @@
         "quantity": 1,
         "eve_type_id": 603,
     }
     params.update(kwargs)
     return CharacterContractItem.objects.create(**params)
 
 
+def create_character_contract_bid(
+    contract: CharacterContract, bidder: EveEntity, **kwargs
+) -> CharacterContractBid:
+    params = {
+        "contract": contract,
+        "bid_id": next_number("contract_item_bid_id"),
+        "amount": random.randint(1_000_000, 10_000_000_000),
+        "bidder": bidder,
+        "date_bid": now(),
+    }
+    params.update(kwargs)
+    return CharacterContractBid.objects.create(**params)
+
+
 def create_compliance_group(states: Iterable[State] = None, **kwargs) -> Group:
     group = create_authgroup(states, internal=True, **kwargs)
     create_compliance_group_designation(group)
     return group
 
 
 def create_compliance_group_designation(
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_archon.txt` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_archon.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_archon_max.txt` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_archon_max.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_svipul.txt` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_svipul.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_tengu.txt` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/fittings/fitting_tengu.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/generate_character.py` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/generate_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/generate_doctrines.py` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/generate_doctrines.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/load_entities.py` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/load_entities.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/load_locations.py` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/load_locations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/pilot_esi_error_handling.py` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/pilot_esi_error_handling.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/testdata/profiler_toolbox.py` & `aa_memberaudit-2.7.0/memberaudit/tests/testdata/profiler_toolbox.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/utils.py` & `aa_memberaudit-2.7.0/memberaudit/tests/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
 from typing import Tuple
 
 from django.contrib.auth.models import User
 from django.http import JsonResponse
-from django.test import RequestFactory
+from django.test import RequestFactory, TestCase
 from esi.models import Token
 from eveuniverse.models import EveEntity, EveSolarSystem, EveType
 
 from allianceauth.authentication.models import CharacterOwnership
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.tests.auth_utils import AuthUtils
-from app_utils.testing import add_character_to_user, response_text
+from allianceauth.utils.cache import get_redis_client
+from app_utils.testing import NoSocketsTestCase, add_character_to_user, response_text
 
 from ..models import Character, Location
 from .testdata.load_entities import load_entities
 from .testdata.load_eveuniverse import load_eveuniverse
 from .testdata.load_locations import load_locations
 
 
@@ -82,7 +83,22 @@
     data = json.loads(response_text(response))
     return data[data_key]
 
 
 def json_response_to_dict_2(response: JsonResponse, key="id", data_key="data") -> dict:
     """Convert JSON response into dict by given key."""
     return {x[key]: x for x in json_response_to_python_2(response, data_key)}
+
+
+def clear_celery_once_locks():
+    """Clear all celery once locks (if any exist)."""
+    r = get_redis_client()
+    if keys := r.keys(":?:qo_memberaudit.*"):
+        r.delete(*keys)
+
+
+class TestCaseWithFixtures(TestCase):
+    fixtures = ["disable_analytics.json"]
+
+
+class NoSocketsTestCaseFixtures(NoSocketsTestCase):
+    fixtures = ["disable_analytics.json"]
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/views/test_admin.py` & `aa_memberaudit-2.7.0/memberaudit/tests/views/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/views/test_character_finder.py` & `aa_memberaudit-2.7.0/memberaudit/tests/views/test_character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/views/test_character_viewer_1.py` & `aa_memberaudit-2.7.0/memberaudit/tests/views/test_character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/views/test_character_viewer_2.py` & `aa_memberaudit-2.7.0/memberaudit/tests/views/test_character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/views/test_characters.py` & `aa_memberaudit-2.7.0/memberaudit/tests/views/test_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/views/test_data_export.py` & `aa_memberaudit-2.7.0/memberaudit/tests/views/test_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tests/views/test_reports.py` & `aa_memberaudit-2.7.0/memberaudit/tests/views/test_reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/tools/drop_tables.sql` & `aa_memberaudit-2.7.0/memberaudit/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/urls.py` & `aa_memberaudit-2.7.0/memberaudit/urls.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/views/_common.py` & `aa_memberaudit-2.7.0/memberaudit/views/_common.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/views/admin.py` & `aa_memberaudit-2.7.0/memberaudit/views/admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/views/character_finder.py` & `aa_memberaudit-2.7.0/memberaudit/views/character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/views/character_viewer_1.py` & `aa_memberaudit-2.7.0/memberaudit/views/character_viewer_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import Optional, Tuple
 
 from django.contrib.auth.decorators import login_required, permission_required
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.db.models import Count, F, Max, Q, Sum
 from django.http import HttpResponse, HttpResponseNotFound, JsonResponse
 from django.shortcuts import render
@@ -704,23 +704,21 @@
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_fw_stats(
     request, character_pk: int, character: Character
 ) -> HttpResponse:
     try:
-        fw_stats: CharacterFwStats = character.fw_stats
+        fw_stats: Optional[CharacterFwStats] = character.fw_stats
     except ObjectDoesNotExist:
         fw_stats = None
-        logo_url = ""
+    if fw_stats:
+        logo_url = fw_stats.faction.logo_url(128) if fw_stats.faction else ""
     else:
-        if fw_stats.faction:
-            logo_url = fw_stats.faction.logo_url(128)
-        else:
-            logo_url = ""
+        logo_url = ""
     context = {"fw_stats": fw_stats, "faction_logo_url": logo_url}
     return render(
         request,
         "memberaudit/partials/character_viewer/tabs/fw_stats_content.html",
         context,
     )
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/views/character_viewer_2.py` & `aa_memberaudit-2.7.0/memberaudit/views/character_viewer_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_mail(
     request, character_pk: int, character: Character, mail_pk: int
-) -> JsonResponse:
+) -> HttpResponse:
     try:
         mail = (
             character.mails.select_related("sender")
             .prefetch_related("recipients")
             .get(pk=mail_pk)
         )
     except CharacterMail.DoesNotExist:
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/views/characters.py` & `aa_memberaudit-2.7.0/memberaudit/views/characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.3/memberaudit/views/data_export.py` & `aa_memberaudit-2.7.0/memberaudit/views/data_export.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required, permission_required
 from django.http import FileResponse, Http404
 from django.shortcuts import redirect, render
-from django.utils.html import format_html
 from django.utils.translation import gettext_lazy as _
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
 from .. import __title__, tasks
 from ..app_settings import MEMBERAUDIT_DATA_EXPORT_MIN_UPDATE_AGE
@@ -44,15 +43,14 @@
     return FileResponse(zip_file.open("rb"))
 
 
 @login_required
 @permission_required("memberaudit.exports_access")
 def data_export_run_update(request, topic: str):
     tasks.export_data_for_topic.delay(topic=topic, user_pk=request.user.pk)
-    format_html
     messages.info(
         request,
         _(
             "Data export for topic <strong>%s</strong> has been started. "
             "This can take a couple of minutes. "
             "You will get a notification once it is completed.",
         )
```

### Comparing `aa_memberaudit-2.6.3/memberaudit/views/reports.py` & `aa_memberaudit-2.7.0/memberaudit/views/reports.py`

 * *Files identical despite different names*

