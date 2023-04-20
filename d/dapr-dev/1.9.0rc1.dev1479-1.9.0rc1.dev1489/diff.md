# Comparing `tmp/dapr-dev-1.9.0rc1.dev1479.tar.gz` & `tmp/dapr-dev-1.9.0rc1.dev1489.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-dev-1.9.0rc1.dev1479.tar", last modified: Wed Apr 19 23:15:22 2023, max compression
+gzip compressed data, was "dist/dapr-dev-1.9.0rc1.dev1489.tar", last modified: Thu Apr 20 19:54:18 2023, max compression
```

## Comparing `dapr-dev-1.9.0rc1.dev1479.tar` & `dapr-dev-1.9.0rc1.dev1489.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/actor_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/client/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/client/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_call_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_method_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_reminder_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_state_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_timer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_type_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/method_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/reentrancy_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/remindable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/state_change.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/state_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/aio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/aio/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/aio/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/aio/clients/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/aio/clients/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/aio/clients/grpc/_asynchelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    48802 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/aio/clients/grpc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    29839 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    47931 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/http/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/http/dapr_actor_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/clients/http/dapr_invocation_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/conf/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/common/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/common/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/common/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/common/v1/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/common/v1/common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18118 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/v1/appcallback_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/v1/appcallback_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    71113 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/v1/dapr_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    57502 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/v1/dapr_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/serializers/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr/version/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/dapr/version/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr_dev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/dapr_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-19 23:15:22.000000 dapr-dev-1.9.0rc1.dev1479/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-19 23:15:10.000000 dapr-dev-1.9.0rc1.dev1479/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/actor_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/client/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_call_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_method_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_reminder_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_state_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_timer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_type_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/method_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/reentrancy_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/remindable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/state_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/state_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/_asynchelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48922 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30396 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48045 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/dapr_actor_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/dapr_invocation_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/conf/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/v1/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/v1/common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18118 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/appcallback_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/appcallback_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71113 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/dapr_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57502 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/dapr_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/serializers/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr/version/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/dapr/version/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-20 19:54:17.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:54:17.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:54:17.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 19:54:17.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 19:54:17.000000 dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-20 19:54:18.000000 dapr-dev-1.9.0rc1.dev1489/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-20 19:54:01.000000 dapr-dev-1.9.0rc1.dev1489/setup.py
```

### Comparing `dapr-dev-1.9.0rc1.dev1479/LICENSE` & `dapr-dev-1.9.0rc1.dev1489/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/PKG-INFO` & `dapr-dev-1.9.0rc1.dev1489/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-dev
-Version: 1.9.0rc1.dev1479
+Version: 1.9.0rc1.dev1489
 Summary: The developmental release for Dapr Python SDK.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-dev-1.9.0rc1.dev1479/README.md` & `dapr-dev-1.9.0rc1.dev1489/README.md`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/actor_interface.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/actor_interface.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/client/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/client/proxy.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/client/proxy.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/id.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/id.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_call_type.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_call_type.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_method_context.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_method_context.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_reminder_data.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_reminder_data.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_state_provider.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_state_provider.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_timer_data.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_timer_data.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_type_information.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_type_information.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/_type_utils.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/_type_utils.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/actor.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/actor.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/config.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/config.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/context.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/context.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/manager.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/manager.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/method_dispatcher.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/method_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/reentrancy_context.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/reentrancy_context.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/remindable.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/remindable.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/runtime.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/state_change.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/state_change.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/actor/runtime/state_manager.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/actor/runtime/state_manager.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/aio/clients/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/aio/clients/grpc/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/aio/clients/grpc/_asynchelpers.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/_asynchelpers.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/aio/clients/grpc/client.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/aio/clients/grpc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import time
 import socket
 
 from urllib.parse import urlencode
 
 from warnings import warn
 
-from typing import Dict, Optional, Union, Sequence, List
+from typing import Callable, Dict, Optional, Text, Union, Sequence, List
 from typing_extensions import Self
 
 from google.protobuf.message import Message as GrpcMessage
 from google.protobuf.empty_pb2 import Empty as GrpcEmpty
 
 import grpc.aio  # type: ignore
 from grpc.aio import (  # type: ignore
@@ -958,61 +958,63 @@
             items=response.items,
             headers=await call.initial_metadata())
 
     async def subscribe_configuration(
             self,
             store_name: str,
             keys: List[str],
-            config_metadata: Optional[Dict[str, str]] = dict()) -> ConfigurationWatcher:
+            handler: Callable[[Text, ConfigurationResponse], None],
+            config_metadata: Optional[Dict[str, str]] = dict()) -> Text:
         """Gets changed value from a config store with a key
 
         The example gets value from a config store:
             from dapr.aio.clients import DaprClient
             async with DaprClient() as d:
                 resp = await d.subscribe_config(
                     store_name='state_store'
                     key='key_1',
+                    handler=handler,
                     config_metadata={"metakey": "metavalue"}
                 )
 
         Args:
             store_name (str): the state store name to get from
             keys (str array): the keys of the key-value pairs to be gotten
+            handler(func (key, ConfigurationResponse)): the callback function to be called
             config_metadata (Dict[str, str], optional): Dapr metadata for configuration
 
         Returns:
-            :class:`ConfigurationResponse` gRPC metadata returned from callee
-            and value obtained from the config store
+            id (str): subscription id, which can be used to unsubscribe later
         """
         warn('The Subscribe Configuration API is an Alpha version and is subject to change.',
              UserWarning, stacklevel=2)
 
         if not store_name or len(store_name) == 0 or len(store_name.strip()) == 0:
             raise ValueError("Config store name cannot be empty to get the configuration")
         configWatcher = ConfigurationWatcher()
-        configWatcher.watch_configuration(self._stub, store_name, keys, config_metadata)
-        return configWatcher
+        id = configWatcher.watch_configuration(self._stub, store_name, keys,
+                                               handler, config_metadata)
+        return id
 
     async def unsubscribe_configuration(
             self,
             store_name: str,
-            key: str) -> bool:
+            id: str) -> bool:
         """Unsubscribes from configuration changes.
 
             Args:
                 store_name (str): the state store name to unsubscribe from
-                key (str): the key of the key-value pair to unsubscribe from
+                id (str): the subscription id to unsubscribe
 
             Returns:
                 bool: True if unsubscribed successfully, False otherwise
         """
         warn('The Unsubscribe Configuration API is an Alpha version and is subject to change.',
              UserWarning, stacklevel=2)
-        req = api_v1.UnsubscribeConfigurationRequest(store_name=store_name, id=key)
-        self._stub.UnsubscribeConfigurationAlpha1(req)
+        req = api_v1.UnsubscribeConfigurationRequest(store_name=store_name, id=id)
         call = self._stub.UnsubscribeConfigurationAlpha1(req)
         response: UnsubscribeConfigurationResponse = await call
         return response.ok
 
     async def try_lock(
             self,
             store_name: str,
```

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/base.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/base.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/exceptions.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/_helpers.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_helpers.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/_request.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_request.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/_response.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 """
 
 from __future__ import annotations
 
 import contextlib
 import threading
 from enum import Enum
-from typing import Dict, Optional, Text, Union, Sequence, List, Mapping, TYPE_CHECKING, NamedTuple
+from typing import (
+    Callable, Dict, List, Optional, Text, Union,
+    Sequence, Mapping, TYPE_CHECKING, NamedTuple
+)
 
 from google.protobuf.any_pb2 import Any as GrpcAny
 from google.protobuf.message import Message as GrpcMessage
 
 from dapr.clients.base import DEFAULT_JSON_CONTENT_TYPE
 from dapr.clients.grpc._helpers import (
     MetadataDict,
@@ -675,36 +678,46 @@
     def items(self) -> Mapping[Text, ConfigurationItem]:
         """Gets the items."""
         return self._items
 
 
 class ConfigurationWatcher():
     def __init__(self):
-        self.items: Dict[str, ConfigurationItem] = {}
-
-    def get_items(self):
-        return self.items
+        self.event: threading.Event = threading.Event()
+        self.id: str = ""
 
     def watch_configuration(self, stub: api_service_v1.DaprStub, store_name: str,
-                            keys: List[str], config_metadata: Optional[Dict[str, str]] = dict()):
+                            keys: List[str], handler: Callable[[Text, ConfigurationResponse], None],
+                            config_metadata: Optional[Dict[str, str]] = dict()):
         req = api_v1.SubscribeConfigurationRequest(
             store_name=store_name, keys=keys, metadata=config_metadata)
-        thread = threading.Thread(target=self._read_subscribe_config, args=(stub, req))
+        thread = threading.Thread(target=self._read_subscribe_config, args=(stub, req, handler))
         thread.daemon = True
         thread.start()
         self.keys = keys
         self.store_name = store_name
+        check = self.event.wait(timeout=5)
+        if not check:
+            print(f"Unable to get configuration id for keys {self.keys}")
+            return None
+        return self.id
 
     def _read_subscribe_config(self, stub: api_service_v1.DaprStub,
-                               req: api_v1.SubscribeConfigurationRequest):
+                               req: api_v1.SubscribeConfigurationRequest,
+                               handler: Callable[[Text, ConfigurationResponse], None]):
         try:
             responses = stub.SubscribeConfigurationAlpha1(req)
+            isFirst = True
             for response in responses:
-                for key in response.items:
-                    self.items[key] = response.items[key]
+                if isFirst:
+                    self.id = response.id
+                    self.event.set()
+                    isFirst = False
+                if len(response.items) > 0:
+                    handler(response.id, ConfigurationResponse(response.items))
         except Exception:
             print(f"{self.store_name} configuration watcher for keys "
                   f"{self.keys} stopped.")
             pass
 
 
 class TopicEventResponseStatus(Enum):
```

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/_state.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/_state.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/grpc/client.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/grpc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import time
 import socket
 
 from urllib.parse import urlencode
 
 from warnings import warn
 
-from typing import Dict, Optional, Union, Sequence, List
+from typing import Callable, Dict, Optional, Text, Union, Sequence, List
 from typing_extensions import Self
 
 from google.protobuf.message import Message as GrpcMessage
 from google.protobuf.empty_pb2 import Empty as GrpcEmpty
 
 import grpc  # type: ignore
 from grpc import (  # type: ignore
@@ -938,65 +938,67 @@
         req = api_v1.GetConfigurationRequest(
             store_name=store_name, keys=keys, metadata=config_metadata)
         response, call = self._stub.GetConfigurationAlpha1.with_call(req)
         return ConfigurationResponse(
             items=response.items,
             headers=call.initial_metadata())
 
-    async def subscribe_configuration(
+    def subscribe_configuration(
             self,
             store_name: str,
             keys: List[str],
-            config_metadata: Optional[Dict[str, str]] = dict()) -> ConfigurationWatcher:
+            handler: Callable[[Text, ConfigurationResponse], None],
+            config_metadata: Optional[Dict[str, str]] = dict()) -> Text:
         """Gets changed value from a config store with a key
 
         The example gets value from a config store:
             from dapr.clients import DaprClient
             with DaprClient() as d:
                 resp = d.subscribe_config(
                     store_name='state_store'
                     key='key_1',
+                    handler=handler,
                     config_metadata={"metakey": "metavalue"}
                 )
 
         Args:
             store_name (str): the state store name to get from
             keys (str array): the keys of the key-value pairs to be gotten
+            handler(func (key, ConfigurationResponse)): the callback function to be called
             config_metadata (Dict[str, str], optional): Dapr metadata for configuration
 
         Returns:
-            :class:`ConfigurationResponse` gRPC metadata returned from callee
-            and value obtained from the config store
+            id (str): subscription id, which can be used to unsubscribe later
         """
         warn('The Subscribe Configuration API is an Alpha version and is subject to change.',
              UserWarning, stacklevel=2)
 
         if not store_name or len(store_name) == 0 or len(store_name.strip()) == 0:
             raise ValueError("Config store name cannot be empty to get the configuration")
         configWatcher = ConfigurationWatcher()
-        configWatcher.watch_configuration(self._stub, store_name, keys, config_metadata)
-        return configWatcher
+        id = configWatcher.watch_configuration(self._stub, store_name, keys,
+                                               handler, config_metadata)
+        return id
 
     def unsubscribe_configuration(
             self,
             store_name: str,
-            key: str) -> bool:
+            id: str) -> bool:
         """Unsubscribes from configuration changes.
 
             Args:
                 store_name (str): the state store name to unsubscribe from
-                key (str): the key of the key-value pair to unsubscribe from
+                id (str): the subscription id to unsubscribe
 
             Returns:
                 bool: True if unsubscribed successfully, False otherwise
         """
         warn('The Unsubscribe Configuration API is an Alpha version and is subject to change.',
              UserWarning, stacklevel=2)
-        req = api_v1.UnsubscribeConfigurationRequest(store_name=store_name, id=key)
-        self._stub.UnsubscribeConfigurationAlpha1(req)
+        req = api_v1.UnsubscribeConfigurationRequest(store_name=store_name, id=id)
         response: UnsubscribeConfigurationResponse = self._stub.UnsubscribeConfigurationAlpha1(req)
         return response.ok
 
     def try_lock(
             self,
             store_name: str,
             resource_id: str,
```

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/http/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/http/client.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/client.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/http/dapr_actor_http_client.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/dapr_actor_http_client.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/clients/http/dapr_invocation_http_client.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/clients/http/dapr_invocation_http_client.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/conf/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/conf/global_settings.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/proto/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/proto/common/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/proto/common/v1/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/proto/common/v1/common_pb2.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/proto/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/v1/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/v1/appcallback_pb2.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/appcallback_pb2.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/v1/appcallback_pb2_grpc.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/appcallback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/v1/dapr_pb2.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/dapr_pb2.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/proto/runtime/v1/dapr_pb2_grpc.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/proto/runtime/v1/dapr_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/serializers/__init__.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/serializers/base.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/serializers/base.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/serializers/json.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/serializers/json.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/serializers/util.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/serializers/util.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr/version/version.py` & `dapr-dev-1.9.0rc1.dev1489/dapr/version/version.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr_dev.egg-info/PKG-INFO` & `dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-dev
-Version: 1.9.0rc1.dev1479
+Version: 1.9.0rc1.dev1489
 Summary: The developmental release for Dapr Python SDK.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-dev-1.9.0rc1.dev1479/dapr_dev.egg-info/SOURCES.txt` & `dapr-dev-1.9.0rc1.dev1489/dapr_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/setup.cfg` & `dapr-dev-1.9.0rc1.dev1489/setup.cfg`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1479/setup.py` & `dapr-dev-1.9.0rc1.dev1489/setup.py`

 * *Files identical despite different names*

