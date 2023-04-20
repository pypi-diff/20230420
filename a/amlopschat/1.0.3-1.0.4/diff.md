# Comparing `tmp/amlopschat-1.0.3.tar.gz` & `tmp/amlopschat-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amlopschat-1.0.3.tar", last modified: Thu Apr 20 15:10:27 2023, max compression
+gzip compressed data, was "amlopschat-1.0.4.tar", last modified: Thu Apr 20 15:16:12 2023, max compression
```

## Comparing `amlopschat-1.0.3.tar` & `amlopschat-1.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:10:27.689188 amlopschat-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 15:09:42.000000 amlopschat-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 15:10:27.689188 amlopschat-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 15:09:42.000000 amlopschat-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:10:27.685188 amlopschat-1.0.3/amlopschat/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:10:27.685188 amlopschat-1.0.3/amlopschat/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:10:27.689188 amlopschat-1.0.3/amlopschat/static/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/RoomHeader.vue
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/RoomMessageWrapper.vue
--rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/arrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/create-room.svg
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/emoji.svg
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/header-chat-menu.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45367 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/index.css
--rw-r--r--   0 runner    (1001) docker     (123)   424592 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/microphone.svg
--rw-r--r--   0 runner    (1001) docker     (123)   450457 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/no-messages.gif
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/read-message.svg
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/search.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/send.svg
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/toggle.svg
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/unread-message.svg
--rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/user.png
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-20 15:10:10.000000 amlopschat-1.0.3/amlopschat/static/chat/vue.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:10:27.685188 amlopschat-1.0.3/amlopschat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 15:10:27.000000 amlopschat-1.0.3/amlopschat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-20 15:10:27.000000 amlopschat-1.0.3/amlopschat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:10:27.000000 amlopschat-1.0.3/amlopschat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 15:10:27.000000 amlopschat-1.0.3/amlopschat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-20 15:10:27.689188 amlopschat-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 15:09:42.000000 amlopschat-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:10:27.689188 amlopschat-1.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 15:10:27.689188 amlopschat-1.0.3/src/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-20 15:09:42.000000 amlopschat-1.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:12.654114 amlopschat-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 15:15:30.000000 amlopschat-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 15:16:12.654114 amlopschat-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 15:15:30.000000 amlopschat-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:12.650114 amlopschat-1.0.4/amlopschat/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:12.650114 amlopschat-1.0.4/amlopschat/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:12.654114 amlopschat-1.0.4/amlopschat/static/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/RoomHeader.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/RoomMessageWrapper.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/create-room.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/emoji.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/header-chat-menu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45367 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)   424592 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/microphone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   450457 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/no-messages.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/read-message.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/send.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/toggle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/unread-message.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/user.png
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-20 15:15:59.000000 amlopschat-1.0.4/amlopschat/static/chat/vue.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:12.650114 amlopschat-1.0.4/amlopschat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 15:16:12.000000 amlopschat-1.0.4/amlopschat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-20 15:16:12.000000 amlopschat-1.0.4/amlopschat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:16:12.000000 amlopschat-1.0.4/amlopschat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 15:16:12.000000 amlopschat-1.0.4/amlopschat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-20 15:16:12.654114 amlopschat-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 15:15:30.000000 amlopschat-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:16:12.654114 amlopschat-1.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 15:16:12.654114 amlopschat-1.0.4/src/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-20 15:15:30.000000 amlopschat-1.0.4/versioneer.py
```

### Comparing `amlopschat-1.0.3/README.md` & `amlopschat-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/amlopschat/_version.py` & `amlopschat-1.0.4/amlopschat/_version.py`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/amlopschat/static/chat/RoomHeader.vue` & `amlopschat-1.0.4/amlopschat/static/chat/RoomHeader.vue`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/amlopschat/static/chat/RoomMessageWrapper.vue` & `amlopschat-1.0.4/amlopschat/static/chat/RoomMessageWrapper.vue`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/amlopschat/static/chat/_version.py` & `amlopschat-1.0.4/amlopschat/static/chat/_version.py`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/amlopschat/static/chat/emoji.svg` & `amlopschat-1.0.4/amlopschat/static/chat/emoji.svg`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/amlopschat/static/chat/index.css` & `amlopschat-1.0.4/amlopschat/static/chat/index.css`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/amlopschat/static/chat/index.js` & `amlopschat-1.0.4/amlopschat/static/chat/index.js`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/amlopschat/static/chat/link.svg` & `amlopschat-1.0.4/amlopschat/static/chat/link.svg`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/amlopschat/static/chat/microphone.svg` & `amlopschat-1.0.4/amlopschat/static/chat/microphone.svg`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/amlopschat/static/chat/no-messages.gif` & `amlopschat-1.0.4/amlopschat/static/chat/no-messages.gif`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/amlopschat/static/chat/user.png` & `amlopschat-1.0.4/amlopschat/static/chat/user.png`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/amlopschat.egg-info/SOURCES.txt` & `amlopschat-1.0.4/amlopschat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.3/versioneer.py` & `amlopschat-1.0.4/versioneer.py`

 * *Files identical despite different names*

