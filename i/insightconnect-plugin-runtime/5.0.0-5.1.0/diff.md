# Comparing `tmp/insightconnect-plugin-runtime-5.0.0.tar.gz` & `tmp/insightconnect-plugin-runtime-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insightconnect-plugin-runtime-5.0.0.tar", last modified: Wed Apr 12 14:16:39 2023, max compression
+gzip compressed data, was "insightconnect-plugin-runtime-5.1.0.tar", last modified: Thu Apr 20 09:53:50 2023, max compression
```

## Comparing `insightconnect-plugin-runtime-5.0.0.tar` & `insightconnect-plugin-runtime-5.1.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.675042 insightconnect-plugin-runtime-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-04-12 14:16:39.675042 insightconnect-plugin-runtime-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-04-12 14:15:48.000000 insightconnect-plugin-runtime-5.0.0/insightconnect-plugin-swagger.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.663042 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/action.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.663042 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26671 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.663042 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/clients/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/clients/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/data/input_message_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/data/output_message_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13942 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.663042 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-04-12 14:16:39.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-12 14:16:39.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:16:39.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-12 14:16:39.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 14:16:39.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:16:39.675042 insightconnect-plugin-runtime-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/
--rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.671042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.671042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.671042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.671042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.671042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/test_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.675042 insightconnect-plugin-runtime-5.0.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_aws_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_custom_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_server_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.047964 insightconnect-plugin-runtime-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-04-20 09:53:50.047964 insightconnect-plugin-runtime-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-04-20 09:53:12.000000 insightconnect-plugin-runtime-5.1.0/insightconnect-plugin-swagger.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.035964 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.035964 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26671 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.035964 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/clients/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/clients/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.035964 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/data/input_message_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/data/output_message_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21108 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.035964 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-04-20 09:53:49.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-20 09:53:49.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:53:49.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-20 09:53:49.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 09:53:49.000000 insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 09:53:50.047964 insightconnect-plugin-runtime-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.035964 insightconnect-plugin-runtime-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.035964 insightconnect-plugin-runtime-5.1.0/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.035964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.039964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.039964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.039964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.039964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.039964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.039964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.039964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.039964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.039964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.043964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.043964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.043964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.043964 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/tests/test_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:53:50.047964 insightconnect-plugin-runtime-5.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_aws_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_custom_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_server_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-20 09:51:08.000000 insightconnect-plugin-runtime-5.1.0/tests/unit/test_variables.py
```

### Comparing `insightconnect-plugin-runtime-5.0.0/PKG-INFO` & `insightconnect-plugin-runtime-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-plugin-runtime
-Version: 5.0.0
+Version: 5.1.0
 Summary: InsightConnect Plugin Runtime
 Home-page: https://github.com/rapid7/komand-plugin-sdk-python
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -150,14 +150,15 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.1.0 - Add new helper functions
 * 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
 * 4.10.1 - Remove raising of exception if request id is not available in header
 * 4.10.0 - Add structlog for structured logging
 * 4.9.0 - Add current SDK version plugin is using to /info endpoint
 * 4.8.0 - Add `OAuth20ClientCredentialMixin` class to clients
 * 4.7.6 - Add `PaginationHelper` to the AWS Client | Refactored the `ActionHelper` | Add `region` handler for AWSAction 
 * 4.7.5 - Add AWS client for assuming role
```

### Comparing `insightconnect-plugin-runtime-5.0.0/README.md` & `insightconnect-plugin-runtime-5.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.1.0 - Add new helper functions
 * 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
 * 4.10.1 - Remove raising of exception if request id is not available in header
 * 4.10.0 - Add structlog for structured logging
 * 4.9.0 - Add current SDK version plugin is using to /info endpoint
 * 4.8.0 - Add `OAuth20ClientCredentialMixin` class to clients
 * 4.7.6 - Add `PaginationHelper` to the AWS Client | Refactored the `ActionHelper` | Add `region` handler for AWSAction 
 * 4.7.5 - Add AWS client for assuming role
```

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect-plugin-swagger.json` & `insightconnect-plugin-runtime-5.1.0/insightconnect-plugin-swagger.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -447,68 +447,68 @@
         "version": "1.0"
     },
     "swagger": "2.0",
     "definitions": {
         "PluginInfo": {
             "type": "object",
             "properties": {
-                "plugin_spec_version": {
-                    "type": "string"
-                },
-                "description": {
-                    "type": "string"
-                },
                 "version": {
                     "type": "string"
                 },
-                "vendor": {
+                "title": {
                     "type": "string"
                 },
-                "name": {
-                    "type": "string"
+                "tags": {
+                    "type": "array",
+                    "items": {
+                        "type": "string"
+                    }
                 },
-                "title": {
+                "sdk_version": {
                     "type": "string"
                 },
-                "number_of_workers": {
-                    "type": "integer",
-                    "format": "int32"
+                "vendor": {
+                    "type": "string"
                 },
                 "threads": {
                     "type": "integer",
                     "format": "int32"
                 },
-                "tags": {
-                    "type": "array",
-                    "items": {
-                        "type": "string"
-                    }
+                "support": {
+                    "type": "string"
+                },
+                "plugin_spec_version": {
+                    "type": "string"
+                },
+                "description": {
+                    "type": "string"
                 },
                 "enable_cache": {
                     "type": "boolean"
                 },
-                "support": {
+                "name": {
                     "type": "string"
                 },
-                "sdk_version": {
-                    "type": "string"
+                "number_of_workers": {
+                    "type": "integer",
+                    "format": "int32"
                 }
             }
         },
         "ActionTriggerOutputBody": {
             "type": "object",
             "properties": {
-                "status": {
-                    "type": "string"
+                "meta": {
+                    "type": "object"
                 },
                 "log": {
                     "type": "string"
                 },
-                "meta": {
-                    "type": "object"
+                "status": {
+                    "type": "string"
                 },
                 "output": {
                     "type": "object"
                 }
             },
             "required": [
                 "log",
@@ -516,233 +516,233 @@
                 "output",
                 "status"
             ]
         },
         "ActionTriggerOutput": {
             "type": "object",
             "properties": {
-                "body": {
-                    "$ref": "#/definitions/ActionTriggerOutputBody"
-                },
                 "version": {
                     "type": "string"
                 },
                 "type": {
                     "type": "string",
                     "enum": [
                         "action_event",
                         "trigger_event"
                     ]
+                },
+                "body": {
+                    "$ref": "#/definitions/ActionTriggerOutputBody"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "TaskOutputBody": {
             "type": "object",
             "properties": {
-                "status": {
-                    "type": "string"
+                "state": {
+                    "type": "object"
+                },
+                "meta": {
+                    "type": "object"
                 },
                 "output": {
                     "type": "object"
                 },
                 "log": {
                     "type": "string"
                 },
-                "meta": {
-                    "type": "object"
-                },
-                "state": {
-                    "type": "object"
+                "status": {
+                    "type": "string"
                 }
             },
             "required": [
                 "log",
                 "meta",
                 "output",
                 "state",
                 "status"
             ]
         },
         "TaskOutput": {
             "type": "object",
             "properties": {
-                "body": {
-                    "$ref": "#/definitions/TaskOutputBody"
-                },
                 "version": {
                     "type": "string"
                 },
                 "type": {
                     "type": "string",
                     "enum": [
                         "task_event"
                     ]
+                },
+                "body": {
+                    "$ref": "#/definitions/TaskOutputBody"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "ActionTriggerInputBody": {
             "type": "object",
             "properties": {
+                "connection": {
+                    "type": "object"
+                },
                 "input": {
                     "type": "object"
                 },
                 "action": {
                     "type": "string"
-                },
-                "connection": {
-                    "type": "object"
                 }
             },
             "required": [
                 "action",
                 "connection",
                 "input"
             ]
         },
         "ActionTriggerInput": {
             "type": "object",
             "properties": {
-                "body": {
-                    "$ref": "#/definitions/ActionTriggerInputBody"
-                },
                 "version": {
                     "type": "string"
                 },
                 "type": {
                     "type": "string",
                     "enum": [
                         "action_event",
                         "trigger_event"
                     ]
+                },
+                "body": {
+                    "$ref": "#/definitions/ActionTriggerInputBody"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "TaskInputBody": {
             "type": "object",
             "properties": {
-                "state": {
-                    "type": "object"
-                },
-                "input": {
-                    "type": "object"
-                },
                 "connection": {
                     "type": "object"
                 },
                 "task": {
                     "type": "string"
+                },
+                "state": {
+                    "type": "object"
+                },
+                "input": {
+                    "type": "object"
                 }
             },
             "required": [
                 "connection",
                 "input",
                 "state",
                 "task"
             ]
         },
         "TaskInput": {
             "type": "object",
             "properties": {
-                "body": {
-                    "$ref": "#/definitions/TaskInputBody"
-                },
                 "version": {
                     "type": "string"
                 },
                 "type": {
                     "type": "string",
                     "enum": [
                         "task_event"
                     ]
+                },
+                "body": {
+                    "$ref": "#/definitions/TaskInputBody"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "ActionTriggerDetails": {
             "type": "object",
             "properties": {
-                "output": {
-                    "type": "object"
-                },
                 "title": {
                     "type": "string"
                 },
+                "description": {
+                    "type": "string"
+                },
                 "input": {
                     "type": "object"
                 },
-                "description": {
-                    "type": "string"
+                "output": {
+                    "type": "object"
                 }
             }
         },
         "ConnectionDetails": {
             "type": "object",
             "properties": {
+                "type": {
+                    "type": "string"
+                },
                 "title": {
                     "type": "string"
                 },
+                "properties": {
+                    "type": "object"
+                },
                 "required": {
                     "type": "array",
                     "items": {
                         "type": "string"
                     }
-                },
-                "type": {
-                    "type": "string"
-                },
-                "properties": {
-                    "type": "object"
                 }
             }
         },
         "ConnectionTestOutput": {
             "type": "object",
             "properties": {
                 "message": {
                     "type": "object"
                 }
             }
         },
         "TaskDetails": {
             "type": "object",
             "properties": {
-                "output": {
-                    "type": "object"
+                "title": {
+                    "type": "string"
                 },
                 "schedule": {
                     "type": "object"
                 },
-                "description": {
-                    "type": "string"
-                },
-                "title": {
-                    "type": "string"
+                "state": {
+                    "type": "object"
                 },
                 "input": {
                     "type": "object"
                 },
-                "state": {
+                "output": {
                     "type": "object"
+                },
+                "description": {
+                    "type": "string"
                 }
             }
         }
     }
 }
```

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/__init__.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/api/endpoints.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/api/schemas.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/api/schemas.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/cli.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/cli.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/clients/aws_client.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/clients/aws_client.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/clients/oauth.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/clients/oauth.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/connection.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/connection.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/data/input_message_schema.json` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/data/input_message_schema.json`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/data/output_message_schema.json` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/data/output_message_schema.json`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/dispatcher.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/dispatcher.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/exceptions.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/exceptions.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/metrics.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/metrics.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/plugin.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/plugin.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/schema.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/server.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/server.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/step.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/step.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/trigger.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/util.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/util.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/variables.py` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime/variables.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/PKG-INFO` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-plugin-runtime
-Version: 5.0.0
+Version: 5.1.0
 Summary: InsightConnect Plugin Runtime
 Home-page: https://github.com/rapid7/komand-plugin-sdk-python
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -150,14 +150,15 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.1.0 - Add new helper functions
 * 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
 * 4.10.1 - Remove raising of exception if request id is not available in header
 * 4.10.0 - Add structlog for structured logging
 * 4.9.0 - Add current SDK version plugin is using to /info endpoint
 * 4.8.0 - Add `OAuth20ClientCredentialMixin` class to clients
 * 4.7.6 - Add `PaginationHelper` to the AWS Client | Refactored the `ActionHelper` | Add `region` handler for AWSAction 
 * 4.7.5 - Add AWS client for assuming role
```

### Comparing `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/SOURCES.txt` & `insightconnect-plugin-runtime-5.1.0/insightconnect_plugin_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/setup.py` & `insightconnect-plugin-runtime-5.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="insightconnect-plugin-runtime",
-    version="5.0.0",
+    version="5.1.0",
     description="InsightConnect Plugin Runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rapid7 Integrations Alliance",
     author_email="integrationalliance@rapid7.com",
     url="https://github.com/rapid7/komand-plugin-sdk-python",
     packages=find_packages(),
```

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/__init__.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/__init__.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/conftest.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/test_cli.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/test_hello_world.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/test_server.py` & `insightconnect-plugin-runtime-5.1.0/tests/plugin/hello_world/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/unit/test_action.py` & `insightconnect-plugin-runtime-5.1.0/tests/unit/test_action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/unit/test_aws_action.py` & `insightconnect-plugin-runtime-5.1.0/tests/unit/test_aws_action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/unit/test_custom_encoder.py` & `insightconnect-plugin-runtime-5.1.0/tests/unit/test_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/unit/test_endpoints.py` & `insightconnect-plugin-runtime-5.1.0/tests/unit/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/unit/test_exceptions.py` & `insightconnect-plugin-runtime-5.1.0/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/unit/test_helpers.py` & `insightconnect-plugin-runtime-5.1.0/tests/unit/test_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -79,14 +79,58 @@
     assert {"one": [1, {}, {"three": 3}], "four": 4} == helper.clean(sample)
 
 
 def test_clean_no_exceptions():
     helper.clean({"one": [1, None, "", {"two": None}, {"three": 3}], "four": 4})
 
 
+def test_return_non_empty_successful():
+    sample = {
+        "test": 1,
+        "test2": ["one", "", None],
+        "test3": {"test": 1, "test2": "", "test3": None},
+        "test4": "",
+    }
+    assert {
+        "test": 1,
+        "test2": ["one"],
+        "test3": {"test": 1},
+    } == helper.return_non_empty(sample)
+
+
+# convert camel to snake
+def test_convert_to_snake_case():
+    sample = "letMeBeConverted"
+    assert helper.convert_to_snake_case(sample) == "let_me_be_converted"
+
+
+def test_convert_dict_to_snake_case():
+    sample = [{"testMe": 1}, {"testMe2": 2, "testMe3": {"testMe4": 1}}]
+    assert helper.convert_dict_to_snake_case(sample) == [
+        {"test_me": 1},
+        {"test_me2": 2, "test_me3": {"test_me4": 1}},
+    ]
+
+
+# convert snake to camel
+
+
+def test_convert_to_camel_case():
+    sample = "let_me_be_converted"
+    assert helper.convert_to_camel_case(sample) == "letMeBeConverted"
+
+
+def test_convert_dict_to_camel_case():
+    sample = [{"test_me": 1}, {"test_me2": 2, "test_me3": {"test_me4": 1}}]
+    assert helper.convert_dict_to_camel_case(sample) == [
+        {"testMe": 1},
+        {"testMe2": 2, "testMe3": {"testMe4": 1}},
+    ]
+
+
 # get_hashes_string
 
 
 def test_get_hashes_string_equal_successful():
     test_string = "abcdefghijklmnopqrstuvwxyz"
 
     assert {
@@ -212,21 +256,21 @@
     set_diff = expected_keys.difference(set(result))
     has_keys = len(set_diff) == 0
     assert has_keys
 
 
 def test_exec_command_pipe_failure():
     result = helper.exec_command("ls -lrt|grep test")
-    has_error = result['stderr'] != ""
+    has_error = result["stderr"] != ""
     assert has_error
 
 
 def test_exec_command_append_failure():
     result = helper.exec_command("ls -lrt >> outfile.log")
-    has_error = result['stderr'] != ""
+    has_error = result["stderr"] != ""
     assert has_error
 
 
 # encode_string
 
 
 def test_encode_string():
```

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/unit/test_metrics.py` & `insightconnect-plugin-runtime-5.1.0/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/unit/test_oauth.py` & `insightconnect-plugin-runtime-5.1.0/tests/unit/test_oauth.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/unit/test_plugin.py` & `insightconnect-plugin-runtime-5.1.0/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/unit/test_schema.py` & `insightconnect-plugin-runtime-5.1.0/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/unit/test_server_spec.py` & `insightconnect-plugin-runtime-5.1.0/tests/unit/test_server_spec.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.0.0/tests/unit/test_trigger.py` & `insightconnect-plugin-runtime-5.1.0/tests/unit/test_trigger.py`

 * *Files identical despite different names*

