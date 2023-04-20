# Comparing `tmp/django-common-task-system-1.1.9.tar.gz` & `tmp/django-common-task-system-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.1.9.tar", last modified: Wed Apr 19 07:40:38 2023, max compression
+gzip compressed data, was "django-common-task-system-1.2.0.tar", last modified: Thu Apr 20 08:34:02 2023, max compression
```

## Comparing `django-common-task-system-1.1.9.tar` & `django-common-task-system-1.2.0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.086089 django-common-task-system-1.1.9/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.1.9/LICENSE
--rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-04-19 07:40:38.086089 django-common-task-system-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.817973 django-common-task-system-1.1.9/django_common_task_system/
--rw-rw-rw-   0        0        0     3014 2023-04-17 02:45:20.000000 django-common-task-system-1.1.9/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0    10500 2023-04-19 07:34:32.000000 django-common-task-system-1.1.9/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.1.9/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.1.9/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.1.9/django_common_task_system/fields.py
--rw-rw-rw-   0        0        0    15733 2023-04-17 08:15:48.000000 django-common-task-system-1.1.9/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.885397 django-common-task-system-1.1.9/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/0006_consumerpermission.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.1.9/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.1.9/django_common_task_system/mixin.py
--rw-rw-rw-   0        0        0    34061 2023-04-18 07:40:32.000000 django-common-task-system-1.1.9/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.1.9/django_common_task_system/permissions.py
--rw-rw-rw-   0        0        0     2086 2023-04-13 06:35:40.000000 django-common-task-system-1.1.9/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.729770 django-common-task-system-1.1.9/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.729770 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.888471 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.890480 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.954847 django-common-task-system-1.1.9/django_common_task_system/system_task/
--rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/__init__.py
--rw-rw-rw-   0        0        0     4987 2023-04-17 08:40:58.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/admin.py
--rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/apps.py
--rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/choices.py
--rw-rw-rw-   0        0        0     4122 2023-04-13 09:07:07.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.999563 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/
--rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
--rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/__init__.py
--rw-rw-rw-   0        0        0    17296 2023-04-18 07:39:59.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/models.py
--rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/process.py
--rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/queue.py
--rw-rw-rw-   0        0        0     1511 2023-04-17 03:57:06.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/serializers.py
--rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/tests.py
--rw-rw-rw-   0        0        0      771 2023-04-14 03:45:06.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/urls.py
--rw-rw-rw-   0        0        0     5308 2023-04-18 02:48:30.000000 django-common-task-system-1.1.9/django_common_task_system/system_task/views.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.006346 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-04-12 09:15:38.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/main.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.014357 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     2660 2023-04-18 07:30:06.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.049153 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-rw-rw-   0        0        0     3500 2023-04-17 05:43:02.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.732264 django-common-task-system-1.1.9/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.732264 django-common-task-system-1.1.9/django_common_task_system/templates/admin/
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.050665 django-common-task-system-1.1.9/django_common_task_system/templates/admin/system_schedule/
--rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.1.9/django_common_task_system/templates/admin/system_schedule/change_list.html
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.059873 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.1.9/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0      991 2023-04-14 03:33:36.000000 django-common-task-system-1.1.9/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.084087 django-common-task-system-1.1.9/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.1.9/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.1.9/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.1.9/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.1.9/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.1.9/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0    10457 2023-04-18 02:48:30.000000 django-common-task-system-1.1.9/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:37.838748 django-common-task-system-1.1.9/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      303 2023-04-19 07:40:37.000000 django-common-task-system-1.1.9/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4253 2023-04-19 07:40:37.000000 django-common-task-system-1.1.9/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:40:37.000000 django-common-task-system-1.1.9/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-04-19 07:40:37.000000 django-common-task-system-1.1.9/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-19 07:40:37.000000 django-common-task-system-1.1.9/django_common_task_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 07:40:38.086089 django-common-task-system-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-04-19 07:38:37.000000 django-common-task-system-1.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:40:38.085086 django-common-task-system-1.1.9/tests/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.1.9/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.131681 django-common-task-system-1.2.0/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      303 2023-04-20 08:34:02.130681 django-common-task-system-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.830295 django-common-task-system-1.2.0/django_common_task_system/
+-rw-rw-rw-   0        0        0     3014 2023-04-17 02:45:20.000000 django-common-task-system-1.2.0/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0    10500 2023-04-19 07:34:32.000000 django-common-task-system-1.2.0/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.2.0/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.2.0/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.2.0/django_common_task_system/fields.py
+-rw-rw-rw-   0        0        0    15733 2023-04-17 08:15:48.000000 django-common-task-system-1.2.0/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.912514 django-common-task-system-1.2.0/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/0006_consumerpermission.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.2.0/django_common_task_system/mixin.py
+-rw-rw-rw-   0        0        0    35781 2023-04-20 05:47:24.000000 django-common-task-system-1.2.0/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.2.0/django_common_task_system/permissions.py
+-rw-rw-rw-   0        0        0     2086 2023-04-13 06:35:40.000000 django-common-task-system-1.2.0/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.737713 django-common-task-system-1.2.0/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.737713 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.926520 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.954514 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.008760 django-common-task-system-1.2.0/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     5005 2023-04-20 07:45:49.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     4130 2023-04-19 09:42:02.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.057761 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
+-rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0    14677 2023-04-20 05:44:40.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/queue.py
+-rw-rw-rw-   0        0        0     1511 2023-04-17 03:57:06.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      771 2023-04-14 03:45:06.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     5308 2023-04-18 02:48:30.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.059760 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.069174 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     2749 2023-04-19 09:51:15.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.093682 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     3500 2023-04-17 05:43:02.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.740710 django-common-task-system-1.2.0/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.740710 django-common-task-system-1.2.0/django_common_task_system/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.094682 django-common-task-system-1.2.0/django_common_task_system/templates/admin/system_schedule/
+-rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.2.0/django_common_task_system/templates/admin/system_schedule/change_list.html
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.108685 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.2.0/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0      991 2023-04-14 03:33:36.000000 django-common-task-system-1.2.0/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.128684 django-common-task-system-1.2.0/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.2.0/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.2.0/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.2.0/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.2.0/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.2.0/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0    11074 2023-04-20 08:31:56.000000 django-common-task-system-1.2.0/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.856425 django-common-task-system-1.2.0/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-04-20 08:34:01.000000 django-common-task-system-1.2.0/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4253 2023-04-20 08:34:01.000000 django-common-task-system-1.2.0/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 08:34:01.000000 django-common-task-system-1.2.0/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-04-20 08:34:01.000000 django-common-task-system-1.2.0/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-20 08:34:01.000000 django-common-task-system-1.2.0/django_common_task_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 08:34:02.131681 django-common-task-system-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-04-20 08:31:56.000000 django-common-task-system-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.129687 django-common-task-system-1.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.2.0/tests/__init__.py
```

### Comparing `django-common-task-system-1.1.9/LICENSE` & `django-common-task-system-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/__init__.py` & `django-common-task-system-1.2.0/django_common_task_system/__init__.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/admin.py` & `django-common-task-system-1.2.0/django_common_task_system/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/choices.py` & `django-common-task-system-1.2.0/django_common_task_system/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/fields.py` & `django-common-task-system-1.2.0/django_common_task_system/fields.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/forms.py` & `django-common-task-system-1.2.0/django_common_task_system/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.2.0/django_common_task_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py` & `django-common-task-system-1.2.0/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py` & `django-common-task-system-1.2.0/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/migrations/0006_consumerpermission.py` & `django-common-task-system-1.2.0/django_common_task_system/migrations/0006_consumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/mixin.py` & `django-common-task-system-1.2.0/django_common_task_system/mixin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/models.py` & `django-common-task-system-1.2.0/django_common_task_system/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from . import settings
 from . permissions import ConsumerPermissionValidator
 import re
 import os
 from django.core.validators import ValidationError
 from django.dispatch import Signal, receiver
 from threading import Event
+from collections import OrderedDict
 
 system_initialize_signal = Signal()
 system_schedule_event = Event()
 
 mdays = [0, 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
 
 
@@ -585,168 +586,223 @@
 
 class ConsumerPermission(AbstractConsumerPermission):
     class Meta(AbstractConsumerPermission.Meta):
         db_table = 'schedule_consumer_permission'
         abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
 
 
-class BaseBuiltinQueues(dict):
-    model = TaskScheduleQueue
+class BuiltinModels(OrderedDict):
+    model: models.Model = None
+    model_unique_kwargs = []
+
+    def init_object(self, obj: models.Model):
+        kwargs = {
+            key: getattr(obj, key) for key in self.model_unique_kwargs
+        }
+        defaults = {
+            filed.name: getattr(obj, filed.name) for filed in obj._meta.fields if filed.name not in kwargs
+        }
+        current = self.model.objects.get_or_create(
+            defaults=defaults, **kwargs
+        )[0]
+        for field in obj._meta.fields:
+            setattr(obj, field.name, getattr(current, field.name))
+        return obj
+
+    def initialize(self):
+        for k, v in self.__dict__.items():
+            if isinstance(v, self.model):
+                obj = self.init_object(v)
+                self.add(obj, k)
+
+    def add(self, obj: models.Model, key=None):
+        if key:
+            self[key] = obj
+
+    def delete(self, obj, key):
+        if key:
+            self.pop(key, None)
+
+
+class BuiltinCallbacks(BuiltinModels):
+    model = TaskScheduleCallback
+    model_unique_kwargs = ['name']
+
+    def __init__(self, user):
+        self.http_log_upload = self.model(
+            name='Http日志上报',
+            trigger_event=TaskCallbackEvent.DONE,
+            status=TaskCallbackStatus.ENABLE.value,
+            user=user,
+        )
+        super(BuiltinCallbacks, self).__init__()
+
+    def init_object(self, obj: models.Model):
+        super(BuiltinCallbacks, self).init_object(obj)
+        
+    def initialize(self):
+        super(BuiltinCallbacks, self).initialize()
+
+
+class BaseBuiltinQueues(BuiltinModels):
+
     status_params_mapping = {
         TaskScheduleStatus.OPENING.value: 'opening',
         TaskScheduleStatus.CLOSED.value: 'closed',
         TaskScheduleStatus.TEST.value: 'test',
         TaskScheduleStatus.DONE.value: 'done',
         TaskScheduleStatus.ERROR.value: 'error',
     }
 
+    model_unique_kwargs = ['code']
+
     def __init__(self):
         super(BaseBuiltinQueues, self).__init__()
         for m in self.model.objects.filter(status=True):
             self.add(m)
 
-    def add(self, instance: AbstractTaskScheduleQueue):
+    def add(self, instance: AbstractTaskScheduleQueue, key=None):
         if instance.status:
             old = self.get(instance.code)
             if not old or old.module != instance.module or old.config != instance.config:
                 instance.queue = import_string(instance.module)(**instance.config)
                 self[instance.code] = instance
         elif not instance.status:
             self.pop(instance.code, None)
 
-    def delete(self, instance: AbstractTaskScheduleQueue):
+    def delete(self, instance: AbstractTaskScheduleQueue, key=None):
         self.pop(instance.code, None)
 
 
 class BuiltinQueues(BaseBuiltinQueues):
+    model = TaskScheduleQueue
+
     def __init__(self):
-        self.opening = self.model.objects.get_or_create(
+        self.opening = self.model(
             code=self.status_params_mapping[TaskScheduleStatus.OPENING.value],
-            defaults={
-                'status': True,
-                'module': ScheduleQueueModule.QUEUE.value,
-                'name': '已启用任务'
-            }
-        )[0]
-        self.test = self.model.objects.get_or_create(
+            status=True,
+            module=ScheduleQueueModule.QUEUE.value,
+            name='已启用任务'
+        )
+        self.test = self.model(
             code=self.status_params_mapping[TaskScheduleStatus.TEST.value],
-            defaults={
-                'status': True,
-                'module': ScheduleQueueModule.QUEUE.value,
-                'name': '测试任务'
-            }
-        )[0]
+            status=True,
+            module=ScheduleQueueModule.QUEUE.value,
+            name='测试任务'
+        )
         super(BuiltinQueues, self).__init__()
 
 
-class BaseBuiltinProducers(dict):
-    model = TaskScheduleProducer
+class BaseBuiltinProducers(BuiltinModels):
+    model_unique_kwargs = ['queue']
 
     def __init__(self):
         super(BaseBuiltinProducers, self).__init__()
         for m in self.model.objects.filter(status=True):
             self.add(m)
 
-    def add(self, instance: AbstractTaskScheduleProducer):
+    def add(self, instance: AbstractTaskScheduleProducer, key=None):
         if instance.status:
             old = self.get(instance.id)
             if not old or old.queue != instance.queue:
                 self[instance.id] = instance
         elif not instance.status:
             self.pop(instance.id, None)
 
-    def delete(self, instance: AbstractTaskScheduleProducer):
+    def delete(self, instance: AbstractTaskScheduleProducer, key=None):
         self.pop(instance.id, None)
 
 
 class BuiltinProducers(BaseBuiltinProducers):
+    model = TaskScheduleProducer
 
     def __init__(self, queues: BuiltinQueues):
-        self.opening = TaskScheduleProducer.objects.get_or_create(
+        self.opening = self.model(
             queue=queues.opening,
             lte_now=True,
-            defaults={
-                'filters': {
-                    'status': TaskScheduleStatus.OPENING.value,
-                },
-                'status': True,
-                'name': '默认'
-            }
-        )[0]
-
-        self.test = TaskScheduleProducer.objects.get_or_create(
+            filters={
+                'status': TaskScheduleStatus.OPENING.value,
+            },
+            status=True,
+            name='默认'
+        )
+        self.test = self.model(
             queue=queues.test,
             lte_now=True,
-            defaults={
-                'filters': {
-                    'status': TaskScheduleStatus.TEST.value,
-                },
-                'status': True,
-                'name': '测试'
-            }
-        )[0]
+            filters={
+                'status': TaskScheduleStatus.TEST.value,
+            },
+            status=True,
+            name='测试'
+        )
         super(BuiltinProducers, self).__init__()
 
 
-class BaseConsumerPermissions(dict):
+class BaseConsumerPermissions(BuiltinModels):
     model = ConsumerPermission
+    model_unique_kwargs = ['producer', 'type']
 
     def __init__(self):
         super(BaseConsumerPermissions, self).__init__()
         for m in self.model.objects.filter(status=True):
             self.add(m)
 
-    def add(self, instance: AbstractConsumerPermission):
+    def add(self, instance: AbstractConsumerPermission, key=None):
         if instance.status:
             old = self.get(instance.producer_id)
             if not old or old.type != instance.type or old.config != instance.config:
                 validator = ConsumerPermissionValidator.get(instance.type)
                 if validator:
                     self[instance.producer.queue.code] = validator(instance.config)
         elif not instance.status:
             self.pop(instance.producer.queue.code, None)
 
-    def delete(self, instance: AbstractConsumerPermission):
+    def delete(self, instance: AbstractConsumerPermission, key=None):
         self.pop(instance.producer.queue.code, None)
 
 
 class BuiltinConsumerPermissions(BaseConsumerPermissions):
     model = ConsumerPermission
 
 
-class Builtins:
+class BaseBuiltins:
+
+    app = None
 
     def __init__(self):
         self._initialized = False
-        self._queues = None
-        self._producers = None
-        self._consumer_permissions = None
+        self.user = UserModel(username='系统', is_superuser=True)
+
+    def init_user(self):
+        user = UserModel.objects.filter(is_superuser=True).order_by('id').first()
+        if not user:
+            raise Exception('请先创建超级用户')
+        for field in user._meta.fields:
+            setattr(self.user, field.name, getattr(user, field.name))
 
     def initialize(self):
         if not self._initialized:
             self._initialized = True
             if os.environ.get('RUN_MAIN') == 'true' and os.environ.get('RUN_CLIENT') != 'true':
                 from django.conf import settings
-                if 'django_common_task_system' in settings.INSTALLED_APPS:
-                    print('初始化内置任务')
-                    self._queues = BuiltinQueues()
-                    self._producers = BuiltinProducers(self._queues)
-                    self._consumer_permissions = BuiltinConsumerPermissions()
-                    system_initialize_signal.send(sender='builtin_initialized', app='django_common_task_system')
+                if self.app in settings.INSTALLED_APPS:
+                    print('[%s]初始化内置任务' % self.app)
+                    self.init_user()
+                    for i in self.__dict__.values():
+                        if isinstance(i, BuiltinModels):
+                            i.initialize()
+                    system_initialize_signal.send(sender='builtin_initialized', app=self.app)
 
-    @property
-    def queues(self) -> BuiltinQueues:
-        self.initialize()
-        return self._queues
 
-    @property
-    def producers(self) -> BuiltinProducers:
-        self.initialize()
-        return self._producers
+class Builtins(BaseBuiltins):
 
-    @property
-    def consumer_permissions(self) -> BuiltinConsumerPermissions:
-        self.initialize()
-        return self._consumer_permissions
+    app = 'django_common_task_system'
+
+    def __init__(self):
+        super(Builtins, self).__init__()
+        self.queues = BuiltinQueues()
+        self.callbacks = BuiltinCallbacks(self.user)
+        self.producers = BuiltinProducers(self.queues)
+        self.consumer_permissions = BuiltinConsumerPermissions()
 
 
 builtins = Builtins()
```

### Comparing `django-common-task-system-1.1.9/django_common_task_system/permissions.py` & `django-common-task-system-1.2.0/django_common_task_system/permissions.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/serializers.py` & `django-common-task-system-1.2.0/django_common_task_system/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from django.shortcuts import reverse
 from django.utils.html import format_html
 from django.db.models.signals import post_delete
 from . import models
 from . import forms
 from .. import admin as base_admin
 from .process import ProcessManager
-from ..system_task_execution.main import start_by_server
+from ..system_task_execution.main import start_system_client
 import os
 
 
 def init_system_process():
     logs_path = os.path.join(os.getcwd(), 'logs')
     if not os.path.exists(logs_path):
         os.mkdir(logs_path)
     models.SystemProcess.objects.all().delete()
     name = 'system-process-default'
     log_file = os.path.join(logs_path, f'{name}.log')
     instance = models.SystemProcess(
         process_name=name,
         log_file=log_file
     )
-    process = ProcessManager.create(start_by_server, instance.log_file)
+    process = ProcessManager.create(start_system_client, instance.log_file)
     instance.process_id = process.pid
     instance.save()
 
 
 def init_system_data():
     from .models import builtins
     builtins.initialize()
@@ -57,15 +57,15 @@
         'description',
     )
     filter_horizontal = []
     list_filter = ('category', 'parent')
 
     def has_delete_permission(self, request, obj=None):
         if obj:
-            return obj.category != models.builtins.tasks.system_default_category
+            return obj.category != models.builtins.categories.system_default_category
         return True
 
 
 class SystemScheduleCallbackAdmin(base_admin.TaskScheduleCallbackAdmin):
     pass
 
 
@@ -77,15 +77,15 @@
     schedule_put_name = 'system_schedule_put'
     list_display = ('id', 'admin_task', 'schedule_type', 'schedule_sub_type', 'next_schedule_time',
                     'status', 'put', 'logs', 'update_time')
     list_filter = ('task__category', )
 
     def has_delete_permission(self, request, obj=None):
         if obj:
-            return obj.task.category != models.builtins.tasks.system_default_category
+            return obj.task.category != models.builtins.categories.system_default_category
         return True
 
 
 class SystemScheduleLogAdmin(base_admin.TaskScheduleLogAdmin):
     schedule_retry_name = 'system_schedule_retry'
```

#### html2text {}

```diff
@@ -1,50 +1,51 @@
 from django.contrib import admin from django.dispatch import receiver from
 django.shortcuts import reverse from django.utils.html import format_html from
 django.db.models.signals import post_delete from . import models from . import
 forms from .. import admin as base_admin from .process import ProcessManager
-from ..system_task_execution.main import start_by_server import os def
+from ..system_task_execution.main import start_system_client import os def
 init_system_process(): logs_path = os.path.join(os.getcwd(), 'logs') if not
 os.path.exists(logs_path): os.mkdir(logs_path) models.SystemProcess.objects.all
 ().delete() name = 'system-process-default' log_file = os.path.join(logs_path,
 f'{name}.log') instance = models.SystemProcess( process_name=name,
-log_file=log_file ) process = ProcessManager.create(start_by_server,
+log_file=log_file ) process = ProcessManager.create(start_system_client,
 instance.log_file) instance.process_id = process.pid instance.save() def
 init_system_data(): from .models import builtins builtins.initialize() if
 os.environ.get('RUN_MAIN') == 'true' and os.environ.get('RUN_CLIENT') !=
 'true': init_system_process() init_system_data() @receiver(post_delete,
 sender=models.SystemProcess) def delete_process(sender, instance:
 models.SystemProcess, **kwargs): ProcessManager.kill(instance.process_id) if
 os.path.isfile(instance.log_file) and not instance.log_file.endswith('system-
 process-default.log'): os.remove(instance.log_file) class SystemTaskAdmin
 (base_admin.TaskAdmin): form = forms.SystemTaskForm schedule_model =
 models.SystemSchedule list_display = ('id', 'admin_parent', 'name', 'category',
 'admin_status', 'schedules', 'update_time') fields = ( ("parent", 'category',),
 ('queue',), ("name", "status",), "config", 'description', ) filter_horizontal =
 [] list_filter = ('category', 'parent') def has_delete_permission(self,
 request, obj=None): if obj: return obj.category !=
-models.builtins.tasks.system_default_category return True class
+models.builtins.categories.system_default_category return True class
 SystemScheduleCallbackAdmin(base_admin.TaskScheduleCallbackAdmin): pass class
 SystemScheduleAdmin(base_admin.TaskScheduleAdmin): task_model =
 models.SystemTask schedule_log_model = models.SystemScheduleLog queues =
 models.builtins.queues schedule_put_name = 'system_schedule_put' list_display =
 ('id', 'admin_task', 'schedule_type', 'schedule_sub_type',
 'next_schedule_time', 'status', 'put', 'logs', 'update_time') list_filter =
 ('task__category', ) def has_delete_permission(self, request, obj=None): if
-obj: return obj.task.category != models.builtins.tasks.system_default_category
-return True class SystemScheduleLogAdmin(base_admin.TaskScheduleLogAdmin):
-schedule_retry_name = 'system_schedule_retry' class SystemProcessAdmin
-(admin.ModelAdmin): list_display = ('process_id', 'process_name', 'log_file',
-'status', 'stop_process', 'show_log', 'update_time') form =
-forms.SystemProcessForm fields = ( 'system_path', 'process_name', 'env',
-'log_file', 'process_id', 'create_time', ) readonly_fields = ('create_time',
-'update_time') def stop_process(self, obj): url = reverse
-('system_process_stop', args=(obj.process_id,)) return format_html( 'åæ­¢' %
-url ) stop_process.short_description = 'åæ­¢è¿è¡' def show_log(self, obj):
-url = reverse('system_process_log', args=(obj.process_id,)) return format_html
+obj: return obj.task.category !=
+models.builtins.categories.system_default_category return True class
+SystemScheduleLogAdmin(base_admin.TaskScheduleLogAdmin): schedule_retry_name =
+'system_schedule_retry' class SystemProcessAdmin(admin.ModelAdmin):
+list_display = ('process_id', 'process_name', 'log_file', 'status',
+'stop_process', 'show_log', 'update_time') form = forms.SystemProcessForm
+fields = ( 'system_path', 'process_name', 'env', 'log_file', 'process_id',
+'create_time', ) readonly_fields = ('create_time', 'update_time') def
+stop_process(self, obj): url = reverse('system_process_stop', args=
+(obj.process_id,)) return format_html( 'åæ­¢' % url )
+stop_process.short_description = 'åæ­¢è¿è¡' def show_log(self, obj): url =
+reverse('system_process_log', args=(obj.process_id,)) return format_html
 ( 'æ¥çæ¥å¿' % url ) show_log.short_description = 'æ¥å¿' def
 has_delete_permission(self, request, obj=None): return False class
 SystemScheduleQueueAdmin(base_admin.TaskScheduleQueueAdmin): form =
 forms.SystemScheduleQueueForm builtins = models.builtins schedule_get_name =
 'system_schedule_get' class SystemScheduleProducerAdmin
 (base_admin.TaskScheduleProducerAdmin): form = forms.SystemScheduleProducerForm
 schedule_get_name = 'system_schedule_get' builtins = models.builtins class
```

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/choices.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/forms.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from . import models
 from django import forms
 import os
 import time
 from .process import ProcessManager
-from ..system_task_execution.main import start_by_server
+from ..system_task_execution.main import start_system_client
 from django_common_task_system.forms import TaskScheduleProducerForm, TaskScheduleQueueForm
 
 
 class SystemTaskForm(forms.ModelForm):
     queue = forms.ModelChoiceField(
         queryset=models.SystemScheduleQueue.objects.all(),
         required=False,
@@ -75,15 +75,15 @@
             self.initial['log_file'] = os.path.join(logs_path,
                                                     'system-process-%s.log' % time.strftime('%Y%m%d%H%M%S'))
 
     def clean(self):
         cleaned_data = super(SystemProcessForm, self).clean()
         log_file = cleaned_data.get('log_file')
         try:
-            p = ProcessManager.create(start_by_server, log_file=log_file)
+            p = ProcessManager.create(start_system_client, log_file=log_file)
         except Exception as e:
             self.add_error('endpoint', '启动失败: %s' % e)
             cleaned_data['status'] = False
         else:
             cleaned_data['process_id'] = p.pid
             cleaned_data['status'] = p.is_alive()
         return cleaned_data
```

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/models.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from django.db import models
 from django.conf import settings
 from django_common_task_system.choices import ScheduleQueueModule, TaskScheduleStatus, ConsumerPermissionType
-from django_common_task_system.models import AbstractTask, AbstractTaskSchedule, AbstractTaskScheduleLog, \
-    TaskScheduleLog, AbstractScheduleCallback, \
-    AbstractTaskScheduleProducer, AbstractTaskScheduleQueue, AbstractConsumerPermission, \
-    BaseBuiltinQueues, BaseBuiltinProducers, BaseConsumerPermissions, system_initialize_signal
+from django_common_task_system.models import (
+    AbstractTask, AbstractTaskSchedule, AbstractTaskScheduleLog, TaskScheduleLog, AbstractScheduleCallback, 
+    AbstractTaskScheduleProducer, AbstractTaskScheduleQueue, AbstractConsumerPermission, 
+    BaseBuiltinQueues, BaseBuiltinProducers, BaseConsumerPermissions, BaseBuiltins, 
+    BuiltinModels
+)
 from django_common_objects.models import CommonCategory
 from django.contrib.auth import get_user_model
-import os
 
 User = get_user_model()
 
 
 class SystemTask(AbstractTask):
 
     class Meta(AbstractTask.Meta):
@@ -19,15 +20,15 @@
         db_table = 'system_task'
         verbose_name = verbose_name_plural = '系统任务'
 
     def save(
         self, force_insert=False, force_update=False, using=None, update_fields=None
     ):
         if self.category_id is None:
-            self.category = builtins.tasks.system_default_category
+            self.category = builtins.categories.system_default_category
         super().save(force_insert, force_update, using, update_fields)
 
 
 class SystemScheduleQueue(AbstractTaskScheduleQueue):
 
     class Meta(AbstractTaskScheduleQueue.Meta):
         db_table = 'system_schedule_queue'
@@ -102,371 +103,314 @@
         db_table = 'system_process'
         verbose_name = verbose_name_plural = '系统进程'
 
     def __str__(self):
         return "%s(%s)" % (self.process_name, self.process_id)
 
 
+class BuiltinCategories(BuiltinModels):
+    model = CommonCategory
+    model_unique_kwargs = ('name',)
+
+    def __init__(self, user):
+        model = SystemTask._meta.label
+        self.system_default_category = self.model(
+            name='系统任务',
+            model=model,
+            user=user,
+        )
+
+        self.system_base_category = self.model(
+            name='系统基础',
+            model=model,
+            user=user,
+        )
+
+        self.system_test_category = self.model(
+            name='系统测试',
+            model=model,
+            user=user,
+        )
+        super(BuiltinCategories, self).__init__()
+
+
 class BuiltinQueues(BaseBuiltinQueues):
     model = SystemScheduleQueue
 
     def __init__(self):
-        self.opening: SystemScheduleQueue = self.model.objects.get_or_create(
+        self.opening = self.model(
             code=self.status_params_mapping[TaskScheduleStatus.OPENING.value],
-            defaults={
-                'status': True,
-                'module': ScheduleQueueModule.QUEUE.value,
-                'name': '系统任务队列'
-            }
-        )[0]
+            status=True,
+            module=ScheduleQueueModule.QUEUE.value,
+            name='系统任务队列'
+        )
 
-        self.test = self.model.objects.get_or_create(
+        self.test = self.model(
             code=self.status_params_mapping[TaskScheduleStatus.TEST.value],
-            defaults={
-                'status': True,
-                'module': ScheduleQueueModule.QUEUE.value,
-                'name': '测试任务队列'
-            }
-        )[0]
+            status=True,
+            module=ScheduleQueueModule.QUEUE.value,
+            name='测试任务队列'
+        )
         super(BuiltinQueues, self).__init__()
 
 
 class BuiltinProducers(BaseBuiltinProducers):
     model = SystemScheduleProducer
 
     def __init__(self, queues: BuiltinQueues):
-        self.opening = SystemScheduleProducer.objects.get_or_create(
+        self.opening = self.model(
             queue=queues.opening,
             lte_now=True,
-            defaults={
-                'filters': {
-                    'status': TaskScheduleStatus.OPENING.value,
-                },
-                'status': True,
-                'name': '默认'
-            }
-        )[0]
-        self.test = SystemScheduleProducer.objects.get_or_create(
+            filters={
+                'status': TaskScheduleStatus.OPENING.value,
+            },
+            status=True,
+            name='默认'
+        )
+        self.test = self.model(
             queue=queues.test,
             lte_now=True,
-            defaults={
-                'filters': {
-                    'status': TaskScheduleStatus.TEST.value,
-                },
-                'status': True,
-                'name': '测试'
-            }
-        )[0]
+            filters={
+                'status': TaskScheduleStatus.TEST.value,
+            },
+            status=True,
+            name='测试'
+        )
         super(BuiltinProducers, self).__init__()
 
 
-class BuiltinTasks:
+class BuiltinTasks(BuiltinModels):
+    model = SystemTask
+    model_unique_kwargs = ['name', 'user', 'parent', 'category']
 
-    def __init__(self, user, queues: BuiltinQueues):
-        self.system_default_category = CommonCategory.objects.get_or_create(
-            name='系统任务',
-            model=SystemTask._meta.label,
-            user=user,
-        )[0]
+    def __init__(self, categories: BuiltinCategories, queues: BuiltinQueues):
+        user = categories.system_default_category.user
 
-        self.system_base_category = CommonCategory.objects.get_or_create(
-            name='系统基础',
-            model=SystemTask._meta.label,
-            user=user,
-        )[0]
-
-        self.system_test_category = CommonCategory.objects.get_or_create(
-            name='系统测试',
-            model=SystemTask._meta.label,
-            user=user,
-        )[0]
-
-        self.shell_execution_parent_task = SystemTask.objects.get_or_create(
+        self.shell_execution_parent_task = self.model(
             name='Shell执行',
             user=user,
-            category=self.system_base_category,
-            defaults={
-                'config': {
-                    'required_fields': ['shell'],
-                }
-            },
-        )[0]
-
-        self.sql_execution_parent_task = SystemTask.objects.get_or_create(
+            category=categories.system_base_category,
+            config={
+                'required_fields': ['shell'],
+            }
+        )
+        self.sql_execution_parent_task = self.model(
             name='SQL执行',
             user=user,
-            category=self.system_base_category,
-            defaults={
-                'config': {
-                    'required_fields': ['sql'],
-                }
-            },
-        )[0]
+            category=categories.system_base_category,
+            config={
+                'required_fields': ['sql'],
+            }
+        )
 
-        self.sql_produce_parent_task = SystemTask.objects.get_or_create(
+        self.sql_produce_parent_task = self.model(
             name='SQL生产',
             user=user,
-            category=self.system_base_category,
-            defaults={
-                'config': {
-                    'required_fields': ['sql', 'queue'],
-                }
-            },
-        )[0]
+            category=categories.system_base_category,
+            config={
+                'required_fields': ['sql', 'queue'],
+            }
+        )
 
         interval = 1
         unit = 'month'
-        self.system_log_cleaning = SystemTask.objects.get_or_create(
+        self.system_log_cleaning = self.model(
             name='系统日志清理',
             parent=self.sql_execution_parent_task,
-            category=self.system_default_category,
+            category=categories.system_default_category,
             user=user,
-            defaults={
-                'config': {
-                    'sql': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
-                           (SystemScheduleLog._meta.db_table, interval, unit)
-                },
-            }
-        )[0]
+            config={
+                'sql': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
+                       (SystemScheduleLog._meta.db_table, interval, unit)
+            },
+        )
 
         max_retry_times = 5
-        self.system_exception_handling = SystemTask.objects.get_or_create(
+        self.system_exception_handling = self.model(
             name='系统异常处理',
             user=user,
-            category=self.system_default_category,
-            defaults={
-                'config': {
-                    'max_retry_times': max_retry_times,
-                },
-            }
-        )[0]
+            category=categories.system_default_category,
+            config={
+                'max_retry_times': max_retry_times,
+            },
+        )
 
         interval = 1
         unit = 'month'
-        self.task_log_cleaning = SystemTask.objects.get_or_create(
+        self.task_log_cleaning = self.model(
             name='任务日志清理',
             user=user,
-            category=self.system_default_category,
+            category=categories.system_default_category,
             parent=self.sql_execution_parent_task,
-            defaults={
-                'config': {
-                    'sql': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
-                           (TaskScheduleLog._meta.db_table, interval, unit)
-                },
-            }
-        )[0]
+            config={
+                'sql': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
+                       (TaskScheduleLog._meta.db_table, interval, unit)
+            },
+        )
 
         max_retry_times = 5
-        self.task_exception_handling = SystemTask.objects.get_or_create(
+        self.task_exception_handling = self.model(
             name='任务异常处理',
             user=user,
-            category=self.system_default_category,
-            defaults={
-                'config': {
-                    'max_retry_times': max_retry_times,
-                },
-            }
-        )[0]
+            category=categories.system_default_category,
+            config={
+                'max_retry_times': max_retry_times,
+            },
+        )
 
-        self.test_sql_execution = SystemTask.objects.get_or_create(
+        self.test_sql_execution = self.model(
             name='测试SQL执行任务',
             parent=self.sql_execution_parent_task,
-            category=self.system_test_category,
+            category=categories.system_test_category,
             config={
                 'sql': 'select * from %s limit 10;' % SystemScheduleLog._meta.db_table
             },
             user=user
-        )[0]
+        )
 
-        self.test_sql_produce = SystemTask.objects.get_or_create(
+        self.test_sql_produce = self.model(
             name='测试SQL生产任务',
             parent=self.sql_produce_parent_task,
-            category=self.system_test_category,
+            category=categories.system_test_category,
             config={
                 'sql': 'select * from %s limit 10;' % SystemScheduleLog._meta.db_table,
                 'queue': queues.test.code
             },
             user=user
-        )[0]
-        self.test_shell_execution = SystemTask.objects.get_or_create(
+        )
+        self.test_shell_execution = self.model(
             name='测试Shell执行任务',
             parent=self.shell_execution_parent_task,
-            category=self.system_test_category,
+            category=categories.system_test_category,
             config={
                 'shell': 'echo "hello world"'
             },
             user=user
-        )[0]
+        )
+        super(BuiltinTasks, self).__init__()
 
 
-class BuiltinSchedules:
+class BuiltinSchedules(BuiltinModels):
+    model_unique_kwargs = ['task', 'user']
+    model = SystemSchedule
 
     def __init__(self, user, tasks: BuiltinTasks):
-        self.system_log_cleaning = SystemSchedule.objects.get_or_create(
+        self.system_log_cleaning = self.model(
             task=tasks.system_log_cleaning,
             user=user,
-            defaults={
-                'config': {
-                    "T": {
-                        "DAY": {
-                            "period": 1
-                        },
-                        "time": "01:00:00",
-                        "type": "DAY"
+            config={
+                "T": {
+                    "DAY": {
+                        "period": 1
                     },
-                    "base_on_now": True,
-                    "schedule_type": "T"
-                }
-            },
-        )[0]
+                    "time": "01:00:00",
+                    "type": "DAY"
+                },
+                "base_on_now": True,
+                "schedule_type": "T"
+            }
+        )
 
-        self.system_exception_handling = SystemSchedule.objects.get_or_create(
+        self.system_exception_handling = self.model(
             task=tasks.system_exception_handling,
             user=user,
-            defaults={
-                'config': {
-                    "S": {
-                        "period": 60,
-                        "schedule_start_time": "2023-04-04 15:31:00"
-                    },
-                    "base_on_now": True,
-                    "schedule_type": "S"
-                }
+            config={
+                "S": {
+                    "period": 60,
+                    "schedule_start_time": "2023-04-04 15:31:00"
+                },
+                "base_on_now": True,
+                "schedule_type": "S"
             }
-        )[0]
+        )
 
-        self.task_log_cleaning = SystemSchedule.objects.get_or_create(
+        self.task_log_cleaning = self.model(
             task=tasks.task_log_cleaning,
             user=user,
-            defaults={
-                'config': {
-                    "T": {
-                        "DAY": {
-                            "period": 1
-                        },
-                        "time": "01:00:00",
-                        "type": "DAY"
+            config={
+                "T": {
+                    "DAY": {
+                        "period": 1
                     },
-                    "base_on_now": True,
-                    "schedule_type": "T"
-                }
+                    "time": "01:00:00",
+                    "type": "DAY"
+                },
+                "base_on_now": True,
+                "schedule_type": "T"
             }
-        )[0]
+        )
 
-        self.task_exception_handling = SystemSchedule.objects.get_or_create(
+        self.task_exception_handling = self.model(
             task=tasks.task_exception_handling,
             user=user,
-            defaults={
-                'config': {
-                    "S": {
-                        "period": 60,
-                        "schedule_start_time": "2023-04-04 15:31:00"
-                    },
-                    "base_on_now": True,
-                    "schedule_type": "S"
-                }
+            config={
+                "S": {
+                    "period": 60,
+                    "schedule_start_time": "2023-04-04 15:31:00"
+                },
+                "base_on_now": True,
+                "schedule_type": "S"
             }
-        )[0]
+        )
 
-        defaults = {
+        config = {
             'config': {
                 "S": {
                     "period": 60,
                     "schedule_start_time": "2023-04-04 15:31:00"
                 },
                 "base_on_now": True,
                 "schedule_type": "S"
             }
         }
 
-        self.test_sql_execution = SystemSchedule.objects.get_or_create(
+        self.test_sql_execution = self.model(
             task=tasks.test_sql_execution,
             user=user,
             status=TaskScheduleStatus.TEST.value,
-            defaults=defaults
-        )[0]
-        self.test_sql_produce = SystemSchedule.objects.get_or_create(
+            config=config
+        )
+        self.test_sql_produce = self.model(
             task=tasks.test_sql_produce,
             user=user,
             status=TaskScheduleStatus.TEST.value,
-            defaults=defaults
-        )[0]
-        self.test_shell_execution = SystemSchedule.objects.get_or_create(
+            config=config
+        )
+        self.test_shell_execution = self.model(
             task=tasks.test_shell_execution,
             user=user,
             status=TaskScheduleStatus.TEST.value,
-            defaults=defaults
-        )[0]
+            config=config
+        )
+
+        super(BuiltinSchedules, self).__init__()
 
 
 class BuiltinConsumerPermissions(BaseConsumerPermissions):
     model = SystemConsumerPermission
 
     def __init__(self, producers: BuiltinProducers):
-        self.system_consumer_permission = self.model.objects.get_or_create(
+        self.system_consumer_permission = self.model(
             producer=producers.opening,
             type=ConsumerPermissionType.IP_WHITE_LIST.value,
-            defaults={
-                'status': True,
-                'config': {
-                    'ip_whitelist': ['127.0.0.1'],
-                }
+            status=True,
+            config={
+                'ip_whitelist': ['127.0.0.1']
             }
-        )[0]
+        )
         super(BuiltinConsumerPermissions, self).__init__()
 
 
-class Builtins:
+class Builtins(BaseBuiltins):
+    app = 'django_common_task_system.system_task'
 
     def __init__(self):
-        self._initialized = False
-        self._tasks = None
-        self._schedules = None
-        self._queues = None
-        self._producers = None
-        self._consumer_permissions = None
-
-    def initialize(self):
-        if not self._initialized:
-            if os.environ.get('RUN_MAIN') == 'true':# and os.environ.get('RUN_CLIENT') != 'true':
-                self._initialized = True
-                from django.conf import settings
-                if 'django_common_task_system.system_task' in settings.INSTALLED_APPS:
-                    print('初始化系统内置任务')
-                    user = User.objects.filter(is_superuser=True).order_by('id').first()
-                    if not user:
-                        raise Exception('未找到超级管理员')
-                    self._queues = BuiltinQueues()
-                    self._producers = BuiltinProducers(self._queues)
-                    self._tasks = BuiltinTasks(user, self._queues)
-                    self._schedules = BuiltinSchedules(user, self._tasks)
-                    self._consumer_permissions = BuiltinConsumerPermissions(self._producers)
-                    system_initialize_signal.send(sender='builtin_initialized',
-                                                    app='django_common_task_system.system_task')
-
-    @property
-    def tasks(self) -> BuiltinTasks:
-        self.initialize()
-        return self._tasks
-
-    @property
-    def schedules(self) -> BuiltinSchedules:
-        self.initialize()
-        return self._schedules
-
-    @property
-    def queues(self) -> BuiltinQueues:
-        self.initialize()
-        return self._queues
-
-    @property
-    def producers(self) -> BuiltinProducers:
-        self.initialize()
-        return self._producers
-
-    @property
-    def consumer_permissions(self) -> BuiltinConsumerPermissions:
-        self.initialize()
-        return self._consumer_permissions
+        super(Builtins, self).__init__()
+        self.queues = BuiltinQueues()
+        self.categories = BuiltinCategories(self.user)
+        self.tasks = BuiltinTasks(self.categories, self.queues)
+        self.schedules = BuiltinSchedules(self.user, self.tasks)
+        self.producers = BuiltinProducers(self.queues)
+        self.consumer_permissions = BuiltinConsumerPermissions(self.producers)
 
 
 builtins = Builtins()
```

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/process.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/process.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/queue.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/queue.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/serializers.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task/views.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task_execution/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 import os
 import argparse
 import sys
 import logging
 from logging.handlers import RotatingFileHandler
 
 
-def start_by_server(log_file=None, **kwargs):
+def start_system_client(log_file=None, **kwargs):
     os.environ['RUN_CLIENT'] = 'true'
-    import django
-    django.setup()
-
-    from .system_task_execution.executor import start_client
-    from .system_task_execution import settings
-    logger = settings.logger
-    logger.handlers.clear()
-    if not os.path.exists(os.path.dirname(log_file)):
-        os.makedirs(os.path.dirname(log_file))
-    if os.path.isfile(log_file):
-        os.remove(log_file)
-    handler = RotatingFileHandler(log_file, maxBytes=1024 * 1024 * 10, encoding='utf-8', backupCount=5)
-    formatter = logging.Formatter('[%(asctime)s][%(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
-    handler.setFormatter(formatter)
-    logger.addHandler(handler)
-    logger.setLevel(logging.INFO)
-
-    start_client(**kwargs)
-
-
-if __name__ == '__main__':
-    import django
     parser = argparse.ArgumentParser()
     parser.add_argument('--system-path', type=str, required=False)
     parser.add_argument('--system-setting', type=str, required=False)
-    shell_args = parser.parse_args()
+    shell_args = parser.parse_known_args()[0]
     if shell_args.system_path:
         assert os.path.exists(shell_args.system_path), 'system path not found'
         sys.path.append(shell_args.system_path)
     env = shell_args.system_setting or os.environ.get('DJANGO_SETTINGS_MODULE')
     assert env, 'django settings module not found'
     os.environ.setdefault('DJANGO_SETTINGS_MODULE', env)
-    os.environ['RUN_CLIENT'] = 'true'
+    import django
     django.setup()
 
+    if log_file:
+        from .system_task_execution import settings
+        logger = settings.logger
+        logger.handlers.clear()
+        if not os.path.exists(os.path.dirname(log_file)):
+            os.makedirs(os.path.dirname(log_file))
+        if os.path.isfile(log_file):
+            os.remove(log_file)
+        handler = RotatingFileHandler(log_file, maxBytes=1024 * 1024 * 10, encoding='utf-8', backupCount=5)
+        formatter = logging.Formatter('[%(asctime)s][%(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
+        logger.setLevel(logging.INFO)
+
     from django_common_task_system.system_task_execution.system_task_execution.executor import start_client
-    start_client()
+    start_client(**kwargs)
+
+
+if __name__ == '__main__':
+    start_system_client()
```

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executor.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import os
 import time
-import copy
 import requests
-from queue import Queue, Empty
+from queue import Queue
 from datetime import datetime
 from django.urls import reverse
 from .executors import Executors
 from . import settings
 from urllib.parse import urljoin
-from django_common_task_system.system_task.models import SystemSchedule, SystemTask
+from django_common_task_system.system_task.models import SystemSchedule, SystemTask, builtins
 from django_common_task_system.models import TaskScheduleCallback
 
 
 system_task_queue = Queue()
 logger = settings.logger
 
 
-def request_system_schedule():
-
-    url = urljoin(settings.HOST, reverse('system_schedule_get', args=('opening', )))
+def request_system_schedule(url):
     response = requests.get(url)
     if response.status_code == 200:
         result = response.json()
         callback = result.pop('callback')
         if callback:
             callback = TaskScheduleCallback(**callback)
         task = result.pop('task')
@@ -42,17 +39,17 @@
             **result
         )
         schedule.queue = queue
         return schedule
         # system_task_queue.put(schedule)
 
 
-def get_system_schedule():
+def get_system_schedule(url):
     while True:
-        schedule = request_system_schedule()
+        schedule = request_system_schedule(url)
         if schedule:
             return schedule
         time.sleep(1)
 
 
 def get_schedule_executor(schedule):
     try:
@@ -63,25 +60,26 @@
         try:
             cls = Executors[schedule.task.name]
         except KeyError:
             raise RuntimeError('executor not found for task name: %s' % schedule.task.name)
     return cls(schedule)
 
 
-def run():
-    schedule = get_system_schedule()
-    logger.info('get system schedule: %s', schedule)
+def run(schedule):
     executor = get_schedule_executor(schedule)
     log, err = executor.start()
     if not err:
         logger.info('system schedule execute success: %s', log.result)
 
 
-def start_client(**kwargs):
+def start_client(queue=None, **kwargs):
     logger.info('system executor start')
     for k, v in os.environ.items():
         logger.info('Env: %s -> %s' % (k, v))
+    consumer_url = urljoin(settings.HOST, reverse('system_schedule_get', args=(queue or builtins.queues.opening.code,)))
     while True:
         try:
-            run()
+            schedule = get_system_schedule(consumer_url)
+            logger.info('get system schedule: %s', schedule)
+            run(schedule)
         except Exception as e:
             logger.exception(e)
```

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py` & `django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/templates/admin/system_schedule/change_list.html` & `django-common-task-system-1.2.0/django_common_task_system/templates/admin/system_schedule/change_list.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/urls.py` & `django-common-task-system-1.2.0/django_common_task_system/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.2.0/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/utils/foreign_key.py` & `django-common-task-system-1.2.0/django_common_task_system/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.2.0/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/django_common_task_system/views.py` & `django-common-task-system-1.2.0/django_common_task_system/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from rest_framework.decorators import api_view
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.views import APIView
 from rest_framework.viewsets import ModelViewSet
 from django.http.response import JsonResponse
 from . import serializers, get_task_model, get_schedule_log_model, get_task_schedule_model, get_task_schedule_serializer
-from .models import TaskSchedule, TaskScheduleProducer, TaskScheduleQueue, ConsumerPermission, builtins
+from .choices import TaskScheduleStatus
+from .models import TaskSchedule, TaskScheduleProducer, TaskScheduleQueue, ConsumerPermission, builtins, ScheduleConfig
 from django_common_objects.rest_view import UserListAPIView, UserRetrieveAPIView
 from queue import Empty
 from datetime import datetime
 from jionlp_time import parse_time
 from .utils.schedule_time import nlp_config_to_schedule_config
 from .models import system_initialize_signal, system_schedule_event
 from threading import Thread
@@ -34,32 +35,41 @@
     queues = builtins.queues
     serializer = ScheduleSerializer
 
     def __init__(self):
         super().__init__(daemon=True)
 
     def produce(self):
+        now = datetime.now()
         for producer in self.producers.values():
             queue = self.queues[producer.queue.code]
             # 队列长度大于1000时不再生产, 防止内存溢出
             if queue.queue.qsize() > 1000:
                 continue
             queryset = self.schedule_model.objects.filter(**producer.filters)
             if producer.lte_now:
                 queryset = queryset.filter(next_schedule_time__lte=datetime.now())
             for schedule in queryset:
-                data = self.serializer(schedule).data
-                data['queue'] = queue.code
-                queue.queue.put(data)
-                schedule.generate_next_schedule()
+                try:
+                    while schedule.next_schedule_time <= now:
+                        data = self.serializer(schedule).data
+                        data['queue'] = queue.code
+                        queue.queue.put(data)
+                        schedule.next_schedule_time = ScheduleConfig(config=schedule.config
+                                                                     ).get_next_time(schedule.next_schedule_time)
+                    schedule.save(update_fields=('next_schedule_time', ))
+                except Exception as e:
+                    schedule.status = TaskScheduleStatus.ERROR.value
+                    schedule.save(update_fields=('status',))
+                    traceback.print_exc()
 
     def run(self) -> None:
         # 等待系统初始化完成, 5秒后自动开始
         system_schedule_event.wait(timeout=5)
-        while system_schedule_event.is_set():
+        while True:
             try:
                 self.produce()
             except Exception as err:
                 traceback.print_exc()
             time.sleep(0.5)
```

### Comparing `django-common-task-system-1.1.9/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.2.0/django_common_task_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.1.9/setup.py` & `django-common-task-system-1.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
     packages=find_packages(exclude=['local_tests']),
-    version='1.1.9',
+    version='1.2.0',
     install_requires=[
         "django-common-objects>=1.0.5",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
```

