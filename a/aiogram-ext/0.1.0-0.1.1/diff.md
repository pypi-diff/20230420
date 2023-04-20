# Comparing `tmp/aiogram-ext-0.1.0.tar.gz` & `tmp/aiogram-ext-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.1.0.tar", last modified: Thu Apr 20 17:09:46 2023, max compression
+gzip compressed data, was "aiogram-ext-0.1.1.tar", last modified: Thu Apr 20 17:19:02 2023, max compression
```

## Comparing `aiogram-ext-0.1.0.tar` & `aiogram-ext-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      882 2023-04-16 22:10:48.315246 aiogram-ext-0.1.0/botty/__init__.py
--rw-r--r--   0        0        0      251 2023-04-14 12:15:49.770806 aiogram-ext-0.1.0/botty/bot.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.1.0/botty/buttons.py
--rw-r--r--   0        0        0      264 2023-04-17 23:58:40.002141 aiogram-ext-0.1.0/botty/config.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.1.0/botty/context.py
--rw-r--r--   0        0        0     1665 2023-04-16 22:10:48.295151 aiogram-ext-0.1.0/botty/deps.py
--rw-r--r--   0        0        0     5655 2023-04-20 17:09:41.994793 aiogram-ext-0.1.0/botty/dispatcher.py
--rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.1.0/botty/env.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.1.0/botty/filters.py
--rw-r--r--   0        0        0      399 2023-04-16 19:04:22.106465 aiogram-ext-0.1.0/botty/helpers.py
--rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.1.0/botty/keyboards.py
--rw-r--r--   0        0        0      519 2023-04-15 14:16:45.313035 aiogram-ext-0.1.0/botty/loader.py
--rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.1.0/botty/middlewares/__init__.py
--rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.1.0/botty/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.1.0/botty/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.1.0/botty/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.1.0/botty/middlewares/throttling.py
--rw-r--r--   0        0        0      455 2023-04-20 17:09:41.975063 aiogram-ext-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.1.0/README.md
--rw-r--r--   0        0        0      239 2023-04-16 23:01:01.500707 aiogram-ext-0.1.0/tests/__main__.py
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      882 2023-04-16 22:10:48.315246 aiogram-ext-0.1.1/botty/__init__.py
+-rw-r--r--   0        0        0      251 2023-04-14 12:15:49.770806 aiogram-ext-0.1.1/botty/bot.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.1.1/botty/buttons.py
+-rw-r--r--   0        0        0      264 2023-04-17 23:58:40.002141 aiogram-ext-0.1.1/botty/config.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.1.1/botty/context.py
+-rw-r--r--   0        0        0     1665 2023-04-16 22:10:48.295151 aiogram-ext-0.1.1/botty/deps.py
+-rw-r--r--   0        0        0     6001 2023-04-20 17:17:51.422853 aiogram-ext-0.1.1/botty/dispatcher.py
+-rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.1.1/botty/env.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.1.1/botty/filters.py
+-rw-r--r--   0        0        0      399 2023-04-16 19:04:22.106465 aiogram-ext-0.1.1/botty/helpers.py
+-rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.1.1/botty/keyboards.py
+-rw-r--r--   0        0        0      519 2023-04-15 14:16:45.313035 aiogram-ext-0.1.1/botty/loader.py
+-rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.1.1/botty/middlewares/__init__.py
+-rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.1.1/botty/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.1.1/botty/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.1.1/botty/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.1.1/botty/middlewares/throttling.py
+-rw-r--r--   0        0        0      455 2023-04-20 17:18:49.293291 aiogram-ext-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.1.1/README.md
+-rw-r--r--   0        0        0      239 2023-04-16 23:01:01.500707 aiogram-ext-0.1.1/tests/__main__.py
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.1.1/PKG-INFO
```

### Comparing `aiogram-ext-0.1.0/botty/__init__.py` & `aiogram-ext-0.1.1/botty/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.0/botty/buttons.py` & `aiogram-ext-0.1.1/botty/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.0/botty/context.py` & `aiogram-ext-0.1.1/botty/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.0/botty/deps.py` & `aiogram-ext-0.1.1/botty/deps.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.0/botty/dispatcher.py` & `aiogram-ext-0.1.1/botty/dispatcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,27 +26,27 @@
         self.PHOTO = self.photo()
         self.TEXT = self.text()
         self.START = self.start()
         self.MESSAGE = self.message()
 
     @staticmethod
     def _gen_payload(
-        locals_: dict, exclude: list[str] = None, default_exclude=("self", "cls")
+            locals_: dict, exclude: list[str] = None, default_exclude=("self", "cls")
     ):
         kwargs = locals_.pop("kwargs", {})
         locals_.update(kwargs)
 
         if exclude is None:
             exclude = []
         return {
             key: value
             for key, value in locals_.items()
             if key not in exclude + list(default_exclude)
-            and value is not None
-            and not key.startswith("_")
+               and value is not None
+               and not key.startswith("_")
         }
 
     def _setup_filters(self):
         filters_factory = self.filters_factory
         filters_factory.bind(
             StorageDataFilter,
             exclude_event_handlers=[
@@ -95,19 +95,19 @@
     def message(self):
         return MessageHandler(self)
 
     def run(self):
         Executor(self).start_polling()
 
     def run_server(
-        self,
-        app_url: str,
-        app: Application = None,
-        path: str = "/bot",
-        port: int = APP_PORT,
+            self,
+            app_url: str,
+            app: Application = None,
+            path: str = "/bot",
+            port: int = APP_PORT,
     ):
         executor = Executor(self)
         executor.set_webhook(path, web_app=app)
         self._set_webhook(app_url + path)
         executor.run_app(port=port)
 
     def _set_webhook(self, url: str):
@@ -145,23 +145,35 @@
 
 class MessageHandler(Handler):
     def __init__(self, dp: Dispatcher, content_types: str | list[str] = "any"):
         super().__init__(dp)
         self._command = None
         self._text = None
         self._content_types = content_types
+        self._is_forwarded = None
+        self._is_reply = None
+
+    def is_forwarded(self):
+        self._is_forwarded = True
+        return self
+
+    def is_reply(self):
+        self._is_reply = True
+        return self
 
     def __call__(self, callback):
         deco = self._dp.message_handler(
             content_types=self._content_types,
             button=self._text,
             commands=self._command,
             state=self._state,
             chat_id=self._chat_id,
             user_id=self._user_id,
+            is_forwarded=self._is_forwarded,
+            is_reply=self._is_reply,
             **self._extra,
         )
         return deco(callback)
 
 
 class TextHandler(MessageHandler):
     def __init__(self, dp: Dispatcher, text: str = None):
```

### Comparing `aiogram-ext-0.1.0/botty/env.py` & `aiogram-ext-0.1.1/botty/env.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.0/botty/filters.py` & `aiogram-ext-0.1.1/botty/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.0/botty/keyboards.py` & `aiogram-ext-0.1.1/botty/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.0/botty/loader.py` & `aiogram-ext-0.1.1/botty/loader.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.0/botty/middlewares/_conversation.py` & `aiogram-ext-0.1.1/botty/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.0/botty/middlewares/_membership.py` & `aiogram-ext-0.1.1/botty/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.0/botty/middlewares/misc.py` & `aiogram-ext-0.1.1/botty/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.0/botty/middlewares/throttling.py` & `aiogram-ext-0.1.1/botty/middlewares/throttling.py`

 * *Files identical despite different names*

