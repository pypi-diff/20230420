# Comparing `tmp/telebot_against_war-0.6.2.tar.gz` & `tmp/telebot_against_war-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_against_war-0.6.2.tar", max compression
+gzip compressed data, was "telebot_against_war-0.6.3.tar", max compression
```

## Comparing `telebot_against_war-0.6.2.tar` & `telebot_against_war-0.6.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    18047 2023-04-18 22:11:17.911768 telebot_against_war-0.6.2/LICENSE
--rw-r--r--   0        0        0     2064 2023-04-18 22:11:17.911768 telebot_against_war-0.6.2/README.md
--rw-r--r--   0        0        0     1103 2023-04-18 22:11:56.904090 telebot_against_war-0.6.2/pyproject.toml
--rw-r--r--   0        0        0   155717 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/__init__.py
--rw-r--r--   0        0        0    81276 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/api.py
--rw-r--r--   0        0        0     5034 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/callback_data.py
--rw-r--r--   0        0        0     2913 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/check_text.py
--rw-r--r--   0        0        0     4733 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/filters.py
--rw-r--r--   0        0        0     8645 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/formatting.py
--rw-r--r--   0        0        0     3225 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/graceful_shutdown.py
--rw-r--r--   0        0        0     2049 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/helpers.py
--rw-r--r--   0        0        0     2046 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/metrics.py
--rw-r--r--   0        0        0        0 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/py.typed
--rw-r--r--   0        0        0     1797 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/runner.py
--rw-r--r--   0        0        0      396 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/storages/__init__.py
--rw-r--r--   0        0        0     1710 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/storages/base_storage.py
--rw-r--r--   0        0        0     2296 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/storages/memory_storage.py
--rw-r--r--   0        0        0     3695 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/storages/pickle_storage.py
--rw-r--r--   0        0        0     5626 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/storages/redis_storage.py
--rw-r--r--   0        0        0    35072 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/test_util.py
--rw-r--r--   0        0        0   156941 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/types/__init__.py
--rw-r--r--   0        0        0     2724 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/types/constants.py
--rw-r--r--   0        0        0     1852 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/types/service.py
--rw-r--r--   0        0        0    10649 2023-04-18 22:11:17.915768 telebot_against_war-0.6.2/telebot/util.py
--rw-r--r--   0        0        0     8202 2023-04-18 22:11:17.919768 telebot_against_war-0.6.2/telebot/webhook.py
--rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 telebot_against_war-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    18047 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/LICENSE
+-rw-r--r--   0        0        0     2064 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/README.md
+-rw-r--r--   0        0        0     1103 2023-04-20 20:27:20.101179 telebot_against_war-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0   155717 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/__init__.py
+-rw-r--r--   0        0        0    81276 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/api.py
+-rw-r--r--   0        0        0     5034 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/callback_data.py
+-rw-r--r--   0        0        0     2913 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/check_text.py
+-rw-r--r--   0        0        0     4733 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/filters.py
+-rw-r--r--   0        0        0     8645 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/formatting.py
+-rw-r--r--   0        0        0     3225 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/graceful_shutdown.py
+-rw-r--r--   0        0        0     2049 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/helpers.py
+-rw-r--r--   0        0        0     2046 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/metrics.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/py.typed
+-rw-r--r--   0        0        0     1797 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/runner.py
+-rw-r--r--   0        0        0      396 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/storages/__init__.py
+-rw-r--r--   0        0        0     1710 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/storages/base_storage.py
+-rw-r--r--   0        0        0     2296 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/storages/memory_storage.py
+-rw-r--r--   0        0        0     3695 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/storages/pickle_storage.py
+-rw-r--r--   0        0        0     5626 2023-04-20 20:26:38.984561 telebot_against_war-0.6.3/telebot/storages/redis_storage.py
+-rw-r--r--   0        0        0    35563 2023-04-20 20:26:38.988561 telebot_against_war-0.6.3/telebot/test_util.py
+-rw-r--r--   0        0        0   156941 2023-04-20 20:26:38.988561 telebot_against_war-0.6.3/telebot/types/__init__.py
+-rw-r--r--   0        0        0     2724 2023-04-20 20:26:38.988561 telebot_against_war-0.6.3/telebot/types/constants.py
+-rw-r--r--   0        0        0     1852 2023-04-20 20:26:38.988561 telebot_against_war-0.6.3/telebot/types/service.py
+-rw-r--r--   0        0        0    10649 2023-04-20 20:26:38.988561 telebot_against_war-0.6.3/telebot/util.py
+-rw-r--r--   0        0        0     8202 2023-04-20 20:26:38.988561 telebot_against_war-0.6.3/telebot/webhook.py
+-rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 telebot_against_war-0.6.3/PKG-INFO
```

### Comparing `telebot_against_war-0.6.2/LICENSE` & `telebot_against_war-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/README.md` & `telebot_against_war-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/pyproject.toml` & `telebot_against_war-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telebot-against-war"
-version = "0.6.2"  # replaced by dynamic versioning plugin
+version = "0.6.3"  # replaced by dynamic versioning plugin
 description = "Async-first fork of pyTelegramBotApi"
 authors = ["Igor Vaiman <gosha.vaiman@gmail.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 repository = "https://github.com/bots-against-war/telebot"
 packages = [
     { include = "telebot" },
```

### Comparing `telebot_against_war-0.6.2/telebot/__init__.py` & `telebot_against_war-0.6.3/telebot/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/api.py` & `telebot_against_war-0.6.3/telebot/api.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/callback_data.py` & `telebot_against_war-0.6.3/telebot/callback_data.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/check_text.py` & `telebot_against_war-0.6.3/telebot/check_text.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/filters.py` & `telebot_against_war-0.6.3/telebot/filters.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/formatting.py` & `telebot_against_war-0.6.3/telebot/formatting.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/graceful_shutdown.py` & `telebot_against_war-0.6.3/telebot/graceful_shutdown.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/helpers.py` & `telebot_against_war-0.6.3/telebot/helpers.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/metrics.py` & `telebot_against_war-0.6.3/telebot/metrics.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/runner.py` & `telebot_against_war-0.6.3/telebot/runner.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/storages/base_storage.py` & `telebot_against_war-0.6.3/telebot/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/storages/memory_storage.py` & `telebot_against_war-0.6.3/telebot/storages/memory_storage.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/storages/pickle_storage.py` & `telebot_against_war-0.6.3/telebot/storages/pickle_storage.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/storages/redis_storage.py` & `telebot_against_war-0.6.3/telebot/storages/redis_storage.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/test_util.py` & `telebot_against_war-0.6.3/telebot/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 # MockAsyncTeleBot aims at mocking only "active" bot actions like sending a message,
 # so these should work as usual
 UNMOCKABLE_METHOD_NAMES = {
     "logger",
     "close",
     "log_out",
-    "reply_to",  # conveniense method, calls, send_message
+    "reply_to",  # conveniense method, calls send_message internally
     "close_session",
     "get_updates",
     "infinity_polling",
     "update_listener",
     "add_custom_filter",
     "skip_updates",
     # update processing logic
@@ -66,17 +66,22 @@
 NO_DEFAULT_RETURN_VALUE = object()
 
 
 class NoDefaultValueException(Exception):
     pass
 
 
-def mocked(method: AsyncTeleBotMethodT, method_name: Optional[str] = None) -> AsyncTeleBotMethodT:
+def mocked(
+    method: AsyncTeleBotMethodT,
+    method_name: Optional[str] = None,
+    do_not_register: bool = False,
+) -> AsyncTeleBotMethodT:
     method_name_ = method_name or method.__name__
-    MOCKED_METHOD_NAMES.add(method_name_)
+    if not do_not_register:
+        MOCKED_METHOD_NAMES.add(method_name_)
 
     async def decorated(self: "MockedAsyncTeleBot", *args, **kwargs):
         method_param_names = [
             param_name for param_name in inspect.signature(method).parameters.keys() if param_name != "self"
         ]
         full_kwargs = dict(zip(method_param_names, args))
         full_kwargs.update(kwargs)
@@ -143,15 +148,24 @@
             for mn in dir(AsyncTeleBot)
             if not (mn.startswith("__") or mn in UNMOCKABLE_METHOD_NAMES or mn in MOCKED_METHOD_NAMES)
         }
         for method_name in no_default_method_names:
             setattr(
                 self,
                 method_name,
-                MethodType(mocked(self._no_default_value_mocked_method, method_name=method_name), self),
+                MethodType(
+                    mocked(
+                        self._no_default_value_mocked_method,
+                        method_name=method_name,
+                        # HACK: if the method being mocked here is registered (is in global MOCKED_METHOD_NAMES)
+                        #       subsequent instantiation of MockedAsyncTeleBot will have these methods NOT mocked
+                        do_not_register=True,
+                    ),
+                    self,
+                ),
             )
 
     async def _no_default_value_mocked_method(self, *args, **kwargs):
         raise NoDefaultValueException()
 
     def add_return_values(self, method_name: str, *values: Any, repeating: bool = False):
         """Can be used from tests to specify return values of mocked methods. Also supports exception to emulate
@@ -216,15 +230,15 @@
         switch_pm_text: Optional[str] = None,
         switch_pm_parameter: Optional[str] = None,
     ) -> bool:
         return True
 
     @mocked
     async def answer_pre_checkout_query(
-        self, pre_checkout_query_id: int, ok: bool, error_message: Optional[str] = None
+        self, pre_checkout_query_id: str, ok: bool, error_message: Optional[str] = None
     ) -> bool:
         return True
 
     @mocked
     async def answer_shipping_query(
         self,
         shipping_query_id: str,
```

### Comparing `telebot_against_war-0.6.2/telebot/types/__init__.py` & `telebot_against_war-0.6.3/telebot/types/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/types/constants.py` & `telebot_against_war-0.6.3/telebot/types/constants.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/types/service.py` & `telebot_against_war-0.6.3/telebot/types/service.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/util.py` & `telebot_against_war-0.6.3/telebot/util.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/telebot/webhook.py` & `telebot_against_war-0.6.3/telebot/webhook.py`

 * *Files identical despite different names*

### Comparing `telebot_against_war-0.6.2/PKG-INFO` & `telebot_against_war-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebot-against-war
-Version: 0.6.2
+Version: 0.6.3
 Summary: Async-first fork of pyTelegramBotApi
 Home-page: https://github.com/bots-against-war/telebot
 License: GPL-2.0-only
 Author: Igor Vaiman
 Author-email: gosha.vaiman@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telebot-against-war Version: 0.6.2 Summary: Async-
+Metadata-Version: 2.1 Name: telebot-against-war Version: 0.6.3 Summary: Async-
 first fork of pyTelegramBotApi Home-page: https://github.com/bots-against-war/
 telebot License: GPL-2.0-only Author: Igor Vaiman Author-email:
 gosha.vaiman@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v2 (GPLv2) Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-
```

