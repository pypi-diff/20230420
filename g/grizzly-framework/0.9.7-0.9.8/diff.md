# Comparing `tmp/grizzly-framework-0.9.7.tar.gz` & `tmp/grizzly-framework-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grizzly-framework-0.9.7.tar", last modified: Tue Oct 20 18:16:40 2020, max compression
+gzip compressed data, was "dist/grizzly-framework-0.9.8.tar", last modified: Wed Oct 21 20:32:12 2020, max compression
```

## Comparing `grizzly-framework-0.9.7.tar` & `grizzly-framework-0.9.8.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-20 18:16:40.160558 grizzly-framework-0.9.7/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3018 2020-10-20 18:16:40.160558 grizzly-framework-0.9.7/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1883 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-20 18:16:40.148557 grizzly-framework-0.9.7/grizzly/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      891 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/__main__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-20 18:16:40.148557 grizzly-framework-0.9.7/grizzly/adapters/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-20 18:16:40.148557 grizzly-framework-0.9.7/grizzly/adapters/NoOpAdapter/
--rw-rw-r--   0 travis    (2000) travis    (2000)      849 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/adapters/NoOpAdapter/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/adapters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9526 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/args.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-20 18:16:40.152557 grizzly-framework-0.9.7/grizzly/common/
--rw-rw-r--   0 travis    (2000) travis    (2000)      978 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4852 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/adapter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2901 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/harness.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4579 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/iomanager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26320 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/reporter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9133 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/runner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14496 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/stack_hasher.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8137 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17142 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/status_reporter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21043 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/storage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2571 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/test_adapter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4125 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/test_iomanager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27232 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/test_reporter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10397 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/test_runner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21634 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/test_stack_hasher.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7433 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/test_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20211 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/test_status_reporter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20547 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/test_storage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      840 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/common/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5865 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/main.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-20 18:16:40.156557 grizzly-framework-0.9.7/grizzly/reduce/
--rw-rw-r--   0 travis    (2000) travis    (2000)      894 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/reduce/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      367 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/reduce/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5985 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/reduce/args.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3884 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/reduce/bucket.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6266 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/reduce/crash.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      500 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/reduce/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47698 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/reduce/reduce.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16073 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/reduce/strategies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7877 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/reduce/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18901 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/reduce/test_interesting.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18049 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/reduce/test_main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32577 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/reduce/test_reduce.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-20 18:16:40.156557 grizzly-framework-0.9.7/grizzly/replay/
--rw-rw-r--   0 travis    (2000) travis    (2000)      321 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/replay/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      367 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/replay/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3573 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/replay/args.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19525 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/replay/replay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11524 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/replay/test_main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25900 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/replay/test_replay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8832 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/session.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-20 18:16:40.156557 grizzly-framework-0.9.7/grizzly/target/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1912 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/target/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10756 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/target/puppet_target.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4599 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/target/target.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/target/target_monitor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14413 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/target/test_puppet_target.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3920 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/target/test_target.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3071 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/target/test_target_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/target/test_target_monitor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2007 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/test_args.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4504 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/test_main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15505 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/grizzly/test_session.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-20 18:16:40.156557 grizzly-framework-0.9.7/grizzly_framework.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3018 2020-10-20 18:16:40.000000 grizzly-framework-0.9.7/grizzly_framework.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2215 2020-10-20 18:16:40.000000 grizzly-framework-0.9.7/grizzly_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-20 18:16:40.000000 grizzly-framework-0.9.7/grizzly_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      180 2020-10-20 18:16:40.000000 grizzly-framework-0.9.7/grizzly_framework.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      213 2020-10-20 18:16:40.000000 grizzly-framework-0.9.7/grizzly_framework.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-10-20 18:16:40.000000 grizzly-framework-0.9.7/grizzly_framework.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-20 18:16:40.160558 grizzly-framework-0.9.7/loki/
--rw-rw-r--   0 travis    (2000) travis    (2000)      352 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/loki/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      275 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/loki/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7245 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/loki/loki.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4566 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/loki/test_loki.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-20 18:16:40.160558 grizzly-framework-0.9.7/sapphire/
--rw-rw-r--   0 travis    (2000) travis    (2000)      537 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2055 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6910 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5634 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/connection_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6318 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8559 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/job.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4223 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/server_map.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4277 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/test_connection_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9693 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/test_job.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26964 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/test_sapphire.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4095 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/test_server_map.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4081 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/test_worker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9066 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/sapphire/worker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      108 2020-10-20 18:16:40.160558 grizzly-framework-0.9.7/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2577 2020-10-20 18:15:40.000000 grizzly-framework-0.9.7/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-21 20:32:12.442237 grizzly-framework-0.9.8/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3018 2020-10-21 20:32:12.442237 grizzly-framework-0.9.8/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1883 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-21 20:32:12.410235 grizzly-framework-0.9.8/grizzly/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      891 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/__main__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-21 20:32:12.410235 grizzly-framework-0.9.8/grizzly/adapters/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-21 20:32:12.410235 grizzly-framework-0.9.8/grizzly/adapters/NoOpAdapter/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      849 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/adapters/NoOpAdapter/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/adapters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9526 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/args.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-21 20:32:12.422236 grizzly-framework-0.9.8/grizzly/common/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      978 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4852 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/adapter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2901 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/harness.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4579 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/iomanager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26320 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/reporter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9133 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/runner.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14496 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/stack_hasher.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8137 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17142 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/status_reporter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21043 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/storage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2571 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/test_adapter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4125 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/test_iomanager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27232 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/test_reporter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10397 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/test_runner.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21634 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/test_stack_hasher.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7433 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/test_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20211 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/test_status_reporter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20547 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/test_storage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      840 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/common/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5865 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/main.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-21 20:32:12.426236 grizzly-framework-0.9.8/grizzly/reduce/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      894 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/reduce/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      367 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/reduce/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5985 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/reduce/args.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3884 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/reduce/bucket.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6266 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/reduce/crash.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      500 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/reduce/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47698 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/reduce/reduce.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16073 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/reduce/strategies.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7877 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/reduce/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18901 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/reduce/test_interesting.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18049 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/reduce/test_main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32577 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/reduce/test_reduce.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-21 20:32:12.430236 grizzly-framework-0.9.8/grizzly/replay/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      321 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/replay/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      367 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/replay/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3573 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/replay/args.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19525 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/replay/replay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11524 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/replay/test_main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25900 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/replay/test_replay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8832 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/session.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-21 20:32:12.430236 grizzly-framework-0.9.8/grizzly/target/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1912 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/target/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10756 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/target/puppet_target.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4599 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/target/target.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/target/target_monitor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14413 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/target/test_puppet_target.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3920 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/target/test_target.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3071 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/target/test_target_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/target/test_target_monitor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2007 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/test_args.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4504 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/test_main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15505 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/grizzly/test_session.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-21 20:32:12.434237 grizzly-framework-0.9.8/grizzly_framework.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3018 2020-10-21 20:32:12.000000 grizzly-framework-0.9.8/grizzly_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2215 2020-10-21 20:32:12.000000 grizzly-framework-0.9.8/grizzly_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-21 20:32:12.000000 grizzly-framework-0.9.8/grizzly_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      180 2020-10-21 20:32:12.000000 grizzly-framework-0.9.8/grizzly_framework.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      221 2020-10-21 20:32:12.000000 grizzly-framework-0.9.8/grizzly_framework.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-10-21 20:32:12.000000 grizzly-framework-0.9.8/grizzly_framework.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-21 20:32:12.438237 grizzly-framework-0.9.8/loki/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      352 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/loki/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      275 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/loki/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7245 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/loki/loki.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4566 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/loki/test_loki.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-21 20:32:12.442237 grizzly-framework-0.9.8/sapphire/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      537 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2055 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6910 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5634 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/connection_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6318 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8559 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/job.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4223 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/server_map.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4277 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/test_connection_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9693 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/test_job.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26964 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/test_sapphire.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4095 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/test_server_map.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4081 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/test_worker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9066 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/sapphire/worker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      108 2020-10-21 20:32:12.446238 grizzly-framework-0.9.8/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2581 2020-10-21 20:31:16.000000 grizzly-framework-0.9.8/setup.py
```

### Comparing `grizzly-framework-0.9.7/PKG-INFO` & `grizzly-framework-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-framework
-Version: 0.9.7
+Version: 0.9.8
 Summary: A framework for developing and running browser fuzzers
 Home-page: https://github.com/MozillaSecurity/grizzly
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
 Description: Grizzly
         =======
```

### Comparing `grizzly-framework-0.9.7/README.md` & `grizzly-framework-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/__main__.py` & `grizzly-framework-0.9.8/grizzly/__main__.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/adapters/NoOpAdapter/__init__.py` & `grizzly-framework-0.9.8/grizzly/adapters/NoOpAdapter/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/adapters/__init__.py` & `grizzly-framework-0.9.8/grizzly/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/args.py` & `grizzly-framework-0.9.8/grizzly/args.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/__init__.py` & `grizzly-framework-0.9.8/grizzly/common/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/adapter.py` & `grizzly-framework-0.9.8/grizzly/common/adapter.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/harness.html` & `grizzly-framework-0.9.8/grizzly/common/harness.html`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/iomanager.py` & `grizzly-framework-0.9.8/grizzly/common/iomanager.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/reporter.py` & `grizzly-framework-0.9.8/grizzly/common/reporter.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/runner.py` & `grizzly-framework-0.9.8/grizzly/common/runner.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/stack_hasher.py` & `grizzly-framework-0.9.8/grizzly/common/stack_hasher.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/status.py` & `grizzly-framework-0.9.8/grizzly/common/status.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/status_reporter.py` & `grizzly-framework-0.9.8/grizzly/common/status_reporter.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/storage.py` & `grizzly-framework-0.9.8/grizzly/common/storage.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/test_adapter.py` & `grizzly-framework-0.9.8/grizzly/common/test_adapter.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/test_iomanager.py` & `grizzly-framework-0.9.8/grizzly/common/test_iomanager.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/test_reporter.py` & `grizzly-framework-0.9.8/grizzly/common/test_reporter.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/test_runner.py` & `grizzly-framework-0.9.8/grizzly/common/test_runner.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/test_stack_hasher.py` & `grizzly-framework-0.9.8/grizzly/common/test_stack_hasher.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/test_status.py` & `grizzly-framework-0.9.8/grizzly/common/test_status.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/test_status_reporter.py` & `grizzly-framework-0.9.8/grizzly/common/test_status_reporter.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/test_storage.py` & `grizzly-framework-0.9.8/grizzly/common/test_storage.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/test_utils.py` & `grizzly-framework-0.9.8/grizzly/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/common/utils.py` & `grizzly-framework-0.9.8/grizzly/common/utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/main.py` & `grizzly-framework-0.9.8/grizzly/main.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/reduce/__init__.py` & `grizzly-framework-0.9.8/grizzly/reduce/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/reduce/args.py` & `grizzly-framework-0.9.8/grizzly/reduce/args.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/reduce/bucket.py` & `grizzly-framework-0.9.8/grizzly/reduce/bucket.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/reduce/crash.py` & `grizzly-framework-0.9.8/grizzly/reduce/crash.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/reduce/reduce.py` & `grizzly-framework-0.9.8/grizzly/reduce/reduce.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/reduce/strategies.py` & `grizzly-framework-0.9.8/grizzly/reduce/strategies.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/reduce/test_common.py` & `grizzly-framework-0.9.8/grizzly/reduce/test_common.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/reduce/test_interesting.py` & `grizzly-framework-0.9.8/grizzly/reduce/test_interesting.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/reduce/test_main.py` & `grizzly-framework-0.9.8/grizzly/reduce/test_main.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/reduce/test_reduce.py` & `grizzly-framework-0.9.8/grizzly/reduce/test_reduce.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/replay/args.py` & `grizzly-framework-0.9.8/grizzly/replay/args.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/replay/replay.py` & `grizzly-framework-0.9.8/grizzly/replay/replay.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/replay/test_main.py` & `grizzly-framework-0.9.8/grizzly/replay/test_main.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/replay/test_replay.py` & `grizzly-framework-0.9.8/grizzly/replay/test_replay.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/session.py` & `grizzly-framework-0.9.8/grizzly/session.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/target/__init__.py` & `grizzly-framework-0.9.8/grizzly/target/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/target/puppet_target.py` & `grizzly-framework-0.9.8/grizzly/target/puppet_target.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/target/target.py` & `grizzly-framework-0.9.8/grizzly/target/target.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/target/target_monitor.py` & `grizzly-framework-0.9.8/grizzly/target/target_monitor.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/target/test_puppet_target.py` & `grizzly-framework-0.9.8/grizzly/target/test_puppet_target.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/target/test_target.py` & `grizzly-framework-0.9.8/grizzly/target/test_target.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/target/test_target_loader.py` & `grizzly-framework-0.9.8/grizzly/target/test_target_loader.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/target/test_target_monitor.py` & `grizzly-framework-0.9.8/grizzly/target/test_target_monitor.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/test_args.py` & `grizzly-framework-0.9.8/grizzly/test_args.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/test_main.py` & `grizzly-framework-0.9.8/grizzly/test_main.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly/test_session.py` & `grizzly-framework-0.9.8/grizzly/test_session.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/grizzly_framework.egg-info/PKG-INFO` & `grizzly-framework-0.9.8/grizzly_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-framework
-Version: 0.9.7
+Version: 0.9.8
 Summary: A framework for developing and running browser fuzzers
 Home-page: https://github.com/MozillaSecurity/grizzly
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
 Description: Grizzly
         =======
```

### Comparing `grizzly-framework-0.9.7/grizzly_framework.egg-info/SOURCES.txt` & `grizzly-framework-0.9.8/grizzly_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/loki/loki.py` & `grizzly-framework-0.9.8/loki/loki.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/loki/test_loki.py` & `grizzly-framework-0.9.8/loki/test_loki.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/__init__.py` & `grizzly-framework-0.9.8/sapphire/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/__main__.py` & `grizzly-framework-0.9.8/sapphire/__main__.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/conftest.py` & `grizzly-framework-0.9.8/sapphire/conftest.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/connection_manager.py` & `grizzly-framework-0.9.8/sapphire/connection_manager.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/core.py` & `grizzly-framework-0.9.8/sapphire/core.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/job.py` & `grizzly-framework-0.9.8/sapphire/job.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/server_map.py` & `grizzly-framework-0.9.8/sapphire/server_map.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/test_connection_manager.py` & `grizzly-framework-0.9.8/sapphire/test_connection_manager.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/test_job.py` & `grizzly-framework-0.9.8/sapphire/test_job.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/test_sapphire.py` & `grizzly-framework-0.9.8/sapphire/test_sapphire.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/test_server_map.py` & `grizzly-framework-0.9.8/sapphire/test_server_map.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/test_worker.py` & `grizzly-framework-0.9.8/sapphire/test_worker.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/sapphire/worker.py` & `grizzly-framework-0.9.8/sapphire/worker.py`

 * *Files identical despite different names*

### Comparing `grizzly-framework-0.9.7/setup.py` & `grizzly-framework-0.9.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """Grizzly setup"""
 from os.path import dirname, join as pathjoin
 from itertools import chain
 from setuptools import setup
 
 
 EXTRAS = {
-    'reduce': ['cssbeautifier', 'lithium-reducer', 'jsbeautifier'],
+    'reduce': ['cssbeautifier', 'lithium-reducer<0.4', 'jsbeautifier'],
     's3': ['boto3'],
 }
 EXTRAS['all'] = list(set(chain.from_iterable(EXTRAS.values())))
 EXTRAS['test'] = ['pytest>=3.9', 'pytest-cov', 'pytest-mock']
 
 
 if __name__ == '__main__':
@@ -66,8 +66,8 @@
             'grizzly.replay',
             'grizzly.target',
             'loki',
             'sapphire',
         ],
         package_data={"grizzly.common": ["harness.html"]},
         url='https://github.com/MozillaSecurity/grizzly',
-        version='0.9.7')
+        version='0.9.8')
```

