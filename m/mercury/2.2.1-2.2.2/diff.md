# Comparing `tmp/mercury-2.2.1.tar.gz` & `tmp/mercury-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-2.2.1.tar", last modified: Wed Apr 12 08:54:34 2023, max compression
+gzip compressed data, was "mercury-2.2.2.tar", last modified: Thu Apr 20 15:51:25 2023, max compression
```

## Comparing `mercury-2.2.1.tar` & `mercury-2.2.2.tar`

### file list

```diff
@@ -1,211 +1,211 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.924365 mercury-2.2.1/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.2.1/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-12 08:54:34.924365 mercury-2.2.1/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4214 2023-02-15 10:26:45.000000 mercury-2.2.1/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2023-04-12 08:53:52.000000 mercury-2.2.1/mercury/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/accounts/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.1/mercury/apps/accounts/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.2.1/mercury/apps/accounts/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.2.1/mercury/apps/accounts/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.2.1/mercury/apps/accounts/fields.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/accounts/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/accounts/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.1/mercury/apps/accounts/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.2.1/mercury/apps/accounts/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.2.1/mercury/apps/accounts/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.2.1/mercury/apps/accounts/tasks.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/accounts/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.2.1/mercury/apps/accounts/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/accounts/tests/test_accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.2.1/mercury/apps/accounts/tests/test_invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/accounts/tests/test_secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-03-31 10:52:58.000000 mercury-2.2.1/mercury/apps/accounts/tests/test_sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/accounts/tests/test_subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2650 2023-03-24 11:47:32.000000 mercury-2.2.1/mercury/apps/accounts/urls.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/accounts/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.2.1/mercury/apps/accounts/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2006 2023-03-27 08:34:35.000000 mercury-2.2.1/mercury/apps/accounts/views/accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.2.1/mercury/apps/accounts/views/invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.2.1/mercury/apps/accounts/views/permissions.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.2.1/mercury/apps/accounts/views/secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6372 2023-03-31 10:52:58.000000 mercury-2.2.1/mercury/apps/accounts/views/sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4152 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/accounts/views/subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      436 2023-03-24 08:45:58.000000 mercury-2.2.1/mercury/apps/accounts/views/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/nb/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/nb/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/nb/exporter.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4086 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/nb/nbrun.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/nb/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.2.1/mercury/apps/nb/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      854 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/nb/tests/test_nbrun.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.2.1/mercury/apps/nb/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/nb/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/apps/nbworker/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/nbworker/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1719 2023-04-05 10:59:50.000000 mercury-2.2.1/mercury/apps/nbworker/__main__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17411 2023-04-12 08:48:16.000000 mercury-2.2.1/mercury/apps/nbworker/nb.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7485 2023-04-06 14:49:56.000000 mercury-2.2.1/mercury/apps/nbworker/rest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4864 2023-03-17 08:55:41.000000 mercury-2.2.1/mercury/apps/nbworker/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/nbworker/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2976 2023-03-31 09:54:03.000000 mercury-2.2.1/mercury/apps/nbworker/ws.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/notebooks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/notebooks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/notebooks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/notebooks/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/notebooks/management/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/notebooks/management/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/notebooks/management/commands/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/notebooks/management/commands/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.2.1/mercury/apps/notebooks/management/commands/add.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.2.1/mercury/apps/notebooks/management/commands/delete.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.2.1/mercury/apps/notebooks/management/commands/list.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/notebooks/management/commands/watch.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/notebooks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/notebooks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/notebooks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.2.1/mercury/apps/notebooks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.2.1/mercury/apps/notebooks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.2.1/mercury/apps/notebooks/slides_themes.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11689 2023-04-03 14:44:43.000000 mercury-2.2.1/mercury/apps/notebooks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.2.1/mercury/apps/notebooks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      567 2023-03-17 12:41:34.000000 mercury-2.2.1/mercury/apps/notebooks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3755 2023-03-17 08:55:41.000000 mercury-2.2.1/mercury/apps/notebooks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/storage/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/storage/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/storage/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/storage/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/storage/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/storage/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.2.1/mercury/apps/storage/migrations/0002_useruploadedfile.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/storage/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/storage/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.2.1/mercury/apps/storage/s3utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.2.1/mercury/apps/storage/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11397 2023-03-31 09:54:03.000000 mercury-2.2.1/mercury/apps/storage/storage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.2.1/mercury/apps/storage/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2132 2023-03-29 09:56:45.000000 mercury-2.2.1/mercury/apps/storage/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      445 2023-03-31 09:54:03.000000 mercury-2.2.1/mercury/apps/storage/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/storage/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.2.1/mercury/apps/storage/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6182 2023-03-31 11:42:07.000000 mercury-2.2.1/mercury/apps/storage/views/dashboardfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.2.1/mercury/apps/storage/views/notebookfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.2.1/mercury/apps/storage/views/workerfiles.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/tasks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/tasks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/tasks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/tasks/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.2.1/mercury/apps/tasks/clean_service.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3840 2023-04-03 14:18:32.000000 mercury-2.2.1/mercury/apps/tasks/export_pdf.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/tasks/export_png.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/tasks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/tasks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/apps/tasks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      762 2022-05-18 10:19:32.000000 mercury-2.2.1/mercury/apps/tasks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/tasks/notify.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.2.1/mercury/apps/tasks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.2.1/mercury/apps/tasks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1314 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/tasks/tasks_export.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/tasks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1401 2023-03-17 12:41:34.000000 mercury-2.2.1/mercury/apps/tasks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8619 2023-03-17 08:55:41.000000 mercury-2.2.1/mercury/apps/tasks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/workers/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/workers/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/workers/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/workers/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/workers/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/workers/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/workers/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      798 2023-03-29 09:06:05.000000 mercury-2.2.1/mercury/apps/workers/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/workers/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/workers/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1053 2023-03-17 12:41:34.000000 mercury-2.2.1/mercury/apps/workers/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3881 2023-03-31 09:54:03.000000 mercury-2.2.1/mercury/apps/workers/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/ws/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/ws/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/ws/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6162 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/ws/client.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/ws/middleware.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.916365 mercury-2.2.1/mercury/apps/ws/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/apps/ws/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.2.1/mercury/apps/ws/routing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2495 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/ws/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-03-01 11:07:38.000000 mercury-2.2.1/mercury/apps/ws/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5106 2023-04-06 13:49:54.000000 mercury-2.2.1/mercury/apps/ws/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1754 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/apps/ws/worker.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.2.1/mercury/demo.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.920365 mercury-2.2.1/mercury/frontend-dist/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/asset-manifest.json
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/favicon-old.ico
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/favicon.ico
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/index.html
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/jupyter-additional.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/jupyter-syntax.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   580386 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/jupyter-theme-light.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/manifest.json
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/mercury_black_logo.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/mercury_logo.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2023-04-12 08:54:20.000000 mercury-2.2.1/mercury/frontend-dist/robots.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury/frontend-dist/static/
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.920365 mercury-2.2.1/mercury/frontend-dist/static/css/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2831 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/css/main.26f96620.chunk.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5260 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.924365 mercury-2.2.1/mercury/frontend-dist/static/js/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/2.20950ecb.chunk.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/2.20950ecb.chunk.js.LICENSE.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)  4973512 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/2.20950ecb.chunk.js.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    83606 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/main.717ee96a.chunk.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   258957 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/main.717ee96a.chunk.js.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/runtime-main.248907bc.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.924365 mercury-2.2.1/mercury/frontend-dist/static/media/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/manage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8376 2023-04-07 10:38:38.000000 mercury-2.2.1/mercury/mercury.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      543 2023-03-30 08:36:26.000000 mercury-2.2.1/mercury/requirements.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.924365 mercury-2.2.1/mercury/server/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.2.1/mercury/server/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/server/asgi.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2771 2023-03-24 08:43:00.000000 mercury-2.2.1/mercury/server/celery.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9844 2023-04-05 13:16:51.000000 mercury-2.2.1/mercury/server/settings.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1572 2023-03-14 07:49:44.000000 mercury-2.2.1/mercury/server/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.2.1/mercury/server/views.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.2.1/mercury/server/wsgi.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.924365 mercury-2.2.1/mercury/widgets/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.1/mercury/widgets/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2029 2023-03-17 11:39:55.000000 mercury-2.2.1/mercury/widgets/app.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2294 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/button.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.2.1/mercury/widgets/chat.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2127 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/checkbox.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.2.1/mercury/widgets/confetti.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3393 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/file.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.2.1/mercury/widgets/json.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6894 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/manager.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.2.1/mercury/widgets/md.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2690 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/multiselect.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1219 2023-02-21 07:48:36.000000 mercury-2.2.1/mercury/widgets/note.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3016 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/numeric.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.2.1/mercury/widgets/outputdir.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3025 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/range.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2403 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/select.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/slider.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.2.1/mercury/widgets/stop.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2039 2023-04-07 10:30:37.000000 mercury-2.2.1/mercury/widgets/text.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-12 08:54:34.912365 mercury-2.2.1/mercury.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6285 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       50 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury.egg-info/entry_points.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      491 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-04-12 08:54:34.000000 mercury-2.2.1/mercury.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.2.1/pyproject.toml
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-04-12 08:54:34.924365 mercury-2.2.1/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1163 2023-04-12 08:54:01.000000 mercury-2.2.1/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.315957 mercury-2.2.2/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.2.2/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-20 15:51:25.315957 mercury-2.2.2/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4214 2023-02-15 10:26:45.000000 mercury-2.2.2/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.299957 mercury-2.2.2/mercury/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2023-04-20 15:50:34.000000 mercury-2.2.2/mercury/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.299957 mercury-2.2.2/mercury/apps/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/apps/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.299957 mercury-2.2.2/mercury/apps/accounts/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.2/mercury/apps/accounts/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.2.2/mercury/apps/accounts/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.2.2/mercury/apps/accounts/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.2.2/mercury/apps/accounts/fields.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.299957 mercury-2.2.2/mercury/apps/accounts/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.2.2/mercury/apps/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.2/mercury/apps/accounts/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.2.2/mercury/apps/accounts/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.2.2/mercury/apps/accounts/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.2.2/mercury/apps/accounts/tasks.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.299957 mercury-2.2.2/mercury/apps/accounts/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.2.2/mercury/apps/accounts/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.2.2/mercury/apps/accounts/tests/test_accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.2.2/mercury/apps/accounts/tests/test_invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.2.2/mercury/apps/accounts/tests/test_secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-03-31 10:52:58.000000 mercury-2.2.2/mercury/apps/accounts/tests/test_sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.2.2/mercury/apps/accounts/tests/test_subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2650 2023-03-24 11:47:32.000000 mercury-2.2.2/mercury/apps/accounts/urls.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.303957 mercury-2.2.2/mercury/apps/accounts/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.2.2/mercury/apps/accounts/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2006 2023-03-27 08:34:35.000000 mercury-2.2.2/mercury/apps/accounts/views/accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.2.2/mercury/apps/accounts/views/invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.2.2/mercury/apps/accounts/views/permissions.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.2.2/mercury/apps/accounts/views/secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6372 2023-03-31 10:52:58.000000 mercury-2.2.2/mercury/apps/accounts/views/sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4152 2023-03-29 09:06:05.000000 mercury-2.2.2/mercury/apps/accounts/views/subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      436 2023-03-24 08:45:58.000000 mercury-2.2.2/mercury/apps/accounts/views/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.303957 mercury-2.2.2/mercury/apps/nb/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/nb/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.2.2/mercury/apps/nb/exporter.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4086 2023-04-06 13:49:54.000000 mercury-2.2.2/mercury/apps/nb/nbrun.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.303957 mercury-2.2.2/mercury/apps/nb/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.2.2/mercury/apps/nb/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      854 2023-04-06 13:49:54.000000 mercury-2.2.2/mercury/apps/nb/tests/test_nbrun.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.2.2/mercury/apps/nb/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/nb/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.303957 mercury-2.2.2/mercury/apps/nbworker/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/nbworker/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1719 2023-04-05 10:59:50.000000 mercury-2.2.2/mercury/apps/nbworker/__main__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    17411 2023-04-12 08:48:16.000000 mercury-2.2.2/mercury/apps/nbworker/nb.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7485 2023-04-06 14:49:56.000000 mercury-2.2.2/mercury/apps/nbworker/rest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4864 2023-03-17 08:55:41.000000 mercury-2.2.2/mercury/apps/nbworker/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.2.2/mercury/apps/nbworker/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2927 2023-04-20 13:08:01.000000 mercury-2.2.2/mercury/apps/nbworker/ws.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.303957 mercury-2.2.2/mercury/apps/notebooks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/apps/notebooks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/apps/notebooks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/apps/notebooks/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.303957 mercury-2.2.2/mercury/apps/notebooks/management/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/apps/notebooks/management/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.303957 mercury-2.2.2/mercury/apps/notebooks/management/commands/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/apps/notebooks/management/commands/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.2.2/mercury/apps/notebooks/management/commands/add.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.2.2/mercury/apps/notebooks/management/commands/delete.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.2.2/mercury/apps/notebooks/management/commands/list.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/notebooks/management/commands/watch.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.303957 mercury-2.2.2/mercury/apps/notebooks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.2.2/mercury/apps/notebooks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/apps/notebooks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.2.2/mercury/apps/notebooks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.2.2/mercury/apps/notebooks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.2.2/mercury/apps/notebooks/slides_themes.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11689 2023-04-03 14:44:43.000000 mercury-2.2.2/mercury/apps/notebooks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.2.2/mercury/apps/notebooks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      567 2023-03-17 12:41:34.000000 mercury-2.2.2/mercury/apps/notebooks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3755 2023-03-17 08:55:41.000000 mercury-2.2.2/mercury/apps/notebooks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.303957 mercury-2.2.2/mercury/apps/storage/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/storage/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/storage/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/storage/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.303957 mercury-2.2.2/mercury/apps/storage/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.2.2/mercury/apps/storage/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.2.2/mercury/apps/storage/migrations/0002_useruploadedfile.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/storage/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.2.2/mercury/apps/storage/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.2.2/mercury/apps/storage/s3utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.2.2/mercury/apps/storage/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11397 2023-03-31 09:54:03.000000 mercury-2.2.2/mercury/apps/storage/storage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.2.2/mercury/apps/storage/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2132 2023-03-29 09:56:45.000000 mercury-2.2.2/mercury/apps/storage/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      445 2023-03-31 09:54:03.000000 mercury-2.2.2/mercury/apps/storage/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.303957 mercury-2.2.2/mercury/apps/storage/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.2.2/mercury/apps/storage/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6182 2023-03-31 11:42:07.000000 mercury-2.2.2/mercury/apps/storage/views/dashboardfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.2.2/mercury/apps/storage/views/notebookfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.2.2/mercury/apps/storage/views/workerfiles.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.303957 mercury-2.2.2/mercury/apps/tasks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/apps/tasks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/apps/tasks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/apps/tasks/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.2.2/mercury/apps/tasks/clean_service.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3840 2023-04-03 14:18:32.000000 mercury-2.2.2/mercury/apps/tasks/export_pdf.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.2.2/mercury/apps/tasks/export_png.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.307957 mercury-2.2.2/mercury/apps/tasks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.2.2/mercury/apps/tasks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/apps/tasks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      762 2022-05-18 10:19:32.000000 mercury-2.2.2/mercury/apps/tasks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/tasks/notify.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.2.2/mercury/apps/tasks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.2.2/mercury/apps/tasks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1314 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/tasks/tasks_export.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.2.2/mercury/apps/tasks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1401 2023-03-17 12:41:34.000000 mercury-2.2.2/mercury/apps/tasks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8619 2023-03-17 08:55:41.000000 mercury-2.2.2/mercury/apps/tasks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.307957 mercury-2.2.2/mercury/apps/workers/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.2/mercury/apps/workers/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.2.2/mercury/apps/workers/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.2.2/mercury/apps/workers/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.307957 mercury-2.2.2/mercury/apps/workers/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.2.2/mercury/apps/workers/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.2/mercury/apps/workers/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      798 2023-03-29 09:06:05.000000 mercury-2.2.2/mercury/apps/workers/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.2.2/mercury/apps/workers/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2023-03-14 07:49:44.000000 mercury-2.2.2/mercury/apps/workers/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1053 2023-03-17 12:41:34.000000 mercury-2.2.2/mercury/apps/workers/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3881 2023-03-31 09:54:03.000000 mercury-2.2.2/mercury/apps/workers/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.307957 mercury-2.2.2/mercury/apps/ws/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/ws/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/ws/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6162 2023-04-20 13:43:38.000000 mercury-2.2.2/mercury/apps/ws/client.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.2.2/mercury/apps/ws/middleware.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.307957 mercury-2.2.2/mercury/apps/ws/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/apps/ws/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.2.2/mercury/apps/ws/routing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2495 2023-04-06 13:49:54.000000 mercury-2.2.2/mercury/apps/ws/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-03-01 11:07:38.000000 mercury-2.2.2/mercury/apps/ws/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5106 2023-04-06 13:49:54.000000 mercury-2.2.2/mercury/apps/ws/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1754 2023-03-14 07:49:44.000000 mercury-2.2.2/mercury/apps/ws/worker.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.2.2/mercury/demo.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.307957 mercury-2.2.2/mercury/frontend-dist/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/asset-manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2023-04-20 15:51:00.000000 mercury-2.2.2/mercury/frontend-dist/favicon-old.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2023-04-20 15:51:00.000000 mercury-2.2.2/mercury/frontend-dist/favicon.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/index.html
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2023-04-20 15:51:00.000000 mercury-2.2.2/mercury/frontend-dist/jupyter-additional.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2023-04-20 15:51:00.000000 mercury-2.2.2/mercury/frontend-dist/jupyter-syntax.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   580386 2023-04-20 15:51:00.000000 mercury-2.2.2/mercury/frontend-dist/jupyter-theme-light.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2023-04-20 15:51:00.000000 mercury-2.2.2/mercury/frontend-dist/manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2023-04-20 15:51:00.000000 mercury-2.2.2/mercury/frontend-dist/mercury_black_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2023-04-20 15:51:00.000000 mercury-2.2.2/mercury/frontend-dist/mercury_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2023-04-20 15:51:00.000000 mercury-2.2.2/mercury/frontend-dist/robots.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.299957 mercury-2.2.2/mercury/frontend-dist/static/
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.307957 mercury-2.2.2/mercury/frontend-dist/static/css/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2831 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/css/main.26f96620.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5260 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.315957 mercury-2.2.2/mercury/frontend-dist/static/js/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/js/2.6305b467.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/js/2.6305b467.chunk.js.LICENSE.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  4973509 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/js/2.6305b467.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    83776 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/js/main.2749a4f6.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   259551 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/js/main.2749a4f6.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/js/runtime-main.248907bc.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.315957 mercury-2.2.2/mercury/frontend-dist/static/media/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2023-04-20 15:51:24.000000 mercury-2.2.2/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/manage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8376 2023-04-07 10:38:38.000000 mercury-2.2.2/mercury/mercury.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      543 2023-03-30 08:36:26.000000 mercury-2.2.2/mercury/requirements.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.315957 mercury-2.2.2/mercury/server/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.2.2/mercury/server/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-03-14 07:49:44.000000 mercury-2.2.2/mercury/server/asgi.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2771 2023-03-24 08:43:00.000000 mercury-2.2.2/mercury/server/celery.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9844 2023-04-05 13:16:51.000000 mercury-2.2.2/mercury/server/settings.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1572 2023-03-14 07:49:44.000000 mercury-2.2.2/mercury/server/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.2.2/mercury/server/views.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.2.2/mercury/server/wsgi.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.315957 mercury-2.2.2/mercury/widgets/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.2/mercury/widgets/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2029 2023-03-17 11:39:55.000000 mercury-2.2.2/mercury/widgets/app.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2294 2023-04-07 10:30:37.000000 mercury-2.2.2/mercury/widgets/button.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.2.2/mercury/widgets/chat.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2127 2023-04-07 10:30:37.000000 mercury-2.2.2/mercury/widgets/checkbox.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.2.2/mercury/widgets/confetti.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3393 2023-04-07 10:30:37.000000 mercury-2.2.2/mercury/widgets/file.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.2.2/mercury/widgets/json.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6894 2023-04-07 10:30:37.000000 mercury-2.2.2/mercury/widgets/manager.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.2.2/mercury/widgets/md.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2690 2023-04-07 10:30:37.000000 mercury-2.2.2/mercury/widgets/multiselect.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1219 2023-02-21 07:48:36.000000 mercury-2.2.2/mercury/widgets/note.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3016 2023-04-07 10:30:37.000000 mercury-2.2.2/mercury/widgets/numeric.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.2.2/mercury/widgets/outputdir.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3025 2023-04-07 10:30:37.000000 mercury-2.2.2/mercury/widgets/range.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2403 2023-04-07 10:30:37.000000 mercury-2.2.2/mercury/widgets/select.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-04-07 10:30:37.000000 mercury-2.2.2/mercury/widgets/slider.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.2.2/mercury/widgets/stop.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2039 2023-04-07 10:30:37.000000 mercury-2.2.2/mercury/widgets/text.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-20 15:51:25.299957 mercury-2.2.2/mercury.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-20 15:51:25.000000 mercury-2.2.2/mercury.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6285 2023-04-20 15:51:25.000000 mercury-2.2.2/mercury.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-04-20 15:51:25.000000 mercury-2.2.2/mercury.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       50 2023-04-20 15:51:25.000000 mercury-2.2.2/mercury.egg-info/entry_points.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      491 2023-04-20 15:51:25.000000 mercury-2.2.2/mercury.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-04-20 15:51:25.000000 mercury-2.2.2/mercury.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.2.2/pyproject.toml
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-04-20 15:51:25.315957 mercury-2.2.2/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1163 2023-04-20 15:50:42.000000 mercury-2.2.2/setup.py
```

### Comparing `mercury-2.2.1/PKG-INFO` & `mercury-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury
-Version: 2.2.1
+Version: 2.2.2
 Summary: Turn Jupyter Notebook to Web App and share with non-technical users
 Home-page: https://github.com/mljar/mercury
 Maintainer: MLJAR Sp. z o.o.
 Maintainer-email: contact@mljar.com
 License: UNKNOWN
 Description:
```

### Comparing `mercury-2.2.1/README.md` & `mercury-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/fields.py` & `mercury-2.2.2/mercury/apps/accounts/fields.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/migrations/0001_initial.py` & `mercury-2.2.2/mercury/apps/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/models.py` & `mercury-2.2.2/mercury/apps/accounts/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/serializers.py` & `mercury-2.2.2/mercury/apps/accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/tasks.py` & `mercury-2.2.2/mercury/apps/accounts/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/tests/test_accounts.py` & `mercury-2.2.2/mercury/apps/accounts/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/tests/test_invitations.py` & `mercury-2.2.2/mercury/apps/accounts/tests/test_invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/tests/test_secrets.py` & `mercury-2.2.2/mercury/apps/accounts/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/tests/test_sites.py` & `mercury-2.2.2/mercury/apps/accounts/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/tests/test_subscription.py` & `mercury-2.2.2/mercury/apps/accounts/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/urls.py` & `mercury-2.2.2/mercury/apps/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/views/accounts.py` & `mercury-2.2.2/mercury/apps/accounts/views/accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/views/invitations.py` & `mercury-2.2.2/mercury/apps/accounts/views/invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/views/permissions.py` & `mercury-2.2.2/mercury/apps/accounts/views/permissions.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/views/secrets.py` & `mercury-2.2.2/mercury/apps/accounts/views/secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/views/sites.py` & `mercury-2.2.2/mercury/apps/accounts/views/sites.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/accounts/views/subscription.py` & `mercury-2.2.2/mercury/apps/accounts/views/subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/nb/exporter.py` & `mercury-2.2.2/mercury/apps/nb/exporter.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/nb/nbrun.py` & `mercury-2.2.2/mercury/apps/nb/nbrun.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/nb/tests/test_nbrun.py` & `mercury-2.2.2/mercury/apps/nb/tests/test_nbrun.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/nb/tests.py` & `mercury-2.2.2/mercury/apps/nb/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/nbworker/__main__.py` & `mercury-2.2.2/mercury/apps/nbworker/__main__.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/nbworker/nb.py` & `mercury-2.2.2/mercury/apps/nbworker/nb.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/nbworker/rest.py` & `mercury-2.2.2/mercury/apps/nbworker/rest.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/nbworker/tests.py` & `mercury-2.2.2/mercury/apps/nbworker/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/nbworker/utils.py` & `mercury-2.2.2/mercury/apps/nbworker/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/nbworker/ws.py` & `mercury-2.2.2/mercury/apps/nbworker/ws.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,17 +43,17 @@
             )
         except Exception:
             log.exception("Exception when WS connect")
 
     def on_open(self, ws):
         log.info("Open ws connection")
         self.queue.put(json.dumps({"purpose": Purpose.InitNotebook}))
-        if self.worker_exists():
-            self.set_worker_state(WorkerState.Running)
-            self.send_state()
+        # just check if exists
+        self.worker_exists()
+        
 
     def on_close(self, ws, close_status_code, close_msg):
         global stop_event
         stop_event.set()
         self.sm.delete_worker_output_dir()
         log.info(f"WS close connection, status={close_status_code}, msg={close_msg}")
```

### Comparing `mercury-2.2.1/mercury/apps/notebooks/management/commands/add.py` & `mercury-2.2.2/mercury/apps/notebooks/management/commands/add.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/notebooks/management/commands/delete.py` & `mercury-2.2.2/mercury/apps/notebooks/management/commands/delete.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/notebooks/management/commands/list.py` & `mercury-2.2.2/mercury/apps/notebooks/management/commands/list.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/notebooks/management/commands/watch.py` & `mercury-2.2.2/mercury/apps/notebooks/management/commands/watch.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/notebooks/migrations/0001_initial.py` & `mercury-2.2.2/mercury/apps/notebooks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/notebooks/models.py` & `mercury-2.2.2/mercury/apps/notebooks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/notebooks/serializers.py` & `mercury-2.2.2/mercury/apps/notebooks/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/notebooks/slides_themes.py` & `mercury-2.2.2/mercury/apps/notebooks/slides_themes.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/notebooks/tasks.py` & `mercury-2.2.2/mercury/apps/notebooks/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/notebooks/urls.py` & `mercury-2.2.2/mercury/apps/notebooks/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/notebooks/views.py` & `mercury-2.2.2/mercury/apps/notebooks/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/storage/migrations/0001_initial.py` & `mercury-2.2.2/mercury/apps/storage/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/storage/migrations/0002_useruploadedfile.py` & `mercury-2.2.2/mercury/apps/storage/migrations/0002_useruploadedfile.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/storage/models.py` & `mercury-2.2.2/mercury/apps/storage/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/storage/s3utils.py` & `mercury-2.2.2/mercury/apps/storage/s3utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/storage/storage.py` & `mercury-2.2.2/mercury/apps/storage/storage.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/storage/tests.py` & `mercury-2.2.2/mercury/apps/storage/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/storage/urls.py` & `mercury-2.2.2/mercury/apps/storage/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/storage/views/dashboardfiles.py` & `mercury-2.2.2/mercury/apps/storage/views/dashboardfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/storage/views/notebookfiles.py` & `mercury-2.2.2/mercury/apps/storage/views/notebookfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/storage/views/workerfiles.py` & `mercury-2.2.2/mercury/apps/storage/views/workerfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/tasks/export_pdf.py` & `mercury-2.2.2/mercury/apps/tasks/export_pdf.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/tasks/export_png.py` & `mercury-2.2.2/mercury/apps/tasks/export_png.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/tasks/migrations/0001_initial.py` & `mercury-2.2.2/mercury/apps/tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/tasks/models.py` & `mercury-2.2.2/mercury/apps/tasks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/tasks/notify.py` & `mercury-2.2.2/mercury/apps/tasks/notify.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/tasks/tasks.py` & `mercury-2.2.2/mercury/apps/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/tasks/tasks_export.py` & `mercury-2.2.2/mercury/apps/tasks/tasks_export.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/tasks/tests.py` & `mercury-2.2.2/mercury/apps/tasks/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/tasks/urls.py` & `mercury-2.2.2/mercury/apps/tasks/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/tasks/views.py` & `mercury-2.2.2/mercury/apps/tasks/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/workers/migrations/0001_initial.py` & `mercury-2.2.2/mercury/apps/workers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/workers/models.py` & `mercury-2.2.2/mercury/apps/workers/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/workers/urls.py` & `mercury-2.2.2/mercury/apps/workers/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/workers/views.py` & `mercury-2.2.2/mercury/apps/workers/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/ws/client.py` & `mercury-2.2.2/mercury/apps/ws/client.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/ws/middleware.py` & `mercury-2.2.2/mercury/apps/ws/middleware.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/ws/tasks.py` & `mercury-2.2.2/mercury/apps/ws/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/ws/utils.py` & `mercury-2.2.2/mercury/apps/ws/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/apps/ws/worker.py` & `mercury-2.2.2/mercury/apps/ws/worker.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/demo.py` & `mercury-2.2.2/mercury/demo.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/asset-manifest.json` & `mercury-2.2.2/mercury/frontend-dist/asset-manifest.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7477678571428572%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/2.6305b467.chunk.js'), (4, "*

 * *                  "'static/js/main.2749a4f6.chunk.js')], delete: [4, 2]}",*

 * * "'files'": "{'main.js': '/static/js/main.2749a4f6.chunk.js', 'main.js.map': "*

 * *            "'/static/js/main.2749a4f6.chunk.js.map', 'static/js/2.6305b467.chunk.js': "*

 * *            "'/static/js/2.6305b467.chunk.js', 'static/js/2.6305b467.chunk.js.map': "*

 * *            "'/static/js/2.6305b467.chunk.js.map', 'static/js/2.6305b467.chunk.js.LICENSE.txt': "*

 * *             […]*

```diff
@@ -1,24 +1,24 @@
 {
     "entrypoints": [
         "static/js/runtime-main.248907bc.js",
         "static/css/2.c6cf5ff9.chunk.css",
-        "static/js/2.20950ecb.chunk.js",
+        "static/js/2.6305b467.chunk.js",
         "static/css/main.26f96620.chunk.css",
-        "static/js/main.717ee96a.chunk.js"
+        "static/js/main.2749a4f6.chunk.js"
     ],
     "files": {
         "index.html": "/index.html",
         "main.css": "/static/css/main.26f96620.chunk.css",
-        "main.js": "/static/js/main.717ee96a.chunk.js",
-        "main.js.map": "/static/js/main.717ee96a.chunk.js.map",
+        "main.js": "/static/js/main.2749a4f6.chunk.js",
+        "main.js.map": "/static/js/main.2749a4f6.chunk.js.map",
         "runtime-main.js": "/static/js/runtime-main.248907bc.js",
         "runtime-main.js.map": "/static/js/runtime-main.248907bc.js.map",
         "static/css/2.c6cf5ff9.chunk.css": "/static/css/2.c6cf5ff9.chunk.css",
         "static/css/2.c6cf5ff9.chunk.css.map": "/static/css/2.c6cf5ff9.chunk.css.map",
         "static/css/main.26f96620.chunk.css.map": "/static/css/main.26f96620.chunk.css.map",
-        "static/js/2.20950ecb.chunk.js": "/static/js/2.20950ecb.chunk.js",
-        "static/js/2.20950ecb.chunk.js.LICENSE.txt": "/static/js/2.20950ecb.chunk.js.LICENSE.txt",
-        "static/js/2.20950ecb.chunk.js.map": "/static/js/2.20950ecb.chunk.js.map",
+        "static/js/2.6305b467.chunk.js": "/static/js/2.6305b467.chunk.js",
+        "static/js/2.6305b467.chunk.js.LICENSE.txt": "/static/js/2.6305b467.chunk.js.LICENSE.txt",
+        "static/js/2.6305b467.chunk.js.map": "/static/js/2.6305b467.chunk.js.map",
         "static/media/font-awesome.min.css": "/static/media/fontawesome-webfont.f691f37e.woff"
     }
 }
```

### Comparing `mercury-2.2.1/mercury/frontend-dist/favicon-old.ico` & `mercury-2.2.2/mercury/frontend-dist/favicon-old.ico`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/favicon.ico` & `mercury-2.2.2/mercury/frontend-dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/index.html` & `mercury-2.2.2/mercury/frontend-dist/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/static/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Mercury: Easily share your Python notebooks"/><link rel="manifest" href="/static/manifest.json"/><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script><link rel="stylesheet" href="/static/jupyter-syntax.css"/><link rel="stylesheet" href="/static/jupyter-additional.css"/><link rel="stylesheet" href="/static/jupyter-theme-light.css"/><title>Mercury - Turn Jupyter Notebook to Web App</title><script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"></script><script>init_mathjax=function(){window.MathJax&&(MathJax.Hub.Config({showProcessingMessages:!1,TeX:{equationNumbers:{autoNumber:"AMS",useLabelIds:!0}},tex2jax:{inlineMath:[["$","$"],["\\(","\\)"]],displayMath:[["$$","$$"],["\\[","\\]"]],processEscapes:!0,processEnvironments:!0},displayAlign:"center",CommonHTML:{linebreaks:{automatic:!0}}}),MathJax.Hub.Queue(["Typeset",MathJax.Hub]))},init_mathjax()</script><link href="/static/css/2.c6cf5ff9.chunk.css" rel="stylesheet"><link href="/static/css/main.26f96620.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function r(r){for(var n,f,l=r[0],i=r[1],a=r[2],c=0,s=[];c<l.length;c++)f=l[c],Object.prototype.hasOwnProperty.call(o,f)&&o[f]&&s.push(o[f][0]),o[f]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(p&&p(r);s.length;)s.shift()();return u.push.apply(u,a||[]),t()}function t(){for(var e,r=0;r<u.length;r++){for(var t=u[r],n=!0,l=1;l<t.length;l++){var i=t[l];0!==o[i]&&(n=!1)}n&&(u.splice(r--,1),e=f(f.s=t[0]))}return e}var n={},o={1:0},u=[];function f(r){if(n[r])return n[r].exports;var t=n[r]={i:r,l:!1,exports:{}};return e[r].call(t.exports,t,t.exports,f),t.l=!0,t.exports}f.m=e,f.c=n,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(e,r){if(1&r&&(e=f(e)),8&r)return e;if(4&r&&"object"==typeof e&&e&&e.__esModule)return e;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:e}),2&r&&"string"!=typeof e)for(var n in e)f.d(t,n,function(r){return e[r]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="/";var l=this.webpackJsonpfrontend=this.webpackJsonpfrontend||[],i=l.push.bind(l);l.push=r,l=l.slice();for(var a=0;a<l.length;a++)r(l[a]);var p=i;t()}([])</script><script src="/static/js/2.20950ecb.chunk.js"></script><script src="/static/js/main.717ee96a.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/static/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Mercury: Easily share your Python notebooks"/><link rel="manifest" href="/static/manifest.json"/><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script><link rel="stylesheet" href="/static/jupyter-syntax.css"/><link rel="stylesheet" href="/static/jupyter-additional.css"/><link rel="stylesheet" href="/static/jupyter-theme-light.css"/><title>Mercury - Turn Jupyter Notebook to Web App</title><script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"></script><script>init_mathjax=function(){window.MathJax&&(MathJax.Hub.Config({showProcessingMessages:!1,TeX:{equationNumbers:{autoNumber:"AMS",useLabelIds:!0}},tex2jax:{inlineMath:[["$","$"],["\\(","\\)"]],displayMath:[["$$","$$"],["\\[","\\]"]],processEscapes:!0,processEnvironments:!0},displayAlign:"center",CommonHTML:{linebreaks:{automatic:!0}}}),MathJax.Hub.Queue(["Typeset",MathJax.Hub]))},init_mathjax()</script><link href="/static/css/2.c6cf5ff9.chunk.css" rel="stylesheet"><link href="/static/css/main.26f96620.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function r(r){for(var n,f,l=r[0],i=r[1],a=r[2],c=0,s=[];c<l.length;c++)f=l[c],Object.prototype.hasOwnProperty.call(o,f)&&o[f]&&s.push(o[f][0]),o[f]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(p&&p(r);s.length;)s.shift()();return u.push.apply(u,a||[]),t()}function t(){for(var e,r=0;r<u.length;r++){for(var t=u[r],n=!0,l=1;l<t.length;l++){var i=t[l];0!==o[i]&&(n=!1)}n&&(u.splice(r--,1),e=f(f.s=t[0]))}return e}var n={},o={1:0},u=[];function f(r){if(n[r])return n[r].exports;var t=n[r]={i:r,l:!1,exports:{}};return e[r].call(t.exports,t,t.exports,f),t.l=!0,t.exports}f.m=e,f.c=n,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(e,r){if(1&r&&(e=f(e)),8&r)return e;if(4&r&&"object"==typeof e&&e&&e.__esModule)return e;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:e}),2&r&&"string"!=typeof e)for(var n in e)f.d(t,n,function(r){return e[r]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="/";var l=this.webpackJsonpfrontend=this.webpackJsonpfrontend||[],i=l.push.bind(l);l.push=r,l=l.slice();for(var a=0;a<l.length;a++)r(l[a]);var p=i;t()}([])</script><script src="/static/js/2.6305b467.chunk.js"></script><script src="/static/js/main.2749a4f6.chunk.js"></script></body></html>
```

### Comparing `mercury-2.2.1/mercury/frontend-dist/jupyter-additional.css` & `mercury-2.2.2/mercury/frontend-dist/jupyter-additional.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/jupyter-syntax.css` & `mercury-2.2.2/mercury/frontend-dist/jupyter-syntax.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/jupyter-theme-light.css` & `mercury-2.2.2/mercury/frontend-dist/jupyter-theme-light.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/mercury_black_logo.svg` & `mercury-2.2.2/mercury/frontend-dist/mercury_black_logo.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/mercury_logo.svg` & `mercury-2.2.2/mercury/frontend-dist/mercury_logo.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css` & `mercury-2.2.2/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map` & `mercury-2.2.2/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/static/css/main.26f96620.chunk.css` & `mercury-2.2.2/mercury/frontend-dist/static/css/main.26f96620.chunk.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map` & `mercury-2.2.2/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/static/js/2.20950ecb.chunk.js` & `mercury-2.2.2/mercury/frontend-dist/static/js/2.6305b467.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 2.20950ecb.chunk.js.LICENSE.txt */
+/*! For license information please see 2.6305b467.chunk.js.LICENSE.txt */
 (this.webpackJsonpfrontend = this.webpackJsonpfrontend || []).push([
     [2],
     [function(e, t, n) {
         "use strict";
         e.exports = n(194)
     }, function(e, t, n) {
         "use strict";
@@ -447,15 +447,15 @@
                     }
             }), [s, u]);
             var f = n || o;
             return i.a.createElement(f.Provider, {
                 value: s
             }, a)
         };
-        n(10), n(40), n(55), n(125);
+        n(10), n(40), n(55), n(126);
 
         function d() {
             return Object(r.useContext)(o)
         }
 
         function p(e) {
             void 0 === e && (e = o);
@@ -6736,15 +6736,15 @@
             }) : e[t] = n, e
         }
         n.d(t, "a", (function() {
             return r
         }))
     }, function(e, t, n) {
         var r = n(262),
-            i = n(121),
+            i = n(122),
             o = n(35),
             a = n(36),
             s = n(72),
             u = n(26),
             l = n(28),
             c = {
                 exports: {}
@@ -7820,15 +7820,15 @@
                     writable: !0,
                     configurable: !0
                 }
             }), t && r(e, t)
         }
     }, function(e, t, n) {
         var r = n(62),
-            i = n(120),
+            i = n(121),
             o = n(268);
         e.exports = function(e) {
             var t = i();
             return function() {
                 var n, i = r(e);
                 if (t) {
                     var a = r(this).constructor;
@@ -7994,15 +7994,15 @@
             var o = n.indexOf(":"),
                 a = n.indexOf("?"),
                 s = n.indexOf("#"),
                 u = n.indexOf("/");
             return o < 0 || u > -1 && o > u || a > -1 && o > a || s > -1 && o > s || t.test(n.slice(0, o)) ? n : ""
         }
     }, function(e, t, n) {
-        var r = n(109),
+        var r = n(110),
             i = "object" == typeof self && self && self.Object === Object && self,
             o = r || i || Function("return this")();
         e.exports = o
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return i
@@ -10891,15 +10891,15 @@
             }
         };
         Object.defineProperty(t, "__esModule", {
             value: !0
         }), t.checkValuesAgainstBoundaries = t.relativeValue = t.useThumbOverlap = t.Direction = t.getTrackBackground = t.Range = void 0;
         var i = r(n(195));
         t.Range = i.default;
-        var o = n(106);
+        var o = n(107);
         Object.defineProperty(t, "getTrackBackground", {
             enumerable: !0,
             get: function() {
                 return o.getTrackBackground
             }
         }), Object.defineProperty(t, "useThumbOverlap", {
             enumerable: !0,
@@ -13566,15 +13566,15 @@
         }));
         var r = n(14),
             i = n(169),
             o = n.n(i),
             a = n(37),
             s = n(30),
             u = n(21),
-            l = n(117),
+            l = n(118),
             c = n(51),
             f = /[#.]/g,
             d = function(e) {
                 for (var t, n, r, i = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "div", o = e || "", a = {}, s = 0; s < o.length;) f.lastIndex = s, r = f.exec(o), (t = o.slice(s, r ? r.index : o.length)) && (n ? "#" === n ? a.id = t : Array.isArray(a.className) ? a.className.push(t) : a.className = [t] : i = t, s += t.length), r && (n = r[0], s++);
                 return {
                     type: "element",
                     tagName: i,
@@ -13807,15 +13807,15 @@
             return e.line && e.column ? e : null
         }
 
         function x(e) {
             return "messages" in e
         }
         var R = n(8),
-            L = n(118),
+            L = n(119),
             M = n(84),
             P = n.n(M),
             F = n(31),
             B = O,
             j = L.a,
             U = {}.hasOwnProperty,
             H = Object(F.a)("root"),
@@ -14497,15 +14497,15 @@
             function(e) {
                 e.Right = "to right", e.Left = "to left", e.Down = "to bottom", e.Up = "to top"
             }(t.Direction || (t.Direction = {}))
     }, function(e, t, n) {
         var r = n(44).Symbol;
         e.exports = r
     }, function(e, t, n) {
-        var r = n(119);
+        var r = n(120);
         e.exports = function(e, t) {
             if (e) {
                 if ("string" === typeof e) return r(e, t);
                 var n = Object.prototype.toString.call(e).slice(8, -1);
                 return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? r(e, t) : void 0
             }
         }
@@ -14676,14 +14676,19 @@
                             }
                         }
                     }
                 }]), n
             }(n(38));
         e.exports = s
     }, function(e, t, n) {
+        var r = n(187),
+            i = n(188),
+            o = i;
+        o.v1 = r, o.v4 = i, e.exports = o
+    }, function(e, t, n) {
         "use strict";
         Object.defineProperty(t, "__esModule", {
             value: !0
         }), t.FilePond = t.FileStatus = t.registerPlugin = void 0;
         var r, i = function() {
                 function e(e, t) {
                     for (var n = 0; n < t.length; n++) {
@@ -15052,15 +15057,15 @@
                         } else i.visibility = "hidden"
                     }
                     g(d), p(i)
                 }
             }), [e, n]), [m, d]
         }
     }, function(e, t, n) {
-        var r = n(108);
+        var r = n(109);
         e.exports = function(e, t) {
             if (e) {
                 if ("string" === typeof e) return r(e, t);
                 var n = Object.prototype.toString.call(e).slice(8, -1);
                 return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? r(e, t) : void 0
             }
         }, e.exports.default = e.exports, e.exports.__esModule = !0
@@ -15073,15 +15078,15 @@
     }, function(e, t, n) {
         (function(t) {
             var n = "object" == typeof t && t && t.Object === Object && t;
             e.exports = n
         }).call(this, n(93))
     }, function(e, t, n) {
         var r = n(61),
-            i = n(111);
+            i = n(112);
         e.exports = function(e) {
             if (!i(e)) return !1;
             var t = r(e);
             return "[object Function]" == t || "[object GeneratorFunction]" == t || "[object AsyncFunction]" == t || "[object Proxy]" == t
         }
     }, function(e, t) {
         e.exports = function(e) {
@@ -15098,16 +15103,16 @@
                 try {
                     return e + ""
                 } catch (t) {}
             }
             return ""
         }
     }, function(e, t, n) {
-        var r = n(110),
-            i = n(114);
+        var r = n(111),
+            i = n(115);
         e.exports = function(e) {
             return null != e && i(e.length) && !r(e)
         }
     }, function(e, t) {
         e.exports = function(e) {
             return "number" == typeof e && e > -1 && e % 1 == 0 && e <= 9007199254740991
         }
@@ -15221,15 +15226,15 @@
         "use strict";
         var r = n(26),
             i = n(28),
             o = n(35),
             a = n(36),
             s = n(38),
             u = n(74),
-            l = n(123),
+            l = n(124),
             c = function(e) {
                 o(n, e);
                 var t = a(n);
 
                 function n(e) {
                     var i;
                     return r(this, n), (i = t.call(this, e)).tokenizer = e, i.posTracker = s.install(e.preprocessor, l), i.currentAttrLocation = null, i.ctLoc = null, i
@@ -15354,19 +15359,14 @@
             }, i(t, n, o || t)
         }
         e.exports = i
     }, function(e, t, n) {
         "use strict";
         e.exports = n(185)
     }, function(e, t, n) {
-        var r = n(187),
-            i = n(188),
-            o = i;
-        o.v1 = r, o.v4 = i, e.exports = o
-    }, function(e, t, n) {
         e.exports = function() {
             "use strict";
             var e = function(e) {
                     return /^image\/jpeg/.test(e.type)
                 },
                 t = {
                     JPEG: 65496,
@@ -33013,16 +33013,16 @@
         }(e.exports);
         try {
             regeneratorRuntime = r
         } catch (i) {
             "object" === typeof globalThis ? globalThis.regeneratorRuntime = r : Function("r", "regeneratorRuntime = r")(r)
         }
     }, function(e, t, n) {
-        var r, i, o = n(104),
-            a = n(105),
+        var r, i, o = n(105),
+            a = n(106),
             s = 0,
             u = 0;
         e.exports = function(e, t, n) {
             var l = t && n || 0,
                 c = t || [],
                 f = (e = e || {}).node || r,
                 d = void 0 !== e.clockseq ? e.clockseq : i;
@@ -33039,16 +33039,16 @@
             c[l++] = v >>> 24 & 255, c[l++] = v >>> 16 & 255, c[l++] = v >>> 8 & 255, c[l++] = 255 & v;
             var b = h / 4294967296 * 1e4 & 268435455;
             c[l++] = b >>> 8 & 255, c[l++] = 255 & b, c[l++] = b >>> 24 & 15 | 16, c[l++] = b >>> 16 & 255, c[l++] = d >>> 8 | 128, c[l++] = 255 & d;
             for (var E = 0; E < 6; ++E) c[l + E] = f[E];
             return t || a(c)
         }
     }, function(e, t, n) {
-        var r = n(104),
-            i = n(105);
+        var r = n(105),
+            i = n(106);
         e.exports = function(e, t, n) {
             var o = t && n || 0;
             "string" == typeof e && (t = "binary" === e ? new Array(16) : null, e = null);
             var a = (e = e || {}).random || (e.rng || r)();
             if (a[6] = 15 & a[6] | 64, a[8] = 63 & a[8] | 128, t)
                 for (var s = 0; s < 16; ++s) t[o + s] = a[s];
             return t || i(a)
@@ -33900,15 +33900,15 @@
                     for (var o = arguments[t], a = 0, s = o.length; a < s; a++, i++) r[i] = o[a];
                 return r
             };
         Object.defineProperty(t, "__esModule", {
             value: !0
         });
         var u = a(n(1)),
-            l = n(106),
+            l = n(107),
             c = n(94),
             f = ["ArrowRight", "ArrowUp", "k", "PageUp"],
             d = ["ArrowLeft", "ArrowDown", "j", "PageDown"],
             p = function(e) {
                 function t(t) {
                     var n = e.call(this, t) || this;
                     if (n.trackRef = u.createRef(), n.thumbRefs = [], n.markRefs = [], n.state = {
@@ -34295,15 +34295,15 @@
                     max: 100
                 }, t
             }(u.Component);
         t.default = p
     }, function(e, t, n) {
         var r = n(197),
             i = n(198),
-            o = n(107),
+            o = n(108),
             a = n(199);
         e.exports = function(e, t) {
             return r(e) || i(e, t) || o(e, t) || a()
         }, e.exports.default = e.exports, e.exports.__esModule = !0
     }, function(e, t) {
         e.exports = function(e) {
             if (Array.isArray(e)) return e
@@ -34351,21 +34351,21 @@
                 o = Object.keys(e);
             for (r = 0; r < o.length; r++) n = o[r], t.indexOf(n) >= 0 || (i[n] = e[n]);
             return i
         }, e.exports.default = e.exports, e.exports.__esModule = !0
     }, function(e, t, n) {
         var r = n(203),
             i = n(204),
-            o = n(107),
+            o = n(108),
             a = n(205);
         e.exports = function(e) {
             return r(e) || i(e) || o(e) || a()
         }, e.exports.default = e.exports, e.exports.__esModule = !0
     }, function(e, t, n) {
-        var r = n(108);
+        var r = n(109);
         e.exports = function(e) {
             if (Array.isArray(e)) return r(e)
         }, e.exports.default = e.exports, e.exports.__esModule = !0
     }, function(e, t) {
         e.exports = function(e) {
             if ("undefined" !== typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
         }, e.exports.default = e.exports, e.exports.__esModule = !0
@@ -40326,15 +40326,15 @@
         }, p.strip = function(e) {
             return p.replace(e, "", !0)
         }, e.exports = p
     }, function(e, t, n) {
         var r = n(95),
             i = n(213),
             o = n(214),
-            a = n(113),
+            a = n(114),
             s = n(226),
             u = n(227),
             l = n(228),
             c = n(229),
             f = n(230),
             d = n(234),
             p = r ? r.iterator : void 0;
@@ -40355,15 +40355,15 @@
     }, function(e, t, n) {
         var r = n(215),
             i = n(222),
             o = n(223),
             a = n(224),
             s = n(225),
             u = n(61),
-            l = n(112),
+            l = n(113),
             c = "[object Map]",
             f = "[object Promise]",
             d = "[object Set]",
             p = "[object WeakMap]",
             h = "[object DataView]",
             m = l(r),
             g = l(i),
@@ -40389,18 +40389,18 @@
             }
             return t
         }), e.exports = y
     }, function(e, t, n) {
         var r = n(60)(n(44), "DataView");
         e.exports = r
     }, function(e, t, n) {
-        var r = n(110),
+        var r = n(111),
             i = n(219),
-            o = n(111),
-            a = n(112),
+            o = n(112),
+            a = n(113),
             s = /^\[object .+?Constructor\]$/,
             u = Function.prototype,
             l = Object.prototype,
             c = u.toString,
             f = l.hasOwnProperty,
             d = RegExp("^" + c.call(f).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
         e.exports = function(e) {
@@ -40453,15 +40453,15 @@
         var r = n(60)(n(44), "Set");
         e.exports = r
     }, function(e, t, n) {
         var r = n(60)(n(44), "WeakMap");
         e.exports = r
     }, function(e, t, n) {
         var r = n(61),
-            i = n(115),
+            i = n(116),
             o = n(71);
         e.exports = function(e) {
             return "string" == typeof e || !i(e) && o(e) && "[object String]" == r(e)
         }
     }, function(e, t) {
         e.exports = function(e) {
             for (var t, n = []; !(t = e.next()).done;) n.push(t.value);
@@ -40531,22 +40531,22 @@
         e.exports = function(e, t) {
             for (var n = -1, r = null == e ? 0 : e.length, i = Array(r); ++n < r;) i[n] = t(e[n], n, e);
             return i
         }
     }, function(e, t, n) {
         var r = n(238),
             i = n(249),
-            o = n(113);
+            o = n(114);
         e.exports = function(e) {
             return o(e) ? r(e) : i(e)
         }
     }, function(e, t, n) {
         var r = n(239),
             i = n(240),
-            o = n(115),
+            o = n(116),
             a = n(242),
             s = n(244),
             u = n(245),
             l = Object.prototype.hasOwnProperty;
         e.exports = function(e, t) {
             var n = o(e),
                 c = !n && i(e),
@@ -40586,15 +40586,15 @@
             var r = n(44),
                 i = n(243),
                 o = t && !t.nodeType && t,
                 a = o && "object" == typeof e && e && !e.nodeType && e,
                 s = a && a.exports === o ? r.Buffer : void 0,
                 u = (s ? s.isBuffer : void 0) || i;
             e.exports = u
-        }).call(this, n(116)(e))
+        }).call(this, n(117)(e))
     }, function(e, t) {
         e.exports = function() {
             return !1
         }
     }, function(e, t) {
         var n = /^(?:0|[1-9]\d*)$/;
         e.exports = function(e, t) {
@@ -40606,40 +40606,40 @@
             i = n(247),
             o = n(248),
             a = o && o.isTypedArray,
             s = a ? i(a) : r;
         e.exports = s
     }, function(e, t, n) {
         var r = n(61),
-            i = n(114),
+            i = n(115),
             o = n(71),
             a = {};
         a["[object Float32Array]"] = a["[object Float64Array]"] = a["[object Int8Array]"] = a["[object Int16Array]"] = a["[object Int32Array]"] = a["[object Uint8Array]"] = a["[object Uint8ClampedArray]"] = a["[object Uint16Array]"] = a["[object Uint32Array]"] = !0, a["[object Arguments]"] = a["[object Array]"] = a["[object ArrayBuffer]"] = a["[object Boolean]"] = a["[object DataView]"] = a["[object Date]"] = a["[object Error]"] = a["[object Function]"] = a["[object Map]"] = a["[object Number]"] = a["[object Object]"] = a["[object RegExp]"] = a["[object Set]"] = a["[object String]"] = a["[object WeakMap]"] = !1, e.exports = function(e) {
             return o(e) && i(e.length) && !!a[r(e)]
         }
     }, function(e, t) {
         e.exports = function(e) {
             return function(t) {
                 return e(t)
             }
         }
     }, function(e, t, n) {
         (function(e) {
-            var r = n(109),
+            var r = n(110),
                 i = t && !t.nodeType && t,
                 o = i && "object" == typeof e && e && !e.nodeType && e,
                 a = o && o.exports === i && r.process,
                 s = function() {
                     try {
                         var e = o && o.require && o.require("util").types;
                         return e || a && a.binding && a.binding("util")
                     } catch (t) {}
                 }();
             e.exports = s
-        }).call(this, n(116)(e))
+        }).call(this, n(117)(e))
     }, function(e, t, n) {
         var r = n(250),
             i = n(251),
             o = Object.prototype.hasOwnProperty;
         e.exports = function(e) {
             if (!r(e)) return i(e);
             var t = [];
@@ -40904,15 +40904,15 @@
             };
             return n.PropTypes = n, n
         }
     }, function(e, t, n) {
         "use strict";
         e.exports = "SECRET_DO_NOT_PASS_THIS_OR_YOU_WILL_BE_FIRED"
     }, function(e, t, n) {
-        var r = n(119);
+        var r = n(120);
         e.exports = function(e) {
             if (Array.isArray(e)) return r(e)
         }
     }, function(e, t) {
         e.exports = function(e) {
             if ("undefined" !== typeof Symbol && Symbol.iterator in Object(e)) return Array.from(e)
         }
@@ -41001,15 +41001,15 @@
         e.exports = s
     }, function(e, t) {
         e.exports = function(e) {
             return -1 !== Function.toString.call(e).indexOf("[native code]")
         }
     }, function(e, t, n) {
         var r = n(97),
-            i = n(120);
+            i = n(121);
 
         function o(t, n, a) {
             return i() ? e.exports = o = Reflect.construct : e.exports = o = function(e, t, n) {
                 var i = [null];
                 i.push.apply(i, t);
                 var o = new(Function.bind.apply(e, i));
                 return n && r(o, n.prototype), o
@@ -41544,15 +41544,15 @@
         "use strict";
         var r = n(26),
             i = n(28),
             o = n(35),
             a = n(36),
             s = n(38),
             u = n(74),
-            l = n(122),
+            l = n(123),
             c = n(276),
             f = n(54).TAG_NAMES,
             d = function(e) {
                 o(n, e);
                 var t = a(n);
 
                 function n(e) {
@@ -41702,15 +41702,15 @@
         "use strict";
         var r = n(26),
             i = n(28),
             o = n(35),
             a = n(36),
             s = n(100),
             u = n(278),
-            l = n(122),
+            l = n(123),
             c = n(38),
             f = function(e) {
                 o(n, e);
                 var t = a(n);
 
                 function n(e, i) {
                     var o;
@@ -41760,20 +41760,20 @@
                 return n
             }(a);
         e.exports = l
     }, function(e, t, n) {
         "use strict";
         var r = n(26),
             i = n(28),
-            o = n(124),
+            o = n(125),
             a = n(62),
             s = n(35),
             u = n(36),
             l = n(100),
-            c = n(123),
+            c = n(124),
             f = n(38),
             d = function(e) {
                 s(n, e);
                 var t = u(n);
 
                 function n(e, i) {
                     var o;
@@ -42159,23 +42159,23 @@
                             return i === c || i === f
                         } return t === u.SVG && (e === s.FOREIGN_OBJECT || e === s.DESC || e === s.TITLE)
             }(e, t, n)) || !(r && r !== u.MATHML || ! function(e, t) {
                 return t === u.MATHML && (e === s.MI || e === s.MO || e === s.MN || e === s.MS || e === s.MTEXT)
             }(e, t))
         }
     }, function(e, t, n) {}, function(e, t, n) {
-        var r = n(124),
+        var r = n(125),
             i = n(62),
             o = n(287),
             a = n(72),
             s = n(35),
             u = n(36),
             l = n(26),
             c = n(28),
-            f = n(121);
+            f = n(122);
         e.exports = function(e) {
             "use strict";
 
             function t(e) {
                 if (e && e.__esModule) return e;
                 var t = Object.create(null);
                 if (e) {
@@ -46341,15 +46341,15 @@
         var x = n(67);
 
         function R(e) {
             if (e) throw e
         }
         var L = n(130),
             M = n.n(L),
-            P = n(102),
+            P = n(103),
             F = n.n(P);
 
         function B(e) {
             if ("[object Object]" !== Object.prototype.toString.call(e)) return !1;
             var t = Object.getPrototypeOf(e);
             return null === t || t === Object.prototype
         }
@@ -49233,16 +49233,16 @@
         var nn = n(132),
             rn = n.n(nn);
 
         function on(e) {
             var t = e && "object" === typeof e && "text" === e.type ? e.value || "" : e;
             return "string" === typeof t && "" === t.replace(/[ \t\n\f\r]/g, "")
         }
-        var an = n(117),
-            sn = n(118),
+        var an = n(118),
+            sn = n(119),
             un = n(53),
             ln = n(52),
             cn = n(84),
             fn = n.n(cn),
             dn = {}.hasOwnProperty,
             pn = new Set(["table", "thead", "tbody", "tfoot", "tr"]);
 
@@ -50788,8 +50788,8 @@
                     if ("no-highlight" === r || "nohighlight" === r) return !1;
                     if ("lang-" === r.slice(0, 5)) return r.slice(5);
                     if ("language-" === r.slice(0, 9)) return r.slice(9)
                 }
         }
     }]
 ]);
-//# sourceMappingURL=2.20950ecb.chunk.js.map
+//# sourceMappingURL=2.6305b467.chunk.js.map
```

### Comparing `mercury-2.2.1/mercury/frontend-dist/static/js/2.20950ecb.chunk.js.LICENSE.txt` & `mercury-2.2.2/mercury/frontend-dist/static/js/2.6305b467.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mercury-2.2.1/mercury/frontend-dist/static/js/2.20950ecb.chunk.js.map` & `mercury-2.2.2/mercury/frontend-dist/static/js/2.6305b467.chunk.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.856661853147056%*

 * *Differences: {"'file'": "'static/js/2.6305b467.chunk.js'",*

 * * "'mappings'": "';kGAGEA,EAAOC,QAAUC,EAAQ,M,6BCAzBF,EAAOC,QAAUC,EAAQ,M,6BCH3B,2UAAIC,EAAS,EAEAC,EAAUC,IACVC,EAAaD,IACbE,EAAoBF,IACpBG,EAASH,IACTI,EAAiBJ,IACjBK,EAAiBL,IACjBM,EAAwBN,IAErC,SAASA,IACP,gBAAO,IAAOF,K,qbCLT,ICWMS,EAAaC,EAAW,YAQxBC,EAAaD,EAAW,MAexBE,EAAgBF,EAAW,cAS3BG,EAAoBH,EAAW,cAU/BI,EAAmBJ,EAAW,kBAkB9BK,EAAaL,EAAW,uBAW9B,SAASM,EAAaC,GAC3B,OAGW,OAATA,IAAkBA,EAAO,IAAe,MAATA,GAW5B,SAASC,EAA0BD,GACxC,OAAgB,OAATA,IAAkBA,EAAO,GAAc,KAATA,GAgBhC,SAASE,EAAm […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/2.20950ecb.chunk.js",
+    "file": "static/js/2.6305b467.chunk.js",
     "names": [
         "module",
         "exports",
         "require",
         "powers",
         "boolean",
         "increment",
@@ -5497,14 +5497,17 @@
         "nestedNoscriptInHead",
         "eofInElementThatCanContainOnlyText",
         "ErrorReportingMixinBase",
         "onParseError",
         "_setErrorLocation",
         "mxn",
         "_reportError",
+        "v1",
+        "v4",
+        "uuid",
         "FilePond",
         "FileStatus",
         "registerPlugin",
         "_react",
         "_react2",
         "_filepond",
         "isSupported",
@@ -5650,17 +5653,14 @@
         "_attachCurrentAttrLocationInfo",
         "modeName",
         "prevPos",
         "reduction",
         "superPropBase",
         "_get",
         "receiver",
-        "v1",
-        "v4",
-        "uuid",
         "isJPEG",
         "Marker",
         "JPEG",
         "APP1",
         "EXIF",
         "TIFF",
         "Orientation",
@@ -11692,14 +11692,15 @@
         "../node_modules/react-range/lib/types.js",
         "../node_modules/lodash/_Symbol.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/unsupportedIterableToArray.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/setPrototypeOf.js",
         "../node_modules/parse5/lib/common/unicode.js",
         "../node_modules/parse5/lib/common/error-codes.js",
         "../node_modules/parse5/lib/extensions/error-reporting/mixin-base.js",
+        "../node_modules/uuid/index.js",
         "../node_modules/react-filepond/dist/react-filepond.js",
         "../node_modules/extend/index.js",
         "../node_modules/uuid/lib/rng-browser.js",
         "../node_modules/uuid/lib/bytesToUuid.js",
         "../node_modules/react-range/lib/utils.js",
         "../node_modules/@babel/runtime/helpers/unsupportedIterableToArray.js",
         "../node_modules/@babel/runtime/helpers/arrayLikeToArray.js",
@@ -11716,15 +11717,14 @@
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/arrayLikeToArray.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/isNativeReflectConstruct.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/slicedToArray.js",
         "../node_modules/parse5/lib/extensions/location-info/tokenizer-mixin.js",
         "../node_modules/parse5/lib/extensions/position-tracking/preprocessor-mixin.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/get.js",
         "../node_modules/react-redux/node_modules/react-is/index.js",
-        "../node_modules/uuid/index.js",
         "../node_modules/filepond-plugin-image-exif-orientation/dist/filepond-plugin-image-exif-orientation.js",
         "../node_modules/filepond-plugin-image-preview/dist/filepond-plugin-image-preview.js",
         "../node_modules/filepond-plugin-file-validate-size/dist/filepond-plugin-file-validate-size.js",
         "../node_modules/unified/node_modules/is-buffer/index.js",
         "../node_modules/vfile/node_modules/is-buffer/index.js",
         "../node_modules/react-markdown/node_modules/react-is/index.js",
         "../node_modules/highlight.js/lib/languages/arduino.js",
@@ -12337,14 +12337,15 @@
         "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.Direction = void 0;\nvar Direction;\n(function (Direction) {\n    Direction[\"Right\"] = \"to right\";\n    Direction[\"Left\"] = \"to left\";\n    Direction[\"Down\"] = \"to bottom\";\n    Direction[\"Up\"] = \"to top\";\n})(Direction = exports.Direction || (exports.Direction = {}));\n",
         "var root = require('./_root');\n\n/** Built-in value references. */\nvar Symbol = root.Symbol;\n\nmodule.exports = Symbol;\n",
         "var arrayLikeToArray = require(\"./arrayLikeToArray\");\n\nfunction _unsupportedIterableToArray(o, minLen) {\n  if (!o) return;\n  if (typeof o === \"string\") return arrayLikeToArray(o, minLen);\n  var n = Object.prototype.toString.call(o).slice(8, -1);\n  if (n === \"Object\" && o.constructor) n = o.constructor.name;\n  if (n === \"Map\" || n === \"Set\") return Array.from(o);\n  if (n === \"Arguments\" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return arrayLikeToArray(o, minLen);\n}\n\nmodule.exports = _unsupportedIterableToArray;",
         "function _setPrototypeOf(o, p) {\n  module.exports = _setPrototypeOf = Object.setPrototypeOf || function _setPrototypeOf(o, p) {\n    o.__proto__ = p;\n    return o;\n  };\n\n  return _setPrototypeOf(o, p);\n}\n\nmodule.exports = _setPrototypeOf;",
         "'use strict';\n\nconst UNDEFINED_CODE_POINTS = [\n    0xfffe,\n    0xffff,\n    0x1fffe,\n    0x1ffff,\n    0x2fffe,\n    0x2ffff,\n    0x3fffe,\n    0x3ffff,\n    0x4fffe,\n    0x4ffff,\n    0x5fffe,\n    0x5ffff,\n    0x6fffe,\n    0x6ffff,\n    0x7fffe,\n    0x7ffff,\n    0x8fffe,\n    0x8ffff,\n    0x9fffe,\n    0x9ffff,\n    0xafffe,\n    0xaffff,\n    0xbfffe,\n    0xbffff,\n    0xcfffe,\n    0xcffff,\n    0xdfffe,\n    0xdffff,\n    0xefffe,\n    0xeffff,\n    0xffffe,\n    0xfffff,\n    0x10fffe,\n    0x10ffff\n];\n\nexports.REPLACEMENT_CHARACTER = '\\uFFFD';\n\nexports.CODE_POINTS = {\n    EOF: -1,\n    NULL: 0x00,\n    TABULATION: 0x09,\n    CARRIAGE_RETURN: 0x0d,\n    LINE_FEED: 0x0a,\n    FORM_FEED: 0x0c,\n    SPACE: 0x20,\n    EXCLAMATION_MARK: 0x21,\n    QUOTATION_MARK: 0x22,\n    NUMBER_SIGN: 0x23,\n    AMPERSAND: 0x26,\n    APOSTROPHE: 0x27,\n    HYPHEN_MINUS: 0x2d,\n    SOLIDUS: 0x2f,\n    DIGIT_0: 0x30,\n    DIGIT_9: 0x39,\n    SEMICOLON: 0x3b,\n    LESS_THAN_SIGN: 0x3c,\n    EQUALS_SIGN: 0x3d,\n    GREATER_THAN_SIGN: 0x3e,\n    QUESTION_MARK: 0x3f,\n    LATIN_CAPITAL_A: 0x41,\n    LATIN_CAPITAL_F: 0x46,\n    LATIN_CAPITAL_X: 0x58,\n    LATIN_CAPITAL_Z: 0x5a,\n    RIGHT_SQUARE_BRACKET: 0x5d,\n    GRAVE_ACCENT: 0x60,\n    LATIN_SMALL_A: 0x61,\n    LATIN_SMALL_F: 0x66,\n    LATIN_SMALL_X: 0x78,\n    LATIN_SMALL_Z: 0x7a,\n    REPLACEMENT_CHARACTER: 0xfffd\n};\n\nexports.CODE_POINT_SEQUENCES = {\n    DASH_DASH_STRING: [0x2d, 0x2d], //--\n    DOCTYPE_STRING: [0x44, 0x4f, 0x43, 0x54, 0x59, 0x50, 0x45], //DOCTYPE\n    CDATA_START_STRING: [0x5b, 0x43, 0x44, 0x41, 0x54, 0x41, 0x5b], //[CDATA[\n    SCRIPT_STRING: [0x73, 0x63, 0x72, 0x69, 0x70, 0x74], //script\n    PUBLIC_STRING: [0x50, 0x55, 0x42, 0x4c, 0x49, 0x43], //PUBLIC\n    SYSTEM_STRING: [0x53, 0x59, 0x53, 0x54, 0x45, 0x4d] //SYSTEM\n};\n\n//Surrogates\nexports.isSurrogate = function(cp) {\n    return cp >= 0xd800 && cp <= 0xdfff;\n};\n\nexports.isSurrogatePair = function(cp) {\n    return cp >= 0xdc00 && cp <= 0xdfff;\n};\n\nexports.getSurrogatePairCodePoint = function(cp1, cp2) {\n    return (cp1 - 0xd800) * 0x400 + 0x2400 + cp2;\n};\n\n//NOTE: excluding NULL and ASCII whitespace\nexports.isControlCodePoint = function(cp) {\n    return (\n        (cp !== 0x20 && cp !== 0x0a && cp !== 0x0d && cp !== 0x09 && cp !== 0x0c && cp >= 0x01 && cp <= 0x1f) ||\n        (cp >= 0x7f && cp <= 0x9f)\n    );\n};\n\nexports.isUndefinedCodePoint = function(cp) {\n    return (cp >= 0xfdd0 && cp <= 0xfdef) || UNDEFINED_CODE_POINTS.indexOf(cp) > -1;\n};\n",
         "'use strict';\n\nmodule.exports = {\n    controlCharacterInInputStream: 'control-character-in-input-stream',\n    noncharacterInInputStream: 'noncharacter-in-input-stream',\n    surrogateInInputStream: 'surrogate-in-input-stream',\n    nonVoidHtmlElementStartTagWithTrailingSolidus: 'non-void-html-element-start-tag-with-trailing-solidus',\n    endTagWithAttributes: 'end-tag-with-attributes',\n    endTagWithTrailingSolidus: 'end-tag-with-trailing-solidus',\n    unexpectedSolidusInTag: 'unexpected-solidus-in-tag',\n    unexpectedNullCharacter: 'unexpected-null-character',\n    unexpectedQuestionMarkInsteadOfTagName: 'unexpected-question-mark-instead-of-tag-name',\n    invalidFirstCharacterOfTagName: 'invalid-first-character-of-tag-name',\n    unexpectedEqualsSignBeforeAttributeName: 'unexpected-equals-sign-before-attribute-name',\n    missingEndTagName: 'missing-end-tag-name',\n    unexpectedCharacterInAttributeName: 'unexpected-character-in-attribute-name',\n    unknownNamedCharacterReference: 'unknown-named-character-reference',\n    missingSemicolonAfterCharacterReference: 'missing-semicolon-after-character-reference',\n    unexpectedCharacterAfterDoctypeSystemIdentifier: 'unexpected-character-after-doctype-system-identifier',\n    unexpectedCharacterInUnquotedAttributeValue: 'unexpected-character-in-unquoted-attribute-value',\n    eofBeforeTagName: 'eof-before-tag-name',\n    eofInTag: 'eof-in-tag',\n    missingAttributeValue: 'missing-attribute-value',\n    missingWhitespaceBetweenAttributes: 'missing-whitespace-between-attributes',\n    missingWhitespaceAfterDoctypePublicKeyword: 'missing-whitespace-after-doctype-public-keyword',\n    missingWhitespaceBetweenDoctypePublicAndSystemIdentifiers:\n        'missing-whitespace-between-doctype-public-and-system-identifiers',\n    missingWhitespaceAfterDoctypeSystemKeyword: 'missing-whitespace-after-doctype-system-keyword',\n    missingQuoteBeforeDoctypePublicIdentifier: 'missing-quote-before-doctype-public-identifier',\n    missingQuoteBeforeDoctypeSystemIdentifier: 'missing-quote-before-doctype-system-identifier',\n    missingDoctypePublicIdentifier: 'missing-doctype-public-identifier',\n    missingDoctypeSystemIdentifier: 'missing-doctype-system-identifier',\n    abruptDoctypePublicIdentifier: 'abrupt-doctype-public-identifier',\n    abruptDoctypeSystemIdentifier: 'abrupt-doctype-system-identifier',\n    cdataInHtmlContent: 'cdata-in-html-content',\n    incorrectlyOpenedComment: 'incorrectly-opened-comment',\n    eofInScriptHtmlCommentLikeText: 'eof-in-script-html-comment-like-text',\n    eofInDoctype: 'eof-in-doctype',\n    nestedComment: 'nested-comment',\n    abruptClosingOfEmptyComment: 'abrupt-closing-of-empty-comment',\n    eofInComment: 'eof-in-comment',\n    incorrectlyClosedComment: 'incorrectly-closed-comment',\n    eofInCdata: 'eof-in-cdata',\n    absenceOfDigitsInNumericCharacterReference: 'absence-of-digits-in-numeric-character-reference',\n    nullCharacterReference: 'null-character-reference',\n    surrogateCharacterReference: 'surrogate-character-reference',\n    characterReferenceOutsideUnicodeRange: 'character-reference-outside-unicode-range',\n    controlCharacterReference: 'control-character-reference',\n    noncharacterCharacterReference: 'noncharacter-character-reference',\n    missingWhitespaceBeforeDoctypeName: 'missing-whitespace-before-doctype-name',\n    missingDoctypeName: 'missing-doctype-name',\n    invalidCharacterSequenceAfterDoctypeName: 'invalid-character-sequence-after-doctype-name',\n    duplicateAttribute: 'duplicate-attribute',\n    nonConformingDoctype: 'non-conforming-doctype',\n    missingDoctype: 'missing-doctype',\n    misplacedDoctype: 'misplaced-doctype',\n    endTagWithoutMatchingOpenElement: 'end-tag-without-matching-open-element',\n    closingOfElementWithOpenChildElements: 'closing-of-element-with-open-child-elements',\n    disallowedContentInNoscriptInHead: 'disallowed-content-in-noscript-in-head',\n    openElementsLeftAfterEof: 'open-elements-left-after-eof',\n    abandonedHeadElementChild: 'abandoned-head-element-child',\n    misplacedStartTagForHeadElement: 'misplaced-start-tag-for-head-element',\n    nestedNoscriptInHead: 'nested-noscript-in-head',\n    eofInElementThatCanContainOnlyText: 'eof-in-element-that-can-contain-only-text'\n};\n",
         "'use strict';\n\nconst Mixin = require('../../utils/mixin');\n\nclass ErrorReportingMixinBase extends Mixin {\n    constructor(host, opts) {\n        super(host);\n\n        this.posTracker = null;\n        this.onParseError = opts.onParseError;\n    }\n\n    _setErrorLocation(err) {\n        err.startLine = err.endLine = this.posTracker.line;\n        err.startCol = err.endCol = this.posTracker.col;\n        err.startOffset = err.endOffset = this.posTracker.offset;\n    }\n\n    _reportError(code) {\n        const err = {\n            code: code,\n            startLine: -1,\n            startCol: -1,\n            startOffset: -1,\n            endLine: -1,\n            endCol: -1,\n            endOffset: -1\n        };\n\n        this._setErrorLocation(err);\n        this.onParseError(err);\n    }\n\n    _getOverriddenMethods(mxn) {\n        return {\n            _err(code) {\n                mxn._reportError(code);\n            }\n        };\n    }\n}\n\nmodule.exports = ErrorReportingMixinBase;\n",
+        "var v1 = require('./v1');\nvar v4 = require('./v4');\n\nvar uuid = v4;\nuuid.v1 = v1;\nuuid.v4 = v4;\n\nmodule.exports = uuid;\n",
         "/*!\n * react-filepond v7.1.1\n * A handy FilePond adapter component for React\n * \n * Copyright (c) 2021 PQINA\n * https://pqina.nl/filepond\n * \n * Licensed under the MIT license.\n */\n\n'use strict';\n\nObject.defineProperty(exports, \"__esModule\", {\n  value: true\n});\nexports.FilePond = exports.FileStatus = exports.registerPlugin = undefined;\n\nvar _createClass = function () { function defineProperties(target, props) { for (var i = 0; i < props.length; i++) { var descriptor = props[i]; descriptor.enumerable = descriptor.enumerable || false; descriptor.configurable = true; if (\"value\" in descriptor) descriptor.writable = true; Object.defineProperty(target, descriptor.key, descriptor); } } return function (Constructor, protoProps, staticProps) { if (protoProps) defineProperties(Constructor.prototype, protoProps); if (staticProps) defineProperties(Constructor, staticProps); return Constructor; }; }();\n\nvar _react = require('react');\n\nvar _react2 = _interopRequireDefault(_react);\n\nvar _filepond = require('filepond');\n\nfunction _interopRequireDefault(obj) { return obj && obj.__esModule ? obj : { default: obj }; }\n\nfunction _classCallCheck(instance, Constructor) { if (!(instance instanceof Constructor)) { throw new TypeError(\"Cannot call a class as a function\"); } }\n\nfunction _possibleConstructorReturn(self, call) { if (!self) { throw new ReferenceError(\"this hasn't been initialised - super() hasn't been called\"); } return call && (typeof call === \"object\" || typeof call === \"function\") ? call : self; }\n\nfunction _inherits(subClass, superClass) { if (typeof superClass !== \"function\" && superClass !== null) { throw new TypeError(\"Super expression must either be null or a function, not \" + typeof superClass); } subClass.prototype = Object.create(superClass && superClass.prototype, { constructor: { value: subClass, enumerable: false, writable: true, configurable: true } }); if (superClass) Object.setPrototypeOf ? Object.setPrototypeOf(subClass, superClass) : subClass.__proto__ = superClass; }\n\n// Import required methods and styles from the FilePond module, should not need anything else\n\n\n// We need to be able to call the registerPlugin method directly so we can add plugins\nexports.registerPlugin = _filepond.registerPlugin;\nexports.FileStatus = _filepond.FileStatus;\n\n// Do this once\n\nvar isSupported = (0, _filepond.supported)();\n\n// filtered methods\nvar filteredMethods = ['setOptions', 'on', 'off', 'onOnce', 'appendTo', 'insertAfter', 'insertBefore', 'isAttachedTo', 'replaceElement', 'restoreElement', 'destroy'];\n\n// The React <FilePond/> wrapper\n\nvar FilePond = exports.FilePond = function (_React$Component) {\n  _inherits(FilePond, _React$Component);\n\n  function FilePond(props) {\n    _classCallCheck(this, FilePond);\n\n    var _this = _possibleConstructorReturn(this, (FilePond.__proto__ || Object.getPrototypeOf(FilePond)).call(this, props));\n\n    _this.allowFilesSync = true;\n    return _this;\n  }\n\n  // Will setup FilePond instance when mounted\n\n\n  _createClass(FilePond, [{\n    key: 'componentDidMount',\n    value: function componentDidMount() {\n      var _this2 = this;\n\n      // exit here if not supported\n      if (!isSupported) return;\n\n      var options = Object.assign({}, this.props);\n\n      // if onupdate files is defined, make sure setFiles does not cause race condition\n      if (options.onupdatefiles) {\n        var cb = options.onupdatefiles;\n        options.onupdatefiles = function (items) {\n          _this2.allowFilesSync = false;\n          cb(items);\n        };\n      }\n\n      // Create our pond\n      this._pond = (0, _filepond.create)(this._element, options);\n\n      // Reference pond methods to FilePond component instance\n      Object.keys(this._pond).filter(function (key) {\n        return !filteredMethods.includes(key);\n      }).forEach(function (key) {\n        _this2[key] = _this2._pond[key];\n      });\n    }\n\n    // Will clean up FilePond instance when unmounted\n\n  }, {\n    key: 'componentWillUnmount',\n    value: function componentWillUnmount() {\n      // exit when no pond defined\n      if (!this._pond) return;\n      this._pond.destroy();\n      this.allowFilesSync = true;\n    }\n  }, {\n    key: 'shouldComponentUpdate',\n    value: function shouldComponentUpdate() {\n      if (!this.allowFilesSync) {\n        this.allowFilesSync = true;\n        return false;\n      }\n      return true;\n    }\n\n    // Something changed\n\n  }, {\n    key: 'componentDidUpdate',\n    value: function componentDidUpdate() {\n\n      // exit when no pond defined\n      if (!this._pond) return;\n\n      var options = Object.assign({}, this.props);\n\n      // this is only set onces, on didmount\n      delete options.onupdatefiles;\n\n      // update pond options based on new props\n      this._pond.setOptions(options);\n    }\n\n    // Renders basic element hook for FilePond to attach to\n\n  }, {\n    key: 'render',\n    value: function render() {\n      var _this3 = this;\n\n      var _props = this.props,\n          id = _props.id,\n          name = _props.name,\n          className = _props.className,\n          allowMultiple = _props.allowMultiple,\n          required = _props.required,\n          captureMethod = _props.captureMethod,\n          acceptedFileTypes = _props.acceptedFileTypes;\n\n      return (0, _react.createElement)('div', { className: 'filepond--wrapper' }, (0, _react.createElement)('input', {\n        type: 'file',\n        name: name,\n        id: id,\n        accept: acceptedFileTypes,\n        multiple: allowMultiple,\n        required: required,\n        className: className,\n        capture: captureMethod,\n        ref: function ref(element) {\n          return _this3._element = element;\n        }\n      }));\n    }\n  }]);\n\n  return FilePond;\n}(_react2.default.Component);\n\n\n",
         "'use strict';\n\nvar hasOwn = Object.prototype.hasOwnProperty;\nvar toStr = Object.prototype.toString;\nvar defineProperty = Object.defineProperty;\nvar gOPD = Object.getOwnPropertyDescriptor;\n\nvar isArray = function isArray(arr) {\n\tif (typeof Array.isArray === 'function') {\n\t\treturn Array.isArray(arr);\n\t}\n\n\treturn toStr.call(arr) === '[object Array]';\n};\n\nvar isPlainObject = function isPlainObject(obj) {\n\tif (!obj || toStr.call(obj) !== '[object Object]') {\n\t\treturn false;\n\t}\n\n\tvar hasOwnConstructor = hasOwn.call(obj, 'constructor');\n\tvar hasIsPrototypeOf = obj.constructor && obj.constructor.prototype && hasOwn.call(obj.constructor.prototype, 'isPrototypeOf');\n\t// Not own constructor property must be Object\n\tif (obj.constructor && !hasOwnConstructor && !hasIsPrototypeOf) {\n\t\treturn false;\n\t}\n\n\t// Own properties are enumerated firstly, so to speed up,\n\t// if last one is own, then all properties are own.\n\tvar key;\n\tfor (key in obj) { /**/ }\n\n\treturn typeof key === 'undefined' || hasOwn.call(obj, key);\n};\n\n// If name is '__proto__', and Object.defineProperty is available, define __proto__ as an own property on target\nvar setProperty = function setProperty(target, options) {\n\tif (defineProperty && options.name === '__proto__') {\n\t\tdefineProperty(target, options.name, {\n\t\t\tenumerable: true,\n\t\t\tconfigurable: true,\n\t\t\tvalue: options.newValue,\n\t\t\twritable: true\n\t\t});\n\t} else {\n\t\ttarget[options.name] = options.newValue;\n\t}\n};\n\n// Return undefined instead of __proto__ if '__proto__' is not an own property\nvar getProperty = function getProperty(obj, name) {\n\tif (name === '__proto__') {\n\t\tif (!hasOwn.call(obj, name)) {\n\t\t\treturn void 0;\n\t\t} else if (gOPD) {\n\t\t\t// In early versions of node, obj['__proto__'] is buggy when obj has\n\t\t\t// __proto__ as an own property. Object.getOwnPropertyDescriptor() works.\n\t\t\treturn gOPD(obj, name).value;\n\t\t}\n\t}\n\n\treturn obj[name];\n};\n\nmodule.exports = function extend() {\n\tvar options, name, src, copy, copyIsArray, clone;\n\tvar target = arguments[0];\n\tvar i = 1;\n\tvar length = arguments.length;\n\tvar deep = false;\n\n\t// Handle a deep copy situation\n\tif (typeof target === 'boolean') {\n\t\tdeep = target;\n\t\ttarget = arguments[1] || {};\n\t\t// skip the boolean and the target\n\t\ti = 2;\n\t}\n\tif (target == null || (typeof target !== 'object' && typeof target !== 'function')) {\n\t\ttarget = {};\n\t}\n\n\tfor (; i < length; ++i) {\n\t\toptions = arguments[i];\n\t\t// Only deal with non-null/undefined values\n\t\tif (options != null) {\n\t\t\t// Extend the base object\n\t\t\tfor (name in options) {\n\t\t\t\tsrc = getProperty(target, name);\n\t\t\t\tcopy = getProperty(options, name);\n\n\t\t\t\t// Prevent never-ending loop\n\t\t\t\tif (target !== copy) {\n\t\t\t\t\t// Recurse if we're merging plain objects or arrays\n\t\t\t\t\tif (deep && copy && (isPlainObject(copy) || (copyIsArray = isArray(copy)))) {\n\t\t\t\t\t\tif (copyIsArray) {\n\t\t\t\t\t\t\tcopyIsArray = false;\n\t\t\t\t\t\t\tclone = src && isArray(src) ? src : [];\n\t\t\t\t\t\t} else {\n\t\t\t\t\t\t\tclone = src && isPlainObject(src) ? src : {};\n\t\t\t\t\t\t}\n\n\t\t\t\t\t\t// Never move original objects, clone them\n\t\t\t\t\t\tsetProperty(target, { name: name, newValue: extend(deep, clone, copy) });\n\n\t\t\t\t\t// Don't bring in undefined values\n\t\t\t\t\t} else if (typeof copy !== 'undefined') {\n\t\t\t\t\t\tsetProperty(target, { name: name, newValue: copy });\n\t\t\t\t\t}\n\t\t\t\t}\n\t\t\t}\n\t\t}\n\t}\n\n\t// Return the modified object\n\treturn target;\n};\n",
         "// Unique ID creation requires a high quality random # generator.  In the\n// browser this is a little complicated due to unknown quality of Math.random()\n// and inconsistent support for the `crypto` API.  We do the best we can via\n// feature-detection\n\n// getRandomValues needs to be invoked in a context where \"this\" is a Crypto\n// implementation. Also, find the complete implementation of crypto on IE11.\nvar getRandomValues = (typeof(crypto) != 'undefined' && crypto.getRandomValues && crypto.getRandomValues.bind(crypto)) ||\n                      (typeof(msCrypto) != 'undefined' && typeof window.msCrypto.getRandomValues == 'function' && msCrypto.getRandomValues.bind(msCrypto));\n\nif (getRandomValues) {\n  // WHATWG crypto RNG - http://wiki.whatwg.org/wiki/Crypto\n  var rnds8 = new Uint8Array(16); // eslint-disable-line no-undef\n\n  module.exports = function whatwgRNG() {\n    getRandomValues(rnds8);\n    return rnds8;\n  };\n} else {\n  // Math.random()-based (RNG)\n  //\n  // If all else fails, use Math.random().  It's fast, but is of unspecified\n  // quality.\n  var rnds = new Array(16);\n\n  module.exports = function mathRNG() {\n    for (var i = 0, r; i < 16; i++) {\n      if ((i & 0x03) === 0) r = Math.random() * 0x100000000;\n      rnds[i] = r >>> ((i & 0x03) << 3) & 0xff;\n    }\n\n    return rnds;\n  };\n}\n",
         "/**\n * Convert array of 16 byte values to UUID string format of the form:\n * XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX\n */\nvar byteToHex = [];\nfor (var i = 0; i < 256; ++i) {\n  byteToHex[i] = (i + 0x100).toString(16).substr(1);\n}\n\nfunction bytesToUuid(buf, offset) {\n  var i = offset || 0;\n  var bth = byteToHex;\n  // join used to fix memory issue caused by concatenation: https://bugs.chromium.org/p/v8/issues/detail?id=3175#c4\n  return ([\n    bth[buf[i++]], bth[buf[i++]],\n    bth[buf[i++]], bth[buf[i++]], '-',\n    bth[buf[i++]], bth[buf[i++]], '-',\n    bth[buf[i++]], bth[buf[i++]], '-',\n    bth[buf[i++]], bth[buf[i++]], '-',\n    bth[buf[i++]], bth[buf[i++]],\n    bth[buf[i++]], bth[buf[i++]],\n    bth[buf[i++]], bth[buf[i++]]\n  ]).join('');\n}\n\nmodule.exports = bytesToUuid;\n",
         "\"use strict\";\nvar __spreadArrays = (this && this.__spreadArrays) || function () {\n    for (var s = 0, i = 0, il = arguments.length; i < il; i++) s += arguments[i].length;\n    for (var r = Array(s), k = 0, i = 0; i < il; i++)\n        for (var a = arguments[i], j = 0, jl = a.length; j < jl; j++, k++)\n            r[k] = a[j];\n    return r;\n};\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.useThumbOverlap = exports.assertUnreachable = exports.voidFn = exports.getTrackBackground = exports.replaceAt = exports.schd = exports.translate = exports.getClosestThumbIndex = exports.translateThumbs = exports.getPaddingAndBorder = exports.getMargin = exports.checkInitialOverlap = exports.checkValuesAgainstBoundaries = exports.checkBoundaries = exports.isVertical = exports.relativeValue = exports.normalizeValue = exports.isStepDivisible = exports.isTouchEvent = exports.getStepDecimals = void 0;\nvar react_1 = require(\"react\");\nvar types_1 = require(\"./types\");\nvar getStepDecimals = function (step) {\n    var decimals = step.toString().split('.')[1];\n    return decimals ? decimals.length : 0;\n};\nexports.getStepDecimals = getStepDecimals;\nfunction isTouchEvent(event) {\n    return ((event.touches && event.touches.length) ||\n        (event.changedTouches && event.changedTouches.length));\n}\nexports.isTouchEvent = isTouchEvent;\nfunction isStepDivisible(min, max, step) {\n    var res = (max - min) / step;\n    var precision = 8;\n    var roundedRes = Number(res.toFixed(precision));\n    return parseInt(roundedRes.toString(), 10) === roundedRes;\n}\nexports.isStepDivisible = isStepDivisible;\nfunction normalizeValue(value, index, min, max, step, allowOverlap, values) {\n    var BIG_NUM = 10e10;\n    value = Math.round(value * BIG_NUM) / BIG_NUM;\n    if (!allowOverlap) {\n        var prev = values[index - 1];\n        var next = values[index + 1];\n        if (prev && prev > value)\n            return prev;\n        if (next && next < value)\n            return next;\n    }\n    if (value > max)\n        return max;\n    if (value < min)\n        return min;\n    // `remainder` is a difference between the given value and a full step value\n    // that is closest lower to the given value and is in the range between the min value\n    // and the given value\n    var remainder = Math.floor(value * BIG_NUM - min * BIG_NUM) %\n        Math.floor(step * BIG_NUM);\n    var closestLowerNum = Math.floor(value * BIG_NUM - Math.abs(remainder));\n    var rounded = remainder === 0 ? value : closestLowerNum / BIG_NUM;\n    // Values with a remainder `< step/2` are rounded to the closest lower value\n    // while values with a remainder `= > step/2` are rounded to the closest bigger value\n    var res = Math.abs(remainder / BIG_NUM) < step / 2\n        ? rounded\n        : rounded + step;\n    var decimalPlaces = exports.getStepDecimals(step);\n    return parseFloat(res.toFixed(decimalPlaces));\n}\nexports.normalizeValue = normalizeValue;\nfunction relativeValue(value, min, max) {\n    return (value - min) / (max - min);\n}\nexports.relativeValue = relativeValue;\nfunction isVertical(direction) {\n    return direction === types_1.Direction.Up || direction === types_1.Direction.Down;\n}\nexports.isVertical = isVertical;\nfunction checkBoundaries(value, min, max) {\n    if (min >= max) {\n        throw new RangeError(\"min (\" + min + \") is equal/bigger than max (\" + max + \")\");\n    }\n    if (value < min) {\n        throw new RangeError(\"value (\" + value + \") is smaller than min (\" + min + \")\");\n    }\n    if (value > max) {\n        throw new RangeError(\"value (\" + value + \") is bigger than max (\" + max + \")\");\n    }\n}\nexports.checkBoundaries = checkBoundaries;\nfunction checkValuesAgainstBoundaries(value, min, max) {\n    if (value < min) {\n        // set selectedValue to min\n        return min;\n    }\n    if (value > max) {\n        // set selectedValue to max\n        return max;\n    }\n    else {\n        return value;\n    }\n}\nexports.checkValuesAgainstBoundaries = checkValuesAgainstBoundaries;\nfunction checkInitialOverlap(values) {\n    if (values.length < 2)\n        return;\n    if (!values.slice(1).every(function (item, i) { return values[i] <= item; })) {\n        throw new RangeError(\"values={[\" + values + \"]} needs to be sorted when allowOverlap={false}\");\n    }\n}\nexports.checkInitialOverlap = checkInitialOverlap;\nfunction getMargin(element) {\n    var style = window.getComputedStyle(element);\n    return {\n        top: parseInt(style['margin-top'], 10),\n        bottom: parseInt(style['margin-bottom'], 10),\n        left: parseInt(style['margin-left'], 10),\n        right: parseInt(style['margin-right'], 10)\n    };\n}\nexports.getMargin = getMargin;\nfunction getPaddingAndBorder(element) {\n    var style = window.getComputedStyle(element);\n    return {\n        top: parseInt(style['padding-top'], 10) + parseInt(style['border-top-width'], 10),\n        bottom: parseInt(style['padding-bottom'], 10) + parseInt(style['border-bottom-width'], 10),\n        left: parseInt(style['padding-left'], 10) + parseInt(style['border-left-width'], 10),\n        right: parseInt(style['padding-right'], 10) + parseInt(style['border-right-width'], 10),\n    };\n}\nexports.getPaddingAndBorder = getPaddingAndBorder;\nfunction translateThumbs(elements, offsets, rtl) {\n    var inverter = rtl ? -1 : 1;\n    elements.forEach(function (element, index) {\n        return translate(element, inverter * offsets[index].x, offsets[index].y);\n    });\n}\nexports.translateThumbs = translateThumbs;\n/**\n * Util function for calculating the index of the thumb that is closes to a given position\n * @param thumbs - array of Thumb element to calculate the distance from\n * @param clientX - target x position (mouse/touch)\n * @param clientY - target y position (mouse/touch)\n * @param direction - the direction of the track\n */\nfunction getClosestThumbIndex(thumbs, clientX, clientY, direction) {\n    var thumbIndex = 0;\n    var minThumbDistance = getThumbDistance(thumbs[0], clientX, clientY, direction);\n    for (var i = 1; i < thumbs.length; i++) {\n        var thumbDistance = getThumbDistance(thumbs[i], clientX, clientY, direction);\n        if (thumbDistance < minThumbDistance) {\n            minThumbDistance = thumbDistance;\n            thumbIndex = i;\n        }\n    }\n    return thumbIndex;\n}\nexports.getClosestThumbIndex = getClosestThumbIndex;\nfunction translate(element, x, y) {\n    element.style.transform = \"translate(\" + x + \"px, \" + y + \"px)\";\n}\nexports.translate = translate;\n// adapted from https://github.com/alexreardon/raf-schd\nvar schd = function (fn) {\n    var lastArgs = [];\n    var frameId = null;\n    var wrapperFn = function () {\n        var args = [];\n        for (var _i = 0; _i < arguments.length; _i++) {\n            args[_i] = arguments[_i];\n        }\n        lastArgs = args;\n        if (frameId) {\n            return;\n        }\n        frameId = requestAnimationFrame(function () {\n            frameId = null;\n            fn.apply(void 0, lastArgs);\n        });\n    };\n    return wrapperFn;\n};\nexports.schd = schd;\nfunction replaceAt(values, index, value) {\n    var ret = values.slice(0);\n    ret[index] = value;\n    return ret;\n}\nexports.replaceAt = replaceAt;\nfunction getTrackBackground(_a) {\n    var values = _a.values, colors = _a.colors, min = _a.min, max = _a.max, _b = _a.direction, direction = _b === void 0 ? types_1.Direction.Right : _b, _c = _a.rtl, rtl = _c === void 0 ? false : _c;\n    if (rtl && direction === types_1.Direction.Right) {\n        direction = types_1.Direction.Left;\n    }\n    else if (rtl && types_1.Direction.Left) {\n        direction = types_1.Direction.Right;\n    }\n    // sort values ascending\n    var progress = values.slice(0).sort(function (a, b) { return a - b; }).map(function (value) { return ((value - min) / (max - min)) * 100; });\n    var middle = progress.reduce(function (acc, point, index) {\n        return acc + \", \" + colors[index] + \" \" + point + \"%, \" + colors[index + 1] + \" \" + point + \"%\";\n    }, '');\n    return \"linear-gradient(\" + direction + \", \" + colors[0] + \" 0%\" + middle + \", \" + colors[colors.length - 1] + \" 100%)\";\n}\nexports.getTrackBackground = getTrackBackground;\nfunction voidFn() { }\nexports.voidFn = voidFn;\nfunction assertUnreachable(x) {\n    throw new Error(\"Didn't expect to get here\");\n}\nexports.assertUnreachable = assertUnreachable;\n/**\n * Util function for grabbing the true largest width of a thumb\n * including the label\n * @param thumbEl - Thumb element to grab the largest width from\n * @param value - Thumb value, not label value\n * @param separator - Label separator value\n */\nvar getThumbWidth = function (thumbEl, value, separator, decimalPlaces, valueToLabel) {\n    if (valueToLabel === void 0) { valueToLabel = function (value) { return value; }; }\n    var width = Math.ceil(__spreadArrays([thumbEl], Array.from(thumbEl.children)).reduce(function (width, el) {\n        var elWidth = Math.ceil(el.getBoundingClientRect().width);\n        /**\n         * If a label contains a merged label value, it won't return the true\n         * label width for that Thumb. Clone the label and change the value\n         * to that individual Thumb value in order to grab the true width.\n         */\n        if (el.innerText &&\n            el.innerText.includes(separator) &&\n            el.childElementCount === 0) {\n            var elClone = el.cloneNode(true);\n            elClone.innerHTML = valueToLabel(value.toFixed(decimalPlaces));\n            elClone.style.visibility = 'hidden';\n            document.body.appendChild(elClone);\n            elWidth = Math.ceil(elClone.getBoundingClientRect().width);\n            document.body.removeChild(elClone);\n        }\n        return elWidth > width ? elWidth : width;\n    }, thumbEl.getBoundingClientRect().width));\n    return width;\n};\n/**\n * Bulk of logic for thumb overlaps\n * Consider a scenario with 5 thumbs;\n * Thumb 1 overlaps with thumb 0 and thumb 2\n * Thumb 2 overlaps with thumb 3\n * We need an array that contains [0, 1, 2, 3]\n * The function needs to return the directly overlapping thumbs\n * and all thumbs overlapping linked to those and so on\n * @param index - Thumb index calculating overlaps for\n * @param offsets - Current Array of Thumb offsets for Range\n * @param thumbs - Array of Thumb elements\n * @param values - Array of Thumb values\n * @param separator - String separator for merged label values\n * @returns overlaps - Array of all overlapping thumbs from the index\n */\nvar getOverlaps = function (index, offsets, thumbs, values, separator, decimalPlaces, valueToLabel) {\n    if (valueToLabel === void 0) { valueToLabel = function (value) { return value; }; }\n    var overlaps = [];\n    /**\n     * Recursive function for building the overlaps Array\n     * If an overlap is found, find the overlaps for that overlap\n     * @param thumbIndex current Thumb index to find overlaps from\n     */\n    var buildOverlaps = function (thumbIndex) {\n        var thumbXWidth = getThumbWidth(thumbs[thumbIndex], values[thumbIndex], separator, decimalPlaces, valueToLabel);\n        var thumbX = offsets[thumbIndex].x;\n        /**\n         * Iterate through the Thumb offsets, if there is a match\n         * add the thumbIndex and siblingIndex to the overlaps Array\n         *\n         * Then build overlaps from the overlapping siblingIndex\n         */\n        offsets.forEach(function (_a, siblingIndex) {\n            var siblingX = _a.x;\n            var siblingWidth = getThumbWidth(thumbs[siblingIndex], values[siblingIndex], separator, decimalPlaces, valueToLabel);\n            if (thumbIndex !== siblingIndex &&\n                ((thumbX >= siblingX && thumbX <= siblingX + siblingWidth) ||\n                    (thumbX + thumbXWidth >= siblingX &&\n                        thumbX + thumbXWidth <= siblingX + siblingWidth))) {\n                if (!overlaps.includes(siblingIndex)) {\n                    overlaps.push(thumbIndex);\n                    overlaps.push(siblingIndex);\n                    overlaps = __spreadArrays(overlaps, [thumbIndex, siblingIndex]);\n                    buildOverlaps(siblingIndex);\n                }\n            }\n        });\n    };\n    buildOverlaps(index);\n    // Sort and remove duplicates from the built overlaps\n    return Array.from(new Set(overlaps.sort()));\n};\n/**\n * A custom React Hook for calculating whether a thumb overlaps\n * another and whether labels could/should merge.\n * @param rangeRef - React ref value of Range component\n * @param values - current Range values Array\n * @param index - thumb index\n * @param step - step value, used to calculate the number of decimal places\n * @param separator - string to separate thumb values\n * @returns label value + styling for thumb label\n */\nvar useThumbOverlap = function (rangeRef, values, index, step, separator, valueToLabel) {\n    if (step === void 0) { step = 0.1; }\n    if (separator === void 0) { separator = ' - '; }\n    if (valueToLabel === void 0) { valueToLabel = function (value) { return value; }; }\n    var decimalPlaces = exports.getStepDecimals(step);\n    // Create initial label style and value. Label value defaults to thumb value\n    var _a = react_1.useState({}), labelStyle = _a[0], setLabelStyle = _a[1];\n    var _b = react_1.useState(valueToLabel(values[index].toFixed(decimalPlaces))), labelValue = _b[0], setLabelValue = _b[1];\n    // When the rangeRef or values change, update the Thumb label values and styling\n    react_1.useEffect(function () {\n        if (rangeRef) {\n            var thumbs = rangeRef.getThumbs();\n            if (thumbs.length < 1)\n                return;\n            var newStyle = {};\n            var offsets_1 = rangeRef.getOffsets();\n            /**\n             * Get any overlaps for the given Thumb index. This must return all linked\n             * Thumbs. So if there are 4 Thumbs and Thumbs 2, 3 and 4 overlap. If we are\n             * getting the overlaps for Thumb 1 and it overlaps only Thumb 2, we must get\n             * 2, 3 and 4 also.\n             */\n            var overlaps = getOverlaps(index, offsets_1, thumbs, values, separator, decimalPlaces, valueToLabel);\n            // Set a default label value of the Thumb value\n            var labelValue_1 = valueToLabel(values[index].toFixed(decimalPlaces));\n            /**\n             * If there are overlaps for the Thumb, we need to calculate the correct\n             * Label value along with the relevant styling. We only want to show a Label\n             * for the left most Thumb in an overlapping set.\n             * All other Thumbs will be set to display: none.\n             */\n            if (overlaps.length) {\n                /**\n                 * Get an Array of the offsets for the overlapping Thumbs\n                 * This is so we can determine if the Thumb we are looking at\n                 * is the left most thumb in an overlapping set\n                 */\n                var offsetsX = overlaps.reduce(function (a, c, i, s) {\n                    return a.length ? __spreadArrays(a, [offsets_1[s[i]].x]) : [offsets_1[s[i]].x];\n                }, []);\n                /**\n                 * If our Thumb is the left most Thumb, we can build a Label value\n                 * and set the style for that Label\n                 */\n                if (Math.min.apply(Math, offsetsX) === offsets_1[index].x) {\n                    /**\n                     * First calculate the Label value. To do this,\n                     * grab all the values for the Thumbs in our overlaps.\n                     * Then convert that to a Set and sort it whilst removing duplicates.\n                     */\n                    var labelValues_1 = [];\n                    overlaps.forEach(function (thumb) {\n                        labelValues_1.push(values[thumb].toFixed(decimalPlaces));\n                    });\n                    /**\n                     *  Update the labelValue with the resulting Array\n                     *  joined by our defined separator\n                     */\n                    labelValue_1 = Array.from(new Set(labelValues_1.sort(function (a, b) { return parseFloat(a) - parseFloat(b); })))\n                        .map(valueToLabel)\n                        .join(separator);\n                    /**\n                     * Lastly, build the label styling. The label styling will\n                     * position the label and apply a transform so that it's centered.\n                     * We want the center point between the left edge of the left most Thumb\n                     * and the right edge of the right most Thumb.\n                     */\n                    var first = Math.min.apply(Math, offsetsX);\n                    var last = Math.max.apply(Math, offsetsX);\n                    var lastWidth = thumbs[overlaps[offsetsX.indexOf(last)]].getBoundingClientRect().width;\n                    newStyle.left = Math.abs(first - (last + lastWidth)) / 2 + \"px\";\n                    newStyle.transform = 'translate(-50%, 0)';\n                }\n                else {\n                    // If the Thumb isn't the left most Thumb, hide the Label!\n                    newStyle.visibility = 'hidden';\n                }\n            }\n            // Update the label value and style\n            setLabelValue(labelValue_1);\n            setLabelStyle(newStyle);\n        }\n    }, [rangeRef, values]);\n    return [labelValue, labelStyle];\n};\nexports.useThumbOverlap = useThumbOverlap;\n/**\n * Util function for calculating the distance of the center of a thumb\n * form a given mouse/touch target's position\n * @param thumbEl - Thumb element to calculate the distance from\n * @param clientX - target x position (mouse/touch)\n * @param clientY - target y position (mouse/touch)\n * @param direction - the direction of the track\n */\nfunction getThumbDistance(thumbEl, clientX, clientY, direction) {\n    var _a = thumbEl.getBoundingClientRect(), left = _a.left, top = _a.top, width = _a.width, height = _a.height;\n    return isVertical(direction) ? Math.abs(clientY - (top + height / 2)) : Math.abs(clientX - (left + width / 2));\n}\n",
         "var arrayLikeToArray = require(\"./arrayLikeToArray.js\");\n\nfunction _unsupportedIterableToArray(o, minLen) {\n  if (!o) return;\n  if (typeof o === \"string\") return arrayLikeToArray(o, minLen);\n  var n = Object.prototype.toString.call(o).slice(8, -1);\n  if (n === \"Object\" && o.constructor) n = o.constructor.name;\n  if (n === \"Map\" || n === \"Set\") return Array.from(o);\n  if (n === \"Arguments\" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return arrayLikeToArray(o, minLen);\n}\n\nmodule.exports = _unsupportedIterableToArray;\nmodule.exports[\"default\"] = module.exports, module.exports.__esModule = true;",
         "function _arrayLikeToArray(arr, len) {\n  if (len == null || len > arr.length) len = arr.length;\n\n  for (var i = 0, arr2 = new Array(len); i < len; i++) {\n    arr2[i] = arr[i];\n  }\n\n  return arr2;\n}\n\nmodule.exports = _arrayLikeToArray;\nmodule.exports[\"default\"] = module.exports, module.exports.__esModule = true;",
@@ -12361,15 +12362,14 @@
         "function _arrayLikeToArray(arr, len) {\n  if (len == null || len > arr.length) len = arr.length;\n\n  for (var i = 0, arr2 = new Array(len); i < len; i++) {\n    arr2[i] = arr[i];\n  }\n\n  return arr2;\n}\n\nmodule.exports = _arrayLikeToArray;",
         "function _isNativeReflectConstruct() {\n  if (typeof Reflect === \"undefined\" || !Reflect.construct) return false;\n  if (Reflect.construct.sham) return false;\n  if (typeof Proxy === \"function\") return true;\n\n  try {\n    Date.prototype.toString.call(Reflect.construct(Date, [], function () {}));\n    return true;\n  } catch (e) {\n    return false;\n  }\n}\n\nmodule.exports = _isNativeReflectConstruct;",
         "var arrayWithHoles = require(\"./arrayWithHoles\");\n\nvar iterableToArrayLimit = require(\"./iterableToArrayLimit\");\n\nvar unsupportedIterableToArray = require(\"./unsupportedIterableToArray\");\n\nvar nonIterableRest = require(\"./nonIterableRest\");\n\nfunction _slicedToArray(arr, i) {\n  return arrayWithHoles(arr) || iterableToArrayLimit(arr, i) || unsupportedIterableToArray(arr, i) || nonIterableRest();\n}\n\nmodule.exports = _slicedToArray;",
         "'use strict';\n\nconst Mixin = require('../../utils/mixin');\nconst Tokenizer = require('../../tokenizer');\nconst PositionTrackingPreprocessorMixin = require('../position-tracking/preprocessor-mixin');\n\nclass LocationInfoTokenizerMixin extends Mixin {\n    constructor(tokenizer) {\n        super(tokenizer);\n\n        this.tokenizer = tokenizer;\n        this.posTracker = Mixin.install(tokenizer.preprocessor, PositionTrackingPreprocessorMixin);\n        this.currentAttrLocation = null;\n        this.ctLoc = null;\n    }\n\n    _getCurrentLocation() {\n        return {\n            startLine: this.posTracker.line,\n            startCol: this.posTracker.col,\n            startOffset: this.posTracker.offset,\n            endLine: -1,\n            endCol: -1,\n            endOffset: -1\n        };\n    }\n\n    _attachCurrentAttrLocationInfo() {\n        this.currentAttrLocation.endLine = this.posTracker.line;\n        this.currentAttrLocation.endCol = this.posTracker.col;\n        this.currentAttrLocation.endOffset = this.posTracker.offset;\n\n        const currentToken = this.tokenizer.currentToken;\n        const currentAttr = this.tokenizer.currentAttr;\n\n        if (!currentToken.location.attrs) {\n            currentToken.location.attrs = Object.create(null);\n        }\n\n        currentToken.location.attrs[currentAttr.name] = this.currentAttrLocation;\n    }\n\n    _getOverriddenMethods(mxn, orig) {\n        const methods = {\n            _createStartTagToken() {\n                orig._createStartTagToken.call(this);\n                this.currentToken.location = mxn.ctLoc;\n            },\n\n            _createEndTagToken() {\n                orig._createEndTagToken.call(this);\n                this.currentToken.location = mxn.ctLoc;\n            },\n\n            _createCommentToken() {\n                orig._createCommentToken.call(this);\n                this.currentToken.location = mxn.ctLoc;\n            },\n\n            _createDoctypeToken(initialName) {\n                orig._createDoctypeToken.call(this, initialName);\n                this.currentToken.location = mxn.ctLoc;\n            },\n\n            _createCharacterToken(type, ch) {\n                orig._createCharacterToken.call(this, type, ch);\n                this.currentCharacterToken.location = mxn.ctLoc;\n            },\n\n            _createEOFToken() {\n                orig._createEOFToken.call(this);\n                this.currentToken.location = mxn._getCurrentLocation();\n            },\n\n            _createAttr(attrNameFirstCh) {\n                orig._createAttr.call(this, attrNameFirstCh);\n                mxn.currentAttrLocation = mxn._getCurrentLocation();\n            },\n\n            _leaveAttrName(toState) {\n                orig._leaveAttrName.call(this, toState);\n                mxn._attachCurrentAttrLocationInfo();\n            },\n\n            _leaveAttrValue(toState) {\n                orig._leaveAttrValue.call(this, toState);\n                mxn._attachCurrentAttrLocationInfo();\n            },\n\n            _emitCurrentToken() {\n                const ctLoc = this.currentToken.location;\n\n                //NOTE: if we have pending character token make it's end location equal to the\n                //current token's start location.\n                if (this.currentCharacterToken) {\n                    this.currentCharacterToken.location.endLine = ctLoc.startLine;\n                    this.currentCharacterToken.location.endCol = ctLoc.startCol;\n                    this.currentCharacterToken.location.endOffset = ctLoc.startOffset;\n                }\n\n                if (this.currentToken.type === Tokenizer.EOF_TOKEN) {\n                    ctLoc.endLine = ctLoc.startLine;\n                    ctLoc.endCol = ctLoc.startCol;\n                    ctLoc.endOffset = ctLoc.startOffset;\n                } else {\n                    ctLoc.endLine = mxn.posTracker.line;\n                    ctLoc.endCol = mxn.posTracker.col + 1;\n                    ctLoc.endOffset = mxn.posTracker.offset + 1;\n                }\n\n                orig._emitCurrentToken.call(this);\n            },\n\n            _emitCurrentCharacterToken() {\n                const ctLoc = this.currentCharacterToken && this.currentCharacterToken.location;\n\n                //NOTE: if we have character token and it's location wasn't set in the _emitCurrentToken(),\n                //then set it's location at the current preprocessor position.\n                //We don't need to increment preprocessor position, since character token\n                //emission is always forced by the start of the next character token here.\n                //So, we already have advanced position.\n                if (ctLoc && ctLoc.endOffset === -1) {\n                    ctLoc.endLine = mxn.posTracker.line;\n                    ctLoc.endCol = mxn.posTracker.col;\n                    ctLoc.endOffset = mxn.posTracker.offset;\n                }\n\n                orig._emitCurrentCharacterToken.call(this);\n            }\n        };\n\n        //NOTE: patch initial states for each mode to obtain token start position\n        Object.keys(Tokenizer.MODE).forEach(modeName => {\n            const state = Tokenizer.MODE[modeName];\n\n            methods[state] = function(cp) {\n                mxn.ctLoc = mxn._getCurrentLocation();\n                orig[state].call(this, cp);\n            };\n        });\n\n        return methods;\n    }\n}\n\nmodule.exports = LocationInfoTokenizerMixin;\n",
         "'use strict';\n\nconst Mixin = require('../../utils/mixin');\n\nclass PositionTrackingPreprocessorMixin extends Mixin {\n    constructor(preprocessor) {\n        super(preprocessor);\n\n        this.preprocessor = preprocessor;\n        this.isEol = false;\n        this.lineStartPos = 0;\n        this.droppedBufferSize = 0;\n\n        this.offset = 0;\n        this.col = 0;\n        this.line = 1;\n    }\n\n    _getOverriddenMethods(mxn, orig) {\n        return {\n            advance() {\n                const pos = this.pos + 1;\n                const ch = this.html[pos];\n\n                //NOTE: LF should be in the last column of the line\n                if (mxn.isEol) {\n                    mxn.isEol = false;\n                    mxn.line++;\n                    mxn.lineStartPos = pos;\n                }\n\n                if (ch === '\\n' || (ch === '\\r' && this.html[pos + 1] !== '\\n')) {\n                    mxn.isEol = true;\n                }\n\n                mxn.col = pos - mxn.lineStartPos + 1;\n                mxn.offset = mxn.droppedBufferSize + pos;\n\n                return orig.advance.call(this);\n            },\n\n            retreat() {\n                orig.retreat.call(this);\n\n                mxn.isEol = false;\n                mxn.col = this.pos - mxn.lineStartPos + 1;\n            },\n\n            dropParsedChunk() {\n                const prevPos = this.pos;\n\n                orig.dropParsedChunk.call(this);\n\n                const reduction = prevPos - this.pos;\n\n                mxn.lineStartPos -= reduction;\n                mxn.droppedBufferSize += reduction;\n                mxn.offset = mxn.droppedBufferSize + this.pos;\n            }\n        };\n    }\n}\n\nmodule.exports = PositionTrackingPreprocessorMixin;\n",
         "var superPropBase = require(\"./superPropBase\");\n\nfunction _get(target, property, receiver) {\n  if (typeof Reflect !== \"undefined\" && Reflect.get) {\n    module.exports = _get = Reflect.get;\n  } else {\n    module.exports = _get = function _get(target, property, receiver) {\n      var base = superPropBase(target, property);\n      if (!base) return;\n      var desc = Object.getOwnPropertyDescriptor(base, property);\n\n      if (desc.get) {\n        return desc.get.call(receiver);\n      }\n\n      return desc.value;\n    };\n  }\n\n  return _get(target, property, receiver || target);\n}\n\nmodule.exports = _get;",
         "'use strict';\n\nif (process.env.NODE_ENV === 'production') {\n  module.exports = require('./cjs/react-is.production.min.js');\n} else {\n  module.exports = require('./cjs/react-is.development.js');\n}\n",
-        "var v1 = require('./v1');\nvar v4 = require('./v4');\n\nvar uuid = v4;\nuuid.v1 = v1;\nuuid.v4 = v4;\n\nmodule.exports = uuid;\n",
         "/*!\n * FilePondPluginImageExifOrientation 1.0.11\n * Licensed under MIT, https://opensource.org/licenses/MIT/\n * Please visit https://pqina.nl/filepond/ for details.\n */\n\n/* eslint-disable */\n\n(function(global, factory) {\n  typeof exports === 'object' && typeof module !== 'undefined'\n    ? (module.exports = factory())\n    : typeof define === 'function' && define.amd\n    ? define(factory)\n    : ((global = global || self),\n      (global.FilePondPluginImageExifOrientation = factory()));\n})(this, function() {\n  'use strict';\n\n  // test if file is of type image\n  var isJPEG = function isJPEG(file) {\n    return /^image\\/jpeg/.test(file.type);\n  };\n\n  var Marker = {\n    JPEG: 0xffd8,\n    APP1: 0xffe1,\n    EXIF: 0x45786966,\n    TIFF: 0x4949,\n    Orientation: 0x0112,\n    Unknown: 0xff00\n  };\n\n  var getUint16 = function getUint16(view, offset) {\n    var little =\n      arguments.length > 2 && arguments[2] !== undefined ? arguments[2] : false;\n    return view.getUint16(offset, little);\n  };\n  var getUint32 = function getUint32(view, offset) {\n    var little =\n      arguments.length > 2 && arguments[2] !== undefined ? arguments[2] : false;\n    return view.getUint32(offset, little);\n  };\n\n  var getImageOrientation = function getImageOrientation(file) {\n    return new Promise(function(resolve, reject) {\n      var reader = new FileReader();\n      reader.onload = function(e) {\n        var view = new DataView(e.target.result);\n\n        // Every JPEG file starts from binary value '0xFFD8'\n        if (getUint16(view, 0) !== Marker.JPEG) {\n          // This aint no JPEG\n          resolve(-1);\n          return;\n        }\n\n        var length = view.byteLength;\n        var offset = 2;\n\n        while (offset < length) {\n          var marker = getUint16(view, offset);\n          offset += 2;\n\n          // There's our APP1 Marker\n          if (marker === Marker.APP1) {\n            if (getUint32(view, (offset += 2)) !== Marker.EXIF) {\n              // no EXIF info defined\n              break;\n            }\n\n            // Get TIFF Header\n            var little = getUint16(view, (offset += 6)) === Marker.TIFF;\n            offset += getUint32(view, offset + 4, little);\n\n            var tags = getUint16(view, offset, little);\n            offset += 2;\n\n            for (var i = 0; i < tags; i++) {\n              // found the orientation tag\n              if (\n                getUint16(view, offset + i * 12, little) === Marker.Orientation\n              ) {\n                resolve(getUint16(view, offset + i * 12 + 8, little));\n\n                return;\n              }\n            }\n          } else if ((marker & Marker.Unknown) !== Marker.Unknown) {\n            // Invalid\n            break;\n          } else {\n            offset += getUint16(view, offset);\n          }\n        }\n\n        // Nothing found\n        resolve(-1);\n      };\n\n      // we don't need to read the entire file to get the orientation\n      reader.readAsArrayBuffer(file.slice(0, 64 * 1024));\n    });\n  };\n\n  var IS_BROWSER = (function() {\n    return (\n      typeof window !== 'undefined' && typeof window.document !== 'undefined'\n    );\n  })();\n  var isBrowser = function isBrowser() {\n    return IS_BROWSER;\n  };\n\n  // 2x1 pixel image 90CW rotated with orientation header\n  var testSrc =\n    'data:image/jpg;base64,/9j/4AAQSkZJRgABAQEASABIAAD/4QA6RXhpZgAATU0AKgAAAAgAAwESAAMAAAABAAYAAAEoAAMAAAABAAIAAAITAAMAAAABAAEAAAAAAAD/2wBDAP//////////////////////////////////////////////////////////////////////////////////////wAALCAABAAIBASIA/8QAJgABAAAAAAAAAAAAAAAAAAAAAxABAAAAAAAAAAAAAAAAAAAAAP/aAAgBAQAAPwBH/9k=';\n\n  // should correct orientation if is presented in landscape, in which case the browser doesn't autocorrect\n  var shouldCorrect = undefined;\n  var testImage = isBrowser() ? new Image() : {};\n  testImage.onload = function() {\n    return (shouldCorrect = testImage.naturalWidth > testImage.naturalHeight);\n  };\n  testImage.src = testSrc;\n\n  var shouldCorrectImageExifOrientation = function shouldCorrectImageExifOrientation() {\n    return shouldCorrect;\n  };\n\n  /**\n   * Read Image Orientation Plugin\n   */\n  var plugin = function plugin(_ref) {\n    var addFilter = _ref.addFilter,\n      utils = _ref.utils;\n    var Type = utils.Type,\n      isFile = utils.isFile;\n\n    // subscribe to file load and append required info\n    addFilter('DID_LOAD_ITEM', function(item, _ref2) {\n      var query = _ref2.query;\n      return new Promise(function(resolve, reject) {\n        // get file reference\n        var file = item.file;\n\n        // if this is not a jpeg image we are not interested\n        if (\n          !isFile(file) ||\n          !isJPEG(file) ||\n          !query('GET_ALLOW_IMAGE_EXIF_ORIENTATION') ||\n          !shouldCorrectImageExifOrientation()\n        ) {\n          // continue with the unaltered dataset\n          return resolve(item);\n        }\n\n        // get orientation from exif data\n        getImageOrientation(file).then(function(orientation) {\n          item.setMetadata('exif', { orientation: orientation });\n          resolve(item);\n        });\n      });\n    });\n\n    // Expose plugin options\n    return {\n      options: {\n        // Enable or disable image orientation reading\n        allowImageExifOrientation: [true, Type.BOOLEAN]\n      }\n    };\n  };\n\n  // fire pluginloaded event if running in browser, this allows registering the plugin when using async script tags\n  var isBrowser$1 =\n    typeof window !== 'undefined' && typeof window.document !== 'undefined';\n  if (isBrowser$1) {\n    document.dispatchEvent(\n      new CustomEvent('FilePond:pluginloaded', { detail: plugin })\n    );\n  }\n\n  return plugin;\n});\n",
         "/*!\n * FilePondPluginImagePreview 4.6.10\n * Licensed under MIT, https://opensource.org/licenses/MIT/\n * Please visit https://pqina.nl/filepond/ for details.\n */\n\n/* eslint-disable */\n\n(function(global, factory) {\n  typeof exports === 'object' && typeof module !== 'undefined'\n    ? (module.exports = factory())\n    : typeof define === 'function' && define.amd\n    ? define(factory)\n    : ((global = global || self),\n      (global.FilePondPluginImagePreview = factory()));\n})(this, function() {\n  'use strict';\n\n  // test if file is of type image and can be viewed in canvas\n  var isPreviewableImage = function isPreviewableImage(file) {\n    return /^image/.test(file.type);\n  };\n\n  function _typeof(obj) {\n    if (typeof Symbol === 'function' && typeof Symbol.iterator === 'symbol') {\n      _typeof = function(obj) {\n        return typeof obj;\n      };\n    } else {\n      _typeof = function(obj) {\n        return obj &&\n          typeof Symbol === 'function' &&\n          obj.constructor === Symbol &&\n          obj !== Symbol.prototype\n          ? 'symbol'\n          : typeof obj;\n      };\n    }\n\n    return _typeof(obj);\n  }\n\n  var REACT_ELEMENT_TYPE;\n\n  function _jsx(type, props, key, children) {\n    if (!REACT_ELEMENT_TYPE) {\n      REACT_ELEMENT_TYPE =\n        (typeof Symbol === 'function' &&\n          Symbol.for &&\n          Symbol.for('react.element')) ||\n        0xeac7;\n    }\n\n    var defaultProps = type && type.defaultProps;\n    var childrenLength = arguments.length - 3;\n\n    if (!props && childrenLength !== 0) {\n      props = {\n        children: void 0\n      };\n    }\n\n    if (props && defaultProps) {\n      for (var propName in defaultProps) {\n        if (props[propName] === void 0) {\n          props[propName] = defaultProps[propName];\n        }\n      }\n    } else if (!props) {\n      props = defaultProps || {};\n    }\n\n    if (childrenLength === 1) {\n      props.children = children;\n    } else if (childrenLength > 1) {\n      var childArray = new Array(childrenLength);\n\n      for (var i = 0; i < childrenLength; i++) {\n        childArray[i] = arguments[i + 3];\n      }\n\n      props.children = childArray;\n    }\n\n    return {\n      $$typeof: REACT_ELEMENT_TYPE,\n      type: type,\n      key: key === undefined ? null : '' + key,\n      ref: null,\n      props: props,\n      _owner: null\n    };\n  }\n\n  function _asyncIterator(iterable) {\n    var method;\n\n    if (typeof Symbol === 'function') {\n      if (Symbol.asyncIterator) {\n        method = iterable[Symbol.asyncIterator];\n        if (method != null) return method.call(iterable);\n      }\n\n      if (Symbol.iterator) {\n        method = iterable[Symbol.iterator];\n        if (method != null) return method.call(iterable);\n      }\n    }\n\n    throw new TypeError('Object is not async iterable');\n  }\n\n  function _AwaitValue(value) {\n    this.wrapped = value;\n  }\n\n  function _AsyncGenerator(gen) {\n    var front, back;\n\n    function send(key, arg) {\n      return new Promise(function(resolve, reject) {\n        var request = {\n          key: key,\n          arg: arg,\n          resolve: resolve,\n          reject: reject,\n          next: null\n        };\n\n        if (back) {\n          back = back.next = request;\n        } else {\n          front = back = request;\n          resume(key, arg);\n        }\n      });\n    }\n\n    function resume(key, arg) {\n      try {\n        var result = gen[key](arg);\n        var value = result.value;\n        var wrappedAwait = value instanceof _AwaitValue;\n        Promise.resolve(wrappedAwait ? value.wrapped : value).then(\n          function(arg) {\n            if (wrappedAwait) {\n              resume('next', arg);\n              return;\n            }\n\n            settle(result.done ? 'return' : 'normal', arg);\n          },\n          function(err) {\n            resume('throw', err);\n          }\n        );\n      } catch (err) {\n        settle('throw', err);\n      }\n    }\n\n    function settle(type, value) {\n      switch (type) {\n        case 'return':\n          front.resolve({\n            value: value,\n            done: true\n          });\n          break;\n\n        case 'throw':\n          front.reject(value);\n          break;\n\n        default:\n          front.resolve({\n            value: value,\n            done: false\n          });\n          break;\n      }\n\n      front = front.next;\n\n      if (front) {\n        resume(front.key, front.arg);\n      } else {\n        back = null;\n      }\n    }\n\n    this._invoke = send;\n\n    if (typeof gen.return !== 'function') {\n      this.return = undefined;\n    }\n  }\n\n  if (typeof Symbol === 'function' && Symbol.asyncIterator) {\n    _AsyncGenerator.prototype[Symbol.asyncIterator] = function() {\n      return this;\n    };\n  }\n\n  _AsyncGenerator.prototype.next = function(arg) {\n    return this._invoke('next', arg);\n  };\n\n  _AsyncGenerator.prototype.throw = function(arg) {\n    return this._invoke('throw', arg);\n  };\n\n  _AsyncGenerator.prototype.return = function(arg) {\n    return this._invoke('return', arg);\n  };\n\n  function _wrapAsyncGenerator(fn) {\n    return function() {\n      return new _AsyncGenerator(fn.apply(this, arguments));\n    };\n  }\n\n  function _awaitAsyncGenerator(value) {\n    return new _AwaitValue(value);\n  }\n\n  function _asyncGeneratorDelegate(inner, awaitWrap) {\n    var iter = {},\n      waiting = false;\n\n    function pump(key, value) {\n      waiting = true;\n      value = new Promise(function(resolve) {\n        resolve(inner[key](value));\n      });\n      return {\n        done: false,\n        value: awaitWrap(value)\n      };\n    }\n\n    if (typeof Symbol === 'function' && Symbol.iterator) {\n      iter[Symbol.iterator] = function() {\n        return this;\n      };\n    }\n\n    iter.next = function(value) {\n      if (waiting) {\n        waiting = false;\n        return value;\n      }\n\n      return pump('next', value);\n    };\n\n    if (typeof inner.throw === 'function') {\n      iter.throw = function(value) {\n        if (waiting) {\n          waiting = false;\n          throw value;\n        }\n\n        return pump('throw', value);\n      };\n    }\n\n    if (typeof inner.return === 'function') {\n      iter.return = function(value) {\n        return pump('return', value);\n      };\n    }\n\n    return iter;\n  }\n\n  function asyncGeneratorStep(gen, resolve, reject, _next, _throw, key, arg) {\n    try {\n      var info = gen[key](arg);\n      var value = info.value;\n    } catch (error) {\n      reject(error);\n      return;\n    }\n\n    if (info.done) {\n      resolve(value);\n    } else {\n      Promise.resolve(value).then(_next, _throw);\n    }\n  }\n\n  function _asyncToGenerator(fn) {\n    return function() {\n      var self = this,\n        args = arguments;\n      return new Promise(function(resolve, reject) {\n        var gen = fn.apply(self, args);\n\n        function _next(value) {\n          asyncGeneratorStep(\n            gen,\n            resolve,\n            reject,\n            _next,\n            _throw,\n            'next',\n            value\n          );\n        }\n\n        function _throw(err) {\n          asyncGeneratorStep(gen, resolve, reject, _next, _throw, 'throw', err);\n        }\n\n        _next(undefined);\n      });\n    };\n  }\n\n  function _classCallCheck(instance, Constructor) {\n    if (!(instance instanceof Constructor)) {\n      throw new TypeError('Cannot call a class as a function');\n    }\n  }\n\n  function _defineProperties(target, props) {\n    for (var i = 0; i < props.length; i++) {\n      var descriptor = props[i];\n      descriptor.enumerable = descriptor.enumerable || false;\n      descriptor.configurable = true;\n      if ('value' in descriptor) descriptor.writable = true;\n      Object.defineProperty(target, descriptor.key, descriptor);\n    }\n  }\n\n  function _createClass(Constructor, protoProps, staticProps) {\n    if (protoProps) _defineProperties(Constructor.prototype, protoProps);\n    if (staticProps) _defineProperties(Constructor, staticProps);\n    return Constructor;\n  }\n\n  function _defineEnumerableProperties(obj, descs) {\n    for (var key in descs) {\n      var desc = descs[key];\n      desc.configurable = desc.enumerable = true;\n      if ('value' in desc) desc.writable = true;\n      Object.defineProperty(obj, key, desc);\n    }\n\n    if (Object.getOwnPropertySymbols) {\n      var objectSymbols = Object.getOwnPropertySymbols(descs);\n\n      for (var i = 0; i < objectSymbols.length; i++) {\n        var sym = objectSymbols[i];\n        var desc = descs[sym];\n        desc.configurable = desc.enumerable = true;\n        if ('value' in desc) desc.writable = true;\n        Object.defineProperty(obj, sym, desc);\n      }\n    }\n\n    return obj;\n  }\n\n  function _defaults(obj, defaults) {\n    var keys = Object.getOwnPropertyNames(defaults);\n\n    for (var i = 0; i < keys.length; i++) {\n      var key = keys[i];\n      var value = Object.getOwnPropertyDescriptor(defaults, key);\n\n      if (value && value.configurable && obj[key] === undefined) {\n        Object.defineProperty(obj, key, value);\n      }\n    }\n\n    return obj;\n  }\n\n  function _defineProperty(obj, key, value) {\n    if (key in obj) {\n      Object.defineProperty(obj, key, {\n        value: value,\n        enumerable: true,\n        configurable: true,\n        writable: true\n      });\n    } else {\n      obj[key] = value;\n    }\n\n    return obj;\n  }\n\n  function _extends() {\n    _extends =\n      Object.assign ||\n      function(target) {\n        for (var i = 1; i < arguments.length; i++) {\n          var source = arguments[i];\n\n          for (var key in source) {\n            if (Object.prototype.hasOwnProperty.call(source, key)) {\n              target[key] = source[key];\n            }\n          }\n        }\n\n        return target;\n      };\n\n    return _extends.apply(this, arguments);\n  }\n\n  function _objectSpread(target) {\n    for (var i = 1; i < arguments.length; i++) {\n      var source = arguments[i] != null ? arguments[i] : {};\n      var ownKeys = Object.keys(source);\n\n      if (typeof Object.getOwnPropertySymbols === 'function') {\n        ownKeys = ownKeys.concat(\n          Object.getOwnPropertySymbols(source).filter(function(sym) {\n            return Object.getOwnPropertyDescriptor(source, sym).enumerable;\n          })\n        );\n      }\n\n      ownKeys.forEach(function(key) {\n        _defineProperty(target, key, source[key]);\n      });\n    }\n\n    return target;\n  }\n\n  function _inherits(subClass, superClass) {\n    if (typeof superClass !== 'function' && superClass !== null) {\n      throw new TypeError('Super expression must either be null or a function');\n    }\n\n    subClass.prototype = Object.create(superClass && superClass.prototype, {\n      constructor: {\n        value: subClass,\n        writable: true,\n        configurable: true\n      }\n    });\n    if (superClass) _setPrototypeOf(subClass, superClass);\n  }\n\n  function _inheritsLoose(subClass, superClass) {\n    subClass.prototype = Object.create(superClass.prototype);\n    subClass.prototype.constructor = subClass;\n    subClass.__proto__ = superClass;\n  }\n\n  function _getPrototypeOf(o) {\n    _getPrototypeOf = Object.setPrototypeOf\n      ? Object.getPrototypeOf\n      : function _getPrototypeOf(o) {\n          return o.__proto__ || Object.getPrototypeOf(o);\n        };\n    return _getPrototypeOf(o);\n  }\n\n  function _setPrototypeOf(o, p) {\n    _setPrototypeOf =\n      Object.setPrototypeOf ||\n      function _setPrototypeOf(o, p) {\n        o.__proto__ = p;\n        return o;\n      };\n\n    return _setPrototypeOf(o, p);\n  }\n\n  function isNativeReflectConstruct() {\n    if (typeof Reflect === 'undefined' || !Reflect.construct) return false;\n    if (Reflect.construct.sham) return false;\n    if (typeof Proxy === 'function') return true;\n\n    try {\n      Date.prototype.toString.call(Reflect.construct(Date, [], function() {}));\n      return true;\n    } catch (e) {\n      return false;\n    }\n  }\n\n  function _construct(Parent, args, Class) {\n    if (isNativeReflectConstruct()) {\n      _construct = Reflect.construct;\n    } else {\n      _construct = function _construct(Parent, args, Class) {\n        var a = [null];\n        a.push.apply(a, args);\n        var Constructor = Function.bind.apply(Parent, a);\n        var instance = new Constructor();\n        if (Class) _setPrototypeOf(instance, Class.prototype);\n        return instance;\n      };\n    }\n\n    return _construct.apply(null, arguments);\n  }\n\n  function _isNativeFunction(fn) {\n    return Function.toString.call(fn).indexOf('[native code]') !== -1;\n  }\n\n  function _wrapNativeSuper(Class) {\n    var _cache = typeof Map === 'function' ? new Map() : undefined;\n\n    _wrapNativeSuper = function _wrapNativeSuper(Class) {\n      if (Class === null || !_isNativeFunction(Class)) return Class;\n\n      if (typeof Class !== 'function') {\n        throw new TypeError(\n          'Super expression must either be null or a function'\n        );\n      }\n\n      if (typeof _cache !== 'undefined') {\n        if (_cache.has(Class)) return _cache.get(Class);\n\n        _cache.set(Class, Wrapper);\n      }\n\n      function Wrapper() {\n        return _construct(Class, arguments, _getPrototypeOf(this).constructor);\n      }\n\n      Wrapper.prototype = Object.create(Class.prototype, {\n        constructor: {\n          value: Wrapper,\n          enumerable: false,\n          writable: true,\n          configurable: true\n        }\n      });\n      return _setPrototypeOf(Wrapper, Class);\n    };\n\n    return _wrapNativeSuper(Class);\n  }\n\n  function _instanceof(left, right) {\n    if (\n      right != null &&\n      typeof Symbol !== 'undefined' &&\n      right[Symbol.hasInstance]\n    ) {\n      return right[Symbol.hasInstance](left);\n    } else {\n      return left instanceof right;\n    }\n  }\n\n  function _interopRequireDefault(obj) {\n    return obj && obj.__esModule\n      ? obj\n      : {\n          default: obj\n        };\n  }\n\n  function _interopRequireWildcard(obj) {\n    if (obj && obj.__esModule) {\n      return obj;\n    } else {\n      var newObj = {};\n\n      if (obj != null) {\n        for (var key in obj) {\n          if (Object.prototype.hasOwnProperty.call(obj, key)) {\n            var desc =\n              Object.defineProperty && Object.getOwnPropertyDescriptor\n                ? Object.getOwnPropertyDescriptor(obj, key)\n                : {};\n\n            if (desc.get || desc.set) {\n              Object.defineProperty(newObj, key, desc);\n            } else {\n              newObj[key] = obj[key];\n            }\n          }\n        }\n      }\n\n      newObj.default = obj;\n      return newObj;\n    }\n  }\n\n  function _newArrowCheck(innerThis, boundThis) {\n    if (innerThis !== boundThis) {\n      throw new TypeError('Cannot instantiate an arrow function');\n    }\n  }\n\n  function _objectDestructuringEmpty(obj) {\n    if (obj == null) throw new TypeError('Cannot destructure undefined');\n  }\n\n  function _objectWithoutPropertiesLoose(source, excluded) {\n    if (source == null) return {};\n    var target = {};\n    var sourceKeys = Object.keys(source);\n    var key, i;\n\n    for (i = 0; i < sourceKeys.length; i++) {\n      key = sourceKeys[i];\n      if (excluded.indexOf(key) >= 0) continue;\n      target[key] = source[key];\n    }\n\n    return target;\n  }\n\n  function _objectWithoutProperties(source, excluded) {\n    if (source == null) return {};\n\n    var target = _objectWithoutPropertiesLoose(source, excluded);\n\n    var key, i;\n\n    if (Object.getOwnPropertySymbols) {\n      var sourceSymbolKeys = Object.getOwnPropertySymbols(source);\n\n      for (i = 0; i < sourceSymbolKeys.length; i++) {\n        key = sourceSymbolKeys[i];\n        if (excluded.indexOf(key) >= 0) continue;\n        if (!Object.prototype.propertyIsEnumerable.call(source, key)) continue;\n        target[key] = source[key];\n      }\n    }\n\n    return target;\n  }\n\n  function _assertThisInitialized(self) {\n    if (self === void 0) {\n      throw new ReferenceError(\n        \"this hasn't been initialised - super() hasn't been called\"\n      );\n    }\n\n    return self;\n  }\n\n  function _possibleConstructorReturn(self, call) {\n    if (call && (typeof call === 'object' || typeof call === 'function')) {\n      return call;\n    }\n\n    return _assertThisInitialized(self);\n  }\n\n  function _superPropBase(object, property) {\n    while (!Object.prototype.hasOwnProperty.call(object, property)) {\n      object = _getPrototypeOf(object);\n      if (object === null) break;\n    }\n\n    return object;\n  }\n\n  function _get(target, property, receiver) {\n    if (typeof Reflect !== 'undefined' && Reflect.get) {\n      _get = Reflect.get;\n    } else {\n      _get = function _get(target, property, receiver) {\n        var base = _superPropBase(target, property);\n\n        if (!base) return;\n        var desc = Object.getOwnPropertyDescriptor(base, property);\n\n        if (desc.get) {\n          return desc.get.call(receiver);\n        }\n\n        return desc.value;\n      };\n    }\n\n    return _get(target, property, receiver || target);\n  }\n\n  function set(target, property, value, receiver) {\n    if (typeof Reflect !== 'undefined' && Reflect.set) {\n      set = Reflect.set;\n    } else {\n      set = function set(target, property, value, receiver) {\n        var base = _superPropBase(target, property);\n\n        var desc;\n\n        if (base) {\n          desc = Object.getOwnPropertyDescriptor(base, property);\n\n          if (desc.set) {\n            desc.set.call(receiver, value);\n            return true;\n          } else if (!desc.writable) {\n            return false;\n          }\n        }\n\n        desc = Object.getOwnPropertyDescriptor(receiver, property);\n\n        if (desc) {\n          if (!desc.writable) {\n            return false;\n          }\n\n          desc.value = value;\n          Object.defineProperty(receiver, property, desc);\n        } else {\n          _defineProperty(receiver, property, value);\n        }\n\n        return true;\n      };\n    }\n\n    return set(target, property, value, receiver);\n  }\n\n  function _set(target, property, value, receiver, isStrict) {\n    var s = set(target, property, value, receiver || target);\n\n    if (!s && isStrict) {\n      throw new Error('failed to set property');\n    }\n\n    return value;\n  }\n\n  function _taggedTemplateLiteral(strings, raw) {\n    if (!raw) {\n      raw = strings.slice(0);\n    }\n\n    return Object.freeze(\n      Object.defineProperties(strings, {\n        raw: {\n          value: Object.freeze(raw)\n        }\n      })\n    );\n  }\n\n  function _taggedTemplateLiteralLoose(strings, raw) {\n    if (!raw) {\n      raw = strings.slice(0);\n    }\n\n    strings.raw = raw;\n    return strings;\n  }\n\n  function _temporalRef(val, name) {\n    if (val === _temporalUndefined) {\n      throw new ReferenceError(name + ' is not defined - temporal dead zone');\n    } else {\n      return val;\n    }\n  }\n\n  function _readOnlyError(name) {\n    throw new Error('\"' + name + '\" is read-only');\n  }\n\n  function _classNameTDZError(name) {\n    throw new Error(\n      'Class \"' + name + '\" cannot be referenced in computed property keys.'\n    );\n  }\n\n  var _temporalUndefined = {};\n\n  function _slicedToArray(arr, i) {\n    return (\n      _arrayWithHoles(arr) ||\n      _iterableToArrayLimit(arr, i) ||\n      _nonIterableRest()\n    );\n  }\n\n  function _slicedToArrayLoose(arr, i) {\n    return (\n      _arrayWithHoles(arr) ||\n      _iterableToArrayLimitLoose(arr, i) ||\n      _nonIterableRest()\n    );\n  }\n\n  function _toArray(arr) {\n    return _arrayWithHoles(arr) || _iterableToArray(arr) || _nonIterableRest();\n  }\n\n  function _toConsumableArray(arr) {\n    return (\n      _arrayWithoutHoles(arr) || _iterableToArray(arr) || _nonIterableSpread()\n    );\n  }\n\n  function _arrayWithoutHoles(arr) {\n    if (Array.isArray(arr)) {\n      for (var i = 0, arr2 = new Array(arr.length); i < arr.length; i++)\n        arr2[i] = arr[i];\n\n      return arr2;\n    }\n  }\n\n  function _arrayWithHoles(arr) {\n    if (Array.isArray(arr)) return arr;\n  }\n\n  function _iterableToArray(iter) {\n    if (\n      Symbol.iterator in Object(iter) ||\n      Object.prototype.toString.call(iter) === '[object Arguments]'\n    )\n      return Array.from(iter);\n  }\n\n  function _iterableToArrayLimit(arr, i) {\n    var _arr = [];\n    var _n = true;\n    var _d = false;\n    var _e = undefined;\n\n    try {\n      for (\n        var _i = arr[Symbol.iterator](), _s;\n        !(_n = (_s = _i.next()).done);\n        _n = true\n      ) {\n        _arr.push(_s.value);\n\n        if (i && _arr.length === i) break;\n      }\n    } catch (err) {\n      _d = true;\n      _e = err;\n    } finally {\n      try {\n        if (!_n && _i['return'] != null) _i['return']();\n      } finally {\n        if (_d) throw _e;\n      }\n    }\n\n    return _arr;\n  }\n\n  function _iterableToArrayLimitLoose(arr, i) {\n    var _arr = [];\n\n    for (\n      var _iterator = arr[Symbol.iterator](), _step;\n      !(_step = _iterator.next()).done;\n\n    ) {\n      _arr.push(_step.value);\n\n      if (i && _arr.length === i) break;\n    }\n\n    return _arr;\n  }\n\n  function _nonIterableSpread() {\n    throw new TypeError('Invalid attempt to spread non-iterable instance');\n  }\n\n  function _nonIterableRest() {\n    throw new TypeError('Invalid attempt to destructure non-iterable instance');\n  }\n\n  function _skipFirstGeneratorNext(fn) {\n    return function() {\n      var it = fn.apply(this, arguments);\n      it.next();\n      return it;\n    };\n  }\n\n  function _toPrimitive(input, hint) {\n    if (typeof input !== 'object' || input === null) return input;\n    var prim = input[Symbol.toPrimitive];\n\n    if (prim !== undefined) {\n      var res = prim.call(input, hint || 'default');\n      if (typeof res !== 'object') return res;\n      throw new TypeError('@@toPrimitive must return a primitive value.');\n    }\n\n    return (hint === 'string' ? String : Number)(input);\n  }\n\n  function _toPropertyKey(arg) {\n    var key = _toPrimitive(arg, 'string');\n\n    return typeof key === 'symbol' ? key : String(key);\n  }\n\n  function _initializerWarningHelper(descriptor, context) {\n    throw new Error(\n      'Decorating class property failed. Please ensure that ' +\n        'proposal-class-properties is enabled and set to use loose mode. ' +\n        'To use proposal-class-properties in spec mode with decorators, wait for ' +\n        'the next major version of decorators in stage 2.'\n    );\n  }\n\n  function _initializerDefineProperty(target, property, descriptor, context) {\n    if (!descriptor) return;\n    Object.defineProperty(target, property, {\n      enumerable: descriptor.enumerable,\n      configurable: descriptor.configurable,\n      writable: descriptor.writable,\n      value: descriptor.initializer\n        ? descriptor.initializer.call(context)\n        : void 0\n    });\n  }\n\n  function _applyDecoratedDescriptor(\n    target,\n    property,\n    decorators,\n    descriptor,\n    context\n  ) {\n    var desc = {};\n    Object.keys(descriptor).forEach(function(key) {\n      desc[key] = descriptor[key];\n    });\n    desc.enumerable = !!desc.enumerable;\n    desc.configurable = !!desc.configurable;\n\n    if ('value' in desc || desc.initializer) {\n      desc.writable = true;\n    }\n\n    desc = decorators\n      .slice()\n      .reverse()\n      .reduce(function(desc, decorator) {\n        return decorator(target, property, desc) || desc;\n      }, desc);\n\n    if (context && desc.initializer !== void 0) {\n      desc.value = desc.initializer ? desc.initializer.call(context) : void 0;\n      desc.initializer = undefined;\n    }\n\n    if (desc.initializer === void 0) {\n      Object.defineProperty(target, property, desc);\n      desc = null;\n    }\n\n    return desc;\n  }\n\n  var id = 0;\n\n  function _classPrivateFieldLooseKey(name) {\n    return '__private_' + id++ + '_' + name;\n  }\n\n  function _classPrivateFieldLooseBase(receiver, privateKey) {\n    if (!Object.prototype.hasOwnProperty.call(receiver, privateKey)) {\n      throw new TypeError('attempted to use private field on non-instance');\n    }\n\n    return receiver;\n  }\n\n  function _classPrivateFieldGet(receiver, privateMap) {\n    if (!privateMap.has(receiver)) {\n      throw new TypeError('attempted to get private field on non-instance');\n    }\n\n    var descriptor = privateMap.get(receiver);\n\n    if (descriptor.get) {\n      return descriptor.get.call(receiver);\n    }\n\n    return descriptor.value;\n  }\n\n  function _classPrivateFieldSet(receiver, privateMap, value) {\n    if (!privateMap.has(receiver)) {\n      throw new TypeError('attempted to set private field on non-instance');\n    }\n\n    var descriptor = privateMap.get(receiver);\n\n    if (descriptor.set) {\n      descriptor.set.call(receiver, value);\n    } else {\n      if (!descriptor.writable) {\n        throw new TypeError('attempted to set read only private field');\n      }\n\n      descriptor.value = value;\n    }\n\n    return value;\n  }\n\n  function _classStaticPrivateFieldSpecGet(\n    receiver,\n    classConstructor,\n    descriptor\n  ) {\n    if (receiver !== classConstructor) {\n      throw new TypeError('Private static access of wrong provenance');\n    }\n\n    return descriptor.value;\n  }\n\n  function _classStaticPrivateFieldSpecSet(\n    receiver,\n    classConstructor,\n    descriptor,\n    value\n  ) {\n    if (receiver !== classConstructor) {\n      throw new TypeError('Private static access of wrong provenance');\n    }\n\n    if (!descriptor.writable) {\n      throw new TypeError('attempted to set read only private field');\n    }\n\n    descriptor.value = value;\n    return value;\n  }\n\n  function _classStaticPrivateMethodGet(receiver, classConstructor, method) {\n    if (receiver !== classConstructor) {\n      throw new TypeError('Private static access of wrong provenance');\n    }\n\n    return method;\n  }\n\n  function _classStaticPrivateMethodSet() {\n    throw new TypeError('attempted to set read only static private field');\n  }\n\n  function _decorate(decorators, factory, superClass, mixins) {\n    var api = _getDecoratorsApi();\n\n    if (mixins) {\n      for (var i = 0; i < mixins.length; i++) {\n        api = mixins[i](api);\n      }\n    }\n\n    var r = factory(function initialize(O) {\n      api.initializeInstanceElements(O, decorated.elements);\n    }, superClass);\n    var decorated = api.decorateClass(\n      _coalesceClassElements(r.d.map(_createElementDescriptor)),\n      decorators\n    );\n    api.initializeClassElements(r.F, decorated.elements);\n    return api.runClassFinishers(r.F, decorated.finishers);\n  }\n\n  function _getDecoratorsApi() {\n    _getDecoratorsApi = function() {\n      return api;\n    };\n\n    var api = {\n      elementsDefinitionOrder: [['method'], ['field']],\n      initializeInstanceElements: function(O, elements) {\n        ['method', 'field'].forEach(function(kind) {\n          elements.forEach(function(element) {\n            if (element.kind === kind && element.placement === 'own') {\n              this.defineClassElement(O, element);\n            }\n          }, this);\n        }, this);\n      },\n      initializeClassElements: function(F, elements) {\n        var proto = F.prototype;\n        ['method', 'field'].forEach(function(kind) {\n          elements.forEach(function(element) {\n            var placement = element.placement;\n\n            if (\n              element.kind === kind &&\n              (placement === 'static' || placement === 'prototype')\n            ) {\n              var receiver = placement === 'static' ? F : proto;\n              this.defineClassElement(receiver, element);\n            }\n          }, this);\n        }, this);\n      },\n      defineClassElement: function(receiver, element) {\n        var descriptor = element.descriptor;\n\n        if (element.kind === 'field') {\n          var initializer = element.initializer;\n          descriptor = {\n            enumerable: descriptor.enumerable,\n            writable: descriptor.writable,\n            configurable: descriptor.configurable,\n            value: initializer === void 0 ? void 0 : initializer.call(receiver)\n          };\n        }\n\n        Object.defineProperty(receiver, element.key, descriptor);\n      },\n      decorateClass: function(elements, decorators) {\n        var newElements = [];\n        var finishers = [];\n        var placements = {\n          static: [],\n          prototype: [],\n          own: []\n        };\n        elements.forEach(function(element) {\n          this.addElementPlacement(element, placements);\n        }, this);\n        elements.forEach(function(element) {\n          if (!_hasDecorators(element)) return newElements.push(element);\n          var elementFinishersExtras = this.decorateElement(\n            element,\n            placements\n          );\n          newElements.push(elementFinishersExtras.element);\n          newElements.push.apply(newElements, elementFinishersExtras.extras);\n          finishers.push.apply(finishers, elementFinishersExtras.finishers);\n        }, this);\n\n        if (!decorators) {\n          return {\n            elements: newElements,\n            finishers: finishers\n          };\n        }\n\n        var result = this.decorateConstructor(newElements, decorators);\n        finishers.push.apply(finishers, result.finishers);\n        result.finishers = finishers;\n        return result;\n      },\n      addElementPlacement: function(element, placements, silent) {\n        var keys = placements[element.placement];\n\n        if (!silent && keys.indexOf(element.key) !== -1) {\n          throw new TypeError('Duplicated element (' + element.key + ')');\n        }\n\n        keys.push(element.key);\n      },\n      decorateElement: function(element, placements) {\n        var extras = [];\n        var finishers = [];\n\n        for (\n          var decorators = element.decorators, i = decorators.length - 1;\n          i >= 0;\n          i--\n        ) {\n          var keys = placements[element.placement];\n          keys.splice(keys.indexOf(element.key), 1);\n          var elementObject = this.fromElementDescriptor(element);\n          var elementFinisherExtras = this.toElementFinisherExtras(\n            (0, decorators[i])(elementObject) || elementObject\n          );\n          element = elementFinisherExtras.element;\n          this.addElementPlacement(element, placements);\n\n          if (elementFinisherExtras.finisher) {\n            finishers.push(elementFinisherExtras.finisher);\n          }\n\n          var newExtras = elementFinisherExtras.extras;\n\n          if (newExtras) {\n            for (var j = 0; j < newExtras.length; j++) {\n              this.addElementPlacement(newExtras[j], placements);\n            }\n\n            extras.push.apply(extras, newExtras);\n          }\n        }\n\n        return {\n          element: element,\n          finishers: finishers,\n          extras: extras\n        };\n      },\n      decorateConstructor: function(elements, decorators) {\n        var finishers = [];\n\n        for (var i = decorators.length - 1; i >= 0; i--) {\n          var obj = this.fromClassDescriptor(elements);\n          var elementsAndFinisher = this.toClassDescriptor(\n            (0, decorators[i])(obj) || obj\n          );\n\n          if (elementsAndFinisher.finisher !== undefined) {\n            finishers.push(elementsAndFinisher.finisher);\n          }\n\n          if (elementsAndFinisher.elements !== undefined) {\n            elements = elementsAndFinisher.elements;\n\n            for (var j = 0; j < elements.length - 1; j++) {\n              for (var k = j + 1; k < elements.length; k++) {\n                if (\n                  elements[j].key === elements[k].key &&\n                  elements[j].placement === elements[k].placement\n                ) {\n                  throw new TypeError(\n                    'Duplicated element (' + elements[j].key + ')'\n                  );\n                }\n              }\n            }\n          }\n        }\n\n        return {\n          elements: elements,\n          finishers: finishers\n        };\n      },\n      fromElementDescriptor: function(element) {\n        var obj = {\n          kind: element.kind,\n          key: element.key,\n          placement: element.placement,\n          descriptor: element.descriptor\n        };\n        var desc = {\n          value: 'Descriptor',\n          configurable: true\n        };\n        Object.defineProperty(obj, Symbol.toStringTag, desc);\n        if (element.kind === 'field') obj.initializer = element.initializer;\n        return obj;\n      },\n      toElementDescriptors: function(elementObjects) {\n        if (elementObjects === undefined) return;\n        return _toArray(elementObjects).map(function(elementObject) {\n          var element = this.toElementDescriptor(elementObject);\n          this.disallowProperty(\n            elementObject,\n            'finisher',\n            'An element descriptor'\n          );\n          this.disallowProperty(\n            elementObject,\n            'extras',\n            'An element descriptor'\n          );\n          return element;\n        }, this);\n      },\n      toElementDescriptor: function(elementObject) {\n        var kind = String(elementObject.kind);\n\n        if (kind !== 'method' && kind !== 'field') {\n          throw new TypeError(\n            'An element descriptor\\'s .kind property must be either \"method\" or' +\n              ' \"field\", but a decorator created an element descriptor with' +\n              ' .kind \"' +\n              kind +\n              '\"'\n          );\n        }\n\n        var key = _toPropertyKey(elementObject.key);\n\n        var placement = String(elementObject.placement);\n\n        if (\n          placement !== 'static' &&\n          placement !== 'prototype' &&\n          placement !== 'own'\n        ) {\n          throw new TypeError(\n            'An element descriptor\\'s .placement property must be one of \"static\",' +\n              ' \"prototype\" or \"own\", but a decorator created an element descriptor' +\n              ' with .placement \"' +\n              placement +\n              '\"'\n          );\n        }\n\n        var descriptor = elementObject.descriptor;\n        this.disallowProperty(\n          elementObject,\n          'elements',\n          'An element descriptor'\n        );\n        var element = {\n          kind: kind,\n          key: key,\n          placement: placement,\n          descriptor: Object.assign({}, descriptor)\n        };\n\n        if (kind !== 'field') {\n          this.disallowProperty(\n            elementObject,\n            'initializer',\n            'A method descriptor'\n          );\n        } else {\n          this.disallowProperty(\n            descriptor,\n            'get',\n            'The property descriptor of a field descriptor'\n          );\n          this.disallowProperty(\n            descriptor,\n            'set',\n            'The property descriptor of a field descriptor'\n          );\n          this.disallowProperty(\n            descriptor,\n            'value',\n            'The property descriptor of a field descriptor'\n          );\n          element.initializer = elementObject.initializer;\n        }\n\n        return element;\n      },\n      toElementFinisherExtras: function(elementObject) {\n        var element = this.toElementDescriptor(elementObject);\n\n        var finisher = _optionalCallableProperty(elementObject, 'finisher');\n\n        var extras = this.toElementDescriptors(elementObject.extras);\n        return {\n          element: element,\n          finisher: finisher,\n          extras: extras\n        };\n      },\n      fromClassDescriptor: function(elements) {\n        var obj = {\n          kind: 'class',\n          elements: elements.map(this.fromElementDescriptor, this)\n        };\n        var desc = {\n          value: 'Descriptor',\n          configurable: true\n        };\n        Object.defineProperty(obj, Symbol.toStringTag, desc);\n        return obj;\n      },\n      toClassDescriptor: function(obj) {\n        var kind = String(obj.kind);\n\n        if (kind !== 'class') {\n          throw new TypeError(\n            'A class descriptor\\'s .kind property must be \"class\", but a decorator' +\n              ' created a class descriptor with .kind \"' +\n              kind +\n              '\"'\n          );\n        }\n\n        this.disallowProperty(obj, 'key', 'A class descriptor');\n        this.disallowProperty(obj, 'placement', 'A class descriptor');\n        this.disallowProperty(obj, 'descriptor', 'A class descriptor');\n        this.disallowProperty(obj, 'initializer', 'A class descriptor');\n        this.disallowProperty(obj, 'extras', 'A class descriptor');\n\n        var finisher = _optionalCallableProperty(obj, 'finisher');\n\n        var elements = this.toElementDescriptors(obj.elements);\n        return {\n          elements: elements,\n          finisher: finisher\n        };\n      },\n      runClassFinishers: function(constructor, finishers) {\n        for (var i = 0; i < finishers.length; i++) {\n          var newConstructor = (0, finishers[i])(constructor);\n\n          if (newConstructor !== undefined) {\n            if (typeof newConstructor !== 'function') {\n              throw new TypeError('Finishers must return a constructor.');\n            }\n\n            constructor = newConstructor;\n          }\n        }\n\n        return constructor;\n      },\n      disallowProperty: function(obj, name, objectType) {\n        if (obj[name] !== undefined) {\n          throw new TypeError(\n            objectType + \" can't have a .\" + name + ' property.'\n          );\n        }\n      }\n    };\n    return api;\n  }\n\n  function _createElementDescriptor(def) {\n    var key = _toPropertyKey(def.key);\n\n    var descriptor;\n\n    if (def.kind === 'method') {\n      descriptor = {\n        value: def.value,\n        writable: true,\n        configurable: true,\n        enumerable: false\n      };\n    } else if (def.kind === 'get') {\n      descriptor = {\n        get: def.value,\n        configurable: true,\n        enumerable: false\n      };\n    } else if (def.kind === 'set') {\n      descriptor = {\n        set: def.value,\n        configurable: true,\n        enumerable: false\n      };\n    } else if (def.kind === 'field') {\n      descriptor = {\n        configurable: true,\n        writable: true,\n        enumerable: true\n      };\n    }\n\n    var element = {\n      kind: def.kind === 'field' ? 'field' : 'method',\n      key: key,\n      placement: def.static\n        ? 'static'\n        : def.kind === 'field'\n        ? 'own'\n        : 'prototype',\n      descriptor: descriptor\n    };\n    if (def.decorators) element.decorators = def.decorators;\n    if (def.kind === 'field') element.initializer = def.value;\n    return element;\n  }\n\n  function _coalesceGetterSetter(element, other) {\n    if (element.descriptor.get !== undefined) {\n      other.descriptor.get = element.descriptor.get;\n    } else {\n      other.descriptor.set = element.descriptor.set;\n    }\n  }\n\n  function _coalesceClassElements(elements) {\n    var newElements = [];\n\n    var isSameElement = function(other) {\n      return (\n        other.kind === 'method' &&\n        other.key === element.key &&\n        other.placement === element.placement\n      );\n    };\n\n    for (var i = 0; i < elements.length; i++) {\n      var element = elements[i];\n      var other;\n\n      if (\n        element.kind === 'method' &&\n        (other = newElements.find(isSameElement))\n      ) {\n        if (\n          _isDataDescriptor(element.descriptor) ||\n          _isDataDescriptor(other.descriptor)\n        ) {\n          if (_hasDecorators(element) || _hasDecorators(other)) {\n            throw new ReferenceError(\n              'Duplicated methods (' + element.key + \") can't be decorated.\"\n            );\n          }\n\n          other.descriptor = element.descriptor;\n        } else {\n          if (_hasDecorators(element)) {\n            if (_hasDecorators(other)) {\n              throw new ReferenceError(\n                \"Decorators can't be placed on different accessors with for \" +\n                  'the same property (' +\n                  element.key +\n                  ').'\n              );\n            }\n\n            other.decorators = element.decorators;\n          }\n\n          _coalesceGetterSetter(element, other);\n        }\n      } else {\n        newElements.push(element);\n      }\n    }\n\n    return newElements;\n  }\n\n  function _hasDecorators(element) {\n    return element.decorators && element.decorators.length;\n  }\n\n  function _isDataDescriptor(desc) {\n    return (\n      desc !== undefined &&\n      !(desc.value === undefined && desc.writable === undefined)\n    );\n  }\n\n  function _optionalCallableProperty(obj, name) {\n    var value = obj[name];\n\n    if (value !== undefined && typeof value !== 'function') {\n      throw new TypeError(\"Expected '\" + name + \"' to be a function\");\n    }\n\n    return value;\n  }\n\n  function _classPrivateMethodGet(receiver, privateSet, fn) {\n    if (!privateSet.has(receiver)) {\n      throw new TypeError('attempted to get private field on non-instance');\n    }\n\n    return fn;\n  }\n\n  function _classPrivateMethodSet() {\n    throw new TypeError('attempted to reassign private method');\n  }\n\n  function _wrapRegExp(re, groups) {\n    _wrapRegExp = function(re, groups) {\n      return new BabelRegExp(re, groups);\n    };\n\n    var _RegExp = _wrapNativeSuper(RegExp);\n\n    var _super = RegExp.prototype;\n\n    var _groups = new WeakMap();\n\n    function BabelRegExp(re, groups) {\n      var _this = _RegExp.call(this, re);\n\n      _groups.set(_this, groups);\n\n      return _this;\n    }\n\n    _inherits(BabelRegExp, _RegExp);\n\n    BabelRegExp.prototype.exec = function(str) {\n      var result = _super.exec.call(this, str);\n\n      if (result) result.groups = buildGroups(result, this);\n      return result;\n    };\n\n    BabelRegExp.prototype[Symbol.replace] = function(str, substitution) {\n      if (typeof substitution === 'string') {\n        var groups = _groups.get(this);\n\n        return _super[Symbol.replace].call(\n          this,\n          str,\n          substitution.replace(/\\$<([^>]+)>/g, function(_, name) {\n            return '$' + groups[name];\n          })\n        );\n      } else if (typeof substitution === 'function') {\n        var _this = this;\n\n        return _super[Symbol.replace].call(this, str, function() {\n          var args = [];\n          args.push.apply(args, arguments);\n\n          if (typeof args[args.length - 1] !== 'object') {\n            args.push(buildGroups(args, _this));\n          }\n\n          return substitution.apply(this, args);\n        });\n      } else {\n        return _super[Symbol.replace].call(this, str, substitution);\n      }\n    };\n\n    function buildGroups(result, re) {\n      var g = _groups.get(re);\n\n      return Object.keys(g).reduce(function(groups, name) {\n        groups[name] = result[g[name]];\n        return groups;\n      }, Object.create(null));\n    }\n\n    return _wrapRegExp.apply(this, arguments);\n  }\n\n  var vectorMultiply = function vectorMultiply(v, amount) {\n    return createVector(v.x * amount, v.y * amount);\n  };\n\n  var vectorAdd = function vectorAdd(a, b) {\n    return createVector(a.x + b.x, a.y + b.y);\n  };\n\n  var vectorNormalize = function vectorNormalize(v) {\n    var l = Math.sqrt(v.x * v.x + v.y * v.y);\n    if (l === 0) {\n      return {\n        x: 0,\n        y: 0\n      };\n    }\n    return createVector(v.x / l, v.y / l);\n  };\n\n  var vectorRotate = function vectorRotate(v, radians, origin) {\n    var cos = Math.cos(radians);\n    var sin = Math.sin(radians);\n    var t = createVector(v.x - origin.x, v.y - origin.y);\n    return createVector(\n      origin.x + cos * t.x - sin * t.y,\n      origin.y + sin * t.x + cos * t.y\n    );\n  };\n\n  var createVector = function createVector() {\n    var x =\n      arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : 0;\n    var y =\n      arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : 0;\n    return { x: x, y: y };\n  };\n\n  var getMarkupValue = function getMarkupValue(value, size) {\n    var scalar =\n      arguments.length > 2 && arguments[2] !== undefined ? arguments[2] : 1;\n    var axis = arguments.length > 3 ? arguments[3] : undefined;\n    if (typeof value === 'string') {\n      return parseFloat(value) * scalar;\n    }\n    if (typeof value === 'number') {\n      return value * (axis ? size[axis] : Math.min(size.width, size.height));\n    }\n    return;\n  };\n\n  var getMarkupStyles = function getMarkupStyles(markup, size, scale) {\n    var lineStyle = markup.borderStyle || markup.lineStyle || 'solid';\n    var fill = markup.backgroundColor || markup.fontColor || 'transparent';\n    var stroke = markup.borderColor || markup.lineColor || 'transparent';\n    var strokeWidth = getMarkupValue(\n      markup.borderWidth || markup.lineWidth,\n      size,\n      scale\n    );\n    var lineCap = markup.lineCap || 'round';\n    var lineJoin = markup.lineJoin || 'round';\n    var dashes =\n      typeof lineStyle === 'string'\n        ? ''\n        : lineStyle\n            .map(function(v) {\n              return getMarkupValue(v, size, scale);\n            })\n            .join(',');\n    var opacity = markup.opacity || 1;\n    return {\n      'stroke-linecap': lineCap,\n      'stroke-linejoin': lineJoin,\n      'stroke-width': strokeWidth || 0,\n      'stroke-dasharray': dashes,\n      stroke: stroke,\n      fill: fill,\n      opacity: opacity\n    };\n  };\n\n  var isDefined = function isDefined(value) {\n    return value != null;\n  };\n\n  var getMarkupRect = function getMarkupRect(rect, size) {\n    var scalar =\n      arguments.length > 2 && arguments[2] !== undefined ? arguments[2] : 1;\n\n    var left =\n      getMarkupValue(rect.x, size, scalar, 'width') ||\n      getMarkupValue(rect.left, size, scalar, 'width');\n    var top =\n      getMarkupValue(rect.y, size, scalar, 'height') ||\n      getMarkupValue(rect.top, size, scalar, 'height');\n    var width = getMarkupValue(rect.width, size, scalar, 'width');\n    var height = getMarkupValue(rect.height, size, scalar, 'height');\n    var right = getMarkupValue(rect.right, size, scalar, 'width');\n    var bottom = getMarkupValue(rect.bottom, size, scalar, 'height');\n\n    if (!isDefined(top)) {\n      if (isDefined(height) && isDefined(bottom)) {\n        top = size.height - height - bottom;\n      } else {\n        top = bottom;\n      }\n    }\n\n    if (!isDefined(left)) {\n      if (isDefined(width) && isDefined(right)) {\n        left = size.width - width - right;\n      } else {\n        left = right;\n      }\n    }\n\n    if (!isDefined(width)) {\n      if (isDefined(left) && isDefined(right)) {\n        width = size.width - left - right;\n      } else {\n        width = 0;\n      }\n    }\n\n    if (!isDefined(height)) {\n      if (isDefined(top) && isDefined(bottom)) {\n        height = size.height - top - bottom;\n      } else {\n        height = 0;\n      }\n    }\n\n    return {\n      x: left || 0,\n      y: top || 0,\n      width: width || 0,\n      height: height || 0\n    };\n  };\n\n  var pointsToPathShape = function pointsToPathShape(points) {\n    return points\n      .map(function(point, index) {\n        return ''\n          .concat(index === 0 ? 'M' : 'L', ' ')\n          .concat(point.x, ' ')\n          .concat(point.y);\n      })\n      .join(' ');\n  };\n\n  var setAttributes = function setAttributes(element, attr) {\n    return Object.keys(attr).forEach(function(key) {\n      return element.setAttribute(key, attr[key]);\n    });\n  };\n\n  var ns = 'http://www.w3.org/2000/svg';\n  var svg = function svg(tag, attr) {\n    var element = document.createElementNS(ns, tag);\n    if (attr) {\n      setAttributes(element, attr);\n    }\n    return element;\n  };\n\n  var updateRect = function updateRect(element) {\n    return setAttributes(\n      element,\n      Object.assign({}, element.rect, element.styles)\n    );\n  };\n\n  var updateEllipse = function updateEllipse(element) {\n    var cx = element.rect.x + element.rect.width * 0.5;\n    var cy = element.rect.y + element.rect.height * 0.5;\n    var rx = element.rect.width * 0.5;\n    var ry = element.rect.height * 0.5;\n    return setAttributes(\n      element,\n      Object.assign(\n        {\n          cx: cx,\n          cy: cy,\n          rx: rx,\n          ry: ry\n        },\n        element.styles\n      )\n    );\n  };\n\n  var IMAGE_FIT_STYLE = {\n    contain: 'xMidYMid meet',\n    cover: 'xMidYMid slice'\n  };\n\n  var updateImage = function updateImage(element, markup) {\n    setAttributes(\n      element,\n      Object.assign({}, element.rect, element.styles, {\n        preserveAspectRatio: IMAGE_FIT_STYLE[markup.fit] || 'none'\n      })\n    );\n  };\n\n  var TEXT_ANCHOR = {\n    left: 'start',\n    center: 'middle',\n    right: 'end'\n  };\n\n  var updateText = function updateText(element, markup, size, scale) {\n    var fontSize = getMarkupValue(markup.fontSize, size, scale);\n    var fontFamily = markup.fontFamily || 'sans-serif';\n    var fontWeight = markup.fontWeight || 'normal';\n    var textAlign = TEXT_ANCHOR[markup.textAlign] || 'start';\n\n    setAttributes(\n      element,\n      Object.assign({}, element.rect, element.styles, {\n        'stroke-width': 0,\n        'font-weight': fontWeight,\n        'font-size': fontSize,\n        'font-family': fontFamily,\n        'text-anchor': textAlign\n      })\n    );\n\n    // update text\n    if (element.text !== markup.text) {\n      element.text = markup.text;\n      element.textContent = markup.text.length ? markup.text : ' ';\n    }\n  };\n\n  var updateLine = function updateLine(element, markup, size, scale) {\n    setAttributes(\n      element,\n      Object.assign({}, element.rect, element.styles, {\n        fill: 'none'\n      })\n    );\n\n    var line = element.childNodes[0];\n    var begin = element.childNodes[1];\n    var end = element.childNodes[2];\n\n    var origin = element.rect;\n\n    var target = {\n      x: element.rect.x + element.rect.width,\n      y: element.rect.y + element.rect.height\n    };\n\n    setAttributes(line, {\n      x1: origin.x,\n      y1: origin.y,\n      x2: target.x,\n      y2: target.y\n    });\n\n    if (!markup.lineDecoration) return;\n\n    begin.style.display = 'none';\n    end.style.display = 'none';\n\n    var v = vectorNormalize({\n      x: target.x - origin.x,\n      y: target.y - origin.y\n    });\n\n    var l = getMarkupValue(0.05, size, scale);\n\n    if (markup.lineDecoration.indexOf('arrow-begin') !== -1) {\n      var arrowBeginRotationPoint = vectorMultiply(v, l);\n      var arrowBeginCenter = vectorAdd(origin, arrowBeginRotationPoint);\n      var arrowBeginA = vectorRotate(origin, 2, arrowBeginCenter);\n      var arrowBeginB = vectorRotate(origin, -2, arrowBeginCenter);\n\n      setAttributes(begin, {\n        style: 'display:block;',\n        d: 'M'\n          .concat(arrowBeginA.x, ',')\n          .concat(arrowBeginA.y, ' L')\n          .concat(origin.x, ',')\n          .concat(origin.y, ' L')\n          .concat(arrowBeginB.x, ',')\n          .concat(arrowBeginB.y)\n      });\n    }\n\n    if (markup.lineDecoration.indexOf('arrow-end') !== -1) {\n      var arrowEndRotationPoint = vectorMultiply(v, -l);\n      var arrowEndCenter = vectorAdd(target, arrowEndRotationPoint);\n      var arrowEndA = vectorRotate(target, 2, arrowEndCenter);\n      var arrowEndB = vectorRotate(target, -2, arrowEndCenter);\n\n      setAttributes(end, {\n        style: 'display:block;',\n        d: 'M'\n          .concat(arrowEndA.x, ',')\n          .concat(arrowEndA.y, ' L')\n          .concat(target.x, ',')\n          .concat(target.y, ' L')\n          .concat(arrowEndB.x, ',')\n          .concat(arrowEndB.y)\n      });\n    }\n  };\n\n  var updatePath = function updatePath(element, markup, size, scale) {\n    setAttributes(\n      element,\n      Object.assign({}, element.styles, {\n        fill: 'none',\n        d: pointsToPathShape(\n          markup.points.map(function(point) {\n            return {\n              x: getMarkupValue(point.x, size, scale, 'width'),\n              y: getMarkupValue(point.y, size, scale, 'height')\n            };\n          })\n        )\n      })\n    );\n  };\n\n  var createShape = function createShape(node) {\n    return function(markup) {\n      return svg(node, { id: markup.id });\n    };\n  };\n\n  var createImage = function createImage(markup) {\n    var shape = svg('image', {\n      id: markup.id,\n      'stroke-linecap': 'round',\n      'stroke-linejoin': 'round',\n      opacity: '0'\n    });\n\n    shape.onload = function() {\n      shape.setAttribute('opacity', markup.opacity || 1);\n    };\n    shape.setAttributeNS(\n      'http://www.w3.org/1999/xlink',\n      'xlink:href',\n      markup.src\n    );\n    return shape;\n  };\n\n  var createLine = function createLine(markup) {\n    var shape = svg('g', {\n      id: markup.id,\n      'stroke-linecap': 'round',\n      'stroke-linejoin': 'round'\n    });\n\n    var line = svg('line');\n    shape.appendChild(line);\n\n    var begin = svg('path');\n    shape.appendChild(begin);\n\n    var end = svg('path');\n    shape.appendChild(end);\n\n    return shape;\n  };\n\n  var CREATE_TYPE_ROUTES = {\n    image: createImage,\n    rect: createShape('rect'),\n    ellipse: createShape('ellipse'),\n    text: createShape('text'),\n    path: createShape('path'),\n    line: createLine\n  };\n\n  var UPDATE_TYPE_ROUTES = {\n    rect: updateRect,\n    ellipse: updateEllipse,\n    image: updateImage,\n    text: updateText,\n    path: updatePath,\n    line: updateLine\n  };\n\n  var createMarkupByType = function createMarkupByType(type, markup) {\n    return CREATE_TYPE_ROUTES[type](markup);\n  };\n\n  var updateMarkupByType = function updateMarkupByType(\n    element,\n    type,\n    markup,\n    size,\n    scale\n  ) {\n    if (type !== 'path') {\n      element.rect = getMarkupRect(markup, size, scale);\n    }\n    element.styles = getMarkupStyles(markup, size, scale);\n    UPDATE_TYPE_ROUTES[type](element, markup, size, scale);\n  };\n\n  var MARKUP_RECT = [\n    'x',\n    'y',\n    'left',\n    'top',\n    'right',\n    'bottom',\n    'width',\n    'height'\n  ];\n\n  var toOptionalFraction = function toOptionalFraction(value) {\n    return typeof value === 'string' && /%/.test(value)\n      ? parseFloat(value) / 100\n      : value;\n  };\n\n  // adds default markup properties, clones markup\n  var prepareMarkup = function prepareMarkup(markup) {\n    var _markup = _slicedToArray(markup, 2),\n      type = _markup[0],\n      props = _markup[1];\n\n    var rect = props.points\n      ? {}\n      : MARKUP_RECT.reduce(function(prev, curr) {\n          prev[curr] = toOptionalFraction(props[curr]);\n          return prev;\n        }, {});\n\n    return [\n      type,\n      Object.assign(\n        {\n          zIndex: 0\n        },\n        props,\n        rect\n      )\n    ];\n  };\n\n  var sortMarkupByZIndex = function sortMarkupByZIndex(a, b) {\n    if (a[1].zIndex > b[1].zIndex) {\n      return 1;\n    }\n    if (a[1].zIndex < b[1].zIndex) {\n      return -1;\n    }\n    return 0;\n  };\n\n  var createMarkupView = function createMarkupView(_) {\n    return _.utils.createView({\n      name: 'image-preview-markup',\n      tag: 'svg',\n      ignoreRect: true,\n      mixins: {\n        apis: ['width', 'height', 'crop', 'markup', 'resize', 'dirty']\n      },\n\n      write: function write(_ref) {\n        var root = _ref.root,\n          props = _ref.props;\n\n        if (!props.dirty) return;\n        var crop = props.crop,\n          resize = props.resize,\n          markup = props.markup;\n\n        var viewWidth = props.width;\n        var viewHeight = props.height;\n\n        var cropWidth = crop.width;\n        var cropHeight = crop.height;\n\n        if (resize) {\n          var _size = resize.size;\n\n          var outputWidth = _size && _size.width;\n          var outputHeight = _size && _size.height;\n          var outputFit = resize.mode;\n          var outputUpscale = resize.upscale;\n\n          if (outputWidth && !outputHeight) outputHeight = outputWidth;\n          if (outputHeight && !outputWidth) outputWidth = outputHeight;\n\n          var shouldUpscale =\n            cropWidth < outputWidth && cropHeight < outputHeight;\n\n          if (!shouldUpscale || (shouldUpscale && outputUpscale)) {\n            var scalarWidth = outputWidth / cropWidth;\n            var scalarHeight = outputHeight / cropHeight;\n\n            if (outputFit === 'force') {\n              cropWidth = outputWidth;\n              cropHeight = outputHeight;\n            } else {\n              var scalar;\n              if (outputFit === 'cover') {\n                scalar = Math.max(scalarWidth, scalarHeight);\n              } else if (outputFit === 'contain') {\n                scalar = Math.min(scalarWidth, scalarHeight);\n              }\n              cropWidth = cropWidth * scalar;\n              cropHeight = cropHeight * scalar;\n            }\n          }\n        }\n\n        var size = {\n          width: viewWidth,\n          height: viewHeight\n        };\n\n        root.element.setAttribute('width', size.width);\n        root.element.setAttribute('height', size.height);\n\n        var scale = Math.min(viewWidth / cropWidth, viewHeight / cropHeight);\n\n        // clear\n        root.element.innerHTML = '';\n\n        // get filter\n        var markupFilter = root.query('GET_IMAGE_PREVIEW_MARKUP_FILTER');\n\n        // draw new\n        markup\n          .filter(markupFilter)\n          .map(prepareMarkup)\n          .sort(sortMarkupByZIndex)\n          .forEach(function(markup) {\n            var _markup = _slicedToArray(markup, 2),\n              type = _markup[0],\n              settings = _markup[1];\n\n            // create\n            var element = createMarkupByType(type, settings);\n\n            // update\n            updateMarkupByType(element, type, settings, size, scale);\n\n            // add\n            root.element.appendChild(element);\n          });\n      }\n    });\n  };\n\n  var createVector$1 = function createVector(x, y) {\n    return { x: x, y: y };\n  };\n\n  var vectorDot = function vectorDot(a, b) {\n    return a.x * b.x + a.y * b.y;\n  };\n\n  var vectorSubtract = function vectorSubtract(a, b) {\n    return createVector$1(a.x - b.x, a.y - b.y);\n  };\n\n  var vectorDistanceSquared = function vectorDistanceSquared(a, b) {\n    return vectorDot(vectorSubtract(a, b), vectorSubtract(a, b));\n  };\n\n  var vectorDistance = function vectorDistance(a, b) {\n    return Math.sqrt(vectorDistanceSquared(a, b));\n  };\n\n  var getOffsetPointOnEdge = function getOffsetPointOnEdge(length, rotation) {\n    var a = length;\n\n    var A = 1.5707963267948966;\n    var B = rotation;\n    var C = 1.5707963267948966 - rotation;\n\n    var sinA = Math.sin(A);\n    var sinB = Math.sin(B);\n    var sinC = Math.sin(C);\n    var cosC = Math.cos(C);\n    var ratio = a / sinA;\n    var b = ratio * sinB;\n    var c = ratio * sinC;\n\n    return createVector$1(cosC * b, cosC * c);\n  };\n\n  var getRotatedRectSize = function getRotatedRectSize(rect, rotation) {\n    var w = rect.width;\n    var h = rect.height;\n\n    var hor = getOffsetPointOnEdge(w, rotation);\n    var ver = getOffsetPointOnEdge(h, rotation);\n\n    var tl = createVector$1(rect.x + Math.abs(hor.x), rect.y - Math.abs(hor.y));\n\n    var tr = createVector$1(\n      rect.x + rect.width + Math.abs(ver.y),\n      rect.y + Math.abs(ver.x)\n    );\n\n    var bl = createVector$1(\n      rect.x - Math.abs(ver.y),\n      rect.y + rect.height - Math.abs(ver.x)\n    );\n\n    return {\n      width: vectorDistance(tl, tr),\n      height: vectorDistance(tl, bl)\n    };\n  };\n\n  var calculateCanvasSize = function calculateCanvasSize(\n    image,\n    canvasAspectRatio\n  ) {\n    var zoom =\n      arguments.length > 2 && arguments[2] !== undefined ? arguments[2] : 1;\n\n    var imageAspectRatio = image.height / image.width;\n\n    // determine actual pixels on x and y axis\n    var canvasWidth = 1;\n    var canvasHeight = canvasAspectRatio;\n    var imgWidth = 1;\n    var imgHeight = imageAspectRatio;\n    if (imgHeight > canvasHeight) {\n      imgHeight = canvasHeight;\n      imgWidth = imgHeight / imageAspectRatio;\n    }\n\n    var scalar = Math.max(canvasWidth / imgWidth, canvasHeight / imgHeight);\n    var width = image.width / (zoom * scalar * imgWidth);\n    var height = width * canvasAspectRatio;\n\n    return {\n      width: width,\n      height: height\n    };\n  };\n\n  var getImageRectZoomFactor = function getImageRectZoomFactor(\n    imageRect,\n    cropRect,\n    rotation,\n    center\n  ) {\n    // calculate available space round image center position\n    var cx = center.x > 0.5 ? 1 - center.x : center.x;\n    var cy = center.y > 0.5 ? 1 - center.y : center.y;\n    var imageWidth = cx * 2 * imageRect.width;\n    var imageHeight = cy * 2 * imageRect.height;\n\n    // calculate rotated crop rectangle size\n    var rotatedCropSize = getRotatedRectSize(cropRect, rotation);\n\n    // calculate scalar required to fit image\n    return Math.max(\n      rotatedCropSize.width / imageWidth,\n      rotatedCropSize.height / imageHeight\n    );\n  };\n\n  var getCenteredCropRect = function getCenteredCropRect(\n    container,\n    aspectRatio\n  ) {\n    var width = container.width;\n    var height = width * aspectRatio;\n    if (height > container.height) {\n      height = container.height;\n      width = height / aspectRatio;\n    }\n    var x = (container.width - width) * 0.5;\n    var y = (container.height - height) * 0.5;\n\n    return {\n      x: x,\n      y: y,\n      width: width,\n      height: height\n    };\n  };\n\n  var getCurrentCropSize = function getCurrentCropSize(imageSize) {\n    var crop =\n      arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};\n    var zoom = crop.zoom,\n      rotation = crop.rotation,\n      center = crop.center,\n      aspectRatio = crop.aspectRatio;\n\n    if (!aspectRatio) aspectRatio = imageSize.height / imageSize.width;\n\n    var canvasSize = calculateCanvasSize(imageSize, aspectRatio, zoom);\n\n    var canvasCenter = {\n      x: canvasSize.width * 0.5,\n      y: canvasSize.height * 0.5\n    };\n\n    var stage = {\n      x: 0,\n      y: 0,\n      width: canvasSize.width,\n      height: canvasSize.height,\n      center: canvasCenter\n    };\n\n    var shouldLimit = typeof crop.scaleToFit === 'undefined' || crop.scaleToFit;\n\n    var stageZoomFactor = getImageRectZoomFactor(\n      imageSize,\n      getCenteredCropRect(stage, aspectRatio),\n      rotation,\n      shouldLimit ? center : { x: 0.5, y: 0.5 }\n    );\n\n    var scale = zoom * stageZoomFactor;\n\n    // start drawing\n    return {\n      widthFloat: canvasSize.width / scale,\n      heightFloat: canvasSize.height / scale,\n      width: Math.round(canvasSize.width / scale),\n      height: Math.round(canvasSize.height / scale)\n    };\n  };\n\n  var IMAGE_SCALE_SPRING_PROPS = {\n    type: 'spring',\n    stiffness: 0.5,\n    damping: 0.45,\n    mass: 10\n  };\n\n  // does horizontal and vertical flipping\n  var createBitmapView = function createBitmapView(_) {\n    return _.utils.createView({\n      name: 'image-bitmap',\n      ignoreRect: true,\n      mixins: { styles: ['scaleX', 'scaleY'] },\n      create: function create(_ref) {\n        var root = _ref.root,\n          props = _ref.props;\n        root.appendChild(props.image);\n      }\n    });\n  };\n\n  // shifts and rotates image\n  var createImageCanvasWrapper = function createImageCanvasWrapper(_) {\n    return _.utils.createView({\n      name: 'image-canvas-wrapper',\n      tag: 'div',\n      ignoreRect: true,\n      mixins: {\n        apis: ['crop', 'width', 'height'],\n\n        styles: [\n          'originX',\n          'originY',\n          'translateX',\n          'translateY',\n          'scaleX',\n          'scaleY',\n          'rotateZ'\n        ],\n\n        animations: {\n          originX: IMAGE_SCALE_SPRING_PROPS,\n          originY: IMAGE_SCALE_SPRING_PROPS,\n          scaleX: IMAGE_SCALE_SPRING_PROPS,\n          scaleY: IMAGE_SCALE_SPRING_PROPS,\n          translateX: IMAGE_SCALE_SPRING_PROPS,\n          translateY: IMAGE_SCALE_SPRING_PROPS,\n          rotateZ: IMAGE_SCALE_SPRING_PROPS\n        }\n      },\n\n      create: function create(_ref2) {\n        var root = _ref2.root,\n          props = _ref2.props;\n        props.width = props.image.width;\n        props.height = props.image.height;\n        root.ref.bitmap = root.appendChildView(\n          root.createChildView(createBitmapView(_), { image: props.image })\n        );\n      },\n      write: function write(_ref3) {\n        var root = _ref3.root,\n          props = _ref3.props;\n        var flip = props.crop.flip;\n        var bitmap = root.ref.bitmap;\n        bitmap.scaleX = flip.horizontal ? -1 : 1;\n        bitmap.scaleY = flip.vertical ? -1 : 1;\n      }\n    });\n  };\n\n  // clips canvas to correct aspect ratio\n  var createClipView = function createClipView(_) {\n    return _.utils.createView({\n      name: 'image-clip',\n      tag: 'div',\n      ignoreRect: true,\n      mixins: {\n        apis: [\n          'crop',\n          'markup',\n          'resize',\n          'width',\n          'height',\n          'dirty',\n          'background'\n        ],\n\n        styles: ['width', 'height', 'opacity'],\n        animations: {\n          opacity: { type: 'tween', duration: 250 }\n        }\n      },\n\n      didWriteView: function didWriteView(_ref4) {\n        var root = _ref4.root,\n          props = _ref4.props;\n        if (!props.background) return;\n        root.element.style.backgroundColor = props.background;\n      },\n      create: function create(_ref5) {\n        var root = _ref5.root,\n          props = _ref5.props;\n\n        root.ref.image = root.appendChildView(\n          root.createChildView(\n            createImageCanvasWrapper(_),\n            Object.assign({}, props)\n          )\n        );\n\n        root.ref.createMarkup = function() {\n          if (root.ref.markup) return;\n          root.ref.markup = root.appendChildView(\n            root.createChildView(createMarkupView(_), Object.assign({}, props))\n          );\n        };\n\n        root.ref.destroyMarkup = function() {\n          if (!root.ref.markup) return;\n          root.removeChildView(root.ref.markup);\n          root.ref.markup = null;\n        };\n\n        // set up transparency grid\n        var transparencyIndicator = root.query(\n          'GET_IMAGE_PREVIEW_TRANSPARENCY_INDICATOR'\n        );\n        if (transparencyIndicator === null) return;\n\n        // grid pattern\n        if (transparencyIndicator === 'grid') {\n          root.element.dataset.transparencyIndicator = transparencyIndicator;\n        }\n        // basic color\n        else {\n          root.element.dataset.transparencyIndicator = 'color';\n        }\n      },\n      write: function write(_ref6) {\n        var root = _ref6.root,\n          props = _ref6.props,\n          shouldOptimize = _ref6.shouldOptimize;\n        var crop = props.crop,\n          markup = props.markup,\n          resize = props.resize,\n          dirty = props.dirty,\n          width = props.width,\n          height = props.height;\n\n        root.ref.image.crop = crop;\n\n        var stage = {\n          x: 0,\n          y: 0,\n          width: width,\n          height: height,\n          center: {\n            x: width * 0.5,\n            y: height * 0.5\n          }\n        };\n\n        var image = {\n          width: root.ref.image.width,\n          height: root.ref.image.height\n        };\n\n        var origin = {\n          x: crop.center.x * image.width,\n          y: crop.center.y * image.height\n        };\n\n        var translation = {\n          x: stage.center.x - image.width * crop.center.x,\n          y: stage.center.y - image.height * crop.center.y\n        };\n\n        var rotation = Math.PI * 2 + (crop.rotation % (Math.PI * 2));\n\n        var cropAspectRatio = crop.aspectRatio || image.height / image.width;\n\n        var shouldLimit =\n          typeof crop.scaleToFit === 'undefined' || crop.scaleToFit;\n\n        var stageZoomFactor = getImageRectZoomFactor(\n          image,\n          getCenteredCropRect(stage, cropAspectRatio),\n\n          rotation,\n          shouldLimit ? crop.center : { x: 0.5, y: 0.5 }\n        );\n\n        var scale = crop.zoom * stageZoomFactor;\n\n        // update markup view\n        if (markup && markup.length) {\n          root.ref.createMarkup();\n          root.ref.markup.width = width;\n          root.ref.markup.height = height;\n          root.ref.markup.resize = resize;\n          root.ref.markup.dirty = dirty;\n          root.ref.markup.markup = markup;\n          root.ref.markup.crop = getCurrentCropSize(image, crop);\n        } else if (root.ref.markup) {\n          root.ref.destroyMarkup();\n        }\n\n        // update image view\n        var imageView = root.ref.image;\n\n        // don't update clip layout\n        if (shouldOptimize) {\n          imageView.originX = null;\n          imageView.originY = null;\n          imageView.translateX = null;\n          imageView.translateY = null;\n          imageView.rotateZ = null;\n          imageView.scaleX = null;\n          imageView.scaleY = null;\n          return;\n        }\n\n        imageView.originX = origin.x;\n        imageView.originY = origin.y;\n        imageView.translateX = translation.x;\n        imageView.translateY = translation.y;\n        imageView.rotateZ = rotation;\n        imageView.scaleX = scale;\n        imageView.scaleY = scale;\n      }\n    });\n  };\n\n  var createImageView = function createImageView(_) {\n    return _.utils.createView({\n      name: 'image-preview',\n      tag: 'div',\n      ignoreRect: true,\n      mixins: {\n        apis: ['image', 'crop', 'markup', 'resize', 'dirty', 'background'],\n\n        styles: ['translateY', 'scaleX', 'scaleY', 'opacity'],\n\n        animations: {\n          scaleX: IMAGE_SCALE_SPRING_PROPS,\n          scaleY: IMAGE_SCALE_SPRING_PROPS,\n          translateY: IMAGE_SCALE_SPRING_PROPS,\n          opacity: { type: 'tween', duration: 400 }\n        }\n      },\n\n      create: function create(_ref7) {\n        var root = _ref7.root,\n          props = _ref7.props;\n        root.ref.clip = root.appendChildView(\n          root.createChildView(createClipView(_), {\n            id: props.id,\n            image: props.image,\n            crop: props.crop,\n            markup: props.markup,\n            resize: props.resize,\n            dirty: props.dirty,\n            background: props.background\n          })\n        );\n      },\n      write: function write(_ref8) {\n        var root = _ref8.root,\n          props = _ref8.props,\n          shouldOptimize = _ref8.shouldOptimize;\n        var clip = root.ref.clip;\n        var image = props.image,\n          crop = props.crop,\n          markup = props.markup,\n          resize = props.resize,\n          dirty = props.dirty;\n\n        clip.crop = crop;\n        clip.markup = markup;\n        clip.resize = resize;\n        clip.dirty = dirty;\n\n        // don't update clip layout\n        clip.opacity = shouldOptimize ? 0 : 1;\n\n        // don't re-render if optimizing or hidden (width will be zero resulting in weird animations)\n        if (shouldOptimize || root.rect.element.hidden) return;\n\n        // calculate scaled preview image size\n        var imageAspectRatio = image.height / image.width;\n        var aspectRatio = crop.aspectRatio || imageAspectRatio;\n\n        // calculate container size\n        var containerWidth = root.rect.inner.width;\n        var containerHeight = root.rect.inner.height;\n\n        var fixedPreviewHeight = root.query('GET_IMAGE_PREVIEW_HEIGHT');\n        var minPreviewHeight = root.query('GET_IMAGE_PREVIEW_MIN_HEIGHT');\n        var maxPreviewHeight = root.query('GET_IMAGE_PREVIEW_MAX_HEIGHT');\n\n        var panelAspectRatio = root.query('GET_PANEL_ASPECT_RATIO');\n        var allowMultiple = root.query('GET_ALLOW_MULTIPLE');\n\n        if (panelAspectRatio && !allowMultiple) {\n          fixedPreviewHeight = containerWidth * panelAspectRatio;\n          aspectRatio = panelAspectRatio;\n        }\n\n        // determine clip width and height\n        var clipHeight =\n          fixedPreviewHeight !== null\n            ? fixedPreviewHeight\n            : Math.max(\n                minPreviewHeight,\n                Math.min(containerWidth * aspectRatio, maxPreviewHeight)\n              );\n\n        var clipWidth = clipHeight / aspectRatio;\n        if (clipWidth > containerWidth) {\n          clipWidth = containerWidth;\n          clipHeight = clipWidth * aspectRatio;\n        }\n\n        if (clipHeight > containerHeight) {\n          clipHeight = containerHeight;\n          clipWidth = containerHeight / aspectRatio;\n        }\n\n        clip.width = clipWidth;\n        clip.height = clipHeight;\n      }\n    });\n  };\n\n  var SVG_MASK =\n    '<svg width=\"500\" height=\"200\" viewBox=\"0 0 500 200\" preserveAspectRatio=\"none\">\\n    <defs>\\n        <radialGradient id=\"gradient-__UID__\" cx=\".5\" cy=\"1.25\" r=\"1.15\">\\n            <stop offset=\\'50%\\' stop-color=\\'#000000\\'/>\\n            <stop offset=\\'56%\\' stop-color=\\'#0a0a0a\\'/>\\n            <stop offset=\\'63%\\' stop-color=\\'#262626\\'/>\\n            <stop offset=\\'69%\\' stop-color=\\'#4f4f4f\\'/>\\n            <stop offset=\\'75%\\' stop-color=\\'#808080\\'/>\\n            <stop offset=\\'81%\\' stop-color=\\'#b1b1b1\\'/>\\n            <stop offset=\\'88%\\' stop-color=\\'#dadada\\'/>\\n            <stop offset=\\'94%\\' stop-color=\\'#f6f6f6\\'/>\\n            <stop offset=\\'100%\\' stop-color=\\'#ffffff\\'/>\\n        </radialGradient>\\n        <mask id=\"mask-__UID__\">\\n            <rect x=\"0\" y=\"0\" width=\"500\" height=\"200\" fill=\"url(#gradient-__UID__)\"></rect>\\n        </mask>\\n    </defs>\\n    <rect x=\"0\" width=\"500\" height=\"200\" fill=\"currentColor\" mask=\"url(#mask-__UID__)\"></rect>\\n</svg>';\n\n  var SVGMaskUniqueId = 0;\n\n  var createImageOverlayView = function createImageOverlayView(fpAPI) {\n    return fpAPI.utils.createView({\n      name: 'image-preview-overlay',\n      tag: 'div',\n      ignoreRect: true,\n      create: function create(_ref) {\n        var root = _ref.root,\n          props = _ref.props;\n        var mask = SVG_MASK;\n        if (document.querySelector('base')) {\n          var url = window.location.href.replace(window.location.hash, '');\n          mask = mask.replace(/url\\(\\#/g, 'url(' + url + '#');\n        }\n\n        SVGMaskUniqueId++;\n        root.element.classList.add(\n          'filepond--image-preview-overlay-'.concat(props.status)\n        );\n\n        root.element.innerHTML = mask.replace(/__UID__/g, SVGMaskUniqueId);\n      },\n      mixins: {\n        styles: ['opacity'],\n        animations: {\n          opacity: { type: 'spring', mass: 25 }\n        }\n      }\n    });\n  };\n\n  /**\n   * Bitmap Worker\n   */\n  var BitmapWorker = function BitmapWorker() {\n    self.onmessage = function(e) {\n      createImageBitmap(e.data.message.file).then(function(bitmap) {\n        self.postMessage({ id: e.data.id, message: bitmap }, [bitmap]);\n      });\n    };\n  };\n\n  /**\n   * ColorMatrix Worker\n   */\n  var ColorMatrixWorker = function ColorMatrixWorker() {\n    self.onmessage = function(e) {\n      var imageData = e.data.message.imageData;\n      var matrix = e.data.message.colorMatrix;\n\n      var data = imageData.data;\n      var l = data.length;\n\n      var m11 = matrix[0];\n      var m12 = matrix[1];\n      var m13 = matrix[2];\n      var m14 = matrix[3];\n      var m15 = matrix[4];\n\n      var m21 = matrix[5];\n      var m22 = matrix[6];\n      var m23 = matrix[7];\n      var m24 = matrix[8];\n      var m25 = matrix[9];\n\n      var m31 = matrix[10];\n      var m32 = matrix[11];\n      var m33 = matrix[12];\n      var m34 = matrix[13];\n      var m35 = matrix[14];\n\n      var m41 = matrix[15];\n      var m42 = matrix[16];\n      var m43 = matrix[17];\n      var m44 = matrix[18];\n      var m45 = matrix[19];\n\n      var index = 0,\n        r = 0.0,\n        g = 0.0,\n        b = 0.0,\n        a = 0.0;\n\n      for (; index < l; index += 4) {\n        r = data[index] / 255;\n        g = data[index + 1] / 255;\n        b = data[index + 2] / 255;\n        a = data[index + 3] / 255;\n        data[index] = Math.max(\n          0,\n          Math.min((r * m11 + g * m12 + b * m13 + a * m14 + m15) * 255, 255)\n        );\n        data[index + 1] = Math.max(\n          0,\n          Math.min((r * m21 + g * m22 + b * m23 + a * m24 + m25) * 255, 255)\n        );\n        data[index + 2] = Math.max(\n          0,\n          Math.min((r * m31 + g * m32 + b * m33 + a * m34 + m35) * 255, 255)\n        );\n        data[index + 3] = Math.max(\n          0,\n          Math.min((r * m41 + g * m42 + b * m43 + a * m44 + m45) * 255, 255)\n        );\n      }\n\n      self.postMessage({ id: e.data.id, message: imageData }, [\n        imageData.data.buffer\n      ]);\n    };\n  };\n\n  var getImageSize = function getImageSize(url, cb) {\n    var image = new Image();\n    image.onload = function() {\n      var width = image.naturalWidth;\n      var height = image.naturalHeight;\n      image = null;\n      cb(width, height);\n    };\n    image.src = url;\n  };\n\n  var transforms = {\n    1: function _() {\n      return [1, 0, 0, 1, 0, 0];\n    },\n    2: function _(width) {\n      return [-1, 0, 0, 1, width, 0];\n    },\n    3: function _(width, height) {\n      return [-1, 0, 0, -1, width, height];\n    },\n    4: function _(width, height) {\n      return [1, 0, 0, -1, 0, height];\n    },\n    5: function _() {\n      return [0, 1, 1, 0, 0, 0];\n    },\n    6: function _(width, height) {\n      return [0, 1, -1, 0, height, 0];\n    },\n    7: function _(width, height) {\n      return [0, -1, -1, 0, height, width];\n    },\n    8: function _(width) {\n      return [0, -1, 1, 0, 0, width];\n    }\n  };\n\n  var fixImageOrientation = function fixImageOrientation(\n    ctx,\n    width,\n    height,\n    orientation\n  ) {\n    // no orientation supplied\n    if (orientation === -1) {\n      return;\n    }\n\n    ctx.transform.apply(ctx, transforms[orientation](width, height));\n  };\n\n  // draws the preview image to canvas\n  var createPreviewImage = function createPreviewImage(\n    data,\n    width,\n    height,\n    orientation\n  ) {\n    // can't draw on half pixels\n    width = Math.round(width);\n    height = Math.round(height);\n\n    // draw image\n    var canvas = document.createElement('canvas');\n    canvas.width = width;\n    canvas.height = height;\n    var ctx = canvas.getContext('2d');\n\n    // if is rotated incorrectly swap width and height\n    if (orientation >= 5 && orientation <= 8) {\n      var _ref = [height, width];\n      width = _ref[0];\n      height = _ref[1];\n    }\n\n    // correct image orientation\n    fixImageOrientation(ctx, width, height, orientation);\n\n    // draw the image\n    ctx.drawImage(data, 0, 0, width, height);\n\n    return canvas;\n  };\n\n  var isBitmap = function isBitmap(file) {\n    return /^image/.test(file.type) && !/svg/.test(file.type);\n  };\n\n  var MAX_WIDTH = 10;\n  var MAX_HEIGHT = 10;\n\n  var calculateAverageColor = function calculateAverageColor(image) {\n    var scalar = Math.min(MAX_WIDTH / image.width, MAX_HEIGHT / image.height);\n\n    var canvas = document.createElement('canvas');\n    var ctx = canvas.getContext('2d');\n    var width = (canvas.width = Math.ceil(image.width * scalar));\n    var height = (canvas.height = Math.ceil(image.height * scalar));\n    ctx.drawImage(image, 0, 0, width, height);\n    var data = null;\n    try {\n      data = ctx.getImageData(0, 0, width, height).data;\n    } catch (e) {\n      return null;\n    }\n    var l = data.length;\n\n    var r = 0;\n    var g = 0;\n    var b = 0;\n    var i = 0;\n\n    for (; i < l; i += 4) {\n      r += data[i] * data[i];\n      g += data[i + 1] * data[i + 1];\n      b += data[i + 2] * data[i + 2];\n    }\n\n    r = averageColor(r, l);\n    g = averageColor(g, l);\n    b = averageColor(b, l);\n\n    return { r: r, g: g, b: b };\n  };\n\n  var averageColor = function averageColor(c, l) {\n    return Math.floor(Math.sqrt(c / (l / 4)));\n  };\n\n  var cloneCanvas = function cloneCanvas(origin, target) {\n    target = target || document.createElement('canvas');\n    target.width = origin.width;\n    target.height = origin.height;\n    var ctx = target.getContext('2d');\n    ctx.drawImage(origin, 0, 0);\n    return target;\n  };\n\n  var cloneImageData = function cloneImageData(imageData) {\n    var id;\n    try {\n      id = new ImageData(imageData.width, imageData.height);\n    } catch (e) {\n      var canvas = document.createElement('canvas');\n      var ctx = canvas.getContext('2d');\n      id = ctx.createImageData(imageData.width, imageData.height);\n    }\n    id.data.set(new Uint8ClampedArray(imageData.data));\n    return id;\n  };\n\n  var loadImage = function loadImage(url) {\n    return new Promise(function(resolve, reject) {\n      var img = new Image();\n      img.crossOrigin = 'Anonymous';\n      img.onload = function() {\n        resolve(img);\n      };\n      img.onerror = function(e) {\n        reject(e);\n      };\n      img.src = url;\n    });\n  };\n\n  var createImageWrapperView = function createImageWrapperView(_) {\n    // create overlay view\n    var OverlayView = createImageOverlayView(_);\n\n    var ImageView = createImageView(_);\n    var createWorker = _.utils.createWorker;\n\n    var applyFilter = function applyFilter(root, filter, target) {\n      return new Promise(function(resolve) {\n        // will store image data for future filter updates\n        if (!root.ref.imageData) {\n          root.ref.imageData = target\n            .getContext('2d')\n            .getImageData(0, 0, target.width, target.height);\n        }\n\n        // get image data reference\n        var imageData = cloneImageData(root.ref.imageData);\n\n        if (!filter || filter.length !== 20) {\n          target.getContext('2d').putImageData(imageData, 0, 0);\n          return resolve();\n        }\n\n        var worker = createWorker(ColorMatrixWorker);\n        worker.post(\n          {\n            imageData: imageData,\n            colorMatrix: filter\n          },\n\n          function(response) {\n            // apply filtered colors\n            target.getContext('2d').putImageData(response, 0, 0);\n\n            // stop worker\n            worker.terminate();\n\n            // done!\n            resolve();\n          },\n          [imageData.data.buffer]\n        );\n      });\n    };\n\n    var removeImageView = function removeImageView(root, imageView) {\n      root.removeChildView(imageView);\n      imageView.image.width = 1;\n      imageView.image.height = 1;\n      imageView._destroy();\n    };\n\n    // remove an image\n    var shiftImage = function shiftImage(_ref) {\n      var root = _ref.root;\n      var imageView = root.ref.images.shift();\n      imageView.opacity = 0;\n      imageView.translateY = -15;\n      root.ref.imageViewBin.push(imageView);\n      return imageView;\n    };\n\n    // add new image\n    var pushImage = function pushImage(_ref2) {\n      var root = _ref2.root,\n        props = _ref2.props,\n        image = _ref2.image;\n      var id = props.id;\n      var item = root.query('GET_ITEM', { id: id });\n      if (!item) return;\n\n      var crop = item.getMetadata('crop') || {\n        center: {\n          x: 0.5,\n          y: 0.5\n        },\n\n        flip: {\n          horizontal: false,\n          vertical: false\n        },\n\n        zoom: 1,\n        rotation: 0,\n        aspectRatio: null\n      };\n\n      var background = root.query(\n        'GET_IMAGE_TRANSFORM_CANVAS_BACKGROUND_COLOR'\n      );\n\n      var markup;\n      var resize;\n      var dirty = false;\n      if (root.query('GET_IMAGE_PREVIEW_MARKUP_SHOW')) {\n        markup = item.getMetadata('markup') || [];\n        resize = item.getMetadata('resize');\n        dirty = true;\n      }\n\n      // append image presenter\n      var imageView = root.appendChildView(\n        root.createChildView(ImageView, {\n          id: id,\n          image: image,\n          crop: crop,\n          resize: resize,\n          markup: markup,\n          dirty: dirty,\n          background: background,\n          opacity: 0,\n          scaleX: 1.15,\n          scaleY: 1.15,\n          translateY: 15\n        }),\n\n        root.childViews.length\n      );\n\n      root.ref.images.push(imageView);\n\n      // reveal the preview image\n      imageView.opacity = 1;\n      imageView.scaleX = 1;\n      imageView.scaleY = 1;\n      imageView.translateY = 0;\n\n      // the preview is now ready to be drawn\n      setTimeout(function() {\n        root.dispatch('DID_IMAGE_PREVIEW_SHOW', { id: id });\n      }, 250);\n    };\n\n    var updateImage = function updateImage(_ref3) {\n      var root = _ref3.root,\n        props = _ref3.props;\n      var item = root.query('GET_ITEM', { id: props.id });\n      if (!item) return;\n      var imageView = root.ref.images[root.ref.images.length - 1];\n      imageView.crop = item.getMetadata('crop');\n      imageView.background = root.query(\n        'GET_IMAGE_TRANSFORM_CANVAS_BACKGROUND_COLOR'\n      );\n\n      if (root.query('GET_IMAGE_PREVIEW_MARKUP_SHOW')) {\n        imageView.dirty = true;\n        imageView.resize = item.getMetadata('resize');\n        imageView.markup = item.getMetadata('markup');\n      }\n    };\n\n    // replace image preview\n    var didUpdateItemMetadata = function didUpdateItemMetadata(_ref4) {\n      var root = _ref4.root,\n        props = _ref4.props,\n        action = _ref4.action;\n      // only filter and crop trigger redraw\n      if (!/crop|filter|markup|resize/.test(action.change.key)) return;\n\n      // no images to update, exit\n      if (!root.ref.images.length) return;\n\n      // no item found, exit\n      var item = root.query('GET_ITEM', { id: props.id });\n      if (!item) return;\n\n      // for now, update existing image when filtering\n      if (/filter/.test(action.change.key)) {\n        var imageView = root.ref.images[root.ref.images.length - 1];\n        applyFilter(root, action.change.value, imageView.image);\n        return;\n      }\n\n      if (/crop|markup|resize/.test(action.change.key)) {\n        var crop = item.getMetadata('crop');\n        var image = root.ref.images[root.ref.images.length - 1];\n\n        // if aspect ratio has changed, we need to create a new image\n        if (\n          crop &&\n          crop.aspectRatio &&\n          image.crop &&\n          image.crop.aspectRatio &&\n          Math.abs(crop.aspectRatio - image.crop.aspectRatio) > 0.00001\n        ) {\n          var _imageView = shiftImage({ root: root });\n          pushImage({\n            root: root,\n            props: props,\n            image: cloneCanvas(_imageView.image)\n          });\n        }\n        // if not, we can update the current image\n        else {\n          updateImage({ root: root, props: props });\n        }\n      }\n    };\n\n    var canCreateImageBitmap = function canCreateImageBitmap(file) {\n      // Firefox versions before 58 will freeze when running createImageBitmap\n      // in a Web Worker so we detect those versions and return false for support\n      var userAgent = window.navigator.userAgent;\n      var isFirefox = userAgent.match(/Firefox\\/([0-9]+)\\./);\n      var firefoxVersion = isFirefox ? parseInt(isFirefox[1]) : null;\n      if (firefoxVersion <= 58) return false;\n\n      return 'createImageBitmap' in window && isBitmap(file);\n    };\n\n    /**\n     * Write handler for when preview container has been created\n     */\n    var didCreatePreviewContainer = function didCreatePreviewContainer(_ref5) {\n      var root = _ref5.root,\n        props = _ref5.props;\n      var id = props.id;\n\n      // we need to get the file data to determine the eventual image size\n      var item = root.query('GET_ITEM', id);\n      if (!item) return;\n\n      // get url to file (we'll revoke it later on when done)\n      var fileURL = URL.createObjectURL(item.file);\n\n      // determine image size of this item\n      getImageSize(fileURL, function(width, height) {\n        // we can now scale the panel to the final size\n        root.dispatch('DID_IMAGE_PREVIEW_CALCULATE_SIZE', {\n          id: id,\n          width: width,\n          height: height\n        });\n      });\n    };\n\n    var drawPreview = function drawPreview(_ref6) {\n      var root = _ref6.root,\n        props = _ref6.props;\n      var id = props.id;\n\n      // we need to get the file data to determine the eventual image size\n      var item = root.query('GET_ITEM', id);\n      if (!item) return;\n\n      // get url to file (we'll revoke it later on when done)\n      var fileURL = URL.createObjectURL(item.file);\n\n      // fallback\n      var loadPreviewFallback = function loadPreviewFallback() {\n        // let's scale the image in the main thread :(\n        loadImage(fileURL).then(previewImageLoaded);\n      };\n\n      // image is now ready\n      var previewImageLoaded = function previewImageLoaded(imageData) {\n        // the file url is no longer needed\n        URL.revokeObjectURL(fileURL);\n\n        // draw the scaled down version here and use that as source so bitmapdata can be closed\n        // orientation info\n        var exif = item.getMetadata('exif') || {};\n        var orientation = exif.orientation || -1;\n\n        // get width and height from action, and swap if orientation is incorrect\n        var width = imageData.width,\n          height = imageData.height;\n\n        // if no width or height, just return early.\n        if (!width || !height) return;\n\n        if (orientation >= 5 && orientation <= 8) {\n          var _ref7 = [height, width];\n          width = _ref7[0];\n          height = _ref7[1];\n        }\n\n        // scale canvas based on pixel density\n        // we multiply by .75 as that creates smaller but still clear images on screens with high res displays\n        var pixelDensityFactor = Math.max(1, window.devicePixelRatio * 0.75);\n\n        // we want as much pixels to work with as possible,\n        // this multiplies the minimum image resolution,\n        // so when zooming in it doesn't get too blurry\n        var zoomFactor = root.query('GET_IMAGE_PREVIEW_ZOOM_FACTOR');\n\n        // imaeg scale factor\n        var scaleFactor = zoomFactor * pixelDensityFactor;\n\n        // calculate scaled preview image size\n        var previewImageRatio = height / width;\n\n        // calculate image preview height and width\n        var previewContainerWidth = root.rect.element.width;\n        var previewContainerHeight = root.rect.element.height;\n\n        var imageWidth = previewContainerWidth;\n        var imageHeight = imageWidth * previewImageRatio;\n\n        if (previewImageRatio > 1) {\n          imageWidth = Math.min(width, previewContainerWidth * scaleFactor);\n          imageHeight = imageWidth * previewImageRatio;\n        } else {\n          imageHeight = Math.min(height, previewContainerHeight * scaleFactor);\n          imageWidth = imageHeight / previewImageRatio;\n        }\n\n        // transfer to image tag so no canvas memory wasted on iOS\n        var previewImage = createPreviewImage(\n          imageData,\n          imageWidth,\n          imageHeight,\n          orientation\n        );\n\n        // done\n        var done = function done() {\n          // calculate average image color, disabled for now\n          var averageColor = root.query(\n            'GET_IMAGE_PREVIEW_CALCULATE_AVERAGE_IMAGE_COLOR'\n          )\n            ? calculateAverageColor(data)\n            : null;\n          item.setMetadata('color', averageColor, true);\n\n          // data has been transferred to canvas ( if was ImageBitmap )\n          if ('close' in imageData) {\n            imageData.close();\n          }\n\n          // show the overlay\n          root.ref.overlayShadow.opacity = 1;\n\n          // create the first image\n          pushImage({ root: root, props: props, image: previewImage });\n        };\n\n        // apply filter\n        var filter = item.getMetadata('filter');\n        if (filter) {\n          applyFilter(root, filter, previewImage).then(done);\n        } else {\n          done();\n        }\n      };\n\n      // if we support scaling using createImageBitmap we use a worker\n      if (canCreateImageBitmap(item.file)) {\n        // let's scale the image in a worker\n        var worker = createWorker(BitmapWorker);\n\n        worker.post(\n          {\n            file: item.file\n          },\n\n          function(imageBitmap) {\n            // destroy worker\n            worker.terminate();\n\n            // no bitmap returned, must be something wrong,\n            // try the oldschool way\n            if (!imageBitmap) {\n              loadPreviewFallback();\n              return;\n            }\n\n            // yay we got our bitmap, let's continue showing the preview\n            previewImageLoaded(imageBitmap);\n          }\n        );\n      } else {\n        // create fallback preview\n        loadPreviewFallback();\n      }\n    };\n\n    /**\n     * Write handler for when the preview image is ready to be animated\n     */\n    var didDrawPreview = function didDrawPreview(_ref8) {\n      var root = _ref8.root;\n      // get last added image\n      var image = root.ref.images[root.ref.images.length - 1];\n      image.translateY = 0;\n      image.scaleX = 1.0;\n      image.scaleY = 1.0;\n      image.opacity = 1;\n    };\n\n    /**\n     * Write handler for when the preview has been loaded\n     */\n    var restoreOverlay = function restoreOverlay(_ref9) {\n      var root = _ref9.root;\n      root.ref.overlayShadow.opacity = 1;\n      root.ref.overlayError.opacity = 0;\n      root.ref.overlaySuccess.opacity = 0;\n    };\n\n    var didThrowError = function didThrowError(_ref10) {\n      var root = _ref10.root;\n      root.ref.overlayShadow.opacity = 0.25;\n      root.ref.overlayError.opacity = 1;\n    };\n\n    var didCompleteProcessing = function didCompleteProcessing(_ref11) {\n      var root = _ref11.root;\n      root.ref.overlayShadow.opacity = 0.25;\n      root.ref.overlaySuccess.opacity = 1;\n    };\n\n    /**\n     * Constructor\n     */\n    var create = function create(_ref12) {\n      var root = _ref12.root;\n      // image view\n      root.ref.images = [];\n\n      // the preview image data (we need this to filter the image)\n      root.ref.imageData = null;\n\n      // image bin\n      root.ref.imageViewBin = [];\n\n      // image overlays\n      root.ref.overlayShadow = root.appendChildView(\n        root.createChildView(OverlayView, {\n          opacity: 0,\n          status: 'idle'\n        })\n      );\n\n      root.ref.overlaySuccess = root.appendChildView(\n        root.createChildView(OverlayView, {\n          opacity: 0,\n          status: 'success'\n        })\n      );\n\n      root.ref.overlayError = root.appendChildView(\n        root.createChildView(OverlayView, {\n          opacity: 0,\n          status: 'failure'\n        })\n      );\n    };\n\n    return _.utils.createView({\n      name: 'image-preview-wrapper',\n      create: create,\n      styles: ['height'],\n      apis: ['height'],\n      destroy: function destroy(_ref13) {\n        var root = _ref13.root;\n        // we resize the image so memory on iOS 12 is released more quickly (it seems)\n        root.ref.images.forEach(function(imageView) {\n          imageView.image.width = 1;\n          imageView.image.height = 1;\n        });\n      },\n      didWriteView: function didWriteView(_ref14) {\n        var root = _ref14.root;\n        root.ref.images.forEach(function(imageView) {\n          imageView.dirty = false;\n        });\n      },\n      write: _.utils.createRoute(\n        {\n          // image preview stated\n          DID_IMAGE_PREVIEW_DRAW: didDrawPreview,\n          DID_IMAGE_PREVIEW_CONTAINER_CREATE: didCreatePreviewContainer,\n          DID_FINISH_CALCULATE_PREVIEWSIZE: drawPreview,\n          DID_UPDATE_ITEM_METADATA: didUpdateItemMetadata,\n\n          // file states\n          DID_THROW_ITEM_LOAD_ERROR: didThrowError,\n          DID_THROW_ITEM_PROCESSING_ERROR: didThrowError,\n          DID_THROW_ITEM_INVALID: didThrowError,\n          DID_COMPLETE_ITEM_PROCESSING: didCompleteProcessing,\n          DID_START_ITEM_PROCESSING: restoreOverlay,\n          DID_REVERT_ITEM_PROCESSING: restoreOverlay\n        },\n\n        function(_ref15) {\n          var root = _ref15.root;\n          // views on death row\n          var viewsToRemove = root.ref.imageViewBin.filter(function(imageView) {\n            return imageView.opacity === 0;\n          });\n\n          // views to retain\n          root.ref.imageViewBin = root.ref.imageViewBin.filter(function(\n            imageView\n          ) {\n            return imageView.opacity > 0;\n          });\n\n          // remove these views\n          viewsToRemove.forEach(function(imageView) {\n            return removeImageView(root, imageView);\n          });\n          viewsToRemove.length = 0;\n        }\n      )\n    });\n  };\n\n  /**\n   * Image Preview Plugin\n   */\n  var plugin = function plugin(fpAPI) {\n    var addFilter = fpAPI.addFilter,\n      utils = fpAPI.utils;\n    var Type = utils.Type,\n      createRoute = utils.createRoute,\n      isFile = utils.isFile;\n\n    // imagePreviewView\n    var imagePreviewView = createImageWrapperView(fpAPI);\n\n    // called for each view that is created right after the 'create' method\n    addFilter('CREATE_VIEW', function(viewAPI) {\n      // get reference to created view\n      var is = viewAPI.is,\n        view = viewAPI.view,\n        query = viewAPI.query;\n\n      // only hook up to item view and only if is enabled for this cropper\n      if (!is('file') || !query('GET_ALLOW_IMAGE_PREVIEW')) return;\n\n      // create the image preview plugin, but only do so if the item is an image\n      var didLoadItem = function didLoadItem(_ref) {\n        var root = _ref.root,\n          props = _ref.props;\n        var id = props.id;\n        var item = query('GET_ITEM', id);\n\n        // item could theoretically have been removed in the mean time\n        if (!item || !isFile(item.file) || item.archived) return;\n\n        // get the file object\n        var file = item.file;\n\n        // exit if this is not an image\n        if (!isPreviewableImage(file)) return;\n\n        // test if is filtered\n        if (!query('GET_IMAGE_PREVIEW_FILTER_ITEM')(item)) return;\n\n        // exit if image size is too high and no createImageBitmap support\n        // this would simply bring the browser to its knees and that is not what we want\n        var supportsCreateImageBitmap = 'createImageBitmap' in (window || {});\n        var maxPreviewFileSize = query('GET_IMAGE_PREVIEW_MAX_FILE_SIZE');\n        if (\n          !supportsCreateImageBitmap &&\n          maxPreviewFileSize &&\n          file.size > maxPreviewFileSize\n        )\n          return;\n\n        // set preview view\n        root.ref.imagePreview = view.appendChildView(\n          view.createChildView(imagePreviewView, { id: id })\n        );\n\n        // update height if is fixed\n        var fixedPreviewHeight = root.query('GET_IMAGE_PREVIEW_HEIGHT');\n        if (fixedPreviewHeight) {\n          root.dispatch('DID_UPDATE_PANEL_HEIGHT', {\n            id: item.id,\n            height: fixedPreviewHeight\n          });\n        }\n\n        // now ready\n        var queue =\n          !supportsCreateImageBitmap &&\n          file.size > query('GET_IMAGE_PREVIEW_MAX_INSTANT_PREVIEW_FILE_SIZE');\n        root.dispatch('DID_IMAGE_PREVIEW_CONTAINER_CREATE', { id: id }, queue);\n      };\n\n      var rescaleItem = function rescaleItem(root, props) {\n        if (!root.ref.imagePreview) return;\n        var id = props.id;\n\n        // get item\n        var item = root.query('GET_ITEM', { id: id });\n        if (!item) return;\n\n        // if is fixed height or panel has aspect ratio, exit here, height has already been defined\n        var panelAspectRatio = root.query('GET_PANEL_ASPECT_RATIO');\n        var itemPanelAspectRatio = root.query('GET_ITEM_PANEL_ASPECT_RATIO');\n        var fixedHeight = root.query('GET_IMAGE_PREVIEW_HEIGHT');\n        if (panelAspectRatio || itemPanelAspectRatio || fixedHeight) return;\n\n        // no data!\n        var _root$ref = root.ref,\n          imageWidth = _root$ref.imageWidth,\n          imageHeight = _root$ref.imageHeight;\n        if (!imageWidth || !imageHeight) return;\n\n        // get height min and max\n        var minPreviewHeight = root.query('GET_IMAGE_PREVIEW_MIN_HEIGHT');\n        var maxPreviewHeight = root.query('GET_IMAGE_PREVIEW_MAX_HEIGHT');\n\n        // orientation info\n        var exif = item.getMetadata('exif') || {};\n        var orientation = exif.orientation || -1;\n\n        // get width and height from action, and swap of orientation is incorrect\n        if (orientation >= 5 && orientation <= 8) {\n          var _ref2 = [imageHeight, imageWidth];\n          imageWidth = _ref2[0];\n          imageHeight = _ref2[1];\n        }\n\n        // scale up width and height when we're dealing with an SVG\n        if (!isBitmap(item.file) || root.query('GET_IMAGE_PREVIEW_UPSCALE')) {\n          var scalar = 2048 / imageWidth;\n          imageWidth *= scalar;\n          imageHeight *= scalar;\n        }\n\n        // image aspect ratio\n        var imageAspectRatio = imageHeight / imageWidth;\n\n        // we need the item to get to the crop size\n        var previewAspectRatio =\n          (item.getMetadata('crop') || {}).aspectRatio || imageAspectRatio;\n\n        // preview height range\n        var previewHeightMax = Math.max(\n          minPreviewHeight,\n          Math.min(imageHeight, maxPreviewHeight)\n        );\n\n        var itemWidth = root.rect.element.width;\n        var previewHeight = Math.min(\n          itemWidth * previewAspectRatio,\n          previewHeightMax\n        );\n\n        // request update to panel height\n        root.dispatch('DID_UPDATE_PANEL_HEIGHT', {\n          id: item.id,\n          height: previewHeight\n        });\n      };\n\n      var didResizeView = function didResizeView(_ref3) {\n        var root = _ref3.root;\n        // actions in next write operation\n        root.ref.shouldRescale = true;\n      };\n\n      var didUpdateItemMetadata = function didUpdateItemMetadata(_ref4) {\n        var root = _ref4.root,\n          action = _ref4.action;\n        if (action.change.key !== 'crop') return;\n\n        // actions in next write operation\n        root.ref.shouldRescale = true;\n      };\n\n      var didCalculatePreviewSize = function didCalculatePreviewSize(_ref5) {\n        var root = _ref5.root,\n          action = _ref5.action;\n        // remember dimensions\n        root.ref.imageWidth = action.width;\n        root.ref.imageHeight = action.height;\n\n        // actions in next write operation\n        root.ref.shouldRescale = true;\n        root.ref.shouldDrawPreview = true;\n\n        // as image load could take a while and fire when draw loop is resting we need to give it a kick\n        root.dispatch('KICK');\n      };\n\n      // start writing\n      view.registerWriter(\n        createRoute(\n          {\n            DID_RESIZE_ROOT: didResizeView,\n            DID_STOP_RESIZE: didResizeView,\n            DID_LOAD_ITEM: didLoadItem,\n            DID_IMAGE_PREVIEW_CALCULATE_SIZE: didCalculatePreviewSize,\n            DID_UPDATE_ITEM_METADATA: didUpdateItemMetadata\n          },\n\n          function(_ref6) {\n            var root = _ref6.root,\n              props = _ref6.props;\n            // no preview view attached\n            if (!root.ref.imagePreview) return;\n\n            // don't do anything while hidden\n            if (root.rect.element.hidden) return;\n\n            // resize the item panel\n            if (root.ref.shouldRescale) {\n              rescaleItem(root, props);\n              root.ref.shouldRescale = false;\n            }\n\n            if (root.ref.shouldDrawPreview) {\n              // queue till next frame so we're sure the height has been applied this forces the draw image call inside the wrapper view to use the correct height\n              requestAnimationFrame(function() {\n                // this requestAnimationFrame nesting is horrible but it fixes an issue with 100hz displays on Chrome\n                // https://github.com/pqina/filepond-plugin-image-preview/issues/57\n                requestAnimationFrame(function() {\n                  root.dispatch('DID_FINISH_CALCULATE_PREVIEWSIZE', {\n                    id: props.id\n                  });\n                });\n              });\n\n              root.ref.shouldDrawPreview = false;\n            }\n          }\n        )\n      );\n    });\n\n    // expose plugin\n    return {\n      options: {\n        // Enable or disable image preview\n        allowImagePreview: [true, Type.BOOLEAN],\n\n        // filters file items to determine which are shown as preview\n        imagePreviewFilterItem: [\n          function() {\n            return true;\n          },\n          Type.FUNCTION\n        ],\n\n        // Fixed preview height\n        imagePreviewHeight: [null, Type.INT],\n\n        // Min image height\n        imagePreviewMinHeight: [44, Type.INT],\n\n        // Max image height\n        imagePreviewMaxHeight: [256, Type.INT],\n\n        // Max size of preview file for when createImageBitmap is not supported\n        imagePreviewMaxFileSize: [null, Type.INT],\n\n        // The amount of extra pixels added to the image preview to allow comfortable zooming\n        imagePreviewZoomFactor: [2, Type.INT],\n\n        // Should we upscale small images to fit the max bounding box of the preview area\n        imagePreviewUpscale: [false, Type.BOOLEAN],\n\n        // Max size of preview file that we allow to try to instant preview if createImageBitmap is not supported, else image is queued for loading\n        imagePreviewMaxInstantPreviewFileSize: [1000000, Type.INT],\n\n        // Style of the transparancy indicator used behind images\n        imagePreviewTransparencyIndicator: [null, Type.STRING],\n\n        // Enables or disables reading average image color\n        imagePreviewCalculateAverageImageColor: [false, Type.BOOLEAN],\n\n        // Enables or disables the previewing of markup\n        imagePreviewMarkupShow: [true, Type.BOOLEAN],\n\n        // Allows filtering of markup to only show certain shapes\n        imagePreviewMarkupFilter: [\n          function() {\n            return true;\n          },\n          Type.FUNCTION\n        ]\n      }\n    };\n  };\n\n  // fire pluginloaded event if running in browser, this allows registering the plugin when using async script tags\n  var isBrowser =\n    typeof window !== 'undefined' && typeof window.document !== 'undefined';\n  if (isBrowser) {\n    document.dispatchEvent(\n      new CustomEvent('FilePond:pluginloaded', { detail: plugin })\n    );\n  }\n\n  return plugin;\n});\n",
         "/*!\n * FilePondPluginFileValidateSize 2.2.5\n * Licensed under MIT, https://opensource.org/licenses/MIT/\n * Please visit https://pqina.nl/filepond/ for details.\n */\n\n/* eslint-disable */\n\n(function(global, factory) {\n    typeof exports === 'object' && typeof module !== 'undefined'\n        ? (module.exports = factory())\n        : typeof define === 'function' && define.amd\n        ? define(factory)\n        : ((global = global || self), (global.FilePondPluginFileValidateSize = factory()));\n})(this, function() {\n    'use strict';\n\n    var plugin = function plugin(_ref) {\n        var addFilter = _ref.addFilter,\n            utils = _ref.utils;\n        // get quick reference to Type utils\n        var Type = utils.Type,\n            replaceInString = utils.replaceInString,\n            toNaturalFileSize = utils.toNaturalFileSize;\n\n        // filtering if an item is allowed in hopper\n        addFilter('ALLOW_HOPPER_ITEM', function(file, _ref2) {\n            var query = _ref2.query;\n            if (!query('GET_ALLOW_FILE_SIZE_VALIDATION')) {\n                return true;\n            }\n\n            var sizeMax = query('GET_MAX_FILE_SIZE');\n            if (sizeMax !== null && file.size >= sizeMax) {\n                return false;\n            }\n\n            var sizeMin = query('GET_MIN_FILE_SIZE');\n            if (sizeMin !== null && file.size <= sizeMin) {\n                return false;\n            }\n\n            return true;\n        });\n\n        // called for each file that is loaded\n        // right before it is set to the item state\n        // should return a promise\n        addFilter('LOAD_FILE', function(file, _ref3) {\n            var query = _ref3.query;\n            return new Promise(function(resolve, reject) {\n                // if not allowed, all fine, exit\n                if (!query('GET_ALLOW_FILE_SIZE_VALIDATION')) {\n                    return resolve(file);\n                }\n\n                // check if file should be filtered\n                var fileFilter = query('GET_FILE_VALIDATE_SIZE_FILTER');\n                if (fileFilter && !fileFilter(file)) {\n                    return resolve(file);\n                }\n\n                // reject or resolve based on file size\n                var sizeMax = query('GET_MAX_FILE_SIZE');\n                if (sizeMax !== null && file.size >= sizeMax) {\n                    reject({\n                        status: {\n                            main: query('GET_LABEL_MAX_FILE_SIZE_EXCEEDED'),\n                            sub: replaceInString(query('GET_LABEL_MAX_FILE_SIZE'), {\n                                filesize: toNaturalFileSize(\n                                    sizeMax,\n                                    '.',\n                                    query('GET_FILE_SIZE_BASE'),\n                                    query('GET_FILE_SIZE_LABELS', query)\n                                ),\n                            }),\n                        },\n                    });\n\n                    return;\n                }\n\n                // reject or resolve based on file size\n                var sizeMin = query('GET_MIN_FILE_SIZE');\n                if (sizeMin !== null && file.size <= sizeMin) {\n                    reject({\n                        status: {\n                            main: query('GET_LABEL_MIN_FILE_SIZE_EXCEEDED'),\n                            sub: replaceInString(query('GET_LABEL_MIN_FILE_SIZE'), {\n                                filesize: toNaturalFileSize(\n                                    sizeMin,\n                                    '.',\n                                    query('GET_FILE_SIZE_BASE'),\n                                    query('GET_FILE_SIZE_LABELS', query)\n                                ),\n                            }),\n                        },\n                    });\n\n                    return;\n                }\n\n                // returns the current option value\n                var totalSizeMax = query('GET_MAX_TOTAL_FILE_SIZE');\n                if (totalSizeMax !== null) {\n                    // get the current total file size\n                    var currentTotalSize = query('GET_ACTIVE_ITEMS').reduce(function(total, item) {\n                        return total + item.fileSize;\n                    }, 0);\n\n                    // get the size of the new file\n                    if (currentTotalSize > totalSizeMax) {\n                        reject({\n                            status: {\n                                main: query('GET_LABEL_MAX_TOTAL_FILE_SIZE_EXCEEDED'),\n                                sub: replaceInString(query('GET_LABEL_MAX_TOTAL_FILE_SIZE'), {\n                                    filesize: toNaturalFileSize(\n                                        totalSizeMax,\n                                        '.',\n                                        query('GET_FILE_SIZE_BASE'),\n                                        query('GET_FILE_SIZE_LABELS', query)\n                                    ),\n                                }),\n                            },\n                        });\n\n                        return;\n                    }\n                }\n\n                // file is fine, let's pass it back\n                resolve(file);\n            });\n        });\n\n        return {\n            options: {\n                // Enable or disable file type validation\n                allowFileSizeValidation: [true, Type.BOOLEAN],\n\n                // Max individual file size in bytes\n                maxFileSize: [null, Type.INT],\n\n                // Min individual file size in bytes\n                minFileSize: [null, Type.INT],\n\n                // Max total file size in bytes\n                maxTotalFileSize: [null, Type.INT],\n\n                // Filter the files that need to be validated for size\n                fileValidateSizeFilter: [null, Type.FUNCTION],\n\n                // error labels\n                labelMinFileSizeExceeded: ['File is too small', Type.STRING],\n                labelMinFileSize: ['Minimum file size is {filesize}', Type.STRING],\n\n                labelMaxFileSizeExceeded: ['File is too large', Type.STRING],\n                labelMaxFileSize: ['Maximum file size is {filesize}', Type.STRING],\n\n                labelMaxTotalFileSizeExceeded: ['Maximum total size exceeded', Type.STRING],\n                labelMaxTotalFileSize: ['Maximum total file size is {filesize}', Type.STRING],\n            },\n        };\n    };\n\n    // fire pluginloaded event if running in browser, this allows registering the plugin when using async script tags\n    var isBrowser = typeof window !== 'undefined' && typeof window.document !== 'undefined';\n    if (isBrowser) {\n        document.dispatchEvent(new CustomEvent('FilePond:pluginloaded', { detail: plugin }));\n    }\n\n    return plugin;\n});\n",
         "/*!\n * Determine if an object is a Buffer\n *\n * @author   Feross Aboukhadijeh <https://feross.org>\n * @license  MIT\n */\n\nmodule.exports = function isBuffer (obj) {\n  return obj != null && obj.constructor != null &&\n    typeof obj.constructor.isBuffer === 'function' && obj.constructor.isBuffer(obj)\n}\n",
         "/*!\n * Determine if an object is a Buffer\n *\n * @author   Feross Aboukhadijeh <https://feross.org>\n * @license  MIT\n */\n\nmodule.exports = function isBuffer (obj) {\n  return obj != null && obj.constructor != null &&\n    typeof obj.constructor.isBuffer === 'function' && obj.constructor.isBuffer(obj)\n}\n",
         "'use strict';\n\nif (process.env.NODE_ENV === 'production') {\n  module.exports = require('./cjs/react-is.production.min.js');\n} else {\n  module.exports = require('./cjs/react-is.development.js');\n}\n",
         "/*\nLanguage: C++\nCategory: common, system\nWebsite: https://isocpp.org\n*/\n\n/** @type LanguageFn */\nfunction cPlusPlus(hljs) {\n  const regex = hljs.regex;\n  // added for historic reasons because `hljs.C_LINE_COMMENT_MODE` does\n  // not include such support nor can we be sure all the grammars depending\n  // on it would desire this behavior\n  const C_LINE_COMMENT_MODE = hljs.COMMENT('//', '$', {\n    contains: [\n      {\n        begin: /\\\\\\n/\n      }\n    ]\n  });\n  const DECLTYPE_AUTO_RE = 'decltype\\\\(auto\\\\)';\n  const NAMESPACE_RE = '[a-zA-Z_]\\\\w*::';\n  const TEMPLATE_ARGUMENT_RE = '<[^<>]+>';\n  const FUNCTION_TYPE_RE = '(?!struct)(' +\n    DECLTYPE_AUTO_RE + '|' +\n    regex.optional(NAMESPACE_RE) +\n    '[a-zA-Z_]\\\\w*' + regex.optional(TEMPLATE_ARGUMENT_RE) +\n  ')';\n\n  const CPP_PRIMITIVE_TYPES = {\n    className: 'type',\n    begin: '\\\\b[a-z\\\\d_]*_t\\\\b'\n  };\n\n  // https://en.cppreference.com/w/cpp/language/escape\n  // \\\\ \\x \\xFF \\u2837 \\u00323747 \\374\n  const CHARACTER_ESCAPES = '\\\\\\\\(x[0-9A-Fa-f]{2}|u[0-9A-Fa-f]{4,8}|[0-7]{3}|\\\\S)';\n  const STRINGS = {\n    className: 'string',\n    variants: [\n      {\n        begin: '(u8?|U|L)?\"',\n        end: '\"',\n        illegal: '\\\\n',\n        contains: [ hljs.BACKSLASH_ESCAPE ]\n      },\n      {\n        begin: '(u8?|U|L)?\\'(' + CHARACTER_ESCAPES + '|.)',\n        end: '\\'',\n        illegal: '.'\n      },\n      hljs.END_SAME_AS_BEGIN({\n        begin: /(?:u8?|U|L)?R\"([^()\\\\ ]{0,16})\\(/,\n        end: /\\)([^()\\\\ ]{0,16})\"/\n      })\n    ]\n  };\n\n  const NUMBERS = {\n    className: 'number',\n    variants: [\n      {\n        begin: '\\\\b(0b[01\\']+)'\n      },\n      {\n        begin: '(-?)\\\\b([\\\\d\\']+(\\\\.[\\\\d\\']*)?|\\\\.[\\\\d\\']+)((ll|LL|l|L)(u|U)?|(u|U)(ll|LL|l|L)?|f|F|b|B)'\n      },\n      {\n        begin: '(-?)(\\\\b0[xX][a-fA-F0-9\\']+|(\\\\b[\\\\d\\']+(\\\\.[\\\\d\\']*)?|\\\\.[\\\\d\\']+)([eE][-+]?[\\\\d\\']+)?)'\n      }\n    ],\n    relevance: 0\n  };\n\n  const PREPROCESSOR = {\n    className: 'meta',\n    begin: /#\\s*[a-z]+\\b/,\n    end: /$/,\n    keywords: {\n      keyword:\n        'if else elif endif define undef warning error line ' +\n        'pragma _Pragma ifdef ifndef include'\n    },\n    contains: [\n      {\n        begin: /\\\\\\n/,\n        relevance: 0\n      },\n      hljs.inherit(STRINGS, {\n        className: 'string'\n      }),\n      {\n        className: 'string',\n        begin: /<.*?>/\n      },\n      C_LINE_COMMENT_MODE,\n      hljs.C_BLOCK_COMMENT_MODE\n    ]\n  };\n\n  const TITLE_MODE = {\n    className: 'title',\n    begin: regex.optional(NAMESPACE_RE) + hljs.IDENT_RE,\n    relevance: 0\n  };\n\n  const FUNCTION_TITLE = regex.optional(NAMESPACE_RE) + hljs.IDENT_RE + '\\\\s*\\\\(';\n\n  // https://en.cppreference.com/w/cpp/keyword\n  const RESERVED_KEYWORDS = [\n    'alignas',\n    'alignof',\n    'and',\n    'and_eq',\n    'asm',\n    'atomic_cancel',\n    'atomic_commit',\n    'atomic_noexcept',\n    'auto',\n    'bitand',\n    'bitor',\n    'break',\n    'case',\n    'catch',\n    'class',\n    'co_await',\n    'co_return',\n    'co_yield',\n    'compl',\n    'concept',\n    'const_cast|10',\n    'consteval',\n    'constexpr',\n    'constinit',\n    'continue',\n    'decltype',\n    'default',\n    'delete',\n    'do',\n    'dynamic_cast|10',\n    'else',\n    'enum',\n    'explicit',\n    'export',\n    'extern',\n    'false',\n    'final',\n    'for',\n    'friend',\n    'goto',\n    'if',\n    'import',\n    'inline',\n    'module',\n    'mutable',\n    'namespace',\n    'new',\n    'noexcept',\n    'not',\n    'not_eq',\n    'nullptr',\n    'operator',\n    'or',\n    'or_eq',\n    'override',\n    'private',\n    'protected',\n    'public',\n    'reflexpr',\n    'register',\n    'reinterpret_cast|10',\n    'requires',\n    'return',\n    'sizeof',\n    'static_assert',\n    'static_cast|10',\n    'struct',\n    'switch',\n    'synchronized',\n    'template',\n    'this',\n    'thread_local',\n    'throw',\n    'transaction_safe',\n    'transaction_safe_dynamic',\n    'true',\n    'try',\n    'typedef',\n    'typeid',\n    'typename',\n    'union',\n    'using',\n    'virtual',\n    'volatile',\n    'while',\n    'xor',\n    'xor_eq'\n  ];\n\n  // https://en.cppreference.com/w/cpp/keyword\n  const RESERVED_TYPES = [\n    'bool',\n    'char',\n    'char16_t',\n    'char32_t',\n    'char8_t',\n    'double',\n    'float',\n    'int',\n    'long',\n    'short',\n    'void',\n    'wchar_t',\n    'unsigned',\n    'signed',\n    'const',\n    'static'\n  ];\n\n  const TYPE_HINTS = [\n    'any',\n    'auto_ptr',\n    'barrier',\n    'binary_semaphore',\n    'bitset',\n    'complex',\n    'condition_variable',\n    'condition_variable_any',\n    'counting_semaphore',\n    'deque',\n    'false_type',\n    'future',\n    'imaginary',\n    'initializer_list',\n    'istringstream',\n    'jthread',\n    'latch',\n    'lock_guard',\n    'multimap',\n    'multiset',\n    'mutex',\n    'optional',\n    'ostringstream',\n    'packaged_task',\n    'pair',\n    'promise',\n    'priority_queue',\n    'queue',\n    'recursive_mutex',\n    'recursive_timed_mutex',\n    'scoped_lock',\n    'set',\n    'shared_future',\n    'shared_lock',\n    'shared_mutex',\n    'shared_timed_mutex',\n    'shared_ptr',\n    'stack',\n    'string_view',\n    'stringstream',\n    'timed_mutex',\n    'thread',\n    'true_type',\n    'tuple',\n    'unique_lock',\n    'unique_ptr',\n    'unordered_map',\n    'unordered_multimap',\n    'unordered_multiset',\n    'unordered_set',\n    'variant',\n    'vector',\n    'weak_ptr',\n    'wstring',\n    'wstring_view'\n  ];\n\n  const FUNCTION_HINTS = [\n    'abort',\n    'abs',\n    'acos',\n    'apply',\n    'as_const',\n    'asin',\n    'atan',\n    'atan2',\n    'calloc',\n    'ceil',\n    'cerr',\n    'cin',\n    'clog',\n    'cos',\n    'cosh',\n    'cout',\n    'declval',\n    'endl',\n    'exchange',\n    'exit',\n    'exp',\n    'fabs',\n    'floor',\n    'fmod',\n    'forward',\n    'fprintf',\n    'fputs',\n    'free',\n    'frexp',\n    'fscanf',\n    'future',\n    'invoke',\n    'isalnum',\n    'isalpha',\n    'iscntrl',\n    'isdigit',\n    'isgraph',\n    'islower',\n    'isprint',\n    'ispunct',\n    'isspace',\n    'isupper',\n    'isxdigit',\n    'labs',\n    'launder',\n    'ldexp',\n    'log',\n    'log10',\n    'make_pair',\n    'make_shared',\n    'make_shared_for_overwrite',\n    'make_tuple',\n    'make_unique',\n    'malloc',\n    'memchr',\n    'memcmp',\n    'memcpy',\n    'memset',\n    'modf',\n    'move',\n    'pow',\n    'printf',\n    'putchar',\n    'puts',\n    'realloc',\n    'scanf',\n    'sin',\n    'sinh',\n    'snprintf',\n    'sprintf',\n    'sqrt',\n    'sscanf',\n    'std',\n    'stderr',\n    'stdin',\n    'stdout',\n    'strcat',\n    'strchr',\n    'strcmp',\n    'strcpy',\n    'strcspn',\n    'strlen',\n    'strncat',\n    'strncmp',\n    'strncpy',\n    'strpbrk',\n    'strrchr',\n    'strspn',\n    'strstr',\n    'swap',\n    'tan',\n    'tanh',\n    'terminate',\n    'to_underlying',\n    'tolower',\n    'toupper',\n    'vfprintf',\n    'visit',\n    'vprintf',\n    'vsprintf'\n  ];\n\n  const LITERALS = [\n    'NULL',\n    'false',\n    'nullopt',\n    'nullptr',\n    'true'\n  ];\n\n  // https://en.cppreference.com/w/cpp/keyword\n  const BUILT_IN = [\n    '_Pragma'\n  ];\n\n  const CPP_KEYWORDS = {\n    type: RESERVED_TYPES,\n    keyword: RESERVED_KEYWORDS,\n    literal: LITERALS,\n    built_in: BUILT_IN,\n    _type_hints: TYPE_HINTS\n  };\n\n  const FUNCTION_DISPATCH = {\n    className: 'function.dispatch',\n    relevance: 0,\n    keywords: {\n      // Only for relevance, not highlighting.\n      _hint: FUNCTION_HINTS\n    },\n    begin: regex.concat(\n      /\\b/,\n      /(?!decltype)/,\n      /(?!if)/,\n      /(?!for)/,\n      /(?!switch)/,\n      /(?!while)/,\n      hljs.IDENT_RE,\n      regex.lookahead(/(<[^<>]+>|)\\s*\\(/))\n  };\n\n  const EXPRESSION_CONTAINS = [\n    FUNCTION_DISPATCH,\n    PREPROCESSOR,\n    CPP_PRIMITIVE_TYPES,\n    C_LINE_COMMENT_MODE,\n    hljs.C_BLOCK_COMMENT_MODE,\n    NUMBERS,\n    STRINGS\n  ];\n\n  const EXPRESSION_CONTEXT = {\n    // This mode covers expression context where we can't expect a function\n    // definition and shouldn't highlight anything that looks like one:\n    // `return some()`, `else if()`, `(x*sum(1, 2))`\n    variants: [\n      {\n        begin: /=/,\n        end: /;/\n      },\n      {\n        begin: /\\(/,\n        end: /\\)/\n      },\n      {\n        beginKeywords: 'new throw return else',\n        end: /;/\n      }\n    ],\n    keywords: CPP_KEYWORDS,\n    contains: EXPRESSION_CONTAINS.concat([\n      {\n        begin: /\\(/,\n        end: /\\)/,\n        keywords: CPP_KEYWORDS,\n        contains: EXPRESSION_CONTAINS.concat([ 'self' ]),\n        relevance: 0\n      }\n    ]),\n    relevance: 0\n  };\n\n  const FUNCTION_DECLARATION = {\n    className: 'function',\n    begin: '(' + FUNCTION_TYPE_RE + '[\\\\*&\\\\s]+)+' + FUNCTION_TITLE,\n    returnBegin: true,\n    end: /[{;=]/,\n    excludeEnd: true,\n    keywords: CPP_KEYWORDS,\n    illegal: /[^\\w\\s\\*&:<>.]/,\n    contains: [\n      { // to prevent it from being confused as the function title\n        begin: DECLTYPE_AUTO_RE,\n        keywords: CPP_KEYWORDS,\n        relevance: 0\n      },\n      {\n        begin: FUNCTION_TITLE,\n        returnBegin: true,\n        contains: [ TITLE_MODE ],\n        relevance: 0\n      },\n      // needed because we do not have look-behind on the below rule\n      // to prevent it from grabbing the final : in a :: pair\n      {\n        begin: /::/,\n        relevance: 0\n      },\n      // initializers\n      {\n        begin: /:/,\n        endsWithParent: true,\n        contains: [\n          STRINGS,\n          NUMBERS\n        ]\n      },\n      // allow for multiple declarations, e.g.:\n      // extern void f(int), g(char);\n      {\n        relevance: 0,\n        match: /,/\n      },\n      {\n        className: 'params',\n        begin: /\\(/,\n        end: /\\)/,\n        keywords: CPP_KEYWORDS,\n        relevance: 0,\n        contains: [\n          C_LINE_COMMENT_MODE,\n          hljs.C_BLOCK_COMMENT_MODE,\n          STRINGS,\n          NUMBERS,\n          CPP_PRIMITIVE_TYPES,\n          // Count matching parentheses.\n          {\n            begin: /\\(/,\n            end: /\\)/,\n            keywords: CPP_KEYWORDS,\n            relevance: 0,\n            contains: [\n              'self',\n              C_LINE_COMMENT_MODE,\n              hljs.C_BLOCK_COMMENT_MODE,\n              STRINGS,\n              NUMBERS,\n              CPP_PRIMITIVE_TYPES\n            ]\n          }\n        ]\n      },\n      CPP_PRIMITIVE_TYPES,\n      C_LINE_COMMENT_MODE,\n      hljs.C_BLOCK_COMMENT_MODE,\n      PREPROCESSOR\n    ]\n  };\n\n  return {\n    name: 'C++',\n    aliases: [\n      'cc',\n      'c++',\n      'h++',\n      'hpp',\n      'hh',\n      'hxx',\n      'cxx'\n    ],\n    keywords: CPP_KEYWORDS,\n    illegal: '</',\n    classNameAliases: {\n      'function.dispatch': 'built_in'\n    },\n    contains: [].concat(\n      EXPRESSION_CONTEXT,\n      FUNCTION_DECLARATION,\n      FUNCTION_DISPATCH,\n      EXPRESSION_CONTAINS,\n      [\n        PREPROCESSOR,\n        { // containers: ie, `vector <int> rooms (9);`\n          begin: '\\\\b(deque|list|queue|priority_queue|pair|stack|vector|map|set|bitset|multiset|multimap|unordered_map|unordered_set|unordered_multiset|unordered_multimap|array|tuple|optional|variant|function)\\\\s*<(?!<)',\n          end: '>',\n          keywords: CPP_KEYWORDS,\n          contains: [\n            'self',\n            CPP_PRIMITIVE_TYPES\n          ]\n        },\n        {\n          begin: hljs.IDENT_RE + '::',\n          keywords: CPP_KEYWORDS\n        },\n        {\n          match: [\n            // extra complexity to deal with `enum class` and `enum struct`\n            /\\b(?:enum(?:\\s+(?:class|struct))?|class|struct|union)/,\n            /\\s+/,\n            /\\w+/\n          ],\n          className: {\n            1: 'keyword',\n            3: 'title.class'\n          }\n        }\n      ])\n  };\n}\n\n/*\nLanguage: Arduino\nAuthor: Stefania Mellai <s.mellai@arduino.cc>\nDescription: The Arduino\u00ae Language is a superset of C++. This rules are designed to highlight the Arduino\u00ae source code. For info about language see http://www.arduino.cc.\nWebsite: https://www.arduino.cc\n*/\n\n/** @type LanguageFn */\nfunction arduino(hljs) {\n  const ARDUINO_KW = {\n    type: [\n      \"boolean\",\n      \"byte\",\n      \"word\",\n      \"String\"\n    ],\n    built_in: [\n      \"KeyboardController\",\n      \"MouseController\",\n      \"SoftwareSerial\",\n      \"EthernetServer\",\n      \"EthernetClient\",\n      \"LiquidCrystal\",\n      \"RobotControl\",\n      \"GSMVoiceCall\",\n      \"EthernetUDP\",\n      \"EsploraTFT\",\n      \"HttpClient\",\n      \"RobotMotor\",\n      \"WiFiClient\",\n      \"GSMScanner\",\n      \"FileSystem\",\n      \"Scheduler\",\n      \"GSMServer\",\n      \"YunClient\",\n      \"YunServer\",\n      \"IPAddress\",\n      \"GSMClient\",\n      \"GSMModem\",\n      \"Keyboard\",\n      \"Ethernet\",\n      \"Console\",\n      \"GSMBand\",\n      \"Esplora\",\n      \"Stepper\",\n      \"Process\",\n      \"WiFiUDP\",\n      \"GSM_SMS\",\n      \"Mailbox\",\n      \"USBHost\",\n      \"Firmata\",\n      \"PImage\",\n      \"Client\",\n      \"Server\",\n      \"GSMPIN\",\n      \"FileIO\",\n      \"Bridge\",\n      \"Serial\",\n      \"EEPROM\",\n      \"Stream\",\n      \"Mouse\",\n      \"Audio\",\n      \"Servo\",\n      \"File\",\n      \"Task\",\n      \"GPRS\",\n      \"WiFi\",\n      \"Wire\",\n      \"TFT\",\n      \"GSM\",\n      \"SPI\",\n      \"SD\"\n    ],\n    _hints: [\n      \"setup\",\n      \"loop\",\n      \"runShellCommandAsynchronously\",\n      \"analogWriteResolution\",\n      \"retrieveCallingNumber\",\n      \"printFirmwareVersion\",\n      \"analogReadResolution\",\n      \"sendDigitalPortPair\",\n      \"noListenOnLocalhost\",\n      \"readJoystickButton\",\n      \"setFirmwareVersion\",\n      \"readJoystickSwitch\",\n      \"scrollDisplayRight\",\n      \"getVoiceCallStatus\",\n      \"scrollDisplayLeft\",\n      \"writeMicroseconds\",\n      \"delayMicroseconds\",\n      \"beginTransmission\",\n      \"getSignalStrength\",\n      \"runAsynchronously\",\n      \"getAsynchronously\",\n      \"listenOnLocalhost\",\n      \"getCurrentCarrier\",\n      \"readAccelerometer\",\n      \"messageAvailable\",\n      \"sendDigitalPorts\",\n      \"lineFollowConfig\",\n      \"countryNameWrite\",\n      \"runShellCommand\",\n      \"readStringUntil\",\n      \"rewindDirectory\",\n      \"readTemperature\",\n      \"setClockDivider\",\n      \"readLightSensor\",\n      \"endTransmission\",\n      \"analogReference\",\n      \"detachInterrupt\",\n      \"countryNameRead\",\n      \"attachInterrupt\",\n      \"encryptionType\",\n      \"readBytesUntil\",\n      \"robotNameWrite\",\n      \"readMicrophone\",\n      \"robotNameRead\",\n      \"cityNameWrite\",\n      \"userNameWrite\",\n      \"readJoystickY\",\n      \"readJoystickX\",\n      \"mouseReleased\",\n      \"openNextFile\",\n      \"scanNetworks\",\n      \"noInterrupts\",\n      \"digitalWrite\",\n      \"beginSpeaker\",\n      \"mousePressed\",\n      \"isActionDone\",\n      \"mouseDragged\",\n      \"displayLogos\",\n      \"noAutoscroll\",\n      \"addParameter\",\n      \"remoteNumber\",\n      \"getModifiers\",\n      \"keyboardRead\",\n      \"userNameRead\",\n      \"waitContinue\",\n      \"processInput\",\n      \"parseCommand\",\n      \"printVersion\",\n      \"readNetworks\",\n      \"writeMessage\",\n      \"blinkVersion\",\n      \"cityNameRead\",\n      \"readMessage\",\n      \"setDataMode\",\n      \"parsePacket\",\n      \"isListening\",\n      \"setBitOrder\",\n      \"beginPacket\",\n      \"isDirectory\",\n      \"motorsWrite\",\n      \"drawCompass\",\n      \"digitalRead\",\n      \"clearScreen\",\n      \"serialEvent\",\n      \"rightToLeft\",\n      \"setTextSize\",\n      \"leftToRight\",\n      \"requestFrom\",\n      \"keyReleased\",\n      \"compassRead\",\n      \"analogWrite\",\n      \"interrupts\",\n      \"WiFiServer\",\n      \"disconnect\",\n      \"playMelody\",\n      \"parseFloat\",\n      \"autoscroll\",\n      \"getPINUsed\",\n      \"setPINUsed\",\n      \"setTimeout\",\n      \"sendAnalog\",\n      \"readSlider\",\n      \"analogRead\",\n      \"beginWrite\",\n      \"createChar\",\n      \"motorsStop\",\n      \"keyPressed\",\n      \"tempoWrite\",\n      \"readButton\",\n      \"subnetMask\",\n      \"debugPrint\",\n      \"macAddress\",\n      \"writeGreen\",\n      \"randomSeed\",\n      \"attachGPRS\",\n      \"readString\",\n      \"sendString\",\n      \"remotePort\",\n      \"releaseAll\",\n      \"mouseMoved\",\n      \"background\",\n      \"getXChange\",\n      \"getYChange\",\n      \"answerCall\",\n      \"getResult\",\n      \"voiceCall\",\n      \"endPacket\",\n      \"constrain\",\n      \"getSocket\",\n      \"writeJSON\",\n      \"getButton\",\n      \"available\",\n      \"connected\",\n      \"findUntil\",\n      \"readBytes\",\n      \"exitValue\",\n      \"readGreen\",\n      \"writeBlue\",\n      \"startLoop\",\n      \"IPAddress\",\n      \"isPressed\",\n      \"sendSysex\",\n      \"pauseMode\",\n      \"gatewayIP\",\n      \"setCursor\",\n      \"getOemKey\",\n      \"tuneWrite\",\n      \"noDisplay\",\n      \"loadImage\",\n      \"switchPIN\",\n      \"onRequest\",\n      \"onReceive\",\n      \"changePIN\",\n      \"playFile\",\n      \"noBuffer\",\n      \"parseInt\",\n      \"overflow\",\n      \"checkPIN\",\n      \"knobRead\",\n      \"beginTFT\",\n      \"bitClear\",\n      \"updateIR\",\n      \"bitWrite\",\n      \"position\",\n      \"writeRGB\",\n      \"highByte\",\n      \"writeRed\",\n      \"setSpeed\",\n      \"readBlue\",\n      \"noStroke\",\n      \"remoteIP\",\n      \"transfer\",\n      \"shutdown\",\n      \"hangCall\",\n      \"beginSMS\",\n      \"endWrite\",\n      \"attached\",\n      \"maintain\",\n      \"noCursor\",\n      \"checkReg\",\n      \"checkPUK\",\n      \"shiftOut\",\n      \"isValid\",\n      \"shiftIn\",\n      \"pulseIn\",\n      \"connect\",\n      \"println\",\n      \"localIP\",\n      \"pinMode\",\n      \"getIMEI\",\n      \"display\",\n      \"noBlink\",\n      \"process\",\n      \"getBand\",\n      \"running\",\n      \"beginSD\",\n      \"drawBMP\",\n      \"lowByte\",\n      \"setBand\",\n      \"release\",\n      \"bitRead\",\n      \"prepare\",\n      \"pointTo\",\n      \"readRed\",\n      \"setMode\",\n      \"noFill\",\n      \"remove\",\n      \"listen\",\n      \"stroke\",\n      \"detach\",\n      \"attach\",\n      \"noTone\",\n      \"exists\",\n      \"buffer\",\n      \"height\",\n      \"bitSet\",\n      \"circle\",\n      \"config\",\n      \"cursor\",\n      \"random\",\n      \"IRread\",\n      \"setDNS\",\n      \"endSMS\",\n      \"getKey\",\n      \"micros\",\n      \"millis\",\n      \"begin\",\n      \"print\",\n      \"write\",\n      \"ready\",\n      \"flush\",\n      \"width\",\n      \"isPIN\",\n      \"blink\",\n      \"clear\",\n      \"press\",\n      \"mkdir\",\n      \"rmdir\",\n      \"close\",\n      \"point\",\n      \"yield\",\n      \"image\",\n      \"BSSID\",\n      \"click\",\n      \"delay\",\n      \"read\",\n      \"text\",\n      \"move\",\n      \"peek\",\n      \"beep\",\n      \"rect\",\n      \"line\",\n      \"open\",\n      \"seek\",\n      \"fill\",\n      \"size\",\n      \"turn\",\n      \"stop\",\n      \"home\",\n      \"find\",\n      \"step\",\n      \"tone\",\n      \"sqrt\",\n      \"RSSI\",\n      \"SSID\",\n      \"end\",\n      \"bit\",\n      \"tan\",\n      \"cos\",\n      \"sin\",\n      \"pow\",\n      \"map\",\n      \"abs\",\n      \"max\",\n      \"min\",\n      \"get\",\n      \"run\",\n      \"put\"\n    ],\n    literal: [\n      \"DIGITAL_MESSAGE\",\n      \"FIRMATA_STRING\",\n      \"ANALOG_MESSAGE\",\n      \"REPORT_DIGITAL\",\n      \"REPORT_ANALOG\",\n      \"INPUT_PULLUP\",\n      \"SET_PIN_MODE\",\n      \"INTERNAL2V56\",\n      \"SYSTEM_RESET\",\n      \"LED_BUILTIN\",\n      \"INTERNAL1V1\",\n      \"SYSEX_START\",\n      \"INTERNAL\",\n      \"EXTERNAL\",\n      \"DEFAULT\",\n      \"OUTPUT\",\n      \"INPUT\",\n      \"HIGH\",\n      \"LOW\"\n    ]\n  };\n\n  const ARDUINO = cPlusPlus(hljs);\n\n  const kws = /** @type {Record<string,any>} */ (ARDUINO.keywords);\n\n  kws.type = [ ...kws.type, ...ARDUINO_KW.type ];\n  kws.literal = [ ...kws.literal, ...ARDUINO_KW.literal ];\n  kws.built_in = [ ...kws.built_in, ...ARDUINO_KW.built_in ];\n  kws._hints = ARDUINO_KW._hints;\n\n  ARDUINO.name = 'Arduino';\n  ARDUINO.aliases = ['ino'];\n  ARDUINO.supersetOf = \"cpp\";\n\n  return ARDUINO;\n}\n\nmodule.exports = arduino;\n",
```

### Comparing `mercury-2.2.1/mercury/frontend-dist/static/js/main.717ee96a.chunk.js` & `mercury-2.2.2/mercury/frontend-dist/static/js/main.2749a4f6.chunk.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -12,20 +12,21 @@
                 r = a(11),
                 c = a(20),
                 l = a(6),
                 d = a.n(l),
                 u = a(13),
                 b = a(25),
                 p = a(22),
-                j = a(126),
+                j = a(101),
                 h = a(75),
                 v = a.n(h),
                 f = function() {
-                    var e = sessionStorage.getItem("sessionId");
-                    return null == e && (e = Object(j.v4)(), sessionStorage.setItem("sessionId", e)), e
+                    var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0],
+                        t = sessionStorage.getItem("sessionId");
+                    return (null == t || e) && (t = Object(j.v4)(), sessionStorage.setItem("sessionId", t)), t
                 },
                 m = function(e) {
                     "undefined" !== typeof e && e ? s.a.defaults.headers.common.Authorization = "Token " + e : delete s.a.defaults.headers.common.Authorization
                 },
                 x = function(e, t) {
                     s.a.get(e, {
                         responseType: "blob"
@@ -193,15 +194,15 @@
                     }), !t && "" === a && Object(E.jsx)(F, {}), "" !== a && Object(E.jsx)(A, {
                         username: a
                     })]
                 })
             }
             var D = a(14),
                 I = a(27),
-                L = Object(b.b)({
+                W = Object(b.b)({
                     name: "app",
                     initialState: {
                         view: "app",
                         files: [],
                         filesState: "unknown",
                         showSideBar: !0,
                         storageType: "media"
@@ -223,21 +224,21 @@
                             e.showSideBar = !e.showSideBar
                         },
                         setStorageType: function(e, t) {
                             e.storageType = t.payload
                         }
                     }
                 }),
-                U = L.reducer,
-                W = L.actions,
-                H = W.setView,
-                z = W.setFilesState,
-                B = W.setFiles,
-                V = W.setShowSideBar,
-                J = (W.toggleShowSideBar, W.setStorageType),
+                L = W.reducer,
+                U = W.actions,
+                H = U.setView,
+                z = U.setFilesState,
+                B = U.setFiles,
+                V = U.setShowSideBar,
+                J = (U.toggleShowSideBar, U.setStorageType),
                 K = function(e) {
                     return e.app.view
                 },
                 q = function(e) {
                     return e.app.filesState
                 },
                 Y = function(e) {
@@ -479,18 +480,18 @@
                 },
                 De = function(e) {
                     return e.notebooks.widgetsUrlValues
                 },
                 Ie = function(e) {
                     return e.notebooks.widgetsInitialized
                 },
-                Le = function(e) {
+                We = function(e) {
                     return e.notebooks.urlValuesUsed
                 },
-                Ue = Object(b.b)({
+                Le = Object(b.b)({
                     name: "tasks",
                     initialState: {
                         currentTask: {},
                         historicTask: {},
                         showCurrent: !0,
                         previousTask: {},
                         exportingToPDF: !1,
@@ -533,16 +534,16 @@
                             e.executionHistory = t.payload
                         },
                         clearExecutionHistory: function(e) {
                             e.executionHistory = []
                         }
                     }
                 }),
-                We = Ue.reducer,
-                He = Ue.actions,
+                Ue = Le.reducer,
+                He = Le.actions,
                 ze = (He.setShowCurrent, He.setCurrentTask, He.setHistoricTask, He.setPreviousTask, He.copyCurrentToPreviousTask, He.setExportingToPDF),
                 Be = He.setExportToPDFJobId,
                 Ve = He.resetExportToPDFCounter,
                 Je = He.increaseExportToPDFCounter,
                 Ke = He.stopPDFExport,
                 qe = (He.setExecutionHistory, He.clearExecutionHistory),
                 Ye = function(e) {
@@ -1146,15 +1147,15 @@
                                     })]
                                 }))
                             }
                         })
                     })]
                 })
             }
-            var ct, lt = a(101),
+            var ct, lt = a(102),
                 dt = a(127),
                 ut = a.n(dt),
                 bt = a(128),
                 pt = a.n(bt),
                 jt = a(129),
                 ht = a.n(jt);
             ! function(e) {
@@ -1195,26 +1196,26 @@
                 St = function() {
                     return function() {
                         var e = Object(u.a)(d.a.mark((function e(t) {
                             var a, n, o, i, r;
                             return d.a.wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
-                                        return e.prev = 0, t(Ot({})), t(gt(ct.Unknown)), a = "single-site", a = window.location.host.split(":")[0], n = "/api/v1/get-site/".concat(a, "/"), e.next = 8, s.a.get(n);
-                                    case 8:
-                                        o = e.sent, i = o.data, t(Ot(i)), "Ready" !== (null === i || void 0 === i ? void 0 : i.status) ? t(gt(ct.NotReady)) : t(gt(ct.Loaded)), e.next = 19;
+                                        return e.prev = 0, t(Ot({})), t(gt(ct.Unknown)), a = "single-site", a = window.location.host.split(":")[0], window.location.origin.endsWith("hf.space") && (a = "localhost"), n = "/api/v1/get-site/".concat(a, "/"), e.next = 9, s.a.get(n);
+                                    case 9:
+                                        o = e.sent, i = o.data, t(Ot(i)), "Ready" !== (null === i || void 0 === i ? void 0 : i.status) ? t(gt(ct.NotReady)) : t(gt(ct.Loaded)), e.next = 20;
                                         break;
-                                    case 14:
-                                        e.prev = 14, e.t0 = e.catch(0), r = e.t0, console.log(r.message), "Network Error" === (null === r || void 0 === r ? void 0 : r.message) ? t(gt(ct.NetworkError)) : 403 === r.response.status ? t(gt(ct.AccessForbidden)) : 404 === r.response.status ? t(gt(ct.NotFound)) : 401 === r.response.status ? (t(N("")), t(S("")), t(gt(ct.PleaseRefresh))) : console.error("Problem during loading site information. ".concat(e.t0));
-                                    case 19:
+                                    case 15:
+                                        e.prev = 15, e.t0 = e.catch(0), r = e.t0, console.log(r.message), "Network Error" === (null === r || void 0 === r ? void 0 : r.message) ? t(gt(ct.NetworkError)) : 403 === r.response.status ? t(gt(ct.AccessForbidden)) : 404 === r.response.status ? t(gt(ct.NotFound)) : 401 === r.response.status ? (t(N("")), t(S("")), t(gt(ct.PleaseRefresh))) : console.error("Problem during loading site information. ".concat(e.t0));
+                                    case 20:
                                     case "end":
                                         return e.stop()
                                 }
                             }), e, null, [
-                                [0, 14]
+                                [0, 15]
                             ])
                         })));
                         return function(t) {
                             return e.apply(this, arguments)
                         }
                     }()
                 };
@@ -1544,15 +1545,15 @@
             var It = {
                     webSocketState: Tt.Unknown,
                     workerState: _t.Unknown,
                     workerId: void 0,
                     notebookSrc: "",
                     tryConnectCount: 0
                 },
-                Lt = Object(b.b)({
+                Wt = Object(b.b)({
                     name: "ws",
                     initialState: It,
                     reducers: {
                         setWebSocketState: function(e, t) {
                             e.webSocketState = t.payload
                         },
                         setWorkerState: function(e, t) {
@@ -1568,22 +1569,22 @@
                             e.tryConnectCount += 1
                         },
                         resetTryConnectCount: function(e) {
                             e.tryConnectCount = 0
                         }
                     }
                 }),
-                Ut = Lt.reducer,
-                Wt = Lt.actions,
-                Ht = Wt.setWebSocketState,
-                zt = Wt.setWorkerState,
-                Bt = Wt.setWorkerId,
-                Vt = Wt.setNotebookSrc,
-                Jt = Wt.increaseTryConnectCount,
-                Kt = Wt.resetTryConnectCount,
+                Lt = Wt.reducer,
+                Ut = Wt.actions,
+                Ht = Ut.setWebSocketState,
+                zt = Ut.setWorkerState,
+                Bt = Ut.setWorkerId,
+                Vt = Ut.setNotebookSrc,
+                Jt = Ut.increaseTryConnectCount,
+                Kt = Ut.resetTryConnectCount,
                 qt = function(e) {
                     return e.ws.webSocketState
                 },
                 Yt = function(e) {
                     return e.ws.workerState
                 },
                 Gt = function(e) {
@@ -1735,24 +1736,24 @@
                 if (void 0 !== v && null !== v && void 0 !== h && null !== h) {
                     for (var F = 0, A = Object.entries(v); F < A.length; F++) {
                         var M = Object(R.a)(A[F], 2),
                             D = M[0],
                             I = M[1];
                         if (void 0 !== h[D]) {
                             if (($(I) || ee(I) || ae(I) || X(I) || te(I) || oe(I)) && null !== (null === I || void 0 === I ? void 0 : I.url_key) && "" !== (null === I || void 0 === I ? void 0 : I.url_key) && (T = !1), ($(I) || ee(I) || te(I) || oe(I)) && null !== (null === I || void 0 === I ? void 0 : I.url_key) && "" !== (null === I || void 0 === I ? void 0 : I.url_key) && (_ += "".concat(null === I || void 0 === I ? void 0 : I.url_key, "=").concat(h[D], "&")), ae(I) && null !== (null === I || void 0 === I ? void 0 : I.url_key) && "" !== (null === I || void 0 === I ? void 0 : I.url_key)) {
-                                var L = h[D];
-                                _ += "".concat(null === I || void 0 === I ? void 0 : I.url_key, "=").concat(L[0], ",").concat(L[1], "&")
+                                var W = h[D];
+                                _ += "".concat(null === I || void 0 === I ? void 0 : I.url_key, "=").concat(W[0], ",").concat(W[1], "&")
                             }
                             if (X(I) && null !== (null === I || void 0 === I ? void 0 : I.url_key) && "" !== (null === I || void 0 === I ? void 0 : I.url_key))
                                 if (null === I || void 0 === I ? void 0 : I.multi) {
-                                    var U = h[D];
-                                    _ += "".concat(null === I || void 0 === I ? void 0 : I.url_key, "=").concat(U.join(","), "&")
+                                    var L = h[D];
+                                    _ += "".concat(null === I || void 0 === I ? void 0 : I.url_key, "=").concat(L.join(","), "&")
                                 } else {
-                                    var W = h[D];
-                                    _ += "".concat(null === I || void 0 === I ? void 0 : I.url_key, "=").concat(W, "&")
+                                    var U = h[D];
+                                    _ += "".concat(null === I || void 0 === I ? void 0 : I.url_key, "=").concat(U, "&")
                                 }
                         }
                     }
                     "?" !== _ && (_ = _.slice(0, _.length - 1))
                 }
                 return Object(E.jsxs)("div", {
                     style: {
@@ -2146,15 +2147,15 @@
                     p = e.staticNotebook,
                     j = e.allowDownload,
                     h = Object(i.b)(),
                     v = Object(i.c)(Me),
                     f = Object(i.c)(De),
                     m = Object(i.c)(Yt),
                     x = Object(i.c)(Ie),
-                    O = Object(i.c)(Le),
+                    O = Object(i.c)(We),
                     g = Object(n.useContext)($t),
                     y = function() {
                         b && w()
                     },
                     w = function() {
                         var e = et();
                         if (h(fe(e)), f) {
@@ -2290,23 +2291,23 @@
                             label: null === I || void 0 === I ? void 0 : I.label,
                             value: v[M],
                             style: null === I || void 0 === I ? void 0 : I.style,
                             runNb: y
                         }, M)) : se(I) || console.log("Unknown widget type", I)
                     }
                 }
-                var L = {};
-                l && (L = {
+                var W = {};
+                l && (W = {
                     padding: "0px"
                 });
-                var U = void 0 === t || null === t || "" === t;
+                var L = void 0 === t || null === t || "" === t;
                 return Object(E.jsx)("nav", {
                     id: "sidebarMenu",
                     className: "col-lg-3 d-md-block bg-light sidebar",
-                    style: Object(D.a)(Object(D.a)({}, L), {}, {
+                    style: Object(D.a)(Object(D.a)({}, W), {}, {
                         overflowY: "auto"
                     }),
                     children: Object(E.jsx)(ca.a, {
                         blocking: !1,
                         message: "",
                         children: Object(E.jsxs)("div", {
                             className: "position-sticky p-3",
@@ -2330,15 +2331,15 @@
                                     })
                                 })]
                             }), Object(E.jsx)("div", {
                                 style: {
                                     padding: "0px"
                                 },
                                 children: Object(E.jsxs)("form", {
-                                    children: [k, U && Object(E.jsx)("div", {
+                                    children: [k, L && Object(E.jsx)("div", {
                                         style: {
                                             padding: "15px"
                                         }
                                     }), Object(E.jsx)("div", {
                                         className: "form-group mb-3 pb-1 pt-2",
                                         children: !b && Object(E.jsx)(ra, {
                                             runNb: w,
@@ -2527,23 +2528,25 @@
                 var k = {
                         paddingTop: "0px",
                         paddingRight: "0px",
                         paddingLeft: h ? "12px" : "0px",
                         display: "files" === t ? "none" : "block"
                     },
                     N = {};
-                return h || (N = {
+                h || (N = {
                     maxWidth: "1140px",
                     margin: "auto"
-                }), Object(E.jsx)("main", {
+                });
+                var S = !1;
+                return p < 12 && window.innerWidth < 992 && (S = !0), Object(E.jsx)("main", {
                     className: "ms-sm-auto col-".concat(p),
                     style: k,
                     children: Object(E.jsx)(ca.a, {
                         tag: "div",
-                        blocking: r,
+                        blocking: !S && r,
                         children: Object(E.jsxs)("div", {
                             style: N,
                             children: ["loading" === a && !l && Object(E.jsx)("p", {
                                 children: "Loading notebook. Please wait ..."
                             }), "error" === a && Object(E.jsx)("p", {
                                 style: {
                                     margin: "20px"
@@ -2857,19 +2860,19 @@
                     N = Object(i.c)(Ae),
                     S = Object(i.c)(G),
                     P = Object(i.c)(Ze),
                     _ = Object(i.c)(Gt),
                     F = Object(i.c)(Yt),
                     A = Object(i.c)(wt),
                     I = Object(i.c)(Nt),
-                    L = function() {
+                    W = function() {
                         var e;
                         return !(null === j || void 0 === j || null === (e = j.params) || void 0 === e ? void 0 : e.static_notebook) && (F !== _t.UsageLimitReached && F !== _t.MaxIdleTimeReached && F !== _t.MaxRunTimeReached && F !== _t.Running)
                     },
-                    U = function() {
+                    L = function() {
                         return "WATCH_READY" === j.state || "WATCH_WAIT" === j.state || "WATCH_ERROR" === j.state
                     };
                 Object(n.useEffect)((function() {
                     void 0 !== A && p(function(e, t) {
                         var a = arguments.length > 2 && void 0 !== arguments[2] && arguments[2];
                         return function() {
                             var n = Object(u.a)(d.a.mark((function n(o) {
@@ -2923,18 +2926,18 @@
                             })));
                             return function(e) {
                                 return a.apply(this, arguments)
                             }
                         }()
                     }(_, j.id))
                 }), [p, O, j, _]);
-                var W = j.default_view_path;
-                v.state && "DONE" === v.state && v.result && (W = v.result);
+                var U = j.default_view_path;
+                v.state && "DONE" === v.state && v.result && (U = v.result);
                 var H = "";
-                v.state && v.result && "ERROR" === v.state && (H = v.result), m.state && "DONE" === m.state && m.result && (W = m.result), m.state && m.result && "ERROR" === m.state && (H = m.result), W === j.default_view_path && x.state && "DONE" === x.state && x.result && (W = x.result);
+                v.state && v.result && "ERROR" === v.state && (H = v.result), m.state && "DONE" === m.state && m.result && (U = m.result), m.state && m.result && "ERROR" === m.state && (H = m.result), U === j.default_view_path && x.state && "DONE" === x.state && x.result && (U = x.result);
                 var J = !1;
                 return j.output && j.output.toLowerCase().startsWith("rest") && (J = !0), Object(E.jsxs)("div", {
                     className: "App",
                     children: [!b && Object(E.jsx)(M, {
                         isSitePublic: I,
                         username: w
                     }), Object(E.jsxs)(ca.a, {
@@ -2946,18 +2949,18 @@
                                 className: "row",
                                 children: [S && Object(E.jsx)(la, {
                                     notebookTitle: j.title,
                                     notebookId: j.id,
                                     notebookSchedule: j.schedule,
                                     taskCreatedAt: v.created_at,
                                     loadingState: h,
-                                    waiting: L(),
+                                    waiting: W(),
                                     widgetsParams: null === j || void 0 === j || null === (t = j.params) || void 0 === t ? void 0 : t.params,
-                                    watchMode: U(),
-                                    notebookPath: W,
+                                    watchMode: L(),
+                                    notebookPath: U,
                                     displayEmbed: b,
                                     showFiles: function(e) {
                                         if (e)
                                             for (var t = 0, a = Object.entries(e); t < a.length; t++) {
                                                 if (se(Object(R.a)(a[t], 2)[1])) return !0
                                             }
                                         return !1
@@ -2974,15 +2977,15 @@
                                     children: Object(E.jsx)("button", {
                                         className: "btn btn-sm  btn-outline-primary",
                                         type: "button",
                                         style: {
                                             position: "absolute",
                                             top: b ? "5px" : "50px",
                                             left: "5px",
-                                            zIndex: "100"
+                                            zIndex: "2000"
                                         },
                                         onClick: function() {
                                             return p(V(!0))
                                         },
                                         "data-toggle": "tooltip",
                                         "data-placement": "right",
                                         title: "Show sidebar",
@@ -2990,37 +2993,37 @@
                                             className: "fa fa-chevron-right",
                                             "aria-hidden": "true"
                                         })
                                     })
                                 }), J && Object(E.jsx)(ja, {
                                     slug: j.slug,
                                     widgetsParams: null === j || void 0 === j || null === (c = j.params) || void 0 === c ? void 0 : c.params,
-                                    notebookPath: W,
+                                    notebookPath: U,
                                     columnsWidth: S ? 9 : 12,
                                     taskSessionId: v.session_id
                                 }), Object(E.jsx)(ua, {
                                     appView: O,
                                     loadingState: h,
-                                    notebookPath: W,
+                                    notebookPath: U,
                                     errorMsg: H,
-                                    waiting: L(),
-                                    watchMode: U(),
+                                    waiting: W(),
+                                    watchMode: L(),
                                     displayEmbed: b,
                                     username: w,
                                     slidesHash: N,
                                     columnsWidth: S ? 9 : 12,
                                     isPresentation: void 0 !== j.output && "slides" === j.output,
                                     fullScreen: function() {
                                         var e, t;
                                         return void 0 === j || null === j || (void 0 === (null === j || void 0 === j || null === (e = j.params) || void 0 === e ? void 0 : e.full_screen) || null === (null === j || void 0 === j || null === (t = j.params) || void 0 === t ? void 0 : t.full_screen) || j.params.full_screen)
                                     }()
                                 }), "files" === O && Object(E.jsx)(ba, {
                                     files: g,
                                     filesState: y,
-                                    waiting: L()
+                                    waiting: W()
                                 })]
                             })
                         })]
                     }), b && Object(E.jsx)(pa, {})]
                 })
             };
 
@@ -3298,19 +3301,19 @@
                                                                     case 0:
                                                                         return n.prev = 0, n.next = 4, s.a.post("/api/v1/auth/password/change/", {
                                                                             old_password: e,
                                                                             new_password1: t,
                                                                             new_password2: a
                                                                         });
                                                                     case 4:
-                                                                        p.b.success("Password changed successfully"), n.next = 11;
+                                                                        p.b.success("Password changed successfully"), n.next = 10;
                                                                         break;
                                                                     case 7:
-                                                                        n.prev = 7, n.t0 = n.catch(0), n.t0, p.b.error("Password not changed. Problem during password change.");
-                                                                    case 11:
+                                                                        n.prev = 7, n.t0 = n.catch(0), p.b.error("Password not changed. Problem during password change.");
+                                                                    case 10:
                                                                     case "end":
                                                                         return n.stop()
                                                                 }
                                                             }), n, null, [
                                                                 [0, 7]
                                                             ])
                                                         })));
@@ -3852,18 +3855,18 @@
                 return Object(E.jsx)(Ma, {
                     children: Object(E.jsx)(E.Fragment, {
                         children: Object(E.jsx)(r.b, {})
                     })
                 })
             }
 
-            function La() {
+            function Wa() {
                 var e = Object(i.b)();
                 return Object(n.useEffect)((function() {
-                    f(), localStorage.getItem("token") && e(N(localStorage.getItem("token"))), localStorage.getItem("username") && e(S(localStorage.getItem("username"))), e(St())
+                    f(!0), localStorage.getItem("token") && e(N(localStorage.getItem("token"))), localStorage.getItem("username") && e(S(localStorage.getItem("username"))), e(St())
                 }), []), Object(E.jsx)(c.a, {
                     children: Object(E.jsx)(Da, {
                         children: Object(E.jsxs)(r.e, {
                             children: [Object(E.jsxs)(r.c, {
                                 path: "/",
                                 element: Object(E.jsx)(Ia, {}),
                                 children: [Object(E.jsx)(r.c, {
@@ -3880,44 +3883,44 @@
                                 path: "/login",
                                 element: Object(E.jsx)(Pa, {})
                             })]
                         })
                     })
                 })
             }
-            var Ua = function(e) {
+            var La = function(e) {
                     var t = e.store;
                     e.history;
                     return Object(E.jsx)(i.a, {
                         store: t,
-                        children: Object(E.jsx)(La, {})
+                        children: Object(E.jsx)(Wa, {})
                     })
                 },
-                Wa = a(15),
+                Ua = a(15),
                 Ha = a(171),
                 za = a(32);
             var Ba, Va = Object(Ha.a)(),
                 Ja = Object(za.b)({
                     notebooks: ue,
-                    tasks: We,
+                    tasks: Ue,
                     version: ya,
-                    app: U,
+                    app: L,
                     auth: w,
-                    ws: Ut,
+                    ws: Lt,
                     sites: mt
                 }),
-                Ka = Object(Wa.a)(Object(b.c)()),
+                Ka = Object(Ua.a)(Object(b.c)()),
                 qa = (a(285), a(286), a(288), a(289), a(290), a(291), a(292), a(293), Object(b.a)({
                     reducer: Ja,
                     middleware: Ka,
                     preloadedState: Ba
                 }));
             s.a.defaults.baseURL = "http://127.0.0.1:8000", document.addEventListener("DOMContentLoaded", (function() {
                 return Object(o.render)(Object(E.jsxs)("div", {
-                    children: [Object(E.jsx)(Ua, {
+                    children: [Object(E.jsx)(La, {
                         store: qa,
                         history: Va
                     }), Object(E.jsx)(p.a, {
                         position: "top-right",
                         autoClose: 3e3,
                         hideProgressBar: !0,
                         newestOnTop: !0,
@@ -3928,8 +3931,8 @@
             }))
         }
     },
     [
         [295, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.717ee96a.chunk.js.map
+//# sourceMappingURL=main.2749a4f6.chunk.js.map
```

### Comparing `mercury-2.2.1/mercury/frontend-dist/static/js/main.717ee96a.chunk.js.map` & `mercury-2.2.2/mercury/frontend-dist/static/js/main.2749a4f6.chunk.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333131443645858%*

 * *Differences: {"'file'": "'static/js/main.2749a4f6.chunk.js'",*

 * * "'mappings'": "'8QAIaA,EAAe,WAA0B,IAAzBC,EAAwB,wDAC7CC,EAAYC,eAAeC,QAAQ,aAQvC,OAPiB,MAAbF,GAGOD,KAFPC,EAAYG,eACZF,eAAeG,QAAQ,YAAaJ,IAKjCA,GAGEK,EAAoB,SAACC,GACT,qBAAVA,GAAyBA,EAEhCC,IAAMC,SAASC,QAAQC,OAAvB,cAAiD,SAAWJ,SAGrDC,IAAMC,SAASC,QAAQC,OAAvB,eAIFC,EAAiB,SAACC,EAAaC,GACxCN,IACKO,IAAIF,EAAK,CACNG,aAAc,SAEjBC,MAAK,SAACC,GACHC,IAAaD,EAAIE,KAAMN,OClB/BO,EAAY,KACZC,aAAanB,QAAQ,WACvBkB,EAAYC,aAAanB,QAAQ,SACjCG,EAAkBe,IAWpB,IAAME,EAAe,CACnBhB,MAAOc,EACPG,SAAU […]*

```diff
@@ -1,12 +1,13 @@
 {
-    "file": "static/js/main.717ee96a.chunk.js",
+    "file": "static/js/main.2749a4f6.chunk.js",
     "names": [
         "getSessionId",
+        "forceReload",
         "sessionId",
         "sessionStorage",
         "getItem",
         "uuidv4",
         "setItem",
         "setAxiosAuthToken",
         "token",
@@ -325,14 +326,16 @@
         "getSiteWelcome",
         "welcome",
         "isPublic",
         "share",
         "fetchSite",
         "siteSlug",
         "host",
+        "origin",
+        "endsWith",
         "status",
         "NotReady",
         "Loaded",
         "err",
         "log",
         "message",
         "NetworkError",
@@ -546,14 +549,15 @@
         "splitted",
         "injectCode",
         "nbSrc",
         "mainStyle",
         "paddingRight",
         "divStyle",
         "maxWidth",
+        "hideBlockUi",
         "tag",
         "srcDoc",
         "html",
         "FilesView",
         "filesLinks",
         "f",
         "fname",
@@ -746,45 +750,45 @@
         "Routes.tsx",
         "Root.tsx",
         "store.ts",
         "rootReducer.ts",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import { v4 as uuidv4 } from 'uuid';\r\nimport axios from \"axios\";\r\nimport fileDownload from \"js-file-download\";\r\n\r\nexport const getSessionId = () => {\r\n    var sessionId = sessionStorage.getItem(\"sessionId\");\r\n    if (sessionId == null) {\r\n        sessionId = uuidv4();\r\n        sessionStorage.setItem(\"sessionId\", sessionId);\r\n    }\r\n    return sessionId;\r\n}\r\n\r\nexport const setAxiosAuthToken = (token: string | null) => {\r\n    if (typeof token !== \"undefined\" && token) {\r\n        // Apply for every request\r\n        axios.defaults.headers.common[\"Authorization\"] = \"Token \" + token;\r\n    } else {\r\n        // Delete auth header\r\n        delete axios.defaults.headers.common[\"Authorization\"];\r\n    }\r\n};\r\n\r\nexport const handleDownload = (url: string, filename: string) => {\r\n    axios\r\n        .get(url, {\r\n            responseType: \"blob\",\r\n        })\r\n        .then((res) => {\r\n            fileDownload(res.data, filename);\r\n        });\r\n};",
-        "/* eslint-disable import/no-cycle */\r\nimport {\r\n  createSlice,\r\n  PayloadAction,\r\n  AnyAction,\r\n  Dispatch,\r\n} from \"@reduxjs/toolkit\";\r\nimport axios, { AxiosError } from \"axios\";\r\nimport { NavigateFunction } from \"react-router-dom\";\r\nimport { toast } from \"react-toastify\";\r\n\r\nimport { RootState } from \"../store\";\r\nimport { setAxiosAuthToken } from \"../utils\";\r\n\r\nlet initToken = null;\r\nif (localStorage.getItem(\"token\")) {\r\n  initToken = localStorage.getItem(\"token\");\r\n  setAxiosAuthToken(initToken);\r\n}\r\n\r\ntype UserType = {\r\n  pk: number;\r\n  username: string;\r\n  first_name: string;\r\n  last_name: string;\r\n  email: string;\r\n};\r\n\r\nconst initialState = {\r\n  token: initToken as string | null,\r\n  username: \"\" as string,\r\n  user: {\r\n    pk: 0,\r\n    username: \"\",\r\n    first_name: \"\",\r\n    last_name: \"\",\r\n    email: \"\",\r\n  } as UserType,\r\n};\r\n\r\nconst authSlice = createSlice({\r\n  name: \"auth\",\r\n  initialState,\r\n  reducers: {\r\n    setToken(state, action: PayloadAction<string | null>) {\r\n      state.token = action.payload;\r\n      setAxiosAuthToken(state.token);\r\n      if (state.token) {\r\n        localStorage.setItem(\"token\", state.token);\r\n      } else {\r\n        localStorage.removeItem(\"token\");\r\n      }\r\n    },\r\n    setUsername(state, action: PayloadAction<string | null>) {\r\n      state.username = action.payload ? action.payload : \"\";\r\n      if (state.username && state.username !== \"\") {\r\n        localStorage.setItem(\"username\", state.username);\r\n      } else {\r\n        localStorage.removeItem(\"username\");\r\n      }\r\n    },\r\n    setUserInfo(state, action: PayloadAction<UserType>) {\r\n      state.user = action.payload;\r\n    },\r\n  },\r\n});\r\n\r\nexport default authSlice.reducer;\r\n\r\nexport const { setToken, setUsername, setUserInfo } = authSlice.actions;\r\n\r\nexport const getToken = (state: RootState) => state.auth.token;\r\nexport const getUsername = (state: RootState) => state.auth.username;\r\nexport const getUserInfo = (state: RootState) => state.auth.user;\r\n\r\nexport const fetchToken =\r\n  (\r\n    email: string,\r\n    password: string,\r\n    redirectPath: string,\r\n    navigate: NavigateFunction\r\n  ) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        const url = \"/api/v1/auth/login/\";\r\n        const { data } = await axios.post(url, { email, password });\r\n\r\n        dispatch(setToken(data.key));\r\n        dispatch(setUsername(email.split(\"@\")[0]));\r\n        toast.success(\"Log in successfull\");\r\n        // redirect ...\r\n        navigate(redirectPath);\r\n      } catch (error) {\r\n        const err = error as AxiosError;\r\n\r\n        if (err?.message === \"Network Error\") {\r\n          toast.info(\"Problem with server connection\")\r\n        } else {\r\n          type RegisterErrorType = {\r\n            non_field_errors?: string[];\r\n\r\n          };\r\n\r\n          const data = err.response?.data as RegisterErrorType;\r\n          let msg = \"Problem during authentication. \";\r\n          if (data.non_field_errors !== undefined) {\r\n            msg += data.non_field_errors;\r\n          }\r\n          toast.error(msg);\r\n        }\r\n      }\r\n    };\r\n\r\nexport const logout =\r\n  (navigate: NavigateFunction) => async (dispatch: Dispatch<AnyAction>) => {\r\n    try {\r\n      const url = \"/api/v1/auth/logout/\";\r\n      await axios.post(url);\r\n      toast.success(\"Log out successfull\");\r\n      dispatch(setToken(\"\"));\r\n      dispatch(setUsername(\"\"));\r\n      navigate(\"/\");\r\n    } catch (error) {\r\n      toast.error(\"Problem during log out\");\r\n    }\r\n  };\r\n\r\nexport const fetchUserInfo = () => async (dispatch: Dispatch<AnyAction>) => {\r\n  try {\r\n    const url = \"/api/v1/auth/user/\";\r\n    const { data } = await axios.get(url);\r\n    dispatch(setUserInfo(data));\r\n  } catch (error) {\r\n    console.log(`Problem during getting user info. ${error}`);\r\n  }\r\n};\r\n\r\nexport const changePassword =\r\n  (oldPassword: string, newPassword1: string, newPassword2: string) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        const url = \"/api/v1/auth/password/change/\";\r\n        await axios.post(url, {\r\n          old_password: oldPassword,\r\n          new_password1: newPassword1,\r\n          new_password2: newPassword2,\r\n        });\r\n        toast.success(\"Password changed successfully\");\r\n      } catch (error) {\r\n        const err = error as AxiosError;\r\n        // if (err !== undefined && err.response !== undefined && err.response.data !== undefined) {\r\n        //   const msg = Object.values(err.response.data);\r\n        //   toast.error(\"Password not changed.\" + msg);\r\n        // } else {\r\n        //   toast.error(\"Password not changed. Problem during password change.\");\r\n        // }\r\n        toast.error(\"Password not changed. Problem during password change.\");\r\n      }\r\n    };\r\n",
+        "import { v4 as uuidv4 } from 'uuid';\r\nimport axios from \"axios\";\r\nimport fileDownload from \"js-file-download\";\r\n\r\nexport const getSessionId = (forceReload = false) => {\r\n    var sessionId = sessionStorage.getItem(\"sessionId\");\r\n    if (sessionId == null) {\r\n        sessionId = uuidv4();\r\n        sessionStorage.setItem(\"sessionId\", sessionId);\r\n    } else if (forceReload) {\r\n        sessionId = uuidv4();\r\n        sessionStorage.setItem(\"sessionId\", sessionId);\r\n    }\r\n    return sessionId;\r\n}\r\n\r\nexport const setAxiosAuthToken = (token: string | null) => {\r\n    if (typeof token !== \"undefined\" && token) {\r\n        // Apply for every request\r\n        axios.defaults.headers.common[\"Authorization\"] = \"Token \" + token;\r\n    } else {\r\n        // Delete auth header\r\n        delete axios.defaults.headers.common[\"Authorization\"];\r\n    }\r\n};\r\n\r\nexport const handleDownload = (url: string, filename: string) => {\r\n    axios\r\n        .get(url, {\r\n            responseType: \"blob\",\r\n        })\r\n        .then((res) => {\r\n            fileDownload(res.data, filename);\r\n        });\r\n};",
+        "/* eslint-disable import/no-cycle */\r\nimport {\r\n  createSlice,\r\n  PayloadAction,\r\n  AnyAction,\r\n  Dispatch,\r\n} from \"@reduxjs/toolkit\";\r\nimport axios, { AxiosError } from \"axios\";\r\nimport { NavigateFunction } from \"react-router-dom\";\r\nimport { toast } from \"react-toastify\";\r\n\r\nimport { RootState } from \"../store\";\r\nimport { setAxiosAuthToken } from \"../utils\";\r\n\r\nlet initToken = null;\r\nif (localStorage.getItem(\"token\")) {\r\n  initToken = localStorage.getItem(\"token\");\r\n  setAxiosAuthToken(initToken);\r\n}\r\n\r\ntype UserType = {\r\n  pk: number;\r\n  username: string;\r\n  first_name: string;\r\n  last_name: string;\r\n  email: string;\r\n};\r\n\r\nconst initialState = {\r\n  token: initToken as string | null,\r\n  username: \"\" as string,\r\n  user: {\r\n    pk: 0,\r\n    username: \"\",\r\n    first_name: \"\",\r\n    last_name: \"\",\r\n    email: \"\",\r\n  } as UserType,\r\n};\r\n\r\nconst authSlice = createSlice({\r\n  name: \"auth\",\r\n  initialState,\r\n  reducers: {\r\n    setToken(state, action: PayloadAction<string | null>) {\r\n      state.token = action.payload;\r\n      setAxiosAuthToken(state.token);\r\n      if (state.token) {\r\n        localStorage.setItem(\"token\", state.token);\r\n      } else {\r\n        localStorage.removeItem(\"token\");\r\n      }\r\n    },\r\n    setUsername(state, action: PayloadAction<string | null>) {\r\n      state.username = action.payload ? action.payload : \"\";\r\n      if (state.username && state.username !== \"\") {\r\n        localStorage.setItem(\"username\", state.username);\r\n      } else {\r\n        localStorage.removeItem(\"username\");\r\n      }\r\n    },\r\n    setUserInfo(state, action: PayloadAction<UserType>) {\r\n      state.user = action.payload;\r\n    },\r\n  },\r\n});\r\n\r\nexport default authSlice.reducer;\r\n\r\nexport const { setToken, setUsername, setUserInfo } = authSlice.actions;\r\n\r\nexport const getToken = (state: RootState) => state.auth.token;\r\nexport const getUsername = (state: RootState) => state.auth.username;\r\nexport const getUserInfo = (state: RootState) => state.auth.user;\r\n\r\nexport const fetchToken =\r\n  (\r\n    email: string,\r\n    password: string,\r\n    redirectPath: string,\r\n    navigate: NavigateFunction\r\n  ) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        const url = \"/api/v1/auth/login/\";\r\n        const { data } = await axios.post(url, { email, password });\r\n\r\n        dispatch(setToken(data.key));\r\n        dispatch(setUsername(email.split(\"@\")[0]));\r\n        toast.success(\"Log in successfull\");\r\n        // redirect ...\r\n        navigate(redirectPath);\r\n      } catch (error) {\r\n        const err = error as AxiosError;\r\n\r\n        if (err?.message === \"Network Error\") {\r\n          toast.info(\"Problem with server connection\")\r\n        } else {\r\n          type RegisterErrorType = {\r\n            non_field_errors?: string[];\r\n\r\n          };\r\n\r\n          const data = err.response?.data as RegisterErrorType;\r\n          let msg = \"Problem during authentication. \";\r\n          if (data.non_field_errors !== undefined) {\r\n            msg += data.non_field_errors;\r\n          }\r\n          toast.error(msg);\r\n        }\r\n      }\r\n    };\r\n\r\nexport const logout =\r\n  (navigate: NavigateFunction) => async (dispatch: Dispatch<AnyAction>) => {\r\n    try {\r\n      const url = \"/api/v1/auth/logout/\";\r\n      await axios.post(url);\r\n      toast.success(\"Log out successfull\");\r\n      dispatch(setToken(\"\"));\r\n      dispatch(setUsername(\"\"));\r\n      navigate(\"/\");\r\n    } catch (error) {\r\n      toast.error(\"Problem during log out\");\r\n    }\r\n  };\r\n\r\nexport const fetchUserInfo = () => async (dispatch: Dispatch<AnyAction>) => {\r\n  try {\r\n    const url = \"/api/v1/auth/user/\";\r\n    const { data } = await axios.get(url);\r\n    dispatch(setUserInfo(data));\r\n  } catch (error) {\r\n    console.log(`Problem during getting user info. ${error}`);\r\n  }\r\n};\r\n\r\nexport const changePassword =\r\n  (oldPassword: string, newPassword1: string, newPassword2: string) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        const url = \"/api/v1/auth/password/change/\";\r\n        await axios.post(url, {\r\n          old_password: oldPassword,\r\n          new_password1: newPassword1,\r\n          new_password2: newPassword2,\r\n        });\r\n        toast.success(\"Password changed successfully\");\r\n      } catch (error) {\r\n        // const err = error as AxiosError;\r\n        // if (err !== undefined && err.response !== undefined && err.response.data !== undefined) {\r\n        //   const msg = Object.values(err.response.data);\r\n        //   toast.error(\"Password not changed.\" + msg);\r\n        // } else {\r\n        //   toast.error(\"Password not changed. Problem during password change.\");\r\n        // }\r\n        toast.error(\"Password not changed. Problem during password change.\");\r\n      }\r\n    };\r\n",
         "import React from \"react\";\nimport { Link } from \"react-router-dom\";\n\nexport default function LoginButton() {\n  return (\n    <div style={{ color: \"white\", padding: \"5px\", float: \"right\" }}>\n      <Link to=\"/login\" className=\"btn btn-primary btn-sm \">\n        <i className=\"fa fa-sign-in\" aria-hidden=\"true\"></i> Log in\n      </Link>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { useNavigate } from \"react-router-dom\";\nimport { logout } from \"../slices/authSlice\";\n\ntype UserButtonProps = {\n  username: string;\n};\n\nexport default function UserButton({ username }: UserButtonProps) {\n  const dispatch = useDispatch();\n  const navigate = useNavigate();\n  return (\n    <div>\n      <div className=\"dropdown\" style={{ float: \"right\" }}>\n        <a\n          className=\"btn btn-secondary btn-sm dropdown-toggle\"\n          style={{ margin: \"5px\" }}\n          href=\"#\"\n          role=\"button\"\n          id=\"dropdownMenuLink\"\n          data-bs-toggle=\"dropdown\"\n          aria-expanded=\"false\"\n        >\n          {username}\n        </a>\n\n        <ul\n          className=\"dropdown-menu dropdown-menu-end\"\n          aria-labelledby=\"dropdownMenuLink\"\n        >\n          <li>\n            <a className=\"dropdown-item\" href=\"/account\">\n              <i className=\"fa fa-user\" aria-hidden=\"true\"></i> Account\n            </a>\n          </li>\n          <li>\n            <hr className=\"dropdown-divider\" />\n          </li>\n          <li>\n            <a\n              className=\"dropdown-item\"\n              onClick={() => dispatch(logout(navigate))}\n            >\n              <i className=\"fa fa-sign-out\" aria-hidden=\"true\"></i> Log out\n            </a>\n          </li>\n        </ul>\n      </div>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport { Link } from \"react-router-dom\";\nimport LoginButton from \"./LoginButton\";\nimport UserButton from \"./UserButton\";\n\ntype NavBarProps = {\n  isSitePublic: boolean;\n  username: string;\n};\n\nexport default function NavBar({ isSitePublic, username }: NavBarProps) {\n  return (\n    <header className=\"navbar navbar-dark sticky-top bg-dark flex-md-nowrap p-0\">\n      <Link className=\"navbar-brand col-md-3 col-lg-3 me-0 px-3\" to=\"/\">\n        <img\n          alt=\"Mercury\"\n          src={\n            process.env.PUBLIC_URL +\n            process.env.REACT_APP_LOCAL_URL +\n            \"/mercury_logo.svg\"\n          }\n          style={{ height: \"28px\", paddingLeft: \"10px\" }} // height was 24px\n        />\n      </Link>\n\n      {!isSitePublic && username === \"\" && <LoginButton />}\n      {username !== \"\" && <UserButton username={username} />}\n    </header>\n  );\n}\n",
         "/* eslint-disable import/no-cycle */\r\nimport {\r\n  createSlice,\r\n  PayloadAction,\r\n  AnyAction,\r\n  Dispatch,\r\n} from '@reduxjs/toolkit';\r\nimport axios from 'axios';\r\n\r\nimport { RootState } from '../store';\r\nimport { getSessionId } from '../utils';\r\n\r\n\r\nconst initialState = {\r\n  view: \"app\",\r\n  files: [] as string[],\r\n  filesState: \"unknown\",\r\n  showSideBar: true,\r\n  storageType: \"media\"\r\n};\r\n\r\nconst appSlice = createSlice({\r\n  name: 'app',\r\n  initialState,\r\n  reducers: {\r\n    setView(state, action: PayloadAction<string>) {\r\n      state.view = action.payload;\r\n    },\r\n    setFilesState(state, action: PayloadAction<string>) {\r\n      state.filesState = action.payload;\r\n    },\r\n    setFiles(state, action: PayloadAction<string[]>) {\r\n      state.files = action.payload;\r\n    },\r\n    setShowSideBar(state, action: PayloadAction<boolean>) {\r\n      state.showSideBar = action.payload;\r\n    },\r\n    toggleShowSideBar(state) {\r\n      state.showSideBar = !state.showSideBar;\r\n    },\r\n    setStorageType(state, action: PayloadAction<string>) {\r\n      state.storageType = action.payload;\r\n    }\r\n  },\r\n});\r\n\r\nexport default appSlice.reducer;\r\n\r\nexport const {\r\n  setView,\r\n  setFilesState,\r\n  setFiles,\r\n  setShowSideBar,\r\n  toggleShowSideBar,\r\n  setStorageType,\r\n} = appSlice.actions;\r\n\r\n\r\nexport const getView = (state: RootState) => state.app.view;\r\nexport const getOutputFilesState = (state: RootState) => state.app.filesState;\r\nexport const getOutputFiles = (state: RootState) => state.app.files;\r\nexport const getShowSideBar = (state: RootState) => state.app.showSideBar;\r\nexport const getStorageType = (state: RootState) => state.app.storageType;\r\n\r\n\r\nexport const fetchOutputFiles =\r\n  (taskId: number) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        dispatch(setFilesState(\"loading\"))\r\n        dispatch(setFiles([]));\r\n        const sessionId = getSessionId();\r\n        const url = `/api/v1/output_files/${sessionId}/${taskId}/`;\r\n        const { data } = await axios.get(url);\r\n        dispatch(setFiles(data));\r\n        dispatch(setFilesState(\"loaded\"))\r\n      } catch (error) {\r\n        dispatch(setFilesState(\"error\"))\r\n        console.error(`Problem during loading output files. ${error}`);\r\n      }\r\n\r\n    };\r\n\r\nexport const fetchWorkerOutputFiles =\r\n  (workerId: number, notebookId: number) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        dispatch(setFilesState(\"loading\"))\r\n        dispatch(setFiles([]));\r\n        const sessionId = getSessionId();\r\n        const url = `/api/v1/worker-output-files/${sessionId}/${workerId}/${notebookId}/`;\r\n        const { data } = await axios.get(url);\r\n        dispatch(setFiles(data));\r\n        dispatch(setFilesState(\"loaded\"))\r\n      } catch (error) {\r\n        dispatch(setFilesState(\"error\"))\r\n        console.error(`Problem during loading worker output files. ${error}`);\r\n      }\r\n\r\n    };\r\n\r\n\r\nexport const fetchStorageType =\r\n  () =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        const url = `/api/v1/storage-type`;\r\n        const { data } = await axios.get(url);\r\n        dispatch(setStorageType(data.storage_type));\r\n\r\n      } catch (error) {\r\n        console.error(`Get storage type error. ${error}`);\r\n      }\r\n\r\n    };\r\n\r\nexport const userFileUploaded =\r\n  (siteId: number, sessionId: string, filename: string) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        const data = { site_id: siteId, session_id: sessionId, filename }\r\n        const url = `/api/v1/nb-file-uploaded`;\r\n        await axios.post(url, data);\r\n      } catch (error) {\r\n        console.error(`Problem with file upload. ${error}`);\r\n      }\r\n    };\r\n\r\n\r\nexport const deleteUserFileUploaded =\r\n  (siteId: number, sessionId: string, filename: string) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        const data = { site_id: siteId, session_id: sessionId, filename }\r\n        const url = `/api/v1/nb-delete-file`;\r\n        await axios.post(url, data);\r\n      } catch (error) {\r\n        console.error(`Problem with file upload. ${error}`);\r\n      }\r\n    };",
         "export interface ISelectWidget {\n  label: string | null;\n  value: string | null;\n  input: string;\n  choices: string[];\n  multi: boolean | undefined;\n  url_key: string;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface ICheckboxWidget {\n  label: string | null;\n  value: boolean | null;\n  input: string;\n  url_key: string;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface INumericWidget {\n  label: string | null;\n  value: number | null;\n  input: string;\n  min: number;\n  max: number;\n  step: number;\n  url_key: string;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface ISliderWidget {\n  vertical: boolean | null;\n  label: string | null;\n  value: number | null;\n  input: string;\n  min: number | null;\n  max: number | null;\n  step: number | null;\n  url_key: string;\n  urlValue: number | null;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface IRangeWidget {\n  vertical: boolean | null;\n  label: string | null;\n  value: [number, number] | null;\n  input: string;\n  min: number | null;\n  max: number | null;\n  step: number | null;\n  url_key: string;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface IFileWidget {\n  label: string | null;\n  value: string | null;\n  input: string;\n  maxFileSize: string | null;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface ITextWidget {\n  label: string | null;\n  value: string | undefined;\n  input: string;\n  rows: number | null;\n  url_key: string;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface IOutputFilesWidget {\n  output: string;\n  input: null;\n  value: null;\n}\n\nexport interface IMarkdownWidget {\n  output: string;\n  input: null;  // we need to add input to be IWidget\n  value: string;\n}\n\nexport interface IButtonWidget {\n  label: string | null;\n  style: string;\n  input: string;\n  value: string | boolean | null;\n  disabled: boolean;\n  hidden: boolean;\n}\n\n\nexport type IWidget =\n  | ISelectWidget\n  | ICheckboxWidget\n  | INumericWidget\n  | ISliderWidget\n  | IRangeWidget\n  | IFileWidget\n  | ITextWidget\n  | IOutputFilesWidget\n  | IMarkdownWidget\n  | IButtonWidget;\n\nexport function isSelectWidget(widget: IWidget): widget is ISelectWidget {\n  return (widget as ISelectWidget).input === \"select\";\n}\n\nexport function isCheckboxWidget(widget: IWidget): widget is ICheckboxWidget {\n  return (widget as ICheckboxWidget).input === \"checkbox\";\n}\n\nexport function isNumericWidget(widget: IWidget): widget is INumericWidget {\n  return (widget as INumericWidget).input === \"numeric\";\n}\n\nexport function isSliderWidget(widget: IWidget): widget is ISliderWidget {\n  return (widget as ISliderWidget).input === \"slider\";\n}\n\nexport function isRangeWidget(widget: IWidget): widget is IRangeWidget {\n  return (widget as IRangeWidget).input === \"range\";\n}\n\nexport function isFileWidget(widget: IWidget): widget is IFileWidget {\n  return (widget as IFileWidget).input === \"file\";\n}\n\nexport function isTextWidget(widget: IWidget): widget is ITextWidget {\n  return (widget as ITextWidget).input === \"text\";\n}\n\nexport function isOutputFilesWidget(widget: IWidget): widget is IOutputFilesWidget {\n  return (widget as IOutputFilesWidget).output === \"dir\";\n}\n\nexport function isMarkdownWidget(widget: IWidget): widget is IMarkdownWidget {\n  return (widget as IMarkdownWidget).output === \"markdown\";\n}\n\nexport function isButtonWidget(widget: IWidget): widget is IButtonWidget {\n  return (widget as IButtonWidget).input === \"button\";\n}\n",
         "// code from https://stackoverflow.com/questions/36862334/get-viewport-window-height-in-reactjs\nimport { useState, useEffect } from \"react\";\n\nexport function getWindowDimensions() {\n  const { innerWidth: width, innerHeight: height } = window;\n  return {\n    width,\n    height,\n  };\n}\n\nexport default function useWindowDimensions() {\n  const [windowDimensions, setWindowDimensions] = useState(\n    getWindowDimensions()\n  );\n\n  useEffect(() => {\n    function handleResize() {\n      setWindowDimensions(getWindowDimensions());\n    }\n\n    window.addEventListener(\"resize\", handleResize);\n    return () => window.removeEventListener(\"resize\", handleResize);\n  }, []);\n\n  return windowDimensions;\n}\n",
         "/* eslint-disable import/no-cycle */\r\nimport {\r\n    createSlice,\r\n    AnyAction,\r\n    Dispatch,\r\n    PayloadAction,\r\n} from '@reduxjs/toolkit';\r\nimport axios from 'axios';\r\nimport { RootState } from '../store';\r\nimport { toast } from \"react-toastify\";\r\nimport { getSessionId, handleDownload } from '../utils';\r\nimport { setSlidesHash } from './notebooksSlice';\r\n\r\nexport interface ITask {\r\n    id: number;\r\n    task_id: string;\r\n    session_id: string;\r\n    created_at: Date;\r\n    state: \"CREATED\" | \"RECEIVED\" | \"DONE\" | \"ERROR\";\r\n    params: string;\r\n    result: string;\r\n}\r\n\r\nconst initialState = {\r\n    currentTask: {} as ITask,\r\n    historicTask: {} as ITask,\r\n    showCurrent: true,\r\n    previousTask: {} as ITask,\r\n    exportingToPDF: false,\r\n    exportToPDFJobId: '',\r\n    exportToPDFCounter: 0,\r\n    executionHistory: [] as ITask[],\r\n};\r\n\r\nconst tasksSlice = createSlice({\r\n    name: 'tasks',\r\n    initialState,\r\n    reducers: {\r\n        setShowCurrent(state, action: PayloadAction<boolean>) {\r\n            state.showCurrent = action.payload;\r\n        },\r\n        setCurrentTask(state, action: PayloadAction<ITask>) {\r\n            state.currentTask = action.payload;\r\n        },\r\n        setHistoricTask(state, action: PayloadAction<ITask>) {\r\n            state.historicTask = action.payload;\r\n        },\r\n        setPreviousTask(state, action: PayloadAction<ITask>) {\r\n            state.previousTask = action.payload;\r\n        },\r\n        copyCurrentToPreviousTask(state) {\r\n            state.previousTask = state.currentTask;\r\n        },\r\n        setExportingToPDF(state, action: PayloadAction<boolean>) {\r\n            state.exportingToPDF = action.payload;\r\n        },\r\n        setExportToPDFJobId(state, action: PayloadAction<string>) {\r\n            state.exportToPDFJobId = action.payload;\r\n        },\r\n        resetExportToPDFCounter(state) {\r\n            state.exportToPDFCounter = 0;\r\n        },\r\n        increaseExportToPDFCounter(state) {\r\n            state.exportToPDFCounter += 1;\r\n        },\r\n        stopPDFExport(state) {\r\n            state.exportingToPDF = false;\r\n            state.exportToPDFJobId = \"\";\r\n            state.exportToPDFCounter = 0;\r\n        },\r\n        setExecutionHistory(state, action: PayloadAction<ITask[]>) {\r\n            state.executionHistory = action.payload;\r\n        },\r\n        clearExecutionHistory(state) {\r\n            state.executionHistory = [];\r\n        }\r\n    },\r\n});\r\n\r\nexport default tasksSlice.reducer;\r\n\r\nexport const {\r\n    setShowCurrent,\r\n    setCurrentTask,\r\n    setHistoricTask,\r\n    setPreviousTask,\r\n    copyCurrentToPreviousTask,\r\n    setExportingToPDF,\r\n    setExportToPDFJobId,\r\n    resetExportToPDFCounter,\r\n    increaseExportToPDFCounter,\r\n    stopPDFExport,\r\n    setExecutionHistory,\r\n    clearExecutionHistory,\r\n} = tasksSlice.actions;\r\n\r\nexport const getShowCurrent = (state: RootState) => state.tasks.showCurrent;\r\nexport const getCurrentTask = (state: RootState) => state.tasks.currentTask;\r\nexport const getHistoricTask = (state: RootState) => state.tasks.historicTask;\r\nexport const getPreviousTask = (state: RootState) => state.tasks.previousTask;\r\nexport const getExportingToPDF = (state: RootState) => state.tasks.exportingToPDF;\r\nexport const getExportToPDFJobId = (state: RootState) => state.tasks.exportToPDFJobId;\r\nexport const getExportToPDFCounter = (state: RootState) => state.tasks.exportToPDFCounter;\r\nexport const getExecutionHistory = (state: RootState) => state.tasks.executionHistory;\r\n\r\nexport const fetchCurrentTask =\r\n    (notebookId: Number) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n\r\n            const sessionId = getSessionId();\r\n\r\n            try {\r\n                const url = `/api/v1/latest_task/${notebookId}/${sessionId}/`;\r\n                const { data } = await axios.get(url);\r\n                dispatch(setCurrentTask(data))\r\n\r\n            } catch (error) {\r\n                // console.clear();\r\n                dispatch(setCurrentTask({} as ITask));\r\n            }\r\n\r\n        };\r\n\r\nexport const scrapeSlidesHash = () => {\r\n    try {\r\n        const iframeElement = (document.getElementById(\"main-iframe\") as HTMLIFrameElement);\r\n        const hash = iframeElement?.contentWindow?.location?.hash;\r\n        if (hash) {\r\n            return hash;\r\n        }\r\n    } catch (error) { }\r\n    return \"\";\r\n}\r\n\r\n\r\nexport const executeNotebook =\r\n    (notebookId: Number) =>\r\n        async (dispatch: Dispatch<AnyAction>, getState: () => any) => {\r\n            const { widgets } = getState().widgets;\r\n            const sessionId = getSessionId();\r\n\r\n            const slidesHash = scrapeSlidesHash();\r\n            dispatch(setSlidesHash(slidesHash));\r\n\r\n            try {\r\n                const task = {\r\n                    session_id: sessionId,\r\n                    params: JSON.stringify(widgets),\r\n                }\r\n                const url = `/api/v1/execute/${notebookId}/`;\r\n                const { data } = await axios.post(url, task);\r\n                dispatch(setCurrentTask(data))\r\n\r\n            } catch (error) {\r\n                console.error(`Problem during notebook execution. ${error}`);\r\n            }\r\n\r\n        };\r\n\r\n\r\nexport const clearTasks =\r\n    (notebookId: Number) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n            try {\r\n                const sessionId = getSessionId();\r\n                const url = `/api/v1/clear_tasks/${notebookId}/${sessionId}/`;\r\n                await axios.post(url);\r\n                dispatch(setCurrentTask({} as ITask));\r\n                dispatch(setHistoricTask({} as ITask));\r\n                dispatch(setPreviousTask({} as ITask));\r\n                dispatch(setExecutionHistory([]));\r\n                toast.success(\"All previous tasks deleted. The default view of the app is displayed.\")\r\n            } catch (error) {\r\n                toast.error(`Trying to clear previous tasks. The error occured. ${error}`)\r\n            }\r\n        };\r\n\r\n\r\nexport const exportToPDF =\r\n    (notebookId: Number, notebookPath: String) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n            try {\r\n                dispatch(setExportingToPDF(true));\r\n                dispatch(resetExportToPDFCounter());\r\n                dispatch(setExportToPDFJobId(\"\"));\r\n\r\n                const sessionId = getSessionId();\r\n                const url = `/api/v1/export_pdf/`;\r\n                // convert from JS camel case to Python undescore variables\r\n                const params = {\r\n                    session_id: sessionId,\r\n                    notebook_id: notebookId,\r\n                    notebook_path: notebookPath,\r\n                }\r\n                const { data } = await axios.post(url, params);\r\n                dispatch(setExportToPDFJobId(data.job_id))\r\n            } catch (error) {\r\n                toast.error(`The error occured during PDF export. ${error}`);\r\n                dispatch(stopPDFExport());\r\n            }\r\n        };\r\n\r\nexport const getPDF =\r\n    (jobId: String) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n            try {\r\n                const url = `/api/v1/get_pdf/${jobId}/`;\r\n                const { data } = await axios.get(url);\r\n                if (data.ready) {\r\n                    dispatch(stopPDFExport());\r\n                    if (data.error !== \"\") {\r\n                        toast.error(data.error);\r\n                    } else {\r\n                        handleDownload(\r\n                            `${axios.defaults.baseURL}${data.url}`,\r\n                            `${data.title}`\r\n                        )\r\n                    }\r\n                } else {\r\n                    dispatch(increaseExportToPDFCounter());\r\n                }\r\n            } catch (error) {\r\n                toast.error(`The error occured during PDF export. ${error}`);\r\n                dispatch(stopPDFExport());\r\n            }\r\n        };\r\n\r\n\r\n\r\nexport const fetchExecutionHistory =\r\n    (notebookId: Number, clearPreviousHistory = true) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n\r\n            dispatch(setHistoricTask({} as ITask));\r\n            if (clearPreviousHistory) {\r\n                dispatch(clearExecutionHistory());\r\n            }\r\n\r\n            const sessionId = getSessionId();\r\n\r\n            try {\r\n                const url = `/api/v1/execution_history/${notebookId}/${sessionId}/`;\r\n                const { data } = await axios.get(url);\r\n                dispatch(setExecutionHistory(data))\r\n            } catch (error) {\r\n                dispatch(clearExecutionHistory());\r\n            }\r\n\r\n        };\r\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect, useState } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { useSearchParams } from \"react-router-dom\";\n\nimport {\n  setUrlValuesUsed,\n  setWidgetUrlValue,\n  setWidgetValue,\n} from \"../slices/notebooksSlice\";\n\ntype CheckboxProps = {\n  widgetKey: string;\n  label: string | null;\n  value: boolean | null;\n  disabled: boolean;\n  hidden: boolean;\n  runNb: () => void;\n  url_key: string;\n};\n\nexport default function CheckboxWidget({\n  widgetKey,\n  label,\n  value,\n  disabled,\n  hidden,\n  runNb,\n  url_key,\n}: CheckboxProps) {\n  const dispatch = useDispatch();\n  const [updated, userInteraction] = useState(false);\n\n  const [searchParams] = useSearchParams();\n\n  useEffect(() => {\n    if (url_key !== undefined && url_key !== \"\") {\n      const urlValue = searchParams.get(url_key)?.toLowerCase();\n\n      if (\n        !updated &&\n        urlValue !== undefined &&\n        (urlValue === \"true\" || urlValue === \"false\")\n      ) {\n        dispatch(\n          setWidgetUrlValue({\n            key: widgetKey,\n            value: urlValue === \"true\",\n          })\n        );\n        dispatch(setUrlValuesUsed(true));\n      }\n    }\n  }, [dispatch, searchParams, updated, url_key, widgetKey]);\n\n  useEffect(() => {\n    if (updated) {\n      runNb();\n    }\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [value]);\n\n  return (\n    <div className=\"form-group form-check form-switch mb-3\"  style={{ display: hidden ? \"none\" : \"\" }}>\n      <input\n        className=\"form-check-input\"\n        type=\"checkbox\"\n        id={`checkbox-${label}`}\n        disabled={disabled}\n        onChange={() => {\n          userInteraction(true);\n          dispatch(setWidgetValue({ key: widgetKey, value: !value }));\n        }}\n        checked={value != null ? value : false}\n      />\n      <label\n        className=\"form-check-label\"\n        htmlFor={`checkbox-${label}`}\n        style={{ color: disabled ? \"#555\" : \"#212529\" }}\n      >\n        {label}\n      </label>\n    </div>\n  );\n}\n",
         "import React, { useEffect, useState } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { useSearchParams } from \"react-router-dom\";\nimport {\n  setUrlValuesUsed,\n  setWidgetUrlValue,\n  setWidgetValue,\n} from \"../slices/notebooksSlice\";\n\ntype NumericProps = {\n  widgetKey: string;\n  label: string | null;\n  value: number | null;\n  min: number | null;\n  max: number | null;\n  step: number | null;\n  disabled: boolean;\n  hidden: boolean;\n  runNb: () => void;\n  continuousUpdate: boolean;\n  url_key: string;\n};\n\nexport default function NumericWidget({\n  widgetKey,\n  label,\n  value,\n  min,\n  max,\n  step,\n  disabled,\n  hidden,\n  runNb,\n  continuousUpdate,\n  url_key,\n}: NumericProps) {\n  const dispatch = useDispatch();\n  const [apply, showApply] = useState(false);\n  const [updated, userInteraction] = useState(false);\n\n  let minValue = 0;\n  let maxValue = 10;\n  let stepValue = 1;\n  if (min !== null) {\n    minValue = min;\n  }\n  if (max !== null) {\n    maxValue = max;\n  }\n  if (step !== null) {\n    stepValue = step;\n  }\n  let displayValue = value !== null && value !== undefined ? value : 0;\n\n  const [searchParams] = useSearchParams();\n  useEffect(() => {\n    if (url_key !== undefined && url_key !== \"\") {\n      const urlValue = searchParams.get(url_key);\n      if (\n        !updated &&\n        urlValue !== undefined &&\n        urlValue !== null &&\n        !isNaN(parseFloat(urlValue)) &&\n        parseFloat(urlValue) >= minValue &&\n        parseFloat(urlValue) <= maxValue\n      ) {\n        dispatch(\n          setWidgetUrlValue({\n            key: widgetKey,\n            value: parseFloat(urlValue),\n          })\n        );\n        dispatch(setUrlValuesUsed(true));\n      }\n    }\n  }, [dispatch, maxValue, minValue, searchParams, updated, url_key, widgetKey]);\n\n  const validateValue = () => {\n    if (min !== null && value !== null && value < min) {\n      dispatch(setWidgetValue({ key: widgetKey, value: min }));\n    }\n    if (max !== null && value !== null && value > max) {\n      dispatch(setWidgetValue({ key: widgetKey, value: max }));\n    }\n  };\n\n  return (\n    <div className=\"form-group mb-3\" style={{ display: hidden ? \"none\" : \"\" }}>\n      <label\n        htmlFor={`checkbox-${label}`}\n        style={{ color: disabled ? \"#555\" : \"#212529\" }}\n      >\n        {label}\n      </label>\n      <input\n        className=\"form-control\"\n        type=\"number\"\n        value={displayValue} // {displayValue as number | string}\n        onChange={(e) => {\n          userInteraction(true);\n          showApply(true);\n          dispatch(setWidgetValue({ key: widgetKey, value: e.target.value }));\n        }}\n        onBlur={(e) => {\n          validateValue();\n        }}\n        onKeyPress={(e) => {\n          if (e.key === \"Enter\") {\n            validateValue();\n            runNb();\n            showApply(false);\n            e.preventDefault();\n          }\n        }}\n        min={minValue}\n        max={maxValue}\n        step={stepValue}\n        disabled={disabled}\n      />\n      {apply && continuousUpdate && (\n        <div\n          style={{\n            float: \"right\",\n            position: \"relative\",\n            top: \"0px\",\n            left: \"0px\",\n          }}\n        >\n          <button\n            className=\"btn btn-sm btn-outline-primary\"\n            onClick={(e) => {\n              validateValue();\n              runNb();\n              showApply(false);\n              e.preventDefault();\n            }}\n            style={{\n              fontSize: \"0.7em\",\n              border: \"none\",\n            }}\n          >\n            Press enter or click to apply\n          </button>\n        </div>\n      )}\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\n\nimport ReactMarkdown from \"react-markdown\";\nimport rehypeHighlight from \"rehype-highlight\";\nimport remarkGfm from \"remark-gfm\";\nimport emoji from \"remark-emoji\";\nimport rehypeRaw from \"rehype-raw\";\n\ntype MarkdownProps = {\n  value: string;\n  disabled: boolean;\n};\n\nexport default function MarkdownWidget({ value, disabled }: MarkdownProps) {\n  return (\n    <div\n      className=\"form-group mb-3\"\n      style={{ color: disabled ? \"#555\" : \"#212529\" }}\n    >\n      <ReactMarkdown\n        rehypePlugins={[remarkGfm, rehypeHighlight, emoji, rehypeRaw]}\n      >\n        {value}\n      </ReactMarkdown>\n    </div>\n  );\n}\n",
@@ -792,15 +796,15 @@
     ],
     "version": 3
 }
```


 * *Files identical despite different names*


 * *Files identical despite different names*





















