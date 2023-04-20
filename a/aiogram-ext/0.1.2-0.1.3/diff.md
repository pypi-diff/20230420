# Comparing `tmp/aiogram-ext-0.1.2.tar.gz` & `tmp/aiogram-ext-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.1.2.tar", last modified: Thu Apr 20 17:26:06 2023, max compression
+gzip compressed data, was "aiogram-ext-0.1.3.tar", last modified: Thu Apr 20 17:37:23 2023, max compression
```

## Comparing `aiogram-ext-0.1.2.tar` & `aiogram-ext-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      882 2023-04-16 22:10:48.315246 aiogram-ext-0.1.2/botty/__init__.py
--rw-r--r--   0        0        0      251 2023-04-14 12:15:49.770806 aiogram-ext-0.1.2/botty/bot.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.1.2/botty/buttons.py
--rw-r--r--   0        0        0      264 2023-04-17 23:58:40.002141 aiogram-ext-0.1.2/botty/config.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.1.2/botty/context.py
--rw-r--r--   0        0        0     1665 2023-04-16 22:10:48.295151 aiogram-ext-0.1.2/botty/deps.py
--rw-r--r--   0        0        0     5999 2023-04-20 17:26:03.233411 aiogram-ext-0.1.2/botty/dispatcher.py
--rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.1.2/botty/env.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.1.2/botty/filters.py
--rw-r--r--   0        0        0      399 2023-04-16 19:04:22.106465 aiogram-ext-0.1.2/botty/helpers.py
--rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.1.2/botty/keyboards.py
--rw-r--r--   0        0        0      519 2023-04-15 14:16:45.313035 aiogram-ext-0.1.2/botty/loader.py
--rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.1.2/botty/middlewares/__init__.py
--rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.1.2/botty/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.1.2/botty/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.1.2/botty/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.1.2/botty/middlewares/throttling.py
--rw-r--r--   0        0        0      455 2023-04-20 17:26:03.214367 aiogram-ext-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.1.2/README.md
--rw-r--r--   0        0        0      239 2023-04-16 23:01:01.500707 aiogram-ext-0.1.2/tests/__main__.py
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      971 2023-04-20 17:37:20.083266 aiogram-ext-0.1.3/botty/__init__.py
+-rw-r--r--   0        0        0      251 2023-04-14 12:15:49.770806 aiogram-ext-0.1.3/botty/bot.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.1.3/botty/buttons.py
+-rw-r--r--   0        0        0      264 2023-04-17 23:58:40.002141 aiogram-ext-0.1.3/botty/config.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.1.3/botty/context.py
+-rw-r--r--   0        0        0     1665 2023-04-16 22:10:48.295151 aiogram-ext-0.1.3/botty/deps.py
+-rw-r--r--   0        0        0     5999 2023-04-20 17:26:03.233411 aiogram-ext-0.1.3/botty/dispatcher.py
+-rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.1.3/botty/env.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.1.3/botty/filters.py
+-rw-r--r--   0        0        0      723 2023-04-20 17:37:20.103225 aiogram-ext-0.1.3/botty/helpers.py
+-rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.1.3/botty/keyboards.py
+-rw-r--r--   0        0        0      519 2023-04-15 14:16:45.313035 aiogram-ext-0.1.3/botty/loader.py
+-rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.1.3/botty/middlewares/__init__.py
+-rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.1.3/botty/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.1.3/botty/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.1.3/botty/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.1.3/botty/middlewares/throttling.py
+-rw-r--r--   0        0        0      455 2023-04-20 17:37:20.121378 aiogram-ext-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.1.3/README.md
+-rw-r--r--   0        0        0      239 2023-04-16 23:01:01.500707 aiogram-ext-0.1.3/tests/__main__.py
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.1.3/PKG-INFO
```

### Comparing `aiogram-ext-0.1.2/botty/__init__.py` & `aiogram-ext-0.1.3/botty/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     StatesGroup,
     SkipHandler,
     CancelHandler,
     TelegramAPIError,
 )
 from .dispatcher import Dispatcher
 from .env import env
-from .helpers import reply
+from .helpers import reply, is_group, is_private, is_channel
 from .keyboards import ReplyKeyboard, InlineKeyboard
 from .loader import bot, dp, logger
 
 __all__ = [
     "Dispatcher",
     "ReplyKeyboard",
     "InlineKeyboard",
@@ -39,8 +39,11 @@
     "Query",
     "State",
     "FSMContext",
     "SkipHandler",
     "StatesGroup",
     "CancelHandler",
     "TelegramAPIError",
+    "is_private",
+    "is_group",
+    "is_channel",
 ]
```

### Comparing `aiogram-ext-0.1.2/botty/buttons.py` & `aiogram-ext-0.1.3/botty/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.2/botty/context.py` & `aiogram-ext-0.1.3/botty/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.2/botty/deps.py` & `aiogram-ext-0.1.3/botty/deps.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.2/botty/dispatcher.py` & `aiogram-ext-0.1.3/botty/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.2/botty/env.py` & `aiogram-ext-0.1.3/botty/env.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.2/botty/filters.py` & `aiogram-ext-0.1.3/botty/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.2/botty/keyboards.py` & `aiogram-ext-0.1.3/botty/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.2/botty/loader.py` & `aiogram-ext-0.1.3/botty/loader.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.2/botty/middlewares/_conversation.py` & `aiogram-ext-0.1.3/botty/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.2/botty/middlewares/_membership.py` & `aiogram-ext-0.1.3/botty/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.2/botty/middlewares/misc.py` & `aiogram-ext-0.1.3/botty/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.2/botty/middlewares/throttling.py` & `aiogram-ext-0.1.3/botty/middlewares/throttling.py`

 * *Files identical despite different names*

