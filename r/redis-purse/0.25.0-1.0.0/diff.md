# Comparing `tmp/redis-purse-0.25.0.tar.gz` & `tmp/redis_purse-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-purse-0.25.0.tar", max compression
+gzip compressed data, was "redis_purse-1.0.0.tar", max compression
```

## Comparing `redis-purse-0.25.0.tar` & `redis_purse-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    11380 2021-10-25 12:47:57.112000 redis-purse-0.25.0/LICENSE
--rw-r--r--   0        0        0     6917 2021-11-28 22:49:14.452925 redis-purse-0.25.0/README.md
--rw-r--r--   0        0        0     1441 2022-11-23 15:24:10.271931 redis-purse-0.25.0/pyproject.toml
--rw-r--r--   0        0        0      370 2022-01-02 14:59:19.176983 redis-purse-0.25.0/src/purse/__init__.py
--rw-r--r--   0        0        0    40771 2022-01-05 15:39:46.521733 redis-purse-0.25.0/src/purse/collections.py
--rw-r--r--   0        0        0        0 2021-09-15 18:36:12.217000 redis-purse-0.25.0/src/purse/py.typed
--rw-r--r--   0        0        0    13554 2021-11-28 22:32:18.037634 redis-purse-0.25.0/src/purse/redlock.py
--rw-r--r--   0        0        0     7864 2022-11-23 15:26:29.517545 redis-purse-0.25.0/setup.py
--rw-r--r--   0        0        0     7786 2022-11-23 15:26:29.518222 redis-purse-0.25.0/PKG-INFO
+-rw-r--r--   0        0        0    11380 2021-10-25 12:47:57.000000 redis_purse-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6999 2023-04-20 13:58:16.641280 redis_purse-1.0.0/README.md
+-rw-r--r--   0        0        0     1442 2023-04-20 13:40:10.467231 redis_purse-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      370 2022-01-02 14:59:19.000000 redis_purse-1.0.0/src/purse/__init__.py
+-rw-r--r--   0        0        0    40776 2023-04-20 13:51:55.485451 redis_purse-1.0.0/src/purse/collections.py
+-rw-r--r--   0        0        0        0 2021-09-15 18:36:12.000000 redis_purse-1.0.0/src/purse/py.typed
+-rw-r--r--   0        0        0    13525 2023-04-20 13:52:56.094040 redis_purse-1.0.0/src/purse/redlock.py
+-rw-r--r--   0        0        0     7966 1970-01-01 00:00:00.000000 redis_purse-1.0.0/PKG-INFO
```

### Comparing `redis-purse-0.25.0/LICENSE` & `redis_purse-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-purse-0.25.0/README.md` & `redis_purse-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,31 +13,39 @@
   * Due to the ``async/await`` nature of the API, it is difficult and sometimes impossible to use python language constructs such as ``myhash["key"] = "value"`` - 
     as of Python 3.10, the language simply doesn't provide async-io methods for those operations and idioms 
   * ``purse`` tries to expose, as much as possible, Redis rich features such as key TTL and pattern matching, among others
 
 Optionally, collections in this library use [pydantic](https://github.com/samuelcolvin/pydantic) 
 to serialize, validate, and deserialize Python Models part of all data storage and retrieval operations
 
+# installation
+
+with pip
+
+```bash
+pip install redis-purse
+```
+
 # Basic Usage
 
 ## RedisList
 
 RedisList provides an API that provides most methods and features of the python ``list`` and ``deque``
 
 ```python
 import asyncio
 from purse.collections import RedisList
-import aioredis
+from redis.asyncio import Redis
 
 
 async def main():
     local_list = ['a', 'b', 'c', 'd', 'e', 'f']
 
     # local Redis >= 6.0.x plain connection with default params
-    red_con = aioredis.Redis()
+    red_con = Redis()
     redis_key = 'redis_list'
 
     # The value_type defines the class to serialize to and from
     redis_list = RedisList(redis=red_con, rkey=redis_key, value_type=str)
 
     # Clear the list, in case it was previously populated
     await redis_list.clear()
@@ -78,26 +86,26 @@
 ## RedisHash
 
 Provides most of the functionality of the Python ``dict``. 
 
 ```python
 import asyncio
 from purse.collections import RedisHash
-import aioredis
+from redis.asyncio import Redis
 from pydantic import BaseModel
 
 
 async def main():
     # Pydantic Model
     class Plant(BaseModel):
         name: str
         healthiness: float
         tasty: bool
 
-    red_con = aioredis.Redis()
+    red_con = Redis()
     redis_key = 'redis_hash'
 
     # This class serializes and deserializes Plant Model objects when storing and retrieving data
     redis_hash = RedisHash(red_con, redis_key, Plant)
     await redis_hash.clear()
 
     plants = [
@@ -143,15 +151,15 @@
 to the last numerical item of that Redis List, with some asyncio delay to simulate real world
 latencies and data processing times.
 
 ```python
 import asyncio
 from purse.redlock import Redlock
 from purse.collections import RedisList
-from aioredis import Redis
+from redis.asyncio import Redis
 from random import random
 
 # The main Redis Store that contains the data that need synchronization
 redis_store = Redis(db=0)
 
 # The Redis Masters for the async Redlock
 # Highly Recommended to be an odd number of masters: typically 1, 3 or 5 masters
```

### Comparing `redis-purse-0.25.0/pyproject.toml` & `redis_purse-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "redis-purse"
-version = "0.25.0"
+version = "1.0.0"
 description = "High Level Asyncio interface to redis"
 license = "Apache-2.0"
 authors = ["mk <mk@plataux.com>"]
 maintainers = []
 readme = "README.md"
 homepage = "https://plataux.com"
 repository = "https://github.com/plataux/purse"
@@ -20,26 +20,26 @@
 ]
 packages = [
     { include = "purse", from = "src" },
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pydantic = "^1.9"
-aioredis = "^2"
+python = ">=3.8,<4"
+pydantic = "^1.10"
+redis = "^4.5"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0"
 tox = "^3.24"
-pytest = "^6.2"
-pytest-cov = "^3.0"
-mypy = "^0.910"
-sphinx = "^4.2"
-sphinx-rtd-theme = "^1.0"
+pytest = "^7.3"
+pytest-cov = "^4.0"
+mypy = "^1.2"
+sphinx = "^4.4"
+sphinx-rtd-theme = "^1.2"
 recommonmark = "^0.7"
 
 [build-system]
 requires = ["setuptools>=42.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
```

### Comparing `redis-purse-0.25.0/src/purse/collections.py` & `redis_purse-1.0.0/src/purse/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from __future__ import annotations
 
 import asyncio
 import json
 from datetime import timedelta
 
-from aioredis import Redis
+from redis.asyncio import Redis
 from typing import Any, Dict, Type, Union, Tuple, Iterable, List
 from typing import TypeVar, Generic
 from collections.abc import Mapping, AsyncIterator
 from pydantic import BaseModel
 
 from uuid import uuid4
 
@@ -626,15 +626,15 @@
         elif issubclass(self._value_type, str):
 
             async def _typed_iter():
                 async for k3, v3 in raw_it:
                     if isinstance(v3, bytes):
                         yield k3.decode(), v3.decode()
                     else:
-                        yield v3, v3.decode()
+                        yield k3, v3
 
         else:
 
             async def _typed_iter():
                 async for k4, v4 in raw_it:
                     if isinstance(v4, str):
                         yield k4.decode(), v4.encode()
@@ -1073,15 +1073,15 @@
         self._value_type: Type[T] = value_type
 
     async def put(self, item: T):
         return await self.redis.lpush(self.rkey, _obj_to_raw(self._value_type, item))
 
     async def get(self, timeout: float = 0) -> T:
         t: Any = timeout
-        res = await self.redis.brpop(self.rkey, timeout=t)
+        _, res = await self.redis.brpop(self.rkey, timeout=t)
 
         if res is None:
             raise asyncio.QueueEmpty("RedisQueue Empty")
 
         return _obj_from_raw(self._value_type, res)
 
     async def get_nowait(self) -> T:
@@ -1108,15 +1108,15 @@
         self._value_type: Type[T] = value_type
 
     async def put(self, item: T):
         return await self.redis.rpush(self.rkey, _obj_to_raw(self._value_type, item))
 
     async def get(self, timeout: float = 0) -> T:
         t: Any = timeout
-        res = await self.redis.brpop(self.rkey, timeout=t)
+        _, res = await self.redis.brpop(self.rkey, timeout=t)
 
         if res is None:
             raise asyncio.QueueEmpty("RedisQueue Empty")
 
         return _obj_from_raw(self._value_type, res)
 
     async def get_nowait(self) -> T:
@@ -1152,15 +1152,15 @@
 
         if res is None:
             raise asyncio.QueueEmpty("RedisQueue Empty")
 
         return _obj_from_raw(self._value_type, res[1][37:]), int(res[2])
 
     async def get_nowait(self) -> Tuple[T, int]:
-        res = await self.redis.zpopmin(self.rkey)
+        _, res = await self.redis.zpopmin(self.rkey)
 
         if res is None:
             raise asyncio.QueueEmpty("RedisQueue Empty")
 
         return _obj_from_raw(self._value_type, res[1][37:]), int(res[2])
 
     async def qsize(self):
```

### Comparing `redis-purse-0.25.0/src/purse/redlock.py` & `redis_purse-1.0.0/src/purse/redlock.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 
 from __future__ import annotations
 
 import contextlib
 from types import TracebackType
 
-from aioredis import Redis, RedisError
-from aioredis.client import Script
+from redis.asyncio import Redis, RedisError
+
 from typing import List, Optional, Literal, Type
 from uuid import uuid4
 import asyncio
 import random
 
 from time import time_ns
```

### Comparing `redis-purse-0.25.0/setup.py` & `redis_purse-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,238 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: redis-purse
+Version: 1.0.0
+Summary: High Level Asyncio interface to redis
+Home-page: https://plataux.com
+License: Apache-2.0
+Keywords: key-value,caching,messaging
+Author: mk
+Author-email: mk@plataux.com
+Requires-Python: >=3.8,<4
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: pydantic (>=1.10,<2.0)
+Requires-Dist: redis (>=4.5,<5.0)
+Project-URL: Repository, https://github.com/plataux/purse
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
 
-packages = \
-['purse']
+# Purse
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aioredis>=2,<3', 'pydantic>=1.9,<2.0']
-
-setup_kwargs = {
-    'name': 'redis-purse',
-    'version': '0.25.0',
-    'description': 'High Level Asyncio interface to redis',
-    'long_description': '\n# Purse\n\nHigh-Level Async-IO Python interface for Redis 6.0.x that provides useful Pythonic abstractions to simplify \nthe usage of Redis as a non-blocking Caching layer, or even as a first-class non-blocking datastore.\n\nInfluenced and Inspired by the great library [pottery](https://github.com/brainix/pottery), with\na few differences in objectives and implementation detail.\n\n* ``purse`` is strictly an Async-IO library that utilizes the excellent Python Redis driver library [aioredis](https://github.com/aio-libs/aioredis-py)\n* ``purse`` tries to adhere as much as possible to familiar APIs and idioms used with familiar python structures\n  (``dict``, ``set``, ``list`` among others), but deviates from those conventions in many instances:\n  * Due to the ``async/await`` nature of the API, it is difficult and sometimes impossible to use python language constructs such as ``myhash["key"] = "value"`` - \n    as of Python 3.10, the language simply doesn\'t provide async-io methods for those operations and idioms \n  * ``purse`` tries to expose, as much as possible, Redis rich features such as key TTL and pattern matching, among others\n\nOptionally, collections in this library use [pydantic](https://github.com/samuelcolvin/pydantic) \nto serialize, validate, and deserialize Python Models part of all data storage and retrieval operations\n\n# Basic Usage\n\n## RedisList\n\nRedisList provides an API that provides most methods and features of the python ``list`` and ``deque``\n\n```python\nimport asyncio\nfrom purse.collections import RedisList\nimport aioredis\n\n\nasync def main():\n    local_list = [\'a\', \'b\', \'c\', \'d\', \'e\', \'f\']\n\n    # local Redis >= 6.0.x plain connection with default params\n    red_con = aioredis.Redis()\n    redis_key = \'redis_list\'\n\n    # The value_type defines the class to serialize to and from\n    redis_list = RedisList(redis=red_con, rkey=redis_key, value_type=str)\n\n    # Clear the list, in case it was previously populated\n    await redis_list.clear()\n\n    # extend a Redis list with a Python list\n    await redis_list.extend(local_list)\n\n    # async list comprehension\n    print([x async for x in redis_list])\n\n    # contains\n    print(await redis_list.contains(\'f\'))  # True\n    print(await redis_list.contains(\'g\'))  # False\n\n    # getting the index of a value\n    print(await redis_list.index(\'c\'))  # 2\n    print(await redis_list.index(\'g\'))  # None, unlike a Python list that raises a ValueError\n\n    # slicing\n    print(await redis_list.slice(2, 5))  # [\'c\', \'d\', \'e\']\n\n    # inserting values\n    await redis_list.insert(2, \'x\')\n    await redis_list.insert(-2, \'y\')\n\n    # getitem\n    assert await redis_list.getitem(2) == \'x\'\n    assert await redis_list.getitem(-3) == \'y\'\n\n    # some deque methods\n    await redis_list.appendleft(\'z\')\n    await redis_list.pop()\n    await redis_list.popleft()\n\nasyncio.run(main())\n```\n\n## RedisHash\n\nProvides most of the functionality of the Python ``dict``. \n\n```python\nimport asyncio\nfrom purse.collections import RedisHash\nimport aioredis\nfrom pydantic import BaseModel\n\n\nasync def main():\n    # Pydantic Model\n    class Plant(BaseModel):\n        name: str\n        healthiness: float\n        tasty: bool\n\n    red_con = aioredis.Redis()\n    redis_key = \'redis_hash\'\n\n    # This class serializes and deserializes Plant Model objects when storing and retrieving data\n    redis_hash = RedisHash(red_con, redis_key, Plant)\n    await redis_hash.clear()\n\n    plants = [\n        Plant(name="spinach", healthiness=9.8, tasty=False),\n        Plant(name="broccoli", healthiness=12.2, tasty=True),\n        Plant(name="lettuce", healthiness=3, tasty=False),\n        Plant(name="avocado", healthiness=8, tasty=True),\n    ]\n\n    # update redis hash with a python dict\n    await redis_hash.update({p.name: p for p in plants})\n\n    await redis_hash.set("carrot", Plant(name="carrot", healthiness=5, tasty=False))\n\n    print(await redis_hash.len())  # currently 5 mappings in total\n    \n    #  RedisHash is a generic type with supports IDE intellisense and type hints\n    p: Plant = await redis_hash.get(\'spinach\')\n    \n    print(p.tasty)  # False\n    \n    # async for syntax\n    async for name, plant in redis_hash.items():\n        print(name, plant)\n\nasyncio.run(main())\n```\n\n## Redlock\n\nDistributed, None-blocking Lock implementation according to the algorithm and logic described here\nhttps://redis.io/topics/distlock, and closely resembling the python implementation here\nhttps://github.com/brainix/pottery/blob/master/pottery/redlock.py.\n\nThis none-blocking implementation is particularly efficient and attractive when a real world\ndistributed application is using many distributed locks over many Redis Masters,\nto synchronize on many Network Resources simultaneously, due to the very small overhead associated with\nasyncio tasks, and any "waiting" that may need to happen to acquire locks, since all of the above\nis happening efficiently on an event-queue.\n\nThis example uses 5 Redis databases on the localhost as the Redlock Masters, to synchronize on\nthe access of a RedisList, where multiple tasks are concurrently synchronizing getting, incrementing and appending\nto the last numerical item of that Redis List, with some asyncio delay to simulate real world\nlatencies and data processing times.\n\n```python\nimport asyncio\nfrom purse.redlock import Redlock\nfrom purse.collections import RedisList\nfrom aioredis import Redis\nfrom random import random\n\n# The main Redis Store that contains the data that need synchronization\nredis_store = Redis(db=0)\n\n# The Redis Masters for the async Redlock\n# Highly Recommended to be an odd number of masters: typically 1, 3 or 5 masters\nredlock_masters = [Redis(db=x) for x in range(5)]\n\n\nasync def do_job(n):\n\n    rlock = Redlock("redlock:list_lock", redlock_masters)\n    rlist = RedisList(redis_store, "redis_list", str)\n\n    for x in range(n):\n        async with rlock:\n            cl = await rlist.len()\n\n            if cl == 0:\n                await rlist.append("0")\n                current_num = 0\n            else:\n                current_num = int(await rlist.getitem(-1))\n\n            # This sleep simulates the processing time of the job - up to 100ms here\n            await asyncio.sleep(0.1 * random())\n\n            # Get the job done, which is add 1 to the last number\n            current_num += 1\n\n            print(f"the task {asyncio.current_task().get_name()} working on item #: {current_num}")\n\n            await rlist.append(str(current_num))\n\n\nasync def main():\n    rlist = RedisList(redis_store, "redis_list", str)\n    await rlist.clear()\n\n    # run 10 async threads (or tasks) in parallel, each one to perform 10 increments\n    await asyncio.gather(\n        *[asyncio.create_task(do_job(10)) for _ in range(10)]\n    )\n\n    # should print 0 to 100 in order, which means synchronization has happened\n    async for item in rlist:\n        print(item)\n\n    return "success"\n\nasyncio.run(main())\n```\n\n',
-    'author': 'mk',
-    'author_email': 'mk@plataux.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://plataux.com',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+High-Level Async-IO Python interface for Redis 6.0.x that provides useful Pythonic abstractions to simplify 
+the usage of Redis as a non-blocking Caching layer, or even as a first-class non-blocking datastore.
+
+Influenced and Inspired by the great library [pottery](https://github.com/brainix/pottery), with
+a few differences in objectives and implementation detail.
+
+* ``purse`` is strictly an Async-IO library that utilizes the excellent Python Redis driver library [aioredis](https://github.com/aio-libs/aioredis-py)
+* ``purse`` tries to adhere as much as possible to familiar APIs and idioms used with familiar python structures
+  (``dict``, ``set``, ``list`` among others), but deviates from those conventions in many instances:
+  * Due to the ``async/await`` nature of the API, it is difficult and sometimes impossible to use python language constructs such as ``myhash["key"] = "value"`` - 
+    as of Python 3.10, the language simply doesn't provide async-io methods for those operations and idioms 
+  * ``purse`` tries to expose, as much as possible, Redis rich features such as key TTL and pattern matching, among others
+
+Optionally, collections in this library use [pydantic](https://github.com/samuelcolvin/pydantic) 
+to serialize, validate, and deserialize Python Models part of all data storage and retrieval operations
+
+# installation
+
+with pip
+
+```bash
+pip install redis-purse
+```
+
+# Basic Usage
+
+## RedisList
+
+RedisList provides an API that provides most methods and features of the python ``list`` and ``deque``
+
+```python
+import asyncio
+from purse.collections import RedisList
+from redis.asyncio import Redis
+
+
+async def main():
+    local_list = ['a', 'b', 'c', 'd', 'e', 'f']
+
+    # local Redis >= 6.0.x plain connection with default params
+    red_con = Redis()
+    redis_key = 'redis_list'
+
+    # The value_type defines the class to serialize to and from
+    redis_list = RedisList(redis=red_con, rkey=redis_key, value_type=str)
+
+    # Clear the list, in case it was previously populated
+    await redis_list.clear()
+
+    # extend a Redis list with a Python list
+    await redis_list.extend(local_list)
+
+    # async list comprehension
+    print([x async for x in redis_list])
+
+    # contains
+    print(await redis_list.contains('f'))  # True
+    print(await redis_list.contains('g'))  # False
+
+    # getting the index of a value
+    print(await redis_list.index('c'))  # 2
+    print(await redis_list.index('g'))  # None, unlike a Python list that raises a ValueError
+
+    # slicing
+    print(await redis_list.slice(2, 5))  # ['c', 'd', 'e']
+
+    # inserting values
+    await redis_list.insert(2, 'x')
+    await redis_list.insert(-2, 'y')
+
+    # getitem
+    assert await redis_list.getitem(2) == 'x'
+    assert await redis_list.getitem(-3) == 'y'
+
+    # some deque methods
+    await redis_list.appendleft('z')
+    await redis_list.pop()
+    await redis_list.popleft()
+
+asyncio.run(main())
+```
+
+## RedisHash
+
+Provides most of the functionality of the Python ``dict``. 
+
+```python
+import asyncio
+from purse.collections import RedisHash
+from redis.asyncio import Redis
+from pydantic import BaseModel
+
+
+async def main():
+    # Pydantic Model
+    class Plant(BaseModel):
+        name: str
+        healthiness: float
+        tasty: bool
+
+    red_con = Redis()
+    redis_key = 'redis_hash'
+
+    # This class serializes and deserializes Plant Model objects when storing and retrieving data
+    redis_hash = RedisHash(red_con, redis_key, Plant)
+    await redis_hash.clear()
+
+    plants = [
+        Plant(name="spinach", healthiness=9.8, tasty=False),
+        Plant(name="broccoli", healthiness=12.2, tasty=True),
+        Plant(name="lettuce", healthiness=3, tasty=False),
+        Plant(name="avocado", healthiness=8, tasty=True),
+    ]
+
+    # update redis hash with a python dict
+    await redis_hash.update({p.name: p for p in plants})
+
+    await redis_hash.set("carrot", Plant(name="carrot", healthiness=5, tasty=False))
+
+    print(await redis_hash.len())  # currently 5 mappings in total
+    
+    #  RedisHash is a generic type with supports IDE intellisense and type hints
+    p: Plant = await redis_hash.get('spinach')
+    
+    print(p.tasty)  # False
+    
+    # async for syntax
+    async for name, plant in redis_hash.items():
+        print(name, plant)
+
+asyncio.run(main())
+```
+
+## Redlock
+
+Distributed, None-blocking Lock implementation according to the algorithm and logic described here
+https://redis.io/topics/distlock, and closely resembling the python implementation here
+https://github.com/brainix/pottery/blob/master/pottery/redlock.py.
+
+This none-blocking implementation is particularly efficient and attractive when a real world
+distributed application is using many distributed locks over many Redis Masters,
+to synchronize on many Network Resources simultaneously, due to the very small overhead associated with
+asyncio tasks, and any "waiting" that may need to happen to acquire locks, since all of the above
+is happening efficiently on an event-queue.
+
+This example uses 5 Redis databases on the localhost as the Redlock Masters, to synchronize on
+the access of a RedisList, where multiple tasks are concurrently synchronizing getting, incrementing and appending
+to the last numerical item of that Redis List, with some asyncio delay to simulate real world
+latencies and data processing times.
+
+```python
+import asyncio
+from purse.redlock import Redlock
+from purse.collections import RedisList
+from redis.asyncio import Redis
+from random import random
+
+# The main Redis Store that contains the data that need synchronization
+redis_store = Redis(db=0)
+
+# The Redis Masters for the async Redlock
+# Highly Recommended to be an odd number of masters: typically 1, 3 or 5 masters
+redlock_masters = [Redis(db=x) for x in range(5)]
+
+
+async def do_job(n):
+
+    rlock = Redlock("redlock:list_lock", redlock_masters)
+    rlist = RedisList(redis_store, "redis_list", str)
+
+    for x in range(n):
+        async with rlock:
+            cl = await rlist.len()
+
+            if cl == 0:
+                await rlist.append("0")
+                current_num = 0
+            else:
+                current_num = int(await rlist.getitem(-1))
+
+            # This sleep simulates the processing time of the job - up to 100ms here
+            await asyncio.sleep(0.1 * random())
+
+            # Get the job done, which is add 1 to the last number
+            current_num += 1
+
+            print(f"the task {asyncio.current_task().get_name()} working on item #: {current_num}")
+
+            await rlist.append(str(current_num))
+
+
+async def main():
+    rlist = RedisList(redis_store, "redis_list", str)
+    await rlist.clear()
+
+    # run 10 async threads (or tasks) in parallel, each one to perform 10 increments
+    await asyncio.gather(
+        *[asyncio.create_task(do_job(10)) for _ in range(10)]
+    )
+
+    # should print 0 to 100 in order, which means synchronization has happened
+    async for item in rlist:
+        print(item)
+
+    return "success"
+
+asyncio.run(main())
+```
 
 
-setup(**setup_kwargs)
```

