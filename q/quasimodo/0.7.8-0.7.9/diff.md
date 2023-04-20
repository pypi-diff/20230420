# Comparing `tmp/quasimodo-0.7.8.tar.gz` & `tmp/quasimodo-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasimodo-0.7.8.tar", max compression
+gzip compressed data, was "quasimodo-0.7.9.tar", max compression
```

## Comparing `quasimodo-0.7.8.tar` & `quasimodo-0.7.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      559 2022-12-03 08:07:55.020341 quasimodo-0.7.8/pyproject.toml
--rw-r--r--   0        0        0      264 2022-05-15 09:06:35.496391 quasimodo-0.7.8/quasimodo/__init__.py
--rw-r--r--   0        0        0    15380 2022-11-07 22:38:36.221016 quasimodo-0.7.8/quasimodo/amqp.py
--rw-r--r--   0        0        0     4350 2022-06-08 16:49:13.408271 quasimodo-0.7.8/quasimodo/base.py
--rw-r--r--   0        0        0     6998 2022-06-08 17:06:19.985612 quasimodo-0.7.8/quasimodo/hunchback.py
--rw-r--r--   0        0        0     4412 2022-09-08 19:57:39.613782 quasimodo-0.7.8/quasimodo/mqtt_websocket.py
--rw-r--r--   0        0        0     1419 2020-05-24 05:24:46.684250 quasimodo-0.7.8/quasimodo/stubs.py
--rw-r--r--   0        0        0      783 2022-12-03 08:08:35.942264 quasimodo-0.7.8/setup.py
--rw-r--r--   0        0        0      529 2022-12-03 08:08:35.942526 quasimodo-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0      559 2023-04-20 11:57:32.253677 quasimodo-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0      264 2022-05-15 09:06:35.496391 quasimodo-0.7.9/quasimodo/__init__.py
+-rw-r--r--   0        0        0    15380 2022-11-07 22:38:36.221016 quasimodo-0.7.9/quasimodo/amqp.py
+-rw-r--r--   0        0        0     4350 2022-06-08 16:49:13.408271 quasimodo-0.7.9/quasimodo/base.py
+-rw-r--r--   0        0        0     7163 2023-04-20 12:02:59.969159 quasimodo-0.7.9/quasimodo/hunchback.py
+-rw-r--r--   0        0        0     4493 2023-04-20 11:58:30.844422 quasimodo-0.7.9/quasimodo/mqtt_websocket.py
+-rw-r--r--   0        0        0     1419 2020-05-24 05:24:46.684250 quasimodo-0.7.9/quasimodo/stubs.py
+-rw-r--r--   0        0        0      783 2023-04-20 12:04:43.621278 quasimodo-0.7.9/setup.py
+-rw-r--r--   0        0        0      529 2023-04-20 12:04:43.621532 quasimodo-0.7.9/PKG-INFO
```

### Comparing `quasimodo-0.7.8/pyproject.toml` & `quasimodo-0.7.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quasimodo"
-version = "0.7.8"
+version = "0.7.9"
 description = "AMQP and MQTT over WebSocket Queue Clients"
 authors = ["doubleO8 <wb008@hdm-stuttgart.de>"]
 license = "GPL"
 
 [tool.poetry.dependencies]
 python = ">=3.7.3,<4.0"
 pika = "^1.2.1"
```

### Comparing `quasimodo-0.7.8/quasimodo/amqp.py` & `quasimodo-0.7.9/quasimodo/amqp.py`

 * *Files identical despite different names*

### Comparing `quasimodo-0.7.8/quasimodo/base.py` & `quasimodo-0.7.9/quasimodo/base.py`

 * *Files identical despite different names*

### Comparing `quasimodo-0.7.8/quasimodo/hunchback.py` & `quasimodo-0.7.9/quasimodo/hunchback.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,20 @@
     connection_group.add_argument(
         "--listen",
         dest="binding_keys",
         default=[],
         action="append",
         help="Subscriptions",
     )
+    connection_group.add_argument(
+        "--client_id",
+        dest="client_id",
+        default=None,
+        help="Client ID to be used when connecting",
+    )
 
     amqp_group = parser.add_argument_group("AMQP Connection Options")
     amqp_group_queue = amqp_group.add_mutually_exclusive_group()
     env_key_queue = "QUASIMODO_QUEUE"
     env_key_exchange = "QUASIMODO_EXCHANGE"
     amqp_group_queue.add_argument(
         "--queue",
```

### Comparing `quasimodo-0.7.8/quasimodo/mqtt_websocket.py` & `quasimodo-0.7.9/quasimodo/mqtt_websocket.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,22 +21,25 @@
 
     def __init__(self, *args, **kwargs):
         quasimodo.base.Q.__init__(self, *args, **kwargs)
         self.log = logging.getLogger(__name__)
 
         self.endpoint = kwargs.get("endpoint", getattr(self, "DEFAULT_ENDPOINT"))
         self.heartbeat_interval = kwargs.get("heartbeat_interval", 60)
-        agent_id = str(uuid.uuid4())
+        client_id = kwargs.get("client_id")
+
+        if client_id is None:
+            client_id = str(uuid.uuid4())
 
         self.exchange_binding_keys = kwargs.get("binding_keys")
 
         self.connected = False
         if self.transport is None:
             self.transport = "websockets"
-        self.client = Client(client_id=agent_id, transport=self.transport)
+        self.client = Client(client_id=client_id, transport=self.transport)
         self.client.ws_set_options(self.endpoint)
         self.client.on_connect = self.__on_connect
         self.client.on_message = self.callback
         self.client.on_subscribe = self.__on_subscribe
 
         self.client.username_pw_set(self.credentials[0], self.credentials[1])
```

### Comparing `quasimodo-0.7.8/quasimodo/stubs.py` & `quasimodo-0.7.9/quasimodo/stubs.py`

 * *Files identical despite different names*

### Comparing `quasimodo-0.7.8/setup.py` & `quasimodo-0.7.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['paho-mqtt>=1.6.1,<2.0.0', 'pika>=1.2.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['quasimonkey = quasimodo.hunchback:hunchback_client']}
 
 setup_kwargs = {
     'name': 'quasimodo',
-    'version': '0.7.8',
+    'version': '0.7.9',
     'description': 'AMQP and MQTT over WebSocket Queue Clients',
     'long_description': None,
     'author': 'doubleO8',
     'author_email': 'wb008@hdm-stuttgart.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `quasimodo-0.7.8/PKG-INFO` & `quasimodo-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quasimodo
-Version: 0.7.8
+Version: 0.7.9
 Summary: AMQP and MQTT over WebSocket Queue Clients
 License: GPL
 Author: doubleO8
 Author-email: wb008@hdm-stuttgart.de
 Requires-Python: >=3.7.3,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

