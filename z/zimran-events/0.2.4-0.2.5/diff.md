# Comparing `tmp/zimran-events-0.2.4.tar.gz` & `tmp/zimran-events-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-events-0.2.4.tar", last modified: Wed Apr 19 10:57:51 2023, max compression
+gzip compressed data, was "zimran-events-0.2.5.tar", last modified: Thu Apr 20 06:21:01 2023, max compression
```

## Comparing `zimran-events-0.2.4.tar` & `zimran-events-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.066606 zimran-events-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.062606 zimran-events-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.066606 zimran-events-0.2.4/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.066606 zimran-events-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-19 10:57:43.000000 zimran-events-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-19 10:57:43.000000 zimran-events-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-19 10:57:51.066606 zimran-events-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-19 10:57:43.000000 zimran-events-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-19 10:57:43.000000 zimran-events-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-19 10:57:43.000000 zimran-events-0.2.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 10:57:51.066606 zimran-events-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.062606 zimran-events-0.2.4/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.066606 zimran-events-0.2.4/zimran/events/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-19 10:57:43.000000 zimran-events-0.2.4/zimran/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:57:51.066606 zimran-events-0.2.4/zimran_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-19 10:57:51.000000 zimran-events-0.2.4/zimran_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 10:57:51.000000 zimran-events-0.2.4/zimran_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:57:51.000000 zimran-events-0.2.4/zimran_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-19 10:57:51.000000 zimran-events-0.2.4/zimran_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 10:57:51.000000 zimran-events-0.2.4/zimran_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.935105 zimran-events-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.931105 zimran-events-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.935105 zimran-events-0.2.5/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.935105 zimran-events-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-20 06:20:52.000000 zimran-events-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-20 06:21:01.935105 zimran-events-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-20 06:20:52.000000 zimran-events-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-20 06:20:52.000000 zimran-events-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-20 06:20:52.000000 zimran-events-0.2.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 06:21:01.935105 zimran-events-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.931105 zimran-events-0.2.5/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.935105 zimran-events-0.2.5/zimran/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.935105 zimran-events-0.2.5/zimran_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-20 06:21:01.000000 zimran-events-0.2.5/zimran_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-20 06:21:01.000000 zimran-events-0.2.5/zimran_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:21:01.000000 zimran-events-0.2.5/zimran_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 06:21:01.000000 zimran-events-0.2.5/zimran_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 06:21:01.000000 zimran-events-0.2.5/zimran_events.egg-info/top_level.txt
```

### Comparing `zimran-events-0.2.4/.github/scripts/release.py` & `zimran-events-0.2.5/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.4/.gitignore` & `zimran-events-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.4/.pre-commit-config.yaml` & `zimran-events-0.2.5/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -75,13 +75,14 @@
         additional_dependencies:
           - flake8-builtins
           - flake8-print
           - flake8-debugger
           - flake8-commas
           - flake8-comprehensions
           - flake8-eradicate
+          - flake8-unused-arguments
 
   - repo: https://github.com/psf/black
     rev: 22.10.0
     hooks:
       - id: black
         args: [--config=pyproject.toml]
```

### Comparing `zimran-events-0.2.4/LICENSE` & `zimran-events-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.4/PKG-INFO` & `zimran-events-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.4
+Version: 0.2.5
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.2.4/README.md` & `zimran-events-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.4/pyproject.toml` & `zimran-events-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zimran-events"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Talgat Abdraimov", email="abdraimov.talga@gmail.com" },
 ]
 description = "The zimran-events provides amqp interface"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
```

### Comparing `zimran-events-0.2.4/zimran/events/connection.py` & `zimran-events-0.2.5/zimran/events/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import asyncio
-
 import aio_pika
 import pika
 from aioretry import retry
+from pika.adapters.blocking_connection import BlockingChannel
 
 from zimran.events.utils import retry_policy
 
 
 try:
     from loguru import logger
 except ImportError:
@@ -23,27 +22,27 @@
         self._channel = None
         self._channel_number = channel_number
 
     def __enter__(self):
         self.connect()
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(self, exc_type, exc_val, exc_tb):  # noqa: U100
         self.disconnect()
 
     @property
     def connection(self):
         if self._connection is None or self._connection.is_closed:
             self._connection = pika.BlockingConnection(parameters=pika.URLParameters(self._url))
             logger.info('AMQP connection established')
 
         return self._connection
 
     @property
-    def channel(self):
+    def channel(self) -> BlockingChannel:
         if self._channel is None or self._channel.is_closed:
             self._channel = self.connection.channel(channel_number=self._channel_number)
             logger.info('Channel connection established')
 
         return self._channel
 
     def connect(self):
@@ -57,33 +56,32 @@
         if self._connection is not None and self._connection.is_open:
             self._connection.close()
 
         logger.info('AMQP Connection disconnected')
 
 
 class AsyncConnection:
-    def __init__(self, *, broker_url: str, loop: asyncio.AbstractEventLoop, channel_number: int = 1):
+    def __init__(self, *, broker_url: str, channel_number: int = 1):
         self._url = broker_url
-        self._loop = loop
 
         self._connection = None
         self._channel = None
         self._channel_number = channel_number
 
     async def __aenter__(self):
         await self.connect()
         return self
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
+    async def __aexit__(self, exc_type, exc_val, exc_tb):  # noqa: U100
         await self.disconnect()
 
     @property
     async def connection(self) -> aio_pika.abc.AbstractRobustConnection:
         if self._connection is None or self._connection.is_closed:
-            self._connection = await aio_pika.connect_robust(url=self._url, loop=self._loop)
+            self._connection = await aio_pika.connect_robust(url=self._url)
             logger.info('AMQP connection established')
 
         return self._connection
 
     @property
     async def channel(self):
         if self._channel is None or self._channel.is_closed:
```

### Comparing `zimran-events-0.2.4/zimran/events/consumer.py` & `zimran-events-0.2.5/zimran/events/consumer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import asyncio
 
-import aio_pika
 from aioretry import retry
-from pika.channel import Channel
 
 
 try:
     from loguru import logger
 except ImportError:
     import logging
 
     logger = logging.getLogger(__name__)
 
 
 from zimran.events.connection import AsyncConnection, Connection
-from zimran.events.constants import DEAD_LETTER_EXCHANGE_NAME, UNROUTABLE_EXCHANGE_NAME, UNROUTABLE_QUEUE_NAME
+from zimran.events.constants import DEAD_LETTER_EXCHANGE_NAME
 from zimran.events.schemas import ExchangeScheme
 from zimran.events.utils import cleanup_and_normalize_queue_name, retry_policy, validate_exchange
 
 
 class ConsumerMixin:
     def handle_event(self, name: str, *, exchange: ExchangeScheme | None = None):
         if exchange is not None:
@@ -58,16 +56,14 @@
         self._event_handlers = {}
 
     def run(self):
         try:
             channel = self.channel
             channel.basic_qos(prefetch_count=self._prefetch_count)
 
-            self._declare_unroutable_exchange(channel)
-
             consumer_amount = 0
             for event_name, data in self._event_handlers.items():
                 queue_name = cleanup_and_normalize_queue_name(f'{self._service_name}.{event_name}')
                 channel.queue_declare(
                     queue_name,
                     durable=True,
                     arguments={
@@ -90,46 +86,36 @@
             logger.info(f'Registered {consumer_amount} consumers')
             channel.start_consuming()
         except Exception as exc:
             logger.error(f'Exception occured | error: {exc} | type: {type(exc)}')
         finally:
             self.disconnect()
 
-    def _declare_unroutable_exchange(self, channel: Channel):
-        channel.exchange_declare(exchange=UNROUTABLE_EXCHANGE_NAME, exchange_type='fanout', durable=True)
-        channel.queue_declare(queue=UNROUTABLE_QUEUE_NAME, durable=True)
-        channel.queue_bind(queue=UNROUTABLE_QUEUE_NAME, exchange=UNROUTABLE_EXCHANGE_NAME, routing_key='')
-
-        logger.info('Declared unroutable events exchange')
-
 
 class AsyncConsumer(AsyncConnection, ConsumerMixin):
     def __init__(
         self,
         *,
         service_name: str,
         broker_url: str,
         channel_number: int = 1,
         prefetch_count: int = 10,
-        loop=None,
     ):
-        loop = loop or asyncio.get_event_loop()
-        super().__init__(broker_url=broker_url, loop=loop, channel_number=channel_number)
+        super().__init__(broker_url=broker_url, channel_number=channel_number)
 
         self._service_name = service_name.replace('-', '_').lower()
         self._prefetch_count = prefetch_count
 
         self._event_handlers = {}
 
     @retry(retry_policy)
     async def run(self):
         try:
             channel = await self.channel
-            tasks = [self._declare_unroutable_queue(channel), channel.set_qos(prefetch_count=self._prefetch_count)]
-            await asyncio.gather(*tasks)
+            await channel.set_qos(prefetch_count=self._prefetch_count)
 
             consumer_amount = 0
             for event_name, data in self._event_handlers.items():
                 queue_name = cleanup_and_normalize_queue_name(f'{self._service_name}.{event_name}')
                 queue = await channel.declare_queue(
                     queue_name,
                     durable=True,
@@ -149,12 +135,7 @@
             logger.info(f'Registered {consumer_amount} consumers')
             await asyncio.Future()
         except Exception as exc:
             logger.error(f'Exception occured | error: {exc}')
             raise exc
         finally:
             await self.disconnect()
-
-    async def _declare_unroutable_queue(self, channel: aio_pika.abc.AbstractRobustChannel):
-        exchange = await channel.declare_exchange(name=UNROUTABLE_EXCHANGE_NAME, type='fanout', durable=True)
-        queue = await channel.declare_queue(name=UNROUTABLE_QUEUE_NAME, durable=True)
-        await queue.bind(exchange=exchange, routing_key='')
```

### Comparing `zimran-events-0.2.4/zimran/events/producer.py` & `zimran-events-0.2.5/zimran/events/producer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import json
 
 import aio_pika
 import pika
 from aioretry import retry
 
 
@@ -11,15 +10,14 @@
 except ImportError:
     import logging
 
     logger = logging.getLogger(__name__)
 
 
 from .connection import AsyncConnection, Connection
-from .constants import UNROUTABLE_EXCHANGE_NAME, UNROUTABLE_QUEUE_NAME
 from .schemas import ChannelPropertiesScheme, ExchangeScheme
 from .utils import retry_policy, validate_channel_properties, validate_exchange
 
 
 class Producer(Connection):
     def __init__(self, *, broker_url: str, channel_number: int = 1):
         super().__init__(broker_url=broker_url, channel_number=channel_number)
@@ -40,41 +38,34 @@
         basic_properties = pika.BasicProperties(**properties.as_dict(exclude_none=True))
         body = json.dumps(payload, default=str)
         if exchange is None:
             self.channel.basic_publish(exchange='', routing_key=routing_key, body=body, properties=basic_properties)
             logger.info(f'Message published to basic exchange | routing_key: {routing_key}')
             return
 
-        self._declare_unroutable_queue()
-
         validate_exchange(exchange)
+
         self.channel.exchange_declare(
             exchange=exchange.name,
             exchange_type=exchange.type,
             **exchange.as_dict(exclude=['name', 'type', 'timeout'], exclude_none=True),
         )
 
         self.channel.basic_publish(
             exchange=exchange.name,
             routing_key=routing_key,
             body=body,
             properties=basic_properties,
         )
         logger.info(f'Message published to {exchange.name} exchange | routing_key: {routing_key}')
 
-    def _declare_unroutable_queue(self):
-        self.channel.exchange_declare(exchange=UNROUTABLE_EXCHANGE_NAME, exchange_type='fanout', durable=True)
-        self.channel.queue_declare(queue=UNROUTABLE_QUEUE_NAME, durable=True)
-        self.channel.queue_bind(queue=UNROUTABLE_QUEUE_NAME, exchange=UNROUTABLE_EXCHANGE_NAME, routing_key='')
-
 
 class AsyncProducer(AsyncConnection):
-    def __init__(self, *, broker_url: str, channel_number: int = 1, loop: asyncio.AbstractEventLoop | None = None):
-        loop = loop or asyncio.get_event_loop()
-        super().__init__(broker_url=broker_url, channel_number=channel_number, loop=loop)
+    def __init__(self, *, broker_url: str, channel_number: int = 1):
+        super().__init__(broker_url=broker_url, channel_number=channel_number)
 
     @retry(retry_policy)
     async def publish(
         self,
         routing_key: str,
         *,
         payload: dict,
@@ -91,21 +82,15 @@
         channel = await self.channel
         if exchange is None:
             await channel.default_exchange.publish(message=message, routing_key=routing_key)
             logger.info(f'Message published to basic exchange | routing_key: {routing_key}')
             return
 
         validate_exchange(exchange)
-        await self._declare_unroutable_queue(channel)
 
         declared_exchange = await channel.declare_exchange(**exchange.as_dict(exclude_none=True))
         await declared_exchange.publish(message=message, routing_key=routing_key)
         logger.info(f'Message published to {exchange.name} exchange | routing_key: {routing_key}')
 
     @staticmethod
     def _get_message(properties: ChannelPropertiesScheme, payload: dict):
         return aio_pika.Message(body=json.dumps(payload, default=str).encode(), **properties.as_dict(exclude_none=True))
-
-    async def _declare_unroutable_queue(self, channel: aio_pika.abc.AbstractRobustChannel):
-        exchange = await channel.declare_exchange(name=UNROUTABLE_EXCHANGE_NAME, type='fanout', durable=True)
-        queue = await channel.declare_queue(name=UNROUTABLE_QUEUE_NAME, durable=True)
-        await queue.bind(exchange=exchange, routing_key='')
```

### Comparing `zimran-events-0.2.4/zimran/events/schemas.py` & `zimran-events-0.2.5/zimran/events/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import datetime
 import uuid
 from dataclasses import asdict, dataclass
 
-from zimran.events.constants import UNROUTABLE_EXCHANGE_NAME
-
 
 class SchemeBase:
     def as_dict(self, exclude: list | None = None, exclude_none: bool = False) -> dict:
         excluded_keys = exclude if isinstance(exclude, (list, tuple)) else []
         data = {key: val for key, val in asdict(self).items() if key not in excluded_keys}
 
         if exclude_none:
@@ -28,17 +26,14 @@
     arguments: dict | None = None
     timeout: float | int | None = None
 
     def __post_init__(self):
         if self.arguments is None:
             self.arguments = {}
 
-        if isinstance(self.arguments, dict):
-            self.arguments.setdefault('alternate-exchange', UNROUTABLE_EXCHANGE_NAME)
-
 
 @dataclass(kw_only=True)
 class ChannelPropertiesScheme(SchemeBase):
     correlation_id: str | None = None
     content_type: str = 'application/json'
     delivery_mode: int = 2  # Persistent
     headers: dict | None = None
```

### Comparing `zimran-events-0.2.4/zimran/events/utils.py` & `zimran-events-0.2.5/zimran/events/utils.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.4/zimran_events.egg-info/PKG-INFO` & `zimran-events-0.2.5/zimran_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.4
+Version: 0.2.5
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.2.4/zimran_events.egg-info/SOURCES.txt` & `zimran-events-0.2.5/zimran_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

