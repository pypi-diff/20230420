# Comparing `tmp/telebot_components-0.7.3.tar.gz` & `tmp/telebot_components-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_components-0.7.3.tar", max compression
+gzip compressed data, was "telebot_components-0.8.0.tar", max compression
```

## Comparing `telebot_components-0.7.3.tar` & `telebot_components-0.8.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0    35148 2023-04-02 14:51:34.102767 telebot_components-0.7.3/LICENSE
--rw-r--r--   0        0        0     2258 2023-04-02 14:51:34.102767 telebot_components-0.7.3/README.md
--rw-r--r--   0        0        0     1267 2023-04-02 14:52:24.517244 telebot_components-0.7.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-02 14:51:34.102767 telebot_components-0.7.3/telebot_components/__init__.py
--rw-r--r--   0        0        0    13052 2023-04-02 14:51:34.102767 telebot_components-0.7.3/telebot_components/broadcast/__init__.py
--rw-r--r--   0        0        0     2835 2023-04-02 14:51:34.102767 telebot_components-0.7.3/telebot_components/broadcast/message_senders.py
--rw-r--r--   0        0        0      159 2023-04-02 14:51:34.102767 telebot_components-0.7.3/telebot_components/broadcast/subscriber.py
--rw-r--r--   0        0        0        0 2023-04-02 14:51:34.102767 telebot_components-0.7.3/telebot_components/constants/__init__.py
--rw-r--r--   0        0        0    15212 2023-04-02 14:51:34.102767 telebot_components-0.7.3/telebot_components/constants/emoji.py
--rw-r--r--   0        0        0      168 2023-04-02 14:51:34.102767 telebot_components-0.7.3/telebot_components/constants/times.py
--rw-r--r--   0        0        0    46905 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/feedback/__init__.py
--rw-r--r--   0        0        0     2075 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/feedback/anti_spam.py
--rw-r--r--   0        0        0        0 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/feedback/integration/__init__.py
--rw-r--r--   0        0        0     8263 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/feedback/integration/aux_feedback_handler.py
--rw-r--r--   0        0        0     3994 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/feedback/integration/interface.py
--rw-r--r--   0        0        0    34403 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/feedback/integration/trello.py
--rw-r--r--   0        0        0      221 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/feedback/trello_integration.py
--rw-r--r--   0        0        0      493 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/feedback/types.py
--rw-r--r--   0        0        0        0 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/form/__init__.py
--rw-r--r--   0        0        0    29358 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/form/field.py
--rw-r--r--   0        0        0    14757 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/form/form.py
--rw-r--r--   0        0        0    20318 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/form/handler.py
--rw-r--r--   0        0        0        0 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/form/helpers/__init__.py
--rw-r--r--   0        0        0     7573 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/form/helpers/calendar_keyboard.py
--rw-r--r--   0        0        0        0 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/menu/__init__.py
--rw-r--r--   0        0        0    11963 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/menu/menu.py
--rw-r--r--   0        0        0        0 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/py.typed
--rw-r--r--   0        0        0        0 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/redis_utils/__init__.py
--rw-r--r--   0        0        0    10640 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/redis_utils/emulation.py
--rw-r--r--   0        0        0     6087 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/redis_utils/interface.py
--rw-r--r--   0        0        0        0 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/stores/__init__.py
--rw-r--r--   0        0        0     1825 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/stores/banned_users.py
--rw-r--r--   0        0        0     8115 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/stores/category.py
--rw-r--r--   0        0        0     9902 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/stores/generic.py
--rw-r--r--   0        0        0     8069 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/stores/language.py
--rw-r--r--   0        0        0      397 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/stores/types.py
--rw-r--r--   0        0        0     3871 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/stores/user_group.py
--rw-r--r--   0        0        0      614 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/stores/utils.py
--rw-r--r--   0        0        0     7647 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/utils/__init__.py
--rw-r--r--   0        0        0     5136 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/utils/airtable.py
--rw-r--r--   0        0        0     2564 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/utils/alerts.py
--rw-r--r--   0        0        0     1257 2023-04-02 14:51:34.106767 telebot_components-0.7.3/telebot_components/utils/strings.py
--rw-r--r--   0        0        0     3369 1970-01-01 00:00:00.000000 telebot_components-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-20 21:06:42.150375 telebot_components-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2258 2023-04-20 21:06:42.150375 telebot_components-0.8.0/README.md
+-rw-r--r--   0        0        0     1573 2023-04-20 21:07:29.130652 telebot_components-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/__init__.py
+-rw-r--r--   0        0        0    13083 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/broadcast/__init__.py
+-rw-r--r--   0        0        0     2835 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/broadcast/message_senders.py
+-rw-r--r--   0        0        0      159 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/broadcast/subscriber.py
+-rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/constants/__init__.py
+-rw-r--r--   0        0        0    15212 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/constants/emoji.py
+-rw-r--r--   0        0        0      168 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/constants/times.py
+-rw-r--r--   0        0        0    50122 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/__init__.py
+-rw-r--r--   0        0        0     2075 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/anti_spam.py
+-rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/integration/__init__.py
+-rw-r--r--   0        0        0     8255 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/integration/aux_feedback_handler.py
+-rw-r--r--   0        0        0     3983 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/integration/interface.py
+-rw-r--r--   0        0        0    34435 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/integration/trello.py
+-rw-r--r--   0        0        0      237 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/trello_integration.py
+-rw-r--r--   0        0        0      493 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/types.py
+-rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/form/__init__.py
+-rw-r--r--   0        0        0    29347 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/form/field.py
+-rw-r--r--   0        0        0    14757 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/form/form.py
+-rw-r--r--   0        0        0    20318 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/form/handler.py
+-rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/form/helpers/__init__.py
+-rw-r--r--   0        0        0     7572 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/form/helpers/calendar_keyboard.py
+-rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/menu/__init__.py
+-rw-r--r--   0        0        0    11976 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/menu/menu.py
+-rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/py.typed
+-rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/redis_utils/__init__.py
+-rw-r--r--   0        0        0    10640 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/redis_utils/emulation.py
+-rw-r--r--   0        0        0     6078 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/redis_utils/interface.py
+-rw-r--r--   0        0        0        0 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/__init__.py
+-rw-r--r--   0        0        0     1825 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/banned_users.py
+-rw-r--r--   0        0        0     8229 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/category.py
+-rw-r--r--   0        0        0     8786 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/forum_topics.py
+-rw-r--r--   0        0        0     9845 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/generic.py
+-rw-r--r--   0        0        0     8066 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/language.py
+-rw-r--r--   0        0        0      397 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/types.py
+-rw-r--r--   0        0        0     3914 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/user_group.py
+-rw-r--r--   0        0        0      614 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/utils.py
+-rw-r--r--   0        0        0     8134 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/utils/__init__.py
+-rw-r--r--   0        0        0     5136 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/utils/airtable.py
+-rw-r--r--   0        0        0     2564 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/utils/alerts.py
+-rw-r--r--   0        0        0     1257 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/utils/strings.py
+-rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 telebot_components-0.8.0/PKG-INFO
```

### Comparing `telebot_components-0.7.3/LICENSE` & `telebot_components-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/README.md` & `telebot_components-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/pyproject.toml` & `telebot_components-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 [tool.poetry]
 name = "telebot-components"
-version = "0.7.3"
+version = "0.8.0"
 description = "Framework/toolkit for building Telegram bots with telebot and redis"
 authors = ["Igor Vaiman <gosha.vaiman@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/bots-against-war/telebot-components"
 packages = [{include = "telebot_components"}]
+[tool.poetry.group.dev.dependencies]
+pyproject-flake8 = "^6.0.0.post1"
+coverage = "^7.2.3"
+
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 dirty = true
 style="semver"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-telebot-against-war = "^0.6.0"
+telebot-against-war = "^0.6.3"
 redis = "^4.3.1"
 py-trello = "^0.18.0"
 markdownify = "^0.11.2"
 pytest-mock = "^3.7.0"
 "ruamel.yaml" = "^0.17.21"
 pyairtable = "^1.3.0"
 Pillow = "^9.2.0"
 markdown = "^3.4.1"
 beautifulsoup4 = "^4.11.1"
 tenacity = "^8.1.0"
+async-lru = "^2.0.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-aiohttp = "1.0.4"
 pytest-asyncio = "^0.18.3"
 python-dotenv = "^0.20.0"
 aioresponses = "0.7.3"
@@ -56,7 +61,14 @@
 markers = [
     'integration: requires a real bot to run',
 ]
 
 [tool.mypy]
 incremental = false
 files = '.'
+
+[tool.flake8]
+max-line-length = 120
+extend-ignore = [
+    "F841",  # local variable 'xxx' is assigned to but never used
+    "E203",  # whitespace before ':' (black formatting compatibility)
+]
```

### Comparing `telebot_components-0.7.3/telebot_components/broadcast/__init__.py` & `telebot_components-0.8.0/telebot_components/broadcast/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
                     await self.current_pending_subscribers_by_topic_store.add_multiple(
                         qb.topic, await self.topic_subscribers(qb.topic)
                     )
                     dequeued_broadcasts.append(qb)
                     if on_broadcast_start is not None:
                         try:
                             await on_broadcast_start(qb)
-                        except:
+                        except Exception:
                             logger.exception("Unexpected error in on_broadcast_start callback, ignoring")
                     self.is_broadcasting = True
                 else:
                     logger.info(
                         f"Overdue broadcast on topic {qb.topic} "
                         + f"scheduled {time.time() - qb.start_time:3f} sec ago "
                         + f"with sender {qb.sender}, waiting for previous broadcast on this topic to finish"
@@ -206,15 +206,16 @@
                 for b in dequeued_broadcasts:
                     await self.broadcast_queue_store.remove(self.CONST_KEY, b)
                 queued_broadcasts = await self.broadcast_queue_store.all(self.CONST_KEY)
             self.next_broadcast_queue_processing_time = (
                 min([qb.start_time for qb in queued_broadcasts]) if queued_broadcasts else time.time() + 300
             )
             logger.info(
-                f"The next broadcast queue processing scheduled in {self.next_broadcast_queue_processing_time - time.time():.2f} sec"
+                "The next broadcast queue processing scheduled "
+                + f"in {self.next_broadcast_queue_processing_time - time.time():.2f} sec"
             )
 
     @prevent_shutdown_on_broadcasting
     @restart_on_errors
     async def _send_current_broadcasts(self, bot: AsyncTeleBot, on_broadcast_end: Optional[BroadcastCallback] = None):
         BATCH_SIZE = 200  # each batch should take around 10-20 sec to complete
         MESSAGES_PER_SECOND_LIMIT = 20  # telegram rate limit is around 30 msg/sec, but we play safe
```

### Comparing `telebot_components-0.7.3/telebot_components/broadcast/message_senders.py` & `telebot_components-0.8.0/telebot_components/broadcast/message_senders.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/telebot_components/constants/emoji.py` & `telebot_components-0.8.0/telebot_components/constants/emoji.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/telebot_components/feedback/__init__.py` & `telebot_components-0.8.0/telebot_components/feedback/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 import copy
 import dataclasses
-import functools
 import logging
 import math
 import random
 from collections.abc import Awaitable
 from dataclasses import dataclass
 from datetime import timedelta
 from typing import Any, Callable, Coroutine, Optional, Protocol, TypedDict, cast
@@ -32,15 +31,16 @@
     UserMessageRepliedFromIntegrationEvent,
 )
 from telebot_components.feedback.integration.trello import TrelloIntegration
 from telebot_components.feedback.types import UserMessageRepliedEvent
 from telebot_components.form.field import TelegramAttachment
 from telebot_components.redis_utils.interface import RedisInterface
 from telebot_components.stores.banned_users import BannedUsersStore
-from telebot_components.stores.category import Category, CategoryStore
+from telebot_components.stores.category import CategoryStore
+from telebot_components.stores.forum_topics import CategoryForumTopicStore
 from telebot_components.stores.generic import (
     KeyFlagStore,
     KeyListStore,
     KeySetStore,
     KeyValueStore,
 )
 from telebot_components.stores.language import (
@@ -141,21 +141,27 @@
 
     # appended to admin chat help under "Other" section; Supports HTML markup
     admin_chat_help_extra: Optional[str] = None
 
     # if True, user messages are not forwarded but copied to admin chat without any back
     # link to the user account; before the message, user id hash is sent for identification
     full_user_anonymization: bool = False
-    # function used to generate user id hash for a particular bot; if full_user_anonymization is False,
-    # it is ignored
+
+    # (user id, bot prefix) -> unique string identifying the user
+    # used to generate user id hash for a particular bot;
     user_id_hash_func: Callable[[int, str], str] = emoji_hash
 
     # how many messages to forward in one go on /log command
     message_log_page_size: int = 30
 
+    # [⚠️ experimental] create new forum topic per new user
+    forum_topic_per_user: bool = False
+
+    user_forum_topic_lifetime: timedelta = timedelta(days=7)
+
 
 @dataclasses.dataclass
 class MessageForwarderResult:
     admin_chat_msg: tg.Message
     user_msg: Optional[tg.Message]
 
 
@@ -171,23 +177,25 @@
      - the bot copies messages back to the user
     """
 
     CONST_KEY = "const"
 
     def __init__(
         self,
+        *,
         admin_chat_id: int,
         redis: RedisInterface,
         bot_prefix: str,
         config: FeedbackConfig,
         anti_spam: AntiSpamInterface,
         service_messages: ServiceMessages,
         banned_users_store: Optional[BannedUsersStore] = None,
         language_store: Optional[LanguageStore] = None,
         category_store: Optional[CategoryStore] = None,
+        forum_topic_store: Optional[CategoryForumTopicStore] = None,
         trello_integration: Optional[TrelloIntegration] = None,
         integrations: Optional[list[FeedbackHandlerIntegration]] = None,
         admin_chat_response_actions: Optional[list[AdminChatAction]] = None,
         # specific feedback handler name in case there are several of them;
         # the default (empty string) makes it backwards compatible
         name: str = "",
     ) -> None:
@@ -202,14 +210,19 @@
         self._admin_chat: Optional[tg.Chat] = None
         self._bot: Optional[AsyncTeleBot] = None
 
         self.anti_spam = anti_spam
         self.banned_users_store = banned_users_store
         self.language_store = language_store
         self.category_store = category_store
+        self.forum_topic_store = forum_topic_store
+        if self.config.forum_topic_per_user and self.forum_topic_store is not None:
+            raise ValueError(
+                "Forum topics can be used either for categories OR created per-user, not both at the same time"
+            )
 
         integrations_ = integrations or []
         if trello_integration is not None:
             self.logger.warning("'trello_integration' argument is deprecated, please use 'integrations' instead")
             integrations_.append(trello_integration)
         self.integrations = integrations_
 
@@ -285,23 +298,34 @@
         self.copied_to_user_data_store = KeyValueStore[CopiedMessageToUserData](
             name="copied-to-user-ok",
             prefix=bot_prefix,
             redis=redis,
             expiration_time=times.FIVE_MINUTES,
         )
 
+        # const key -> last sent user id hash to avoid repeating it on multiple consequtive messages
         self.last_sent_user_id_hash_store = KeyValueStore[str](
             name="last-sent-user-id-hash",
             prefix=bot_prefix,
             redis=redis,
             expiration_time=timedelta(hours=12),
             loader=str,
             dumper=str,
         )
 
+        # message
+        self.message_thread_id_by_user_id_store = KeyValueStore[int](
+            name="message-thread-id-by-user",
+            prefix=bot_prefix,
+            redis=redis,
+            expiration_time=self.config.user_forum_topic_lifetime,
+            loader=int,
+            dumper=str,
+        )
+
     @property
     def bot(self) -> AsyncTeleBot:
         if self._bot is None:
             raise RuntimeError("Bot was not initialized")
         return self._bot
 
     async def admin_chat(self) -> tg.Chat:
@@ -337,16 +361,16 @@
         paragraphs = [
             "<b>Справка-памятка для админского чата</b>",
             "<i>Сообщение сгенерировано автоматически по команде /help</i>",
         ]
         copies_or_forwards = "пересылает" if not self.config.full_user_anonymization else "копирует"
         paragraphs.append(
             "💬 <i>Основное</i>\n"
-            + f"· В этот чат бот {copies_or_forwards} все сообщения (кроме специальных случаев вроде /команд), которые ему "
-            + "пишут в личку.\n"
+            + f"· В этот чат бот {copies_or_forwards} все сообщения (кроме специальных случаев вроде /команд), "
+            + "которые ему пишут в личку.\n"
             + (
                 (
                     "· Перед скопированным сообщением бот указывает анонимизированный идентификатор пользователь_ницы, "
                     + f"например такой: «{self.config.user_id_hash_func(random.randint(1, 1000), self.bot_prefix)}»\n"
                 )
                 if self.config.full_user_anonymization
                 else ""
@@ -370,23 +394,24 @@
                 categories_help += "· Выбор категории необязателен, боту можно написать и без него."
 
             paragraphs.append(categories_help)
 
         security_help = (
             "🛡️ <i>Защита и безопасность</i>\n"
             + "· Бот никак не выдаёт, кто отвечает пользователь_нице из этого чата. Насколько возможно судить, "
-            + "никакого способа взломать бота нет. Однако всё, что вы отвечаете через бота, сразу пересылается человеку "
-            + "на другом конце, и отменить отправку можно лишь в течении первых 5 минут, поэтому будьте внимательны!"
+            + "никакого способа взломать бота нет. Однако всё, что вы отвечаете через бота, "
+            + "сразу пересылается человеку на другом конце, и отменить отправку можно лишь в течении первых "
+            + "5 минут, поэтому будьте внимательны!"
         )
         if isinstance(self.anti_spam, AntiSpam):
             security_help += (
                 "\n"
                 + "· Бот автоматически ограничивает число сообщений, присылаемых ему в единицу времени. "
-                + f"Конфигурация на данный момент: не больше {self.anti_spam.config.throttle_after_messages} сообщений за "
-                + f"{self.anti_spam.config.throttle_duration}. При необходимости её можно изменять."
+                + f"Конфигурация на данный момент: не больше {self.anti_spam.config.throttle_after_messages} "
+                + f"сообщений за {self.anti_spam.config.throttle_duration}. При необходимости её можно изменять."
             )
         if self.banned_users_store is not None:
             security_help += (
                 "\n· Если ответить на пересланное сообщение командой /ban, "
                 + "пользователь_ница будет заблокирован_а, а все сообщения от них в чате — удалены"
             )
         paragraphs.append(security_help)
@@ -399,16 +424,16 @@
             + (
                 "в этот чат. Можно настроить бота так, чтобы бот пересылал историю не сюда, а "
                 + "в диалог с администратор_кой, которая её запросила."
                 if self.config.message_log_to_admin_chat
                 else "вам в личку (для этого вы должны хотя бы раз что-то ему написать). Можно настроить бота так, "
                 + "чтобы чтобы бот пересылал историю сообщений не в личку, а прямо в этот чат."
             )
-            + f"\n· По умолчанию бот пересылает первые {self.config.message_log_page_size} сообщений, дальше можно листать "
-            + "по страницам: «/log 2», «/log 3», и так далее"
+            + f"\n· По умолчанию бот пересылает первые {self.config.message_log_page_size} сообщений, "
+            + "дальше можно листать по страницам: «/log 2», «/log 3», и так далее"
         )
 
         integration_help_messages = [integration.help_message_section() for integration in self.integrations]
         paragraphs.extend([m for m in integration_help_messages if m])
 
         if self.config.admin_chat_help_extra:
             paragraphs.append("🪄 <i>Другое</i>\n" + self.config.admin_chat_help_extra)
@@ -420,15 +445,15 @@
         else:
             return True
 
     async def _handle_user_message(
         self,
         bot: AsyncTeleBot,
         user: tg.User,
-        message_forwarder: Callable[[], Awaitable[MessageForwarderResult]],
+        message_forwarder: Callable[[Optional[int]], Awaitable[MessageForwarderResult]],
         user_replier: Callable[[str, Optional[tg.ReplyMarkup]], Coroutine[None, None, Any]],
         send_user_id_hash: bool,
         export_to_integrations: bool = True,
     ) -> Optional[int]:
         if self.banned_users_store is not None and await self.banned_users_store.is_banned(user.id):
             return None
         anti_spam_status = await self.anti_spam.status(user)
@@ -440,20 +465,42 @@
         else:
             language = None
         if anti_spam_status is AntiSpamStatus.THROTTLING:
             anti_spam = cast(AntiSpam, self.anti_spam)  # only real AntiSpam can return this status
             await user_replier(self.service_messages.throttling(anti_spam.config, language), None)
             return None
 
+        category = await self.category_store.get_user_category(user) if self.category_store is not None else None
+        if self.forum_topic_store is not None:
+            message_thread_id: Optional[int] = await self.forum_topic_store.get_message_thread_id(category)
+        elif self.config.forum_topic_per_user:
+            message_thread_id = await self.message_thread_id_by_user_id_store.load(user.id)
+            if message_thread_id is None:
+                try:
+                    new_topic = await bot.create_forum_topic(
+                        chat_id=self.admin_chat_id,
+                        name=self.config.user_id_hash_func(
+                            user.id,
+                            self.bot_prefix,
+                        ),
+                    )
+                    # TODO: sent the topic to redis-backed queue for cleanup...
+                    message_thread_id = new_topic.message_thread_id
+                    await self.message_thread_id_by_user_id_store.save(user.id, message_thread_id)
+                except Exception:
+                    self.logger.exception(
+                        f"Error creating forum topic for user {user}, will send without message thread id"
+                    )
+        else:
+            message_thread_id = None
+
         hashtag_msg_data: Optional[HashtagMessageData] = None
-        category: Optional[Category] = None
         if self.config.hashtags_in_admin_chat:
             category_hashtag = None  # sentinel
             if self.category_store is not None:
-                category = await self.category_store.get_user_category(user)
                 if category is None:
                     if self.config.force_category_selection:
                         # see validate_service_messages
                         you_must_select_category = cast(AnyText, self.service_messages.you_must_select_category)
                         await user_replier(
                             any_text_to_str(you_must_select_category, language),
                             await self.category_store.markup_for_user(user),
@@ -472,36 +519,43 @@
                     hashtags = [self.config.unanswered_hashtag]
                 else:
                     hashtags = []
                 if category_hashtag is not None:
                     hashtags.append(category_hashtag)
 
                 if hashtags:
-                    # TODO: multiple categories per user support
-                    hashtag_msg = await bot.send_message(self.admin_chat_id, _join_hashtags(hashtags))
+                    hashtag_msg = await bot.send_message(
+                        self.admin_chat_id,
+                        _join_hashtags(hashtags),
+                        message_thread_id=message_thread_id,
+                    )
                     await self.user_related_messages_store.add(user.id, hashtag_msg.id, reset_ttl=False)
                     hashtag_msg_data = HashtagMessageData(message_id=hashtag_msg.id, hashtags=hashtags)
                     await self.recent_hashtag_message_for_user_store.save(user.id, hashtag_msg_data)
 
         if send_user_id_hash:
             user_id_hash = self.config.user_id_hash_func(user.id, self.bot_prefix)
             last_sent_user_id_hash = await self.last_sent_user_id_hash_store.load(self.CONST_KEY)
             if last_sent_user_id_hash is None or last_sent_user_id_hash != user_id_hash:
-                user_id_hash_msg = await bot.send_message(self.admin_chat_id, user_id_hash)
+                user_id_hash_msg = await bot.send_message(
+                    self.admin_chat_id,
+                    user_id_hash,
+                    message_thread_id=message_thread_id,
+                )
                 await self.last_sent_user_id_hash_store.save(self.CONST_KEY, user_id_hash)
                 await self.save_message_from_user(user, user_id_hash_msg.id)
 
         preforwarded_msg = None
         if self.config.before_forwarding is not None:
             preforwarded_msg = await self.config.before_forwarding(user)
             if isinstance(preforwarded_msg, tg.Message):
                 await self.save_message_from_user(user, preforwarded_msg.id)
 
         # admin_chat_forwarded_msg_id, user_content_message = await message_forwarder()
-        message_forwarder_result = await message_forwarder()
+        message_forwarder_result = await message_forwarder(message_thread_id)
         await self.save_message_from_user(user, message_forwarder_result.admin_chat_msg.id)
 
         postforwarded_msg = None
         if self.config.after_forwarding is not None:
             postforwarded_msg = await self.config.after_forwarding(user)
             if isinstance(postforwarded_msg, tg.Message):
                 await self.save_message_from_user(user, postforwarded_msg.id)
@@ -519,18 +573,14 @@
                 any_text_to_str(self.service_messages.forwarded_to_admin_ok, language),
                 None,
             )
             if self.config.confirm_forwarded_to_admin_rarer_than is not None:
                 await self.recently_sent_confirmation_flag_store.set_flag(user.id)
 
         if export_to_integrations:
-            # NOTE: category may already be loaded, if so -- reusing the value here
-            if category is None and self.category_store is not None:
-                category = await self.category_store.get_user_category(user)
-
             # integrations have no concept of pre- and post-forwarded messages, so we just patch their texts
             # to the admin chat msg; their attachments and other info is lost, which is fine because we don't
             # use them that often anymore
             if preforwarded_msg is not None:
                 message_forwarder_result.admin_chat_msg.text = (
                     "[pre]: "
                     + preforwarded_msg.text_content
@@ -584,19 +634,31 @@
         """Sometimes we want FeedbackHandler to act like the user has sent us a message, but without actually
         a message there (they might have pressed a button or interacted with the bot in some other way). This
         method can be used in such cases.
 
         If the message has been successfully sent to the admin chat, this method returns its id.
         """
 
-        async def message_forwarder() -> MessageForwarderResult:
+        async def message_forwarder(message_thread_id: Optional[int]) -> MessageForwarderResult:
             if attachment is None:
-                sent_msg = await bot.send_message(self.admin_chat_id, text=text, **send_message_kwargs)
+                sent_msg = await bot.send_message(
+                    self.admin_chat_id,
+                    text=text,
+                    message_thread_id=message_thread_id,
+                    **send_message_kwargs,
+                )
             else:
-                sent_msg = await send_attachment(bot, self.admin_chat_id, attachment, text, remove_exif_data)
+                sent_msg = await send_attachment(
+                    bot,
+                    self.admin_chat_id,
+                    attachment,
+                    text,
+                    remove_exif_data,
+                    message_thread_id=message_thread_id,
+                )
             return MessageForwarderResult(
                 admin_chat_msg=sent_msg,
                 user_msg=None,
             )
 
         async def user_replier(text: str, reply_markup: Optional[tg.ReplyMarkup]) -> Optional[tg.Message]:
             if no_response:
@@ -610,28 +672,32 @@
             message_forwarder=message_forwarder,
             user_replier=user_replier,
             send_user_id_hash=send_user_id_hash_message,
             export_to_integrations=export_to_trello,
         )
 
     async def handle_user_message(self, message: tg.Message, bot: AsyncTeleBot, reply_to_user: bool) -> Optional[int]:
-        async def message_forwarder() -> MessageForwarderResult:
+        async def message_forwarder(message_thread_id: Optional[int]) -> MessageForwarderResult:
             if self.config.full_user_anonymization:
                 copied_message_id = await bot.copy_message(
                     chat_id=self.admin_chat_id,
                     from_chat_id=message.chat.id,
                     message_id=message.id,
+                    message_thread_id=message_thread_id,
                 )
                 fake_admin_chat_message = copy.deepcopy(message)
                 fake_admin_chat_message.chat = await self.admin_chat()
                 fake_admin_chat_message.id = copied_message_id.message_id
                 return MessageForwarderResult(admin_chat_msg=fake_admin_chat_message, user_msg=message)
             else:
                 forwarded_message = await bot.forward_message(
-                    self.admin_chat_id, from_chat_id=message.chat.id, message_id=message.id
+                    self.admin_chat_id,
+                    from_chat_id=message.chat.id,
+                    message_id=message.id,
+                    message_thread_id=message_thread_id,
                 )
                 return MessageForwarderResult(admin_chat_msg=forwarded_message, user_msg=message)
 
         async def user_replier(text: str, reply_markup: Optional[tg.ReplyMarkup]):
             if reply_to_user:
                 return await bot.reply_to(message, text, reply_markup=reply_markup)
 
@@ -650,37 +716,43 @@
             chat_types=[tg_constants.ChatType.private],
             content_types=list(tg_constants.MediaContentType),
             priority=-100,  # lower priority to process the rest of the handlers first
         )
         async def handle_user_message(message: tg.Message) -> None:
             await self.handle_user_message(message, bot=bot, reply_to_user=True)
 
+        await self.setup_without_user_message_handler(bot)
+
+    async def setup_without_user_message_handler(self, bot: AsyncTeleBot) -> None:
         await self.setup_admin_chat_handlers(bot)
-        self.set_bot(bot)
+        self._bot = bot
         for integration in self.integrations:
             await integration.setup(bot)
-
-    def set_bot(self, bot: AsyncTeleBot) -> None:
-        self._bot = bot
+        if self.forum_topic_store is not None:
+            await self.forum_topic_store.setup(bot)
 
     async def aux_endpoints(self) -> list[AuxBotEndpoint]:
         endpoints: list[AuxBotEndpoint] = []
         for integration in self.integrations:
             endpoints.extend(await integration.aux_endpoints())
         return endpoints
 
     def background_jobs(
         self,
         base_url: Optional[str],
         server_listening_future: Optional[asyncio.Future[None]],
     ) -> list[Coroutine[None, None, None]]:
-        return [
+        integration_backgroung_jobs = [
             i.background_job(FeedbackIntegrationBackgroundContext(base_url, server_listening_future))
             for i in self.integrations
         ]
+        self_background_jobs: list[Coroutine[None, None, None]] = []
+        if self.forum_topic_store is not None:
+            self_background_jobs.append(self.forum_topic_store.background_job())
+        return self_background_jobs + integration_backgroung_jobs
 
     async def _remove_unanswered_hashtag(self, bot: AsyncTeleBot, message_id: int):
         if self.hashtag_message_for_forwarded_message_store is None:
             return
         hashtag_message_data = await self.hashtag_message_for_forwarded_message_store.load(message_id)
         if hashtag_message_data is None:
             return
@@ -731,21 +803,21 @@
             parse_mode="HTML",
         )
 
         await self.message_log_store.push(event.origin_chat_id, cloned_reply_message.id)
 
         if notify_integrations:
             # do not notify integration about its own replies
-            integrations_to_notify = [i for i in self.integrations if not i is event.integration]
+            integrations_to_notify = [i for i in self.integrations if i is not event.integration]
             self.logger.debug(f"Notifying integrations: {[i.name() for i in integrations_to_notify]}")
             await asyncio.gather(
                 *[integration.handle_user_message_replied_elsewhere(event) for integration in integrations_to_notify]
             )
         else:
-            self.logger.debug(f"Will not notify integrations")
+            self.logger.debug("Will not notify integrations")
 
     async def setup_admin_chat_handlers(
         self,
         bot: AsyncTeleBot,
         on_admin_reply_to_bot: Optional[Callable[[], Awaitable[None]]] = None,
     ) -> None:
         @bot.message_handler(chat_id=[self.admin_chat_id], commands=["help"])
@@ -821,35 +893,37 @@
                         try:
                             page_str = extract_arguments(message.text_content) or "1"
                             page = int(page_str)
                             if page > 0:
                                 page -= 1  # one based to zero based
                         except Exception:
                             await bot.reply_to(
-                                message, f"Bad command, expected format is '/log' or '/log <page number>'"
+                                message, "Bad command, expected format is '/log' or '/log <page number>'"
                             )
                             return
                         log_message_ids = await self.message_log_store.all(origin_chat_id)
                         total_pages = int(math.ceil(len(log_message_ids) / self.config.message_log_page_size))
                         if page < 0:
                             page = page % total_pages  # wrapping so that -1 = last, -2 = second to last, etc
                         start_idx = self.config.message_log_page_size * page
                         end_idx = self.config.message_log_page_size * (page + 1)
                         log_message_ids_page = log_message_ids[start_idx:end_idx]
                         self.logger.info(
-                            f"Forwarding log page {page} / {total_pages} (from {message.text_content!r}) received for origin chat id "
-                            + f"{origin_chat_id}, total messages: {len(log_message_ids)}, on current page: {len(log_message_ids_page)}"
+                            f"Forwarding log page {page} / {total_pages} (from {message.text_content!r}) "
+                            + f"received for origin chat id {origin_chat_id}, total messages: {len(log_message_ids)}, "
+                            + f"on current page: {len(log_message_ids_page)}"
                         )
                         if not log_message_ids_page:
                             if page == 0:
                                 await bot.reply_to(message, "Message log with this user is not available :(")
                             else:
                                 await bot.reply_to(
                                     message,
-                                    f"Only {len(log_message_ids)} messages are available in log, not enough messages for page {page}",
+                                    f"Only {len(log_message_ids)} messages are available in log, "
+                                    + f"not enough messages for page {page}",
                                 )
                             return
                         log_destination_chat_id = (
                             self.admin_chat_id if self.config.message_log_to_admin_chat else message.from_user.id
                         )
                         await bot.send_message(
                             chat_id=log_destination_chat_id,
@@ -935,12 +1009,12 @@
                                 )
                             )
                             for integration in self.integrations
                         ]
                     )
             except Exception as e:
                 await bot.reply_to(message, f"Something went wrong! {e}")
-                self.logger.exception(f"Unexpected error while replying to forwarded msg")
+                self.logger.exception("Unexpected error while replying to forwarded msg")
 
 
 def _join_hashtags(hashtags: list[str]) -> str:
     return " ".join(["#" + h for h in hashtags])
```

### Comparing `telebot_components-0.7.3/telebot_components/feedback/anti_spam.py` & `telebot_components-0.8.0/telebot_components/feedback/anti_spam.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/telebot_components/feedback/integration/aux_feedback_handler.py` & `telebot_components-0.8.0/telebot_components/feedback/integration/aux_feedback_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import copy
-import dataclasses
 import logging
 from typing import Optional
 
 from telebot import AsyncTeleBot
 from telebot import types as tg
 
 from telebot_components.feedback import FeedbackHandler, MessageForwarderResult
 from telebot_components.feedback.integration.interface import (
     FeedbackHandlerIntegration,
-    FeedbackIntegrationBackgroundContext,
     UserMessageRepliedFromIntegrationEvent,
 )
 from telebot_components.feedback.types import UserMessageRepliedEvent
 from telebot_components.redis_utils.interface import RedisInterface
 from telebot_components.stores.category import Category
 from telebot_components.stores.generic import KeyValueStore
 
@@ -46,15 +44,15 @@
             return
         # the terminology is reversed here, because for integration's POV, aux chat is main and vice versa
         aux_admin_chat_message_id = event.main_admin_chat_message_id
         main_admin_chat_message_id = await self.aux.main_by_aux_admin_chat_message_id_store.load(
             aux_admin_chat_message_id
         )
         if main_admin_chat_message_id is None:
-            self.logger.error(f"Message in aux admin chat has no saved main admin chat message id")
+            self.logger.error("Message in aux admin chat has no saved main admin chat message id")
             return
         await self.aux.message_replied_callback(
             UserMessageRepliedFromIntegrationEvent(
                 bot=event.bot,
                 origin_chat_id=event.origin_chat_id,
                 reply_text=event.reply_text,
                 reply_has_attachments=event.reply_has_attachments,
@@ -115,19 +113,20 @@
             )
             if aux_admin_message_id:  # if the message was actually sent to the aux admin chat
                 await self.main_by_aux_admin_chat_message_id_store.save(aux_admin_message_id, admin_chat_message.id)
                 await self.aux_by_main_admin_chat_message_id_store.save(admin_chat_message.id, aux_admin_message_id)
         else:
             # if we got no user message (e.g. the message in admin chat is emulated), we just clone the message
             # from the main admin chat to the aux one
-            async def message_forwarder() -> MessageForwarderResult:
+            async def message_forwarder(message_thread_id: Optional[int]) -> MessageForwarderResult:
                 copied_message = await bot.copy_message(
                     chat_id=self.feedback_handler.admin_chat_id,
                     from_chat_id=admin_chat_message.chat.id,
                     message_id=admin_chat_message.id,
+                    message_thread_id=message_thread_id,
                 )
                 await self.main_by_aux_admin_chat_message_id_store.save(
                     copied_message.message_id, admin_chat_message.id
                 )
                 await self.aux_by_main_admin_chat_message_id_store.save(
                     admin_chat_message.id, copied_message.message_id
                 )
@@ -149,15 +148,15 @@
             )
 
     async def handle_user_message_replied_elsewhere(self, event: UserMessageRepliedEvent) -> None:
         aux_admin_chat_message_id = await self.aux_by_main_admin_chat_message_id_store.load(
             event.main_admin_chat_message_id
         )
         if aux_admin_chat_message_id is None:
-            self.logger.error(f"Message in the main admin chat has no saved aux admin chat message id")
+            self.logger.error("Message in the main admin chat has no saved aux admin chat message id")
             return
         # from aux feedback handler's POV, aux admin chat msg id is main
         event.main_admin_chat_message_id = aux_admin_chat_message_id
 
         if not isinstance(event, UserMessageRepliedFromIntegrationEvent):
             event = UserMessageRepliedFromIntegrationEvent(
                 bot=event.bot,
@@ -169,9 +168,8 @@
                 main_admin_chat_message_id=event.main_admin_chat_message_id,
                 # this is fake _MainFeedbackHandlerIntegration inserted in __init__
                 integration=self.feedback_handler.integrations[0],
             )
         await self.feedback_handler.message_replied_from_integration_callback(event, notify_integrations=False)
 
     async def setup(self, bot: AsyncTeleBot) -> None:
-        await self.feedback_handler.setup_admin_chat_handlers(bot)
-        self.feedback_handler.set_bot(bot)
+        await self.feedback_handler.setup_without_user_message_handler(bot)
```

### Comparing `telebot_components-0.7.3/telebot_components/feedback/integration/interface.py` & `telebot_components-0.8.0/telebot_components/feedback/integration/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         category: Optional[Category],
         bot: AsyncTeleBot,
     ) -> None:
         """
         The method is invoked on all user messages (including emulated) passing through the feedback handler.
         - `admin_chat_message` is a message as it appears in the main admin chat, allows backlinking and other stuff
         - `user` is a original message author
-        - `user_message` is a message as it was originally sent by the user; not always available (e.g. emulated messages)
+        - `user_message` is a message as it was sent by the user; not always available (e.g. emulated messages)
         - `category` is a user category, if enabled in the main admin chat
         - `bot` is a bot
         """
         ...
 
     @abc.abstractmethod
     async def handle_user_message_replied_elsewhere(self, event: UserMessageRepliedEvent) -> None:
```

### Comparing `telebot_components-0.7.3/telebot_components/feedback/integration/trello.py` & `telebot_components-0.8.0/telebot_components/feedback/integration/trello.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,16 @@
     # Trello board url has form https://trello.com/b/<board-id>/some-human-readable-name
     board_id: Optional[str] = None
 
     def __post_init__(self) -> None:
         if self.board_id is not None:
             if not (self.organization_name is None and self.board_name is None):
                 raise ValueError(
-                    "Legacy Trello board lookup config (organization and board name) can't be used together with board id"
+                    "Legacy Trello board lookup config (organization and board name) "
+                    "can't be used together with board id"
                 )
         else:
             if self.organization_name is None or self.board_name is None:
                 raise ValueError(
                     "At least one board lookup name must be specified: board id or organization and board name (legacy)"
                 )
 
@@ -202,16 +203,16 @@
             raise RuntimeError("TrelloIntegration was not properly initialized: self._bot is not set")
         return self._bot
 
     def help_message_section(self) -> str:
         trello_help = "🗂️ <i>Интеграция с Trello</i>\n"
         trello_help += (
             f'· Помимо чата сообщения выгружаются на {html_link(self.board.url, "доску Trello")} '
-            + f"в списки: "
-            + ", ".join(f"<b>{l.name}</b>" for l in self.lists_by_category_name.values())
+            + "в списки: "
+            + ", ".join(f"<b>{lst.name}</b>" for lst in self.lists_by_category_name.values())
             + "\n"
             "· В карточки переносятся присланные в бот фотографии и документы. Для каждого сообщения доступна "
             + "обратная ссылка на этот чат."
         )
         if self.reply_with_card_comments:
             trello_help += (
                 "\n"
@@ -259,15 +260,15 @@
                     f"Board not found in the {organization.name!r} organization: {self.credentials.board_name!r}"
                 )
             if len(matching_boards) > 1:
                 raise TrelloIntegrationCredentialsError(f"Ambiguous board name, several found: {matching_boards}")
             self.board = matching_boards[0]
 
         lists_on_board = await loop.run_in_executor(self.thread_pool, self.board.all_lists)
-        lists_by_name: dict[str, trello.List] = {l.name: l for l in lists_on_board}
+        lists_by_name: dict[str, trello.List] = {lst.name: lst for lst in lists_on_board}
         self.lists_by_category_name: dict[str, trello.List] = dict()
 
         for category in self.categories:
             if category.name in lists_by_name:
                 list_ = lists_by_name[category.name]
             else:
                 self.logger.info(f"Creating new list '{category.name}'")
@@ -589,15 +590,15 @@
             try:
                 trello_card = await self._append_card_content(
                     card_id=existing_trello_card_data["id"],
                     content=card_content,
                     user_id=user.id,
                 )
             except Exception:
-                self.logger.exception(f"Unexpected error appending card content, will try creating a new one")
+                self.logger.exception("Unexpected error appending card content, will try creating a new one")
                 new_card_reason = "error occured appending to existing card"
         elif existing_trello_card_data is None:
             new_card_reason = "no saved card data found for the user"
         else:
             new_card_reason = "user category has changed"
 
         if trello_card is None:
@@ -744,15 +745,15 @@
         except trello.ResourceUnavailable:
             self.logger.debug(f"Error removing label {label.id} from card {trello_card.id}, ignoring", exc_info=True)
 
 
 def safe_markdownify(html_text: str, fallback_text: str) -> str:
     try:
         md: str = markdownify(html_text)
-        md = md.replace("#", "\#")
+        md = md.replace("#", r"\#")
         return md
     except Exception:
         return fallback_text + "\n⚠️ Не удалось отобразить часть текста, оригинал сообщения по ссылке."
 
 
 def concatenate_card_text_sections(first: str, second: str) -> str:
     if not first:
```

### Comparing `telebot_components-0.7.3/telebot_components/form/field.py` & `telebot_components-0.8.0/telebot_components/form/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,16 @@
     possible_next_field_names: list[Optional[str]]
     # filled on Form object initialization
     fields_by_name: Optional[Dict[str, "FormField"]] = None
 
     async def __call__(self, user: tg.User, value: Optional[FieldValueT]) -> Optional["FormField"]:
         if self.fields_by_name is None:
             raise RuntimeError(
-                "Next field getter hasn't been properly initialized, did you forget to pass your fields in a Form object?"
+                "Next field getter hasn't been properly initialized, "
+                + "did you forget to pass your fields in a Form object?"
             )
         next_field_name = self.next_field_name_getter(user, value)
         if next_field_name is None:
             return None
         else:
             return self.fields_by_name[next_field_name]
 
@@ -567,18 +568,18 @@
                         f"Error parsing callback payload {callback_payload!r} as Enum value {list(self.EnumClass)}"
                     )
                 new_value = copy.deepcopy(current_value)
                 if selected_option in new_value:
                     new_value.remove(selected_option)
                 else:
                     new_value.add(selected_option)
-                selected_option_page = list(self.EnumClass).index(selected_option) // self.options_per_page  # type: ignore
+                page = list(self.EnumClass).index(selected_option) // self.options_per_page  # type: ignore
                 return CallbackProcessingResult(
                     response_to_user=None,
-                    updated_inline_markup=self.get_reply_markup(language, new_value, selected_option_page),
+                    updated_inline_markup=self.get_reply_markup(language, new_value, page),
                     complete_field=False,
                     new_field_value=new_value,
                 )
             else:
                 raise ValueError(f"Unknown callback payload prefix: {callback_payload!r}!")
         except Exception as e:
             logger.exception("Unexpected error processing callback query")
```

### Comparing `telebot_components-0.7.3/telebot_components/form/form.py` & `telebot_components-0.8.0/telebot_components/form/form.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/telebot_components/form/handler.py` & `telebot_components-0.8.0/telebot_components/form/handler.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/telebot_components/form/helpers/calendar_keyboard.py` & `telebot_components-0.8.0/telebot_components/form/helpers/calendar_keyboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             if self.year is None or self.month is None or self.day is None:
                 raise RuntimeError(
                     "All fields must be specified for SELECT action, but "
                     + f"{self.year = } {self.month = } {self.day = }"
                 )
         if self.action is CalendarAction.UPDATE:
             if self.year is None or self.month is None:
-                raise RuntimeError(f"Year and month must be specified for UPDATE action")
+                raise RuntimeError("Year and month must be specified for UPDATE action")
 
     def dump(self) -> str:
         parts: list[str] = [self.action.value]
         if self.year is not None:
             parts.append(f"y{self.year}")
         if self.month is not None:
             parts.append(f"m{self.month}")
```

### Comparing `telebot_components-0.7.3/telebot_components/menu/menu.py` & `telebot_components-0.8.0/telebot_components/menu/menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from dataclasses import dataclass
-from typing import Awaitable, Callable, Coroutine, Optional
+from typing import Awaitable, Callable, Optional
 
 from telebot import AsyncTeleBot
 from telebot import types as tg
 from telebot.api import ApiHTTPException
 from telebot.callback_data import CallbackData
 
 from telebot_components.stores.category import Category, CategoryStore
@@ -197,15 +197,16 @@
         self.menu_by_id: dict[str, Menu] = {m.id: m for m in self.menus_list}
 
         self.menu_items_list = self.init_item_ids_and_get_item_list()
         menu_items_with_bound_categories = [mi for mi in self.menu_items_list if mi.bound_category is not None]
         if menu_items_with_bound_categories:
             if self.category_store is None:
                 raise ValueError(
-                    f"Menu items have bound categories, but category store is not passed to MenuHandler: {menu_items_with_bound_categories}"
+                    "Menu items have bound categories, but category store "
+                    + f"is not passed to MenuHandler: {menu_items_with_bound_categories}"
                 )
             menu_items_with_non_storable_categories = [
                 mi
                 for mi in menu_items_with_bound_categories
                 if mi.bound_category and not self.category_store.is_storable(mi.bound_category)
             ]
             if menu_items_with_non_storable_categories:
@@ -313,8 +314,8 @@
                 try:
                     await bot.edit_message_reply_markup(
                         chat_id=user.id,
                         message_id=call.message.id,
                         reply_markup=current_menu.get_inactive_keyboard_markup(selected_menu_item_id),
                     )
                 except ApiHTTPException:
-                    self.logger.info(f"Error editing message reply markup", exc_info=True)
+                    self.logger.info("Error editing message reply markup", exc_info=True)
```

### Comparing `telebot_components-0.7.3/telebot_components/redis_utils/emulation.py` & `telebot_components-0.8.0/telebot_components/redis_utils/emulation.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/telebot_components/redis_utils/interface.py` & `telebot_components-0.8.0/telebot_components/redis_utils/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 from abc import ABC, abstractmethod
-from typing import Mapping, Optional, TypeVar, Union
+from typing import Mapping, Optional, Union
 
 # type defs copied from redis
 
 
 class RedisInterface(ABC):
     """Abstract interface for the parts of redis.asyncio.Redis class we're using;
     please update when utilizing new methods.
```

### Comparing `telebot_components-0.7.3/telebot_components/stores/banned_users.py` & `telebot_components-0.8.0/telebot_components/stores/banned_users.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/telebot_components/stores/category.py` & `telebot_components-0.8.0/telebot_components/stores/category.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import logging
-import re
 from dataclasses import dataclass
 from datetime import timedelta
 from typing import Awaitable, Callable, Optional
 
+from async_lru import alru_cache
 from telebot import AsyncTeleBot
 from telebot import types as tg
 from telebot.callback_data import CallbackData
 
 from telebot_components.redis_utils.interface import RedisInterface
 from telebot_components.stores.generic import KeyValueStore
 from telebot_components.stores.language import (
     AnyText,
-    Language,
     LanguageStore,
     MaybeLanguage,
     any_text_to_str,
     vaildate_singlelang_text,
 )
 from telebot_components.stores.types import OnOptionSelected
 from telebot_components.stores.utils import callback_query_processing_error
 
 
-@dataclass
+@dataclass(frozen=True)
 class Category:
     name: str
     button_caption: Optional[AnyText] = None
     hashtag: Optional[str] = None
-    hidden: bool = False  # hide category from menu for new users while keeping them for those who already selected it
+    # hides category from menu for new users while keeping them for those who already selected it
+    hidden: bool = False
 
     def get_localized_button_caption(self, language: MaybeLanguage) -> str:
         return any_text_to_str(self.button_caption, language) if self.button_caption is not None else self.name
 
 
 @dataclass
 class CategorySelectedContext:
@@ -89,22 +89,24 @@
 
     def is_storable(self, category: Category) -> bool:
         return category.name in self.categories_by_name
 
     async def save_user_category(self, user: tg.User, category: Category) -> bool:
         if category.name not in self.categories_by_name:
             self.logger.warning("Saving category that has not been passed to the store on initialization")
+        self.get_user_category.cache_invalidate(user)
         result = await self.user_category_store.save(user.id, category)
         if self.on_category_selected is not None:
             try:
                 await self.on_category_selected(CategorySelectedContext(category, user, None, None))
             except Exception:
                 self.logger.exception("Error in on_category_selected callback")
         return result
 
+    @alru_cache(maxsize=1_000_000)
     async def get_user_category(self, user: tg.User) -> Optional[Category]:
         return await self.user_category_store.load(user.id) or self.default_category
 
     def setup(self, bot: AsyncTeleBot, on_category_selected: Optional[OnOptionSelected[Category]] = None):
         if on_category_selected is not None:
             if self.on_category_selected is not None:
                 raise RuntimeError(
@@ -134,15 +136,15 @@
             if category is None:
                 await callback_query_processing_error(
                     bot, call, f"unknown category name: {category_name}", self.logger, error_level=False
                 )
                 return
             category_saved = await self.save_user_category(user, category)
             if not category_saved:
-                await callback_query_processing_error(bot, call, f"unable to save category", self.logger)
+                await callback_query_processing_error(bot, call, "unable to save category", self.logger)
                 return
             try:
                 await bot.answer_callback_query(call.id)
                 await bot.edit_message_reply_markup(
                     user.id, call.message.id, reply_markup=(await self.markup_for_user(call.from_user))
                 )
             except Exception:
```

### Comparing `telebot_components-0.7.3/telebot_components/stores/generic.py` & `telebot_components-0.8.0/telebot_components/stores/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,13 @@
 import json
 import logging
 from dataclasses import dataclass
 from datetime import timedelta
 from hashlib import md5
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    ClassVar,
-    Generic,
-    Optional,
-    Protocol,
-    TypeVar,
-    cast,
-)
+from typing import Callable, ClassVar, Generic, Optional, Protocol, TypeVar, cast
 
 import tenacity
 
 from telebot_components.constants.times import MONTH
 from telebot_components.redis_utils.interface import RedisInterface
 
 T = TypeVar("T")
```

### Comparing `telebot_components-0.7.3/telebot_components/stores/language.py` & `telebot_components-0.8.0/telebot_components/stores/language.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,18 +65,18 @@
 
 
 def any_text_to_str(t: AnyText, language: MaybeLanguage) -> str:
     if language is None:
         if isinstance(t, str):
             return t
         else:
-            raise ValueError(f"MultilangText requires a valid Language for localisation")
+            raise ValueError("MultilangText requires a valid Language for localisation")
     else:
         if isinstance(t, str):
-            raise ValueError(f"Plain string text requires language=None")
+            raise ValueError("Plain string text requires language=None")
         else:
             localised_t = t.get(language)
             if not isinstance(localised_t, str):
                 raise ValueError(f"No valid localisation found for language '{language}'")
             return localised_t
 
 
@@ -144,15 +144,15 @@
 
             if language not in self.languages:
                 await callback_query_processing_error(bot, call, f"language '{language}' is not supported", self.logger)
                 return
 
             language_saved = await self.set_user_language(user, language)
             if not language_saved:
-                await callback_query_processing_error(bot, call, f"unable to save selected language", self.logger)
+                await callback_query_processing_error(bot, call, "unable to save selected language", self.logger)
                 return
             try:
                 await bot.answer_callback_query(call.id)
                 await bot.edit_message_reply_markup(
                     user.id, call.message.id, reply_markup=self.markup_for_selected_language(language)
                 )
             except Exception:
```

### Comparing `telebot_components-0.7.3/telebot_components/stores/user_group.py` & `telebot_components-0.8.0/telebot_components/stores/user_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import functools
 import logging
-from typing import Any, Awaitable, Callable, Coroutine, Optional
+from typing import Any, Awaitable, Callable, Optional, TypeVar
 
 from telebot import AsyncTeleBot, invoke_handler
 from telebot import types as tg
 from telebot.types.service import HandlerFunction
 
 from telebot_components.redis_utils.interface import RedisInterface
 from telebot_components.stores.generic import SetStore
 
 logger = logging.getLogger(__name__)
 
 
-unity = lambda x: x
+ArgT = TypeVar("ArgT")
+
+
+def unity(x: ArgT) -> ArgT:
+    return x
 
 
 async def telegram_user_id_identity(user: tg.User) -> str:
     return str(user.id)
 
 
 class UserGroupStore:
@@ -64,15 +68,15 @@
             return await self.is_member_by_identity(uid)
         except Exception:
             return False
 
     def membership_required(self, bot: AsyncTeleBot, membership_required_reply_text: Optional[str] = None):
         def decorator(handler_func: HandlerFunction[tg.Message]) -> HandlerFunction[tg.Message]:
             @functools.wraps(handler_func)
-            async def wrapped(*args) -> None:
+            async def wrapped(*args) -> Any:
                 try:
                     message: tg.Message = args[0]
                     if await self.is_member(message.from_user):
                         return await invoke_handler(handler_func, message, bot)
                     else:
                         if membership_required_reply_text:
                             await bot.send_message(message.from_user.id, membership_required_reply_text)
```

### Comparing `telebot_components-0.7.3/telebot_components/stores/utils.py` & `telebot_components-0.8.0/telebot_components/stores/utils.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/telebot_components/utils/__init__.py` & `telebot_components-0.8.0/telebot_components/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         current_len += len(word) + 1
         if current_len > target_len:
             return " ".join(words) + "..."
     return message
 
 
 def join_paragraphs(lines: list[str]) -> str:
-    return "\n\n".join([l for l in lines if l])
+    return "\n\n".join([line for line in lines if line])
 
 
 yaml = YAML(typ="unsafe")
 
 
 def to_yaml_unsafe(obj: Any) -> str:
     in_memory_stream = io.StringIO()
@@ -148,37 +148,59 @@
 
 async def send_attachment(
     bot: AsyncTeleBot,
     chat_id: Union[int, str],
     attachment: TelegramAttachment,
     caption: Optional[str] = None,
     remove_metadata: bool = True,
+    message_thread_id: Optional[int] = None,
 ):
     if isinstance(attachment, list) and all(isinstance(att, tg.PhotoSize) for att in attachment):
-        return await bot.send_photo(chat_id, photo=attachment[0].file_id, caption=caption)
+        return await bot.send_photo(
+            chat_id,
+            photo=attachment[0].file_id,
+            caption=caption,
+            message_thread_id=message_thread_id,
+        )
     elif isinstance(attachment, tg.Document):
         doc_to_send: Union[str, bytes]
 
         if (attachment.mime_type == "image/jpeg" or attachment.mime_type == "image/png") and remove_metadata:
             doc_to_send = await download_photo_document_and_remove_metadata(bot, attachment)
         else:
             doc_to_send = attachment.file_id
 
         return await bot.send_document(
             chat_id,
             document=doc_to_send,
             caption=caption,
             visible_file_name=attachment.file_name,
+            message_thread_id=message_thread_id,
         )
     elif isinstance(attachment, tg.Video):
-        return await bot.send_video(chat_id, video=attachment.file_id, caption=caption)
+        return await bot.send_video(
+            chat_id,
+            video=attachment.file_id,
+            caption=caption,
+            message_thread_id=message_thread_id,
+        )
     elif isinstance(attachment, tg.Animation):
-        return await bot.send_animation(chat_id, animation=attachment.file_id, caption=caption)
+        return await bot.send_animation(
+            chat_id,
+            animation=attachment.file_id,
+            caption=caption,
+            message_thread_id=message_thread_id,
+        )
     elif isinstance(attachment, tg.Audio):
-        return await bot.send_audio(chat_id, audio=attachment.file_id, caption=caption)
+        return await bot.send_audio(
+            chat_id,
+            audio=attachment.file_id,
+            caption=caption,
+            message_thread_id=message_thread_id,
+        )
     else:
         raise TypeError(f"Can not send attachment of type: {type(attachment)!r}.")
 
 
 async def download_photo_document_and_remove_metadata(bot: AsyncTeleBot, document: tg.Document) -> Union[bytes, str]:
     if document.mime_type != "image/jpeg" and document.mime_type != "image/png":
         logger.exception(
```

### Comparing `telebot_components-0.7.3/telebot_components/utils/airtable.py` & `telebot_components-0.8.0/telebot_components/utils/airtable.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/telebot_components/utils/alerts.py` & `telebot_components-0.8.0/telebot_components/utils/alerts.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/telebot_components/utils/strings.py` & `telebot_components-0.8.0/telebot_components/utils/strings.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.7.3/PKG-INFO` & `telebot_components-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: telebot-components
-Version: 0.7.3
+Version: 0.8.0
 Summary: Framework/toolkit for building Telegram bots with telebot and redis
 Home-page: https://github.com/bots-against-war/telebot-components
 License: GPLv3
 Author: Igor Vaiman
 Author-email: gosha.vaiman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
+Requires-Dist: async-lru (>=2.0.2,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: markdownify (>=0.11.2,<0.12.0)
 Requires-Dist: py-trello (>=0.18.0,<0.19.0)
 Requires-Dist: pyairtable (>=1.3.0,<2.0.0)
 Requires-Dist: pytest-mock (>=3.7.0,<4.0.0)
 Requires-Dist: redis (>=4.3.1,<5.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
-Requires-Dist: telebot-against-war (>=0.6.0,<0.7.0)
+Requires-Dist: telebot-against-war (>=0.6.3,<0.7.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Project-URL: Repository, https://github.com/bots-against-war/telebot-components
 Description-Content-Type: text/markdown
 
 # telebot-components
 
 Framework / toolkit for building bots with [telebot](https://github.com/bots-against-war/telebot).
```

