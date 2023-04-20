# Comparing `tmp/globus-compute-endpoint-2.0.1a3.tar.gz` & `tmp/globus-compute-endpoint-2.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.0.1a3.tar", last modified: Tue Apr 18 22:06:06 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.0.1a4.tar", last modified: Thu Apr 20 15:07:51 2023, max compression
```

## Comparing `globus-compute-endpoint-2.0.1a3.tar` & `globus-compute-endpoint-2.0.1a4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.902616 globus-compute-endpoint-2.0.1a3/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-18 19:39:56.000000 globus-compute-endpoint-2.0.1a3/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1840 2023-04-18 22:06:06.902681 globus-compute-endpoint-2.0.1a3/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-18 19:39:56.000000 globus-compute-endpoint-2.0.1a3/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.896664 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    18802 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.898723 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/config.py
--rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/default_config.py
--rw-r--r--   0 lei        (501) staff       (20)    26053 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 lei        (501) staff       (20)    25351 2023-04-18 19:39:56.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     2773 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.899349 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.899591 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6026 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/utils/config.py
--rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.899710 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.901128 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2104 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-r--r--   0 lei        (501) staff       (20)    34995 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 lei        (501) staff       (20)    48886 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 lei        (501) staff       (20)    35860 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-r--r--   0 lei        (501) staff       (20)     8401 2023-04-14 16:35:15.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-r--r--   0 lei        (501) staff       (20)    18606 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.901248 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/
--rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.901589 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    12874 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.902175 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/
--rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 lei        (501) staff       (20)     5106 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 lei        (501) staff       (20)      806 2023-04-18 22:04:21.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.897506 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1840 2023-04-18 22:06:06.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     2657 2023-04-18 22:06:06.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-18 22:06:06.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      359 2023-04-18 22:06:06.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-18 22:06:06.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       30 2023-04-18 22:06:06.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-18 22:06:06.902937 globus-compute-endpoint-2.0.1a3/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3634 2023-04-18 22:04:18.000000 globus-compute-endpoint-2.0.1a3/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.902505 globus-compute-endpoint-2.0.1a3/tests/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/tests/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2693 2023-04-13 00:34:31.000000 globus-compute-endpoint-2.0.1a3/tests/conftest.py
--rw-r--r--   0 lei        (501) staff       (20)     2276 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/tests/utils.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.234129 globus-compute-endpoint-2.0.1a4/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.0.1a4/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1840 2023-04-20 15:07:51.234213 globus-compute-endpoint-2.0.1a4/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.0.1a4/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.226309 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    19298 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.228979 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/config.py
+-rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/default_config.py
+-rw-r--r--   0 lei        (501) staff       (20)    26053 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 lei        (501) staff       (20)    24838 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     2773 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.229728 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.230025 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     6026 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/utils/config.py
+-rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.230172 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.232028 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2104 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/container_sched.py
+-rw-r--r--   0 lei        (501) staff       (20)    35357 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 lei        (501) staff       (20)    48886 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 lei        (501) staff       (20)    35860 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/messages.py
+-rw-r--r--   0 lei        (501) staff       (20)     8683 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/worker.py
+-rw-r--r--   0 lei        (501) staff       (20)    18606 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/worker_map.py
+-rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.232268 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/
+-rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.232649 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    12874 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.233367 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/
+-rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     5106 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 lei        (501) staff       (20)      806 2023-04-20 15:03:56.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.227092 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1840 2023-04-20 15:07:51.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     2657 2023-04-20 15:07:51.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-20 15:07:51.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      359 2023-04-20 15:07:51.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)      308 2023-04-20 15:07:51.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       30 2023-04-20 15:07:51.000000 globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-20 15:07:51.234479 globus-compute-endpoint-2.0.1a4/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3635 2023-04-20 15:03:52.000000 globus-compute-endpoint-2.0.1a4/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:51.233987 globus-compute-endpoint-2.0.1a4/tests/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/tests/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2693 2023-04-13 00:34:31.000000 globus-compute-endpoint-2.0.1a4/tests/conftest.py
+-rw-r--r--   0 lei        (501) staff       (20)     2276 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a4/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.0.1a3/LICENSE` & `globus-compute-endpoint-2.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/PKG-INFO` & `globus-compute-endpoint-2.0.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.1a3
+Version: 2.0.1a4
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.0.1a3/PyPI.md` & `globus-compute-endpoint-2.0.1a4/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from globus_compute_endpoint.endpoint.endpoint_manager import EndpointManager
 from globus_compute_endpoint.endpoint.utils.config import Config
 from globus_compute_endpoint.logging_config import setup_logging
 from globus_compute_endpoint.version import DEPRECATION_FUNCX_ENDPOINT
 from globus_compute_sdk.sdk.login_manager import LoginManager
 from globus_compute_sdk.sdk.login_manager.tokenstore import ensure_compute_dir
 from globus_compute_sdk.sdk.login_manager.whoami import print_whoami_info
+from packaging.version import Version
 
 log = logging.getLogger(__name__)
 
 
 class CommandState:
     def __init__(self):
         self.endpoint_config_dir: pathlib.Path = init_config_dir()
@@ -361,14 +362,27 @@
         raise ClickException(msg) from err
 
 
 def read_config(endpoint_dir: pathlib.Path) -> Config:
     endpoint_name = endpoint_dir.name
 
     try:
+        import funcx_endpoint
+
+        if Version(funcx_endpoint.__version__) < Version("2.0.0"):
+            msg = (
+                "To avoid compatibility issues with Globus Compute, please uninstall "
+                "funcx-endpoint or upgrade funcx-endpoint to >=2.0.0. Note that the "
+                "funcx-endpoint package is now deprecated."
+            )
+            raise ClickException(msg)
+    except ModuleNotFoundError:
+        pass
+
+    try:
         conf_path = endpoint_dir / "config.py"
         spec = importlib.util.spec_from_file_location("config", conf_path)
         if not (spec and spec.loader):
             raise Exception(f"Unable to import configuration (no spec): {conf_path}")
         config = importlib.util.module_from_spec(spec)
         if not config:
             raise Exception(f"Unable to import configuration (no config): {conf_path}")
@@ -424,15 +438,15 @@
             raise ClickException(msg) from err
         else:
             log.exception(err.msg)
             raise
 
     except Exception:
         log.exception(
-            "Globus Compute v0.2.0 made several non-backwards compatible changes to "
+            "Globus Compute v2.0.0 made several non-backwards compatible changes to "
             "the config. Your config might be out of date. "
             "Refer to "
             "https://funcx.readthedocs.io/en/latest/endpoints.html#configuring-funcx"
         )
         raise
```

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/config.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/default_config.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/interchange.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import platform
 import queue
 import random
 import signal
 import sys
 import threading
 import time
+import typing as t
 
 # multiprocessing.Event is a method, not a class
 # to annotate, we need the "real" class
 # see: https://github.com/python/typeshed/issues/4266
 from multiprocessing.synchronize import Event as EventType
 
 import globus_compute_endpoint.endpoint.utils.config
@@ -33,18 +34,20 @@
 )
 from globus_compute_endpoint.endpoint.rabbit_mq import (
     ResultQueuePublisher,
     TaskQueueSubscriber,
 )
 from globus_compute_endpoint.endpoint.result_store import ResultStore
 from globus_compute_endpoint.exception_handling import get_result_error_details
-from globus_compute_endpoint.executors.high_throughput.mac_safe_queue import mpQueue
 from globus_compute_sdk import __version__ as funcx_sdk_version
 from parsl.version import VERSION as PARSL_VERSION
 
+if t.TYPE_CHECKING:
+    from globus_compute_endpoint.executors import HighThroughputExecutor
+
 log = logging.getLogger(__name__)
 
 
 class EndpointInterchange:
     """Interchange is a task orchestrator for distributed systems.
 
     1. Asynchronously queue large volume of tasks (>100K)
@@ -126,49 +129,29 @@
             "os": platform.system(),
             "hname": platform.node(),
             "funcx_sdk_version": funcx_sdk_version,
             "funcx_endpoint_version": funcx_endpoint_version,
             "registration": self.endpoint_id,
             "dir": os.getcwd(),
         }
-
         log.info(f"Platform info: {self.current_platform}")
-        try:
-            self.load_config()
-        except Exception:
-            log.exception("Caught exception")
-            raise
 
+        self.results_passthrough: queue.Queue[
+            dict[str, bytes | str | None]
+        ] = queue.Queue()
+        self.executor: HighThroughputExecutor = self.config.executors[0]
         self._test_start = False
 
-    def load_config(self):
-        """Load the config"""
-        log.info("Loading endpoint local config")
-        self.results_passthrough = mpQueue()
-        self.executors: dict[
-            str, globus_compute_endpoint.executors.HighThroughputExecutor
-        ] = {}
-        for executor in self.config.executors:
-            log.info(f"Initializing executor: {executor.label}")
-            if not executor.endpoint_id:
-                executor.endpoint_id = self.endpoint_id
-            else:
-                if not executor.endpoint_id == self.endpoint_id:
-                    eep_id = f"Executor({executor.endpoint_id})"
-                    sep_id = f"Interchange({self.endpoint_id})"
-                    raise Exception(f"InconsistentEndpointId: {eep_id} != {sep_id}")
-            self.executors[executor.label] = executor
-            if executor.run_dir is None:
-                executor.run_dir = self.logdir
-
-    def start_executors(self):
-        log.info("Starting Executors")
-        for executor in self.config.executors:
-            if hasattr(executor, "passthrough") and executor.passthrough is True:
-                executor.start(results_passthrough=self.results_passthrough)
+    def start_executor(self):
+        log.info("Starting Executor")
+        self.executor.start(
+            results_passthrough=self.results_passthrough,
+            endpoint_id=self.endpoint_id,
+            run_dir=self.logdir,
+        )
 
     def migrate_tasks_to_internal(
         self,
         connection_params: dict,
         endpoint_uuid: str,
         pending_task_queue: multiprocessing.Queue,
         quiesce_event: EventType,
@@ -222,16 +205,15 @@
 
         # kill_event must be set before quiesce_event because we need to guarantee that
         # once the quiesce is complete, the interchange will not try to start again
         self._kill_event.set()
         self._quiesce_event.set()
 
     def cleanup(self):
-        for label in self.executors:
-            self.executors[label].shutdown()
+        self.executor.shutdown()
 
     def handle_sigterm(self, sig_num, curr_stack_frame):
         log.warning("Received SIGTERM, setting termination flag.")
         self.time_to_quit = True
 
     def start(self):
         """Start the Interchange"""
@@ -266,15 +248,15 @@
             ).start()
 
         log.info("Starting EndpointInterchange")
 
         # NOTE: currently we only start the executors once because
         # the current behavior is to keep them running decoupled while
         # the endpoint is waiting for reconnection
-        self.start_executors()
+        self.start_executor()
 
         while not self._kill_event.is_set():
             if self._reconnect_fail_counter >= self.reconnect_attempt_limit:
                 log.critical(
                     f"Failed {self._reconnect_fail_counter} consecutive times."
                     "  Shutting down."
                 )
@@ -346,15 +328,15 @@
         this method.
         """
         log.debug("_main_loop begins")
 
         results_publisher = ResultQueuePublisher(queue_info=self.result_q_info)
 
         with results_publisher:
-            executor = list(self.executors.values())[0]
+            executor = self.executor
 
             num_tasks_forwarded = 0
             num_results_forwarded = 0
 
             def process_stored_results():
                 # Handle any previously stored results, either from a previous run or
                 # from a quarter of a second-ago.  Basically, check every second
@@ -429,17 +411,14 @@
                 nonlocal num_results_forwarded
                 while not self._quiesce_event.is_set():
                     try:
                         result = self.results_passthrough.get(timeout=1)
                         task_id: str | None = result["task_id"]
                         packed_result: bytes = result["message"]
 
-                        if not task_id:
-                            raise AssertionError("task_id: empty or None")
-
                     except queue.Empty:
                         # Empty queue!  Let's see if we have any prior results to send
                         continue
 
                     except Exception as exc:
                         log.warning(
                             f"Invalid message received: no task_id.  Ignoring. {exc}"
@@ -449,14 +428,21 @@
                     try:
                         # This either works or it doesn't; if it doesn't, then
                         # serialize an exception and send _that_
                         # will be a packed EPStatusReport or Result
                         message = try_convert_to_messagepack(packed_result)
 
                     except Exception as exc:
+                        if not task_id:
+                            log.exception(
+                                "Unable to parse result message; no task id, so"
+                                " likely a garbled EPStatusReport; ignoring"
+                            )
+                            continue
+
                         log.exception(
                             f"Unable to parse result message for task {task_id}."
                             "   Marking task as failed."
                         )
 
                         err = f"[Task ID: {task_id}] ({exc.__class__.__name__}) {exc}"
 
@@ -599,13 +585,20 @@
             task_processor_thread.join(timeout=5)
             result_processor_thread.join(timeout=5)
 
             # let higher-level error handling take over if the following excepts
             message = EPStatusReport(
                 endpoint_id=self.endpoint_id,
                 # 0 == "no more heartbeats coming"
-                global_state={"heartbeat_period": 0},
+                global_state={
+                    "managers": 0,
+                    "total_workers": 0,
+                    "idle_workers": 0,
+                    "pending_tasks": 0,
+                    "outstanding_tasks": {},
+                    "heartbeat_period": 0,
+                },
                 task_statuses={},
             )
             results_publisher.publish(pack(message))
 
             log.debug("_main_loop exits")
```

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/utils/config.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/endpoint/utils/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 to be addressed.
 """
 from __future__ import annotations
 
 import concurrent.futures
 import ipaddress
 import logging
-import multiprocessing
 import os
 import queue
 import threading
 import time
+import uuid
 from multiprocessing import Process
 
 import daemon
 import dill
 from globus_compute_endpoint.executors.high_throughput import interchange, zmq_pipes
 from globus_compute_endpoint.executors.high_throughput.mac_safe_queue import mpQueue
 from globus_compute_endpoint.executors.high_throughput.messages import (
@@ -310,15 +310,15 @@
         self.passthrough = passthrough
         self.task_status_queue = task_status_queue
         self.tasks = {}
 
         self.outgoing_q: zmq_pipes.TasksOutgoing | None = None
         self.incoming_q: zmq_pipes.ResultsIncoming | None = None
         self.command_client: zmq_pipes.CommandClient | None = None
-        self.results_passthrough: multiprocessing.Queue | None = None
+        self.results_passthrough: queue.Queue | None = None
         self._queue_management_thread: threading.Thread | None = None
 
         self.is_alive = False
 
         # Set the available accelerators
         if available_accelerators is None:
             self.available_accelerators = ()
@@ -348,16 +348,28 @@
                 "--logdir={logdir} "
                 "--hb_period={heartbeat_period} "
                 "--hb_threshold={heartbeat_threshold} "
                 "--mode={worker_mode} "
                 "--container_image={container_image} "
             )
 
-    def start(self, results_passthrough: multiprocessing.Queue = None):
+    def start(
+        self,
+        *args,
+        endpoint_id: uuid.UUID | None = None,
+        run_dir: str | None = None,
+        results_passthrough: queue.Queue[dict[str, bytes | str | None]] | None = None,
+        **kwargs,
+    ):
         """Create the Interchange process and connect to it."""
+        assert run_dir, "GCExecutor requires kwarg:run_dir at start"
+        assert endpoint_id, "GCExecutor requires kwarg:endpoint_id at start"
+        self.run_dir = run_dir
+        self.endpoint_id = endpoint_id
+
         self.outgoing_q = zmq_pipes.TasksOutgoing(
             "127.0.0.1", self.interchange_port_range
         )
         self.incoming_q = zmq_pipes.ResultsIncoming(
             "127.0.0.1", self.interchange_port_range
         )
         self.command_client = zmq_pipes.CommandClient(
```

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     get_result_error_details,
 )
 from globus_compute_endpoint.exceptions import CouldNotExecuteUserTaskError
 from globus_compute_endpoint.executors.high_throughput.messages import Message
 from globus_compute_endpoint.logging_config import setup_logging
 from globus_compute_sdk.errors import MaxResultSizeExceeded
 from globus_compute_sdk.serialize import ComputeSerializer
+from parsl.app.python import timeout
 
 log = logging.getLogger(__name__)
 
 DEFAULT_RESULT_SIZE_LIMIT_MB = 10
 DEFAULT_RESULT_SIZE_LIMIT_B = DEFAULT_RESULT_SIZE_LIMIT_MB * 1024 * 1024
 
 
@@ -175,14 +176,18 @@
             messagepack.InvalidMessageError,
             messagepack.UnrecognizedProtocolVersion,
         ):
             task = Message.unpack(message)
             task_data = task.task_buffer.decode("utf-8")  # type: ignore[attr-defined]
 
         f, args, kwargs = self.serializer.unpack_and_deserialize(task_data)
+        GC_TASK_TIMEOUT = max(0.0, float(os.environ.get("GC_TASK_TIMEOUT", 0.0)))
+        if GC_TASK_TIMEOUT > 0.0:
+            log.debug(f"Setting task timeout to GC_TASK_TIMEOUT={GC_TASK_TIMEOUT}s")
+            f = timeout(f, GC_TASK_TIMEOUT)
         result_data = f(*args, **kwargs)
         serialized_data = self.serialize(result_data)
 
         if len(serialized_data) > self.result_size_limit:
             raise MaxResultSizeExceeded(len(serialized_data), self.result_size_limit)
 
         return serialized_data
```

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.1a3"
+__version__ = "2.0.1a4"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.1a3
+Version: 2.0.1a4
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.0.1a4/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/setup.py` & `globus-compute-endpoint-2.0.1a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk>=2.0.1a3",
+    "globus-compute-sdk>=2.0.1a4",
     "globus-compute-common==0.1.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
@@ -29,15 +29,15 @@
     # building from source, which may mean there's an issue in the packaged library
     # further investigation may be needed if the issue persists in the next pyzmq
     # release
     "pyzmq>=22.0.0,!=22.3.0,<=23.2.0",
     # 'parsl' is a core requirement of the globus-compute-endpoint, essential to a range
     # of different features and functions
     # pin exact versions because it does not use semver
-    "parsl==2023.1.23",
+    "parsl==2023.03.27",
     "pika>=1.2.0",
     "setproctitle>=1.3.2,<1.4",
 ]
 
 TEST_REQUIRES = [
     "responses",
     "pytest>=7.2",
```

### Comparing `globus-compute-endpoint-2.0.1a3/tests/conftest.py` & `globus-compute-endpoint-2.0.1a4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a3/tests/utils.py` & `globus-compute-endpoint-2.0.1a4/tests/utils.py`

 * *Files identical despite different names*

