# Comparing `tmp/amlopschat-1.0.0.tar.gz` & `tmp/amlopschat-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amlopschat-1.0.0.tar", last modified: Thu Apr 20 13:04:40 2023, max compression
+gzip compressed data, was "amlopschat-1.0.1.tar", last modified: Thu Apr 20 13:14:14 2023, max compression
```

## Comparing `amlopschat-1.0.0.tar` & `amlopschat-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:04:40.850665 amlopschat-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 13:04:01.000000 amlopschat-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 13:04:40.850665 amlopschat-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 13:04:01.000000 amlopschat-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:04:40.846665 amlopschat-1.0.0/amlopschat/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 13:04:29.000000 amlopschat-1.0.0/amlopschat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-20 13:04:29.000000 amlopschat-1.0.0/amlopschat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:04:40.846665 amlopschat-1.0.0/amlopschat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 13:04:40.000000 amlopschat-1.0.0/amlopschat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-20 13:04:40.000000 amlopschat-1.0.0/amlopschat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:04:40.000000 amlopschat-1.0.0/amlopschat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 13:04:40.000000 amlopschat-1.0.0/amlopschat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-20 13:04:40.850665 amlopschat-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 13:04:01.000000 amlopschat-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:04:40.850665 amlopschat-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 13:04:40.850665 amlopschat-1.0.0/src/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-20 13:04:01.000000 amlopschat-1.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:14:14.466442 amlopschat-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 13:13:33.000000 amlopschat-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 13:14:14.466442 amlopschat-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 13:13:33.000000 amlopschat-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:14:14.462442 amlopschat-1.0.1/amlopschat/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:14:14.462442 amlopschat-1.0.1/amlopschat/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:14:14.466442 amlopschat-1.0.1/amlopschat/static/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/RoomHeader.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/RoomMessageWrapper.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/create-room.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/emoji.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/header-chat-menu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45367 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)   424491 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/microphone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   450457 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/no-messages.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/read-message.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/send.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/toggle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/unread-message.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/user.png
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/static/chat/vue.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:14:14.466442 amlopschat-1.0.1/amlopschat/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-20 13:14:01.000000 amlopschat-1.0.1/amlopschat/templates/chat_ui_full.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:14:14.466442 amlopschat-1.0.1/amlopschat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 13:14:14.000000 amlopschat-1.0.1/amlopschat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-20 13:14:14.000000 amlopschat-1.0.1/amlopschat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:14:14.000000 amlopschat-1.0.1/amlopschat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 13:14:14.000000 amlopschat-1.0.1/amlopschat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-20 13:14:14.470442 amlopschat-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 13:13:33.000000 amlopschat-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:14:14.470442 amlopschat-1.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 13:14:14.470442 amlopschat-1.0.1/src/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-20 13:13:33.000000 amlopschat-1.0.1/versioneer.py
```

### Comparing `amlopschat-1.0.0/README.md` & `amlopschat-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.0/amlopschat/_version.py` & `amlopschat-1.0.1/amlopschat/_version.py`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.0/versioneer.py` & `amlopschat-1.0.1/versioneer.py`

 * *Files identical despite different names*

