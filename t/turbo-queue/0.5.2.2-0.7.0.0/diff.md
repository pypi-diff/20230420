# Comparing `tmp/turbo_queue-0.5.2.2.tar.gz` & `tmp/turbo_queue-0.7.0.0.tar.gz`

## Comparing `turbo_queue-0.5.2.2.tar` & `turbo_queue-0.7.0.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0  1145211 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/monitor_queue.gif
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/requirements.txt
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/src/turbo_queue/__init__.py
--rw-r--r--   0        0        0    20992 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/src/turbo_queue/_turbo_queue.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/LICENSE
--rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/README.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/pyproject.toml
--rw-r--r--   0        0        0     8866 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/PKG-INFO
+-rw-r--r--   0        0        0  1145211 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/monitor_queue.gif
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/requirements.txt
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/src/turbo_queue/__init__.py
+-rw-r--r--   0        0        0    15235 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/src/turbo_queue/_turbo_queue_kafka.py
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/src/turbo_queue/_turbo_queue_multi_task.py
+-rw-r--r--   0        0        0    21538 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/src/turbo_queue/turbo_queue.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/LICENSE
+-rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/README.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 turbo_queue-0.7.0.0/PKG-INFO
```

### Comparing `turbo_queue-0.5.2.2/monitor_queue.gif` & `turbo_queue-0.7.0.0/monitor_queue.gif`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.5.2.2/src/turbo_queue/_turbo_queue.py` & `turbo_queue-0.7.0.0/src/turbo_queue/turbo_queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,51 +11,50 @@
 from os import rename
 from pathlib import Path
 
 
 class _turbo_queue_base:
     def __init__(self):
         # self._age = 0
+        self.version = "0.7.0.0"
         self._queue_name = "example_queue_name"  # name of the queue
         self._root_path = "/dc_data"
         # self._queue_folder = ''
-        self._num_loaders = (
-            1  # number of processes that will be loading the files (inbound)
-        )
+        self._num_loaders = 1  # number of processes that will load the files (inbound)
         self._num_queues = 1  # number of queues/processes that will have the loaded files distributed amongst
         self._max_ready_files = (
-            1  # maximum number of ready files - loading will pause when reached
+            1  # maximum number of ready files - load will pause when reached
         )
         self._max_events_per_file = 80000  # maximum number of events per DB file that will be loaded, before a new DB file is created
         self._max_batch_age = 10  # approximate maximum number of seconds before a batch is flushed and a new one created
-        self._enqueue_active = False  # pause/ resume loading to file
-        self._dequeue_active = True  # pause/ resume loading to queues
+        self._enqueue_active = False  # pause/ resume load to file
+        self._dequeue_active = True  # pause/ resume load to queues
         self._processing_hold = (
             False  # additional hold while processing DB rename and recreate
         )
         self._remove_invalid = True  # remove files marked as invalid
 
         # auto-recover stale events in the queue folder
-        # existing loading will be renamed to ready, to be picked up by the dequeue process when it is started
-        # existing or stale chosen
+        # existing load will be renamed to ready, to be picked up by the dequeue process when it is started
+        # existing or stale unload
         self._recover_on_restart = (
             True  # on start, in-case of shutdown while processing
         )
         self._recover_on_stale = (
             True  # while running, check for stale events if processing stops
         )
         self._recover_on_stale_check_frequency = 300  # frequency to check in seconds
-        self._loading_stale_age = (
+        self._load_stale_age = (
             self._max_batch_age * 2
         )  # default is _max_batch_age * 2 (seconds)
-        self._chosen_stale_age = (
+        self._unload_stale_age = (
             100  # this should be adjusted based on average time it takes to rpocess
         )
 
-        self._max_chosen_age = 100
+        self._max_unload_age = 100
 
         self._drop_overflow = False  # default of FALSE - used for TESTING ONLY - will DROP overflow rather than just change fold status
         self._db_conn = None
         self._db_cursor = None
         self._db_name = None
         self._db_path = None
 
@@ -100,15 +99,15 @@
     def queue_folder(self, a):
         if type(a) != str:
             raise ValueError("Sorry, this must be a string")
         self._queue_folder = a
     """
 
     #
-    # num_loaders - number of processes that will be loading the files (inbound)
+    # num_loaders - number of processes that will load the files (inbound)
     @property
     def num_loaders(self):
         return self._num_loaders
 
     @num_loaders.setter
     def num_loaders(self, a):
         if type(a) != int or a < 1:
@@ -124,15 +123,15 @@
     @num_queues.setter
     def num_queues(self, a):
         if type(a) != int or a < 1:
             raise ValueError("Sorry, num_queues must be an integer > 0")
         self._num_queues = a
 
     #
-    # max_ready_files - maximum number of ready(able) files - loading will pause when reached
+    # max_ready_files - maximum number of ready(able) files - load will pause when reached
     @property
     def max_ready_files(self):
         return self._max_ready_files
 
     @max_ready_files.setter
     def max_ready_files(self, a):
         if type(a) != int or a < 1:
@@ -160,52 +159,52 @@
     @max_batch_age.setter
     def max_batch_age(self, a):
         if type(a) != int or a < 1:
             raise ValueError("Sorry, max_batch_age must be an integer > 0")
         self._max_batch_age = a
 
     #
-    # enqueue_active - pause/ resume loading to file
+    # enqueue_active - pause/ resume load to file
     @property
     def enqueue_active(self):
         return self._enqueue_active
 
     @enqueue_active.setter
     def enqueue_active(self, a):
         if type(a) != bool:
             raise ValueError("Sorry, enqueue_active must be True or False")
         self._enqueue_active = a
 
     #
-    # dequeue_active - pause/ resume loading to queues
+    # dequeue_active - pause/ resume load to queues
     @property
     def dequeue_active(self):
         return self._dequeue_active
 
     @dequeue_active.setter
     def dequeue_active(self, a):
         if type(a) != bool:
             raise ValueError("Sorry, dequeue_active must be True or False")
         self._dequeue_active = a
 
     #
-    # processing_hold - pause/ resume loading to queues
+    # processing_hold - pause/ resume load to queues
     @property
     def processing_hold(self):
         return self._processing_hold
 
     @processing_hold.setter
     def processing_hold(self, a):
         if type(a) != bool:
             raise ValueError("Sorry, processing_hold must be True or False")
         self._processing_hold = a
 
     #
 
-    # drop_overflow - pause/ resume loading to queues
+    # drop_overflow - pause/ resume load to queues
     @property
     def drop_overflow(self):
         return self._drop_overflow
 
     @drop_overflow.setter
     def drop_overflow(self, a):
         if type(a) != bool:
@@ -270,29 +269,35 @@
                     except:
                         file_error = True
                 if file_error:
                     if self._remove_invalid:
                         try:
                             os.remove(file)
                         except:
-                            #rename(
+                            # rename(
                             #    file,
                             #    f"{new_file_path}/invalid_file_{self.get_current_epoch_int()}_{self.get_uuid()}_recovered.db",
-                            #)
+                            # )
                             pass
                     else:
+                        try:
+                            rename(
+                                file,
+                                f"{new_file_path}/invalid_file_{self.get_current_epoch_int()}_{self.get_uuid()}_recovered.db",
+                            )
+                        except:
+                            pass
+                else:
+                    try:
                         rename(
                             file,
-                            f"{new_file_path}/invalid_file_{self.get_current_epoch_int()}_{self.get_uuid()}_recovered.db",
+                            f"{new_file_path}/{new_prefix}_{self.get_current_epoch_int()}_{self.get_uuid()}_recovered.db",
                         )
-                else:
-                    rename(
-                        file,
-                        f"{new_file_path}/{new_prefix}_{self.get_current_epoch_int()}_{self.get_uuid()}_recovered.db",
-                    )
+                    except:
+                        pass
         print(f"recover_stale complete: {match_prefix} {new_prefix}")
         return
 
     def get_ready_length(self):
         """
         get count of *.ready files
         """
@@ -351,43 +356,47 @@
         super().__init__()
 
     def on_start_cleanup(self):
         """
         call once prior to starting queues
         recovers any stale batches that were left uprocessed, by moving them to ready, to be picked up by the queue on restart.
         """
+        self._recover_stale("load_*", "ready")
+        self._recover_stale("unload_*", "ready")
+        #
+        # for upgrade < 0.6.0.0:
         self._recover_stale("loading_*", "ready")
         self._recover_stale("chosen_*", "ready")
         #
-        # for upgrade:
+        # for upgrade < 0.2.0.0:
         self._recover_stale("avail_*", "ready")
         self._recover_stale("assigned_*", "ready")
         return
 
 
 class enqueue(_turbo_queue_base):
-    """class with methods for loading the queue"""
+    """class with methods for load the queue"""
 
     def __init__(self):
         self.desc = "turbo_queue class for queue high performance"
         super().__init__()
         self._create_epoch = 1  # default value to start
         self.loop = asyncio.new_event_loop()
         asyncio.set_event_loop(self.loop)
         # self.loop.create_task(self.check_batch_age())
         # self.loop.run_forever()
 
     #
-    def _new_loading_db(self):
+    def _new_load_db(self):
         path = f"{self.root_path}/{self.queue_name}"
         # Check whether the specified path exists or not
         self.check_path_and_create(path)
         self._create_epoch = self.get_current_epoch_int()
         self._db_name = f"{self._create_epoch}_{self.get_uuid()}.db"
-        self.db_state = "loading"
+        self.db_state = "load"
         self._db_path = (
             f"{self.root_path}/{self.queue_name}/{self.db_state}_{self._db_name}"
         )
         # improve:
         # try:
         # creating database for first time{self._db_path}
         self._db_conn = sqlite3.connect(self._db_path)
@@ -401,42 +410,42 @@
         # test transaction:
         self._db_cursor.execute("BEGIN TRANSACTION")
 
         self.row_count = 0
         return
 
     #
-    def insert_loading_db(self, log_data):
+    def insert_load_db(self, log_data):
         """
         insert data into DB
         """
         self._db_cursor.execute(
             """INSERT INTO logs (log_data) VALUES (?)""", (json.dumps(log_data),)
         )
         return
 
     #
     def start(self):
         """
-        create an initial DB to begin loading data into
+        create an initial DB to begin load data into
         """
-        self._new_loading_db()
+        self._new_load_db()
         return
 
     #
     def add(self, dict_to_add):
         """
         add data to queue
         """
         if self.enqueue_active == False and self._drop_overflow == True:
             # dont insert, we are dropping overflow
             # WIP
             pass
         else:
-            self.insert_loading_db(dict_to_add)
+            self.insert_load_db(dict_to_add)
             self.row_count += 1
             if self.row_count >= self.max_events_per_file:
                 self._roll_next_batch()
         return
 
     def _roll_next_batch(self):
         # put on hold while processing, and force re-check on next loop
@@ -444,15 +453,15 @@
         self.enqueue_active = False
         #
         self.row_count = 0
         self._close_db()
         rename(
             self._db_path, f"{self.root_path}/{self.queue_name}/ready_{self._db_name}"
         )
-        self._new_loading_db()
+        self._new_load_db()
         self.update_enqueue_active_state()
         self.processing_hold = False
         return
 
     def check_time(self):
         """
         provides method to check the time the batch has been loading, and if exceeds timeout,
@@ -555,19 +564,27 @@
         --------
         >>> get_data = my_out_queue.get()
         >>> doc = next(get_data)
         >>> while doc:
                 <do something with doc>
         """
         if self._db_path == None:
-            result = self._get_chosen_from_ready()
+            result = self._get_unload_from_ready()
             if result == False:
                 yield None
             else:
                 self._total_batch += 1
+        # verify table:
+        listOfTables = self._db_conn.execute(
+            """SELECT name FROM sqlite_master WHERE type='table'
+            AND name='logs'; """
+        ).fetchall()
+
+        if listOfTables == []:
+            yield None
         for row in self._db_conn.execute("SELECT log_data FROM logs"):
             # WIP
             # self.totalMessages += 1
             # pollCount += 1
             # rowcount += 1
             data = json.loads(row[0])
             self._total_gets += 1
@@ -597,19 +614,19 @@
             self._db_conn.execute("pragma synchronous=0;")
             self._db_cursor = self._db_conn.cursor()
             return True
         except:
             self.logger.info(f"ERROR opening database for first time{self._db_path}")
             return False
 
-    def _get_chosen_from_ready(self):
+    def _get_unload_from_ready(self):
         """
-        get a path to a 'chosen' file to process, from one of the 'ready'able files
+        get a path to a 'unload' file to process, from one of the 'ready'able files
         will attempt max_attempts times to get a ready file set to self_db_path
-        will return True when successful or when already chosen
+        will return True when successful or when already unload
         will return False after 10 failed attempts, allowing the calling process to reset and try again
         """
         attempts = 0
         max_attempts = 10
         while attempts < max_attempts:
             attempts += 1
             path1 = f"{self.root_path}/{self.queue_name}"
@@ -618,17 +635,17 @@
             if next_file:
                 try:
                     # quickly grab the file
                     rename(next_file, f"{next_file}_temp_hold")
                     filename = os.path.basename(next_file)
                     filename_parts = filename.split("_", 1)
                     if self.proc_num:
-                        new_name = f"chosen_{filename_parts[1]}_{self.proc_num}"
+                        new_name = f"unload_{filename_parts[1]}_{self.proc_num}"
                     else:
-                        new_name = f"chosen_{filename_parts[1]}"
+                        new_name = f"unload_{filename_parts[1]}"
                     new_path = f"{self.root_path}/{self.queue_name}/{new_name}"
                     rename(f"{next_file}_temp_hold", new_path)
                     self._db_path = new_path
                     self._db_name = new_name
                     result_open = self._open_db()
                     if result_open == False:
                         self._db_path = None
```

### Comparing `turbo_queue-0.5.2.2/LICENSE` & `turbo_queue-0.7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.5.2.2/README.md` & `turbo_queue-0.7.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 ### Install
 ```
 pip install turbo-queue
 ```
 
 #### Updates:
+v0.7:
+- added kafka consumer, producer connectors
+- added multi_tasks helper class
+- modified file name pattern (load,ready,unload)
+
+v0.5:
 - added timer to clear out slow batches
 - cleanup class to clear out leftover events from restart
   - will ensure events still on disk are reloaded into the queue to be sent
 - standardized naming convention of the queue files
 - added troubleshooting steps
 
 #### Todo:
@@ -68,15 +74,15 @@
   enqueue.add(data)
   enqueue.update_enqueue_active_state()
   # update_enqueue_active_state needs to be run at some frequency
   # if the number of ready files exceeds the max, the state will will be set to False
   # this is the mechanism used to address downstream backup in the queue
 
 ### Dequeue data
-dequeue = fast_queue.dequeue(1)
+dequeue = turbo_queue.dequeue(1)
 dequeue.queue_name = queue_name
 dequeue.root_path = root_path
 get_data = dequeue.get()
 data = next(get_data)
 while data:
     data = next(get_data)
 # data = None when the queue is currently empty
```

### Comparing `turbo_queue-0.5.2.2/pyproject.toml` & `turbo_queue-0.7.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "turbo-queue"
-version = "0.5.2.2"
+version = "0.7.0.0"
 authors = [
   { name="Dave Waters", email="dave@1waters.com" },
 ]
 description = "A Python module to improve performance of multiprocessing queues"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `turbo_queue-0.5.2.2/PKG-INFO` & `turbo_queue-0.7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-queue
-Version: 0.5.2.2
+Version: 0.7.0.0
 Summary: A Python module to improve performance of multiprocessing queues
 Project-URL: Homepage, https://github.com/davewat/turbo-queue
 Project-URL: Bug Tracker, https://github.com/davewat/turbo-queue/issues
 Author-email: Dave Waters <dave@1waters.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,20 @@
 
 ### Install
 ```
 pip install turbo-queue
 ```
 
 #### Updates:
+v0.7:
+- added kafka consumer, producer connectors
+- added multi_tasks helper class
+- modified file name pattern (load,ready,unload)
+
+v0.5:
 - added timer to clear out slow batches
 - cleanup class to clear out leftover events from restart
   - will ensure events still on disk are reloaded into the queue to be sent
 - standardized naming convention of the queue files
 - added troubleshooting steps
 
 #### Todo:
@@ -82,15 +88,15 @@
   enqueue.add(data)
   enqueue.update_enqueue_active_state()
   # update_enqueue_active_state needs to be run at some frequency
   # if the number of ready files exceeds the max, the state will will be set to False
   # this is the mechanism used to address downstream backup in the queue
 
 ### Dequeue data
-dequeue = fast_queue.dequeue(1)
+dequeue = turbo_queue.dequeue(1)
 dequeue.queue_name = queue_name
 dequeue.root_path = root_path
 get_data = dequeue.get()
 data = next(get_data)
 while data:
     data = next(get_data)
 # data = None when the queue is currently empty
```

