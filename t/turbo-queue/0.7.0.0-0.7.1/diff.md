# Comparing `tmp/turbo_queue-0.7.0.0.tar.gz` & `tmp/turbo_queue-0.7.1.tar.gz`

## Comparing `turbo_queue-0.7.0.0.tar` & `turbo_queue-0.7.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0  1145211 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/monitor_queue.gif
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/requirements.txt
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/src/turbo_queue/__init__.py
--rw-r--r--   0        0        0    15235 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/src/turbo_queue/_turbo_queue_kafka.py
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/src/turbo_queue/_turbo_queue_multi_task.py
--rw-r--r--   0        0        0    21538 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/src/turbo_queue/turbo_queue.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/LICENSE
--rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/README.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/pyproject.toml
--rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/.DS_Store
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/requirements.txt
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/docs/how_it_works.md
+-rw-r--r--   0        0        0   412842 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/docs/monitor_queue.gif
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/src/turbo_queue/__init__.py
+-rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/src/turbo_queue/_turbo_queue_kafka.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/src/turbo_queue/_turbo_queue_multi_task.py
+-rw-r--r--   0        0        0    21382 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/src/turbo_queue/turbo_queue.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/README.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/PKG-INFO
```

### Comparing `turbo_queue-0.7.0.0/src/turbo_queue/_turbo_queue_kafka.py` & `turbo_queue-0.7.1/src/turbo_queue/_turbo_queue_kafka.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from confluent_kafka import Consumer, Producer
 
 from . import turbo_queue
 
 
 # class _turbo_queue_base:
-class _kafka_turbo_queue_base:
+class _KafkaTurboQueueBase:
     def __init__(self):
         # self._age = 0
         self._turbo_queue_queue_name = None
         self._turbo_queue_root_path = None
         self._kafka_brokers = None
         self._kafka_client_id = None
         self._queue_name = "example_queue_name"  # name of the queue
@@ -86,15 +86,15 @@
     @kafka_client_id.setter
     def kafka_client_id(self, a):
         if type(a) != str:
             raise ValueError("Sorry, this must be an string")
         self._kafka_client_id = a
 
 
-class KafkaEnqueue(_kafka_turbo_queue_base):
+class KafkaEnqueue(_KafkaTurboQueueBase):
     """
     Create a Kafka Consumer that enqueues all data into a Turbo Queue
 
         Parameters:
             turbo_queue_queue_name: the name of the Turbo Queue
             turbo_queue_root_path: path of the Turbo Queue
             turbo_queue_max_ready_files: maxiumum number of ready files to then pause the Consumer
@@ -232,15 +232,15 @@
                 continue
             doc = json.loads(msg.value())
             self.enqueue.add(doc)
         await asyncio.sleep(0.1)
         self.loop.create_task(self.loadEvents())
 
 
-class KafkaDequeue(_kafka_turbo_queue_base):
+class KafkaDequeue(_KafkaTurboQueueBase):
     """
     Class to dequeues events from Turbo Queue and produce to a Kafka topic
 
         Parameters:
             turbo_queue_queue_name: the name of the Turbo Queue
             turbo_queue_root_path: path of the Turbo Queue
             turbo_queue_max_ready_files: maxiumum number of ready files to then pause the Consumer
```

### Comparing `turbo_queue-0.7.0.0/src/turbo_queue/_turbo_queue_multi_task.py` & `turbo_queue-0.7.1/src/turbo_queue/_turbo_queue_multi_task.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-__all__ = ["multi_task", "task_group"]
-import logging
-
-logging.basicConfig(filename="./test_multi.log", level=logging.INFO)
-# logging.Formatter("%(asctime)s : %(levelname)s : %(message)s")
-logging.Formatter(
-    "%(asctime)s,%(msecs)d %(levelname)-8s [%(pathname)s:%(lineno)d in function %(funcName)s] %(message)s",
-    "%Y-%m-%d:%H:%M:%S",
-)
-logging.propagate = True
-
-import os
+__all__ = ["MultiTask", "TaskGroup"]
 import asyncio
 import atexit
-
+import logging
 import multiprocessing as mp
+import os
 
 logger = mp.log_to_stderr(logging.INFO)
 
-import time
 import signal
+import time
 from sys import exit
 
+logging.basicConfig(filename="./test_multi.log", level=logging.INFO)
+# logging.Formatter("%(asctime)s : %(levelname)s : %(message)s")
+logging.Formatter(
+    "%(asctime)s,%(msecs)d %(levelname)-8s [%(pathname)s:%(lineno)d in function %(funcName)s] %(message)s",
+    "%Y-%m-%d:%H:%M:%S",
+)
+logging.propagate = True
 
-class task_group:
-    """
-    build a task to run
-    will automatically add a 'process_id' as the last kwargs to pass to your task
-    """
 
+class TaskGroup:
     def __init__(self):
+        """
+        build a task to run
+        will automatically add a 'process_id' as the last kwargs to pass to your task
+        """
         self.function_to_call = None  # pass the actuall function to call
         self.kwargs = {}  # kwargs as dict {'arg1':123,'arg2':456}
         self.daemon = True  # run as daemon
         self.include_task_number = (
             True  # will pass the process counter as kwarg task_number
         )
         self.process_count = 1  # number of independent processes to start
         self.process_number_start = (
             11  # start labeling the task number, beginning with this value +1
         )
 
 
-class multi_task:
+class MultiTask:
     def __init__(self):
+        """Class to help in spinning up many processes for an application"""
         self.process_list = []
         self.loop = asyncio.new_event_loop()
         self.task_group_list = []
         logging.info("class loaded")
 
     def _goodbye(self, name, adjective, *args):
         logging.info(f"Shutting down processes")
```

### Comparing `turbo_queue-0.7.0.0/src/turbo_queue/turbo_queue.py` & `turbo_queue-0.7.1/src/turbo_queue/turbo_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-__all__ = ["dequeue", "enqueue", "startup"]
+__all__ = ["Dequeue", "Enqueue", "Startup"]
 
 import asyncio
 import json
 import logging
 import os
 import sqlite3
 import time
 import uuid
 from os import remove as file_remove
 from os import rename
 from pathlib import Path
 
 
-class _turbo_queue_base:
+class _TurboQueueBase:
     def __init__(self):
         # self._age = 0
         self.version = "0.7.0.0"
         self._queue_name = "example_queue_name"  # name of the queue
         self._root_path = "/dc_data"
         # self._queue_folder = ''
         self._num_loaders = 1  # number of processes that will load the files (inbound)
@@ -344,19 +344,17 @@
         try:
             next_file = str(sorted(Path(pp).glob("ready_*"))[0])
         except:
             next_file = None
         return next_file
 
 
-class startup(_turbo_queue_base):
-    """class with methods for startup operations"""
-
+class Startup(_TurboQueueBase):
     def __init__(self):
-        self.desc = "turbo_queue class for queue high performance"
+        """class with methods for startup operations"""
         super().__init__()
 
     def on_start_cleanup(self):
         """
         call once prior to starting queues
         recovers any stale batches that were left uprocessed, by moving them to ready, to be picked up by the queue on restart.
         """
@@ -369,19 +367,17 @@
         #
         # for upgrade < 0.2.0.0:
         self._recover_stale("avail_*", "ready")
         self._recover_stale("assigned_*", "ready")
         return
 
 
-class enqueue(_turbo_queue_base):
-    """class with methods for load the queue"""
-
+class Enqueue(_TurboQueueBase):
     def __init__(self):
-        self.desc = "turbo_queue class for queue high performance"
+        """class with methods for load the queue"""
         super().__init__()
         self._create_epoch = 1  # default value to start
         self.loop = asyncio.new_event_loop()
         asyncio.set_event_loop(self.loop)
         # self.loop.create_task(self.check_batch_age())
         # self.loop.run_forever()
 
@@ -475,43 +471,37 @@
         if (
             self._create_epoch + int(self._max_batch_age)
         ) < self.get_current_epoch_int():
             self._roll_next_batch()
         self.loop.create_task(self.check_batch_age())
 
 
-class dequeue(_turbo_queue_base):
-    """Class to remove data from a Turbo Queue
+class Dequeue(_TurboQueueBase):
+    def __init__(self, proc_num=None):
+        """Class to remove data from a Turbo Queue
 
-    Parameters
-    ----------
-    proc_num(required)
-        An integer to uniquely identify this process vs other processes that will dequeue from this queue.
-
-    Returns
-    -------
-    New dequeue object
-        A dequeue object.  Additional parameters can be set.  Primary function is get()
-
-    Examples
-    --------
-    >>> import turbo_queue
-    >>> my_out_queue = turbo_queue.dequeue(1)
-    >>> my_out_queue.root_path = '/path/to/queue'
-    >>> my_out_queue.queue_name = 'my_queue'
-    >>> get_data = my_out_queue.get()
-    >>> doc = next(get_data)
-    >>> while doc:
-            #<do something with doc>
-    """
+        Args:
+            proc_num (integer, optional): unique number to track individual processes. Defaults to None.
 
-    def __init__(self, proc_num=None):
-        self.desc = "turbo_queue class for high performance IPC"
+        Returns:
+            Dequeue: A Dequeue object.  Additional parameters can be set.  Primary function is get()
+
+        Example:
+            >>> import turbo_queue
+            >>> my_out_queue = turbo_queue.Dequeue(1)
+            >>> my_out_queue.root_path = '/path/to/queue'
+            >>> my_out_queue.queue_name = 'my_queue'
+            >>> get_data = my_out_queue.get()
+            >>> doc = next(get_data)
+            >>> while doc:
+                >>> #<do something with doc>
+
+        """
         super().__init__()
-        self.proc_num = None
+        self.proc_num = proc_num
         self._total_gets = 0
         self._total_batch = 0
         self._auto_cleanup = True
 
     #
     # auto_cleanup
     @property
@@ -534,15 +524,15 @@
 
     def clean_up(self):
         """
         clean-up process called to remove the current batch after all events have been processed
         this is automatically called by default.
         Setting auto_cleanup to False will allow you to call in manually (or raise errors and not process).
         You MUST call cleanup() after the last get()-yield if you wish to continue to the next ready batch,
-        otherwise, you are choosing to leave the batch
+        otherwise, you are choosing to leave the batch on disk, and it will be reprocessed
         """
         self._close_db()
         file_remove(self._db_path)
         self._db_name = None
         self._db_path = None
         return
```

### Comparing `turbo_queue-0.7.0.0/LICENSE` & `turbo_queue-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.0.0/pyproject.toml` & `turbo_queue-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "turbo-queue"
-version = "0.7.0.0"
+version = "0.7.1"
 authors = [
   { name="Dave Waters", email="dave@1waters.com" },
 ]
 description = "A Python module to improve performance of multiprocessing queues"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

