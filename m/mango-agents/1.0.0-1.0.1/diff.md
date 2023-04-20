# Comparing `tmp/mango-agents-1.0.0.tar.gz` & `tmp/mango-agents-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-agents-1.0.0.tar", last modified: Thu Apr  6 08:12:11 2023, max compression
+gzip compressed data, was "mango-agents-1.0.1.tar", last modified: Thu Apr 20 09:23:20 2023, max compression
```

## Comparing `mango-agents-1.0.0.tar` & `mango-agents-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 08:12:11.353723 mango-agents-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-06 08:11:42.000000 mango-agents-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8272 2023-04-06 08:12:11.353723 mango-agents-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 08:12:11.340722 mango-agents-1.0.0/mango/
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 08:12:11.341722 mango-agents-1.0.0/mango/agent/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17621 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/agent/core.py
--rw-rw-rw-   0 root         (0) root         (0)    15150 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/agent/role.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 08:12:11.344722 mango-agents-1.0.0/mango/container/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/container/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10472 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/container/core.py
--rw-rw-rw-   0 root         (0) root         (0)     8977 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/container/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     5557 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/container/mosaik.py
--rw-rw-rw-   0 root         (0) root         (0)    10900 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/container/mqtt.py
--rw-rw-rw-   0 root         (0) root         (0)     4486 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/container/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     4350 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/container/tcp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 08:12:11.346722 mango-agents-1.0.0/mango/messages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/messages/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14633 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/messages/acl_message_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10753 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/messages/codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     6006 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/messages/message.py
--rw-rw-rw-   0 root         (0) root         (0)     2686 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/messages/other_proto_msgs_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 08:12:11.348722 mango-agents-1.0.0/mango/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2590 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/modules/base_module.py
--rw-rw-rw-   0 root         (0) root         (0)     4167 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/modules/mqtt_module.py
--rw-rw-rw-   0 root         (0) root         (0)     4180 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/modules/rabbit_module.py
--rw-rw-rw-   0 root         (0) root         (0)     2827 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/modules/zero_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 08:12:11.350722 mango-agents-1.0.0/mango/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2670 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/util/clock.py
--rw-rw-rw-   0 root         (0) root         (0)     4199 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/util/distributed_clock.py
--rw-rw-rw-   0 root         (0) root         (0)    26401 2023-04-06 08:11:42.000000 mango-agents-1.0.0/mango/util/scheduling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 08:12:11.352723 mango-agents-1.0.0/mango_agents.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8272 2023-04-06 08:12:11.000000 mango-agents-1.0.0/mango_agents.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      852 2023-04-06 08:12:11.000000 mango-agents-1.0.0/mango_agents.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 08:12:11.000000 mango-agents-1.0.0/mango_agents.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-06 08:12:11.000000 mango-agents-1.0.0/mango_agents.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-06 08:12:11.000000 mango-agents-1.0.0/mango_agents.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 08:12:11.353723 mango-agents-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4079 2023-04-06 08:11:42.000000 mango-agents-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.700207 mango-agents-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-20 09:22:58.000000 mango-agents-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8272 2023-04-20 09:23:20.700207 mango-agents-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.688206 mango-agents-1.0.1/mango/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.689206 mango-agents-1.0.1/mango/agent/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17913 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/agent/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    15150 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/agent/role.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.692206 mango-agents-1.0.1/mango/container/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10475 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     8981 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5557 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/mosaik.py
+-rw-rw-rw-   0 root         (0) root         (0)     9654 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/mqtt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     4343 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/container/tcp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.694207 mango-agents-1.0.1/mango/messages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/messages/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14633 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/messages/acl_message_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10753 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/messages/codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     6006 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/messages/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     2686 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/messages/other_proto_msgs_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.696207 mango-agents-1.0.1/mango/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2591 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/modules/base_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     4167 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/modules/mqtt_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     4180 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/modules/rabbit_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     2827 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/modules/zero_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.698207 mango-agents-1.0.1/mango/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2670 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/util/clock.py
+-rw-rw-rw-   0 root         (0) root         (0)     4211 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/util/distributed_clock.py
+-rw-rw-rw-   0 root         (0) root         (0)    26401 2023-04-20 09:22:58.000000 mango-agents-1.0.1/mango/util/scheduling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:23:20.700207 mango-agents-1.0.1/mango_agents.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8272 2023-04-20 09:23:20.000000 mango-agents-1.0.1/mango_agents.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      852 2023-04-20 09:23:20.000000 mango-agents-1.0.1/mango_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 09:23:20.000000 mango-agents-1.0.1/mango_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-20 09:23:20.000000 mango-agents-1.0.1/mango_agents.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-20 09:23:20.000000 mango-agents-1.0.1/mango_agents.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 09:23:20.701207 mango-agents-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4079 2023-04-20 09:22:58.000000 mango-agents-1.0.1/setup.py
```

### Comparing `mango-agents-1.0.0/LICENSE` & `mango-agents-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/PKG-INFO` & `mango-agents-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-agents
-Version: 1.0.0
+Version: 1.0.1
 Summary: Modular Python Agent Framework
 Author: mango Team
 Author-email: mango@offis.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mango-agents-1.0.0/mango/agent/core.py` & `mango-agents-1.0.1/mango/agent/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,25 @@
 
 
 class AgentDelegates:
     def __init__(self, context, scheduler) -> None:
         self._context: AgentContext = context
         self._scheduler: Scheduler = scheduler
 
+    @property
+    def current_timestamp(self) -> float:
+        """
+        Method that returns the current unix timestamp given the clock within the container
+        """
+        return self._context.current_timestamp
+
+    @property
+    def addr(self):
+        return self._context.addr
+
     async def send_message(
         self,
         content,
         receiver_addr: Union[str, Tuple[str, int]],
         receiver_id: Optional[str] = None,
         **kwargs,
     ):
@@ -417,15 +428,15 @@
 
         super().__init__(context, scheduler)
 
         self._check_inbox_task = asyncio.create_task(self._check_inbox())
         self._check_inbox_task.add_done_callback(self.raise_exceptions)
         self._stopped = asyncio.Future()
 
-        logger.info(f"Agent {self.aid}: start running in container {container.addr}")
+        logger.info("Agent %s: start running in container %s", self.aid, self.addr)
 
     def raise_exceptions(self, fut: asyncio.Future):
         """
         Inline function used as a callback to raise exceptions
         :param fut: The Future object of the task
         """
         if fut.exception() is not None:
@@ -433,19 +444,19 @@
                 f"Agent {self.aid}: Caught the following exception in _check_inbox: {fut.exception()}"
             )
             raise fut.exception()
 
     async def _check_inbox(self):
         """Task for waiting on new message in the inbox"""
 
-        logger.debug(f"Agent {self.aid}: Start waiting for messages")
+        logger.debug("Agent %s: Start waiting for messages", self.aid)
         while True:
             # run in infinite loop until it is cancelled from outside
             message = await self.inbox.get()
-            logger.debug(f"Agent {self.aid}: Received message;{message}")
+            logger.debug("Agent %s: Received message;%s", self.aid, message)
 
             # message should be tuples of (priority, content, meta)
             priority, content, meta = message
             meta["priority"] = priority
             
             self.handle_message(content=content, meta=meta)
 
@@ -476,8 +487,8 @@
             self._check_inbox_task.cancel()
             await self._check_inbox_task
 
             await self._scheduler.stop()
         except asyncio.CancelledError:
             pass
         finally:
-            logger.info(f"Agent {self.aid}: Shutdown successful")
+            logger.info("Agent %s: Shutdown successful", self.aid)
```

### Comparing `mango-agents-1.0.0/mango/agent/role.py` & `mango-agents-1.0.1/mango/agent/role.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/mango/container/core.py` & `mango-agents-1.0.1/mango/container/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 AGENT_PATTERN_NAME_PRE = "agent"
 
 
 class Container(ABC):
     """Superclass for a mango container"""
 
     def __init__(
-        self, *, addr, name: str, codec, loop, clock: Clock, copy_internal_messages=True
+        self, *, addr, name: str, codec, loop, clock: Clock, copy_internal_messages=False
     ):
         self.name: str = name
         self.addr = addr
         self.clock = clock
         self._copy_internal_messages = copy_internal_messages
 
         self.codec: Codec = codec
@@ -74,15 +74,15 @@
             or self.__check_agent_aid_pattern_match(suggested_aid)
         ):
             aid = f"{AGENT_PATTERN_NAME_PRE}{self._aid_counter}"
             self._aid_counter += 1
         else:
             aid = suggested_aid
         self._agents[aid] = agent
-        logger.info(f"Successfully registered agent;{aid}")
+        logger.info("Successfully registered agent;%s", aid)
         return aid
 
     def deregister_agent(self, aid):
         """
         Deregister an agent
         :param aid:
         :return:
@@ -257,15 +257,15 @@
             f"Received message with content and meta;{str(content)};{str(meta)}"
         )
         receiver_id = meta.get("receiver_id", None)
         if receiver_id and receiver_id in self._agents.keys():
             receiver = self._agents[receiver_id]
             await receiver.inbox.put((priority, content, meta))
         else:
-            logger.warning(f"Received a message for an unknown receiver;{receiver_id}")
+            logger.warning("Received a message for an unknown receiver;%s", receiver_id)
 
     async def shutdown(self):
         """Shutdown all agents in the container and the container itself"""
         self.running = False
         futs = []
         for agent in self._agents.values():
             # shutdown all running agents
```

### Comparing `mango-agents-1.0.0/mango/container/factory.py` & `mango-agents-1.0.1/mango/container/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             mqtt_messenger.tls_set(**tls_kwargs)
 
         # Future that is triggered, on successful connection
         connected = asyncio.Future()
 
         # callbacks to check for successful connection
         def on_con(client, userdata, flags, returncode):
-            logger.info(f"Connection Callback with the following flags: {flags}")
+            logger.info("Connection Callback with the following flags: %s", flags)
             loop.call_soon_threadsafe(connected.set_result, returncode)
 
         mqtt_messenger.on_connect = on_con
 
         # check broker_addr input and connect
         if isinstance(broker_addr, tuple):
             if not 0 < len(broker_addr) < 4:
@@ -155,15 +155,15 @@
             mqtt_messenger.connect(**broker_addr, **mqtt_kwargs)
 
         else:
             if not isinstance(broker_addr, str):
                 raise ValueError("Invalid broker address")
             mqtt_messenger.connect(broker_addr, **mqtt_kwargs)
 
-        logger.info(f"[{client_id}]: Going to connect to broker at {broker_addr}..")
+        logger.info("[%s]: Going to connect to broker at %s..", client_id, broker_addr)
 
         counter = 0
         # process MQTT messages for maximum of 10 seconds to
         # receive connection callback
         while not connected.done() and counter < 100:
             mqtt_messenger.loop()
             # wait for the thread to trigger the future
```

### Comparing `mango-agents-1.0.0/mango/container/mosaik.py` & `mango-agents-1.0.1/mango/container/mosaik.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/mango/container/mqtt.py` & `mango-agents-1.0.1/mango/container/mqtt.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,14 @@
 
         self.client_id: str = client_id
         # the configured and connected paho client
         self.mqtt_client: paho.Client = mqtt_client
         self.inbox_topic: Optional[str] = addr
         # dict mapping additionally subscribed topics to a set of aids
         self.additional_subscriptions: Dict[str, Set[str]] = {}
-        # dict mapping subscribed topics to the expected class
-        self.subscriptions_to_class: Dict[str, Any] = {}
         # Future for pending sub requests
         self.pending_sub_request: Optional[asyncio.Future] = None
 
         # set the callbacks
         self._set_mqtt_callbacks()
 
         # start the mqtt client
@@ -102,18 +100,17 @@
             # decode message and extract content and meta
             content, message_meta = self.decode_mqtt_message(
                 payload=message.payload, topic=message.topic
             )
             # update meta dict
             meta.update(message_meta)
             # put information to inbox
-            if content is not None:
-                self.loop.call_soon_threadsafe(
-                    self.inbox.put_nowait, (0, content, meta)
-                )
+            self.loop.call_soon_threadsafe(
+                self.inbox.put_nowait, (0, content, meta)
+            )
 
         self.mqtt_client.on_message = on_message
         self.mqtt_client.enable_logger(logger)
 
     async def shutdown(self):
         """
         Shutdown container, disconnect from broker and stop mqtt thread
@@ -131,52 +128,42 @@
         :param topic: the topic on which the message arrived
         :param payload: the serialized message
         :return: content and meta
         """
         meta = {}
         content = None
 
-        # check if there is a class definition for the topic
-        for sub, sub_class in self.subscriptions_to_class.items():
-            if paho.topic_matches_sub(sub, topic):
-                # instantiate the provided class
-                content = sub_class()
-                break
-
         decoded = self.codec.decode(payload)
-        if isinstance(content, ACLMessage):
-            meta = decoded.extract_meta()
-            content = decoded.content
+        if isinstance(decoded, ACLMessage):
+            content, meta = decoded.split_content_and_meta()
+        else:
+            content = decoded
 
-        return decoded, meta
+        return content, meta
 
     async def _handle_message(self, *, priority: int, content, meta: Dict[str, Any]):
         """
         This is called as a separate task for every message that is read
         :param priority: priority of the message
         :param content: Deserialized content of the message
         :param meta: Dict with additional information (e.g. topic)
         """
         topic = meta["topic"]
         logger.debug(
             f"Received message with content and meta;{str(content)};{str(meta)}"
         )
-        if hasattr(content, "split_content_and_meta"):
-            content, message_meta = content.split_content_and_meta()
-            meta.update(message_meta)
-            content = content
         if topic == self.inbox_topic:
             # General inbox topic, so no receiver is specified by the topic
             # try to find the receiver from meta
             receiver_id = meta.get("receiver_id", None)
             if receiver_id and receiver_id in self._agents.keys():
                 receiver = self._agents[receiver_id]
                 await receiver.inbox.put((priority, content, meta))
             else:
-                logger.warning(f"Receiver ID is unknown;{receiver_id}")
+                logger.warning("Receiver ID is unknown;%s", receiver_id)
         else:
             # no inbox topic. Check who has subscribed the topic.
             receivers = set()
             for sub, rec in self.additional_subscriptions.items():
                 if paho.topic_matches_sub(sub, topic):
                     receivers.update(rec)
             if not receivers:
@@ -236,33 +223,28 @@
         """
 
         :param topic: MQTT topic
         :param message: The ACL message
         :return:
         """
         encoded_message = self.codec.encode(message)
-        logger.debug(f"Sending message;{message};{topic}")
+        logger.debug("Sending message;%s;%s", message, topic)
         self.mqtt_client.publish(topic, encoded_message)
 
     async def subscribe_for_agent(
-        self, *, aid: str, topic: str, qos: int = 0, expected_class=None
-    ) -> bool:
+        self, *, aid: str, topic: str, qos: int = 0) -> bool:
         """
 
         :param aid: aid of the corresponding agent
         :param topic: topic to subscribe (wildcards are allowed)
         :param qos: The quality of service for the subscription
-        :param expected_class: The class to expect from the topic, defaults
-        to ACL
         :return: A boolean signaling if subscription was true or not
         """
         if aid not in self._agents.keys():
             raise ValueError("Given aid is not known")
-        if expected_class:
-            self.subscriptions_to_class[topic] = expected_class
 
         if topic in self.additional_subscriptions.keys():
             self.additional_subscriptions[topic].add(aid)
             return True
 
         self.additional_subscriptions[topic] = {aid}
         self.pending_sub_request = asyncio.Future()
@@ -271,25 +253,14 @@
         if result != paho.MQTT_ERR_SUCCESS:
             self.pending_sub_request.set_result(False)
             return False
 
         await self.pending_sub_request
         return True
 
-    def set_expected_class(self, *, topic: str, expected_class):
-        """
-        Sets an expected class to a subscription
-        wildcards are allowed here
-        :param topic: The subscription
-        :param expected_class: The expected class
-        :return:
-        """
-        self.subscriptions_to_class[topic] = expected_class
-        logger.debug(f"Expected class updated;{self.subscriptions_to_class}")
-
     def deregister_agent(self, aid):
         """
 
         :param aid:
         :return:
         """
         super().deregister_agent(aid)
```

### Comparing `mango-agents-1.0.0/mango/container/protocol.py` & `mango-agents-1.0.1/mango/container/protocol.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/mango/container/tcp.py` & `mango-agents-1.0.1/mango/container/tcp.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,29 +66,29 @@
         :param kwargs: Additional parameters to provide protocol specific settings
         """
         if isinstance(receiver_addr, str) and ":" in receiver_addr:
             receiver_addr = receiver_addr.split(":")
         elif isinstance(receiver_addr, (tuple, list)) and len(receiver_addr) == 2:
             receiver_addr = tuple(receiver_addr)
         else:
-            logger.warning(f"Address for sending message is not valid;{receiver_addr}")
+            logger.warning("Address for sending message is not valid;%s", receiver_addr)
             return False
 
         message = content
 
         if receiver_addr == self.addr:
             if not receiver_id:
                 receiver_id = message.receiver_id
 
             # internal message
             meta = {"network_protocol": "tcp"}
             receiver = self._agents.get(receiver_id, None)
             if receiver is None:
                 logger.warning(
-                    f"Sending internal message not successful, receiver id unknown;{receiver_id}"
+                    "Sending internal message not successful, receiver id unknown;%s", receiver_id
                 )
                 return False
             success = self._send_internal_message(
                 message, default_meta=meta, target_inbox_overwrite=receiver.inbox
             )
         else:
             success = await self._send_external_message(receiver_addr, message)
@@ -112,23 +112,23 @@
             transport, protocol = await self.loop.create_connection(
                 lambda: ContainerProtocol(
                     container=self, loop=self.loop, codec=self.codec
                 ),
                 addr[0],
                 addr[1],
             )
-            logger.debug(f"Connection established to addr;{str(addr)}")
+            logger.debug("Connection established to addr;{str(addr)}")
 
             protocol.write(self.codec.encode(message))
 
-            logger.debug(f"Message sent to addr;{str(addr)}")
+            logger.debug("Message sent to addr;%s", addr)
             await protocol.shutdown()
         except OSError:
             logger.warning(
-                f"Could not establish connection to receiver of a message;{str(addr)}"
+                "Could not establish connection to receiver of a message;%s", addr
             )
             return False
         return True
 
     async def shutdown(self):
         """
         calls shutdown() from super class Container and closes the server
```

### Comparing `mango-agents-1.0.0/mango/messages/acl_message_pb2.py` & `mango-agents-1.0.1/mango/messages/acl_message_pb2.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/mango/messages/codecs.py` & `mango-agents-1.0.1/mango/messages/codecs.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/mango/messages/message.py` & `mango-agents-1.0.1/mango/messages/message.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/mango/messages/other_proto_msgs_pb2.py` & `mango-agents-1.0.1/mango/messages/other_proto_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/mango/modules/base_module.py` & `mango-agents-1.0.1/mango/modules/base_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,10 +62,10 @@
             print(f"exception in {self.name}")
             print(f"exception: {exception}")
             raise exception
 
     # def handle_exception(loop, context):
     #     # context["message"] will always be there; but context["exception"] may not
     #     msg = context.get("exception", context["message"])
-    #     logging.error(f"Caught exception: {msg}")
+    #     logging.error("Caught exception: %s", msg)
     #     logging.info("Shutting down...")
     #     asyncio.create_task(shutdown(loop))
```

### Comparing `mango-agents-1.0.0/mango/modules/mqtt_module.py` & `mango-agents-1.0.1/mango/modules/mqtt_module.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/mango/modules/rabbit_module.py` & `mango-agents-1.0.1/mango/modules/rabbit_module.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/mango/modules/zero_module.py` & `mango-agents-1.0.1/mango/modules/zero_module.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/mango/util/clock.py` & `mango-agents-1.0.1/mango/util/clock.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/mango/util/distributed_clock.py` & `mango-agents-1.0.1/mango/util/distributed_clock.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 
     def handle_message(self, content: float, meta):
         if isinstance(meta["sender_addr"], list):
             sender_addr = tuple(meta["sender_addr"])
         else:
             sender_addr = meta["sender_addr"]
 
-        logger.debug(f"clockmanager: {content} from {sender_addr}")
+        logger.debug("clockmanager: %s from %s", content, sender_addr)
         if content:
             assert isinstance(content, float), f"{content} was {type(content)}"
             self.schedules.append(content)
 
         if not self.futures[sender_addr].done():
             self.futures[sender_addr].set_result(True)
         else:
-            logger.warning(f"got another message from agent {sender_addr}")
+            logger.warning("got another message from agent %s", sender_addr)
 
     async def broadcast(self, message, add_futures=True):
         for receiver_addr in self.receiver_clock_addresses:
-            logger.debug(f"clockmanager send: {message} - {receiver_addr}")
+            logger.debug("clockmanager send: %s - %s", message, receiver_addr)
             send_worked = await self.send_acl_message(
                 message,
                 receiver_addr,
                 "clock_agent",
                 acl_metadata={"sender_id": self.aid},
             )
             if send_worked and add_futures:
@@ -56,42 +56,42 @@
         await super().shutdown()
 
     async def distribute_time(self):
         self.schedules = []
         await asyncio.sleep(0.01)
         # wait until all jobs in other containers are finished
         for container_id, fut in self.futures.items():
-            logger.debug(f"waiting for {container_id}")
+            logger.debug("waiting for %s", container_id)
             # waits forever if manager was started first
             # as answer is never received
             await fut
         # wait for our container too
         await self.wait_all_done()
         if self._scheduler.clock.get_next_activity() is not None:
             self.schedules.append(self._scheduler.clock.get_next_activity())
 
         if self.schedules:
             next_event = min(self.schedules)
         else:
             logger.warning("no new events, time stands still")
             next_event = self._scheduler.clock.time
-        logger.debug(f"next event at {next_event}")
+        logger.debug("next event at %s", next_event)
         self.schedule_instant_task(coroutine=self.broadcast(next_event))
         return next_event
 
 
 class DistributedClockAgent(ClockAgent):
     def __init__(self, container):
         super().__init__(container, "clock_agent")
         self.stopped = asyncio.Future()
 
     def handle_message(self, content: float, meta):
         sender_addr = meta["sender_addr"]
         sender_id = meta["sender_id"]
-        logger.info(f"clockagent: {content} from {sender_addr}")
+        logger.info("clockagent: %s from %s", content, sender_addr)
         if content == "stop":
             if not self.stopped.done():
                 self.stopped.set_result(True)
         else:
             assert isinstance(content, (int, float)), f"{content} was {type(content)}"
             self._scheduler.clock.set_time(content)
```

### Comparing `mango-agents-1.0.0/mango/util/scheduling.py` & `mango-agents-1.0.1/mango/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/mango_agents.egg-info/PKG-INFO` & `mango-agents-1.0.1/mango_agents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-agents
-Version: 1.0.0
+Version: 1.0.1
 Summary: Modular Python Agent Framework
 Author: mango Team
 Author-email: mango@offis.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mango-agents-1.0.0/mango_agents.egg-info/SOURCES.txt` & `mango-agents-1.0.1/mango_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mango-agents-1.0.0/setup.py` & `mango-agents-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # Package meta-data.
 NAME = 'mango-agents'
 DESCRIPTION = 'Modular Python Agent Framework'
 URL = 'https://gitlab.com/mango-agents/mango'
 EMAIL = 'mango@offis.de'
 AUTHOR = 'mango Team'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'paho-mqtt==1.5.1', 'protobuf==3.13.0', 'python-dateutil==2.8.2'
+    'paho-mqtt==1.5.1', 'protobuf==3.19.1', 'python-dateutil==2.8.2'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

