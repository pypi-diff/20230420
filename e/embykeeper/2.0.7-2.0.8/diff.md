# Comparing `tmp/embykeeper-2.0.7.tar.gz` & `tmp/embykeeper-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/embykeeper-2.0.7.tar", last modified: Mon Apr  3 02:40:16 2023, max compression
+gzip compressed data, was "embykeeper-2.0.8.tar", last modified: Thu Apr 20 10:52:59 2023, max compression
```

## Comparing `embykeeper-2.0.7.tar` & `embykeeper-2.0.8.tar`

### file list

```diff
@@ -1,54 +1,59 @@
-drwxrwxr-x   0 zzs       (1000) zzs       (1000)        0 2023-04-03 02:40:16.000000 embykeeper-2.0.7/
--rw-r--r--   0 zzs       (1000) zzs       (1000)       93 2023-03-27 09:11:27.000000 embykeeper-2.0.7/MANIFEST.in
--rw-rw-r--   0 zzs       (1000) zzs       (1000)    17680 2023-04-03 02:40:16.000000 embykeeper-2.0.7/PKG-INFO
--rw-rw-r--   0 zzs       (1000) zzs       (1000)    14390 2023-04-02 19:04:32.000000 embykeeper-2.0.7/README.md
-drwxrwxr-x   0 zzs       (1000) zzs       (1000)        0 2023-04-03 02:40:15.000000 embykeeper-2.0.7/embykeeper/
--rw-r--r--   0 zzs       (1000) zzs       (1000)      130 2023-04-03 02:25:27.000000 embykeeper-2.0.7/embykeeper/__init__.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)     6876 2023-04-03 02:24:37.000000 embykeeper-2.0.7/embykeeper/cli.py
-drwxrwxr-x   0 zzs       (1000) zzs       (1000)        0 2023-04-03 02:40:15.000000 embykeeper-2.0.7/embykeeper/embywatcher/
--rw-r--r--   0 zzs       (1000) zzs       (1000)        0 2023-03-27 09:11:23.000000 embykeeper-2.0.7/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)     3380 2023-04-03 02:24:37.000000 embykeeper-2.0.7/embykeeper/embywatcher/emby.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)     7177 2023-04-03 02:24:37.000000 embykeeper-2.0.7/embykeeper/embywatcher/main.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)     1166 2023-03-29 00:43:32.000000 embykeeper-2.0.7/embykeeper/log.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)     1925 2023-03-28 16:57:39.000000 embykeeper-2.0.7/embykeeper/loop.py
--rw-rw-r--   0 zzs       (1000) zzs       (1000)     6450 2023-03-29 11:37:19.000000 embykeeper-2.0.7/embykeeper/settings.py
-drwxrwxr-x   0 zzs       (1000) zzs       (1000)        0 2023-04-03 02:40:15.000000 embykeeper-2.0.7/embykeeper/telechecker/
--rw-r--r--   0 zzs       (1000) zzs       (1000)        0 2023-03-27 09:11:26.000000 embykeeper-2.0.7/embykeeper/telechecker/__init__.py
-drwxrwxr-x   0 zzs       (1000) zzs       (1000)        0 2023-04-03 02:40:16.000000 embykeeper-2.0.7/embykeeper/telechecker/bots/
--rw-r--r--   0 zzs       (1000) zzs       (1000)        0 2023-03-27 09:11:24.000000 embykeeper-2.0.7/embykeeper/telechecker/bots/__init__.py
--rw-rw-r--   0 zzs       (1000) zzs       (1000)    13508 2023-04-03 02:24:37.000000 embykeeper-2.0.7/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)      297 2023-03-30 07:14:49.000000 embykeeper-2.0.7/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)      146 2023-03-27 09:11:24.000000 embykeeper-2.0.7/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)      650 2023-03-27 09:11:24.000000 embykeeper-2.0.7/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)      340 2023-03-27 09:11:24.000000 embykeeper-2.0.7/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)      469 2023-04-03 02:24:37.000000 embykeeper-2.0.7/embykeeper/telechecker/bots/ljyy.py
--rw-rw-r--   0 zzs       (1000) zzs       (1000)     3325 2023-03-29 15:20:25.000000 embykeeper-2.0.7/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)      669 2023-03-27 09:11:24.000000 embykeeper-2.0.7/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)      687 2023-03-27 09:11:24.000000 embykeeper-2.0.7/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)      288 2023-03-27 09:11:24.000000 embykeeper-2.0.7/embykeeper/telechecker/bots/terminus.py
--rw-rw-r--   0 zzs       (1000) zzs       (1000)     4643 2023-03-30 07:05:53.000000 embykeeper-2.0.7/embykeeper/telechecker/link.py
--rw-rw-r--   0 zzs       (1000) zzs       (1000)    13622 2023-03-29 15:20:25.000000 embykeeper-2.0.7/embykeeper/telechecker/main.py
-drwxrwxr-x   0 zzs       (1000) zzs       (1000)        0 2023-04-03 02:40:16.000000 embykeeper-2.0.7/embykeeper/telechecker/messager/
--rw-r--r--   0 zzs       (1000) zzs       (1000)        0 2023-03-27 09:11:25.000000 embykeeper-2.0.7/embykeeper/telechecker/messager/__init__.py
--rw-rw-r--   0 zzs       (1000) zzs       (1000)     4632 2023-04-03 02:37:58.000000 embykeeper-2.0.7/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)     3133 2023-04-03 02:24:29.000000 embykeeper-2.0.7/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)      191 2023-04-02 15:14:55.000000 embykeeper-2.0.7/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)      302 2023-03-27 09:11:25.000000 embykeeper-2.0.7/embykeeper/telechecker/messager/test.py
-drwxrwxr-x   0 zzs       (1000) zzs       (1000)        0 2023-04-03 02:40:16.000000 embykeeper-2.0.7/embykeeper/telechecker/monitor/
--rw-r--r--   0 zzs       (1000) zzs       (1000)        0 2023-03-27 09:11:26.000000 embykeeper-2.0.7/embykeeper/telechecker/monitor/__init__.py
--rw-rw-r--   0 zzs       (1000) zzs       (1000)     8189 2023-04-03 02:24:37.000000 embykeeper-2.0.7/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)      530 2023-03-27 09:11:25.000000 embykeeper-2.0.7/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)     1019 2023-03-27 09:11:25.000000 embykeeper-2.0.7/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)      617 2023-03-27 09:11:25.000000 embykeeper-2.0.7/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)    10996 2023-04-03 02:24:37.000000 embykeeper-2.0.7/embykeeper/telechecker/tele.py
--rw-r--r--   0 zzs       (1000) zzs       (1000)     4424 2023-04-03 02:24:37.000000 embykeeper-2.0.7/embykeeper/utils.py
-drwxrwxr-x   0 zzs       (1000) zzs       (1000)        0 2023-04-03 02:40:15.000000 embykeeper-2.0.7/embykeeper.egg-info/
--rw-rw-r--   0 zzs       (1000) zzs       (1000)    17680 2023-04-03 02:40:15.000000 embykeeper-2.0.7/embykeeper.egg-info/PKG-INFO
--rw-rw-r--   0 zzs       (1000) zzs       (1000)     1459 2023-04-03 02:40:15.000000 embykeeper-2.0.7/embykeeper.egg-info/SOURCES.txt
--rw-rw-r--   0 zzs       (1000) zzs       (1000)        1 2023-04-03 02:40:15.000000 embykeeper-2.0.7/embykeeper.egg-info/dependency_links.txt
--rw-rw-r--   0 zzs       (1000) zzs       (1000)       51 2023-04-03 02:40:15.000000 embykeeper-2.0.7/embykeeper.egg-info/entry_points.txt
--rw-rw-r--   0 zzs       (1000) zzs       (1000)        1 2023-03-29 11:38:19.000000 embykeeper-2.0.7/embykeeper.egg-info/not-zip-safe
--rw-rw-r--   0 zzs       (1000) zzs       (1000)      188 2023-04-03 02:40:15.000000 embykeeper-2.0.7/embykeeper.egg-info/requires.txt
--rw-rw-r--   0 zzs       (1000) zzs       (1000)       11 2023-04-03 02:40:15.000000 embykeeper-2.0.7/embykeeper.egg-info/top_level.txt
--rw-r--r--   0 zzs       (1000) zzs       (1000)      399 2023-04-03 02:40:16.000000 embykeeper-2.0.7/setup.cfg
--rw-r--r--   0 zzs       (1000) zzs       (1000)     1266 2023-04-03 02:25:27.000000 embykeeper-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.446127 embykeeper-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 10:52:40.000000 embykeeper-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 10:52:40.000000 embykeeper-2.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-04-20 10:52:59.446127 embykeeper-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-04-20 10:52:40.000000 embykeeper-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.442127 embykeeper-2.0.8/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.442127 embykeeper-2.0.8/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.442127 embykeeper-2.0.8/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.446127 embykeeper-2.0.8/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/sosdbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.446127 embykeeper-2.0.8/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.446127 embykeeper-2.0.8/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/monitor/pornemby_exam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-20 10:52:40.000000 embykeeper-2.0.8/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:52:59.442127 embykeeper-2.0.8/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 10:52:59.000000 embykeeper-2.0.8/embykeeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 10:52:40.000000 embykeeper-2.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-20 10:52:59.446127 embykeeper-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-20 10:52:40.000000 embykeeper-2.0.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `embykeeper-2.0.7/PKG-INFO` & `embykeeper-2.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,329 +1,401 @@
-Metadata-Version: 2.1
-Name: embykeeper
-Version: 2.0.7
-Summary: Daily checkin automator for emby bots in telegram.
-Home-page: https://github.com/embykeeper/embykeeper
-Author: jackzzs
-Author-email: jackzzs@outlook.com
-License: UNKNOWN
-Description: [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
-        
-        <p align="center">
-          <a href='https://github.com/embykeeper/embykeeper'>
-            <img src="https://github.com/embykeeper/embykeeper/blob/main/images/logo.svg" alt="Embykeeper" />
-          </a>
-        </p>
-        <p align="center">
-            <b>自动签到 定时保号 按需水群</b>
-        </p>
-        
-        ---
-        
-        Embykeeper 是一个在中文社群规则下用于 Emby 影视服务器的签到和保号的自动执行工具, 基于 Pyrogram 编写并具有可拓展性。
-        
-        ## 声明
-        
-        本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关，在使用 Embykeeper 时造成的一切损失（包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁）与开发团队无关。
-        
-        本项目设计初衷是在中文 Emby 社群规则下，保号要求逐渐苛刻（部分要求每月登录或每日签到），这使得休闲时间紧张的人士难以安心使用。本项目仅旨在帮助该类人群保号，不鼓励持有大量 Emby 账号而不使用，导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为，开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器。本项目仅提供工具，具体使用形式及造成的影响和后果与开发团队无关。
-        
-        本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以删除或关闭与项目开发不直接相关的不友善讨论。
-        
-        当您使用 "消息提示" 功能，该工具时候将自动向 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 发送关键的成功/失败日志以供向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题。
-        
-        当您安装并使用该工具，默认您已经阅读并同意上述声明，并确认自己并非出于"集邮"目的而安装。
-        
-        ## 功能
-        
-        - Telegram 机器人签到
-          - 支持群组
-            - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
-            - 卷毛鼠: [频道]() [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
-            - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
-            - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
-            - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
-            - BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)
-            - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
-            - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
-            - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
-          - 高级特性
-            - 验证码识别与自动重试
-            - 多账户签到
-            - 网页类型签到
-        - Emby 保活
-          - 定时模拟账号登录视频播放
-          - 播放时间与进度模拟
-        - Telegram 自动水群 (默认使用内建话术列表, 请谨慎使用)
-          - NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)
-        - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
-          - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
-          - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
-        
-        ## 安装与使用
-        
-        Embykeeper 需要 Python 环境以运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
-        
-        您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7`):
-        
-        ```bash
-        pip install embykeeper
-        ```
-        
-        或者您也可以通过源码构建:
-        
-        ```bash
-        git clone https://github.com/embykeeper/embykeeper.git
-        cd embykeeper
-        make develop
-        ```
-        
-        随后，您需要执行:
-        
-        ```bash
-        embykeeper
-        ```
-        
-        命令将会在当前目录生成模板 `config.toml` 文件，您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
-        
-        ```toml
-        [proxy]
-        hostname = "127.0.0.1"
-        port = "1080"
-        scheme = "socks5"
-        
-        [[telegram]]
-        api_id = "27894236"
-        api_hash = "622159182fdd4b15b627eeb3ac695271"
-        phone = "+8612109347899"
-        
-        [[emby]]
-        url = "https://weiss-griffin.com/"
-        username = "carrie19"
-        password = "s*D7MMCpS$"
-        ```
-        
-        对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 API development tools, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要更换应用名称/短名称/代理/清除浏览器记录并重试.
-        
-        然后, 运行:
-        
-        ```bash
-        embykeeper config.toml
-        ```
-        
-        您将被询问设备验证码以登录，登录成功后，Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
-        
-        恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以运行:
-        
-        ```bash
-        tmux
-        ```
-        
-        这将启动一个 `tmux` 终端，您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端。
-        
-        您随时可以通过运行:
-        
-        ```bash
-        tmux a
-        ```
-        
-        以重新连接到 `tmux` 终端.
-        
-        ## 命令行帮助
-        
-        您可以通过运行 `embykeeper -h` 以获取帮助:
-        
-        ```bash
-        $ embykeeper -h
-        
-        欢迎使用 Embykeeper. 🎦 无参数默认开启全部功能.
-        
-        参数:
-            config  配置文件 (置空以生成)
-        模块开关:
-            --checkin     -c   启用每日指定时间签到 (不指定值时默认为6:00PM)
-            --emby        -e   启用每隔天数Emby自动保活 (不指定值时默认为每7天)
-            --monitor     -m   启用群聊监视
-            --send        -s   启用自动水群
-        调试参数:
-            --no-instant  -I   不立刻执行一次计划任务
-            --debug       -d   开启调试模式, 错误将会导致程序停止运行
-            --version     -v   打印 Embykeeper 版本
-            --follow      -f   仅启动消息调试
-            --analyze     -a   仅启动历史信息分析
-        ```
-        
-        例如:
-        
-        ```bash
-        # 仅启动每日签到
-        $ embykeeper config.toml -c
-        
-        # 仅启动每日 8:00 PM 签到
-        $ embykeeper config.toml -c 8:00PM
-        
-        # 启动所有功能, 同时调整签到时间为 8:00 AM, 调整保活间隔天数为 14
-        $ embykeeper config.toml -c 8:00PM -e 14 -m -s
-        ```
-        
-        您也可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
-        
-        ```bash
-        # 启动历史信息分析
-        $ embykeeper config.toml -a
-        
-        请输入群组用户名 (以空格分隔): https://t.me/XXX YYY 10253512
-        请输入关键词 (以空格分隔):
-        输入时间范围 (以"-"分割): 8:00AM-10:00AM
-        请输入各群组最大获取数量 [1000]:
-        ```
-        
-        该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
-        
-        另一个工具是即时信息分析:
-        
-        ![follow screenshot](images/follow.svg)
-        
-        该工具可以实时输出消息的 ID 等信息, 以方便调试.
-        
-        ## 消息推送与高级用户
-        
-        您可以通过设置项 "`notifier`" 设置 成功/失败 通知将被发送的 Telegram 账号, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot) 设置消息每日发送的时间.
-        
-        本项目涉及的需要 Cloudflare 验证码付费跳过的操作（例如 Nebula 签到）、可能会引起竞争的操作（例如自动抢邀请码）将需要高级用户，您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) 成为高级用户.
-        
-        目前有三种方式成为高级用户:
-        
-        1. 分享 1 个邀请制 Emby 的邀请码;
-        2. 为本项目提供 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 并被合并;
-        3. 通过爱发电赞助一个[小包子](https://afdian.net/a/jackzzs);
-        
-        ## 支持 Embykeeper
-        
-        ##### 开发者团队
-        
-        - [jackzzs](https://github.com/jackzzs)
-        
-        ##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
-        
-        ![kitty](images/kitty.gif)
-        
-        ## 配置项
-        
-        | 设置项       | 值类型             | 简介                                         | 默认值  |
-        | ------------ | ------------------ | -------------------------------------------- | ------- |
-        | `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
-        | `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `10`    |
-        | `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
-        | `random`     | `int`              | Telegram 机器人签到定时任务时间随机量 (分钟) | `15`    |
-        | `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
-        | `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
-        | `proxy`      | `dict`             | 代理设置                                     | `{}`    |
-        | `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
-        | `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
-        
-        `service`设置可以为:
-        
-        | 设置项      | 值类型 | 简介           | 默认值               |
-        | ----------- | ------ | -------------- | -------------------- |
-        | `checkiner` | `list` | 启用的签到站点 | (当前所有支持的站点) |
-        | `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
-        | `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
-        
-        注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
-        
-        `proxy` 设置可以为:
-        
-        | 设置项     | 值类型 | 简介                                    | 默认值      |
-        | ---------- | ------ | --------------------------------------- | ----------- |
-        | `hostname` | `str`  | 代理服务器地址                          | `localhost` |
-        | `port`     | `int`  | 代理端口号                              | `1080`      |
-        | `scheme`   | `str`  | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
-        
-        `telegram` 设置可以为:
-        
-        | 设置项     | 值类型 | 简介                                                               | 默认值  |
-        | ---------- | ------ | ------------------------------------------------------------------ | ------- |
-        | `api_id`   | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
-        | `api_hash` | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
-        | `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                      |         |
-        | `monitor`  | `bool` | 启用群组监控系列功能                                               | `false` |
-        | `send`     | `bool` | 启用自动水群系列功能                                               | `false` |
-        
-        `emby` 设置可以为:
-        
-        | 设置项     | 值类型 | 简介                                                      | 默认值 |
-        | ---------- | ------ | --------------------------------------------------------- | ------ |
-        | `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
-        | `username` | `str`  | Emby 服务器用户名                                         |        |
-        | `password` | `str`  | Emby 服务器密码                                           |        |
-        | `time`     | `int`  | 模拟观看的时间 (秒)                                       | `800`  |
-        | `progress` | `int`  | 观看后模拟进度条保存的时间 (秒)                           | `1000` |
-        
-        ## 代码重用与开发
-        
-        代码架构如下:
-        
-        ```mermaid
-        flowchart TD
-            A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
-            A --> C(fa:fa-play embywatcher)
-            B --checker--> E[fa:fa-robot Bot]
-            B --monitor--> G[fa:fa-eye Monitor]
-            B --messager--> F[fa:fa-message Messager]
-            C --watcher--> H[fa:fa-circle-play EmbyWatcher]
-            F ---- |schedule| A
-        ```
-        
-        主要可以扩展的类位于:
-        
-        - `embykeeper.telechecker.bots`
-        - `embykeeper.telechecker.monitor`
-        - `embykeeper.telechecker.messager`
-        
-        通常来说, 增加一个机器人的签到非常简单, 您需要在 `bots` 中增加一个文件 `dummy.py`:
-        
-        ```python
-        from .base import BotCheckin
-        
-        class DummyCheckin(BotCheckin):
-            name = "Dummy"
-            bot_username = "dummy"
-            bot_captcha_len = 4
-        ```
-        
-        您即增加一个名为 "`Dummy`" 的签到器，将会向用户名为 "`dummy`" 的机器人发送 "`/checkin`" 并等候一个 4 位的验证码，识别验证码后将发送.
-        
-        若您希望识别验证码后点击按钮, 您可以使用 `AnswerBotCheckin`, 您也可以重写 `on_captcha` 函数来实现自定义功能:
-        
-        ```python
-        from .base import AnswerBotCheckin
-        
-        class DummyCheckin(AnswerBotCheckin):
-            ....
-            async def on_captcha(self, message: Message, captcha: str):
-                for l in captcha:
-                    try:
-                        await self.message.click(l)
-                    except ValueError:
-                        self.log.info(f'未能找到对应 "{l}" 的按键, 正在重试.')
-                        await self.retry()
-                        break
-        ```
-        
-        上述代码实现每次按对应一个字符按键的功能.
-        
-        当您实现一个新的签到器时, 欢迎您提出 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 以帮助更多人使用!
-        
-Keywords: emby,telegram,checkin,automator
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7,<3.11
-Description-Content-Type: text/markdown
+[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
+
+<p align="center">
+  <a href='https://github.com/embykeeper/embykeeper'>
+    <img src="https://github.com/embykeeper/embykeeper/blob/main/images/logo.svg" alt="Embykeeper" />
+  </a>
+</p>
+<p align="center">
+    <b>自动签到 定时保号 按需水群</b>
+</p>
+
+---
+
+Embykeeper 是一个在中文社群规则下用于 Emby 影视服务器的签到和保号的自动执行工具, 基于 Pyrogram 编写并具有可拓展性.
+
+## 声明
+
+本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关. 
+
+本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关. 
+
+本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Telegram 讨论组](https://t.me/embykeeper_chat) 与开发团队进行交流.
+
+当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题. 
+
+当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装. 
+
+## 功能
+
+- Telegram 机器人签到
+  - 支持群组
+    - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
+    - 卷毛鼠: [频道]() [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
+    - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
+    - BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)
+    - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
+    - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
+    - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
+    - Pornemby (_测试中_): [频道](https://t.me/pornembyservice) [机器人](https://t.me/PronembyTGBot2_bot)
+    - 其他非 Emby 相关:
+      - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加) (_测试中_)
+    - 默认禁用:
+      - Pornemby 科举考试 (_测试中_): [活动频道](https://t.me/PornembyFun)
+      - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
+      - ~~垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)~~ (无响应)
+  - 特性
+    - 验证码识别与自动重试
+    - 多账户签到
+    - 网页类型签到
+- Emby 保活
+  - 定时模拟账号登录视频播放
+  - 播放时间与进度模拟
+- Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
+  - NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)
+- Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
+  - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
+  - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
+
+## 安装与使用
+
+### 从 Docker 安装
+
+Embykeeper 可以通过 `docker` 运行, 您需[安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
+
+```bash
+touch config.toml
+docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
+```
+
+命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+
+```toml
+[proxy]
+hostname = "127.0.0.1"
+port = "1080"
+scheme = "socks5"
+
+[[telegram]]
+api_id = "27894236"
+api_hash = "622159182fdd4b15b627eeb3ac695271"
+phone = "+8612109347899"
+
+[[emby]]
+url = "https://weiss-griffin.com/"
+username = "carrie19"
+password = "s*D7MMCpS$"
+```
+
+对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要更换应用名称/短名称/代理/清除浏览器记录并重试.
+
+随后, 您需要再次执行:
+
+```bash
+docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
+```
+
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+
+```bash
+docker run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper
+```
+
+或者使用 [docker-compose](https://docs.docker.com/compose/) ([watchtower](https://github.com/containrrr/watchtower) 被用于自动更新容器服务):
+
+```yaml
+version: '3'
+services:
+  embykeeper:
+    container_name: embykeeper
+    image: cembykeeper/embykeeper
+    restart: unless-stopped
+    volumes:
+      - ./config.toml:/app/config.toml
+  watchtower:
+    container_name: watchtower
+    image: containrrr/watchtower
+    restart: unless-stopped
+    volumes:
+      - /var/run/docker.sock:/var/run/docker.sock:rw
+```
+
+即可在后台启动 embykeeper.
+
+您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
+
+如果您需要使用主机上的代理服务器 (例如 `https://localhost:1080`), 您可能需要使用 `--net=host` 参数以使用主机网络模式.
+
+### 从 Pypi 安装
+
+Embykeeper 需要 Python 环境以运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
+
+您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7, < 3.11`):
+
+```bash
+pip install embykeeper
+```
+
+随后, 您需要执行:
+
+```bash
+embykeeper
+```
+
+命令将会在当前目录生成模板 `config.toml` 文件, 您需要修改您的账号配置 (详见[从 Docker 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E%20Docker%20%E5%AE%89%E8%A3%85)).
+
+随后, 您需要再次执行:
+
+```bash
+embykeeper
+```
+
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+
+```bash
+tmux
+```
+
+这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端. 
+
+您随时可以通过运行:
+
+```bash
+tmux a
+```
+
+以重新连接到 `tmux` 终端.
+
+当版本更新时, 您需要执行:
+
+```
+pip install -U embykeeper
+```
+
+然后重新运行应用.
+
+### 从源码构建
+
+首先拉取 Github 并安装:
+
+```bash
+git clone https://github.com/embykeeper/embykeeper.git
+cd embykeeper
+make develop
+```
+
+然后即可执行 Embykeeper:
+
+```bash
+embykeeper
+```
+
+详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E%20Pypi%20%E5%AE%89%E8%A3%85).
+
+当版本更新时, 您需要执行:
+
+```
+git pull
+```
+
+然后重新运行应用.
+
+## 命令行帮助
+
+您可以通过运行 `embykeeper -h` 以获取帮助:
+
+```bash
+$ embykeeper -h
+
+欢迎使用 Embykeeper. 🎦 无参数默认开启全部功能.
+
+参数:
+    config  配置文件 (置空以生成)
+模块开关:
+    --checkin     -c   启用每日指定时间签到 (不指定值时默认为6:00PM)
+    --emby        -e   启用每隔天数Emby自动保活 (不指定值时默认为每7天)
+    --monitor     -m   启用群聊监视
+    --send        -s   启用自动水群
+调试参数:
+    --no-instant  -I   不立刻执行一次计划任务
+    --debug       -d   开启调试模式, 错误将会导致程序停止运行
+    --version     -v   打印 Embykeeper 版本
+    --follow      -f   仅启动消息调试
+    --analyze     -a   仅启动历史信息分析
+```
+
+例如:
+
+```bash
+# 仅启动每日签到
+$ embykeeper config.toml -c
+
+# 仅启动每日 8:00 PM 签到
+$ embykeeper config.toml -c 8:00PM
+
+# 启动所有功能, 同时调整签到时间为 8:00 AM, 调整保活间隔天数为 14
+$ embykeeper config.toml -c 8:00PM -e 14 -m -s
+```
+
+您也可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
+
+```bash
+# 启动历史信息分析
+$ embykeeper config.toml -a
+
+请输入群组用户名 (以空格分隔): https://t.me/XXX YYY 10253512
+请输入关键词 (以空格分隔):
+输入时间范围 (以"-"分割): 8:00AM-10:00AM
+请输入各群组最大获取数量 [1000]:
+```
+
+该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
+
+另一个工具是即时信息分析:
+
+![follow screenshot](images/follow.svg)
+
+该工具可以实时输出消息的 ID 等信息, 以方便调试.
+
+## 消息推送与高级用户
+
+您可以通过设置项 "`notifier`" 设置 成功/失败 通知将被发送的 Telegram 账号, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot) 设置消息每日发送的时间.
+
+本项目涉及的需要 Cloudflare 验证码付费跳过的操作 (例如 Nebula 签到)、可能会引起竞争的操作 (例如自动抢邀请码)将需要高级用户, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) 成为高级用户.
+
+目前有三种方式成为高级用户:
+
+1. 分享 1 个邀请制 Emby 的邀请码;
+2. 为本项目提供 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 并被合并;
+3. 通过爱发电赞助一个[小包子](https://afdian.net/a/jackzzs);
+
+## 支持 Embykeeper
+
+##### 开发者团队
+
+- [jackzzs](https://github.com/jackzzs)
+
+##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
+
+![kitty](images/kitty.gif)
+
+## 配置项
+
+| 设置项       | 值类型             | 简介                                         | 默认值  |
+| ------------ | ------------------ | -------------------------------------------- | ------- |
+| `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
+| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `10`    |
+| `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
+| `random`     | `int`              | Telegram 机器人签到定时任务时间随机量 (分钟) | `15`    |
+| `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
+| `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
+| `proxy`      | `dict`             | 代理设置                                     | `{}`    |
+| `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
+| `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
+
+`service`设置可以为:
+
+| 设置项      | 值类型 | 简介           | 默认值               |
+| ----------- | ------ | -------------- | -------------------- |
+| `checkiner` | `list` | 启用的签到站点 | (当前所有支持的站点) |
+| `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
+| `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
+
+注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
+若您需要禁用部分签到站点, 您可以在列表中删除对应的名称.
+若您需要使用默认禁用的签到站点, 您可以在列表中增加对应的名称.
+当前支持的名称包括:
+| 站点 | 名称 | | 站点 | 名称 |
+| --- | --- | --- |--- | --- |
+| 垃圾影音 | `ljyy` | | 搜书神器 | `sosdbot` |
+| 卷毛鼠 IPTV | `jms_iptv` | | 终点站 | `terminus` |
+| Pornemby | `pornemby` | | Singularity | `singularity` |
+| Peach | `peach` | | Nebula | `nebula` |
+| Bluesea | `bluesea` | | Embyhub | `embyhub` |
+| 卷毛鼠 | `jms` | | | |
+
+`proxy` 设置可以为:
+
+| 设置项     | 值类型 | 简介                                    | 默认值      |
+| ---------- | ------ | --------------------------------------- | ----------- |
+| `hostname` | `str`  | 代理服务器地址                          | `localhost` |
+| `port`     | `int`  | 代理端口号                              | `1080`      |
+| `scheme`   | `str`  | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
+
+`telegram` 设置可以为:
+
+| 设置项     | 值类型 | 简介                                                               | 默认值  |
+| ---------- | ------ | ------------------------------------------------------------------ | ------- |
+| `api_id`   | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
+| `api_hash` | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
+| `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                      |         |
+| `monitor`  | `bool` | 启用群组监控系列功能                                               | `false` |
+| `send`     | `bool` | 启用自动水群系列功能                                               | `false` |
+
+`emby` 设置可以为:
+
+| 设置项     | 值类型 | 简介                                                      | 默认值 |
+| ---------- | ------ | --------------------------------------------------------- | ------ |
+| `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
+| `username` | `str`  | Emby 服务器用户名                                         |        |
+| `password` | `str`  | Emby 服务器密码                                           |        |
+| `time`     | `int`  | 模拟观看的时间 (秒)                                       | `800`  |
+| `progress` | `int`  | 观看后模拟进度条保存的时间 (秒)                           | `1000` |
+
+## 代码重用与开发
+
+代码架构如下:
+
+```mermaid
+flowchart TD
+    A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
+    A --> C(fa:fa-play embywatcher)
+    B --checker--> E[fa:fa-robot Bot]
+    B --monitor--> G[fa:fa-eye Monitor]
+    B --messager--> F[fa:fa-message Messager]
+    C --watcher--> H[fa:fa-circle-play EmbyWatcher]
+    F ---- |schedule| A
+```
+
+主要可以扩展的类位于:
+
+- `embykeeper.telechecker.bots`
+- `embykeeper.telechecker.monitor`
+- `embykeeper.telechecker.messager`
+
+通常来说, 增加一个机器人的签到非常简单, 您需要在 `bots` 中增加一个文件 `dummy.py`:
+
+```python
+from .base import BotCheckin
+
+class DummyCheckin(BotCheckin):
+    name = "Dummy"
+    bot_username = "dummy"
+    bot_captcha_len = 4
+```
+
+您即增加一个名为 "`Dummy`" 的签到器, 将会向用户名为 "`dummy`" 的机器人发送 "`/checkin`" 并等候一个 4 位的验证码, 识别验证码后将发送.
+
+若您希望识别验证码后点击按钮, 您可以使用 `AnswerBotCheckin`, 您也可以重写 `on_captcha` 函数来实现自定义功能:
+
+```python
+from .base import AnswerBotCheckin
+
+class DummyCheckin(AnswerBotCheckin):
+    ....
+    async def on_captcha(self, message: Message, captcha: str):
+        for l in captcha:
+            try:
+                await self.message.click(l)
+            except ValueError:
+                self.log.info(f'未能找到对应 "{l}" 的按键, 正在重试.')
+                await self.retry()
+                break
+```
+
+上述代码实现每次按对应一个字符按键的功能.
+
+当您实现一个新的签到器时, 欢迎您提出 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 以帮助更多人使用!
```

#### html2text {}

```diff
@@ -1,103 +1,140 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.0.7 Summary: Daily checkin
-automator for emby bots in telegram. Home-page: https://github.com/embykeeper/
-embykeeper Author: jackzzs Author-email: jackzzs@outlook.com License: UNKNOWN
-Description: [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://
-pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/
-dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
+[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/
+project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/
+embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
 pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/
 pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license
 badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://
 github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://
 img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [!
 [telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://
 t.me/embykeeper)
                                  [Embykeeper]
                     èªå¨ç­¾å° å®æ¶ä¿å· æéæ°´ç¾¤
 --- Embykeeper æ¯ä¸ä¸ªå¨ä¸­æç¤¾ç¾¤è§åä¸ç¨äº Emby
 å½±è§æå¡å¨çç­¾å°åä¿å·çèªå¨æ§è¡å·¥å·, åºäº Pyrogram
-ç¼åå¹¶å·æå¯æå±æ§ã ## å£°æ æ¬é¡¹ç®æ¶åçä¸å Emby
-æå¡å¨ä¸ Embykeeper å¼åå¢éæ å³ï¼å¨ä½¿ç¨ Embykeeper
-æ¶é æçä¸åæå¤±ï¼åæ¬ä½ä¸éäº Emby æ Telegram
-è´¦å·è¢«å°ç¦æè¢«ç¾¤å°ç¦ï¼ä¸å¼åå¢éæ å³ã
-æ¬é¡¹ç®è®¾è®¡åè¡·æ¯å¨ä¸­æ Emby
-ç¤¾ç¾¤è§åä¸ï¼ä¿å·è¦æ±éæ¸èå»ï¼é¨åè¦æ±æ¯æç»å½ææ¯æ¥ç­¾å°ï¼ï¼è¿ä½¿å¾ä¼é²æ¶é´ç´§å¼ çäººå£«é¾ä»¥å®å¿ä½¿ç¨ãæ¬é¡¹ç®ä»æ¨å¨å¸®å©è¯¥ç±»äººç¾¤ä¿å·ï¼ä¸é¼å±ææå¤§é
-Emby
-è´¦å·èä¸ä½¿ç¨ï¼å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸ºï¼å¼åå¢éä¹å¼åä»ä¿ç
-1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby
-æå¡å¨ãæ¬é¡¹ç®ä»æä¾å·¥å·ï¼å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³ã
+ç¼åå¹¶å·æå¯æå±æ§. ## å£°æ æ¬é¡¹ç®æ¶åçä¸å Emby
+æå¡å¨ä¸ Embykeeper å¼åå¢éæ å³, å¨ä½¿ç¨ Embykeeper
+æ¶é æçä¸åæå¤± (åæ¬ä½ä¸éäº Emby æ Telegram
+è´¦å·è¢«å°ç¦æè¢«ç¾¤å°ç¦) ä¸å¼åå¢éæ å³.
+æ¬é¡¹ç®è®¾è®¡åè¡·æ¯å¨ä¸­æ Emby ç¤¾ç¾¤è§åä¸,
+ä¿å·è¦æ±éæ¸èå» (é¨åè¦æ±æ¯æç»å½ææ¯æ¥ç­¾å°),
+è¿ä½¿å¾ä¼é²æ¶é´ç´§å¼ çäººå£«é¾ä»¥å®å¿ä½¿ç¨.
+æ¬é¡¹ç®ä»æ¨å¨å¸®å©è¯¥ç±»äººç¾¤ä¿å·, ä¸é¼å±ææå¤§é Emby
+è´¦å·èä¸ä½¿ç¨,
+å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸º,
+å¼åå¢éä¹å¼åä»ä¿ç 1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby æå¡å¨.
+æ¬é¡¹ç®ä»æä¾å·¥å·,
+å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³.
 æ¬é¡¹ç®æ¬¢è¿ååè®¨è®ºä¸å»ºè®®, æ¨å¯ä»¥éè¿ [Github Issue](https://
 github.com/embykeeper/embykeeper) éå¾åé¦,
-å¹¶è®¤å¯å¼åå¢éå¯ä»¥å é¤æå³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®ºã
-å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½ï¼è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
-Bot](https://t.me/embykeeper_bot)" åéå³é®çæå/
-å¤±è´¥æ¥å¿ä»¥ä¾åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
-æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢ã
-å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·ï¼é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æï¼å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£ã
-## åè½ - Telegram æºå¨äººç­¾å° - æ¯æç¾¤ç» - ç»ç¹ç«: [é¢é]
-(https://t.me/embypub) [ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://
-t.me/EmbyPublicBot) - å·æ¯é¼ : [é¢é]() [ç¾¤ç»](https://t.me/Curly_Mouse)
-[æºå¨äºº](https://t.me/jmsembybot) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/
-CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://
-t.me/JMSIPTV_bot)~~ (æ ååº) - Peach: [é¢é](https://t.me/
-peach_emby_channel) [ç¾¤ç»](https://t.me/peach_emby_chat) [æºå¨äºº](https://
-t.me/peach_emby_bot) - åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1)
-[æºå¨äºº](https://t.me/zckllflbot) - BlueSea: [ç¾¤ç»](https://t.me/
-blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot) - EmbyHub: [é¢é]
-(https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
-t.me/EdHubot) - Singularity: [é¢é](https://t.me/Singularity_Emby_Channel)
-[ç¾¤ç»](https://t.me/Singularity_Emby_Group) [æºå¨äºº](https://t.me/
-Singularity_Emby_Bot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»]
-(https://t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
+å¹¶è®¤å¯å¼åå¢éå¯ä»¥å³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®º.
+æ¨ä¹å¯ä»¥éè¿ [Telegram è®¨è®ºç»](https://t.me/embykeeper_chat)
+ä¸å¼åå¢éè¿è¡äº¤æµ. å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½,
+è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper Auth Bot](https://t.me/
+embykeeper_auth_bot)" åéå³é®çæå/å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper
+Bot](https://t.me/embykeeper_bot)" åæ¨æ¨é,
+æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
+æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
+å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
+å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
+æºå¨äººç­¾å° - æ¯æç¾¤ç» - ç»ç¹ç«: [é¢é](https://t.me/embypub)
+[ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://t.me/EmbyPublicBot) -
+å·æ¯é¼ : [é¢é]() [ç¾¤ç»](https://t.me/Curly_Mouse) [æºå¨äºº](https://
+t.me/jmsembybot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»](https://
+t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
 (ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
-t.me/embykeeper_bot?start=__prime)) - é«çº§ç¹æ§ -
-éªè¯ç è¯å«ä¸èªå¨éè¯ - å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby
+t.me/embykeeper_bot?start=__prime)) - BlueSea: [ç¾¤ç»](https://t.me/
+blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot) - Singularity: [é¢é]
+(https://t.me/Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/
+Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach:
+[é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
+peach_emby_chat) [æºå¨äºº](https://t.me/peach_emby_bot) - EmbyHub: [é¢é]
+(https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
+t.me/EdHubot) - Pornemby (_æµè¯ä¸­_): [é¢é](https://t.me/pornembyservice)
+[æºå¨äºº](https://t.me/PronembyTGBot2_bot) - å¶ä»é Emby ç¸å³: -
+æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/pull/8)
+å¢å ) (_æµè¯ä¸­_) - é»è®¤ç¦ç¨: - Pornemby ç§ä¸¾èè¯ (_æµè¯ä¸­_):
+[æ´»å¨é¢é](https://t.me/PornembyFun) - ~~å·æ¯é¼  IPTV: [é¢é](https://
+t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https:/
+/t.me/JMSIPTV_bot)~~ (æ ååº) - ~~åå¾å½±é³: [ç¾¤ç»](https://t.me/
++3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://t.me/zckllflbot)~~ (æ ååº) - ç¹æ§
+- éªè¯ç è¯å«ä¸èªå¨éè¯ - å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby
 ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
-Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, è¯·è°¨æä½¿ç¨) -
-NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://t.me/NakoNetwork) [æºå¨äºº](https://
-t.me/nakonetwork_bot) - Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·]
-(https://t.me/embykeeper_bot?start=__prime)) - ä¸ç»ç æ¢éè¯·ç : [ç¾¤ç»]
-(https://t.me/Ephemeralemby) [æºå¨äºº](https://t.me/UnknownEmbyBot) - Embyhub
-å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
-emby_hub) [æºå¨äºº](https://t.me/EdHubot) ## å®è£ä¸ä½¿ç¨ Embykeeper
-éè¦ Python ç¯å¢ä»¥è¿è¡, æ¨å¯ä»¥éè¿ [conda](https://github.com/
-conda/conda) æ [virtualvenv](https://virtualenv.pypa.io/
-) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip` å®è£ `embykeeper`
-(éè¦ `python >= 3.7`): ```bash pip install embykeeper ```
-æèæ¨ä¹å¯ä»¥éè¿æºç æå»º: ```bash git clone https://github.com/
-embykeeper/embykeeper.git cd embykeeper make develop ```
-éåï¼æ¨éè¦æ§è¡: ```bash embykeeper ```
-å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml`
-æä»¶ï¼æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ,
-ä»ååè): ```toml [proxy] hostname = "127.0.0.1" port = "1080" scheme =
-"socks5" [[telegram]] api_id = "27894236" api_hash =
-"622159182fdd4b15b627eeb3ac695271" phone = "+8612109347899" [[emby]] url =
-"https://weiss-griffin.com/" username = "carrie19" password = "s*D7MMCpS$" ```
-å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿ [Telegram å®ç½](https://
-my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© API
-development tools, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
-æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
-æ¨å¯è½éè¦æ´æ¢åºç¨åç§°/ç­åç§°/ä»£ç/
-æ¸é¤æµè§å¨è®°å½å¹¶éè¯. ç¶å, è¿è¡: ```bash embykeeper config.toml
-``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½ï¼ç»å½æååï¼Embykeeper
+Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+è¯·è°¨æä½¿ç¨) - NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://t.me/NakoNetwork)
+[æºå¨äºº](https://t.me/nakonetwork_bot) - Telegram èªå¨çæ§ä¿¡æ¯ (éè¦
+[è¶çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) - ä¸ç»ç
+æ¢éè¯·ç : [ç¾¤ç»](https://t.me/Ephemeralemby) [æºå¨äºº](https://t.me/
+UnknownEmbyBot) - Embyhub å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub)
+[ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) ##
+å®è£ä¸ä½¿ç¨ ### ä» Docker å®è£ Embykeeper å¯ä»¥éè¿ `docker` è¿è¡,
+æ¨é[å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
+ç¶åæ§è¡: ```bash touch config.toml docker run -v $(pwd)/config.toml:/app/
+config.toml --rm -it embykeeper/embykeeper ```
+å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
+```toml [proxy] hostname = "127.0.0.1" port = "1080" scheme = "socks5" [
+[telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
+phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+"carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
+[Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
+ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
+è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
+"Error", æ¨å¯è½éè¦æ´æ¢åºç¨åç§°/ç­åç§°/ä»£ç/
+æ¸é¤æµè§å¨è®°å½å¹¶éè¯. éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
+run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥è¿è¡: ```bash tmux ``` è¿å°å¯å¨ä¸ä¸ª `tmux`
-ç»ç«¯ï¼æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`),
-å¹¶æ Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯ã
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash docker
+run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper ```
+æèä½¿ç¨ [docker-compose](https://docs.docker.com/compose/) ([watchtower]
+(https://github.com/containrrr/watchtower) è¢«ç¨äºèªå¨æ´æ°å®¹å¨æå¡):
+```yaml version: '3' services: embykeeper: container_name: embykeeper image:
+cembykeeper/embykeeper restart: unless-stopped volumes: - ./config.toml:/app/
+config.toml watchtower: container_name: watchtower image: containrrr/watchtower
+restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/docker.sock:rw
+``` å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -
+f embykeeper` æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿.
+å¦ææ¨éè¦ä½¿ç¨ä¸»æºä¸çä»£çæå¡å¨ (ä¾å¦ `https://localhost:
+1080`), æ¨å¯è½éè¦ä½¿ç¨ `--net=host` åæ°ä»¥ä½¿ç¨ä¸»æºç½ç»æ¨¡å¼.
+### ä» Pypi å®è£ Embykeeper éè¦ Python ç¯å¢ä»¥è¿è¡, æ¨å¯ä»¥éè¿
+[conda](https://github.com/conda/conda) æ [virtualvenv](https://
+virtualenv.pypa.io/) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip`
+å®è£ `embykeeper` (éè¦ `python >= 3.7, < 3.11`): ```bash pip install
+embykeeper ``` éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
+å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦ä¿®æ¹æ¨çè´¦å·éç½® (è¯¦è§[ä» Docker å®è£](https://
+github.com/embykeeper/embykeeper#%E4%BB%8E%20Docker%20%E5%AE%89%E8%A3%85)).
+éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
+æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
+Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
 æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
-ç»ç«¯. ## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h`
-ä»¥è·åå¸®å©: ```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
-æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
-(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å°
-(ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´»
-(ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --monitor -m å¯ç¨ç¾¤èçè§ --send -
-s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-instant -
-I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
+ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
+ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæå Github å¹¶å®è£:
+```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
+make develop ``` ç¶åå³å¯æ§è¡ Embykeeper: ```bash embykeeper ```
+è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£](https://github.com/embykeeper/
+embykeeper#%E4%BB%8E%20Pypi%20%E5%AE%89%E8%A3%85). å½çæ¬æ´æ°æ¶,
+æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å©
+æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -
+h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°:
+config éç½®æä»¶ (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -
+c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å° (ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -
+e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
+monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
+instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
 follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ ```
 ä¾å¦: ```bash # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
 å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
 è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -
 s ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
@@ -109,17 +146,18 @@
 ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
 å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
 è¯¥å·¥å·å¯ä»¥å®æ¶è¾åºæ¶æ¯ç ID ç­ä¿¡æ¯, ä»¥æ¹ä¾¿è°è¯. ##
 æ¶æ¯æ¨éä¸é«çº§ç¨æ· æ¨å¯ä»¥éè¿è®¾ç½®é¡¹ "`notifier`" è®¾ç½®
 æå/å¤±è´¥ éç¥å°è¢«åéç Telegram è´¦å·, æ¨å¯ä»¥éè¿
 [Embykeeper Bot](https://t.me/embykeeper_bot)
 è®¾ç½®æ¶æ¯æ¯æ¥åéçæ¶é´. æ¬é¡¹ç®æ¶åçéè¦ Cloudflare
-éªè¯ç ä»è´¹è·³è¿çæä½ï¼ä¾å¦ Nebula
-ç­¾å°ï¼ãå¯è½ä¼å¼èµ·ç«äºçæä½ï¼ä¾å¦èªå¨æ¢éè¯·ç ï¼å°éè¦é«çº§ç¨æ·ï¼æ¨å¯ä»¥éè¿
-[Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
+éªè¯ç ä»è´¹è·³è¿çæä½ (ä¾å¦ Nebula
+ç­¾å°)ãå¯è½ä¼å¼èµ·ç«äºçæä½
+(ä¾å¦èªå¨æ¢éè¯·ç )å°éè¦é«çº§ç¨æ·, æ¨å¯ä»¥éè¿ [Embykeeper
+Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
 ç®åæä¸ç§æ¹å¼æä¸ºé«çº§ç¨æ·: 1. åäº« 1 ä¸ªéè¯·å¶ Emby
 çéè¯·ç ; 2. ä¸ºæ¬é¡¹ç®æä¾ [Pull Requests](https://github.com/
 embykeeper/embykeeper/pulls) å¹¶è¢«åå¹¶; 3. éè¿ç±åçµèµå©ä¸ä¸ª
 [å°åå­](https://afdian.net/a/jackzzs); ## æ¯æ Embykeeper #####
 å¼åèå¢é - [jackzzs](https://github.com/jackzzs) ##### éè¿[ç±åçµ]
 (https://afdian.net/a/jackzzs)èµå© ![kitty](images/kitty.gif) ## éç½®é¡¹ |
 è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ------------ | -----------------
@@ -134,56 +172,56 @@
 Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | | `emby` | `list` | Emby
 è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | `service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
 å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------- | ------ | -------------- | ----
 ---------------- | | `checkiner` | `list` | å¯ç¨çç­¾å°ç«ç¹ |
 (å½åæææ¯æçç«ç¹) | | `monitor` | `list` | å¯ç¨ççè§ä¼è¯ |
 (å½åæææ¯æçä¼è¯) | | `messager` | `list` | å¯ç¨çæ°´ç¾¤ä¼è¯ |
 (å½åæææ¯æçä¼è¯) | æ³¨æ, å½æ¨æªæ¾ä¸ç«ç¹æºå¨äººå¯¹è¯,
-è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡. `proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
-å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
------------------ | ----------- | | `hostname` | `str` | ä»£çæå¡å¨å°å
-| `localhost` | | `port` | `int` | ä»£çç«¯å£å· | `1080` | | `scheme` |
-`str` | ä»£çåè®®, å¯ä»¥ä¸º "`socks5`" æ "`http`" | `socks5` | `telegram`
+è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡. è¥æ¨éè¦ç¦ç¨é¨åç­¾å°ç«ç¹,
+æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
+è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
+æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
+ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | --- | --- | --- |--- | --- | |
+åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` | | å·æ¯é¼  IPTV |
+`jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby | `pornemby` | | Singularity
+| `singularity` | | Peach | `peach` | | Nebula | `nebula` | | Bluesea |
+`bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms` | | | | `proxy`
 è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
------- | ------------------------------------------------------------------ | -
------- | | `api_id` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/
-)ç³è¯·ç Application ID | | | `api_hash` | `str` | ä»[Telegram å®ç½]
-(https://my.telegram.org/)ç³è¯·ç Application Hash | | | `phone` | `str` |
-è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | | `monitor` | `bool` |
-å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` | `bool` |
-å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹
-| å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | --------------------
-------------------------------------- | ------ | | `url` | `str` | Emby
-æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | | `username`
-| `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
+------ | --------------------------------------- | ----------- | | `hostname` |
+`str` | ä»£çæå¡å¨å°å | `localhost` | | `port` | `int` |
+ä»£çç«¯å£å· | `1080` | | `scheme` | `str` | ä»£çåè®®, å¯ä»¥ä¸º
+"`socks5`" æ "`http`" | `socks5` | `telegram` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
+å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
+-------------------------------------------- | ------- | | `api_id` | `str` |
+ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID | | |
+`api_hash` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç
+Application Hash | | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`"
+| | | `monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send`
+| `bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: |
+è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------
+----------------------------------------------- | ------ | | `url` | `str` |
+Emby æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | |
+`username` | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
 æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
 `progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
 ## ä»£ç éç¨ä¸å¼å ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-
 terminal cli) --> B(fa:fa-telegram telechecker) A --> C(fa:fa-play embywatcher)
 B --checker--> E[fa:fa-robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --
 messager--> F[fa:fa-message Messager] C --watcher--> H[fa:fa-circle-play
 EmbyWatcher] F ---- |schedule| A ``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: -
 `embykeeper.telechecker.bots` - `embykeeper.telechecker.monitor` -
 `embykeeper.telechecker.messager` éå¸¸æ¥è¯´,
 å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
 ä¸­å¢å ä¸ä¸ªæä»¶ `dummy.py`: ```python from .base import BotCheckin class
 DummyCheckin(BotCheckin): name = "Dummy" bot_username = "dummy" bot_captcha_len
-= 4 ``` æ¨å³å¢å ä¸ä¸ªåä¸º "`Dummy`" çç­¾å°å¨ï¼å°ä¼åç¨æ·åä¸º
-"`dummy`" çæºå¨äººåé "`/checkin`" å¹¶ç­åä¸ä¸ª 4
-ä½çéªè¯ç ï¼è¯å«éªè¯ç åå°åé.
-è¥æ¨å¸æè¯å«éªè¯ç åç¹å»æé®, æ¨å¯ä»¥ä½¿ç¨ `AnswerBotCheckin`,
-æ¨ä¹å¯ä»¥éå `on_captcha` å½æ°æ¥å®ç°èªå®ä¹åè½: ```python from
-.base import AnswerBotCheckin class DummyCheckin(AnswerBotCheckin): .... async
-def on_captcha(self, message: Message, captcha: str): for l in captcha: try:
-await self.message.click(l) except ValueError: self.log.info
-(f'æªè½æ¾å°å¯¹åº "{l}" çæé®, æ­£å¨éè¯.') await self.retry() break
-``` ä¸è¿°ä»£ç å®ç°æ¯æ¬¡æå¯¹åºä¸ä¸ªå­ç¬¦æé®çåè½.
+= 4 ``` æ¨å³å¢å ä¸ä¸ªåä¸º "`Dummy`" çç­¾å°å¨, å°ä¼åç¨æ·åä¸º
+"`dummy`" çæºå¨äººåé "`/checkin`" å¹¶ç­åä¸ä¸ª 4 ä½çéªè¯ç ,
+è¯å«éªè¯ç åå°åé. è¥æ¨å¸æè¯å«éªè¯ç åç¹å»æé®,
+æ¨å¯ä»¥ä½¿ç¨ `AnswerBotCheckin`, æ¨ä¹å¯ä»¥éå `on_captcha`
+å½æ°æ¥å®ç°èªå®ä¹åè½: ```python from .base import AnswerBotCheckin
+class DummyCheckin(AnswerBotCheckin): .... async def on_captcha(self, message:
+Message, captcha: str): for l in captcha: try: await self.message.click(l)
+except ValueError: self.log.info(f'æªè½æ¾å°å¯¹åº "{l}" çæé®,
+æ­£å¨éè¯.') await self.retry() break ```
+ä¸è¿°ä»£ç å®ç°æ¯æ¬¡æå¯¹åºä¸ä¸ªå­ç¬¦æé®çåè½.
 å½æ¨å®ç°ä¸ä¸ªæ°çç­¾å°å¨æ¶, æ¬¢è¿æ¨æåº [Pull Requests](https://
-github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨! Keywords:
-emby,telegram,checkin,automator Platform: UNKNOWN Classifier: Development
-Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
-Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
-(Simplified) Classifier: License :: OSI Approved :: GNU General Public License
-v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Requires-
-Python: >=3.7,<3.11 Description-Content-Type: text/markdown
+github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨!
```

### Comparing `embykeeper-2.0.7/README.md` & `embykeeper-2.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,85 +1,98 @@
+Metadata-Version: 2.1
+Name: embykeeper
+Version: 2.0.8
+Summary: Daily checkin automator for emby bots in telegram.
+Home-page: https://github.com/embykeeper/embykeeper
+Author: jackzzs
+Author-email: jackzzs@outlook.com
+Keywords: emby,telegram,checkin,automator
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.7,<3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
 
 <p align="center">
   <a href='https://github.com/embykeeper/embykeeper'>
     <img src="https://github.com/embykeeper/embykeeper/blob/main/images/logo.svg" alt="Embykeeper" />
   </a>
 </p>
 <p align="center">
     <b>自动签到 定时保号 按需水群</b>
 </p>
 
 ---
 
-Embykeeper 是一个在中文社群规则下用于 Emby 影视服务器的签到和保号的自动执行工具, 基于 Pyrogram 编写并具有可拓展性。
+Embykeeper 是一个在中文社群规则下用于 Emby 影视服务器的签到和保号的自动执行工具, 基于 Pyrogram 编写并具有可拓展性.
 
 ## 声明
 
-本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关，在使用 Embykeeper 时造成的一切损失（包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁）与开发团队无关。
+本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关. 
 
-本项目设计初衷是在中文 Emby 社群规则下，保号要求逐渐苛刻（部分要求每月登录或每日签到），这使得休闲时间紧张的人士难以安心使用。本项目仅旨在帮助该类人群保号，不鼓励持有大量 Emby 账号而不使用，导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为，开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器。本项目仅提供工具，具体使用形式及造成的影响和后果与开发团队无关。
+本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关. 
 
-本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以删除或关闭与项目开发不直接相关的不友善讨论。
+本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Telegram 讨论组](https://t.me/embykeeper_chat) 与开发团队进行交流.
 
-当您使用 "消息提示" 功能，该工具时候将自动向 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 发送关键的成功/失败日志以供向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题。
+当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题. 
 
-当您安装并使用该工具，默认您已经阅读并同意上述声明，并确认自己并非出于"集邮"目的而安装。
+当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装. 
 
 ## 功能
 
 - Telegram 机器人签到
   - 支持群组
     - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
     - 卷毛鼠: [频道]() [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
-    - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
-    - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
-    - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
+    - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
     - BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)
-    - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
     - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
-    - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
-  - 高级特性
+    - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
+    - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
+    - Pornemby (_测试中_): [频道](https://t.me/pornembyservice) [机器人](https://t.me/PronembyTGBot2_bot)
+    - 其他非 Emby 相关:
+      - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加) (_测试中_)
+    - 默认禁用:
+      - Pornemby 科举考试 (_测试中_): [活动频道](https://t.me/PornembyFun)
+      - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
+      - ~~垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)~~ (无响应)
+  - 特性
     - 验证码识别与自动重试
     - 多账户签到
     - 网页类型签到
 - Emby 保活
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
-- Telegram 自动水群 (默认使用内建话术列表, 请谨慎使用)
+- Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
   - NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
   - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
 
 ## 安装与使用
 
-Embykeeper 需要 Python 环境以运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
-
-您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7`):
-
-```bash
-pip install embykeeper
-```
-
-或者您也可以通过源码构建:
-
-```bash
-git clone https://github.com/embykeeper/embykeeper.git
-cd embykeeper
-make develop
-```
+### 从 Docker 安装
 
-随后，您需要执行:
+Embykeeper 可以通过 `docker` 运行, 您需[安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
-embykeeper
+touch config.toml
+docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
 ```
 
-命令将会在当前目录生成模板 `config.toml` 文件，您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
 
 ```toml
 [proxy]
 hostname = "127.0.0.1"
 port = "1080"
 scheme = "socks5"
 
@@ -90,40 +103,131 @@
 
 [[emby]]
 url = "https://weiss-griffin.com/"
 username = "carrie19"
 password = "s*D7MMCpS$"
 ```
 
-对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 API development tools, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要更换应用名称/短名称/代理/清除浏览器记录并重试.
+对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要更换应用名称/短名称/代理/清除浏览器记录并重试.
 
-然后, 运行:
+随后, 您需要再次执行:
 
 ```bash
-embykeeper config.toml
+docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
 ```
 
-您将被询问设备验证码以登录，登录成功后，Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以运行:
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+
+```bash
+docker run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper
+```
+
+或者使用 [docker-compose](https://docs.docker.com/compose/) ([watchtower](https://github.com/containrrr/watchtower) 被用于自动更新容器服务):
+
+```yaml
+version: '3'
+services:
+  embykeeper:
+    container_name: embykeeper
+    image: cembykeeper/embykeeper
+    restart: unless-stopped
+    volumes:
+      - ./config.toml:/app/config.toml
+  watchtower:
+    container_name: watchtower
+    image: containrrr/watchtower
+    restart: unless-stopped
+    volumes:
+      - /var/run/docker.sock:/var/run/docker.sock:rw
+```
+
+即可在后台启动 embykeeper.
+
+您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
+
+如果您需要使用主机上的代理服务器 (例如 `https://localhost:1080`), 您可能需要使用 `--net=host` 参数以使用主机网络模式.
+
+### 从 Pypi 安装
+
+Embykeeper 需要 Python 环境以运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
+
+您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7, < 3.11`):
+
+```bash
+pip install embykeeper
+```
+
+随后, 您需要执行:
+
+```bash
+embykeeper
+```
+
+命令将会在当前目录生成模板 `config.toml` 文件, 您需要修改您的账号配置 (详见[从 Docker 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E%20Docker%20%E5%AE%89%E8%A3%85)).
+
+随后, 您需要再次执行:
+
+```bash
+embykeeper
+```
+
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
 
 ```bash
 tmux
 ```
 
-这将启动一个 `tmux` 终端，您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端。
+这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端. 
 
 您随时可以通过运行:
 
 ```bash
 tmux a
 ```
 
 以重新连接到 `tmux` 终端.
 
+当版本更新时, 您需要执行:
+
+```
+pip install -U embykeeper
+```
+
+然后重新运行应用.
+
+### 从源码构建
+
+首先拉取 Github 并安装:
+
+```bash
+git clone https://github.com/embykeeper/embykeeper.git
+cd embykeeper
+make develop
+```
+
+然后即可执行 Embykeeper:
+
+```bash
+embykeeper
+```
+
+详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E%20Pypi%20%E5%AE%89%E8%A3%85).
+
+当版本更新时, 您需要执行:
+
+```
+git pull
+```
+
+然后重新运行应用.
+
 ## 命令行帮助
 
 您可以通过运行 `embykeeper -h` 以获取帮助:
 
 ```bash
 $ embykeeper -h
 
@@ -177,15 +281,15 @@
 
 该工具可以实时输出消息的 ID 等信息, 以方便调试.
 
 ## 消息推送与高级用户
 
 您可以通过设置项 "`notifier`" 设置 成功/失败 通知将被发送的 Telegram 账号, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot) 设置消息每日发送的时间.
 
-本项目涉及的需要 Cloudflare 验证码付费跳过的操作（例如 Nebula 签到）、可能会引起竞争的操作（例如自动抢邀请码）将需要高级用户，您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) 成为高级用户.
+本项目涉及的需要 Cloudflare 验证码付费跳过的操作 (例如 Nebula 签到)、可能会引起竞争的操作 (例如自动抢邀请码)将需要高级用户, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) 成为高级用户.
 
 目前有三种方式成为高级用户:
 
 1. 分享 1 个邀请制 Emby 的邀请码;
 2. 为本项目提供 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 并被合并;
 3. 通过爱发电赞助一个[小包子](https://afdian.net/a/jackzzs);
 
@@ -218,14 +322,25 @@
 | 设置项      | 值类型 | 简介           | 默认值               |
 | ----------- | ------ | -------------- | -------------------- |
 | `checkiner` | `list` | 启用的签到站点 | (当前所有支持的站点) |
 | `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
 | `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
 
 注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
+若您需要禁用部分签到站点, 您可以在列表中删除对应的名称.
+若您需要使用默认禁用的签到站点, 您可以在列表中增加对应的名称.
+当前支持的名称包括:
+| 站点 | 名称 | | 站点 | 名称 |
+| --- | --- | --- |--- | --- |
+| 垃圾影音 | `ljyy` | | 搜书神器 | `sosdbot` |
+| 卷毛鼠 IPTV | `jms_iptv` | | 终点站 | `terminus` |
+| Pornemby | `pornemby` | | Singularity | `singularity` |
+| Peach | `peach` | | Nebula | `nebula` |
+| Bluesea | `bluesea` | | Embyhub | `embyhub` |
+| 卷毛鼠 | `jms` | | | |
 
 `proxy` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                    | 默认值      |
 | ---------- | ------ | --------------------------------------- | ----------- |
 | `hostname` | `str`  | 代理服务器地址                          | `localhost` |
 | `port`     | `int`  | 代理端口号                              | `1080`      |
@@ -279,15 +394,15 @@
 
 class DummyCheckin(BotCheckin):
     name = "Dummy"
     bot_username = "dummy"
     bot_captcha_len = 4
 ```
 
-您即增加一个名为 "`Dummy`" 的签到器，将会向用户名为 "`dummy`" 的机器人发送 "`/checkin`" 并等候一个 4 位的验证码，识别验证码后将发送.
+您即增加一个名为 "`Dummy`" 的签到器, 将会向用户名为 "`dummy`" 的机器人发送 "`/checkin`" 并等候一个 4 位的验证码, 识别验证码后将发送.
 
 若您希望识别验证码后点击按钮, 您可以使用 `AnswerBotCheckin`, 您也可以重写 `on_captcha` 函数来实现自定义功能:
 
 ```python
 from .base import AnswerBotCheckin
 
 class DummyCheckin(AnswerBotCheckin):
```

#### html2text {}

```diff
@@ -1,100 +1,151 @@
-[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/
-project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/
+Metadata-Version: 2.1 Name: embykeeper Version: 2.0.8 Summary: Daily checkin
+automator for emby bots in telegram. Home-page: https://github.com/embykeeper/
+embykeeper Author: jackzzs Author-email: jackzzs@outlook.com Keywords:
+emby,telegram,checkin,automator Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
+Desktop Classifier: Natural Language :: Chinese (Simplified) Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Requires-Python: >=3.7,<3.11 Description-
+Content-Type: text/markdown License-File: LICENSE [![pypi badge](https://
+img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [!
+[downloads badge](https://img.shields.io/pypi/dm/
 embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
 pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/
 pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license
 badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://
 github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://
 img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [!
 [telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://
 t.me/embykeeper)
                                  [Embykeeper]
                     èªå¨ç­¾å° å®æ¶ä¿å· æéæ°´ç¾¤
 --- Embykeeper æ¯ä¸ä¸ªå¨ä¸­æç¤¾ç¾¤è§åä¸ç¨äº Emby
 å½±è§æå¡å¨çç­¾å°åä¿å·çèªå¨æ§è¡å·¥å·, åºäº Pyrogram
-ç¼åå¹¶å·æå¯æå±æ§ã ## å£°æ æ¬é¡¹ç®æ¶åçä¸å Emby
-æå¡å¨ä¸ Embykeeper å¼åå¢éæ å³ï¼å¨ä½¿ç¨ Embykeeper
-æ¶é æçä¸åæå¤±ï¼åæ¬ä½ä¸éäº Emby æ Telegram
-è´¦å·è¢«å°ç¦æè¢«ç¾¤å°ç¦ï¼ä¸å¼åå¢éæ å³ã
-æ¬é¡¹ç®è®¾è®¡åè¡·æ¯å¨ä¸­æ Emby
-ç¤¾ç¾¤è§åä¸ï¼ä¿å·è¦æ±éæ¸èå»ï¼é¨åè¦æ±æ¯æç»å½ææ¯æ¥ç­¾å°ï¼ï¼è¿ä½¿å¾ä¼é²æ¶é´ç´§å¼ çäººå£«é¾ä»¥å®å¿ä½¿ç¨ãæ¬é¡¹ç®ä»æ¨å¨å¸®å©è¯¥ç±»äººç¾¤ä¿å·ï¼ä¸é¼å±ææå¤§é
-Emby
-è´¦å·èä¸ä½¿ç¨ï¼å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸ºï¼å¼åå¢éä¹å¼åä»ä¿ç
-1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby
-æå¡å¨ãæ¬é¡¹ç®ä»æä¾å·¥å·ï¼å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³ã
+ç¼åå¹¶å·æå¯æå±æ§. ## å£°æ æ¬é¡¹ç®æ¶åçä¸å Emby
+æå¡å¨ä¸ Embykeeper å¼åå¢éæ å³, å¨ä½¿ç¨ Embykeeper
+æ¶é æçä¸åæå¤± (åæ¬ä½ä¸éäº Emby æ Telegram
+è´¦å·è¢«å°ç¦æè¢«ç¾¤å°ç¦) ä¸å¼åå¢éæ å³.
+æ¬é¡¹ç®è®¾è®¡åè¡·æ¯å¨ä¸­æ Emby ç¤¾ç¾¤è§åä¸,
+ä¿å·è¦æ±éæ¸èå» (é¨åè¦æ±æ¯æç»å½ææ¯æ¥ç­¾å°),
+è¿ä½¿å¾ä¼é²æ¶é´ç´§å¼ çäººå£«é¾ä»¥å®å¿ä½¿ç¨.
+æ¬é¡¹ç®ä»æ¨å¨å¸®å©è¯¥ç±»äººç¾¤ä¿å·, ä¸é¼å±ææå¤§é Emby
+è´¦å·èä¸ä½¿ç¨,
+å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸º,
+å¼åå¢éä¹å¼åä»ä¿ç 1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby æå¡å¨.
+æ¬é¡¹ç®ä»æä¾å·¥å·,
+å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³.
 æ¬é¡¹ç®æ¬¢è¿ååè®¨è®ºä¸å»ºè®®, æ¨å¯ä»¥éè¿ [Github Issue](https://
 github.com/embykeeper/embykeeper) éå¾åé¦,
-å¹¶è®¤å¯å¼åå¢éå¯ä»¥å é¤æå³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®ºã
-å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½ï¼è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
-Bot](https://t.me/embykeeper_bot)" åéå³é®çæå/
-å¤±è´¥æ¥å¿ä»¥ä¾åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
-æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢ã
-å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·ï¼é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æï¼å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£ã
-## åè½ - Telegram æºå¨äººç­¾å° - æ¯æç¾¤ç» - ç»ç¹ç«: [é¢é]
-(https://t.me/embypub) [ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://
-t.me/EmbyPublicBot) - å·æ¯é¼ : [é¢é]() [ç¾¤ç»](https://t.me/Curly_Mouse)
-[æºå¨äºº](https://t.me/jmsembybot) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/
-CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://
-t.me/JMSIPTV_bot)~~ (æ ååº) - Peach: [é¢é](https://t.me/
-peach_emby_channel) [ç¾¤ç»](https://t.me/peach_emby_chat) [æºå¨äºº](https://
-t.me/peach_emby_bot) - åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1)
-[æºå¨äºº](https://t.me/zckllflbot) - BlueSea: [ç¾¤ç»](https://t.me/
-blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot) - EmbyHub: [é¢é]
-(https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
-t.me/EdHubot) - Singularity: [é¢é](https://t.me/Singularity_Emby_Channel)
-[ç¾¤ç»](https://t.me/Singularity_Emby_Group) [æºå¨äºº](https://t.me/
-Singularity_Emby_Bot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»]
-(https://t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
+å¹¶è®¤å¯å¼åå¢éå¯ä»¥å³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®º.
+æ¨ä¹å¯ä»¥éè¿ [Telegram è®¨è®ºç»](https://t.me/embykeeper_chat)
+ä¸å¼åå¢éè¿è¡äº¤æµ. å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½,
+è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper Auth Bot](https://t.me/
+embykeeper_auth_bot)" åéå³é®çæå/å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper
+Bot](https://t.me/embykeeper_bot)" åæ¨æ¨é,
+æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
+æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
+å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
+å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
+æºå¨äººç­¾å° - æ¯æç¾¤ç» - ç»ç¹ç«: [é¢é](https://t.me/embypub)
+[ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://t.me/EmbyPublicBot) -
+å·æ¯é¼ : [é¢é]() [ç¾¤ç»](https://t.me/Curly_Mouse) [æºå¨äºº](https://
+t.me/jmsembybot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»](https://
+t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
 (ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
-t.me/embykeeper_bot?start=__prime)) - é«çº§ç¹æ§ -
-éªè¯ç è¯å«ä¸èªå¨éè¯ - å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby
+t.me/embykeeper_bot?start=__prime)) - BlueSea: [ç¾¤ç»](https://t.me/
+blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot) - Singularity: [é¢é]
+(https://t.me/Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/
+Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach:
+[é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
+peach_emby_chat) [æºå¨äºº](https://t.me/peach_emby_bot) - EmbyHub: [é¢é]
+(https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
+t.me/EdHubot) - Pornemby (_æµè¯ä¸­_): [é¢é](https://t.me/pornembyservice)
+[æºå¨äºº](https://t.me/PronembyTGBot2_bot) - å¶ä»é Emby ç¸å³: -
+æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/pull/8)
+å¢å ) (_æµè¯ä¸­_) - é»è®¤ç¦ç¨: - Pornemby ç§ä¸¾èè¯ (_æµè¯ä¸­_):
+[æ´»å¨é¢é](https://t.me/PornembyFun) - ~~å·æ¯é¼  IPTV: [é¢é](https://
+t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https:/
+/t.me/JMSIPTV_bot)~~ (æ ååº) - ~~åå¾å½±é³: [ç¾¤ç»](https://t.me/
++3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://t.me/zckllflbot)~~ (æ ååº) - ç¹æ§
+- éªè¯ç è¯å«ä¸èªå¨éè¯ - å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby
 ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
-Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, è¯·è°¨æä½¿ç¨) -
-NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://t.me/NakoNetwork) [æºå¨äºº](https://
-t.me/nakonetwork_bot) - Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·]
-(https://t.me/embykeeper_bot?start=__prime)) - ä¸ç»ç æ¢éè¯·ç : [ç¾¤ç»]
-(https://t.me/Ephemeralemby) [æºå¨äºº](https://t.me/UnknownEmbyBot) - Embyhub
-å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
-emby_hub) [æºå¨äºº](https://t.me/EdHubot) ## å®è£ä¸ä½¿ç¨ Embykeeper
-éè¦ Python ç¯å¢ä»¥è¿è¡, æ¨å¯ä»¥éè¿ [conda](https://github.com/
-conda/conda) æ [virtualvenv](https://virtualenv.pypa.io/
-) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip` å®è£ `embykeeper`
-(éè¦ `python >= 3.7`): ```bash pip install embykeeper ```
-æèæ¨ä¹å¯ä»¥éè¿æºç æå»º: ```bash git clone https://github.com/
-embykeeper/embykeeper.git cd embykeeper make develop ```
-éåï¼æ¨éè¦æ§è¡: ```bash embykeeper ```
-å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml`
-æä»¶ï¼æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ,
-ä»ååè): ```toml [proxy] hostname = "127.0.0.1" port = "1080" scheme =
-"socks5" [[telegram]] api_id = "27894236" api_hash =
-"622159182fdd4b15b627eeb3ac695271" phone = "+8612109347899" [[emby]] url =
-"https://weiss-griffin.com/" username = "carrie19" password = "s*D7MMCpS$" ```
-å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿ [Telegram å®ç½](https://
-my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© API
-development tools, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
-æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
-æ¨å¯è½éè¦æ´æ¢åºç¨åç§°/ç­åç§°/ä»£ç/
-æ¸é¤æµè§å¨è®°å½å¹¶éè¯. ç¶å, è¿è¡: ```bash embykeeper config.toml
-``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½ï¼ç»å½æååï¼Embykeeper
+Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+è¯·è°¨æä½¿ç¨) - NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://t.me/NakoNetwork)
+[æºå¨äºº](https://t.me/nakonetwork_bot) - Telegram èªå¨çæ§ä¿¡æ¯ (éè¦
+[è¶çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) - ä¸ç»ç
+æ¢éè¯·ç : [ç¾¤ç»](https://t.me/Ephemeralemby) [æºå¨äºº](https://t.me/
+UnknownEmbyBot) - Embyhub å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub)
+[ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) ##
+å®è£ä¸ä½¿ç¨ ### ä» Docker å®è£ Embykeeper å¯ä»¥éè¿ `docker` è¿è¡,
+æ¨é[å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
+ç¶åæ§è¡: ```bash touch config.toml docker run -v $(pwd)/config.toml:/app/
+config.toml --rm -it embykeeper/embykeeper ```
+å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
+```toml [proxy] hostname = "127.0.0.1" port = "1080" scheme = "socks5" [
+[telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
+phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+"carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
+[Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
+ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
+è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
+"Error", æ¨å¯è½éè¦æ´æ¢åºç¨åç§°/ç­åç§°/ä»£ç/
+æ¸é¤æµè§å¨è®°å½å¹¶éè¯. éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
+run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥è¿è¡: ```bash tmux ``` è¿å°å¯å¨ä¸ä¸ª `tmux`
-ç»ç«¯ï¼æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`),
-å¹¶æ Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯ã
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash docker
+run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper ```
+æèä½¿ç¨ [docker-compose](https://docs.docker.com/compose/) ([watchtower]
+(https://github.com/containrrr/watchtower) è¢«ç¨äºèªå¨æ´æ°å®¹å¨æå¡):
+```yaml version: '3' services: embykeeper: container_name: embykeeper image:
+cembykeeper/embykeeper restart: unless-stopped volumes: - ./config.toml:/app/
+config.toml watchtower: container_name: watchtower image: containrrr/watchtower
+restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/docker.sock:rw
+``` å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -
+f embykeeper` æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿.
+å¦ææ¨éè¦ä½¿ç¨ä¸»æºä¸çä»£çæå¡å¨ (ä¾å¦ `https://localhost:
+1080`), æ¨å¯è½éè¦ä½¿ç¨ `--net=host` åæ°ä»¥ä½¿ç¨ä¸»æºç½ç»æ¨¡å¼.
+### ä» Pypi å®è£ Embykeeper éè¦ Python ç¯å¢ä»¥è¿è¡, æ¨å¯ä»¥éè¿
+[conda](https://github.com/conda/conda) æ [virtualvenv](https://
+virtualenv.pypa.io/) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip`
+å®è£ `embykeeper` (éè¦ `python >= 3.7, < 3.11`): ```bash pip install
+embykeeper ``` éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
+å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦ä¿®æ¹æ¨çè´¦å·éç½® (è¯¦è§[ä» Docker å®è£](https://
+github.com/embykeeper/embykeeper#%E4%BB%8E%20Docker%20%E5%AE%89%E8%A3%85)).
+éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
+æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
+Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
 æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
-ç»ç«¯. ## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h`
-ä»¥è·åå¸®å©: ```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
-æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
-(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å°
-(ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´»
-(ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --monitor -m å¯ç¨ç¾¤èçè§ --send -
-s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-instant -
-I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
+ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
+ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæå Github å¹¶å®è£:
+```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
+make develop ``` ç¶åå³å¯æ§è¡ Embykeeper: ```bash embykeeper ```
+è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£](https://github.com/embykeeper/
+embykeeper#%E4%BB%8E%20Pypi%20%E5%AE%89%E8%A3%85). å½çæ¬æ´æ°æ¶,
+æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å©
+æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -
+h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°:
+config éç½®æä»¶ (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -
+c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å° (ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -
+e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
+monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
+instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
 follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ ```
 ä¾å¦: ```bash # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
 å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
 è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -
 s ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
@@ -106,17 +157,18 @@
 ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
 å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
 è¯¥å·¥å·å¯ä»¥å®æ¶è¾åºæ¶æ¯ç ID ç­ä¿¡æ¯, ä»¥æ¹ä¾¿è°è¯. ##
 æ¶æ¯æ¨éä¸é«çº§ç¨æ· æ¨å¯ä»¥éè¿è®¾ç½®é¡¹ "`notifier`" è®¾ç½®
 æå/å¤±è´¥ éç¥å°è¢«åéç Telegram è´¦å·, æ¨å¯ä»¥éè¿
 [Embykeeper Bot](https://t.me/embykeeper_bot)
 è®¾ç½®æ¶æ¯æ¯æ¥åéçæ¶é´. æ¬é¡¹ç®æ¶åçéè¦ Cloudflare
-éªè¯ç ä»è´¹è·³è¿çæä½ï¼ä¾å¦ Nebula
-ç­¾å°ï¼ãå¯è½ä¼å¼èµ·ç«äºçæä½ï¼ä¾å¦èªå¨æ¢éè¯·ç ï¼å°éè¦é«çº§ç¨æ·ï¼æ¨å¯ä»¥éè¿
-[Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
+éªè¯ç ä»è´¹è·³è¿çæä½ (ä¾å¦ Nebula
+ç­¾å°)ãå¯è½ä¼å¼èµ·ç«äºçæä½
+(ä¾å¦èªå¨æ¢éè¯·ç )å°éè¦é«çº§ç¨æ·, æ¨å¯ä»¥éè¿ [Embykeeper
+Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
 ç®åæä¸ç§æ¹å¼æä¸ºé«çº§ç¨æ·: 1. åäº« 1 ä¸ªéè¯·å¶ Emby
 çéè¯·ç ; 2. ä¸ºæ¬é¡¹ç®æä¾ [Pull Requests](https://github.com/
 embykeeper/embykeeper/pulls) å¹¶è¢«åå¹¶; 3. éè¿ç±åçµèµå©ä¸ä¸ª
 [å°åå­](https://afdian.net/a/jackzzs); ## æ¯æ Embykeeper #####
 å¼åèå¢é - [jackzzs](https://github.com/jackzzs) ##### éè¿[ç±åçµ]
 (https://afdian.net/a/jackzzs)èµå© ![kitty](images/kitty.gif) ## éç½®é¡¹ |
 è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ------------ | -----------------
@@ -131,48 +183,56 @@
 Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | | `emby` | `list` | Emby
 è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | `service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
 å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------- | ------ | -------------- | ----
 ---------------- | | `checkiner` | `list` | å¯ç¨çç­¾å°ç«ç¹ |
 (å½åæææ¯æçç«ç¹) | | `monitor` | `list` | å¯ç¨ççè§ä¼è¯ |
 (å½åæææ¯æçä¼è¯) | | `messager` | `list` | å¯ç¨çæ°´ç¾¤ä¼è¯ |
 (å½åæææ¯æçä¼è¯) | æ³¨æ, å½æ¨æªæ¾ä¸ç«ç¹æºå¨äººå¯¹è¯,
-è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡. `proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
-å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
------------------ | ----------- | | `hostname` | `str` | ä»£çæå¡å¨å°å
-| `localhost` | | `port` | `int` | ä»£çç«¯å£å· | `1080` | | `scheme` |
-`str` | ä»£çåè®®, å¯ä»¥ä¸º "`socks5`" æ "`http`" | `socks5` | `telegram`
+è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡. è¥æ¨éè¦ç¦ç¨é¨åç­¾å°ç«ç¹,
+æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
+è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
+æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
+ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | --- | --- | --- |--- | --- | |
+åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` | | å·æ¯é¼  IPTV |
+`jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby | `pornemby` | | Singularity
+| `singularity` | | Peach | `peach` | | Nebula | `nebula` | | Bluesea |
+`bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms` | | | | `proxy`
 è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
------- | ------------------------------------------------------------------ | -
------- | | `api_id` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/
-)ç³è¯·ç Application ID | | | `api_hash` | `str` | ä»[Telegram å®ç½]
-(https://my.telegram.org/)ç³è¯·ç Application Hash | | | `phone` | `str` |
-è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | | `monitor` | `bool` |
-å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` | `bool` |
-å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹
-| å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | --------------------
-------------------------------------- | ------ | | `url` | `str` | Emby
-æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | | `username`
-| `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
+------ | --------------------------------------- | ----------- | | `hostname` |
+`str` | ä»£çæå¡å¨å°å | `localhost` | | `port` | `int` |
+ä»£çç«¯å£å· | `1080` | | `scheme` | `str` | ä»£çåè®®, å¯ä»¥ä¸º
+"`socks5`" æ "`http`" | `socks5` | `telegram` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
+å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
+-------------------------------------------- | ------- | | `api_id` | `str` |
+ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID | | |
+`api_hash` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç
+Application Hash | | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`"
+| | | `monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send`
+| `bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: |
+è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------
+----------------------------------------------- | ------ | | `url` | `str` |
+Emby æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | |
+`username` | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
 æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
 `progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
 ## ä»£ç éç¨ä¸å¼å ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-
 terminal cli) --> B(fa:fa-telegram telechecker) A --> C(fa:fa-play embywatcher)
 B --checker--> E[fa:fa-robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --
 messager--> F[fa:fa-message Messager] C --watcher--> H[fa:fa-circle-play
 EmbyWatcher] F ---- |schedule| A ``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: -
 `embykeeper.telechecker.bots` - `embykeeper.telechecker.monitor` -
 `embykeeper.telechecker.messager` éå¸¸æ¥è¯´,
 å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
 ä¸­å¢å ä¸ä¸ªæä»¶ `dummy.py`: ```python from .base import BotCheckin class
 DummyCheckin(BotCheckin): name = "Dummy" bot_username = "dummy" bot_captcha_len
-= 4 ``` æ¨å³å¢å ä¸ä¸ªåä¸º "`Dummy`" çç­¾å°å¨ï¼å°ä¼åç¨æ·åä¸º
-"`dummy`" çæºå¨äººåé "`/checkin`" å¹¶ç­åä¸ä¸ª 4
-ä½çéªè¯ç ï¼è¯å«éªè¯ç åå°åé.
-è¥æ¨å¸æè¯å«éªè¯ç åç¹å»æé®, æ¨å¯ä»¥ä½¿ç¨ `AnswerBotCheckin`,
-æ¨ä¹å¯ä»¥éå `on_captcha` å½æ°æ¥å®ç°èªå®ä¹åè½: ```python from
-.base import AnswerBotCheckin class DummyCheckin(AnswerBotCheckin): .... async
-def on_captcha(self, message: Message, captcha: str): for l in captcha: try:
-await self.message.click(l) except ValueError: self.log.info
-(f'æªè½æ¾å°å¯¹åº "{l}" çæé®, æ­£å¨éè¯.') await self.retry() break
-``` ä¸è¿°ä»£ç å®ç°æ¯æ¬¡æå¯¹åºä¸ä¸ªå­ç¬¦æé®çåè½.
+= 4 ``` æ¨å³å¢å ä¸ä¸ªåä¸º "`Dummy`" çç­¾å°å¨, å°ä¼åç¨æ·åä¸º
+"`dummy`" çæºå¨äººåé "`/checkin`" å¹¶ç­åä¸ä¸ª 4 ä½çéªè¯ç ,
+è¯å«éªè¯ç åå°åé. è¥æ¨å¸æè¯å«éªè¯ç åç¹å»æé®,
+æ¨å¯ä»¥ä½¿ç¨ `AnswerBotCheckin`, æ¨ä¹å¯ä»¥éå `on_captcha`
+å½æ°æ¥å®ç°èªå®ä¹åè½: ```python from .base import AnswerBotCheckin
+class DummyCheckin(AnswerBotCheckin): .... async def on_captcha(self, message:
+Message, captcha: str): for l in captcha: try: await self.message.click(l)
+except ValueError: self.log.info(f'æªè½æ¾å°å¯¹åº "{l}" çæé®,
+æ­£å¨éè¯.') await self.retry() break ```
+ä¸è¿°ä»£ç å®ç°æ¯æ¬¡æå¯¹åºä¸ä¸ªå­ç¬¦æé®çåè½.
 å½æ¨å®ç°ä¸ä¸ªæ°çç­¾å°å¨æ¶, æ¬¢è¿æ¨æåº [Pull Requests](https://
 github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨!
```

### Comparing `embykeeper-2.0.7/embykeeper/cli.py` & `embykeeper-2.0.8/embykeeper/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import typer
 import asyncio
 from appdirs import user_data_dir
 from schedule import Scheduler
 from dateutil import parser
 
 from . import __author__, __name__, __url__, __version__
-from .utils import Flagged, FlagValueCommand, AsyncTyper, AsyncTaskPool, fail_message
+from .utils import Flagged, FlagValueCommand, AsyncTyper, AsyncTaskPool
 from .settings import prepare_config
 
 app = AsyncTyper(
     pretty_exceptions_show_locals=False,
     rich_markup_mode="rich",
     add_completion=False,
     context_settings={"help_option_names": ["-h", "--help"]},
```

### Comparing `embykeeper-2.0.7/embykeeper/embywatcher/emby.py` & `embykeeper-2.0.8/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.7/embykeeper/embywatcher/main.py` & `embykeeper-2.0.8/embykeeper/embywatcher/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.7/embykeeper/log.py` & `embykeeper-2.0.8/embykeeper/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.7/embykeeper/loop.py` & `embykeeper-2.0.8/embykeeper/loop.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.7/embykeeper/settings.py` & `embykeeper-2.0.8/embykeeper/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
     from tomlkit import document, nl, comment, item, dump, table
     from faker import Faker
     from faker.providers import internet, profile
 
     from .telechecker.main import get_names
     from . import __name__, __version__
 
+    logger.warning("需要输入一个toml格式的config文件.")
+    logger.warning(f'您可以根据生成的参考配置文件 "{path}" 进行配置')
+
     fake = Faker()
     fake.add_provider(internet)
     fake.add_provider(profile)
 
     doc = document()
     doc.add(comment("This is an example config file."))
     doc.add(comment("Please fill in your account information."))
@@ -130,15 +133,15 @@
             }
         )
         t["api_id"].comment("通过 Telegram 官网申请 API: https://my.telegram.org/")
         t["api_hash"].comment("通过 Telegram 官网申请 API: https://my.telegram.org/")
         telegram.append(t)
     doc["telegram"] = telegram
     for t in doc["telegram"]:
-        t.value.item("send").comment("启用该账号的自动水群功能 (需要高级账号)")
+        t.value.item("send").comment("启用该账号的自动水群功能 (谨慎使用)")
         t.value.item("monitor").comment("启用该账号的自动监控功能 (需要高级账号)")
     doc.add(nl())
     doc.add(comment("Emby 账号设置, 您可以重复该片段多次以增加多个账号."))
     emby = []
     for _ in range(2):
         t = item(
             {
@@ -154,23 +157,22 @@
         emby.append(t)
     doc["emby"] = emby
     with open(path, "w+") as f:
         dump(doc, f)
 
 
 def prepare_config(config=None):
+    default_config = "config.toml"
     if not config:
-        logger.warning("需要输入一个toml格式的config文件.")
-        default_config = "config.toml"
         if not Path(default_config).exists():
-            write_faked_config(default_config)
-            logger.warning(f'您可以根据生成的参考配置文件 "{default_config}" 进行配置')
-        return
+            return write_faked_config(default_config)
     with open(config, "rb") as f:
         config = tomllib.load(f)
+    if not config:
+        return write_faked_config(default_config)
     if not check_config(config):
         return
     proxy = config.get("proxy", None)
     if proxy:
         proxy.setdefault("scheme", "socks5")
         proxy.setdefault("hostname", "127.0.0.1")
         proxy.setdefault("port", "1080")
```

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/bots/base.py` & `embykeeper-2.0.8/embykeeper/telechecker/bots/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,15 @@
 
     def __init__(self, client: Client, retries=10, timeout=120, nofail=True):
         self.client = client
         self.retries = retries
         self.timeout = timeout
         self.nofail = nofail
         self.finished = asyncio.Event()
-        username = f"{self.client.me.first_name} {self.client.me.last_name}"
-        self.log = logger.bind(scheme="telechecker", name=self.name, username=username)
+        self.log = logger.bind(scheme="telechecker", name=self.name, username=client.me.name)
 
     async def _start(self):
         try:
             return await self.start()
         except asyncio.CancelledError:
             raise
         except Exception as e:
@@ -78,26 +77,30 @@
     chat_name: str = None  # 在群聊中向机器人签到
 
     def __init__(self, *args, **kw):
         super().__init__(*args, **kw)
         self._is_archived = False
         self._retries = 0
 
-    @asynccontextmanager
-    async def listener(self):
+    def get_filter(self):
         filter = filters.user(self.bot_id or self.bot_username)
         if self.chat_name:
             filter = filter & filters.chat(self.chat_name)
+        return filter
 
-        handlers = [
-            MessageHandler(self._message_handler, filter),
-            EditedMessageHandler(self._message_handler, filter),
+    def get_handlers(self):
+        return [
+            MessageHandler(self._message_handler, self.get_filter()),
+            EditedMessageHandler(self._message_handler, self.get_filter()),
         ]
 
+    @asynccontextmanager
+    async def listener(self):
         group = await self.group_pool.append(self)
+        handlers = self.get_handlers()
         for h in handlers:
             self.client.add_handler(h, group=group)
         yield
         for h in handlers:
             try:
                 self.client.remove_handler(h, group=group)
             except ValueError:
@@ -119,15 +122,15 @@
                 if d.chat.id == chat.id:
                     break
             else:
                 if not self.bot_allow_from_scratch:
                     self.log.info(f'跳过签到: 从未与 "{ident}" 交流.')
                     return None
         bot = await self.client.get_users(self.bot_id or self.bot_username)
-        msg = f"开始执行签到: [green]{bot.first_name}[/] [gray50](@{bot.username})[/]"
+        msg = f"开始执行签到: [green]{bot.name}[/] [gray50](@{bot.username})[/]"
         if chat.title:
             msg += f" @ [green]{chat.title}[/] [gray50](@{chat.username})[/]"
         self.log.info(msg + ".")
         try:
             async with self.listener():
                 if self.bot_use_history is None:
                     await self.send_checkin()
@@ -179,18 +182,19 @@
             await self.message_handler(client, message)
         except OSError as e:
             self.log.info(f'发生错误: "{e}", 正在重试.')
             await self.retry()
         except asyncio.CancelledError:
             raise
         except Exception as e:
-            self.finished.set()
             if self.nofail:
                 self.log.opt(exception=e).warning(f"发生错误:")
+                await self.fail()
             else:
+                await self.fail()
                 raise
         finally:
             message.continue_propagation()
 
     async def message_handler(self, client: Client, message: Message, type=None):
         type = type or self.message_type(message)
         if MessageType.TEXT in type:
@@ -235,43 +239,47 @@
 
     async def on_captcha(self, message: Message, captcha: str):
         await message.reply(captcha)
 
     async def on_text(self, message: Message, text: str):
         if any(s in text for s in to_iterable(self.bot_text_ignore)):
             pass
-        elif any(s in text for s in ("失败", "错误", "超时")):
+        elif any(s in text for s in ("失败", "错误", "超时", "拉黑", "黑名单", "冻结")):
             self.log.info(f"签到失败: 验证码错误, 正在重试.")
             await self.retry()
         elif any(s in text for s in ("成功", "通过", "完成")):
             matches = re.search(self.bot_success_pat, text)
             if matches:
                 self.log.info(f"[yellow]签到成功[/]: + {matches.group(1)} 分 -> {matches.group(2)} 分.")
             else:
                 matches = re.search(r"\d+", text)
                 if matches:
                     self.log.info(f"[yellow]签到成功[/]: 当前 {matches.group(0)} 分.")
                 else:
                     self.log.info(f"[yellow]签到成功[/].")
             self.finished.set()
-        elif any(s in text for s in ("只能", "已经", "下次", "过了", "签过")):
+        elif any(s in text for s in ("只能", "已经", "下次", "过了", "签过", "明日再来")):
             self.log.info(f"今日已经签到过了.")
             self.finished.set()
         else:
             self.log.warning(f"接收到异常返回信息: {text}")
 
     async def retry(self):
         self._retries += 1
         if self._retries <= self.retries:
             await asyncio.sleep(self.bot_retry_wait)
             await self.send_checkin()
         else:
             self.log.warning("超过最大重试次数.")
             self.finished.set()
 
+    async def fail(self, message=None):
+        self.finished.set()
+        self._retries = float("inf")
+
 
 class AnswerBotCheckin(BotCheckin):
     """签到类, 用于按钮模式签到."""
 
     bot_checkin_button_pat: str = None  # 所有按键需要满足的 regex 条件
 
     def __init__(self, *args, **kw):
@@ -319,16 +327,16 @@
 
     def message_type(self, message: Message):
         if self.is_valid_answer(message):
             return MessageType.ANSWER | super().message_type(message)
         else:
             return super().message_type(message)
 
-    async def message_handler(self, client: Client, message: Message):
-        type = self.message_type(message)
+    async def message_handler(self, client: Client, message: Message, type=None):
+        type = type or self.message_type(message)
         if MessageType.ANSWER in type:
             await self.on_answer(message)
         await super().message_handler(client, message, type=type)
 
     async def on_answer(self, message: Message):
         async with self.mutex:
             if self.message:
```

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.0.8/embykeeper/telechecker/bots/jms.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.0.8/embykeeper/telechecker/bots/nebula.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             self.log.warning("无法在时限内完成签到.")
             return False
         else:
             return not self.failed
 
     async def _checkin(self):
         bot = await self.client.get_users(self.bot_username)
-        self.log.info(f"开始执行签到: [green]{bot.first_name}[/] [gray50](@{bot.username})[/].")
+        self.log.info(f"开始执行签到: [green]{bot.name}[/] [gray50](@{bot.username})[/].")
         bot_peer = await self.client.resolve_peer(self.bot_username)
         user_full = await self.client.invoke(GetFullUser(id=bot_peer))
         url = user_full.full_user.bot_info.menu_button.url
         url_auth = (
             await self.client.invoke(RequestWebView(peer=bot_peer, bot=bot_peer, platform="ios", url=url))
         ).url
         scheme = urlparse(url_auth)
```

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.0.8/embykeeper/telechecker/bots/peach.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     name = "Peach"
     bot_username = "peach_emby_bot"
     bot_checkin_cmd = "/start"
     bot_captcha_len = None
     bot_checkin_caption_pat = "请输入验证码"
 
     async def message_handler(self, client, message: Message):
-        if "欢迎使用" in message.caption and message.reply_markup:
+        if message.caption and "欢迎使用" in message.caption and message.reply_markup:
             keys = [k.text for r in message.reply_markup.inline_keyboard for k in r]
             for k in keys:
                 if "签到" in k:
                     await message.click(k)
                     return
         await super().message_handler(client, message)
```

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.0.8/embykeeper/telechecker/bots/singularity.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     name = "Singularity"
     bot_username = "Singularity_Emby_Bot"
     bot_checkin_cmd = "/start"
     bot_captcha_len = None
     bot_checkin_caption_pat = "请输入验证码"
 
     async def message_handler(self, client, message: Message):
-        if "欢迎使用" in message.caption and message.reply_markup:
+        if message.caption and "欢迎使用" in message.caption and message.reply_markup:
             keys = [k.text for r in message.reply_markup.inline_keyboard for k in r]
             for k in keys:
                 if "签到" in k:
                     await message.click(k)
                     return
         await super().message_handler(client, message)
```

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/link.py` & `embykeeper-2.0.8/embykeeper/telechecker/link.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 import asyncio
 import io
 import random
+from typing import Callable, List, Optional, Tuple
 import uuid
 
 import tomli
 from loguru import logger
 from pyrogram import Client, filters
 from pyrogram.handlers import MessageHandler
-from pyrogram.raw.functions.messages import DeleteHistory
 from pyrogram.types import Message
 from rich.text import Text
 
 
 class Link:
     bot = "embykeeper_auth_bot"
 
     def __init__(self, client: Client):
         self.client = client
-        username = f"{self.client.me.first_name} {self.client.me.last_name}"
-        self.log = logger.bind(scheme="telelink", username=username)
+        self.log = logger.bind(scheme="telelink", username=client.me.name)
 
     @property
     def instance(self):
         rd = random.Random()
         rd.seed(uuid.getnode())
         return uuid.UUID(int=rd.getrandbits(128))
 
     @staticmethod
-    async def delete_messages(messages):
-        async def delete(m):
+    async def delete_messages(messages: List[Message]):
+        async def delete(m: Message):
             try:
-                await m.delete(revoke=False)
+                await m.delete(revoke=True)
             except asyncio.CancelledError:
                 pass
 
         return await asyncio.gather(*[delete(m) for m in messages])
 
-    async def post(self, cmd, condition=None, timeout=10):
+    async def post(
+        self, cmd, condition: Callable = None, timeout: int = 10, name: str = None
+    ) -> Tuple[Optional[str], Optional[str]]:
         results = {}
         ok = asyncio.Event()
         handler = self.get_handler(cmd, results, ok, condition)
         handler = MessageHandler(handler, filters.text & filters.bot & filters.user(self.bot))
         self.client.add_handler(handler)
         messages = []
         messages.append(await self.client.send_message(self.bot, f"/start quiet"))
@@ -51,77 +52,85 @@
         except asyncio.CancelledError:
             try:
                 await asyncio.wait_for(self.delete_messages(messages), 1.0)
             except asyncio.TimeoutError:
                 pass
             finally:
                 raise
-        else:
-            await self.delete_messages(messages)
-            return results
-        finally:
-            self.client.remove_handler(handler)
-
-    async def preprocess(self, post, name):
-        try:
-            results = await post
         except asyncio.TimeoutError:
+            await self.delete_messages(messages)
             self.log.warning(f"{name}超时.")
             return None
-        status, errmsg = [results.get(p, None) for p in ("status", "errmsg")]
-        if status == "error":
-            self.log.warning(f"{name}错误: {errmsg}.")
-            return None
-        elif status == "ok":
-            return results
         else:
-            self.log.warning(f"{name}出现未知错误.")
-            return None
+            await self.delete_messages(messages)
+            status, errmsg = [results.get(p, None) for p in ("status", "errmsg")]
+            if status == "error":
+                self.log.warning(f"{name}错误: {errmsg}.")
+                return None
+            elif status == "ok":
+                return results
+            else:
+                self.log.warning(f"{name}出现未知错误.")
+                return None
+        finally:
+            self.client.remove_handler(handler)
 
     @staticmethod
     def get_handler(cmd, results, ok, condition=None):
         async def _handler(client: Client, message: Message):
             try:
                 toml = tomli.loads(message.text)
             except tomli.TOMLDecodeError:
                 await message.delete(revoke=False)
                 return
             else:
-                if toml.get("command", None) == cmd:
-                    if condition is None:
-                        cond = True
-                    elif asyncio.iscoroutinefunction(condition):
-                        cond = await condition(toml)
-                    elif callable(condition):
-                        cond = condition(toml)
-                    if cond:
-                        results.update(toml)
-                        ok.set()
-                        await message.delete(revoke=False)
-                        return
-                message.continue_propagation()
+                try:
+                    if toml.get("command", None) == cmd:
+                        if condition is None:
+                            cond = True
+                        elif asyncio.iscoroutinefunction(condition):
+                            cond = await condition(toml)
+                        elif callable(condition):
+                            cond = condition(toml)
+                        if cond:
+                            results.update(toml)
+                            ok.set()
+                            await asyncio.sleep(0.5)
+                            await message.delete(revoke=False)
+                            return
+                except asyncio.CancelledError:
+                    try:
+                        await asyncio.wait_for(message.delete(revoke=False), 1.0)
+                    except asyncio.TimeoutError:
+                        pass
+                    finally:
+                        raise
+                else:
+                    message.continue_propagation()
 
         return _handler
 
     async def auth(self, service: str):
-        post = self.post(f"/auth {service} {self.instance}")
-        results = await self.preprocess(post, name=f"服务 {service.capitalize()} 认证")
+        results = await self.post(f"/auth {service} {self.instance}", name=f"服务 {service.capitalize()} 认证")
         return bool(results)
 
     async def captcha(self):
-        post = self.post("/captcha", timeout=240)
-        results = await self.preprocess(post, name="请求跳过验证码")
+        results = await self.post(f"/captcha {self.instance}", timeout=240, name="请求跳过验证码")
         if results:
             return [results.get(p, None) for p in ("token", "proxy", "useragent")]
         else:
             return None, None, None
 
+    async def answer(self, question: str):
+        results = await self.post(f"/answer {self.instance} {question}", timeout=60, name="请求问题回答")
+        if results:
+            return results.get("answer", None)
+
     async def sendlog(self, message):
-        post = self.post(f"/log {self.instance} {message}")
-        results = await self.preprocess(post, name="发送日志到 Telegram ")
+        results = await self.post(f"/log {self.instance} {message}", name="发送日志到 Telegram ")
         return bool(results)
 
 
 class TelegramStream(io.TextIOWrapper):
     def __init__(self, link: Link = None):
         super().__init__(io.BytesIO(), line_buffering=True)
         self.link = link
```

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/main.py` & `embykeeper-2.0.8/embykeeper/telechecker/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 from logging import StreamHandler
 from typing import List, Type
 from importlib import import_module
 
 from dateutil import parser
 from pyrogram.enums import ChatType
 from pyrogram.handlers import MessageHandler
-from pyrogram.types import Message
+from pyrogram.types import Message, Update
 from rich import box
 from rich.live import Live
 from rich.panel import Panel
 from rich.progress import MofNCompleteColumn, Progress, SpinnerColumn
 from rich.table import Column, Table
 from rich.text import Text
+from rich.pretty import pprint
 
 from ..utils import batch, flatten, idle, time_in_range, async_partial
 from ..log import logger, formatter
 from . import __name__
 from .link import Link, TelegramStream
 from .tele import Client, ClientsSession
 from .bots.base import BaseBotCheckin
@@ -91,15 +92,15 @@
         user = message.from_user
         sender_id = str(user.id)
         sender_icon = "👤"
         if message.outgoing:
             sender = Text("Me", style="bold red")
             text = Text(text, style="red")
         else:
-            sender = f"{user.first_name} {user.last_name}"
+            sender = user.name
             if user.is_bot:
                 sender_icon = "🤖"
                 sender = Text(sender, style="bold yellow")
     else:
         sender = sender_id = sender_icon = None
 
     chat_id = "{: }".format(message.chat.id)
@@ -111,15 +112,15 @@
         chat_icon = "📢"
     elif message.chat.type == ChatType.BOT:
         chat = None
         chat_icon = "🤖"
     else:
         chat = chat_icon = None
     return table.add_row(
-        f"{client.me.first_name} {client.me.last_name}",
+        f"{client.me.name}",
         "│",
         chat_icon,
         chat,
         chat_id,
         "│",
         sender_icon,
         sender,
@@ -136,20 +137,18 @@
 
 
 async def gather_task(tasks, username):
     return username, await asyncio.gather(*tasks)
 
 
 async def checkiner(config: dict, instant=False):
-    asyncio.sleep(10)
     async with ClientsSession.from_config(config) as clients:
         coros = []
         async for tg in clients:
-            username = f"{tg.me.first_name} {tg.me.last_name}"
-            log = logger.bind(scheme="telechecker", username=username)
+            log = logger.bind(scheme="telechecker", username=tg.me.name)
             if not await Link(tg).auth("checkiner"):
                 log.error(f"功能初始化失败: 权限校验不通过.")
                 continue
             sem = asyncio.Semaphore(int(config.get("concurrent", 1)))
             clses = extract(get_cls("checkiner", names=config.get("service", {}).get("checkiner", None)))
             checkiners = [
                 cls(
@@ -161,15 +160,15 @@
                 for cls in clses
             ]
             tasks = []
             for c in checkiners:
                 wait = 0 if instant else random.randint(0, 60 * config.get("random", 15))
                 task = asyncio.create_task(checkin_task(c, sem, wait))
                 tasks.append(task)
-            coros.append(gather_task(tasks, username=username))
+            coros.append(gather_task(tasks, username=tg.me.name))
         while coros:
             done, coros = await asyncio.wait(coros, return_when=asyncio.FIRST_COMPLETED)
             for t in done:
                 username, results = await t
                 log = logger.bind(scheme="telechecker", username=username)
                 failed = []
                 ignored = []
@@ -194,16 +193,15 @@
                     log.bind(notify=True).info(f"签到成功 ({spec}).")
 
 
 async def monitorer(config: dict):
     jobs = []
     async with ClientsSession.from_config(config, monitor=True) as clients:
         async for tg in clients:
-            username = f"{tg.me.first_name} {tg.me.last_name}"
-            log = logger.bind(scheme="telemonitor", username=username)
+            log = logger.bind(scheme="telemonitor", username=tg.me.name)
             if not await Link(tg).auth("monitorer"):
                 log.error(f"功能初始化失败: 权限校验不通过.")
                 continue
             clses = extract(get_cls("monitor", names=config.get("service", {}).get("monitor", None)))
             names = []
             for cls in clses:
                 jobs.append(asyncio.create_task(cls(tg, nofail=config.get("nofail", True))._start()))
@@ -212,25 +210,24 @@
                 log.info(f'已启用监控器: {",".join(names)}')
         await asyncio.gather(*jobs)
 
 
 async def messager(config: dict, scheduler):
     async with ClientsSession.from_config(config, send=True) as clients:
         async for tg in clients:
-            username = f"{tg.me.first_name} {tg.me.last_name}"
-            log = logger.bind(scheme="telemessager", username=username)
+            log = logger.bind(scheme="telemessager", username=tg.me.name)
             if not await Link(tg).auth("messager"):
                 log.error(f"功能初始化失败: 权限校验不通过.")
                 continue
             clses = extract(get_cls("messager", names=config.get("service", {}).get("messager", None)))
             for cls in clses:
                 cls(
                     {"api_id": tg.api_id, "api_hash": tg.api_hash, "phone": tg.phone_number},
                     scheduler,
-                    username=username,
+                    username=tg.me.name,
                     proxy=config.get("proxy", None),
                     nofail=config.get("nofail", True),
                 ).start()
 
 
 async def follower(config: dict):
     columns = [
@@ -275,17 +272,16 @@
         return page
 
     texts = {}
     if timerange:
         start, end = (parser.parse(t).time() for t in timerange)
     async with ClientsSession.from_config(config) as clients:
         async for tg in clients:
-            username = f"{tg.me.first_name} {tg.me.last_name}"
-            target = f"{username}.msgs"
-            logger.info(f'开始分析账号: "{username}", 结果将写入"{target}".')
+            target = f"{tg.me.name}.msgs"
+            logger.info(f'开始分析账号: "{tg.me.name}", 结果将写入"{target}".')
             pcs = list(Progress.get_default_columns())
             pcs.insert(0, SpinnerColumn())
             pcs.insert(3, MofNCompleteColumn(table_column=Column(justify="center")))
             p = Progress(*pcs, transient=True)
             with Live(render_page(p, texts)) as live:
                 updates = 0
                 pchats = p.add_task("[red]会话: ", total=len(chats))
```

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/messager/base.py` & `embykeeper-2.0.8/embykeeper/telechecker/messager/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,16 +63,15 @@
             if only.startswith("weekday") and today.weekday() > 4:
                 return self.log.info(f"由于非周末, 本次发送被跳过.")
             if only.startswith("weekend") and today.weekday() < 5:
                 return self.log.info(f"由于非工作日, 本次发送被跳过.")
         async with ClientsSession([self.account], proxy=self.proxy) as clients:
             async for tg in clients:
                 chat = await tg.get_chat(self.chat_name)
-                username = f"{tg.me.first_name} {tg.me.last_name}"
-                self.log.bind(username=username).info(f'向聊天 "{chat.title or chat.first_name}" 发送: {message}')
+                self.log.bind(username=tg.me.name).info(f'向聊天 "{chat.name}" 发送: {message}')
                 try:
                     await tg.send_message(self.chat_name, message)
                 except BadRequest as e:
                     self.log.warning(f"发送失败: {e}.")
                 except KeyError as e:
                     self.log.warning(f"发送失败, 您可能已被封禁: {e}.")
             reschedule()
@@ -94,15 +93,15 @@
 
     def schedule(self, message, at, every, possibility, only):
         def once(*args):
             try:
                 asyncio.create_task(self._send(*args))
             finally:
                 return CancelJob
-            
+
         def reschedule():
             if not at:
                 return
             _at = [a if isinstance(a, time) else parser.parse(a).time() for a in to_iterable(at)]
             if len(_at) == 1:
                 t = _at[0]
             elif len(_at) == 2:
@@ -114,10 +113,12 @@
             else:
                 m = message
             _every = every.split()
             if len(_every) > 1:
                 n, *_every = _every
             else:
                 n = 1
-            getattr(self.scheduler.every(int(n)), _every[0]).at(t.strftime("%H:%M:%S")).do(once, m, reschedule, possibility, only)
+            getattr(self.scheduler.every(int(n)), _every[0]).at(t.strftime("%H:%M:%S")).do(
+                once, m, reschedule, possibility, only
+            )
 
         reschedule()
```

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/messager/common.py` & `embykeeper-2.0.8/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.0.8/embykeeper/telechecker/monitor/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 import asyncio
 import random
 import re
 from contextlib import asynccontextmanager
+import string
 from typing import List, Sized, Union
 
 from loguru import logger
 from pyrogram import filters
 from pyrogram.enums import ChatMemberStatus
 from pyrogram.errors import UsernameNotOccupied, UserNotParticipant
 from pyrogram.handlers import EditedMessageHandler, MessageHandler
-from pyrogram.types import Message
+from pyrogram.types import Message, User
 
 from ...utils import to_iterable, truncate_str, AsyncCountPool
 from ..tele import Client
 
 __ignore__ = True
 
 
@@ -59,49 +60,76 @@
 
     async def cancel(self):
         self.canceled.set()
         self.delayed.set()
         self.followed.set()
 
 
+class UniqueUsername(dict):
+    def __getitem__(self, user: User):
+        if not user.id in self:
+            self[user.id] = self.get_unique(user)
+        return dict.__getitem__(self, user.id)
+
+    @staticmethod
+    def get_unique(user: User):
+        log = logger.bind(scheme="telemonitor", username=user.name)
+        if user.username:
+            unique = user.username
+        else:
+            unique: str = user.name.lower()
+        unique = re.sub(r"[^A-Za-z0-9]", "", unique)
+        random_bits = 10 - len(unique)
+        if random_bits:
+            random_bits = "".join(random.choice(string.digits) for _ in range(random_bits))
+            unique = unique + random_bits
+        log.info(f'当监控到开注时, 将以用户名 "{unique}" 注册, 请[yellow]保证[/]具有一定独特性以避免注册失败.')
+        return unique
+
+
 class Monitor:
     group_pool = AsyncCountPool(base=1000)
+    unique_cache = UniqueUsername()
 
     name: str = None  # 监控器名称
     chat_name: str = None  # 群聊名称
     chat_allow_outgoing: bool = False  # 是否支持自己发言触发
     chat_user: Union[str, List[str]] = []  # 仅被列表中用户的发言触发
     chat_keyword: Union[str, List[str]] = []  # 仅当消息含有列表中的关键词时触发, 支持 regex
     chat_probability: float = 1.0  # 发信概率
     chat_delay: int = 0  # 发信延迟
     chat_follow_user: int = 0  # 需要等待 N 个用户发送 {chat_reply} 方可回复
     chat_reply: str = None  # 回复的内容, 可以通过 @property 类属性重写.
+    notify_create_name: bool = False  # 启动时生成 unique name 并提示
 
     def __init__(self, client: Client, nofail=True):
         self.client = client
         self.nofail = nofail
-        username = f"{self.client.me.first_name} {self.client.me.last_name}"
-        self.log = logger.bind(scheme="telemonitor", name=self.name, username=username)
+        self.log = logger.bind(scheme="telemonitor", name=self.name, username=client.me.name)
         self.session = None
         self.failed = asyncio.Event()
 
-    @asynccontextmanager
-    async def listener(self):
+    def get_filter(self):
         filter = filters.caption | filters.text
         if self.chat_name:
             filter = filter & filters.chat(self.chat_name)
         if not self.chat_allow_outgoing:
             filter = filter & (~filters.outgoing)
+        return filter
 
-        handlers = [
-            MessageHandler(self._message_handler, filter),
-            EditedMessageHandler(self._message_handler, filter),
+    def get_handlers(self):
+        return [
+            MessageHandler(self._message_handler, self.get_filter()),
+            EditedMessageHandler(self._message_handler, self.get_filter()),
         ]
 
+    @asynccontextmanager
+    async def listener(self):
         group = await self.group_pool.append(self)
+        handlers = self.get_handlers()
         for h in handlers:
             self.client.add_handler(h, group=group)
         yield
         for h in handlers:
             try:
                 self.client.remove_handler(h, group=group)
             except ValueError:
@@ -130,14 +158,16 @@
             me = await chat.get_member("me")
         except UserNotParticipant:
             self.log.warning(f'初始化错误: 尚未加入群组 "{chat.title}".')
             return False
         if me.status in (ChatMemberStatus.LEFT, ChatMemberStatus.RESTRICTED):
             self.log.warning(f'初始化错误: 被群组 "{chat.title}" 禁言.')
             return False
+        if self.notify_create_name:
+            self.unique_name = self.get_unique_name()
         spec = f"[green]{chat.title}[/] [gray50](@{chat.username})[/]"
         self.log.info(f"开始监视: {spec}.")
         async with self.listener():
             await self.failed.wait()
             self.log.error(f"发生错误, 不再监视: {spec}.")
             return False
 
@@ -213,13 +243,16 @@
                 await self.on_trigger(message, keys, reply)
         else:
             if self.session and not self.session.followed.is_set():
                 text = message.text or message.caption
                 if self.session.reply == text:
                     now = await self.session.follow()
                     self.log.info(
-                        f'从众计数 ({self.chat_follow_user - now}/{self.chat_follow_user}): "{message.from_user.first_name}"'
+                        f'从众计数 ({self.chat_follow_user - now}/{self.chat_follow_user}): "{message.from_user.name}"'
                     )
 
     async def on_trigger(self, message: Message, keys: Union[List[str], str], reply: str):
         if reply:
             return await self.client.send_message(message.chat.id, reply)
+
+    def get_unique_name(self):
+        return Monitor.unique_cache[self.client.me]
```

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.0.8/embykeeper/telechecker/monitor/bgk.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,12 +4,14 @@
 
 
 class BGKMonitor(Monitor):
     name = "不给看"
     chat_name = "Ephemeralemby"
     chat_keyword = r"(?:^|\s)([a-zA-Z0-9]{32})(?!\S)"
     bot_username = "UnknownEmbyBot"
+    notify_create_name = True
 
     async def on_trigger(self, message: Message, keys, reply):
         await self.client.send_message(self.bot_username, "/invite")
         await self.client.send_message(self.bot_username, keys[0])
+        await self.client.send_message(self.bot_username, self.unique_name)
         self.log.bind(notify=True).info(f'已向Bot发送邀请码: "{keys[0]}", 请查看.')
```

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.0.8/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.7/embykeeper/telechecker/tele.py` & `embykeeper-2.0.8/embykeeper/telechecker/tele.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,40 @@
 import asyncio
-from typing import AsyncGenerator, Optional
+from typing import AsyncGenerator, Optional, Union
 
 from rich.prompt import Prompt
 from appdirs import user_data_dir
 from loguru import logger
 from pyrogram import Client as _Client
 from pyrogram import raw, types, utils
 from pyrogram.enums import SentCodeType
 from pyrogram.errors import BadRequest, RPCError, Unauthorized, SessionPasswordNeeded
 from aiocache import Cache
-from aiocache.serializers import PickleSerializer
 
 from .. import __name__, __version__
 from ..utils import to_iterable
 
 logger = logger.bind(scheme="telegram")
 
 
+def _name(self: Union[types.User, types.Chat]):
+    return " ".join([n for n in (self.first_name, self.last_name) if n])
+
+
+def _chat_name(self: types.Chat):
+    if self.title:
+        return self.title
+    else:
+        return _name(self)
+
+
+setattr(types.User, "name", property(_name))
+setattr(types.Chat, "name", property(_chat_name))
+
+
 class Client(_Client):
     def __init__(self, *args, **kw):
         super().__init__(*args, **kw)
         self.cache = Cache()
 
     async def authorize(self):
         if self.bot_token:
```

### Comparing `embykeeper-2.0.7/embykeeper/utils.py` & `embykeeper-2.0.8/embykeeper/utils.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.0.7/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.0.8/embykeeper.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,329 +1,422 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.0.7
+Version: 2.0.8
 Summary: Daily checkin automator for emby bots in telegram.
 Home-page: https://github.com/embykeeper/embykeeper
 Author: jackzzs
 Author-email: jackzzs@outlook.com
-License: UNKNOWN
-Description: [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
-        
-        <p align="center">
-          <a href='https://github.com/embykeeper/embykeeper'>
-            <img src="https://github.com/embykeeper/embykeeper/blob/main/images/logo.svg" alt="Embykeeper" />
-          </a>
-        </p>
-        <p align="center">
-            <b>自动签到 定时保号 按需水群</b>
-        </p>
-        
-        ---
-        
-        Embykeeper 是一个在中文社群规则下用于 Emby 影视服务器的签到和保号的自动执行工具, 基于 Pyrogram 编写并具有可拓展性。
-        
-        ## 声明
-        
-        本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关，在使用 Embykeeper 时造成的一切损失（包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁）与开发团队无关。
-        
-        本项目设计初衷是在中文 Emby 社群规则下，保号要求逐渐苛刻（部分要求每月登录或每日签到），这使得休闲时间紧张的人士难以安心使用。本项目仅旨在帮助该类人群保号，不鼓励持有大量 Emby 账号而不使用，导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为，开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器。本项目仅提供工具，具体使用形式及造成的影响和后果与开发团队无关。
-        
-        本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以删除或关闭与项目开发不直接相关的不友善讨论。
-        
-        当您使用 "消息提示" 功能，该工具时候将自动向 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 发送关键的成功/失败日志以供向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题。
-        
-        当您安装并使用该工具，默认您已经阅读并同意上述声明，并确认自己并非出于"集邮"目的而安装。
-        
-        ## 功能
-        
-        - Telegram 机器人签到
-          - 支持群组
-            - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
-            - 卷毛鼠: [频道]() [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
-            - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
-            - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
-            - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
-            - BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)
-            - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
-            - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
-            - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
-          - 高级特性
-            - 验证码识别与自动重试
-            - 多账户签到
-            - 网页类型签到
-        - Emby 保活
-          - 定时模拟账号登录视频播放
-          - 播放时间与进度模拟
-        - Telegram 自动水群 (默认使用内建话术列表, 请谨慎使用)
-          - NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)
-        - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
-          - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
-          - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
-        
-        ## 安装与使用
-        
-        Embykeeper 需要 Python 环境以运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
-        
-        您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7`):
-        
-        ```bash
-        pip install embykeeper
-        ```
-        
-        或者您也可以通过源码构建:
-        
-        ```bash
-        git clone https://github.com/embykeeper/embykeeper.git
-        cd embykeeper
-        make develop
-        ```
-        
-        随后，您需要执行:
-        
-        ```bash
-        embykeeper
-        ```
-        
-        命令将会在当前目录生成模板 `config.toml` 文件，您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
-        
-        ```toml
-        [proxy]
-        hostname = "127.0.0.1"
-        port = "1080"
-        scheme = "socks5"
-        
-        [[telegram]]
-        api_id = "27894236"
-        api_hash = "622159182fdd4b15b627eeb3ac695271"
-        phone = "+8612109347899"
-        
-        [[emby]]
-        url = "https://weiss-griffin.com/"
-        username = "carrie19"
-        password = "s*D7MMCpS$"
-        ```
-        
-        对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 API development tools, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要更换应用名称/短名称/代理/清除浏览器记录并重试.
-        
-        然后, 运行:
-        
-        ```bash
-        embykeeper config.toml
-        ```
-        
-        您将被询问设备验证码以登录，登录成功后，Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
-        
-        恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以运行:
-        
-        ```bash
-        tmux
-        ```
-        
-        这将启动一个 `tmux` 终端，您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端。
-        
-        您随时可以通过运行:
-        
-        ```bash
-        tmux a
-        ```
-        
-        以重新连接到 `tmux` 终端.
-        
-        ## 命令行帮助
-        
-        您可以通过运行 `embykeeper -h` 以获取帮助:
-        
-        ```bash
-        $ embykeeper -h
-        
-        欢迎使用 Embykeeper. 🎦 无参数默认开启全部功能.
-        
-        参数:
-            config  配置文件 (置空以生成)
-        模块开关:
-            --checkin     -c   启用每日指定时间签到 (不指定值时默认为6:00PM)
-            --emby        -e   启用每隔天数Emby自动保活 (不指定值时默认为每7天)
-            --monitor     -m   启用群聊监视
-            --send        -s   启用自动水群
-        调试参数:
-            --no-instant  -I   不立刻执行一次计划任务
-            --debug       -d   开启调试模式, 错误将会导致程序停止运行
-            --version     -v   打印 Embykeeper 版本
-            --follow      -f   仅启动消息调试
-            --analyze     -a   仅启动历史信息分析
-        ```
-        
-        例如:
-        
-        ```bash
-        # 仅启动每日签到
-        $ embykeeper config.toml -c
-        
-        # 仅启动每日 8:00 PM 签到
-        $ embykeeper config.toml -c 8:00PM
-        
-        # 启动所有功能, 同时调整签到时间为 8:00 AM, 调整保活间隔天数为 14
-        $ embykeeper config.toml -c 8:00PM -e 14 -m -s
-        ```
-        
-        您也可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
-        
-        ```bash
-        # 启动历史信息分析
-        $ embykeeper config.toml -a
-        
-        请输入群组用户名 (以空格分隔): https://t.me/XXX YYY 10253512
-        请输入关键词 (以空格分隔):
-        输入时间范围 (以"-"分割): 8:00AM-10:00AM
-        请输入各群组最大获取数量 [1000]:
-        ```
-        
-        该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
-        
-        另一个工具是即时信息分析:
-        
-        ![follow screenshot](images/follow.svg)
-        
-        该工具可以实时输出消息的 ID 等信息, 以方便调试.
-        
-        ## 消息推送与高级用户
-        
-        您可以通过设置项 "`notifier`" 设置 成功/失败 通知将被发送的 Telegram 账号, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot) 设置消息每日发送的时间.
-        
-        本项目涉及的需要 Cloudflare 验证码付费跳过的操作（例如 Nebula 签到）、可能会引起竞争的操作（例如自动抢邀请码）将需要高级用户，您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) 成为高级用户.
-        
-        目前有三种方式成为高级用户:
-        
-        1. 分享 1 个邀请制 Emby 的邀请码;
-        2. 为本项目提供 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 并被合并;
-        3. 通过爱发电赞助一个[小包子](https://afdian.net/a/jackzzs);
-        
-        ## 支持 Embykeeper
-        
-        ##### 开发者团队
-        
-        - [jackzzs](https://github.com/jackzzs)
-        
-        ##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
-        
-        ![kitty](images/kitty.gif)
-        
-        ## 配置项
-        
-        | 设置项       | 值类型             | 简介                                         | 默认值  |
-        | ------------ | ------------------ | -------------------------------------------- | ------- |
-        | `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
-        | `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `10`    |
-        | `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
-        | `random`     | `int`              | Telegram 机器人签到定时任务时间随机量 (分钟) | `15`    |
-        | `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
-        | `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
-        | `proxy`      | `dict`             | 代理设置                                     | `{}`    |
-        | `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
-        | `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
-        
-        `service`设置可以为:
-        
-        | 设置项      | 值类型 | 简介           | 默认值               |
-        | ----------- | ------ | -------------- | -------------------- |
-        | `checkiner` | `list` | 启用的签到站点 | (当前所有支持的站点) |
-        | `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
-        | `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
-        
-        注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
-        
-        `proxy` 设置可以为:
-        
-        | 设置项     | 值类型 | 简介                                    | 默认值      |
-        | ---------- | ------ | --------------------------------------- | ----------- |
-        | `hostname` | `str`  | 代理服务器地址                          | `localhost` |
-        | `port`     | `int`  | 代理端口号                              | `1080`      |
-        | `scheme`   | `str`  | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
-        
-        `telegram` 设置可以为:
-        
-        | 设置项     | 值类型 | 简介                                                               | 默认值  |
-        | ---------- | ------ | ------------------------------------------------------------------ | ------- |
-        | `api_id`   | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
-        | `api_hash` | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
-        | `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                      |         |
-        | `monitor`  | `bool` | 启用群组监控系列功能                                               | `false` |
-        | `send`     | `bool` | 启用自动水群系列功能                                               | `false` |
-        
-        `emby` 设置可以为:
-        
-        | 设置项     | 值类型 | 简介                                                      | 默认值 |
-        | ---------- | ------ | --------------------------------------------------------- | ------ |
-        | `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
-        | `username` | `str`  | Emby 服务器用户名                                         |        |
-        | `password` | `str`  | Emby 服务器密码                                           |        |
-        | `time`     | `int`  | 模拟观看的时间 (秒)                                       | `800`  |
-        | `progress` | `int`  | 观看后模拟进度条保存的时间 (秒)                           | `1000` |
-        
-        ## 代码重用与开发
-        
-        代码架构如下:
-        
-        ```mermaid
-        flowchart TD
-            A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
-            A --> C(fa:fa-play embywatcher)
-            B --checker--> E[fa:fa-robot Bot]
-            B --monitor--> G[fa:fa-eye Monitor]
-            B --messager--> F[fa:fa-message Messager]
-            C --watcher--> H[fa:fa-circle-play EmbyWatcher]
-            F ---- |schedule| A
-        ```
-        
-        主要可以扩展的类位于:
-        
-        - `embykeeper.telechecker.bots`
-        - `embykeeper.telechecker.monitor`
-        - `embykeeper.telechecker.messager`
-        
-        通常来说, 增加一个机器人的签到非常简单, 您需要在 `bots` 中增加一个文件 `dummy.py`:
-        
-        ```python
-        from .base import BotCheckin
-        
-        class DummyCheckin(BotCheckin):
-            name = "Dummy"
-            bot_username = "dummy"
-            bot_captcha_len = 4
-        ```
-        
-        您即增加一个名为 "`Dummy`" 的签到器，将会向用户名为 "`dummy`" 的机器人发送 "`/checkin`" 并等候一个 4 位的验证码，识别验证码后将发送.
-        
-        若您希望识别验证码后点击按钮, 您可以使用 `AnswerBotCheckin`, 您也可以重写 `on_captcha` 函数来实现自定义功能:
-        
-        ```python
-        from .base import AnswerBotCheckin
-        
-        class DummyCheckin(AnswerBotCheckin):
-            ....
-            async def on_captcha(self, message: Message, captcha: str):
-                for l in captcha:
-                    try:
-                        await self.message.click(l)
-                    except ValueError:
-                        self.log.info(f'未能找到对应 "{l}" 的按键, 正在重试.')
-                        await self.retry()
-                        break
-        ```
-        
-        上述代码实现每次按对应一个字符按键的功能.
-        
-        当您实现一个新的签到器时, 欢迎您提出 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 以帮助更多人使用!
-        
 Keywords: emby,telegram,checkin,automator
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7,<3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
+
+<p align="center">
+  <a href='https://github.com/embykeeper/embykeeper'>
+    <img src="https://github.com/embykeeper/embykeeper/blob/main/images/logo.svg" alt="Embykeeper" />
+  </a>
+</p>
+<p align="center">
+    <b>自动签到 定时保号 按需水群</b>
+</p>
+
+---
+
+Embykeeper 是一个在中文社群规则下用于 Emby 影视服务器的签到和保号的自动执行工具, 基于 Pyrogram 编写并具有可拓展性.
+
+## 声明
+
+本项目涉及的一切 Emby 服务器与 Embykeeper 开发团队无关, 在使用 Embykeeper 时造成的一切损失 (包括但不限于 Emby 或 Telegram 账号被封禁或被群封禁) 与开发团队无关. 
+
+本项目设计初衷是在中文 Emby 社群规则下, 保号要求逐渐苛刻 (部分要求每月登录或每日签到), 这使得休闲时间紧张的人士难以安心使用. 本项目仅旨在帮助该类人群保号, 不鼓励持有大量 Emby 账号而不使用, 导致真正需要的人、为中文影视资源分享和翻译有贡献的人难以获得账号的行为, 开发团队也呼吁仅保留 1-2 个较全面质量较高的 Emby 服务器. 本项目仅提供工具, 具体使用形式及造成的影响和后果与开发团队无关. 
+
+本项目欢迎友善讨论与建议, 您可以通过 [Github Issue](https://github.com/embykeeper/embykeeper) 途径反馈, 并认可开发团队可以关闭与项目开发不直接相关的不友善讨论. 您也可以通过 [Telegram 讨论组](https://t.me/embykeeper_chat) 与开发团队进行交流.
+
+当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题. 
+
+当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装. 
+
+## 功能
+
+- Telegram 机器人签到
+  - 支持群组
+    - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
+    - 卷毛鼠: [频道]() [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
+    - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
+    - BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)
+    - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
+    - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
+    - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
+    - Pornemby (_测试中_): [频道](https://t.me/pornembyservice) [机器人](https://t.me/PronembyTGBot2_bot)
+    - 其他非 Emby 相关:
+      - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加) (_测试中_)
+    - 默认禁用:
+      - Pornemby 科举考试 (_测试中_): [活动频道](https://t.me/PornembyFun)
+      - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
+      - ~~垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)~~ (无响应)
+  - 特性
+    - 验证码识别与自动重试
+    - 多账户签到
+    - 网页类型签到
+- Emby 保活
+  - 定时模拟账号登录视频播放
+  - 播放时间与进度模拟
+- Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
+  - NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)
+- Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
+  - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
+  - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
+
+## 安装与使用
+
+### 从 Docker 安装
+
+Embykeeper 可以通过 `docker` 运行, 您需[安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
+
+```bash
+touch config.toml
+docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
+```
+
+命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+
+```toml
+[proxy]
+hostname = "127.0.0.1"
+port = "1080"
+scheme = "socks5"
+
+[[telegram]]
+api_id = "27894236"
+api_hash = "622159182fdd4b15b627eeb3ac695271"
+phone = "+8612109347899"
+
+[[emby]]
+url = "https://weiss-griffin.com/"
+username = "carrie19"
+password = "s*D7MMCpS$"
+```
+
+对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要更换应用名称/短名称/代理/清除浏览器记录并重试.
+
+随后, 您需要再次执行:
+
+```bash
+docker run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper
+```
+
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+
+```bash
+docker run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper
+```
+
+或者使用 [docker-compose](https://docs.docker.com/compose/) ([watchtower](https://github.com/containrrr/watchtower) 被用于自动更新容器服务):
+
+```yaml
+version: '3'
+services:
+  embykeeper:
+    container_name: embykeeper
+    image: cembykeeper/embykeeper
+    restart: unless-stopped
+    volumes:
+      - ./config.toml:/app/config.toml
+  watchtower:
+    container_name: watchtower
+    image: containrrr/watchtower
+    restart: unless-stopped
+    volumes:
+      - /var/run/docker.sock:/var/run/docker.sock:rw
+```
+
+即可在后台启动 embykeeper.
+
+您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
+
+如果您需要使用主机上的代理服务器 (例如 `https://localhost:1080`), 您可能需要使用 `--net=host` 参数以使用主机网络模式.
+
+### 从 Pypi 安装
+
+Embykeeper 需要 Python 环境以运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
+
+您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7, < 3.11`):
+
+```bash
+pip install embykeeper
+```
+
+随后, 您需要执行:
+
+```bash
+embykeeper
+```
+
+命令将会在当前目录生成模板 `config.toml` 文件, 您需要修改您的账号配置 (详见[从 Docker 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E%20Docker%20%E5%AE%89%E8%A3%85)).
+
+随后, 您需要再次执行:
+
+```bash
+embykeeper
+```
+
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
+
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+
+```bash
+tmux
+```
+
+这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端. 
+
+您随时可以通过运行:
+
+```bash
+tmux a
+```
+
+以重新连接到 `tmux` 终端.
+
+当版本更新时, 您需要执行:
+
+```
+pip install -U embykeeper
+```
+
+然后重新运行应用.
+
+### 从源码构建
+
+首先拉取 Github 并安装:
+
+```bash
+git clone https://github.com/embykeeper/embykeeper.git
+cd embykeeper
+make develop
+```
+
+然后即可执行 Embykeeper:
+
+```bash
+embykeeper
+```
+
+详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E%20Pypi%20%E5%AE%89%E8%A3%85).
+
+当版本更新时, 您需要执行:
+
+```
+git pull
+```
+
+然后重新运行应用.
+
+## 命令行帮助
+
+您可以通过运行 `embykeeper -h` 以获取帮助:
+
+```bash
+$ embykeeper -h
+
+欢迎使用 Embykeeper. 🎦 无参数默认开启全部功能.
+
+参数:
+    config  配置文件 (置空以生成)
+模块开关:
+    --checkin     -c   启用每日指定时间签到 (不指定值时默认为6:00PM)
+    --emby        -e   启用每隔天数Emby自动保活 (不指定值时默认为每7天)
+    --monitor     -m   启用群聊监视
+    --send        -s   启用自动水群
+调试参数:
+    --no-instant  -I   不立刻执行一次计划任务
+    --debug       -d   开启调试模式, 错误将会导致程序停止运行
+    --version     -v   打印 Embykeeper 版本
+    --follow      -f   仅启动消息调试
+    --analyze     -a   仅启动历史信息分析
+```
+
+例如:
+
+```bash
+# 仅启动每日签到
+$ embykeeper config.toml -c
+
+# 仅启动每日 8:00 PM 签到
+$ embykeeper config.toml -c 8:00PM
+
+# 启动所有功能, 同时调整签到时间为 8:00 AM, 调整保活间隔天数为 14
+$ embykeeper config.toml -c 8:00PM -e 14 -m -s
+```
+
+您也可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
+
+```bash
+# 启动历史信息分析
+$ embykeeper config.toml -a
+
+请输入群组用户名 (以空格分隔): https://t.me/XXX YYY 10253512
+请输入关键词 (以空格分隔):
+输入时间范围 (以"-"分割): 8:00AM-10:00AM
+请输入各群组最大获取数量 [1000]:
+```
+
+该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
+
+另一个工具是即时信息分析:
+
+![follow screenshot](images/follow.svg)
+
+该工具可以实时输出消息的 ID 等信息, 以方便调试.
+
+## 消息推送与高级用户
+
+您可以通过设置项 "`notifier`" 设置 成功/失败 通知将被发送的 Telegram 账号, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot) 设置消息每日发送的时间.
+
+本项目涉及的需要 Cloudflare 验证码付费跳过的操作 (例如 Nebula 签到)、可能会引起竞争的操作 (例如自动抢邀请码)将需要高级用户, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) 成为高级用户.
+
+目前有三种方式成为高级用户:
+
+1. 分享 1 个邀请制 Emby 的邀请码;
+2. 为本项目提供 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 并被合并;
+3. 通过爱发电赞助一个[小包子](https://afdian.net/a/jackzzs);
+
+## 支持 Embykeeper
+
+##### 开发者团队
+
+- [jackzzs](https://github.com/jackzzs)
+
+##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
+
+![kitty](images/kitty.gif)
+
+## 配置项
+
+| 设置项       | 值类型             | 简介                                         | 默认值  |
+| ------------ | ------------------ | -------------------------------------------- | ------- |
+| `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
+| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `10`    |
+| `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
+| `random`     | `int`              | Telegram 机器人签到定时任务时间随机量 (分钟) | `15`    |
+| `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
+| `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
+| `proxy`      | `dict`             | 代理设置                                     | `{}`    |
+| `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
+| `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
+
+`service`设置可以为:
+
+| 设置项      | 值类型 | 简介           | 默认值               |
+| ----------- | ------ | -------------- | -------------------- |
+| `checkiner` | `list` | 启用的签到站点 | (当前所有支持的站点) |
+| `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
+| `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
+
+注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
+若您需要禁用部分签到站点, 您可以在列表中删除对应的名称.
+若您需要使用默认禁用的签到站点, 您可以在列表中增加对应的名称.
+当前支持的名称包括:
+| 站点 | 名称 | | 站点 | 名称 |
+| --- | --- | --- |--- | --- |
+| 垃圾影音 | `ljyy` | | 搜书神器 | `sosdbot` |
+| 卷毛鼠 IPTV | `jms_iptv` | | 终点站 | `terminus` |
+| Pornemby | `pornemby` | | Singularity | `singularity` |
+| Peach | `peach` | | Nebula | `nebula` |
+| Bluesea | `bluesea` | | Embyhub | `embyhub` |
+| 卷毛鼠 | `jms` | | | |
+
+`proxy` 设置可以为:
+
+| 设置项     | 值类型 | 简介                                    | 默认值      |
+| ---------- | ------ | --------------------------------------- | ----------- |
+| `hostname` | `str`  | 代理服务器地址                          | `localhost` |
+| `port`     | `int`  | 代理端口号                              | `1080`      |
+| `scheme`   | `str`  | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
+
+`telegram` 设置可以为:
+
+| 设置项     | 值类型 | 简介                                                               | 默认值  |
+| ---------- | ------ | ------------------------------------------------------------------ | ------- |
+| `api_id`   | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
+| `api_hash` | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
+| `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                      |         |
+| `monitor`  | `bool` | 启用群组监控系列功能                                               | `false` |
+| `send`     | `bool` | 启用自动水群系列功能                                               | `false` |
+
+`emby` 设置可以为:
+
+| 设置项     | 值类型 | 简介                                                      | 默认值 |
+| ---------- | ------ | --------------------------------------------------------- | ------ |
+| `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
+| `username` | `str`  | Emby 服务器用户名                                         |        |
+| `password` | `str`  | Emby 服务器密码                                           |        |
+| `time`     | `int`  | 模拟观看的时间 (秒)                                       | `800`  |
+| `progress` | `int`  | 观看后模拟进度条保存的时间 (秒)                           | `1000` |
+
+## 代码重用与开发
+
+代码架构如下:
+
+```mermaid
+flowchart TD
+    A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
+    A --> C(fa:fa-play embywatcher)
+    B --checker--> E[fa:fa-robot Bot]
+    B --monitor--> G[fa:fa-eye Monitor]
+    B --messager--> F[fa:fa-message Messager]
+    C --watcher--> H[fa:fa-circle-play EmbyWatcher]
+    F ---- |schedule| A
+```
+
+主要可以扩展的类位于:
+
+- `embykeeper.telechecker.bots`
+- `embykeeper.telechecker.monitor`
+- `embykeeper.telechecker.messager`
+
+通常来说, 增加一个机器人的签到非常简单, 您需要在 `bots` 中增加一个文件 `dummy.py`:
+
+```python
+from .base import BotCheckin
+
+class DummyCheckin(BotCheckin):
+    name = "Dummy"
+    bot_username = "dummy"
+    bot_captcha_len = 4
+```
+
+您即增加一个名为 "`Dummy`" 的签到器, 将会向用户名为 "`dummy`" 的机器人发送 "`/checkin`" 并等候一个 4 位的验证码, 识别验证码后将发送.
+
+若您希望识别验证码后点击按钮, 您可以使用 `AnswerBotCheckin`, 您也可以重写 `on_captcha` 函数来实现自定义功能:
+
+```python
+from .base import AnswerBotCheckin
+
+class DummyCheckin(AnswerBotCheckin):
+    ....
+    async def on_captcha(self, message: Message, captcha: str):
+        for l in captcha:
+            try:
+                await self.message.click(l)
+            except ValueError:
+                self.log.info(f'未能找到对应 "{l}" 的按键, 正在重试.')
+                await self.retry()
+                break
+```
+
+上述代码实现每次按对应一个字符按键的功能.
+
+当您实现一个新的签到器时, 欢迎您提出 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 以帮助更多人使用!
```

#### html2text {}

```diff
@@ -1,103 +1,151 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.0.7 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.0.8 Summary: Daily checkin
 automator for emby bots in telegram. Home-page: https://github.com/embykeeper/
-embykeeper Author: jackzzs Author-email: jackzzs@outlook.com License: UNKNOWN
-Description: [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://
-pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/
-dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
+embykeeper Author: jackzzs Author-email: jackzzs@outlook.com Keywords:
+emby,telegram,checkin,automator Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
+Desktop Classifier: Natural Language :: Chinese (Simplified) Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Requires-Python: >=3.7,<3.11 Description-
+Content-Type: text/markdown License-File: LICENSE [![pypi badge](https://
+img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [!
+[downloads badge](https://img.shields.io/pypi/dm/
+embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
 pypi.org/project/embykeeper/) [![python versions badge](https://img.shields.io/
 pypi/pyversions/embykeeper)](https://pypi.org/project/embykeeper/) [![license
 badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://
 github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://
 img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [!
 [telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://
 t.me/embykeeper)
                                  [Embykeeper]
                     èªå¨ç­¾å° å®æ¶ä¿å· æéæ°´ç¾¤
 --- Embykeeper æ¯ä¸ä¸ªå¨ä¸­æç¤¾ç¾¤è§åä¸ç¨äº Emby
 å½±è§æå¡å¨çç­¾å°åä¿å·çèªå¨æ§è¡å·¥å·, åºäº Pyrogram
-ç¼åå¹¶å·æå¯æå±æ§ã ## å£°æ æ¬é¡¹ç®æ¶åçä¸å Emby
-æå¡å¨ä¸ Embykeeper å¼åå¢éæ å³ï¼å¨ä½¿ç¨ Embykeeper
-æ¶é æçä¸åæå¤±ï¼åæ¬ä½ä¸éäº Emby æ Telegram
-è´¦å·è¢«å°ç¦æè¢«ç¾¤å°ç¦ï¼ä¸å¼åå¢éæ å³ã
-æ¬é¡¹ç®è®¾è®¡åè¡·æ¯å¨ä¸­æ Emby
-ç¤¾ç¾¤è§åä¸ï¼ä¿å·è¦æ±éæ¸èå»ï¼é¨åè¦æ±æ¯æç»å½ææ¯æ¥ç­¾å°ï¼ï¼è¿ä½¿å¾ä¼é²æ¶é´ç´§å¼ çäººå£«é¾ä»¥å®å¿ä½¿ç¨ãæ¬é¡¹ç®ä»æ¨å¨å¸®å©è¯¥ç±»äººç¾¤ä¿å·ï¼ä¸é¼å±ææå¤§é
-Emby
-è´¦å·èä¸ä½¿ç¨ï¼å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸ºï¼å¼åå¢éä¹å¼åä»ä¿ç
-1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby
-æå¡å¨ãæ¬é¡¹ç®ä»æä¾å·¥å·ï¼å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³ã
+ç¼åå¹¶å·æå¯æå±æ§. ## å£°æ æ¬é¡¹ç®æ¶åçä¸å Emby
+æå¡å¨ä¸ Embykeeper å¼åå¢éæ å³, å¨ä½¿ç¨ Embykeeper
+æ¶é æçä¸åæå¤± (åæ¬ä½ä¸éäº Emby æ Telegram
+è´¦å·è¢«å°ç¦æè¢«ç¾¤å°ç¦) ä¸å¼åå¢éæ å³.
+æ¬é¡¹ç®è®¾è®¡åè¡·æ¯å¨ä¸­æ Emby ç¤¾ç¾¤è§åä¸,
+ä¿å·è¦æ±éæ¸èå» (é¨åè¦æ±æ¯æç»å½ææ¯æ¥ç­¾å°),
+è¿ä½¿å¾ä¼é²æ¶é´ç´§å¼ çäººå£«é¾ä»¥å®å¿ä½¿ç¨.
+æ¬é¡¹ç®ä»æ¨å¨å¸®å©è¯¥ç±»äººç¾¤ä¿å·, ä¸é¼å±ææå¤§é Emby
+è´¦å·èä¸ä½¿ç¨,
+å¯¼è´çæ­£éè¦çäººãä¸ºä¸­æå½±è§èµæºåäº«åç¿»è¯æè´¡ç®çäººé¾ä»¥è·å¾è´¦å·çè¡ä¸º,
+å¼åå¢éä¹å¼åä»ä¿ç 1-2 ä¸ªè¾å¨é¢è´¨éè¾é«ç Emby æå¡å¨.
+æ¬é¡¹ç®ä»æä¾å·¥å·,
+å·ä½ä½¿ç¨å½¢å¼åé æçå½±åååæä¸å¼åå¢éæ å³.
 æ¬é¡¹ç®æ¬¢è¿ååè®¨è®ºä¸å»ºè®®, æ¨å¯ä»¥éè¿ [Github Issue](https://
 github.com/embykeeper/embykeeper) éå¾åé¦,
-å¹¶è®¤å¯å¼åå¢éå¯ä»¥å é¤æå³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®ºã
-å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½ï¼è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
-Bot](https://t.me/embykeeper_bot)" åéå³é®çæå/
-å¤±è´¥æ¥å¿ä»¥ä¾åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
-æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢ã
-å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·ï¼é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æï¼å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£ã
-## åè½ - Telegram æºå¨äººç­¾å° - æ¯æç¾¤ç» - ç»ç¹ç«: [é¢é]
-(https://t.me/embypub) [ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://
-t.me/EmbyPublicBot) - å·æ¯é¼ : [é¢é]() [ç¾¤ç»](https://t.me/Curly_Mouse)
-[æºå¨äºº](https://t.me/jmsembybot) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/
-CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://
-t.me/JMSIPTV_bot)~~ (æ ååº) - Peach: [é¢é](https://t.me/
-peach_emby_channel) [ç¾¤ç»](https://t.me/peach_emby_chat) [æºå¨äºº](https://
-t.me/peach_emby_bot) - åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1)
-[æºå¨äºº](https://t.me/zckllflbot) - BlueSea: [ç¾¤ç»](https://t.me/
-blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot) - EmbyHub: [é¢é]
-(https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
-t.me/EdHubot) - Singularity: [é¢é](https://t.me/Singularity_Emby_Channel)
-[ç¾¤ç»](https://t.me/Singularity_Emby_Group) [æºå¨äºº](https://t.me/
-Singularity_Emby_Bot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»]
-(https://t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
+å¹¶è®¤å¯å¼åå¢éå¯ä»¥å³é­ä¸é¡¹ç®å¼åä¸ç´æ¥ç¸å³çä¸ååè®¨è®º.
+æ¨ä¹å¯ä»¥éè¿ [Telegram è®¨è®ºç»](https://t.me/embykeeper_chat)
+ä¸å¼åå¢éè¿è¡äº¤æµ. å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½,
+è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper Auth Bot](https://t.me/
+embykeeper_auth_bot)" åéå³é®çæå/å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper
+Bot](https://t.me/embykeeper_bot)" åæ¨æ¨é,
+æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
+æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
+å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
+å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
+æºå¨äººç­¾å° - æ¯æç¾¤ç» - ç»ç¹ç«: [é¢é](https://t.me/embypub)
+[ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://t.me/EmbyPublicBot) -
+å·æ¯é¼ : [é¢é]() [ç¾¤ç»](https://t.me/Curly_Mouse) [æºå¨äºº](https://
+t.me/jmsembybot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»](https://
+t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
 (ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
-t.me/embykeeper_bot?start=__prime)) - é«çº§ç¹æ§ -
-éªè¯ç è¯å«ä¸èªå¨éè¯ - å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby
+t.me/embykeeper_bot?start=__prime)) - BlueSea: [ç¾¤ç»](https://t.me/
+blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot) - Singularity: [é¢é]
+(https://t.me/Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/
+Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach:
+[é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
+peach_emby_chat) [æºå¨äºº](https://t.me/peach_emby_bot) - EmbyHub: [é¢é]
+(https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
+t.me/EdHubot) - Pornemby (_æµè¯ä¸­_): [é¢é](https://t.me/pornembyservice)
+[æºå¨äºº](https://t.me/PronembyTGBot2_bot) - å¶ä»é Emby ç¸å³: -
+æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/pull/8)
+å¢å ) (_æµè¯ä¸­_) - é»è®¤ç¦ç¨: - Pornemby ç§ä¸¾èè¯ (_æµè¯ä¸­_):
+[æ´»å¨é¢é](https://t.me/PornembyFun) - ~~å·æ¯é¼  IPTV: [é¢é](https://
+t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https:/
+/t.me/JMSIPTV_bot)~~ (æ ååº) - ~~åå¾å½±é³: [ç¾¤ç»](https://t.me/
++3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://t.me/zckllflbot)~~ (æ ååº) - ç¹æ§
+- éªè¯ç è¯å«ä¸èªå¨éè¯ - å¤è´¦æ·ç­¾å° - ç½é¡µç±»åç­¾å° - Emby
 ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
-Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, è¯·è°¨æä½¿ç¨) -
-NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://t.me/NakoNetwork) [æºå¨äºº](https://
-t.me/nakonetwork_bot) - Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·]
-(https://t.me/embykeeper_bot?start=__prime)) - ä¸ç»ç æ¢éè¯·ç : [ç¾¤ç»]
-(https://t.me/Ephemeralemby) [æºå¨äºº](https://t.me/UnknownEmbyBot) - Embyhub
-å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
-emby_hub) [æºå¨äºº](https://t.me/EdHubot) ## å®è£ä¸ä½¿ç¨ Embykeeper
-éè¦ Python ç¯å¢ä»¥è¿è¡, æ¨å¯ä»¥éè¿ [conda](https://github.com/
-conda/conda) æ [virtualvenv](https://virtualenv.pypa.io/
-) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip` å®è£ `embykeeper`
-(éè¦ `python >= 3.7`): ```bash pip install embykeeper ```
-æèæ¨ä¹å¯ä»¥éè¿æºç æå»º: ```bash git clone https://github.com/
-embykeeper/embykeeper.git cd embykeeper make develop ```
-éåï¼æ¨éè¦æ§è¡: ```bash embykeeper ```
-å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml`
-æä»¶ï¼æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ,
-ä»ååè): ```toml [proxy] hostname = "127.0.0.1" port = "1080" scheme =
-"socks5" [[telegram]] api_id = "27894236" api_hash =
-"622159182fdd4b15b627eeb3ac695271" phone = "+8612109347899" [[emby]] url =
-"https://weiss-griffin.com/" username = "carrie19" password = "s*D7MMCpS$" ```
-å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿ [Telegram å®ç½](https://
-my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© API
-development tools, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
-æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
-æ¨å¯è½éè¦æ´æ¢åºç¨åç§°/ç­åç§°/ä»£ç/
-æ¸é¤æµè§å¨è®°å½å¹¶éè¯. ç¶å, è¿è¡: ```bash embykeeper config.toml
-``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½ï¼ç»å½æååï¼Embykeeper
+Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+è¯·è°¨æä½¿ç¨) - NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://t.me/NakoNetwork)
+[æºå¨äºº](https://t.me/nakonetwork_bot) - Telegram èªå¨çæ§ä¿¡æ¯ (éè¦
+[è¶çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) - ä¸ç»ç
+æ¢éè¯·ç : [ç¾¤ç»](https://t.me/Ephemeralemby) [æºå¨äºº](https://t.me/
+UnknownEmbyBot) - Embyhub å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub)
+[ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) ##
+å®è£ä¸ä½¿ç¨ ### ä» Docker å®è£ Embykeeper å¯ä»¥éè¿ `docker` è¿è¡,
+æ¨é[å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
+ç¶åæ§è¡: ```bash touch config.toml docker run -v $(pwd)/config.toml:/app/
+config.toml --rm -it embykeeper/embykeeper ```
+å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
+```toml [proxy] hostname = "127.0.0.1" port = "1080" scheme = "socks5" [
+[telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
+phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+"carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
+[Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
+ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
+è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
+"Error", æ¨å¯è½éè¦æ´æ¢åºç¨åç§°/ç­åç§°/ä»£ç/
+æ¸é¤æµè§å¨è®°å½å¹¶éè¯. éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
+run -v $(pwd)/config.toml:/app/config.toml --rm -it embykeeper/embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥è¿è¡: ```bash tmux ``` è¿å°å¯å¨ä¸ä¸ª `tmux`
-ç»ç«¯ï¼æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`),
-å¹¶æ Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯ã
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash docker
+run -d -v $(pwd)/config.toml:/app/config.toml embykeeper/embykeeper ```
+æèä½¿ç¨ [docker-compose](https://docs.docker.com/compose/) ([watchtower]
+(https://github.com/containrrr/watchtower) è¢«ç¨äºèªå¨æ´æ°å®¹å¨æå¡):
+```yaml version: '3' services: embykeeper: container_name: embykeeper image:
+cembykeeper/embykeeper restart: unless-stopped volumes: - ./config.toml:/app/
+config.toml watchtower: container_name: watchtower image: containrrr/watchtower
+restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/docker.sock:rw
+``` å³å¯å¨åå°å¯å¨ embykeeper. æ¨å¯ä»¥éè¿ `docker logs -
+f embykeeper` æ `docker-compose logs -f embykeeper` ä»¥æ¥çææ°æ¥å¿.
+å¦ææ¨éè¦ä½¿ç¨ä¸»æºä¸çä»£çæå¡å¨ (ä¾å¦ `https://localhost:
+1080`), æ¨å¯è½éè¦ä½¿ç¨ `--net=host` åæ°ä»¥ä½¿ç¨ä¸»æºç½ç»æ¨¡å¼.
+### ä» Pypi å®è£ Embykeeper éè¦ Python ç¯å¢ä»¥è¿è¡, æ¨å¯ä»¥éè¿
+[conda](https://github.com/conda/conda) æ [virtualvenv](https://
+virtualenv.pypa.io/) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip`
+å®è£ `embykeeper` (éè¦ `python >= 3.7, < 3.11`): ```bash pip install
+embykeeper ``` éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
+å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦ä¿®æ¹æ¨çè´¦å·éç½® (è¯¦è§[ä» Docker å®è£](https://
+github.com/embykeeper/embykeeper#%E4%BB%8E%20Docker%20%E5%AE%89%E8%A3%85)).
+éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
+æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
+Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
 æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
-ç»ç«¯. ## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h`
-ä»¥è·åå¸®å©: ```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦
-æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
-(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å°
-(ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´»
-(ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --monitor -m å¯ç¨ç¾¤èçè§ --send -
-s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-instant -
-I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
+ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
+ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæå Github å¹¶å®è£:
+```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
+make develop ``` ç¶åå³å¯æ§è¡ Embykeeper: ```bash embykeeper ```
+è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£](https://github.com/embykeeper/
+embykeeper#%E4%BB%8E%20Pypi%20%E5%AE%89%E8%A3%85). å½çæ¬æ´æ°æ¶,
+æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å©
+æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -
+h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°:
+config éç½®æä»¶ (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -
+c å¯ç¨æ¯æ¥æå®æ¶é´ç­¾å° (ä¸æå®å¼æ¶é»è®¤ä¸º6:00PM) --emby -
+e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
+monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
+instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --debug -d å¼å¯è°è¯æ¨¡å¼,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
 follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ ```
 ä¾å¦: ```bash # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
 å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
 è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -
 s ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
@@ -109,17 +157,18 @@
 ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
 å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
 è¯¥å·¥å·å¯ä»¥å®æ¶è¾åºæ¶æ¯ç ID ç­ä¿¡æ¯, ä»¥æ¹ä¾¿è°è¯. ##
 æ¶æ¯æ¨éä¸é«çº§ç¨æ· æ¨å¯ä»¥éè¿è®¾ç½®é¡¹ "`notifier`" è®¾ç½®
 æå/å¤±è´¥ éç¥å°è¢«åéç Telegram è´¦å·, æ¨å¯ä»¥éè¿
 [Embykeeper Bot](https://t.me/embykeeper_bot)
 è®¾ç½®æ¶æ¯æ¯æ¥åéçæ¶é´. æ¬é¡¹ç®æ¶åçéè¦ Cloudflare
-éªè¯ç ä»è´¹è·³è¿çæä½ï¼ä¾å¦ Nebula
-ç­¾å°ï¼ãå¯è½ä¼å¼èµ·ç«äºçæä½ï¼ä¾å¦èªå¨æ¢éè¯·ç ï¼å°éè¦é«çº§ç¨æ·ï¼æ¨å¯ä»¥éè¿
-[Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
+éªè¯ç ä»è´¹è·³è¿çæä½ (ä¾å¦ Nebula
+ç­¾å°)ãå¯è½ä¼å¼èµ·ç«äºçæä½
+(ä¾å¦èªå¨æ¢éè¯·ç )å°éè¦é«çº§ç¨æ·, æ¨å¯ä»¥éè¿ [Embykeeper
+Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
 ç®åæä¸ç§æ¹å¼æä¸ºé«çº§ç¨æ·: 1. åäº« 1 ä¸ªéè¯·å¶ Emby
 çéè¯·ç ; 2. ä¸ºæ¬é¡¹ç®æä¾ [Pull Requests](https://github.com/
 embykeeper/embykeeper/pulls) å¹¶è¢«åå¹¶; 3. éè¿ç±åçµèµå©ä¸ä¸ª
 [å°åå­](https://afdian.net/a/jackzzs); ## æ¯æ Embykeeper #####
 å¼åèå¢é - [jackzzs](https://github.com/jackzzs) ##### éè¿[ç±åçµ]
 (https://afdian.net/a/jackzzs)èµå© ![kitty](images/kitty.gif) ## éç½®é¡¹ |
 è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ------------ | -----------------
@@ -134,56 +183,56 @@
 Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | | `emby` | `list` | Emby
 è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | `service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
 å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------- | ------ | -------------- | ----
 ---------------- | | `checkiner` | `list` | å¯ç¨çç­¾å°ç«ç¹ |
 (å½åæææ¯æçç«ç¹) | | `monitor` | `list` | å¯ç¨ççè§ä¼è¯ |
 (å½åæææ¯æçä¼è¯) | | `messager` | `list` | å¯ç¨çæ°´ç¾¤ä¼è¯ |
 (å½åæææ¯æçä¼è¯) | æ³¨æ, å½æ¨æªæ¾ä¸ç«ç¹æºå¨äººå¯¹è¯,
-è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡. `proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
-å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
------------------ | ----------- | | `hostname` | `str` | ä»£çæå¡å¨å°å
-| `localhost` | | `port` | `int` | ä»£çç«¯å£å· | `1080` | | `scheme` |
-`str` | ä»£çåè®®, å¯ä»¥ä¸º "`socks5`" æ "`http`" | `socks5` | `telegram`
+è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡. è¥æ¨éè¦ç¦ç¨é¨åç­¾å°ç«ç¹,
+æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
+è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
+æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
+ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | --- | --- | --- |--- | --- | |
+åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` | | å·æ¯é¼  IPTV |
+`jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby | `pornemby` | | Singularity
+| `singularity` | | Peach | `peach` | | Nebula | `nebula` | | Bluesea |
+`bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms` | | | | `proxy`
 è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
------- | ------------------------------------------------------------------ | -
------- | | `api_id` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/
-)ç³è¯·ç Application ID | | | `api_hash` | `str` | ä»[Telegram å®ç½]
-(https://my.telegram.org/)ç³è¯·ç Application Hash | | | `phone` | `str` |
-è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | | `monitor` | `bool` |
-å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` | `bool` |
-å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹
-| å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | --------------------
-------------------------------------- | ------ | | `url` | `str` | Emby
-æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | | `username`
-| `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
+------ | --------------------------------------- | ----------- | | `hostname` |
+`str` | ä»£çæå¡å¨å°å | `localhost` | | `port` | `int` |
+ä»£çç«¯å£å· | `1080` | | `scheme` | `str` | ä»£çåè®®, å¯ä»¥ä¸º
+"`socks5`" æ "`http`" | `socks5` | `telegram` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
+å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
+-------------------------------------------- | ------- | | `api_id` | `str` |
+ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID | | |
+`api_hash` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç
+Application Hash | | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`"
+| | | `monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send`
+| `bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: |
+è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------
+----------------------------------------------- | ------ | | `url` | `str` |
+Emby æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | |
+`username` | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
 æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
 `progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
 ## ä»£ç éç¨ä¸å¼å ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-
 terminal cli) --> B(fa:fa-telegram telechecker) A --> C(fa:fa-play embywatcher)
 B --checker--> E[fa:fa-robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --
 messager--> F[fa:fa-message Messager] C --watcher--> H[fa:fa-circle-play
 EmbyWatcher] F ---- |schedule| A ``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: -
 `embykeeper.telechecker.bots` - `embykeeper.telechecker.monitor` -
 `embykeeper.telechecker.messager` éå¸¸æ¥è¯´,
 å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
 ä¸­å¢å ä¸ä¸ªæä»¶ `dummy.py`: ```python from .base import BotCheckin class
 DummyCheckin(BotCheckin): name = "Dummy" bot_username = "dummy" bot_captcha_len
-= 4 ``` æ¨å³å¢å ä¸ä¸ªåä¸º "`Dummy`" çç­¾å°å¨ï¼å°ä¼åç¨æ·åä¸º
-"`dummy`" çæºå¨äººåé "`/checkin`" å¹¶ç­åä¸ä¸ª 4
-ä½çéªè¯ç ï¼è¯å«éªè¯ç åå°åé.
-è¥æ¨å¸æè¯å«éªè¯ç åç¹å»æé®, æ¨å¯ä»¥ä½¿ç¨ `AnswerBotCheckin`,
-æ¨ä¹å¯ä»¥éå `on_captcha` å½æ°æ¥å®ç°èªå®ä¹åè½: ```python from
-.base import AnswerBotCheckin class DummyCheckin(AnswerBotCheckin): .... async
-def on_captcha(self, message: Message, captcha: str): for l in captcha: try:
-await self.message.click(l) except ValueError: self.log.info
-(f'æªè½æ¾å°å¯¹åº "{l}" çæé®, æ­£å¨éè¯.') await self.retry() break
-``` ä¸è¿°ä»£ç å®ç°æ¯æ¬¡æå¯¹åºä¸ä¸ªå­ç¬¦æé®çåè½.
+= 4 ``` æ¨å³å¢å ä¸ä¸ªåä¸º "`Dummy`" çç­¾å°å¨, å°ä¼åç¨æ·åä¸º
+"`dummy`" çæºå¨äººåé "`/checkin`" å¹¶ç­åä¸ä¸ª 4 ä½çéªè¯ç ,
+è¯å«éªè¯ç åå°åé. è¥æ¨å¸æè¯å«éªè¯ç åç¹å»æé®,
+æ¨å¯ä»¥ä½¿ç¨ `AnswerBotCheckin`, æ¨ä¹å¯ä»¥éå `on_captcha`
+å½æ°æ¥å®ç°èªå®ä¹åè½: ```python from .base import AnswerBotCheckin
+class DummyCheckin(AnswerBotCheckin): .... async def on_captcha(self, message:
+Message, captcha: str): for l in captcha: try: await self.message.click(l)
+except ValueError: self.log.info(f'æªè½æ¾å°å¯¹åº "{l}" çæé®,
+æ­£å¨éè¯.') await self.retry() break ```
+ä¸è¿°ä»£ç å®ç°æ¯æ¬¡æå¯¹åºä¸ä¸ªå­ç¬¦æé®çåè½.
 å½æ¨å®ç°ä¸ä¸ªæ°çç­¾å°å¨æ¶, æ¬¢è¿æ¨æåº [Pull Requests](https://
-github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨! Keywords:
-emby,telegram,checkin,automator Platform: UNKNOWN Classifier: Development
-Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
-Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
-(Simplified) Classifier: License :: OSI Approved :: GNU General Public License
-v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Requires-
-Python: >=3.7,<3.11 Description-Content-Type: text/markdown
+github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨!
```

### Comparing `embykeeper-2.0.7/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.0.8/embykeeper.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+./requirements.txt
 embykeeper/__init__.py
 embykeeper/cli.py
 embykeeper/log.py
 embykeeper/loop.py
 embykeeper/settings.py
 embykeeper/utils.py
 embykeeper.egg-info/PKG-INFO
@@ -27,19 +29,22 @@
 embykeeper/telechecker/bots/bluesea.py
 embykeeper/telechecker/bots/embyhub.py
 embykeeper/telechecker/bots/jms.py
 embykeeper/telechecker/bots/jms_iptv.py
 embykeeper/telechecker/bots/ljyy.py
 embykeeper/telechecker/bots/nebula.py
 embykeeper/telechecker/bots/peach.py
+embykeeper/telechecker/bots/pornemby.py
 embykeeper/telechecker/bots/singularity.py
+embykeeper/telechecker/bots/sosdbot.py
 embykeeper/telechecker/bots/terminus.py
 embykeeper/telechecker/messager/__init__.py
 embykeeper/telechecker/messager/base.py
 embykeeper/telechecker/messager/common.py
 embykeeper/telechecker/messager/nakonako.py
 embykeeper/telechecker/messager/test.py
 embykeeper/telechecker/monitor/__init__.py
 embykeeper/telechecker/monitor/base.py
 embykeeper/telechecker/monitor/bgk.py
 embykeeper/telechecker/monitor/embyhub.py
+embykeeper/telechecker/monitor/pornemby_exam.py
 embykeeper/telechecker/monitor/test.py
```

### Comparing `embykeeper-2.0.7/setup.py` & `embykeeper-2.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords=["emby", "telegram", "checkin", "automator"],
     name="embykeeper",
     packages=find_packages(include=["embykeeper", "embykeeper.*"]),
     url="https://github.com/embykeeper/embykeeper",
-    version="2.0.7",
+    version="2.0.8",
     zip_safe=False,
 )
```

