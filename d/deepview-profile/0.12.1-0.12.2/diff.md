# Comparing `tmp/deepview-profile-0.12.1.tar.gz` & `tmp/deepview-profile-0.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepview-profile-0.12.1.tar", max compression
+gzip compressed data, was "deepview-profile-0.12.2.tar", max compression
```

## Comparing `deepview-profile-0.12.1.tar` & `deepview-profile-0.12.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    10173 2022-11-29 16:49:51.810194 deepview-profile-0.12.1/LICENSE
--rw-r--r--   0        0        0     5824 2023-04-20 15:13:52.998459 deepview-profile-0.12.1/README.md
--rw-r--r--   0        0        0      324 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/__init__.py
--rw-r--r--   0        0        0     1123 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/__main__.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/analysis/__init__.py
--rw-r--r--   0        0        0     7313 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/analysis/request_manager.py
--rw-r--r--   0        0        0     1664 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/analysis/runner.py
--rw-r--r--   0        0        0    23297 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/analysis/session.py
--rw-r--r--   0        0        0     1373 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/analysis/static.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/commands/__init__.py
--rw-r--r--   0        0        0     2002 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/commands/interactive.py
--rw-r--r--   0        0        0     3021 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/commands/measurements.py
--rw-r--r--   0        0        0     1729 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/commands/memory.py
--rw-r--r--   0        0        0     2749 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/commands/prediction_models.py
--rw-r--r--   0        0        0     1788 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/commands/time.py
--rw-r--r--   0        0        0      879 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/config/__init__.py
--rw-r--r--   0        0        0      150 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/data/__init__.py
--rw-r--r--   0        0        0      598 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/data/hints.yml
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/db/__init__.py
--rw-r--r--   0        0        0     2969 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/db/database.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/energy/__init__.py
--rw-r--r--   0        0        0     3727 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/energy/measurer.py
--rw-r--r--   0        0        0      722 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/error_printing.py
--rw-r--r--   0        0        0      683 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/evaluate.py
--rw-r--r--   0        0        0     3297 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/exceptions.py
--rw-r--r--   0        0        0     1914 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/initialization.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/io/__init__.py
--rw-r--r--   0        0        0     4440 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/io/connection.py
--rw-r--r--   0        0        0     2452 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/io/connection_acceptor.py
--rw-r--r--   0        0        0     2062 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/io/connection_manager.py
--rw-r--r--   0        0        0      765 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/io/sentinel.py
--rw-r--r--   0        0        0     2261 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/lru_cache.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/models/__init__.py
--rw-r--r--   0        0        0     3832 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/models/analysis.py
--rw-r--r--   0        0        0     1061 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/models/source_map.py
--rw-r--r--   0        0        0      455 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/nvml.py
--rw-r--r--   0        0        0     1245 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/profiler/__init__.py
--rw-r--r--   0        0        0     3054 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/profiler/autograd.py
--rw-r--r--   0        0        0     2943 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/profiler/backward.py
--rw-r--r--   0        0        0     8500 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/profiler/iteration.py
--rw-r--r--   0        0        0     5301 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/profiler/operation.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/protocol/__init__.py
--rw-r--r--   0        0        0     5862 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/protocol/message_handler.py
--rw-r--r--   0        0        0     3385 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/protocol/message_sender.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/protocol_gen/__init__.py
--rw-r--r--   0        0        0    64719 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/protocol_gen/innpv_pb2.py
--rw-r--r--   0        0        0     3441 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/server.py
--rw-r--r--   0        0        0     1067 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/skyline.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tests/__init__.py
--rw-r--r--   0        0        0     7188 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tests/test_lru_cache.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/__init__.py
--rw-r--r--   0        0        0      779 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/backward_interceptor.py
--rw-r--r--   0        0        0     1109 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/base.py
--rw-r--r--   0        0        0    10919 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/breakdown.py
--rw-r--r--   0        0        0     1439 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/call_stack.py
--rw-r--r--   0        0        0     4106 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/callable_tracker.py
--rw-r--r--   0        0        0     1630 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/hook_manager.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/memory/__init__.py
--rw-r--r--   0        0        0     8090 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/memory/activations.py
--rw-r--r--   0        0        0     4085 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/memory/report.py
--rw-r--r--   0        0        0     3437 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/memory/report_queries.py
--rw-r--r--   0        0        0     1903 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/memory/weights.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/time/__init__.py
--rw-r--r--   0        0        0     2634 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/time/operation.py
--rw-r--r--   0        0        0     2199 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/time/report.py
--rw-r--r--   0        0        0     1267 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/time/report_queries.py
--rw-r--r--   0        0        0     6258 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/tracker.py
--rw-r--r--   0        0        0      362 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/tracking/utils.py
--rw-r--r--   0        0        0     2680 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/user_code_utils.py
--rw-r--r--   0        0        0     1884 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/deepview_profile/version_utils.py
--rw-r--r--   0        0        0     1089 2023-04-20 14:57:42.364394 deepview-profile-0.12.1/pyproject.toml
--rw-r--r--   0        0        0     7363 2023-04-20 15:14:48.775375 deepview-profile-0.12.1/setup.py
--rw-r--r--   0        0        0     7053 2023-04-20 15:14:48.775905 deepview-profile-0.12.1/PKG-INFO
+-rw-r--r--   0        0        0    10173 2022-11-29 16:49:51.810194 deepview-profile-0.12.2/LICENSE
+-rw-r--r--   0        0        0     5824 2023-04-20 15:13:52.998459 deepview-profile-0.12.2/README.md
+-rw-r--r--   0        0        0      324 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/__init__.py
+-rw-r--r--   0        0        0     1123 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/analysis/__init__.py
+-rw-r--r--   0        0        0     7313 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/analysis/request_manager.py
+-rw-r--r--   0        0        0     1664 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/analysis/runner.py
+-rw-r--r--   0        0        0    23297 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/analysis/session.py
+-rw-r--r--   0        0        0     1373 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/analysis/static.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/commands/__init__.py
+-rw-r--r--   0        0        0     2002 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/commands/interactive.py
+-rw-r--r--   0        0        0     3021 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/commands/measurements.py
+-rw-r--r--   0        0        0     1729 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/commands/memory.py
+-rw-r--r--   0        0        0     2749 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/commands/prediction_models.py
+-rw-r--r--   0        0        0     1788 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/commands/time.py
+-rw-r--r--   0        0        0      879 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/config/__init__.py
+-rw-r--r--   0        0        0      150 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/data/__init__.py
+-rw-r--r--   0        0        0      598 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/data/hints.yml
+-rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/db/__init__.py
+-rw-r--r--   0        0        0     2968 2023-04-20 16:33:06.385513 deepview-profile-0.12.2/deepview_profile/db/database.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/energy/__init__.py
+-rw-r--r--   0        0        0     3727 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/energy/measurer.py
+-rw-r--r--   0        0        0      722 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/error_printing.py
+-rw-r--r--   0        0        0      683 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/evaluate.py
+-rw-r--r--   0        0        0     3297 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/exceptions.py
+-rw-r--r--   0        0        0     1914 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/initialization.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/io/__init__.py
+-rw-r--r--   0        0        0     4440 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/io/connection.py
+-rw-r--r--   0        0        0     2452 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/io/connection_acceptor.py
+-rw-r--r--   0        0        0     2062 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/io/connection_manager.py
+-rw-r--r--   0        0        0      765 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/io/sentinel.py
+-rw-r--r--   0        0        0     2261 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/lru_cache.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/models/__init__.py
+-rw-r--r--   0        0        0     3832 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/models/analysis.py
+-rw-r--r--   0        0        0     1061 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/models/source_map.py
+-rw-r--r--   0        0        0      455 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/nvml.py
+-rw-r--r--   0        0        0     1245 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/profiler/__init__.py
+-rw-r--r--   0        0        0     3054 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/profiler/autograd.py
+-rw-r--r--   0        0        0     2943 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/profiler/backward.py
+-rw-r--r--   0        0        0     8500 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/profiler/iteration.py
+-rw-r--r--   0        0        0     5301 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/profiler/operation.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/protocol/__init__.py
+-rw-r--r--   0        0        0     5862 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/protocol/message_handler.py
+-rw-r--r--   0        0        0     3385 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/protocol/message_sender.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/protocol_gen/__init__.py
+-rw-r--r--   0        0        0    64719 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/protocol_gen/innpv_pb2.py
+-rw-r--r--   0        0        0     3441 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/server.py
+-rw-r--r--   0        0        0     1067 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/skyline.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tests/__init__.py
+-rw-r--r--   0        0        0     7188 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tests/test_lru_cache.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/__init__.py
+-rw-r--r--   0        0        0      779 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/backward_interceptor.py
+-rw-r--r--   0        0        0     1109 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/base.py
+-rw-r--r--   0        0        0    10919 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/breakdown.py
+-rw-r--r--   0        0        0     1439 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/call_stack.py
+-rw-r--r--   0        0        0     4106 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/callable_tracker.py
+-rw-r--r--   0        0        0     1630 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/hook_manager.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/memory/__init__.py
+-rw-r--r--   0        0        0     8090 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/memory/activations.py
+-rw-r--r--   0        0        0     4085 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/memory/report.py
+-rw-r--r--   0        0        0     3437 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/memory/report_queries.py
+-rw-r--r--   0        0        0     1903 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/memory/weights.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/time/__init__.py
+-rw-r--r--   0        0        0     2634 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/time/operation.py
+-rw-r--r--   0        0        0     2199 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/time/report.py
+-rw-r--r--   0        0        0     1267 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/time/report_queries.py
+-rw-r--r--   0        0        0     6258 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/tracker.py
+-rw-r--r--   0        0        0      362 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/utils.py
+-rw-r--r--   0        0        0     2680 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/user_code_utils.py
+-rw-r--r--   0        0        0     1884 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/version_utils.py
+-rw-r--r--   0        0        0     1089 2023-04-20 16:38:46.232525 deepview-profile-0.12.2/pyproject.toml
+-rw-r--r--   0        0        0     7363 2023-04-20 16:39:55.941080 deepview-profile-0.12.2/setup.py
+-rw-r--r--   0        0        0     7053 2023-04-20 16:39:55.941570 deepview-profile-0.12.2/PKG-INFO
```

### Comparing `deepview-profile-0.12.1/LICENSE` & `deepview-profile-0.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/README.md` & `deepview-profile-0.12.2/README.md`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/__main__.py` & `deepview-profile-0.12.2/deepview_profile/__main__.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/analysis/request_manager.py` & `deepview-profile-0.12.2/deepview_profile/analysis/request_manager.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/analysis/runner.py` & `deepview-profile-0.12.2/deepview_profile/analysis/runner.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/analysis/session.py` & `deepview-profile-0.12.2/deepview_profile/analysis/session.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/analysis/static.py` & `deepview-profile-0.12.2/deepview_profile/analysis/static.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/commands/interactive.py` & `deepview-profile-0.12.2/deepview_profile/commands/interactive.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/commands/measurements.py` & `deepview-profile-0.12.2/deepview_profile/commands/measurements.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/commands/memory.py` & `deepview-profile-0.12.2/deepview_profile/commands/memory.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/commands/prediction_models.py` & `deepview-profile-0.12.2/deepview_profile/commands/prediction_models.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/commands/time.py` & `deepview-profile-0.12.2/deepview_profile/commands/time.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/config/__init__.py` & `deepview-profile-0.12.2/deepview_profile/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/data/hints.yml` & `deepview-profile-0.12.2/deepview_profile/data/hints.yml`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/db/database.py` & `deepview-profile-0.12.2/deepview_profile/db/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime 
 import os
 import sqlite3
 
-BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 DB_PATH = os.path.join(BASE_DIR, "deepview.sqlite3")
 
 class DatabaseInterface:
     def __init__(self, database_name=DB_PATH) -> None:
         self.connection = sqlite3.connect(database_name, detect_types=sqlite3.PARSE_DECLTYPES|sqlite3.PARSE_COLNAMES)
         self.create_energy_table()
```

### Comparing `deepview-profile-0.12.1/deepview_profile/energy/measurer.py` & `deepview-profile-0.12.2/deepview_profile/energy/measurer.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/error_printing.py` & `deepview-profile-0.12.2/deepview_profile/error_printing.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/evaluate.py` & `deepview-profile-0.12.2/deepview_profile/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/exceptions.py` & `deepview-profile-0.12.2/deepview_profile/exceptions.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/initialization.py` & `deepview-profile-0.12.2/deepview_profile/initialization.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/io/connection.py` & `deepview-profile-0.12.2/deepview_profile/io/connection.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/io/connection_acceptor.py` & `deepview-profile-0.12.2/deepview_profile/io/connection_acceptor.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/io/connection_manager.py` & `deepview-profile-0.12.2/deepview_profile/io/connection_manager.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/io/sentinel.py` & `deepview-profile-0.12.2/deepview_profile/io/sentinel.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/lru_cache.py` & `deepview-profile-0.12.2/deepview_profile/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/models/analysis.py` & `deepview-profile-0.12.2/deepview_profile/models/analysis.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/models/source_map.py` & `deepview-profile-0.12.2/deepview_profile/models/source_map.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/profiler/__init__.py` & `deepview-profile-0.12.2/deepview_profile/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/profiler/autograd.py` & `deepview-profile-0.12.2/deepview_profile/profiler/autograd.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/profiler/backward.py` & `deepview-profile-0.12.2/deepview_profile/profiler/backward.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/profiler/iteration.py` & `deepview-profile-0.12.2/deepview_profile/profiler/iteration.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/profiler/operation.py` & `deepview-profile-0.12.2/deepview_profile/profiler/operation.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/protocol/message_handler.py` & `deepview-profile-0.12.2/deepview_profile/protocol/message_handler.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/protocol/message_sender.py` & `deepview-profile-0.12.2/deepview_profile/protocol/message_sender.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/protocol_gen/innpv_pb2.py` & `deepview-profile-0.12.2/deepview_profile/protocol_gen/innpv_pb2.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/server.py` & `deepview-profile-0.12.2/deepview_profile/server.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/skyline.py` & `deepview-profile-0.12.2/deepview_profile/skyline.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tests/test_lru_cache.py` & `deepview-profile-0.12.2/deepview_profile/tests/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/backward_interceptor.py` & `deepview-profile-0.12.2/deepview_profile/tracking/backward_interceptor.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/base.py` & `deepview-profile-0.12.2/deepview_profile/tracking/base.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/breakdown.py` & `deepview-profile-0.12.2/deepview_profile/tracking/breakdown.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/call_stack.py` & `deepview-profile-0.12.2/deepview_profile/tracking/call_stack.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/callable_tracker.py` & `deepview-profile-0.12.2/deepview_profile/tracking/callable_tracker.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/hook_manager.py` & `deepview-profile-0.12.2/deepview_profile/tracking/hook_manager.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/memory/activations.py` & `deepview-profile-0.12.2/deepview_profile/tracking/memory/activations.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/memory/report.py` & `deepview-profile-0.12.2/deepview_profile/tracking/memory/report.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/memory/report_queries.py` & `deepview-profile-0.12.2/deepview_profile/tracking/memory/report_queries.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/memory/weights.py` & `deepview-profile-0.12.2/deepview_profile/tracking/memory/weights.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/time/operation.py` & `deepview-profile-0.12.2/deepview_profile/tracking/time/operation.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/time/report.py` & `deepview-profile-0.12.2/deepview_profile/tracking/time/report.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/time/report_queries.py` & `deepview-profile-0.12.2/deepview_profile/tracking/time/report_queries.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/tracking/tracker.py` & `deepview-profile-0.12.2/deepview_profile/tracking/tracker.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/user_code_utils.py` & `deepview-profile-0.12.2/deepview_profile/user_code_utils.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/deepview_profile/version_utils.py` & `deepview-profile-0.12.2/deepview_profile/version_utils.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.1/pyproject.toml` & `deepview-profile-0.12.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepview-profile"
-version = "0.12.1"
+version = "0.12.2"
 description = "Interactive performance profiling and debugging tool for PyTorch neural networks."
 authors = ["CentML <support@centml.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/CentML/DeepView.Profile"
 keywords = ["pytorch", "neural networks", "debugger", "profiler"]
 classifiers = [
```

### Comparing `deepview-profile-0.12.1/setup.py` & `deepview-profile-0.12.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'torch']
 
 entry_points = \
 {'console_scripts': ['deepview = deepview_profile.deepview_profile:main']}
 
 setup_kwargs = {
     'name': 'deepview-profile',
-    'version': '0.12.1',
+    'version': '0.12.2',
     'description': 'Interactive performance profiling and debugging tool for PyTorch neural networks.',
     'long_description': '![DeepView](https://raw.githubusercontent.com/CentML/DeepView.Profile/main/assets/deepview.png)\n[![License](https://img.shields.io/badge/license-Apache--2.0-green?style=flat)](https://github.com/CentML/DeepView.Profile/blob/main/LICENSE)\n![](https://img.shields.io/pypi/pyversions/deepview-profile.svg)\n[![](https://img.shields.io/pypi/v/deepview-profile.svg)](https://pypi.org/project/deepview-profile/)\n\nDeepView.Profile is a tool to profile and debug the training performance of [PyTorch](https://pytorch.org) neural networks.\n\n- [Installation](#installation)\n- [Usage example](#getting-started)\n- [Development Environment Setup](#dev-setup)\n- [Release Process](#release-process)\n- [Release History](#release-history)\n- [Meta](#meta)\n- [Contributing](#contributing)\n\n<h2 id="installation">Installation</h2>\n\nDeepView.Profile works with *GPU-based* neural networks that are implemented in [PyTorch](https://pytorch.org).\n\nTo run DeepView.Profile, you need:\n- A system equipped with an NVIDIA GPU\n- Python 3.7+\n- PyTorch 1.1.0+ with CUDA\n  - **NOTE:**  We assume you have the correct version of PyTorch installed for their GPU. Default PyTorch installation on Linux distros might not have CUDA support. If you see error similar to below, your PyTorch version is incompatible with your version of CUDA. You can download the appropriate version from the [PyTorch site](https://pytorch.org/get-started/locally/)\n    ```NVIDIA GeForce RTX 3060 Ti with CUDA capability sm_86 is not compatible with the current PyTorch installation.\n    The current PyTorch install supports CUDA capabilities sm_37 sm_50 sm_60 sm_70.\n    If you want to use the NVIDIA GeForce RTX 3060 Ti GPU with PyTorch, please check the instructions at https://pytorch.org/get-started/locally/\n    ```\n\n### Installation from PyPi\n\nInstalling with [Pip](https://packaging.python.org/en/latest/tutorials/installing-packages/#use-pip-for-installing)\n```zsh\npip install deepview-profile\n```\n\n### Installation from source\n```bash\ngit clone https://github.com/CentML/DeepView.Profile\ncd DeepView.Profile\npoetry install\npoetry run deepview --help\n```\n\n<h2 id="getting-started">Usage example</h2>\n\nTo use DeepView.Profile in your project, you need to first write an entry point file, which is a regular Python file that describes how your model is created and trained. See the [Entry Point](docs/providers.md) for more information.\n\nOnce your entry point file is ready, there are two ways to profile interactive profiling and standalone profiling.\n\n### Interactive Profiling\nInteractive profiling is done with VSCode with the [DeepView.Explore](https://github.com/CentML/DeepView.Explore) plugin. Install the plugin in VSCode and run the profiling session to interactively profile your models.\n```zsh\npython3 -m deepview_profile interactive\n```\n\n### Standalone Profiling\nStandalone profiling is useful when you just want access to DeepView.Profile\'s profiling functionality. DeepView.Profile will save the profiling results (called a "report") into a [SQLite database file](https://www.sqlite.org/) that you can then query yourself. We describe the database schema for DeepView.Profile\'s run time and memory reports in the [Run Time Report Format](docs/run-time-report.md) and [Memory Report Format](docs/memory-report.md) pages respectively.\n\nTo have DeepView.Profile perform run time profiling, you use the `deepview time`\nsubcommand. In addition to the entry point file, you also need to specify the\nfile where you want DeepView.Profile to save the run time profiling report using the\n`--output` or `-o` flag.\n\n```zsh\npython3 -m deepview_profile time entry_point.py --output my_output_file.sqlite\n```\n\nLaunching memory profiling is almost the same as launching run time profiling.\nYou just need to use `deepview memory` instead of `deepview time`.\n\n```zsh\npython3 -m deepview_profile memory entry_point.py --output my_output_file.sqlite\n```\n\n<h2 id="dev-setup">Development Environment Setup</h2>\n\nFrom the project root, do\n```zsh\npoetry install\n```\n<h2 id="release-process">Release Process</h2>\n\n1. Make sure you\'re on main branch and it is clean\n1. Run [tools/prepare-release.sh](tools/prepare-release.sh) which will:\n    * Increment the version\n    * Create a release branch\n    * Create a release PR\n1. After the PR is merged [build-and-publish-new-version.yml](.github/workflows/build-and-publish-new-version.yml) GitHub action will:\n    * build the Python Wheels\n    * GitHub release\n    * Publish to Test PyPI\n    * Subject to approval publish to PyPI\n\n<h2 id="release-history">Release History</h2>\n\nSee [Releases](https://github.com/CentML/DeepView.Profile/releases)\n\n<h2 id="meta">Meta</h2>\n\nDeepView.Profile began as a research project at the [University of Toronto](https://web.cs.toronto.edu) in collaboration with [Geofrey Yu](mailto:gxyu@cs.toronto.edu), [Tovi Grossman](https://www.tovigrossman.com) and [Gennady Pekhimenko](https://www.cs.toronto.edu/~pekhimenko/).\n\nThe accompanying research paper appears in the proceedings of UIST\'20. If you are interested, you can read a preprint of the paper [here](https://arxiv.org/pdf/2008.06798.pdf).\n\nIf you use DeepView.Profile in your research, please consider citing our paper:\n\n```bibtex\n@inproceedings{skyline-yu20,\n  title = {{Skyline: Interactive In-Editor Computational Performance Profiling\n    for Deep Neural Network Training}},\n  author = {Yu, Geoffrey X. and Grossman, Tovi and Pekhimenko, Gennady},\n  booktitle = {{Proceedings of the 33rd ACM Symposium on User Interface\n    Software and Technology (UIST\'20)}},\n  year = {2020},\n}\n```\n\nIt is distributed under Apache 2.0 license. See [LICENSE](LICENSE) and [NOTICE](NOTICE) for more information.\n\n<h2 id="contributing">Contributing</h2>\n\nCheck out [CONTRIBUTING.md](CONTRIBUTING.md) for more information on how to help with DeepView.Profile.\n',
     'author': 'CentML',
     'author_email': 'support@centml.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/CentML/DeepView.Profile',
```

### Comparing `deepview-profile-0.12.1/PKG-INFO` & `deepview-profile-0.12.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepview-profile
-Version: 0.12.1
+Version: 0.12.2
 Summary: Interactive performance profiling and debugging tool for PyTorch neural networks.
 Home-page: https://github.com/CentML/DeepView.Profile
 License: Apache-2.0
 Keywords: pytorch,neural networks,debugger,profiler
 Author: CentML
 Author-email: support@centml.ai
 Requires-Python: >=3.7,<4.0
```

