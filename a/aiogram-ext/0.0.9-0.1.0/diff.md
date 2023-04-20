# Comparing `tmp/aiogram-ext-0.0.9.tar.gz` & `tmp/aiogram-ext-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.0.9.tar", last modified: Thu Apr 13 14:15:48 2023, max compression
+gzip compressed data, was "aiogram-ext-0.1.0.tar", last modified: Thu Apr 20 17:09:46 2023, max compression
```

## Comparing `aiogram-ext-0.0.9.tar` & `aiogram-ext-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      855 2023-04-13 14:00:40.168816 aiogram-ext-0.0.9/aiogram_ext/__init__.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.0.9/aiogram_ext/buttons.py
--rw-r--r--   0        0        0      269 2023-04-13 14:01:13.830112 aiogram-ext-0.0.9/aiogram_ext/config.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.0.9/aiogram_ext/context.py
--rw-r--r--   0        0        0     1483 2023-04-13 14:00:40.159310 aiogram-ext-0.0.9/aiogram_ext/deps.py
--rw-r--r--   0        0        0     5981 2023-04-13 14:15:39.821528 aiogram-ext-0.0.9/aiogram_ext/dispatcher.py
--rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.0.9/aiogram_ext/env.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.0.9/aiogram_ext/filters.py
--rw-r--r--   0        0        0      459 2023-04-12 10:56:42.149572 aiogram-ext-0.0.9/aiogram_ext/helpers.py
--rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.0.9/aiogram_ext/keyboards.py
--rw-r--r--   0        0        0      810 2023-04-13 14:08:18.534155 aiogram-ext-0.0.9/aiogram_ext/loader.py
--rw-r--r--   0        0        0      154 2023-04-12 10:34:24.400978 aiogram-ext-0.0.9/aiogram_ext/middlewares/__init__.py
--rw-r--r--   0        0        0     6983 2023-04-12 10:34:24.432621 aiogram-ext-0.0.9/aiogram_ext/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.0.9/aiogram_ext/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.0.9/aiogram_ext/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.0.9/aiogram_ext/middlewares/throttling.py
--rw-r--r--   0        0        0      594 2023-04-13 13:42:05.708666 aiogram-ext-0.0.9/aiogram_ext/texts.py
--rw-r--r--   0        0        0      367 2023-04-13 14:15:43.996408 aiogram-ext-0.0.9/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.0.9/README.md
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      882 2023-04-16 22:10:48.315246 aiogram-ext-0.1.0/botty/__init__.py
+-rw-r--r--   0        0        0      251 2023-04-14 12:15:49.770806 aiogram-ext-0.1.0/botty/bot.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.1.0/botty/buttons.py
+-rw-r--r--   0        0        0      264 2023-04-17 23:58:40.002141 aiogram-ext-0.1.0/botty/config.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.1.0/botty/context.py
+-rw-r--r--   0        0        0     1665 2023-04-16 22:10:48.295151 aiogram-ext-0.1.0/botty/deps.py
+-rw-r--r--   0        0        0     5655 2023-04-20 17:09:41.994793 aiogram-ext-0.1.0/botty/dispatcher.py
+-rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.1.0/botty/env.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.1.0/botty/filters.py
+-rw-r--r--   0        0        0      399 2023-04-16 19:04:22.106465 aiogram-ext-0.1.0/botty/helpers.py
+-rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.1.0/botty/keyboards.py
+-rw-r--r--   0        0        0      519 2023-04-15 14:16:45.313035 aiogram-ext-0.1.0/botty/loader.py
+-rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.1.0/botty/middlewares/__init__.py
+-rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.1.0/botty/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.1.0/botty/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.1.0/botty/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.1.0/botty/middlewares/throttling.py
+-rw-r--r--   0        0        0      455 2023-04-20 17:09:41.975063 aiogram-ext-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.1.0/README.md
+-rw-r--r--   0        0        0      239 2023-04-16 23:01:01.500707 aiogram-ext-0.1.0/tests/__main__.py
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.1.0/PKG-INFO
```

### Comparing `aiogram-ext-0.0.9/aiogram_ext/__init__.py` & `aiogram-ext-0.1.0/botty/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,20 +9,21 @@
     Message,
     Query,
     FSMContext,
     State,
     StatesGroup,
     SkipHandler,
     CancelHandler,
+    TelegramAPIError,
 )
 from .dispatcher import Dispatcher
 from .env import env
 from .helpers import reply
 from .keyboards import ReplyKeyboard, InlineKeyboard
-from .loader import bot, dp, logger, texts
+from .loader import bot, dp, logger
 
 __all__ = [
     "Dispatcher",
     "ReplyKeyboard",
     "InlineKeyboard",
     "InlineButton",
     "CallbackButton",
@@ -30,16 +31,16 @@
     "InlineQueryButton",
     "ContactRequestButton",
     "reply",
     "env",
     "bot",
     "dp",
     "logger",
-    "texts",
     "Message",
     "Query",
     "State",
     "FSMContext",
     "SkipHandler",
     "StatesGroup",
     "CancelHandler",
+    "TelegramAPIError",
 ]
```

### Comparing `aiogram-ext-0.0.9/aiogram_ext/buttons.py` & `aiogram-ext-0.1.0/botty/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.9/aiogram_ext/context.py` & `aiogram-ext-0.1.0/botty/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.9/aiogram_ext/deps.py` & `aiogram-ext-0.1.0/botty/deps.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     Poll,
     PollAnswer,
     ChatMemberUpdated,
     ReplyKeyboardRemove,
 )
 from aiogram.utils import executor
 from aiogram.utils.mixins import ContextInstanceMixin
+from aiogram.utils.exceptions import TelegramAPIError
 
 __all__ = [
     "ReplyKeyboardMarkup",
     "InlineKeyboardMarkup",
     "InlineKeyboardButton",
     "KeyboardButton",
     "Bot",
@@ -58,8 +59,12 @@
     "Callable",
     "Any",
     "environ",
     "MongoStorage",
     "SkipHandler",
     "CancelHandler",
     "StatesGroup",
+    "ReplyMarkup",
+    "TelegramAPIError",
 ]
+
+ReplyMarkup = ReplyKeyboardMarkup | InlineKeyboardMarkup | ReplyKeyboardRemove
```

### Comparing `aiogram-ext-0.0.9/aiogram_ext/env.py` & `aiogram-ext-0.1.0/botty/env.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.9/aiogram_ext/filters.py` & `aiogram-ext-0.1.0/botty/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.9/aiogram_ext/keyboards.py` & `aiogram-ext-0.1.0/botty/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.9/aiogram_ext/middlewares/_conversation.py` & `aiogram-ext-0.1.0/botty/middlewares/_conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing import TypeVar, Union, Optional, Literal
 
 from aiogram import types, Dispatcher, Bot
 from aiogram.dispatcher import FSMContext
 from aiogram.dispatcher.middlewares import BaseMiddleware
 from aiogram.dispatcher.storage import FSMContextProxy
 
-from aiogram_ext._questions import ConvState, ConvStatesGroup, ConvStatesGroupMeta
-from aiogram_ext._questions import Quest, Quests, QuestText, QuestFunc
+from botty._questions import ConvState, ConvStatesGroup, ConvStatesGroupMeta
+from botty._questions import Quest, Quests, QuestText, QuestFunc
 
 __all__ = ["UpdateData", "UpdateUserState", "AnswerOnReturn"]
 
 T = TypeVar("T")
 _StorageData = Union[str, int, tuple, dict, None]
 StorageData = Union[_StorageData, list[_StorageData]]
 NewState = Union[
```

### Comparing `aiogram-ext-0.0.9/aiogram_ext/middlewares/_membership.py` & `aiogram-ext-0.1.0/botty/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.9/aiogram_ext/middlewares/misc.py` & `aiogram-ext-0.1.0/botty/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.9/aiogram_ext/middlewares/throttling.py` & `aiogram-ext-0.1.0/botty/middlewares/throttling.py`

 * *Files identical despite different names*

