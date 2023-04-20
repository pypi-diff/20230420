# Comparing `tmp/renus-1.0.9.tar.gz` & `tmp/renus-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renus-1.0.9.tar", last modified: Sun Apr 16 07:16:42 2023, max compression
+gzip compressed data, was "renus-1.1.0.tar", last modified: Thu Apr 20 05:38:00 2023, max compression
```

## Comparing `renus-1.0.9.tar` & `renus-1.1.0.tar`

### file list

```diff
@@ -1,66 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.709578 renus-1.0.9/
--rw-rw-rw-   0        0        0     1514 2022-12-05 06:16:54.000000 renus-1.0.9/LICENSE
--rw-rw-rw-   0        0        0      220 2023-04-16 07:16:42.708579 renus-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.580325 renus-1.0.9/renus/
--rw-rw-rw-   0        0        0       23 2022-08-01 09:27:06.000000 renus-1.0.9/renus/__init__.py
--rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.0.9/renus/app.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.599473 renus-1.0.9/renus/commands/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.9/renus/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.602472 renus-1.0.9/renus/commands/app/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.9/renus/commands/app/__init__.py
--rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.0.9/renus/commands/app/run.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.605476 renus-1.0.9/renus/commands/backup/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.9/renus/commands/backup/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.0.9/renus/commands/backup/run.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.607456 renus-1.0.9/renus/commands/copy/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.9/renus/commands/copy/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.0.9/renus/commands/copy/run.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.610473 renus-1.0.9/renus/commands/default/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.9/renus/commands/default/__init__.py
--rw-rw-rw-   0        0        0     2272 2023-04-13 07:56:44.000000 renus-1.0.9/renus/commands/default/run.py
--rw-rw-rw-   0        0        0     1416 2023-04-15 07:24:18.000000 renus-1.0.9/renus/commands/help.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.618473 renus-1.0.9/renus/commands/install/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.9/renus/commands/install/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.0.9/renus/commands/install/build.py
--rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.0.9/renus/commands/install/run.py
--rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.0.9/renus/commands/install/service.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.620467 renus-1.0.9/renus/commands/permission/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.9/renus/commands/permission/__init__.py
--rw-rw-rw-   0        0        0      763 2023-03-14 08:51:15.000000 renus-1.0.9/renus/commands/permission/run.py
--rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.0.9/renus/commands/run.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.681403 renus-1.0.9/renus/core/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.9/renus/core/__init__.py
--rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.0.9/renus/core/cache.py
--rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.0.9/renus/core/concurrency.py
--rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.0.9/renus/core/config.py
--rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.0.9/renus/core/crypt.py
--rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.0.9/renus/core/datastructures.py
--rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.0.9/renus/core/exception.py
--rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.0.9/renus/core/formparsers.py
--rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.0.9/renus/core/injection.py
--rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.0.9/renus/core/log.py
--rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.0.9/renus/core/middleware.py
--rw-rw-rw-   0        0        0    14378 2023-04-16 06:58:20.000000 renus-1.0.9/renus/core/model.py
--rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.0.9/renus/core/request.py
--rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.0.9/renus/core/response.py
--rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.0.9/renus/core/routing.py
--rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.0.9/renus/core/schedule.py
--rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.0.9/renus/core/serialize.py
--rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.0.9/renus/core/status.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.699568 renus-1.0.9/renus/core/validation/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.9/renus/core/validation/__init__.py
--rw-rw-rw-   0        0        0     8773 2022-10-23 08:35:28.000000 renus-1.0.9/renus/core/validation/rules.py
--rw-rw-rw-   0        0        0     3235 2022-08-31 08:30:44.000000 renus-1.0.9/renus/core/validation/validate.py
--rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.0.9/renus/core/websockets.py
--rw-rw-rw-   0        0        0      301 2023-04-16 07:15:30.000000 renus-1.0.9/renus/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.707602 renus-1.0.9/renus/util/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.0.9/renus/util/__init__.py
--rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.0.9/renus/util/helper.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:16:42.594324 renus-1.0.9/renus.egg-info/
--rw-rw-rw-   0        0        0      220 2023-04-16 07:16:42.000000 renus-1.0.9/renus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2023-04-16 07:16:42.000000 renus-1.0.9/renus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 07:16:42.000000 renus-1.0.9/renus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-16 07:16:42.000000 renus-1.0.9/renus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 07:16:42.709578 renus-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      301 2023-04-16 07:15:30.000000 renus-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.844318 renus-1.1.0/
+-rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      220 2023-04-20 05:38:00.844318 renus-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.378322 renus-1.1.0/renus/
+-rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.0/renus/__init__.py
+-rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.0/renus/app.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.490378 renus-1.1.0/renus/commands/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.545339 renus-1.1.0/renus/commands/app/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/app/__init__.py
+-rw-rw-rw-   0        0        0     1787 2023-04-18 05:34:21.000000 renus-1.1.0/renus/commands/app/controller.temp
+-rw-rw-rw-   0        0        0      979 2023-04-18 05:34:20.000000 renus-1.1.0/renus/commands/app/model.temp
+-rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.0/renus/commands/app/route.temp
+-rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.1.0/renus/commands/app/run.py
+-rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.0/renus/commands/app/vue.temp
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.567322 renus-1.1.0/renus/commands/backup/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/backup/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.0/renus/commands/backup/run.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.585327 renus-1.1.0/renus/commands/copy/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/copy/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.0/renus/commands/copy/run.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.588322 renus-1.1.0/renus/commands/default/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/default/__init__.py
+-rw-rw-rw-   0        0        0     2153 2023-04-20 05:35:39.000000 renus-1.1.0/renus/commands/default/run.py
+-rw-rw-rw-   0        0        0     1416 2023-04-15 07:24:18.000000 renus-1.1.0/renus/commands/help.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.615321 renus-1.1.0/renus/commands/install/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/install/__init__.py
+-rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.1.0/renus/commands/install/build.py
+-rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.1.0/renus/commands/install/run.py
+-rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.0/renus/commands/install/service.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.617324 renus-1.1.0/renus/commands/permission/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/permission/__init__.py
+-rw-rw-rw-   0        0        0      704 2023-04-20 05:35:39.000000 renus-1.1.0/renus/commands/permission/run.py
+-rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.0/renus/commands/run.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.812322 renus-1.1.0/renus/core/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/__init__.py
+-rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.0/renus/core/cache.py
+-rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/concurrency.py
+-rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/config.py
+-rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.0/renus/core/crypt.py
+-rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/datastructures.py
+-rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.0/renus/core/exception.py
+-rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.0/renus/core/formparsers.py
+-rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.0/renus/core/injection.py
+-rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/log.py
+-rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/middleware.py
+-rw-rw-rw-   0        0        0    14287 2023-04-18 05:31:57.000000 renus-1.1.0/renus/core/model.py
+-rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.0/renus/core/request.py
+-rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.0/renus/core/response.py
+-rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.0/renus/core/routing.py
+-rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.0/renus/core/schedule.py
+-rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.1.0/renus/core/serialize.py
+-rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/status.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.832318 renus-1.1.0/renus/core/validation/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/validation/__init__.py
+-rw-rw-rw-   0        0        0     8773 2022-10-23 08:35:28.000000 renus-1.1.0/renus/core/validation/rules.py
+-rw-rw-rw-   0        0        0     3235 2022-08-31 08:30:44.000000 renus-1.1.0/renus/core/validation/validate.py
+-rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.0/renus/core/websockets.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.842318 renus-1.1.0/renus/util/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.0/renus/util/__init__.py
+-rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.0/renus/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:38:00.426356 renus-1.1.0/renus.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-04-20 05:38:00.000000 renus-1.1.0/renus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1405 2023-04-20 05:38:00.000000 renus-1.1.0/renus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 05:38:00.000000 renus-1.1.0/renus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 05:38:00.000000 renus-1.1.0/renus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 05:38:00.845319 renus-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-04-20 05:37:22.000000 renus-1.1.0/setup.py
```

### Comparing `renus-1.0.9/LICENSE` & `renus-1.1.0/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2021, smkoBa
+Copyright (c) 2022, https://github.com/smkoBa/renus
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `renus-1.0.9/renus/app.py` & `renus-1.1.0/renus/app.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/commands/app/run.py` & `renus-1.1.0/renus/commands/app/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/commands/backup/run.py` & `renus-1.1.0/renus/commands/backup/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/commands/copy/run.py` & `renus-1.1.0/renus/commands/copy/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/commands/default/run.py` & `renus-1.1.0/renus/commands/default/run.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 
 from renus.core.routing import Router
 from renus.util.helper import hash_new_password
 
 
 def run(args):
     if args[0] == 'setting':
-        from app.extension.renus.setting.model import Setting
+        from renus.app import Setting
         Setting('').where({'_id': {'$ne': 1}}).delete(True)
         with open('extension/renus/setting/db.json','r') as db:
             d=json.loads(db.read())
             for item in d:
                 Setting('').where({
                     'name':item['name']
                 }).update(item, True)
         print('DB Settings Created.')
 
     if args[0] == 'translate':
-        from app.extension.renus.translate.model import Translate
+        from renus.app import Translate
         Translate('').where({'_id':{'$ne':1}}).delete(True)
         with open('extension/renus/translate/db.json','r') as db:
             d=json.loads(db.read())
             for item in d:
                 Translate('').where({
                     'key':item['key']
                 }).update(item, True)
         print('DB Translates Created.')
 
     if args[0]=='super_admin':
-        from app.extension.renus.role.model import Role
-        from app.extension.renus.permission.model import Permission
-        from app.extension.renus.user.model import User
+        from renus.app import Role
+        from renus.app import Permission
+        from renus.app import User
         country_code = int(input('country_code: '))
         phone = int(input('phone: '))
         name = input('name: ')
         Permission('').where({
             'name': '*'
         }).update({}, True)
         permissions = Permission('').where({
```

### Comparing `renus-1.0.9/renus/commands/help.py` & `renus-1.1.0/renus/commands/help.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/commands/install/build.py` & `renus-1.1.0/renus/commands/install/build.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/commands/install/run.py` & `renus-1.1.0/renus/commands/install/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/commands/install/service.py` & `renus-1.1.0/renus/commands/install/service.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/cache.py` & `renus-1.1.0/renus/core/cache.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/concurrency.py` & `renus-1.1.0/renus/core/concurrency.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/crypt.py` & `renus-1.1.0/renus/core/crypt.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/datastructures.py` & `renus-1.1.0/renus/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/exception.py` & `renus-1.1.0/renus/core/exception.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/formparsers.py` & `renus-1.1.0/renus/core/formparsers.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/injection.py` & `renus-1.1.0/renus/core/injection.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/log.py` & `renus-1.1.0/renus/core/log.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/model.py` & `renus-1.1.0/renus/core/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import typing
 
 from bson import ObjectId
 from pymongo import MongoClient
 from datetime import datetime
 from renus.core.config import Config
-from renus.core.request import Request
 from renus.util.helper import dictAttribute
 
 class ModelBase:
     _client = MongoClient(Config('database').get('host', '127.0.0.1'),
                           Config('database').get('port', 27017),
                           username=Config('database').get('username', None),
                           password=Config('database').get('password', None))
@@ -17,16 +16,15 @@
     _database_name = Config('database').get('name', 'renus')
     _collection_name=None
     metro = None
     _public_folder='public'
     hidden_fields = []
     fields = {}
     _base_model=dictAttribute
-    def __init__(self, request: Request) -> None:
-        self._request = request
+    def __init__(self) -> None:
         self._steps = None
         self._where = None
         self._distinct = None
         self._limit = None
         self._skip = None
         self._sort = None
         self._select = None
```

### Comparing `renus-1.0.9/renus/core/request.py` & `renus-1.1.0/renus/core/request.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/response.py` & `renus-1.1.0/renus/core/response.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/routing.py` & `renus-1.1.0/renus/core/routing.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/schedule.py` & `renus-1.1.0/renus/core/schedule.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/serialize.py` & `renus-1.1.0/renus/core/serialize.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/status.py` & `renus-1.1.0/renus/core/status.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/validation/rules.py` & `renus-1.1.0/renus/core/validation/rules.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/validation/validate.py` & `renus-1.1.0/renus/core/validation/validate.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/core/websockets.py` & `renus-1.1.0/renus/core/websockets.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus/util/helper.py` & `renus-1.1.0/renus/util/helper.py`

 * *Files identical despite different names*

### Comparing `renus-1.0.9/renus.egg-info/SOURCES.txt` & `renus-1.1.0/renus.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 renus/__init__.py
 renus/app.py
-renus/setup.py
 renus.egg-info/PKG-INFO
 renus.egg-info/SOURCES.txt
 renus.egg-info/dependency_links.txt
 renus.egg-info/top_level.txt
 renus/commands/__init__.py
 renus/commands/help.py
 renus/commands/run.py
 renus/commands/app/__init__.py
+renus/commands/app/controller.temp
+renus/commands/app/model.temp
+renus/commands/app/route.temp
 renus/commands/app/run.py
+renus/commands/app/vue.temp
 renus/commands/backup/__init__.py
 renus/commands/backup/run.py
 renus/commands/copy/__init__.py
 renus/commands/copy/run.py
 renus/commands/default/__init__.py
 renus/commands/default/run.py
 renus/commands/install/__init__.py
```

