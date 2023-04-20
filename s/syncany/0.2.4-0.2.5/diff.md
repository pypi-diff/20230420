# Comparing `tmp/syncany-0.2.4.tar.gz` & `tmp/syncany-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncany-0.2.4.tar", last modified: Wed Apr 19 09:45:41 2023, max compression
+gzip compressed data, was "syncany-0.2.5.tar", last modified: Thu Apr 20 08:44:39 2023, max compression
```

## Comparing `syncany-0.2.4.tar` & `syncany-0.2.5.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:45:41.315862 syncany-0.2.4/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2022-08-13 12:36:15.000000 syncany-0.2.4/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-19 09:45:41.317863 syncany-0.2.4/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5832 2022-08-13 12:36:15.000000 syncany-0.2.4/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-19 09:45:41.326862 syncany-0.2.4/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1928 2023-04-19 08:35:11.000000 syncany-0.2.4/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:45:35.850699 syncany-0.2.4/syncany/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      607 2023-04-19 08:35:11.000000 syncany-0.2.4/syncany/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:45:36.591003 syncany-0.2.4/syncany/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3587 2023-03-28 01:46:34.000000 syncany-0.2.4/syncany/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    39302 2023-04-19 07:06:22.000000 syncany-0.2.4/syncany/calculaters/builtin.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4394 2023-03-24 09:30:00.000000 syncany-0.2.4/syncany/calculaters/calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7999 2023-03-27 08:30:23.000000 syncany-0.2.4/syncany/calculaters/convert_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4573 2023-03-23 03:10:08.000000 syncany-0.2.4/syncany/calculaters/datetime_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2255 2023-03-23 03:10:08.000000 syncany-0.2.4/syncany/calculaters/import_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3167 2023-03-23 03:10:08.000000 syncany-0.2.4/syncany/calculaters/textline_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13697 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/calculaters/transform_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:45:37.681356 syncany-0.2.4/syncany/database/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4055 2023-03-28 03:25:41.000000 syncany-0.2.4/syncany/database/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8756 2023-03-24 06:27:35.000000 syncany-0.2.4/syncany/database/beanstalk.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15303 2023-02-24 09:40:27.000000 syncany-0.2.4/syncany/database/clickhouse.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15571 2023-03-25 11:28:20.000000 syncany-0.2.4/syncany/database/csv.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10626 2023-02-23 11:47:13.000000 syncany-0.2.4/syncany/database/database.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12481 2023-02-24 09:33:28.000000 syncany-0.2.4/syncany/database/elasticsearch.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14331 2023-03-24 06:27:35.000000 syncany-0.2.4/syncany/database/excel.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14218 2023-02-22 05:00:17.000000 syncany-0.2.4/syncany/database/http.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    17931 2023-02-24 09:33:28.000000 syncany-0.2.4/syncany/database/influxdb.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11892 2023-03-24 06:27:35.000000 syncany-0.2.4/syncany/database/json.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11786 2023-03-24 06:27:35.000000 syncany-0.2.4/syncany/database/memory.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14344 2023-02-24 09:35:33.000000 syncany-0.2.4/syncany/database/mongodb.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14437 2023-02-24 09:28:32.000000 syncany-0.2.4/syncany/database/mysql.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14572 2023-02-24 09:33:28.000000 syncany-0.2.4/syncany/database/postgresql.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    17848 2023-03-24 06:27:35.000000 syncany-0.2.4/syncany/database/redis.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13949 2023-03-28 03:39:46.000000 syncany-0.2.4/syncany/database/sqlite.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15203 2023-02-24 09:28:33.000000 syncany-0.2.4/syncany/database/sqlserver.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    17813 2023-03-25 11:15:36.000000 syncany-0.2.4/syncany/database/textline.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      685 2022-08-23 12:03:29.000000 syncany-0.2.4/syncany/errors.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:45:37.856989 syncany-0.2.4/syncany/filters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      996 2023-03-25 04:34:57.000000 syncany-0.2.4/syncany/filters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    19439 2023-04-01 08:20:13.000000 syncany-0.2.4/syncany/filters/builtin.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      309 2022-08-13 12:36:15.000000 syncany-0.2.4/syncany/filters/filter.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2023-02-16 02:10:09.000000 syncany-0.2.4/syncany/hook.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:45:38.287635 syncany-0.2.4/syncany/loaders/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      927 2023-03-25 04:34:57.000000 syncany-0.2.4/syncany/loaders/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1401 2023-02-10 08:39:32.000000 syncany-0.2.4/syncany/loaders/cache.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1148 2023-03-21 06:16:11.000000 syncany-0.2.4/syncany/loaders/const.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6106 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/loaders/db.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9117 2023-03-30 02:17:02.000000 syncany-0.2.4/syncany/loaders/db_join.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1752 2023-02-24 04:31:16.000000 syncany-0.2.4/syncany/loaders/db_pull.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8808 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/loaders/loader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      214 2022-08-13 12:36:15.000000 syncany-0.2.4/syncany/logger.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13966 2023-03-24 04:36:02.000000 syncany-0.2.4/syncany/main.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:45:38.702443 syncany-0.2.4/syncany/outputers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1161 2023-03-25 04:34:57.000000 syncany-0.2.4/syncany/outputers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1491 2023-02-24 04:31:16.000000 syncany-0.2.4/syncany/outputers/db.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1920 2023-02-15 06:50:55.000000 syncany-0.2.4/syncany/outputers/db_delete_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      887 2022-08-13 12:36:15.000000 syncany-0.2.4/syncany/outputers/db_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5697 2023-03-18 13:41:32.000000 syncany-0.2.4/syncany/outputers/db_update_delete_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4209 2023-03-18 13:41:32.000000 syncany-0.2.4/syncany/outputers/db_update_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2864 2023-03-22 02:35:53.000000 syncany-0.2.4/syncany/outputers/outputer.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:45:38.992216 syncany-0.2.4/syncany/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       52 2022-08-13 12:36:15.000000 syncany-0.2.4/syncany/taskers/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:45:39.488168 syncany-0.2.4/syncany/taskers/config/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1794 2023-03-25 04:34:57.000000 syncany-0.2.4/syncany/taskers/config/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      405 2022-08-23 12:07:09.000000 syncany-0.2.4/syncany/taskers/config/file_reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      937 2022-08-23 12:07:09.000000 syncany-0.2.4/syncany/taskers/config/http_reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      195 2022-08-13 12:36:15.000000 syncany-0.2.4/syncany/taskers/config/json_parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      208 2022-08-13 12:36:15.000000 syncany-0.2.4/syncany/taskers/config/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      204 2022-08-23 11:55:44.000000 syncany-0.2.4/syncany/taskers/config/reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5006 2022-08-13 12:36:15.000000 syncany-0.2.4/syncany/taskers/config/yaml_parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1377 2023-02-24 02:44:01.000000 syncany-0.2.4/syncany/taskers/context.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:45:39.945435 syncany-0.2.4/syncany/taskers/core/
--rwxrwxrwx   0 snower    (1000) snower    (1000)    72944 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/taskers/core/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2192 2023-03-21 06:17:51.000000 syncany-0.2.4/syncany/taskers/core/loader_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      256 2022-08-13 12:36:15.000000 syncany-0.2.4/syncany/taskers/core/option.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2592 2023-02-10 08:39:32.000000 syncany-0.2.4/syncany/taskers/core/outputer_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4736 2022-08-13 12:36:15.000000 syncany-0.2.4/syncany/taskers/core/states.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15689 2023-02-25 11:47:43.000000 syncany-0.2.4/syncany/taskers/core/valuer_compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    40757 2023-03-24 06:10:54.000000 syncany-0.2.4/syncany/taskers/core/valuer_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      760 2023-02-25 12:43:51.000000 syncany-0.2.4/syncany/taskers/iterator.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      245 2022-08-13 12:36:15.000000 syncany-0.2.4/syncany/taskers/manager.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7122 2023-02-25 03:46:05.000000 syncany-0.2.4/syncany/taskers/tasker.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9961 2023-03-27 02:39:01.000000 syncany-0.2.4/syncany/utils.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:45:41.268033 syncany-0.2.4/syncany/valuers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2098 2023-03-25 04:34:57.000000 syncany-0.2.4/syncany/valuers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4574 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/aggregate.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3714 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/assign.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5209 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/cache.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3956 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/calculate.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6445 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/call.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5526 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/case.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4729 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/condition.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      548 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/const.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2965 2023-03-30 01:52:08.000000 syncany-0.2.4/syncany/valuers/data.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5059 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/db_join.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2043 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/db_load.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1877 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/function.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6018 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/generator.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3468 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/inherit.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3379 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/let.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12327 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/loop.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7510 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/make.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10283 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/match.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1247 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/schema.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4336 2023-03-29 08:52:57.000000 syncany-0.2.4/syncany/valuers/state.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6066 2023-03-30 01:52:08.000000 syncany-0.2.4/syncany/valuers/valuer.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:45:36.111084 syncany-0.2.4/syncany.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-19 09:45:33.000000 syncany-0.2.4/syncany.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2889 2023-04-19 09:45:35.000000 syncany-0.2.4/syncany.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-19 09:45:33.000000 syncany-0.2.4/syncany.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       47 2023-04-19 09:45:33.000000 syncany-0.2.4/syncany.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2022-08-15 03:43:33.000000 syncany-0.2.4/syncany.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      371 2023-04-19 09:45:33.000000 syncany-0.2.4/syncany.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        8 2023-04-19 09:45:33.000000 syncany-0.2.4/syncany.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:39.483163 syncany-0.2.5/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2022-08-13 12:36:15.000000 syncany-0.2.5/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-20 08:44:39.484190 syncany-0.2.5/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5832 2022-08-13 12:36:15.000000 syncany-0.2.5/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-20 08:44:39.494187 syncany-0.2.5/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1928 2023-04-20 03:39:41.000000 syncany-0.2.5/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:34.324661 syncany-0.2.5/syncany/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      607 2023-04-20 03:39:41.000000 syncany-0.2.5/syncany/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:35.054704 syncany-0.2.5/syncany/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3587 2023-04-20 05:48:06.000000 syncany-0.2.5/syncany/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    39302 2023-04-19 07:06:22.000000 syncany-0.2.5/syncany/calculaters/builtin.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4394 2023-03-24 09:30:00.000000 syncany-0.2.5/syncany/calculaters/calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7999 2023-03-27 08:30:23.000000 syncany-0.2.5/syncany/calculaters/convert_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4573 2023-03-23 03:10:08.000000 syncany-0.2.5/syncany/calculaters/datetime_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2255 2023-03-23 03:10:08.000000 syncany-0.2.5/syncany/calculaters/import_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3167 2023-03-23 03:10:08.000000 syncany-0.2.5/syncany/calculaters/textline_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13697 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/calculaters/transform_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:36.043453 syncany-0.2.5/syncany/database/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4055 2023-03-28 03:25:41.000000 syncany-0.2.5/syncany/database/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8756 2023-03-24 06:27:35.000000 syncany-0.2.5/syncany/database/beanstalk.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15303 2023-02-24 09:40:27.000000 syncany-0.2.5/syncany/database/clickhouse.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15571 2023-03-25 11:28:20.000000 syncany-0.2.5/syncany/database/csv.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10626 2023-02-23 11:47:13.000000 syncany-0.2.5/syncany/database/database.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12481 2023-02-24 09:33:28.000000 syncany-0.2.5/syncany/database/elasticsearch.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14331 2023-03-24 06:27:35.000000 syncany-0.2.5/syncany/database/excel.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14218 2023-02-22 05:00:17.000000 syncany-0.2.5/syncany/database/http.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    17931 2023-02-24 09:33:28.000000 syncany-0.2.5/syncany/database/influxdb.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11892 2023-03-24 06:27:35.000000 syncany-0.2.5/syncany/database/json.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11786 2023-03-24 06:27:35.000000 syncany-0.2.5/syncany/database/memory.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14344 2023-02-24 09:35:33.000000 syncany-0.2.5/syncany/database/mongodb.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14437 2023-02-24 09:28:32.000000 syncany-0.2.5/syncany/database/mysql.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14572 2023-02-24 09:33:28.000000 syncany-0.2.5/syncany/database/postgresql.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    17848 2023-03-24 06:27:35.000000 syncany-0.2.5/syncany/database/redis.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13949 2023-03-28 03:39:46.000000 syncany-0.2.5/syncany/database/sqlite.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15203 2023-02-24 09:28:33.000000 syncany-0.2.5/syncany/database/sqlserver.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    17813 2023-03-25 11:15:36.000000 syncany-0.2.5/syncany/database/textline.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      685 2022-08-23 12:03:29.000000 syncany-0.2.5/syncany/errors.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:36.216452 syncany-0.2.5/syncany/filters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      996 2023-03-25 04:34:57.000000 syncany-0.2.5/syncany/filters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    19439 2023-04-01 08:20:13.000000 syncany-0.2.5/syncany/filters/builtin.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      309 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/filters/filter.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2023-02-16 02:10:09.000000 syncany-0.2.5/syncany/hook.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:36.590473 syncany-0.2.5/syncany/loaders/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      927 2023-03-25 04:34:57.000000 syncany-0.2.5/syncany/loaders/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1401 2023-02-10 08:39:32.000000 syncany-0.2.5/syncany/loaders/cache.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1148 2023-03-21 06:16:11.000000 syncany-0.2.5/syncany/loaders/const.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6106 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/loaders/db.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9117 2023-03-30 02:17:02.000000 syncany-0.2.5/syncany/loaders/db_join.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1752 2023-02-24 04:31:16.000000 syncany-0.2.5/syncany/loaders/db_pull.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8751 2023-04-20 05:37:24.000000 syncany-0.2.5/syncany/loaders/loader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      214 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/logger.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13966 2023-03-24 04:36:02.000000 syncany-0.2.5/syncany/main.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:36.977243 syncany-0.2.5/syncany/outputers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1161 2023-03-25 04:34:57.000000 syncany-0.2.5/syncany/outputers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1491 2023-02-24 04:31:16.000000 syncany-0.2.5/syncany/outputers/db.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1920 2023-02-15 06:50:55.000000 syncany-0.2.5/syncany/outputers/db_delete_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      887 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/outputers/db_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5697 2023-03-18 13:41:32.000000 syncany-0.2.5/syncany/outputers/db_update_delete_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4209 2023-03-18 13:41:32.000000 syncany-0.2.5/syncany/outputers/db_update_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2864 2023-03-22 02:35:53.000000 syncany-0.2.5/syncany/outputers/outputer.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:37.258948 syncany-0.2.5/syncany/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       52 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:37.716628 syncany-0.2.5/syncany/taskers/config/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1794 2023-03-25 04:34:57.000000 syncany-0.2.5/syncany/taskers/config/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      405 2022-08-23 12:07:09.000000 syncany-0.2.5/syncany/taskers/config/file_reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      937 2022-08-23 12:07:09.000000 syncany-0.2.5/syncany/taskers/config/http_reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      195 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/config/json_parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      208 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/config/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      204 2022-08-23 11:55:44.000000 syncany-0.2.5/syncany/taskers/config/reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5006 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/config/yaml_parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1377 2023-02-24 02:44:01.000000 syncany-0.2.5/syncany/taskers/context.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:38.185759 syncany-0.2.5/syncany/taskers/core/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    72944 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/taskers/core/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2192 2023-03-21 06:17:51.000000 syncany-0.2.5/syncany/taskers/core/loader_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      256 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/core/option.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2592 2023-02-10 08:39:32.000000 syncany-0.2.5/syncany/taskers/core/outputer_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4736 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/core/states.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15689 2023-02-25 11:47:43.000000 syncany-0.2.5/syncany/taskers/core/valuer_compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    40757 2023-03-24 06:10:54.000000 syncany-0.2.5/syncany/taskers/core/valuer_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      760 2023-02-25 12:43:51.000000 syncany-0.2.5/syncany/taskers/iterator.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      245 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/manager.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7122 2023-04-20 05:48:37.000000 syncany-0.2.5/syncany/taskers/tasker.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11025 2023-04-20 03:35:47.000000 syncany-0.2.5/syncany/utils.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:39.439949 syncany-0.2.5/syncany/valuers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2098 2023-03-25 04:34:57.000000 syncany-0.2.5/syncany/valuers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4574 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/aggregate.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3714 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/assign.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5209 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/cache.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3956 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/calculate.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6445 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/call.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5526 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/case.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4729 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/condition.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      548 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/const.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2965 2023-03-30 01:52:08.000000 syncany-0.2.5/syncany/valuers/data.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5059 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/db_join.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2043 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/db_load.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1877 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/function.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6018 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/generator.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3468 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/inherit.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3379 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/let.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12327 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/loop.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7510 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/make.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10283 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/match.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1247 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/schema.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4336 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/state.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6066 2023-03-30 01:52:08.000000 syncany-0.2.5/syncany/valuers/valuer.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:34.591915 syncany-0.2.5/syncany.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-20 08:44:32.000000 syncany-0.2.5/syncany.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2889 2023-04-20 08:44:33.000000 syncany-0.2.5/syncany.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-20 08:44:32.000000 syncany-0.2.5/syncany.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       47 2023-04-20 08:44:32.000000 syncany-0.2.5/syncany.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2022-08-15 03:43:33.000000 syncany-0.2.5/syncany.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      371 2023-04-20 08:44:32.000000 syncany-0.2.5/syncany.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        8 2023-04-20 08:44:32.000000 syncany-0.2.5/syncany.egg-info/top_level.txt
```

### Comparing `syncany-0.2.4/LICENSE` & `syncany-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/PKG-INFO` & `syncany-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncany
-Version: 0.2.4
+Version: 0.2.5
 Summary: 简单易用的数据同步转换导出框架
 Home-page: https://github.com/snower/syncany
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany
```

### Comparing `syncany-0.2.4/README.md` & `syncany-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/setup.py` & `syncany-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 18/8/6
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.2.4"
+version = "0.2.5"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
```

### Comparing `syncany-0.2.4/syncany/__init__.py` & `syncany-0.2.5/syncany/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
-version = "0.2.4"
-version_info = (0, 2, 4)
+version = "0.2.5"
+version_info = (0, 2, 5)
 
 from .loaders import Loader, register_loader
 from .outputers import Outputer, register_outputer
 from .valuers import Valuer, register_valuer
 from .filters import Filter, register_filter
 from .database import DataBase, register_database
 from .calculaters import Calculater, TypeFormatCalculater, TypingCalculater, MathematicalCalculater, \
```

### Comparing `syncany-0.2.4/syncany/calculaters/__init__.py` & `syncany-0.2.5/syncany/calculaters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/calculaters/builtin.py` & `syncany-0.2.5/syncany/calculaters/builtin.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/calculaters/calculater.py` & `syncany-0.2.5/syncany/calculaters/calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/calculaters/convert_calculater.py` & `syncany-0.2.5/syncany/calculaters/convert_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/calculaters/datetime_calculater.py` & `syncany-0.2.5/syncany/calculaters/datetime_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/calculaters/import_calculater.py` & `syncany-0.2.5/syncany/calculaters/import_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/calculaters/textline_calculater.py` & `syncany-0.2.5/syncany/calculaters/textline_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/calculaters/transform_calculater.py` & `syncany-0.2.5/syncany/calculaters/transform_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/__init__.py` & `syncany-0.2.5/syncany/database/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/beanstalk.py` & `syncany-0.2.5/syncany/database/beanstalk.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/clickhouse.py` & `syncany-0.2.5/syncany/database/clickhouse.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/csv.py` & `syncany-0.2.5/syncany/database/csv.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/database.py` & `syncany-0.2.5/syncany/database/database.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/elasticsearch.py` & `syncany-0.2.5/syncany/database/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/excel.py` & `syncany-0.2.5/syncany/database/excel.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/http.py` & `syncany-0.2.5/syncany/database/http.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/influxdb.py` & `syncany-0.2.5/syncany/database/influxdb.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/json.py` & `syncany-0.2.5/syncany/database/json.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/memory.py` & `syncany-0.2.5/syncany/database/memory.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/mongodb.py` & `syncany-0.2.5/syncany/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/mysql.py` & `syncany-0.2.5/syncany/database/mysql.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/postgresql.py` & `syncany-0.2.5/syncany/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/redis.py` & `syncany-0.2.5/syncany/database/redis.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/sqlite.py` & `syncany-0.2.5/syncany/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/sqlserver.py` & `syncany-0.2.5/syncany/database/sqlserver.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/database/textline.py` & `syncany-0.2.5/syncany/database/textline.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/errors.py` & `syncany-0.2.5/syncany/errors.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/filters/__init__.py` & `syncany-0.2.5/syncany/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/filters/builtin.py` & `syncany-0.2.5/syncany/filters/builtin.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/hook.py` & `syncany-0.2.5/syncany/hook.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/loaders/__init__.py` & `syncany-0.2.5/syncany/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/loaders/cache.py` & `syncany-0.2.5/syncany/loaders/cache.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/loaders/const.py` & `syncany-0.2.5/syncany/loaders/const.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/loaders/db.py` & `syncany-0.2.5/syncany/loaders/db.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/loaders/db_join.py` & `syncany-0.2.5/syncany/loaders/db_join.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/loaders/db_pull.py` & `syncany-0.2.5/syncany/loaders/db_pull.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/loaders/loader.py` & `syncany-0.2.5/syncany/loaders/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,17 +180,15 @@
                     self.datas.append(odata)
         self.geted = True
         return self.datas
 
     def check_intercepts(self, data):
         intercept_stoped = False
         for intercept in self.intercepts:
-            intercept = intercept.clone()
-            intercept.fill(data)
-            intercept_result = intercept.get()
+            intercept_result = intercept.reinit().fill(data).get()
             if intercept_result is not None and not intercept_result:
                 intercept_stoped = True
                 break
         return intercept_stoped
 
     def add_filter(self, key, exp, value):
         self.filters.append([key, exp, value])
```

### Comparing `syncany-0.2.4/syncany/main.py` & `syncany-0.2.5/syncany/main.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/outputers/__init__.py` & `syncany-0.2.5/syncany/outputers/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/outputers/db.py` & `syncany-0.2.5/syncany/outputers/db.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/outputers/db_delete_insert.py` & `syncany-0.2.5/syncany/outputers/db_delete_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/outputers/db_insert.py` & `syncany-0.2.5/syncany/outputers/db_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/outputers/db_update_delete_insert.py` & `syncany-0.2.5/syncany/outputers/db_update_delete_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/outputers/db_update_insert.py` & `syncany-0.2.5/syncany/outputers/db_update_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/outputers/outputer.py` & `syncany-0.2.5/syncany/outputers/outputer.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/taskers/config/__init__.py` & `syncany-0.2.5/syncany/taskers/config/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/taskers/config/http_reader.py` & `syncany-0.2.5/syncany/taskers/config/http_reader.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/taskers/config/yaml_parser.py` & `syncany-0.2.5/syncany/taskers/config/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/taskers/context.py` & `syncany-0.2.5/syncany/taskers/context.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/taskers/core/__init__.py` & `syncany-0.2.5/syncany/taskers/core/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/taskers/core/loader_creater.py` & `syncany-0.2.5/syncany/taskers/core/loader_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/taskers/core/outputer_creater.py` & `syncany-0.2.5/syncany/taskers/core/outputer_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/taskers/core/states.py` & `syncany-0.2.5/syncany/taskers/core/states.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/taskers/core/valuer_compiler.py` & `syncany-0.2.5/syncany/taskers/core/valuer_compiler.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/taskers/core/valuer_creater.py` & `syncany-0.2.5/syncany/taskers/core/valuer_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/taskers/iterator.py` & `syncany-0.2.5/syncany/taskers/iterator.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/taskers/tasker.py` & `syncany-0.2.5/syncany/taskers/tasker.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/utils.py` & `syncany-0.2.5/syncany/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,44 +105,63 @@
     except:
         return dt
     return dt
 
 def parse_datetime(value, fmt, tz):
     try:
         dt = pendulum_parse(value)
-        if isinstance(dt, datetime.datetime):
-            if tz != dt.tzinfo:
-                dt = dt.astimezone(tz=tz)
-            return dt
-        if isinstance(dt, datetime.date):
-            return datetime.datetime(dt.year, dt.month, dt.day, tzinfo=tz)
-        if isinstance(dt, datetime.time):
-            now = datetime.datetime.now()
-            return datetime.datetime(now.year, now.month, now.day, dt.hour, dt.minute, dt.second, dt.microsecond, tzinfo=tz)
     except ParserError:
-        pass
+        try:
+            if "." in value:
+                if len(value.split(".")[0]) == 6:
+                    dt = datetime.datetime.strptime(value, "%H%M%S.%f")
+                    now = datetime.datetime.now()
+                    return datetime.datetime(now.year, now.month, now.day, dt.hour, dt.minute, dt.second,
+                                             dt.microsecond, tzinfo=tz)
+                dt = datetime.datetime.strptime(value, "%Y%m%d%H%M%S.%f")
+            elif len(value) == 8:
+                dt = datetime.datetime.strptime(value, "%Y%m%d%H%M%S.%f")
+            elif len(value) == 6:
+                dt = datetime.datetime.strptime(value, "%H%M%S")
+                now = datetime.datetime.now()
+                return datetime.datetime(now.year, now.month, now.day, dt.hour, dt.minute, dt.second, dt.microsecond,
+                                         tzinfo=tz)
+            else:
+                dt = datetime.datetime.strptime(value, "%Y%m%d%H%M%S")
+        except:
+            return datetime.datetime.strptime(value, fmt or "%Y-%m-%d %H:%M:%S")
+
+    if isinstance(dt, datetime.datetime):
+        if tz != dt.tzinfo:
+            dt = dt.astimezone(tz=tz)
+        return dt
+    if isinstance(dt, datetime.date):
+        return datetime.datetime(dt.year, dt.month, dt.day, tzinfo=tz)
+    if isinstance(dt, datetime.time):
+        now = datetime.datetime.now()
+        return datetime.datetime(now.year, now.month, now.day, dt.hour, dt.minute, dt.second, dt.microsecond, tzinfo=tz)
     return datetime.datetime.strptime(value, fmt or "%Y-%m-%d %H:%M:%S")
 
 def parse_date(value, fmt, tz):
     try:
-        dt = pendulum_parse(value)
+        dt = parse_datetime(value, fmt, tz)
         if isinstance(dt, datetime.datetime):
             if tz != dt.tzinfo:
                 dt = dt.astimezone(tz=tz)
             return datetime.date(dt.year, dt.month, dt.day)
         if isinstance(dt, datetime.date):
             return dt
     except ParserError:
         pass
     dt = datetime.datetime.strptime(value, fmt or "%Y-%m-%d")
     return datetime.date(dt.year, dt.month, dt.day)
 
 def parse_time(value, fmt, tz):
     try:
-        dt = pendulum_parse(value)
+        dt = parse_datetime(value, fmt, tz)
         if isinstance(dt, datetime.datetime):
             if tz != dt.tzinfo:
                 dt = dt.astimezone(tz=tz)
             return datetime.time(dt.hour, dt.minute, dt.second, dt.microsecond)
         if isinstance(dt, datetime.time):
             return datetime.date.today()
     except ParserError:
```

### Comparing `syncany-0.2.4/syncany/valuers/__init__.py` & `syncany-0.2.5/syncany/valuers/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/aggregate.py` & `syncany-0.2.5/syncany/valuers/aggregate.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/assign.py` & `syncany-0.2.5/syncany/valuers/assign.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/cache.py` & `syncany-0.2.5/syncany/valuers/cache.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/calculate.py` & `syncany-0.2.5/syncany/valuers/calculate.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/call.py` & `syncany-0.2.5/syncany/valuers/call.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/case.py` & `syncany-0.2.5/syncany/valuers/case.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/condition.py` & `syncany-0.2.5/syncany/valuers/condition.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/const.py` & `syncany-0.2.5/syncany/valuers/const.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/data.py` & `syncany-0.2.5/syncany/valuers/data.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/db_join.py` & `syncany-0.2.5/syncany/valuers/db_join.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/db_load.py` & `syncany-0.2.5/syncany/valuers/db_load.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/function.py` & `syncany-0.2.5/syncany/valuers/function.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/generator.py` & `syncany-0.2.5/syncany/valuers/generator.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/inherit.py` & `syncany-0.2.5/syncany/valuers/inherit.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/let.py` & `syncany-0.2.5/syncany/valuers/let.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/loop.py` & `syncany-0.2.5/syncany/valuers/loop.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/make.py` & `syncany-0.2.5/syncany/valuers/make.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/match.py` & `syncany-0.2.5/syncany/valuers/match.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/schema.py` & `syncany-0.2.5/syncany/valuers/schema.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/state.py` & `syncany-0.2.5/syncany/valuers/state.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany/valuers/valuer.py` & `syncany-0.2.5/syncany/valuers/valuer.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.4/syncany.egg-info/PKG-INFO` & `syncany-0.2.5/syncany.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncany
-Version: 0.2.4
+Version: 0.2.5
 Summary: 简单易用的数据同步转换导出框架
 Home-page: https://github.com/snower/syncany
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany
```

### Comparing `syncany-0.2.4/syncany.egg-info/SOURCES.txt` & `syncany-0.2.5/syncany.egg-info/SOURCES.txt`

 * *Files identical despite different names*

