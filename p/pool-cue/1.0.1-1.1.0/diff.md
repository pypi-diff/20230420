# Comparing `tmp/pool_cue-1.0.1.tar.gz` & `tmp/pool_cue-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pool_cue-1.0.1.tar", max compression
+gzip compressed data, was "pool_cue-1.1.0.tar", max compression
```

## Comparing `pool_cue-1.0.1.tar` & `pool_cue-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1065 2023-04-19 13:28:07.967658 pool_cue-1.0.1/LICENSE
--rw-r--r--   0        0        0     1416 2023-04-19 13:28:07.967658 pool_cue-1.0.1/README.md
--rw-r--r--   0        0        0      309 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/__init__.py
--rw-r--r--   0        0        0      938 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/config.py
--rw-r--r--   0        0        0     1053 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/context.py
--rw-r--r--   0        0        0      158 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/exceptions.py
--rw-r--r--   0        0        0     5808 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/jobs.py
--rw-r--r--   0        0        0     3472 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/queue.py
--rw-r--r--   0        0        0      426 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/serializers.py
--rw-r--r--   0        0        0     2358 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/threading.py
--rw-r--r--   0        0        0      968 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/typing.py
--rw-r--r--   0        0        0      984 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/utils.py
--rw-r--r--   0        0        0     3967 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pool_cue/worker.py
--rw-r--r--   0        0        0      666 2023-04-19 13:28:07.967658 pool_cue-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 pool_cue-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-20 07:47:24.577156 pool_cue-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1417 2023-04-20 07:47:24.577156 pool_cue-1.1.0/README.md
+-rw-r--r--   0        0        0      309 2023-04-20 07:47:24.577156 pool_cue-1.1.0/pool_cue/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-20 07:47:24.577156 pool_cue-1.1.0/pool_cue/config.py
+-rw-r--r--   0        0        0     1053 2023-04-20 07:47:24.577156 pool_cue-1.1.0/pool_cue/context.py
+-rw-r--r--   0        0        0      158 2023-04-20 07:47:24.577156 pool_cue-1.1.0/pool_cue/exceptions.py
+-rw-r--r--   0        0        0     5709 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/jobs.py
+-rw-r--r--   0        0        0     3451 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/queue.py
+-rw-r--r--   0        0        0      426 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/serializers.py
+-rw-r--r--   0        0        0     2247 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/threading.py
+-rw-r--r--   0        0        0      968 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/typing.py
+-rw-r--r--   0        0        0      984 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/utils.py
+-rw-r--r--   0        0        0     3967 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pool_cue/worker.py
+-rw-r--r--   0        0        0      666 2023-04-20 07:47:24.581156 pool_cue-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 pool_cue-1.1.0/PKG-INFO
```

### Comparing `pool_cue-1.0.1/LICENSE` & `pool_cue-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pool_cue-1.0.1/README.md` & `pool_cue-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 And push jobs to the queue:
 
 ```python
 from pool_cue import Queue
 from example.main import settings
 
 async with Queue(settings=settings) as queue:
-    await queue.push_job(func='test_task', extra_keyword_argument="foo")
+    await queue.push_job(_func='test_task', extra_keyword_argument="foo")
 ```
 
 Example worker output:
 
 ```
 12:28:57: Starting worker for 2 functions: test_child_task, test_task
 12:28:57: redis_version=7.0.10 mem_usage=1.46M clients_connected=2 db_keys=0
```

### Comparing `pool_cue-1.0.1/pool_cue/config.py` & `pool_cue-1.1.0/pool_cue/config.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.0.1/pool_cue/context.py` & `pool_cue-1.1.0/pool_cue/context.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.0.1/pool_cue/jobs.py` & `pool_cue-1.1.0/pool_cue/jobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     :param _redis: Redis queue connection.
     :param _func: Job function name.
     :param _job_id: Optional job ID used by arq to enforce job uniqueness.
         By default, the job will be given an ID based on its function name, children, and keyword arguments.
     :param _children: Optional list of other job function names.
         Used to stop jobs that spawn child jobs from being queued as long as any of its children remain in the queue.
-    :param _delay: Optional duration (in seconds) to wait before adding the job to the queue.
+    :param _delay: Duration (in seconds) to wait before running the job.
         The duration will be chosen randomly from within the given range.
     :param _force: If True, the job will be added to the queue even if it or its children already exist in the queue.
         Combine with the '_job_id' argument to skip enforcing job uniqueness.
     :param _queue_name: Redis queue name.
         The default queue name from the Redis connection will be used if not specified.
     :param kwargs: Keyword arguments to pass to the job function.
     """
@@ -116,20 +116,19 @@
         _id = _job_id
     if not _force:
         if await _job_already_exists(
             _redis=_redis, _func=_func, _children=_children, _queue_name=_queue_name, **kwargs
         ):
             logger.warning("Job '%s' is already queued!", _id or _func)
             return
-    if _delay:
-        a, b = _delay
-        job_delay: int = randint(a=a, b=b)
-        logger.debug("Adding job '%s' to the queue in %s sec...", _id or _func, job_delay)
-        await asyncio.sleep(delay=job_delay)
-    else:
-        logger.debug("Adding job '%s' to the queue...", _id or _func)
+    _defer_by: int | None = randint(a=_delay[0], b=_delay[1]) if _delay else None
+    logger.debug("Adding job '%s' to the queue...", _id or _func)
     try:
         await _redis.enqueue_job(
-            function=_func, _job_id=_id, _queue_name=_queue_name or _redis.default_queue_name, **kwargs
+            function=_func,
+            _job_id=_id,
+            _queue_name=_queue_name or _redis.default_queue_name,
+            _defer_by=_defer_by,
+            **kwargs,
         )
     except Exception as exc:
         logger.error("Failed to add job '%s' to the queue!", _id or _func, exc_info=exc)
```

### Comparing `pool_cue-1.0.1/pool_cue/queue.py` & `pool_cue-1.1.0/pool_cue/queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         By default, a job will not be added to the queue if it (or any of its children) already exists in the queue.
         This behaviour cam be controlled using the '_children' and '_force' keyword arguments.
 
         :param _func: Job function name.
         :param _job_id: Optional job ID used by arq to enforce job uniqueness.
         :param _children: Optional list of other job function names.
             Used to stop new 'parent jobs' from being queued as long as any of its children remain in the queue.
-        :param _delay: Optional duration (in seconds) to wait before adding the job to the queue.
+        :param _delay: Duration (in seconds) to wait before running the job.
         :param _force: If True, the job will be added to the queue even if it
             or its children already exist in the queue.
         :param kwargs: Keyword arguments to pass to the job function.
         """
         await self._assert_redis_connection()
         return await push_job(
             _redis=self.redis,
```

### Comparing `pool_cue-1.0.1/pool_cue/threading.py` & `pool_cue-1.1.0/pool_cue/threading.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,48 +12,45 @@
 from .context import Context
 
 logger: logging.Logger = logging.getLogger(name="pool_cue")
 
 THREAD_POOL_EVENT_LOOPS: dict[int, asyncio.AbstractEventLoop] = {}
 
 
-def _run_coro_in_thread_pool(coro: Callable, *args, **kwargs) -> None:
+def _run_coro_in_thread_pool(_coro: Callable, *args, **kwargs) -> None:
     """
     Function used by 'run_in_thread_pool' to support running asynchronous functions in sub threads:
     Creates a new event loop in the current (sub) thread (if one doesn't already exist)
     to make it possible to call async functions.
 
     Based on:
     https://stackoverflow.com/questions/46074841/why-coroutines-cannot-be-used-with-run-in-executor/63106889#63106889
     """
     current_thread_id: int = threading.current_thread().ident
-    loop: asyncio.AbstractEventLoop
-    if current_thread_id in THREAD_POOL_EVENT_LOOPS:
-        loop = THREAD_POOL_EVENT_LOOPS[current_thread_id]
-    else:
+    if current_thread_id not in THREAD_POOL_EVENT_LOOPS:
         logger.debug("Creating new event loop in sub thread %s...", current_thread_id)
-        loop = asyncio.new_event_loop()
-        THREAD_POOL_EVENT_LOOPS[current_thread_id] = loop
-    future: Coroutine = coro(*args, **kwargs)
-    return loop.run_until_complete(future=future)
+        THREAD_POOL_EVENT_LOOPS[current_thread_id] = asyncio.new_event_loop()
+    loop: asyncio.AbstractEventLoop = THREAD_POOL_EVENT_LOOPS[current_thread_id]
+    future: Coroutine = _coro(*args, **kwargs)
+    loop.run_until_complete(future=future)
 
 
-async def run_in_thread_pool(ctx: Context, func: Callable, *args, **kwargs) -> None:
+async def run_in_thread_pool(_ctx: Context, _func: Callable, *args, **kwargs) -> None:
     """
     Run the given function in the queue worker's dedicated thread pool.
     Use this to run I/O bound tasks without blocking the worker's main thread.
 
     Supports both synchronous and asynchronous functions.
 
-    :param ctx: The worker context.
-    :param func: The function you want to run in a sub thread.
-    :param args: Extra positional arguments that will be passed to the task function.
-    :param kwargs: Extra keyword arguments that will be passed to the task function.
+    :param _ctx: The worker context.
+    :param _func: The function to run in a sub thread.
+    :param args: Positional arguments to pass to the function.
+    :param kwargs: Keyword arguments to pass to the function.
     """
     loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
-    thread_pool: ThreadPoolExecutor = ctx["pool"]
-    if asyncio.iscoroutinefunction(func=func):
+    pool: ThreadPoolExecutor = _ctx["pool"]
+    if asyncio.iscoroutinefunction(func=_func):
         await loop.run_in_executor(
-            executor=thread_pool, func=functools.partial(_run_coro_in_thread_pool, coro=func, *args, **kwargs)
+            executor=pool, func=functools.partial(_run_coro_in_thread_pool, _coro=_func, *args, **kwargs)
         )
     else:
-        await loop.run_in_executor(executor=thread_pool, func=functools.partial(func, *args, **kwargs))
+        await loop.run_in_executor(executor=pool, func=functools.partial(_func, *args, **kwargs))
```

### Comparing `pool_cue-1.0.1/pool_cue/typing.py` & `pool_cue-1.1.0/pool_cue/typing.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.0.1/pool_cue/utils.py` & `pool_cue-1.1.0/pool_cue/utils.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.0.1/pool_cue/worker.py` & `pool_cue-1.1.0/pool_cue/worker.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.0.1/pyproject.toml` & `pool_cue-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pool-cue"
-version = "1.0.1"
+version = "1.1.0"
 description = "Tools for working with arq job queues"
 authors = ["skarre-r <skarre-r@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/skarre-r/pool-cue"
 packages = [
     { include = "pool_cue" }
 ]
```

### Comparing `pool_cue-1.0.1/PKG-INFO` & `pool_cue-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pool-cue
-Version: 1.0.1
+Version: 1.1.0
 Summary: Tools for working with arq job queues
 Home-page: https://github.com/skarre-r/pool-cue
 Author: skarre-r
 Author-email: skarre-r@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -61,15 +61,15 @@
 And push jobs to the queue:
 
 ```python
 from pool_cue import Queue
 from example.main import settings
 
 async with Queue(settings=settings) as queue:
-    await queue.push_job(func='test_task', extra_keyword_argument="foo")
+    await queue.push_job(_func='test_task', extra_keyword_argument="foo")
 ```
 
 Example worker output:
 
 ```
 12:28:57: Starting worker for 2 functions: test_child_task, test_task
 12:28:57: redis_version=7.0.10 mem_usage=1.46M clients_connected=2 db_keys=0
```

