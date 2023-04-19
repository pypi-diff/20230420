# Comparing `tmp/kwil-0.0.2.tar.gz` & `tmp/kwil-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwil-0.0.2.tar", last modified: Wed Apr 12 20:54:09 2023, max compression
+gzip compressed data, was "kwil-0.0.3.tar", last modified: Wed Apr 19 22:10:21 2023, max compression
```

## Comparing `kwil-0.0.2.tar` & `kwil-0.0.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.191761 kwil-0.0.2/
--rw-r--r--   0 gavin      (501) staff       (20)     1020 2023-04-12 20:54:09.191630 kwil-0.0.2/PKG-INFO
--rw-r--r--   0 gavin      (501) staff       (20)      360 2023-04-12 18:40:46.000000 kwil-0.0.2/README.md
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.182269 kwil-0.0.2/kwil/
--rw-r--r--   0 gavin      (501) staff       (20)       87 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/__about__.py
--rw-r--r--   0 gavin      (501) staff       (20)      322 2023-04-12 20:39:28.000000 kwil-0.0.2/kwil/__init__.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.186215 kwil-0.0.2/kwil/_utils/
--rw-r--r--   0 gavin      (501) staff       (20)        0 2023-04-03 19:04:31.000000 kwil-0.0.2/kwil/_utils/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     1555 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/action.py
--rw-r--r--   0 gavin      (501) staff       (20)      346 2023-04-10 22:57:27.000000 kwil-0.0.2/kwil/_utils/dataset.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.186610 kwil-0.0.2/kwil/_utils/grpc/
--rw-r--r--   0 gavin      (501) staff       (20)       56 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/grpc/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     2935 2023-04-12 20:45:39.000000 kwil-0.0.2/kwil/_utils/grpc/client.py
--rw-r--r--   0 gavin      (501) staff       (20)     2183 2023-04-12 15:56:08.000000 kwil-0.0.2/kwil/_utils/method_formatters.py
--rw-r--r--   0 gavin      (501) staff       (20)      719 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/naming_converter.py
--rw-r--r--   0 gavin      (501) staff       (20)     2796 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/request.py
--rw-r--r--   0 gavin      (501) staff       (20)      504 2023-04-09 22:05:10.000000 kwil-0.0.2/kwil/_utils/rpcs.py
--rw-r--r--   0 gavin      (501) staff       (20)     1807 2023-04-12 20:01:31.000000 kwil-0.0.2/kwil/_utils/signature.py
--rw-r--r--   0 gavin      (501) staff       (20)      185 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/signing.py
--rw-r--r--   0 gavin      (501) staff       (20)     1210 2023-04-12 14:59:57.000000 kwil-0.0.2/kwil/_utils/transaction.py
--rw-r--r--   0 gavin      (501) staff       (20)      419 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/utils.py
--rw-r--r--   0 gavin      (501) staff       (20)     3566 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/validation.py
--rw-r--r--   0 gavin      (501) staff       (20)      404 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/exceptions.py
--rw-r--r--   0 gavin      (501) staff       (20)     1436 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/kwild.py
--rw-r--r--   0 gavin      (501) staff       (20)     4341 2023-04-12 16:17:47.000000 kwil-0.0.2/kwil/main.py
--rw-r--r--   0 gavin      (501) staff       (20)     1774 2023-04-12 15:18:49.000000 kwil-0.0.2/kwil/manager.py
--rw-r--r--   0 gavin      (501) staff       (20)     1808 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/method.py
--rw-r--r--   0 gavin      (501) staff       (20)      783 2023-04-12 15:19:39.000000 kwil-0.0.2/kwil/middleware.py
--rw-r--r--   0 gavin      (501) staff       (20)     1014 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/module.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.187491 kwil-0.0.2/kwil/provider/
--rw-r--r--   0 gavin      (501) staff       (20)      167 2023-04-12 15:29:34.000000 kwil-0.0.2/kwil/provider/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     2074 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/provider/auto.py
--rw-r--r--   0 gavin      (501) staff       (20)     2344 2023-04-12 15:25:27.000000 kwil-0.0.2/kwil/provider/base.py
--rw-r--r--   0 gavin      (501) staff       (20)     1634 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/provider/grpc.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.178865 kwil-0.0.2/kwil/tx/
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.190413 kwil-0.0.2/kwil/tx/v1/
--rw-r--r--   0 gavin      (501) staff       (20)     1511 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/account_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/account_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1388 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/broadcast_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/broadcast_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1360 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/config_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/config_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     3435 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/dataset_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/dataset_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1264 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/list_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/list_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1219 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/ping_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/ping_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1375 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/price_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/price_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1264 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/query_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/query_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     4479 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/service_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)    14437 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/service_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     2062 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/tx_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/tx_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     3413 2023-04-12 20:01:31.000000 kwil-0.0.2/kwil/types.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.182946 kwil-0.0.2/kwil.egg-info/
--rw-r--r--   0 gavin      (501) staff       (20)     1020 2023-04-12 20:54:09.000000 kwil-0.0.2/kwil.egg-info/PKG-INFO
--rw-r--r--   0 gavin      (501) staff       (20)     1398 2023-04-12 20:54:09.000000 kwil-0.0.2/kwil.egg-info/SOURCES.txt
--rw-r--r--   0 gavin      (501) staff       (20)        1 2023-04-12 20:54:09.000000 kwil-0.0.2/kwil.egg-info/dependency_links.txt
--rw-r--r--   0 gavin      (501) staff       (20)      306 2023-04-12 20:54:09.000000 kwil-0.0.2/kwil.egg-info/requires.txt
--rw-r--r--   0 gavin      (501) staff       (20)       28 2023-04-12 20:54:09.000000 kwil-0.0.2/kwil.egg-info/top_level.txt
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.190836 kwil-0.0.2/kwil_typing/
--rw-r--r--   0 gavin      (501) staff       (20)       81 2023-04-12 15:29:41.000000 kwil-0.0.2/kwil_typing/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)      148 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil_typing/kvm.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.191377 kwil-0.0.2/kwil_utils/
--rw-r--r--   0 gavin      (501) staff       (20)      129 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil_utils/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     1065 2023-04-05 19:34:56.000000 kwil-0.0.2/kwil_utils/types.py
--rw-r--r--   0 gavin      (501) staff       (20)     1558 2023-04-12 20:52:23.000000 kwil-0.0.2/pyproject.toml
--rw-r--r--   0 gavin      (501) staff       (20)       38 2023-04-12 20:54:09.191796 kwil-0.0.2/setup.cfg
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.011729 kwil-0.0.3/
+-rw-r--r--   0 gavin      (501) staff       (20)     1064 2023-04-19 22:10:21.011576 kwil-0.0.3/PKG-INFO
+-rw-r--r--   0 gavin      (501) staff       (20)      404 2023-04-19 19:09:29.000000 kwil-0.0.3/README.md
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.001652 kwil-0.0.3/kwil/
+-rw-r--r--   0 gavin      (501) staff       (20)       87 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/__about__.py
+-rw-r--r--   0 gavin      (501) staff       (20)      322 2023-04-12 20:39:28.000000 kwil-0.0.3/kwil/__init__.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.005232 kwil-0.0.3/kwil/_utils/
+-rw-r--r--   0 gavin      (501) staff       (20)        0 2023-04-03 19:04:31.000000 kwil-0.0.3/kwil/_utils/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1555 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/action.py
+-rw-r--r--   0 gavin      (501) staff       (20)      346 2023-04-10 22:57:27.000000 kwil-0.0.3/kwil/_utils/dataset.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.005719 kwil-0.0.3/kwil/_utils/grpc/
+-rw-r--r--   0 gavin      (501) staff       (20)       56 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/grpc/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2935 2023-04-12 20:45:39.000000 kwil-0.0.3/kwil/_utils/grpc/client.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2183 2023-04-12 15:56:08.000000 kwil-0.0.3/kwil/_utils/method_formatters.py
+-rw-r--r--   0 gavin      (501) staff       (20)      719 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/naming_converter.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2796 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/request.py
+-rw-r--r--   0 gavin      (501) staff       (20)      504 2023-04-09 22:05:10.000000 kwil-0.0.3/kwil/_utils/rpcs.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1807 2023-04-12 20:01:31.000000 kwil-0.0.3/kwil/_utils/signature.py
+-rw-r--r--   0 gavin      (501) staff       (20)      185 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/signing.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1210 2023-04-12 14:59:57.000000 kwil-0.0.3/kwil/_utils/transaction.py
+-rw-r--r--   0 gavin      (501) staff       (20)      419 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/utils.py
+-rw-r--r--   0 gavin      (501) staff       (20)     3566 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/validation.py
+-rw-r--r--   0 gavin      (501) staff       (20)      404 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/exceptions.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1436 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/kwild.py
+-rw-r--r--   0 gavin      (501) staff       (20)     4463 2023-04-19 21:52:22.000000 kwil-0.0.3/kwil/main.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1774 2023-04-12 15:18:49.000000 kwil-0.0.3/kwil/manager.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1808 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/method.py
+-rw-r--r--   0 gavin      (501) staff       (20)      783 2023-04-12 15:19:39.000000 kwil-0.0.3/kwil/middleware.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1014 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/module.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.006732 kwil-0.0.3/kwil/provider/
+-rw-r--r--   0 gavin      (501) staff       (20)      167 2023-04-12 15:29:34.000000 kwil-0.0.3/kwil/provider/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2074 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/provider/auto.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2344 2023-04-12 15:25:27.000000 kwil-0.0.3/kwil/provider/base.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1634 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/provider/grpc.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:20.998353 kwil-0.0.3/kwil/tx/
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.010243 kwil-0.0.3/kwil/tx/v1/
+-rw-r--r--   0 gavin      (501) staff       (20)     1511 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/account_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/account_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1388 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/broadcast_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/broadcast_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1360 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/config_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/config_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     3435 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/dataset_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/dataset_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1264 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/list_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/list_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1219 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/ping_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/ping_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1375 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/price_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/price_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1264 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/query_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/query_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     4479 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/service_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)    14437 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/service_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2062 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/tx_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/tx_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     3413 2023-04-12 20:01:31.000000 kwil-0.0.3/kwil/types.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.002475 kwil-0.0.3/kwil.egg-info/
+-rw-r--r--   0 gavin      (501) staff       (20)     1064 2023-04-19 22:10:20.000000 kwil-0.0.3/kwil.egg-info/PKG-INFO
+-rw-r--r--   0 gavin      (501) staff       (20)     1398 2023-04-19 22:10:20.000000 kwil-0.0.3/kwil.egg-info/SOURCES.txt
+-rw-r--r--   0 gavin      (501) staff       (20)        1 2023-04-19 22:10:20.000000 kwil-0.0.3/kwil.egg-info/dependency_links.txt
+-rw-r--r--   0 gavin      (501) staff       (20)      306 2023-04-19 22:10:20.000000 kwil-0.0.3/kwil.egg-info/requires.txt
+-rw-r--r--   0 gavin      (501) staff       (20)       28 2023-04-19 22:10:20.000000 kwil-0.0.3/kwil.egg-info/top_level.txt
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.010713 kwil-0.0.3/kwil_typing/
+-rw-r--r--   0 gavin      (501) staff       (20)       81 2023-04-12 15:29:41.000000 kwil-0.0.3/kwil_typing/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)      148 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil_typing/kvm.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.011247 kwil-0.0.3/kwil_utils/
+-rw-r--r--   0 gavin      (501) staff       (20)      129 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil_utils/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1065 2023-04-05 19:34:56.000000 kwil-0.0.3/kwil_utils/types.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1558 2023-04-19 22:04:12.000000 kwil-0.0.3/pyproject.toml
+-rw-r--r--   0 gavin      (501) staff       (20)       38 2023-04-19 22:10:21.011772 kwil-0.0.3/setup.cfg
```

### Comparing `kwil-0.0.2/PKG-INFO` & `kwil-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwil
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for interacting with the kwil blockchain
 Author-email: yaiba <4yaiba@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/kwilteam/kwil.py
 Keywords: kwil
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -22,13 +22,13 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/kwil.svg)](https://pypi.org/project/kwil)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kwil.svg)](https://pypi.org/project/kwil)
 
 Borrows heavily from [web3.py](https://github.com/ethereum/web3.py)
 
 -----
 
-Check [quickstart](./docs/quickstart.md) to get started.
+Check [quickstart](https://github.com/kwilteam/kwil.py/blob/main/docs/quickstart.md) to get started.
 
 
 ## License
 
 MIT
```

### Comparing `kwil-0.0.2/kwil/_utils/action.py` & `kwil-0.0.3/kwil/_utils/action.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/_utils/grpc/client.py` & `kwil-0.0.3/kwil/_utils/grpc/client.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/_utils/method_formatters.py` & `kwil-0.0.3/kwil/_utils/method_formatters.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/_utils/naming_converter.py` & `kwil-0.0.3/kwil/_utils/naming_converter.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/_utils/request.py` & `kwil-0.0.3/kwil/_utils/request.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/_utils/signature.py` & `kwil-0.0.3/kwil/_utils/signature.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/_utils/transaction.py` & `kwil-0.0.3/kwil/_utils/transaction.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/_utils/validation.py` & `kwil-0.0.3/kwil/_utils/validation.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/kwild.py` & `kwil-0.0.3/kwil/kwild.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/main.py` & `kwil-0.0.3/kwil/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,27 +35,30 @@
 
         return __version__
 
     @classmethod
     def generate_dbi(cls, owner: str, db_name: str) -> DBIdentifier:
         return generate_dbi(owner, db_name)
 
+    @classmethod
+    def load_wallet(cls, private_key: str) -> LocalAccount:
+        return load_wallet(private_key)
+
 
 class Kwil(BaseKwil):
     def __init__(
         self,
         provider: Optional[BaseProvider] = None,
         wallet: Optional[LocalAccount] = None,
     ):
         self.manager = self.RequestManager(self, provider)
-
         self.kwild = Kwild(self)
 
         if wallet is None:
-            self._wallet = load_wallet(os.getenv("KWIL_ETH_PRIVATE_KEY"))
+            self._wallet = self.load_wallet(os.getenv("KWIL_ETH_PRIVATE_KEY"))
         else:
             self._wallet = wallet
 
     @property
     def kwil_provider(self) -> BaseProvider:
         return cast(BaseProvider, self.manager.provider)
```

### Comparing `kwil-0.0.2/kwil/manager.py` & `kwil-0.0.3/kwil/manager.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/method.py` & `kwil-0.0.3/kwil/method.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/middleware.py` & `kwil-0.0.3/kwil/middleware.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/module.py` & `kwil-0.0.3/kwil/module.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/provider/auto.py` & `kwil-0.0.3/kwil/provider/auto.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/provider/base.py` & `kwil-0.0.3/kwil/provider/base.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/provider/grpc.py` & `kwil-0.0.3/kwil/provider/grpc.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/tx/v1/account_pb2.py` & `kwil-0.0.3/kwil/tx/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/tx/v1/broadcast_pb2.py` & `kwil-0.0.3/kwil/tx/v1/broadcast_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/tx/v1/config_pb2.py` & `kwil-0.0.3/kwil/tx/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/tx/v1/dataset_pb2.py` & `kwil-0.0.3/kwil/tx/v1/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/tx/v1/list_pb2.py` & `kwil-0.0.3/kwil/tx/v1/list_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/tx/v1/ping_pb2.py` & `kwil-0.0.3/kwil/tx/v1/ping_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/tx/v1/price_pb2.py` & `kwil-0.0.3/kwil/tx/v1/price_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/tx/v1/query_pb2.py` & `kwil-0.0.3/kwil/tx/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/tx/v1/service_pb2.py` & `kwil-0.0.3/kwil/tx/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/tx/v1/service_pb2_grpc.py` & `kwil-0.0.3/kwil/tx/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/tx/v1/tx_pb2.py` & `kwil-0.0.3/kwil/tx/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil/types.py` & `kwil-0.0.3/kwil/types.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil.egg-info/PKG-INFO` & `kwil-0.0.3/kwil.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwil
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for interacting with the kwil blockchain
 Author-email: yaiba <4yaiba@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/kwilteam/kwil.py
 Keywords: kwil
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -22,13 +22,13 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/kwil.svg)](https://pypi.org/project/kwil)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kwil.svg)](https://pypi.org/project/kwil)
 
 Borrows heavily from [web3.py](https://github.com/ethereum/web3.py)
 
 -----
 
-Check [quickstart](./docs/quickstart.md) to get started.
+Check [quickstart](https://github.com/kwilteam/kwil.py/blob/main/docs/quickstart.md) to get started.
 
 
 ## License
 
 MIT
```

### Comparing `kwil-0.0.2/kwil.egg-info/SOURCES.txt` & `kwil-0.0.3/kwil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/kwil_utils/types.py` & `kwil-0.0.3/kwil_utils/types.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.2/pyproject.toml` & `kwil-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=67.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kwil"
 description = 'Library for interacting with the kwil blockchain'
-version = "0.0.2"
+version = "0.0.3"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT License"}
 keywords = ["kwil"]
 authors = [
   { name = "yaiba", email = "4yaiba@gmail.com" },
 ]
```

