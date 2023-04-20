# Comparing `tmp/oxalis-0.5.1.tar.gz` & `tmp/oxalis-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxalis-0.5.1.tar", max compression
+gzip compressed data, was "oxalis-0.5.2.tar", max compression
```

## Comparing `oxalis-0.5.1.tar` & `oxalis-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.5.1/LICENSE
--rw-r--r--   0        0        0     6896 2023-03-09 12:50:46.866544 oxalis-0.5.1/README.md
--rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.5.1/oxalis/__init__.py
--rw-r--r--   0        0        0    10828 2022-08-25 07:41:56.902264 oxalis-0.5.1/oxalis/amqp.py
--rw-r--r--   0        0        0     6289 2023-03-09 12:59:45.657732 oxalis-0.5.1/oxalis/base.py
--rw-r--r--   0        0        0     1654 2022-07-12 02:08:37.164774 oxalis-0.5.1/oxalis/beater.py
--rw-r--r--   0        0        0     3465 2023-03-09 12:59:13.870488 oxalis-0.5.1/oxalis/pool.py
--rw-r--r--   0        0        0     6405 2023-03-09 12:47:33.943158 oxalis-0.5.1/oxalis/redis.py
--rw-r--r--   0        0        0      950 2023-03-09 12:59:32.258051 oxalis-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     7847 1970-01-01 00:00:00.000000 oxalis-0.5.1/setup.py
--rw-r--r--   0        0        0     7976 1970-01-01 00:00:00.000000 oxalis-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.5.2/LICENSE
+-rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.5.2/README.md
+-rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.5.2/oxalis/__init__.py
+-rw-r--r--   0        0        0    10949 2023-04-20 05:15:02.504528 oxalis-0.5.2/oxalis/amqp.py
+-rw-r--r--   0        0        0     6836 2023-04-20 05:15:02.504528 oxalis-0.5.2/oxalis/base.py
+-rw-r--r--   0        0        0     1654 2022-07-12 02:08:37.164774 oxalis-0.5.2/oxalis/beater.py
+-rw-r--r--   0        0        0     3626 2023-04-20 05:15:02.504528 oxalis-0.5.2/oxalis/kafka.py
+-rw-r--r--   0        0        0     3506 2023-04-20 05:15:02.508527 oxalis-0.5.2/oxalis/pool.py
+-rw-r--r--   0        0        0     6575 2023-04-20 05:15:02.508527 oxalis-0.5.2/oxalis/redis.py
+-rw-r--r--   0        0        0      972 2023-04-20 05:15:15.440218 oxalis-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     7859 1970-01-01 00:00:00.000000 oxalis-0.5.2/setup.py
+-rw-r--r--   0        0        0     8003 1970-01-01 00:00:00.000000 oxalis-0.5.2/PKG-INFO
```

### Comparing `oxalis-0.5.1/LICENSE` & `oxalis-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.1/README.md` & `oxalis-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.1/oxalis/amqp.py` & `oxalis-0.5.2/oxalis/amqp.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,17 @@
     @property
     def channel(self) -> aio_pika.abc.AbstractChannel:
         if not self.channels:
             raise RuntimeError("Call connect first!")
         return self.channels[0]
 
     async def connect(self):
+        self.connection = self.connection.__class__(
+            self.connection.url, **self.connection.kwargs
+        )
         await self.connection.connect(timeout=self.timeout)
         channel = self.connection.channel()
         await channel.initialize(timeout=self.timeout)
         self.channels.append(channel)
         await self.declare(self.queues)
         await self.declare(self.exchanges)
         for q, e, k in self.bindings:
```

### Comparing `oxalis-0.5.1/oxalis/base.py` & `oxalis-0.5.2/oxalis/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 import typing as tp
 
 from .pool import Pool
 
 logger = logging.getLogger("oxalis")
 
 
+TASK_TV = tp.TypeVar("TASK_TV", bound="Task")
+
+
 class Task:
     def __init__(
         self,
         oxalis: Oxalis,
         func: tp.Callable,
         name="",
         timeout: float = -1,
@@ -154,14 +157,15 @@
         )
         await self.disconnect()
 
     def close_worker(self, force: bool = False):
         logger.info(f"Close worker{'(force)' if force else ''}: {self}...")
         self.running = False
         if force:
+            logger.warning(f"Force close: {self}, may lose some message!")
             for p in self.pools:
                 p.force_close()
             sys.exit()
 
     def register_task(self, task: Task):
         if task.name in self.tasks:
             raise ValueError("double task, check task name")
@@ -194,29 +198,39 @@
         if task_name not in self.tasks:
             logger.warning(f"Received task {task_name} not found")
             return None, False
         else:
             task = self.tasks[task_name]
             pool = task.pool
             if self.pool_wait_spawn:
-                await pool.wait_spawn(
+                if await pool.wait_spawn(
                     self.exec_task(task, *args, *task_args, **task_kwargs),
                     timeout=task.timeout,
-                )
+                ):
+                    return task, True
+                else:
+                    logger.warning(
+                        f"Spawn task to closed pool, message {task} may losed"
+                    )
+                    return task, False
             else:
                 if pool.running:
                     pool.spawn(
                         self.exec_task(task, *args, *task_args, **task_kwargs),
                         timeout=task.timeout,
                     )
+                    return task, True
                 else:
+                    logger.warning(
+                        f"Spawn task to closed pool, message {task} may losed"
+                    )
                     return task, False
-            return task, True
 
     def close(self, *_):
+        """Close self but wait pool"""
         if not self.is_worker:
             return
         self._on_close_signal_count += 1
         self.close_worker(force=self._on_close_signal_count >= 2)
 
     def on_worker_init(self):
         pass
```

### Comparing `oxalis-0.5.1/oxalis/beater.py` & `oxalis-0.5.2/oxalis/beater.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.1/oxalis/pool.py` & `oxalis-0.5.2/oxalis/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,21 +49,22 @@
         f = asyncio.ensure_future(asyncio.wait_for(coroutine, timeout=timeout))
         f.add_done_callback(self.on_future_done)
         self.futures.add(f)
         return f
 
     async def wait_spawn(
         self, coroutine: tp.Awaitable, timeout: float = -1
-    ) -> asyncio.Future:
-        while True:
+    ) -> tp.Optional[asyncio.Future]:
+        while self.running:
             f = self.spawn(coroutine, pending=False, timeout=timeout)
             if f:
                 return f
             else:
                 await self.done_queue.get()
+        return None
 
     @property
     def done(self) -> bool:
         return not (self.running_count or self.pending_queue.qsize())
 
     async def wait_done(self):
         while not self.done:
```

### Comparing `oxalis-0.5.1/oxalis/redis.py` & `oxalis-0.5.2/oxalis/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,34 +150,40 @@
                     except Exception as e:
                         logger.exception(e)
             if count < fetch_count:
                 await asyncio.sleep(time_offset)
 
     async def _receive_message(self, queue_names: tp.Set[str]):
         self._receiving = True
-        while self.running:
-            content = await self.client.blpop(list(queue_names), timeout=self.timeout)
-            if not content:
-                continue
-            else:
-                await self.on_message_receive(content[1])
-        self._receiving = False
+        try:
+            while self.running:
+                content = await self.client.blpop(
+                    list(queue_names), timeout=self.timeout
+                )
+                if not content:
+                    continue
+                else:
+                    await self.on_message_receive(content[1])
+        finally:
+            self._receiving = False
 
     async def _receive_pubsub_message(self, queue_names: tp.Set[str]):
-        while self.running:
-            if not self.pubsub.subscribed:
-                await self.pubsub.subscribe(*queue_names)
-            content = await self.pubsub.get_message(
-                ignore_subscribe_messages=True, timeout=self.timeout
-            )
-            if not content:
-                continue
-            else:
-                await self.on_message_receive(content["data"])
-        await self.pubsub.close()
+        try:
+            while self.running:
+                if not self.pubsub.subscribed:
+                    await self.pubsub.subscribe(*queue_names)
+                content = await self.pubsub.get_message(
+                    ignore_subscribe_messages=True, timeout=self.timeout
+                )
+                if not content:
+                    continue
+                else:
+                    await self.on_message_receive(content["data"])
+        finally:
+            await self.pubsub.close()
 
     def _run_worker(self):
         """
         Limit queue consume concurrency by pool
         """
         queue_names = defaultdict(set)
         pubsub_queue_names = defaultdict(set)
```

### Comparing `oxalis-0.5.1/pyproject.toml` & `oxalis-0.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxalis"
-version = "0.5.1"
+version = "0.5.2"
 description = "Distributed async task/job queue"
 authors = ["strongbugman <strongbugman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     "Environment :: Console",
     "Programming Language :: Python :: 3.7",
@@ -18,15 +18,16 @@
     { include = "oxalis" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 aio-pika = ">=8.0.3"
 croniter = ">=1.3.5"
-redis = "^4.5.1"
+redis = ">=4.5.1"
+aiokafka = ">=0.8.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=4.6"
 pytest-asyncio = ">=0.8.0"
 pytest-cov = ">=2.5.1"
 mypy = ">=0.910"
 flake8 = ">=3.9.2"
```

### Comparing `oxalis-0.5.1/setup.py` & `oxalis-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['oxalis']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aio-pika>=8.0.3', 'croniter>=1.3.5', 'redis>=4.5.1,<5.0.0']
+['aio-pika>=8.0.3', 'aiokafka>=0.8.0', 'croniter>=1.3.5', 'redis>=4.5.1']
 
 setup_kwargs = {
     'name': 'oxalis',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': 'Distributed async task/job queue',
     'long_description': '<p>\n<a href="https://pypi.org/project/oxalis/">\n    <img src="https://badge.fury.io/py/oxalis.svg" alt="Package version">\n</a>\n</p>\n\n# Oxalis  \n\nDistributed async task/job queue, like Celery for `asyncio` world\n\n## Feature\n\n* Redis and AMQP(RabbitMQ etc.) support\n* Task timeout and concurrency limit support\n* Delayed task(Both Redis and RabbitMQ) support\n* Cron task/job beater\n* Built-in coroutine pool with concurrency and time limit\n\n## Install\n\n```pip install oxalis```\n\n## Example with Redis backend\n\nDefine task:\n```python\nfrom redis.asyncio.client import Redis\nfrom oxalis.redis import Oxalis\n\n\noxalis = Oxalis(Redis(host=os.getenv("REDIS_HOST", "redis")))\n\n@oxalis.register()\nasync def hello_task():\n    print("Hello oxalis")\n```\n\nRun worker(consumer):\n```python\noxalis.run_worker_master()\n```\n\n```shell\npython ex.py\nINFO:oxalis:Registered Task: <Task(hello_task)>\nINFO:oxalis:Run worker: <Oxalis(pid-101547)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101548)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101549)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101550)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101551)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101552)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101554)>...\n```\n\nRun client(producer):\n```python\nimport asyncio\n\nasyncio.get_event_loop().run_until_complete(oxalis.connect())\nfor i in range(10):\n    asyncio.get_event_loop().run_until_complete(hello_task.delay())\n    asyncio.get_event_loop().run_until_complete(hello_task.delay(_delay=1))  # delay execution after 1s\n```\n\nRun cron beater:\n```python\nfrom oxalis.beater import Beater\n\nbeater = Beater(oxalis)\n\nbeater.register("*/1 * * * *", hello_task)\nbeater.run()\n```\n```shell\npython exb.py \nINFO:oxalis:Beat task: <Task(hello_task)> at <*/1 * * * *> ...\n```\n\n## TaskCodec\n\nThe `TaskCodec` will encode/decode task args, default codec will use `json`\n\nCustom task codec:\n```python\nfrom oxalis.base import TaskCodec\n\nclass MyTaskCodec(TaskCodec):\n    @classmethod\n    def encode(\n        cls,\n        task: Task,\n        task_args: tp.Sequence[tp.Any],\n        task_kwargs: tp.Dict[str, tp.Any],\n    ) -> bytes:\n        ...\n\n    @classmethod\n    def decode(cls, content: bytes) -> TaskCodec.MESSAGE_TYPE:\n        ...\n\n\n\noxalis = Oxalis(Redis(host=os.getenv("REDIS_HOST", "redis")), task_codec=MyTaskCodec())\n...\n```\n\n\n## Task pool\n\nOxalis use one coroutine pool with concurrency limit and timeout limit to run all task\n\nCustom pool:\n\n```python\nfrom redis.asyncio.client import Redis\nfrom oxalis.redis import Oxalis\nfrom oxalis.pool import Pool\n\noxalis = Oxalis(Redis(host=os.getenv("REDIS_HOST", "redis")), pool=Pool(concurrency=10, timeout=60))\n```\n\n* For Redis task, the `queue` will be blocked util `pool` is not fully loaded\n* For AMQP task, oxalis use AMQP\'s QOS to limit worker concurrency(`pool`\'s concurrency will be -1 which means the pool\'s concurrency will not be limited)\n* `asyncio.TimeoutError` will be raised if one task is timeout\n* Every worker process has owned limited pool\n\n\nSpecified one task timeout limit:\n```python\n@oxalis.register(queue=custom_queue, timeout=10)\ndef custom_task():\n    print("Hello oxalis")\n```\n\n## Custom hook\n\nOxalis defined some hook API for inherited subclass:\n```python\nclass MyOxalis(Oxalis):\n    def on_worker_init():\n        # will be called before worker started\n        pass\n\n    def on_worker_close():\n        # will be called after worker started\n        pass\n```\n\nSome API can be rewritten or inherited for custom usage, eg:\n```python\nimport sentry_sdk\n\nclass MyOxalis(Oxalis):\n    async def exec_task(self, task: Task, *task_args, **task_kwargs):\n        """\n        capture exception to sentry\n        """\n        try:\n            await super().exec_task(task, *task_args, **task_kwargs)\n        except Exception as e:\n            sentry_sdk.capture_exception(e)\n```\n\n\n## Redis Backend Detail\n\nOxalis use redis\'s `list` and `pubsub` structure as a message queue\n\n### Queue\n\nCustom queue:\n```python\nfrom oxalis.redis import Queue, PubsubQueue\n\ncustom_queue = Queue("custom")\nbus_queue = PubsubQueue("bus")\n```\n\nRegister task:\n```python\n@oxalis.register(queue=custom_queue)\ndef custom_task():\n    print("Hello oxalis")\n\n@oxalis.register(queue=bus_queue)\ndef bus_task():\n    print("Hello oxalis")\n```\n\n* For task producer, the task will send to specified queue when call `task.delay()`\n* For task consumer, oxalis will listen those queues and receive task from them\n\n### Concurrency limit\n\nOxalis using coroutine pool\'s concurrency limit way, we can set different concurrency limit with specified pool for one task:\n\n```python\n@oxalis.register(pool=Pool(concurrency=1))\ndef custom_task():\n    print("Hello oxalis")\n```\n\n### Delayed task\n\nSupport by redis [zset](https://redis.com/ebook/part-2-core-concepts/chapter-6-application-components-in-redis/6-4-task-queues/6-4-2-delayed-tasks/)\n\n##  AMQP Backend Detail\n\n\n### Custom Queue and Exchange\n\nOxalis using AMQP\'s way to define Exchange, Queue and their bindings\n\n```python\nimport asyncio\nimport logging\nimport time\n\nfrom aio_pika import RobustConnection\nfrom oxalis.amqp import Exchange, ExchangeType, Oxalis, Pool, Queue\n\ne = Exchange("test")\nq = Queue("test", durable=False)\ne2 = Exchange("testfanout", type=ExchangeType.FANOUT)\nq2 = Queue("testfanout", durable=False)\n\n\noxalis = Oxalis(RobustConnection("amqp://root:letmein@rabbitmq:5672/"))\noxalis.register_binding(q, e, "test")\noxalis.register_binding(q2, e2, "")\noxalis.register_queues([q, q2])\n\n\n@oxalis.register(exchange=e, routing_key="test")\nasync def task1():\n    await asyncio.sleep(1)\n    print("hello oxalis")\n\n\n@oxalis.register(exchange=e2)\nasync def task2():\n    await asyncio.sleep(10)\n    print("hello oxalis")\n\n```\n\n* For producer, task `oxalis.register`  defined one task message will send to which exchange(by routing key)\n* For consumer, `register_queues` defined which queues oxalis will listened\n* Task routing defined by bindings\n\n### Concurrency limit\n\nOxalis use AMQP\'s QOS to limit worker concurrency(Task\'s `ack_later` should be true), so coroutine pool\'s concurrency should not be limited.\n\nCustom queue QOS:\n```python\noxalis = Oxalis(RobustConnection("amqp://root:letmein@rabbitmq:5672/"), default_queue=Queue("custom",consumer_prefetch_count=10))\n...\nfanout_queue = Queue("testfanout", durable=False, consumer_prefetch_count=3)\noxalis.register_queues([fanout_queue])\n...\n```\n\n### Custom task behavior\n\nDefine task how to perform `ack` and `reject` \n\n```python\n# always ack even task failed(raise exception)\n@oxalis.register(ack_always=True, reject=False)\nasync def task2():\n    await asyncio.sleep(10)\n    print("hello oxalis")\n\n#  reject with requeue when task failed\n@oxalis.register(reject_requeue=True)\nasync def task2():\n    await asyncio.sleep(10)\n    print("hello oxalis")\n```\n\n### Delayed task\n\nSupport by RabbitMq\'s [plugin](https://blog.rabbitmq.com/posts/2015/04/scheduling-messages-with-rabbitmq)\n',
     'author': 'strongbugman',
     'author_email': 'strongbugman@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['oxalis']
 package_data = \ {'': ['*']} install_requires = \ ['aio-pika>=8.0.3',
-'croniter>=1.3.5', 'redis>=4.5.1,<5.0.0'] setup_kwargs = { 'name': 'oxalis',
-'version': '0.5.1', 'description': 'Distributed async task/job queue',
-'long_description': '
+'aiokafka>=0.8.0', 'croniter>=1.3.5', 'redis>=4.5.1'] setup_kwargs = { 'name':
+'oxalis', 'version': '0.5.2', 'description': 'Distributed async task/job
+queue', 'long_description': '
 \n\n_[Package_version]\n\n
 \n\n# Oxalis \n\nDistributed async task/job queue, like Celery for `asyncio`
 world\n\n## Feature\n\n* Redis and AMQP(RabbitMQ etc.) support\n* Task timeout
 and concurrency limit support\n* Delayed task(Both Redis and RabbitMQ)
 support\n* Cron task/job beater\n* Built-in coroutine pool with concurrency and
 time limit\n\n## Install\n\n```pip install oxalis```\n\n## Example with Redis
 backend\n\nDefine task:\n```python\nfrom redis.asyncio.client import
```

### Comparing `oxalis-0.5.1/PKG-INFO` & `oxalis-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxalis
-Version: 0.5.1
+Version: 0.5.2
 Summary: Distributed async task/job queue
 License: MIT
 Author: strongbugman
 Author-email: strongbugman@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -17,16 +17,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aio-pika (>=8.0.3)
+Requires-Dist: aiokafka (>=0.8.0)
 Requires-Dist: croniter (>=1.3.5)
-Requires-Dist: redis (>=4.5.1,<5.0.0)
+Requires-Dist: redis (>=4.5.1)
 Description-Content-Type: text/markdown
 
 <p>
 <a href="https://pypi.org/project/oxalis/">
     <img src="https://badge.fury.io/py/oxalis.svg" alt="Package version">
 </a>
 </p>
```

