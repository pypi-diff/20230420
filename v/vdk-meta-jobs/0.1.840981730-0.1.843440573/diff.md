# Comparing `tmp/vdk-meta-jobs-0.1.840981730.tar.gz` & `tmp/vdk-meta-jobs-0.1.843440573.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-meta-jobs-0.1.840981730.tar", last modified: Tue Apr 18 14:42:56 2023, max compression
+gzip compressed data, was "vdk-meta-jobs-0.1.843440573.tar", last modified: Thu Apr 20 13:17:42 2023, max compression
```

## Comparing `vdk-meta-jobs-0.1.840981730.tar` & `vdk-meta-jobs-0.1.843440573.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.147864 vdk-meta-jobs-0.1.840981730/
--rw-r--r--   0 root         (0) root         (0)     8391 2023-04-18 14:42:56.147864 vdk-meta-jobs-0.1.840981730/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7818 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 14:42:56.147864 vdk-meta-jobs-0.1.840981730/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-04-18 14:42:46.000000 vdk-meta-jobs-0.1.840981730/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.143864 vdk-meta-jobs-0.1.840981730/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.143864 vdk-meta-jobs-0.1.840981730/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.143864 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.143864 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.143864 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/api/
--rw-rw-rw-   0 root         (0) root         (0)     1402 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/api/meta_job.py
--rw-rw-rw-   0 root         (0) root         (0)     9347 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/cached_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     7949 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/dag_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/dags_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2269 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     6713 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     6148 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta_dag.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta_job_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     9344 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/remote_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1743 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/remote_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     2579 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/time_based_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.143864 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8391 2023-04-18 14:42:56.000000 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      858 2023-04-18 14:42:56.000000 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 14:42:56.000000 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-18 14:42:56.000000 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-18 14:42:56.000000 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-18 14:42:56.000000 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.147864 vdk-meta-jobs-0.1.840981730/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/tests/test_meta_dag.py
--rw-rw-rw-   0 root         (0) root         (0)    15096 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/tests/test_meta_job.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/tests/test_time_based_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2303 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/tests/test_tracking_job_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.420170 vdk-meta-jobs-0.1.843440573/
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-04-20 13:17:42.420170 vdk-meta-jobs-0.1.843440573/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7936 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 13:17:42.420170 vdk-meta-jobs-0.1.843440573/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-04-20 13:17:30.000000 vdk-meta-jobs-0.1.843440573/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.416170 vdk-meta-jobs-0.1.843440573/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.416170 vdk-meta-jobs-0.1.843440573/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.416170 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.416170 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.416170 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1402 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/api/meta_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     9347 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/cached_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7949 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/dag_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/dags_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     6713 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6438 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta_job_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     9344 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/remote_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1743 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/remote_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/time_based_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.420170 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-04-20 13:17:42.000000 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      858 2023-04-20 13:17:42.000000 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 13:17:42.000000 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 13:17:42.000000 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-20 13:17:42.000000 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-20 13:17:42.000000 vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 13:17:42.420170 vdk-meta-jobs-0.1.843440573/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/tests/test_meta_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)    15096 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/tests/test_meta_job.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/tests/test_time_based_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2303 2023-04-20 13:17:27.000000 vdk-meta-jobs-0.1.843440573/tests/test_tracking_job_executor.py
```

### Comparing `vdk-meta-jobs-0.1.840981730/PKG-INFO` & `vdk-meta-jobs-0.1.843440573/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: vdk-meta-jobs
-Version: 0.1.840981730
+Version: 0.1.843440573
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Meta Jobs
 
+## This plugin has been deprecated. Please use vdk-dag instead. You may install it by running `pip install vdk-dag`.
+
 Express dependencies between data jobs.
 
 A plugin for Versatile Data Kit extends its Job API with an additional feature that allows users to trigger so-called Meta Jobs.
 
 A meta job is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
 In this way, there's nothing different from other data jobs except for its purpose. See [Data Job types](https://github.com/vmware/versatile-data-kit/wiki/User-Guide#data-job-types) for more info.
```

### Comparing `vdk-meta-jobs-0.1.840981730/README.md` & `vdk-meta-jobs-0.1.843440573/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Meta Jobs
 
+## This plugin has been deprecated. Please use vdk-dag instead. You may install it by running `pip install vdk-dag`.
+
 Express dependencies between data jobs.
 
 A plugin for Versatile Data Kit extends its Job API with an additional feature that allows users to trigger so-called Meta Jobs.
 
 A meta job is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
 In this way, there's nothing different from other data jobs except for its purpose. See [Data Job types](https://github.com/vmware/versatile-data-kit/wiki/User-Guide#data-job-types) for more info.
```

### Comparing `vdk-meta-jobs-0.1.840981730/setup.py` & `vdk-meta-jobs-0.1.843440573/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.840981730"
+__version__ = "0.1.843440573"
 
 setuptools.setup(
     name="vdk-meta-jobs",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Express dependecies between data jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/api/meta_job.py` & `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/api/meta_job.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/cached_data_job_executor.py` & `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/cached_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/dag_validator.py` & `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/dag_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/dags_plugin.py` & `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/dags_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta.py` & `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta_configuration.py` & `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta_dag.py` & `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta_dag.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,20 @@
     def __init__(self, team_name: str, meta_config: MetaPluginConfiguration):
         """
         This module deals with all the DAG-related operations such as build and execute.
 
         :param team_name: the name of the owning team
         :param meta_config: the DAG job configuration
         """
+        log.warning(
+            "-------------------------------------------"
+            "This plugin has been deprecated. Please use vdk-dag instead. "
+            "You may install it by running `pip install vdk-dag`."
+            "-------------------------------------------"
+        )
         self._team_name = team_name
         self._topological_sorter = TopologicalSorter()
         self._delayed_starting_jobs = TimeBasedQueue(
             min_ready_time_seconds=meta_config.meta_jobs_delayed_jobs_min_delay_seconds(),
             randomize_delay_seconds=meta_config.meta_jobs_delayed_jobs_randomized_added_delay_seconds(),
         )
         self._max_concurrent_running_jobs = (
```

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta_job_runner.py` & `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/meta_job_runner.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/remote_data_job.py` & `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/remote_data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/remote_data_job_executor.py` & `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/remote_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/time_based_queue.py` & `vdk-meta-jobs-0.1.843440573/src/vdk/plugin/meta_jobs/time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/PKG-INFO` & `vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: vdk-meta-jobs
-Version: 0.1.840981730
+Version: 0.1.843440573
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Meta Jobs
 
+## This plugin has been deprecated. Please use vdk-dag instead. You may install it by running `pip install vdk-dag`.
+
 Express dependencies between data jobs.
 
 A plugin for Versatile Data Kit extends its Job API with an additional feature that allows users to trigger so-called Meta Jobs.
 
 A meta job is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
 In this way, there's nothing different from other data jobs except for its purpose. See [Data Job types](https://github.com/vmware/versatile-data-kit/wiki/User-Guide#data-job-types) for more info.
```

### Comparing `vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/SOURCES.txt` & `vdk-meta-jobs-0.1.843440573/src/vdk_meta_jobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/tests/test_meta_dag.py` & `vdk-meta-jobs-0.1.843440573/tests/test_meta_dag.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/tests/test_meta_job.py` & `vdk-meta-jobs-0.1.843440573/tests/test_meta_job.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/tests/test_time_based_queue.py` & `vdk-meta-jobs-0.1.843440573/tests/test_time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.840981730/tests/test_tracking_job_executor.py` & `vdk-meta-jobs-0.1.843440573/tests/test_tracking_job_executor.py`

 * *Files identical despite different names*

