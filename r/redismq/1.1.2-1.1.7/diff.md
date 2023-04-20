# Comparing `tmp/redismq-1.1.2.tar.gz` & `tmp/redismq-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redismq-1.1.2.tar", last modified: Wed Apr  6 21:35:45 2022, max compression
+gzip compressed data, was "redismq-1.1.7.tar", last modified: Thu Apr 20 21:15:37 2023, max compression
```

## Comparing `redismq-1.1.2.tar` & `redismq-1.1.7.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-06 21:35:45.637797 redismq-1.1.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4626 2022-04-06 21:35:45.637797 redismq-1.1.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4105 2022-04-06 21:34:54.000000 redismq-1.1.2/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-06 21:35:45.637797 redismq-1.1.2/redismq/
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2022-04-06 21:34:54.000000 redismq-1.1.2/redismq/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8009 2022-04-06 21:34:54.000000 redismq-1.1.2/redismq/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7628 2022-04-06 21:34:54.000000 redismq-1.1.2/redismq/consumer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3020 2022-04-06 21:34:54.000000 redismq-1.1.2/redismq/debugging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5199 2022-04-06 21:34:54.000000 redismq-1.1.2/redismq/producer.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-06 21:35:45.637797 redismq-1.1.2/redismq.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4626 2022-04-06 21:35:44.000000 redismq-1.1.2/redismq.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      281 2022-04-06 21:35:45.000000 redismq-1.1.2/redismq.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-04-06 21:35:45.000000 redismq-1.1.2/redismq.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2022-04-06 21:35:45.000000 redismq-1.1.2/redismq.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2022-04-06 21:35:45.000000 redismq-1.1.2/redismq.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       74 2022-04-06 21:35:45.637797 redismq-1.1.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1321 2022-04-06 21:34:54.000000 redismq-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:15:37.105231 redismq-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-20 21:15:37.105231 redismq-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-20 21:15:26.000000 redismq-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:15:37.105231 redismq-1.1.7/redismq/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-20 21:15:26.000000 redismq-1.1.7/redismq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-04-20 21:15:26.000000 redismq-1.1.7/redismq/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-20 21:15:26.000000 redismq-1.1.7/redismq/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-20 21:15:26.000000 redismq-1.1.7/redismq/debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-20 21:15:26.000000 redismq-1.1.7/redismq/producer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:15:37.105231 redismq-1.1.7/redismq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-20 21:15:37.000000 redismq-1.1.7/redismq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-20 21:15:37.000000 redismq-1.1.7/redismq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:15:37.000000 redismq-1.1.7/redismq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 21:15:37.000000 redismq-1.1.7/redismq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 21:15:37.000000 redismq-1.1.7/redismq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 21:15:37.105231 redismq-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-20 21:15:26.000000 redismq-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:15:37.105231 redismq-1.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-20 21:15:26.000000 redismq-1.1.7/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-04-20 21:15:26.000000 redismq-1.1.7/tests/test_confirmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-20 21:15:26.000000 redismq-1.1.7/tests/test_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-20 21:15:26.000000 redismq-1.1.7/tests/test_unconfirmed.py
```

### Comparing `redismq-1.1.2/PKG-INFO` & `redismq-1.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: redismq
-Version: 1.1.2
+Version: 1.1.7
 Summary: Message Queueing for Redis Streams
 Home-page: https://github.com/stevemandl/pyredismq
 Author: Steve Mandl
 Author-email: sjm34@cornell.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -68,14 +66,20 @@
 testing:
 
 ```console
 pipenv install --dev
 pipenv run pytest
 ```
 
+debugging:
+
+```console
+export REDISMQ=DEBUG
+...
+```
 ## Getting Started
 
 RedisMQ needs to connect to an existing redis server, so you will need the address and port of the server you want to use. RedisMQ also stores global state in the redis server. By default the namespace used for global keys is rmq:*. If you need to change this so it does not conflict with other data stored in redis, the configuration parameter redismq_namespace should be set to something different.
 
 ## Examples
 
 Here are some examples of using the pyredismq module. See [more examples](https://github.com/stevemandl/pyredismq/tree/main/examples) here.
@@ -129,8 +133,7 @@
 >>>     resp = 'I got your message' if payload.responseChannel else ''
 >>>     await payload.ack(resp)
 ```
 ## More Information
 
 RedisMQ is free software under the New BSD license, see LICENSE.txt for
 details.
-
```

### Comparing `redismq-1.1.2/README.md` & `redismq-1.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,20 @@
 testing:
 
 ```console
 pipenv install --dev
 pipenv run pytest
 ```
 
+debugging:
+
+```console
+export REDISMQ=DEBUG
+...
+```
 ## Getting Started
 
 RedisMQ needs to connect to an existing redis server, so you will need the address and port of the server you want to use. RedisMQ also stores global state in the redis server. By default the namespace used for global keys is rmq:*. If you need to change this so it does not conflict with other data stored in redis, the configuration parameter redismq_namespace should be set to something different.
 
 ## Examples
 
 Here are some examples of using the pyredismq module. See [more examples](https://github.com/stevemandl/pyredismq/tree/main/examples) here.
```

### Comparing `redismq-1.1.2/redismq/client.py` & `redismq-1.1.7/redismq/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     """
 
     log_debug: Callable[..., None]
 
     status: str
     namespace: str
     redis: Any
+    pubsub: Any
+    sub_task: Any
 
     payloads: Set[Any]
     payloads_updated: asyncio.Condition
 
     producer_registry: Dict[str, Producer]
 
     def __init__(self) -> None:
@@ -66,24 +68,29 @@
         # set the namespace
         if namespace:
             cls.namespace = namespace
 
         # we are 'connecting' but not really until the PING
         client.status = "connecting"
 
-        # create a connection pool
-        client.redis = aioredis.from_url(
+        # create a blocking connection pool to wait for a connection to become available
+        # rather than raising an exception
+        # see https://aioredis.readthedocs.io/en/latest/api/low-level/#aioredis.connection.BlockingConnectionPool
+        pool = aioredis.BlockingConnectionPool.from_url(
             address, max_connections=10, decode_responses=True
         )
+        client.redis = aioredis.Redis(connection_pool=pool)
         Client.log_debug("    - redis: %s", client.redis)
 
         # try to ping it
         rslt = await client.redis.ping()
         Client.log_debug("    - ping: %r", rslt)
 
+        client.pubsub = client.redis.pubsub(ignore_subscribe_messages=True)
+        client.sub_task = asyncio.get_running_loop().create_task(client.pubsub.run())
         client.status = "ready"
 
         return client
 
     async def close(self) -> None:
         """
         Call to wait for all of the active payloads to complete.
@@ -95,16 +102,25 @@
             raise RuntimeError("Client is not ready to close")
 
         self.status = "closing"
 
         # wait for the event that says no more pending
         Client.log_debug(f"    - payloads: {self.payloads}")
         await self.payloads_event.wait()
+        self.sub_task.cancel()
+        try:
+            await self.sub_task
+        except asyncio.CancelledError:
+            Client.log_debug(f"    - sub_task cancelled")
+        await self.pubsub.close()
+        Client.log_debug(f"    - pubsub closed")
         await self.redis.close()
+        Client.log_debug(f"    - redis closed")
         await self.redis.connection_pool.disconnect()
+        Client.log_debug(f"    - connection_pool disconnected")
 
         self.status = "closed"
 
     async def producer(
         self, stream_name: str, maxlen: int = MAXLEN, timeout: float = TIMEOUT
     ) -> Producer:
         """
```

### Comparing `redismq-1.1.2/redismq/consumer.py` & `redismq-1.1.7/redismq/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
             args = {
                 "groupname": self.group_name,
                 "consumername": self.consumer_name,
                 "count": 1,
                 "block": self.xread_timeout,
                 "streams": {self.stream_name: latest_id},
             }
+            messages = None
             try:
                 messages = await self.client.redis.xreadgroup(**args)
                 Consumer.log_debug("    - messages: %r", messages)
             except Exception as err:
                 Consumer.log_debug("    - xreadgroup exception: %r", err)
 
             if not messages:
```

### Comparing `redismq-1.1.2/redismq/debugging.py` & `redismq-1.1.7/redismq/debugging.py`

 * *Files identical despite different names*

### Comparing `redismq-1.1.2/redismq/producer.py` & `redismq-1.1.7/redismq/producer.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from __future__ import annotations
 
 import asyncio
 import json
 import time
 
 from typing import TYPE_CHECKING, Any, Callable, Dict, TypedDict, Optional, cast
-from redis import Connection # type: ignore[attr-defined]
+from redis import Connection  # type: ignore[attr-defined]
 from .debugging import debugging
 
-Client = TypedDict('Client', redis=Connection)
+Client = TypedDict("Client", redis=Connection)
 
 # class is declared as generic in stubs but not at runtime
 AnyFuture = asyncio.Future
 
 # settings
 MAXLEN = 100
 TIMEOUT = 10.0
@@ -52,65 +52,39 @@
         self.stream_name = stream_name
         self.channel_key = "%s:responseid" % client.namespace
         self.maxlen = maxlen
         self.timeout = timeout
 
         self.id = time.time_ns()
 
-    async def _resp_task(
-        self, payload: Dict[str, Any], response_channel_id: Optional[str]
-    ) -> Any:
-        """
-        utility method for a confirmed request
-        """
-        Producer.log_debug("_resp_task: %r %r", payload, response_channel_id)
-
-        # get a unique channel identifier if one hasn't been provided
-        if response_channel_id is None:
-            uid = await self.client.redis.incr(self.channel_key)
-            response_channel_id = "%s:response.%d" % (self.client.namespace, uid)
-        Producer.log_debug("    - response_channel_id: %r", response_channel_id)
-
-        # pack it into the request payload
-        payload["response_channel"] = response_channel_id
-
-        async with self.client.redis.pubsub() as pubsub:
-            Producer.log_debug("    - pubsub: %r", pubsub)
-
-            # start listening for a response
-            await pubsub.subscribe(response_channel_id)
-            Producer.log_debug("    - subscribed")
-
-            # put the request into the stream
-            message_id: str = await self.client.redis.xadd(
-                self.stream_name, payload, maxlen=self.maxlen
-            )
-            Producer.log_debug("    - message_id: %r", message_id)
-
+    # make the handler for the channel
+    def get_handler(self, channel_id, fut: AnyFuture):
+        Producer.log_debug("get_handler channel_id %r fut %r" % (channel_id, fut))
+
+        async def _handler(json_message=None):
+            Producer.log_debug("_handler json_message: %r", json_message)
+            response = None
             try:
-                # wait for the response to come back encoded as JSON
-                while True:
-                    json_message = await pubsub.get_message(
-                        ignore_subscribe_messages=True, timeout=self.timeout
-                    )
-                    Producer.log_debug("    - json_message: %r", json_message)
-                    if json_message:
-                        response = json.loads(json_message["data"])
-                        break
+                if json_message:
+                    response = json.loads(json_message["data"])
             except ValueError as err:
-                Producer.log_debug("    - value/decoding error %s", response_channel_id)
+                Producer.log_debug("    - value/decoding error %s", channel_id)
                 response = {"message": "JSON Decoding Error", "err": err}
-            except asyncio.CancelledError as err:
-                Producer.log_debug("    - canceled %s", response_channel_id)
-                response = {"message": "Cancelled Error", "err": err}
+            except TypeError as err:
+                Producer.log_debug("    - type error %s", channel_id)
+                response = {"message": "Type Error", "err": err}
             finally:
-                Producer.log_debug("    - finally %s", response_channel_id)
-                await pubsub.unsubscribe(response_channel_id)
+                Producer.log_debug("    - finally %s", channel_id)
+                await self.client.pubsub.unsubscribe(channel_id)
+                Producer.log_debug("    - unsubscribed %s", channel_id)
+                if not fut.cancelled():
+                    Producer.log_debug("    -setting result %s", response)
+                    fut.set_result(response)
 
-        return response
+        return _handler
 
     # pylint: disable=invalid-name
     def addUnconfirmedMessage(
         self, message: Any, response_channel_id: str = None
     ) -> AnyFuture:
         """
         Return a task that adds an unconfirmed message to the message queue.
@@ -119,37 +93,66 @@
 
         # JSON encode the message
         payload = {"message": json.dumps(message)}
         if response_channel_id is not None:
             payload["response_channel"] = response_channel_id
 
         # create a task to add it to the stream
-        future = self.client.redis.xadd(
-            self.stream_name, payload, maxlen=self.maxlen
-        )
+        future = self.client.redis.xadd(self.stream_name, payload, maxlen=self.maxlen)
 
         return cast(AnyFuture, future)
 
     # pylint: disable=invalid-name
-    def addConfirmedMessage(
-        self, message: Any, response_channel_id: Optional[str] = None
-    ) -> AnyFuture:
+    async def addConfirmedMessage(self, message: Any):
         """
-        Return a task that adds a confirmed message to the message queue and
-        waits for the response.
+        Adds a confirmed message to the message queue and
+        results in the confirmed response.
         """
         Producer.log_debug("addConfirmedMessage %r", message)
 
         # JSON encode the message
         payload = {"message": json.dumps(message)}
+        # create a future
+        future = asyncio.get_running_loop().create_future()
 
-        # create a task to add it to the stream
-        future = self._resp_task(payload, response_channel_id)
+        # get a unique channel identifier
+        uid = await self.client.redis.incr(self.channel_key)
+        response_channel_id = "%s:response.%d" % (self.client.namespace, uid)
+        Producer.log_debug("    - response_channel_id: %r", response_channel_id)
 
-        return cast(AnyFuture, future)
+        # pack it into the request payload
+        payload["response_channel"] = response_channel_id
+
+        # start listening for a response
+        _handler = self.get_handler(response_channel_id, future)
+        kwargs = {response_channel_id: _handler}
+        try:
+            await self.client.pubsub.subscribe(**kwargs)
+            Producer.log_debug("    - subscribed")
+
+            # put the request into the stream
+            message_id: str = await self.client.redis.xadd(
+                self.stream_name, payload, maxlen=self.maxlen
+            )
+            Producer.log_debug("    - message_id: %r", message_id)
+            # future will get the result set by the handler when the response is published
+            resp = await asyncio.wait_for(future, self.timeout)
+        except asyncio.TimeoutError as err:
+            Producer.log_debug("    - timeout waiting for future: %r", err)
+            await _handler()
+            resp = {"message": "Timeout Error", "err": err}
+        except asyncio.CancelledError as err:
+            Producer.log_debug("    - cancelled %r", err)
+            await _handler()
+            resp = {"message": "Cancelled Error", "err": err}
+        except BaseException as err:
+            #Producer.log_debug("    - unexpected error %r", err)
+            await _handler()
+            resp = {"message": "Unexpected Error", "err": err}
+        return resp
 
     # pylint: disable=invalid-name
     def destroy(self) -> None:
         """
         Stops this producer from working. This is automatically called when
         client.dispose_producer() is called with this producer.
         """
```

### Comparing `redismq-1.1.2/redismq.egg-info/PKG-INFO` & `redismq-1.1.7/redismq.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: redismq
-Version: 1.1.2
+Version: 1.1.7
 Summary: Message Queueing for Redis Streams
 Home-page: https://github.com/stevemandl/pyredismq
 Author: Steve Mandl
 Author-email: sjm34@cornell.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -68,14 +66,20 @@
 testing:
 
 ```console
 pipenv install --dev
 pipenv run pytest
 ```
 
+debugging:
+
+```console
+export REDISMQ=DEBUG
+...
+```
 ## Getting Started
 
 RedisMQ needs to connect to an existing redis server, so you will need the address and port of the server you want to use. RedisMQ also stores global state in the redis server. By default the namespace used for global keys is rmq:*. If you need to change this so it does not conflict with other data stored in redis, the configuration parameter redismq_namespace should be set to something different.
 
 ## Examples
 
 Here are some examples of using the pyredismq module. See [more examples](https://github.com/stevemandl/pyredismq/tree/main/examples) here.
@@ -129,8 +133,7 @@
 >>>     resp = 'I got your message' if payload.responseChannel else ''
 >>>     await payload.ack(resp)
 ```
 ## More Information
 
 RedisMQ is free software under the New BSD license, see LICENSE.txt for
 details.
-
```

### Comparing `redismq-1.1.2/setup.py` & `redismq-1.1.7/setup.py`

 * *Files identical despite different names*

