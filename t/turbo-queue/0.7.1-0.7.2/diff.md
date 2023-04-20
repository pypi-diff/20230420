# Comparing `tmp/turbo_queue-0.7.1.tar.gz` & `tmp/turbo_queue-0.7.2.tar.gz`

## Comparing `turbo_queue-0.7.1.tar` & `turbo_queue-0.7.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/.DS_Store
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/CHANGELOG.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/requirements.txt
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/docs/how_it_works.md
--rw-r--r--   0        0        0   412842 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/docs/monitor_queue.gif
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/src/turbo_queue/__init__.py
--rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/src/turbo_queue/_turbo_queue_kafka.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/src/turbo_queue/_turbo_queue_multi_task.py
--rw-r--r--   0        0        0    21382 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/src/turbo_queue/turbo_queue.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/LICENSE
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/README.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 turbo_queue-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/.DS_Store
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/CHANGELOG.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/requirements.txt
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/docs/how_it_works.md
+-rw-r--r--   0        0        0   412842 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/docs/monitor_queue.gif
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/src/turbo_queue/__init__.py
+-rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/src/turbo_queue/_turbo_queue_kafka.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/src/turbo_queue/_turbo_queue_multi_task.py
+-rw-r--r--   0        0        0    21382 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/src/turbo_queue/turbo_queue.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/LICENSE
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/README.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 turbo_queue-0.7.2/PKG-INFO
```

### Comparing `turbo_queue-0.7.1/.DS_Store` & `turbo_queue-0.7.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.1/CHANGELOG.md` & `turbo_queue-0.7.2/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 ## [Unreleased]
 - improve logging
 - improve documentation
 - examples
 - process specific connectors
 
+## [0.7.2] - 2023-04-20
+
+### Fixed
+- Update class names in Kafka connector
+
 ## [0.7.1] - 2023-04-20
 
 ### Added
 
 - Minor documentation updates
 
 ### Changed
```

### Comparing `turbo_queue-0.7.1/docs/how_it_works.md` & `turbo_queue-0.7.2/docs/how_it_works.md`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.1/docs/monitor_queue.gif` & `turbo_queue-0.7.2/docs/monitor_queue.gif`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.1/src/turbo_queue/_turbo_queue_kafka.py` & `turbo_queue-0.7.2/src/turbo_queue/_turbo_queue_kafka.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
             and self._turbo_queue_queue_name
             and self._turbo_queue_root_path
             and self._kafka_brokers
             and len(self._consumer_topic_list) > 0
         ):
             logging.info("kafka_consumer_to_connector start3")
             # self.enqueue = fast_queue.enqueue()
-            self.enqueue = turbo_queue.enqueue()
+            self.enqueue = turbo_queue.Enqueue()
             self.enqueue.setup_logging()
             self.enqueue.queue_name = self._turbo_queue_queue_name
             self.enqueue.root_path = self._turbo_queue_root_path
             self.enqueue.max_ready_files = self._turbo_queue_max_ready_files
             self.enqueue.max_events_per_file = self._turbo_queue_max_events_per_file
 
             # now start
@@ -295,15 +295,15 @@
         if type(a) != str:
             raise ValueError("Sorry, this must be an string")
         self._kafka_producer_topic = a
 
     def start(self):
         self.producer = Producer(self.settings())
         if self.use_turbo_queue:
-            self.connector_dequeue = turbo_queue.dequeue()
+            self.connector_dequeue = turbo_queue.Dequeue()
             self.connector_dequeue.root_path = self._turbo_queue_root_path
             self.connector_dequeue.queue_name = self._turbo_queue_queue_name
             self.loop.create_task(self.loadEvents())
             self.loop.run_forever()
 
     def settings(self):
         settings = {
```

### Comparing `turbo_queue-0.7.1/src/turbo_queue/_turbo_queue_multi_task.py` & `turbo_queue-0.7.2/src/turbo_queue/_turbo_queue_multi_task.py`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.1/src/turbo_queue/turbo_queue.py` & `turbo_queue-0.7.2/src/turbo_queue/turbo_queue.py`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.1/LICENSE` & `turbo_queue-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.1/README.md` & `turbo_queue-0.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,48 @@
-WIP  
-*Not ready for PRs yet*
+
 
 ### Install
 ```
 pip install turbo-queue
 ```
-
+#### Project Status
+WIP - Not ready for PRs yet
 
 # Turbo Queue
-High performance, multi-processing queue. Works across child processes, and even between indivdual Python applications!
-
+High performance, multi-processing queue. Works across child processes, and even between individual Python applications!
 
 # Contents
- - [Overview](#Overview) 
- - [Quickstart](#Quickstart) 
+ - [Overview](#overview)
+ - [Use Cases](#use-cases)
+ - [Solution](#solution)
+ - [Results](#results)
+ - [Quickstart](#quickstart)
+ - [How It Works](docs/how_it_works.md)
 
 ## Overview
-Turbo Queue is used in place of the Python Multiprocessing Queue, with simple add/get symantecs, allowing you to create multiple processes that share a queue.
+Turbo Queue is used in place of the Python Multiprocessing Queue with simple add/get semantics, allowing you to create multiple processes that share a queue.
 
 Turbo Queue was designed to improve performance in situations where the Python Multiprocessing Queues is typically used. We found that as the number of processes subscribed to a single Multiprocessing Queue increased, the performance improvement on each successive process decreased. This appeared to be due to contention, with the processes locking/unlocking the queue to load/get data.
 
 ## Use Cases
 - Stream data from Kafka, run CPU intensive operations on the data, and then stream back to Kafka, on the order of billions of events per day.
 - Stream data from Kafka, reformat, and send to Elasticsearch.
 - Stream data from Kafka, reformat, and send to a service API.
 - Pull data from an API at high volume, process, and send to another API.
 
-
 ## Solution
-Our solution was to develop the Turbo Queue class. It is a shared nothing "queue" that uses the file system to provide the basis for coordination between the process. We use an agreed upon set of rules (as defined in the class) to create and manage files to store and process the data. SQLite is used a high-performance file storage format. File names (and re-naming) are used as the control mechanisms. In our use case we work in batches of data, and that is utilized here as well. We allow tuning of the batch size (which equates to the rows in the SQLite file) for optimal performance. A side benefit of the shared nothing approach allows entirely seperate applications (not just sub-processes) to use the queue.
+Our solution was to develop the Turbo Queue class. It is a shared nothing "queue" that uses the file system to provide the basis for coordination between the process. We use an agreed upon set of rules (as defined in the class) to create and manage files to store and process the data. SQLite is used a high-performance file storage format. File names (and re-naming) are used as the control mechanisms. In our use case we work in batches of data, and that is utilized here as well. We allow tuning of the batch size (which equates to the rows in the SQLite file) for optimal performance. A side benefit of the shared nothing approach allows entirely separate applications (not just sub-processes) to use the queue.
 
 ## Results
-Before Turbo Queue, using the built-in Multiprocessing Queue resulted in deminishing returns with 3 or more processes. While performance increased with each process, the throughput was not well correlated to the number of processes. 
+Before Turbo Queue, using the built-in Multiprocessing Queue resulted in diminishing returns with 3 or more processes. While performance increased with each process, the throughput was not well correlated to the number of processes. 
   
-However, with Turbo Queue, we were able to max out our processors on a single system(40+) with a substantial throughput increase. We actually began to hit limitations with our network and Kafka stack. In one instance, we were able to reduce our requirements from 40 python applications (running 2 subprocesses each), to 2 python apps with 30 subprocesses.
+However, with Turbo Queue, we were able to max out our processors on a single system(40+) with a substantial throughput increase. We began to hit limitations with our network and Kafka stack. In one instance, we were able to reduce our requirements from 40 python applications (running 2 subprocesses each), to 2 python apps with 30 subprocesses.
 
 ## Will this help you?
-YMMV. This worked well for our use case: CPU intesive processes, moving large volumes of data to and from Kafka and other services, and CPU dense hardware.
-
-## Documentation
-wip
-
-[How It Works](docs/how_it_works.md)
+YMMV. This worked well for our use case: CPU intensive processes, moving large volumes of data to and from Kafka and other services, and CPU dense hardware.
 
 ## Quickstart
 A very basic example:  
 
 ```
 import turbo_queue
```

### Comparing `turbo_queue-0.7.1/pyproject.toml` & `turbo_queue-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "turbo-queue"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="Dave Waters", email="dave@1waters.com" },
 ]
 description = "A Python module to improve performance of multiprocessing queues"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `turbo_queue-0.7.1/PKG-INFO` & `turbo_queue-0.7.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,62 @@
 Metadata-Version: 2.1
 Name: turbo-queue
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Python module to improve performance of multiprocessing queues
 Project-URL: Homepage, https://github.com/davewat/turbo-queue
 Project-URL: Bug Tracker, https://github.com/davewat/turbo-queue/issues
 Author-email: Dave Waters <dave@1waters.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-WIP  
-*Not ready for PRs yet*
+
 
 ### Install
 ```
 pip install turbo-queue
 ```
-
+#### Project Status
+WIP - Not ready for PRs yet
 
 # Turbo Queue
-High performance, multi-processing queue. Works across child processes, and even between indivdual Python applications!
-
+High performance, multi-processing queue. Works across child processes, and even between individual Python applications!
 
 # Contents
- - [Overview](#Overview) 
- - [Quickstart](#Quickstart) 
+ - [Overview](#overview)
+ - [Use Cases](#use-cases)
+ - [Solution](#solution)
+ - [Results](#results)
+ - [Quickstart](#quickstart)
+ - [How It Works](docs/how_it_works.md)
 
 ## Overview
-Turbo Queue is used in place of the Python Multiprocessing Queue, with simple add/get symantecs, allowing you to create multiple processes that share a queue.
+Turbo Queue is used in place of the Python Multiprocessing Queue with simple add/get semantics, allowing you to create multiple processes that share a queue.
 
 Turbo Queue was designed to improve performance in situations where the Python Multiprocessing Queues is typically used. We found that as the number of processes subscribed to a single Multiprocessing Queue increased, the performance improvement on each successive process decreased. This appeared to be due to contention, with the processes locking/unlocking the queue to load/get data.
 
 ## Use Cases
 - Stream data from Kafka, run CPU intensive operations on the data, and then stream back to Kafka, on the order of billions of events per day.
 - Stream data from Kafka, reformat, and send to Elasticsearch.
 - Stream data from Kafka, reformat, and send to a service API.
 - Pull data from an API at high volume, process, and send to another API.
 
-
 ## Solution
-Our solution was to develop the Turbo Queue class. It is a shared nothing "queue" that uses the file system to provide the basis for coordination between the process. We use an agreed upon set of rules (as defined in the class) to create and manage files to store and process the data. SQLite is used a high-performance file storage format. File names (and re-naming) are used as the control mechanisms. In our use case we work in batches of data, and that is utilized here as well. We allow tuning of the batch size (which equates to the rows in the SQLite file) for optimal performance. A side benefit of the shared nothing approach allows entirely seperate applications (not just sub-processes) to use the queue.
+Our solution was to develop the Turbo Queue class. It is a shared nothing "queue" that uses the file system to provide the basis for coordination between the process. We use an agreed upon set of rules (as defined in the class) to create and manage files to store and process the data. SQLite is used a high-performance file storage format. File names (and re-naming) are used as the control mechanisms. In our use case we work in batches of data, and that is utilized here as well. We allow tuning of the batch size (which equates to the rows in the SQLite file) for optimal performance. A side benefit of the shared nothing approach allows entirely separate applications (not just sub-processes) to use the queue.
 
 ## Results
-Before Turbo Queue, using the built-in Multiprocessing Queue resulted in deminishing returns with 3 or more processes. While performance increased with each process, the throughput was not well correlated to the number of processes. 
+Before Turbo Queue, using the built-in Multiprocessing Queue resulted in diminishing returns with 3 or more processes. While performance increased with each process, the throughput was not well correlated to the number of processes. 
   
-However, with Turbo Queue, we were able to max out our processors on a single system(40+) with a substantial throughput increase. We actually began to hit limitations with our network and Kafka stack. In one instance, we were able to reduce our requirements from 40 python applications (running 2 subprocesses each), to 2 python apps with 30 subprocesses.
+However, with Turbo Queue, we were able to max out our processors on a single system(40+) with a substantial throughput increase. We began to hit limitations with our network and Kafka stack. In one instance, we were able to reduce our requirements from 40 python applications (running 2 subprocesses each), to 2 python apps with 30 subprocesses.
 
 ## Will this help you?
-YMMV. This worked well for our use case: CPU intesive processes, moving large volumes of data to and from Kafka and other services, and CPU dense hardware.
-
-## Documentation
-wip
-
-[How It Works](docs/how_it_works.md)
+YMMV. This worked well for our use case: CPU intensive processes, moving large volumes of data to and from Kafka and other services, and CPU dense hardware.
 
 ## Quickstart
 A very basic example:  
 
 ```
 import turbo_queue
```

