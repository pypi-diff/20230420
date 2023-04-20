# Comparing `tmp/modelaapi-0.5.98.tar.gz` & `tmp/modelaapi-0.5.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelaapi-0.5.98.tar", last modified: Mon Sep 26 14:33:41 2022, max compression
+gzip compressed data, was "modelaapi-0.5.99.tar", last modified: Thu Sep 29 13:45:24 2022, max compression
```

## Comparing `modelaapi-0.5.98.tar` & `modelaapi-0.5.99.tar`

### file list

```diff
@@ -1,625 +1,625 @@
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.167627 modelaapi-0.5.98/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1416 2021-09-06 18:34:35.000000 modelaapi-0.5.98/.gitignore
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      139 2021-09-08 18:07:30.000000 modelaapi-0.5.98/AUTHORS.rst
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     3579 2021-10-28 18:18:31.000000 modelaapi-0.5.98/CONTRIBUTING.rst
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        0 2021-09-06 18:34:35.000000 modelaapi-0.5.98/DESCRIPTION.md
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)       89 2021-09-08 18:07:30.000000 modelaapi-0.5.98/HISTORY.rst
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11351 2021-09-06 18:34:35.000000 modelaapi-0.5.98/LICENSE.txt
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      437 2021-09-06 18:34:35.000000 modelaapi-0.5.98/MANIFEST.in
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1047 2022-03-12 21:07:22.000000 modelaapi-0.5.98/Makefile
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1413 2022-09-26 14:33:41.167627 modelaapi-0.5.98/PKG-INFO
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      762 2021-09-07 01:59:55.000000 modelaapi-0.5.98/README.md
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     5004 2022-02-24 22:17:22.000000 modelaapi-0.5.98/freeze.txt
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/gogo/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/gogo/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/gogo/protobuf/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/gogo/protobuf/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/gogo/protobuf/gogoproto/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/gogo/protobuf/gogoproto/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    21783 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/catalog/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    46858 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/data/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)   152309 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/inference/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    57823 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/infra/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)   141293 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/team/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    27490 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.067627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/training/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)   134900 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/account/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/account/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/account/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/account/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    25761 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    26423 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/alert/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/alert/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/alert/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13623 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11335 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/apitoken/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/apitoken/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/apitoken/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/apitoken/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16410 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/apitoken/v1/apitoken_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11800 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/apitoken/v1/apitoken_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/attachment/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/attachment/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/attachment/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    15551 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12110 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/batchpredictord/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/batchpredictord/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     7382 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     5517 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/catalog/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/catalog/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/catalog/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    40012 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    33508 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cloudproxyd/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17719 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14390 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/commit/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/commit/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/commit/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14479 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11490 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/common/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/common/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/common/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/common/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13579 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.077627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/connection/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/connection/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/connection/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16406 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14287 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/conversation/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/conversation/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/conversation/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    31897 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11484 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronprediction/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronprediction/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronprediction/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronprediction/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19227 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronprediction/v1/cronprediction_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19607 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronprediction/v1/cronprediction_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronreport/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronreport/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronreport/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronreport/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    18033 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronreport/v1/cronreport_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    18639 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronreport/v1/cronreport_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/curtain/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/curtain/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/curtain/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/curtain/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11853 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/curtain/v1/curtain_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11645 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/curtain/v1/curtain_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/data/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/data/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/data/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/data/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)   125460 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    94472 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataapp/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataapp/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataapp/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17089 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17941 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipeline/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipeline/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14921 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14642 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipelinerun/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19638 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19897 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproduct/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproduct/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14056 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12265 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproductversion/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.087627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproductversion/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14482 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13350 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataset/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataset/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataset/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    37400 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    35095 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datasource/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datasource/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datasource/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16743 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16324 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dbproxyd/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dbproxyd/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)   284084 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)   562344 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/entity/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/entity/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/entity/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11715 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11503 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/feature/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/feature/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/feature/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/feature/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11840 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/feature/v1/feature_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11645 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/feature/v1/feature_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurehistogram/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurehistogram/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13777 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13040 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipeline/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipeline/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipeline/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipeline/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17633 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipeline/v1/featurepipeline_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17562 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipeline/v1/featurepipeline_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipelinerun/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipelinerun/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipelinerun/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipelinerun/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14219 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipelinerun/v1/featurepipelinerun_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13344 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipelinerun/v1/featurepipelinerun_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featureset/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featureset/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featureset/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featureset/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12433 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featureset/v1/featureset_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12104 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featureset/v1/featureset_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/fileservices/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-16 19:26:25.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/fileservices/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.097627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/fileservices/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-16 19:26:20.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     3811 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     3345 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.047627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpc/
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.047627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpc/health/
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpc/health/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     2901 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     3056 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpcinferenceservice/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    38989 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    24869 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/k8score/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/k8score/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/k8score/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    41796 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    26279 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/lab/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/lab/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/lab/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13037 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11025 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipeline/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipeline/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipeline/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipeline/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17875 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipeline/v1/labelingpipeline_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17775 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipeline/v1/labelingpipeline_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipelinerun/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipelinerun/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipelinerun/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipelinerun/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14391 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipelinerun/v1/labelingpipelinerun_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13499 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipelinerun/v1/labelingpipelinerun_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/license/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/license/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/license/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/license/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    15310 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13831 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/meeting/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/meeting/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/meeting/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/meeting/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12619 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/meeting/v1/meeting_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11645 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/meeting/v1/meeting_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/model/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/model/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/model/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/model/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    38281 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    40277 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.107627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelasystem/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelasystem/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    24203 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19008 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    51863 2021-09-06 20:27:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12420 2021-09-06 20:27:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelautobuilder/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelautobuilder/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelautobuilder/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelautobuilder/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13817 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelautobuilder/v1/modelautobuilder_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13040 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelautobuilder/v1/modelautobuilder_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelcompilerrun/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelcompilerrun/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelcompilerrun/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelcompilerrun/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14484 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelcompilerrun/v1/modelcompilerrun_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13040 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelcompilerrun/v1/modelcompilerrun_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modeldsystem/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modeldsystem/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    51863 2021-09-07 02:02:44.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12420 2021-09-07 02:02:44.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipeline/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipeline/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipeline/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipeline/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19603 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipeline/v1/modelpipeline_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19393 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipeline/v1/modelpipeline_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipelinerun/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipelinerun/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipelinerun/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipelinerun/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    24987 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipelinerun/v1/modelpipelinerun_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    24886 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipelinerun/v1/modelpipelinerun_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebook/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebook/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebook/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebook/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12816 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebook/v1/notebook_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11800 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebook/v1/notebook_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebookrun/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebookrun/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebookrun/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebookrun/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13543 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebookrun/v1/notebookrun_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12265 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebookrun/v1/notebookrun_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notifier/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notifier/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notifier/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12814 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11800 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.117627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/objectstored/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/objectstored/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/objectstored/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     5944 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     9814 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/offlinefeaturestored/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14122 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    15252 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/onlinefeaturestored/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13713 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14925 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/postmortem/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/postmortem/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/postmortem/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12447 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12110 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/prediction/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/prediction/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/prediction/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16220 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16389 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictionstore/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictionstore/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     3804 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     3486 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictor/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictor/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictor/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16835 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16147 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/publisherd/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/publisherd/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/publisherd/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14571 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     9701 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/recipe/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/recipe/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/recipe/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    15635 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    15629 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/reciperun/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/reciperun/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/reciperun/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12224 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11955 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.127627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/report/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/report/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/report/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/report/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13410 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13561 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/review/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/review/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/review/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/review/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13565 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11484 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/runbook/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/runbook/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/runbook/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11795 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11645 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/servingsite/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/servingsite/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/servingsite/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12694 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12265 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlquery/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-10-31 22:37:41.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlquery/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-10-31 22:37:47.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13739 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13906 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlqueryrun/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-11-09 23:34:25.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-11-09 23:34:29.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14535 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14465 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/study/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/study/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/study/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/study/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    22327 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    23824 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/system/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/system/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/system/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/system/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14859 2021-10-23 14:06:51.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     7442 2021-10-23 14:06:51.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/tenant/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/tenant/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/tenant/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    15643 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13629 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/todo/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/todo/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/todo/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11282 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11180 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.137627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/trainerd/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/trainerd/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/trainerd/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    37187 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17719 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/userroleclass/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-04-05 16:56:53.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/userroleclass/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-04-05 16:56:56.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16143 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12588 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualbucket/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualbucket/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13015 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12575 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualcluster/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualcluster/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualcluster/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualcluster/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14210 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualcluster/v1/virtualcluster_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12730 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualcluster/v1/virtualcluster_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualvolume/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualvolume/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualvolume/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualvolume/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13877 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualvolume/v1/virtualvolume_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12575 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualvolume/v1/virtualvolume_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequest/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequest/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequest/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequest/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14244 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequest/v1/webrequest_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14274 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequest/v1/webrequest_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequestrun/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-11-09 23:34:40.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequestrun/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequestrun/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-11-09 23:34:44.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequestrun/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13029 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequestrun/v1/webrequestrun_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12575 2022-09-26 14:31:31.000000 modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequestrun/v1/webrequestrun_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/google/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/google/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/google/api/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/google/api/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1545 2022-09-26 14:31:31.000000 modelaapi-0.5.98/google/api/annotations_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/google/api/annotations_pb2_grpc.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     2997 2022-09-26 14:31:31.000000 modelaapi-0.5.98/google/api/http_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/google/api/http_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/k8s/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/k8s/io/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/k8s/io/api/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/api/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/k8s/io/api/apps/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2022-02-10 00:17:26.000000 modelaapi-0.5.98/k8s/io/api/apps/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.147627 modelaapi-0.5.98/k8s/io/api/apps/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2022-02-10 00:17:26.000000 modelaapi-0.5.98/k8s/io/api/apps/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    24763 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/api/apps/v1/generated_pb2.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/api/core/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/api/core/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/api/core/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/api/core/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)   183700 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/api/core/v1/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/api/core/v1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/api/rbac/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/api/rbac/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/api/rbac/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/api/rbac/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     9104 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/api/rbac/v1/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/api/rbac/v1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/apimachinery/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/apimachinery/pkg/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/apimachinery/pkg/api/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/api/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/apimachinery/pkg/api/resource/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/api/resource/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1971 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/apimachinery/pkg/apis/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/apis/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/apimachinery/pkg/apis/meta/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/apis/meta/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/apimachinery/pkg/apis/meta/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    33000 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/apimachinery/pkg/runtime/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/runtime/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     2609 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/apimachinery/pkg/runtime/schema/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      950 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/apimachinery/pkg/util/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/util/__init__.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/apimachinery/pkg/util/intstr/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/util/intstr/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1525 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.98/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.057627 modelaapi-0.5.98/k8s/io/apps/
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/apps/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/apps/v1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.057627 modelaapi-0.5.98/k8s/io/core/
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/core/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/core/v1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.057627 modelaapi-0.5.98/k8s/io/pkg/
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.057627 modelaapi-0.5.98/k8s/io/pkg/api/
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/pkg/api/resource/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/pkg/api/resource/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.057627 modelaapi-0.5.98/k8s/io/pkg/apis/
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.057627 modelaapi-0.5.98/k8s/io/pkg/apis/meta/
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/pkg/apis/meta/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/pkg/runtime/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/pkg/runtime/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/pkg/runtime/schema/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/pkg/runtime/schema/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.057627 modelaapi-0.5.98/k8s/io/pkg/util/
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/pkg/util/intstr/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/pkg/util/intstr/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.057627 modelaapi-0.5.98/k8s/io/rbac/
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.157627 modelaapi-0.5.98/k8s/io/rbac/v1/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-26 14:31:31.000000 modelaapi-0.5.98/k8s/io/rbac/v1/generated_pb2_grpc.py
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.167627 modelaapi-0.5.98/modelaapi/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      257 2021-09-06 18:34:35.000000 modelaapi-0.5.98/modelaapi/__init__.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     4077 2021-12-15 00:13:48.000000 modelaapi-0.5.98/modelaapi/custom_transformers.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1200 2022-09-26 14:33:36.000000 modelaapi-0.5.98/modelaapi/version.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        0 2021-09-06 18:34:35.000000 modelaapi-0.5.98/modelaapi/vim
-drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-26 14:33:41.167627 modelaapi-0.5.98/modelaapi.egg-info/
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1413 2022-09-26 14:33:40.000000 modelaapi-0.5.98/modelaapi.egg-info/PKG-INFO
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)    25319 2022-09-26 14:33:40.000000 modelaapi-0.5.98/modelaapi.egg-info/SOURCES.txt
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-09-26 14:33:40.000000 modelaapi-0.5.98/modelaapi.egg-info/dependency_links.txt
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-10-29 15:43:24.000000 modelaapi-0.5.98/modelaapi.egg-info/not-zip-safe
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)       36 2022-09-26 14:33:40.000000 modelaapi-0.5.98/modelaapi.egg-info/requires.txt
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)       28 2022-09-26 14:33:40.000000 modelaapi-0.5.98/modelaapi.egg-info/top_level.txt
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      645 2021-10-29 15:36:30.000000 modelaapi-0.5.98/packagify.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)       36 2022-09-13 21:08:38.000000 modelaapi-0.5.98/requirements.txt
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)      790 2022-09-26 14:33:41.167627 modelaapi-0.5.98/setup.cfg
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)     5349 2021-10-29 15:41:47.000000 modelaapi-0.5.98/setup.py
--rw-r--r--   0 tsagi     (1000) tsagi     (1000)        0 2022-08-04 00:22:23.000000 modelaapi-0.5.98/version.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.299281 modelaapi-0.5.99/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1416 2021-09-06 18:34:35.000000 modelaapi-0.5.99/.gitignore
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      139 2021-09-08 18:07:30.000000 modelaapi-0.5.99/AUTHORS.rst
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     3579 2021-10-28 18:18:31.000000 modelaapi-0.5.99/CONTRIBUTING.rst
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        0 2021-09-06 18:34:35.000000 modelaapi-0.5.99/DESCRIPTION.md
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)       89 2021-09-08 18:07:30.000000 modelaapi-0.5.99/HISTORY.rst
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11351 2021-09-06 18:34:35.000000 modelaapi-0.5.99/LICENSE.txt
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      437 2021-09-06 18:34:35.000000 modelaapi-0.5.99/MANIFEST.in
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1047 2022-03-12 21:07:22.000000 modelaapi-0.5.99/Makefile
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1413 2022-09-29 13:45:24.299281 modelaapi-0.5.99/PKG-INFO
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      762 2021-09-07 01:59:55.000000 modelaapi-0.5.99/README.md
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     5004 2022-02-24 22:17:22.000000 modelaapi-0.5.99/freeze.txt
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.999281 modelaapi-0.5.99/github/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.999281 modelaapi-0.5.99/github/com/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.999281 modelaapi-0.5.99/github/com/gogo/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/gogo/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.999281 modelaapi-0.5.99/github/com/gogo/protobuf/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/gogo/protobuf/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.009281 modelaapi-0.5.99/github/com/gogo/protobuf/gogoproto/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/gogo/protobuf/gogoproto/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    21783 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.009281 modelaapi-0.5.99/github/com/metaprov/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.009281 modelaapi-0.5.99/github/com/metaprov/modelaapi/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.009281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.009281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.009281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/catalog/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.009281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    47486 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.009281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/data/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.009281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)   151328 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.009281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/inference/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.019281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    57823 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.019281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/infra/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.039281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)   141293 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.039281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/team/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.039281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    27490 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.039281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/training/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.039281 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)   134807 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.039281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.039281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/account/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/account/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.039281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/account/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/account/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    25761 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    26423 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.049281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/alert/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/alert/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.049281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/alert/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13623 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11335 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.049281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/apitoken/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/apitoken/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.049281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/apitoken/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/apitoken/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16410 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/apitoken/v1/apitoken_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11800 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/apitoken/v1/apitoken_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.049281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/attachment/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/attachment/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.049281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/attachment/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    15551 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12110 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.049281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/batchpredictord/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.049281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/batchpredictord/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     7382 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     5517 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.049281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/catalog/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/catalog/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.049281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/catalog/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    40012 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    33508 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.059281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cloudproxyd/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.059281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17719 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14390 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.059281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/commit/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/commit/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.059281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/commit/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14479 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11490 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.059281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/common/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/common/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.059281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/common/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/common/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13579 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.059281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/connection/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/connection/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.059281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/connection/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16406 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14287 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.069281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/conversation/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/conversation/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.069281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/conversation/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    31897 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11484 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.069281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronprediction/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronprediction/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.069281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronprediction/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronprediction/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19227 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronprediction/v1/cronprediction_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19607 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronprediction/v1/cronprediction_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.069281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronreport/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronreport/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.069281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronreport/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronreport/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    18033 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronreport/v1/cronreport_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    18639 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronreport/v1/cronreport_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.069281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/curtain/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/curtain/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.069281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/curtain/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/curtain/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11853 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/curtain/v1/curtain_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11645 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/curtain/v1/curtain_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.069281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/data/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/data/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.089281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/data/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/data/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)   125460 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    94472 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.099281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataapp/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataapp/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.099281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataapp/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17089 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17941 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.099281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipeline/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.099281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipeline/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14921 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14642 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.099281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipelinerun/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.099281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19638 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19897 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.099281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproduct/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.099281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproduct/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14056 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12265 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.099281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproductversion/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.109281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproductversion/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14482 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13350 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.109281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataset/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataset/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.109281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataset/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    37400 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    35095 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.109281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datasource/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datasource/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.109281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datasource/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16743 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16324 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.119281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dbproxyd/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.119281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dbproxyd/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)   284084 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)   562344 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.119281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/entity/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/entity/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.119281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/entity/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11715 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11503 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.119281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/feature/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/feature/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.119281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/feature/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/feature/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11840 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/feature/v1/feature_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11645 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/feature/v1/feature_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.119281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurehistogram/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.129281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurehistogram/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13777 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13040 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.129281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipeline/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipeline/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.129281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipeline/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipeline/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17633 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipeline/v1/featurepipeline_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17562 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipeline/v1/featurepipeline_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.129281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipelinerun/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipelinerun/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.129281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipelinerun/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipelinerun/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14219 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipelinerun/v1/featurepipelinerun_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13344 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipelinerun/v1/featurepipelinerun_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.129281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featureset/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featureset/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.129281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featureset/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featureset/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12433 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featureset/v1/featureset_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12104 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featureset/v1/featureset_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.129281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/fileservices/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-16 19:26:25.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/fileservices/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.139281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/fileservices/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-16 19:26:20.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     3811 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     3345 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.939281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpc/
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.939281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpc/health/
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.139281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpc/health/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     2901 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     3056 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.139281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpcinferenceservice/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.139281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    38989 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    24869 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.139281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/k8score/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/k8score/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.139281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/k8score/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    41796 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    26279 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.139281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/lab/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/lab/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.139281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/lab/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13037 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11025 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.139281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipeline/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipeline/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.149281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipeline/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipeline/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17875 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipeline/v1/labelingpipeline_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17775 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipeline/v1/labelingpipeline_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.149281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipelinerun/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipelinerun/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.149281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipelinerun/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipelinerun/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14391 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipelinerun/v1/labelingpipelinerun_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13499 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipelinerun/v1/labelingpipelinerun_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.149281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/license/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/license/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.149281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/license/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/license/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    15310 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13831 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.149281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/meeting/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/meeting/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.149281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/meeting/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/meeting/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12619 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/meeting/v1/meeting_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11645 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/meeting/v1/meeting_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.149281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/model/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/model/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.159281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/model/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/model/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    38281 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    40277 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.159281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelasystem/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.159281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelasystem/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    24203 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19008 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    51863 2021-09-06 20:27:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12420 2021-09-06 20:27:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.159281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelautobuilder/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelautobuilder/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.159281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelautobuilder/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelautobuilder/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13817 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelautobuilder/v1/modelautobuilder_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13040 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelautobuilder/v1/modelautobuilder_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.159281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelcompilerrun/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelcompilerrun/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.159281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelcompilerrun/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelcompilerrun/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14484 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelcompilerrun/v1/modelcompilerrun_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13040 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelcompilerrun/v1/modelcompilerrun_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.159281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modeldsystem/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.169281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modeldsystem/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    51863 2021-09-07 02:02:44.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12420 2021-09-07 02:02:44.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.169281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipeline/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipeline/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.179281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipeline/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipeline/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19603 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipeline/v1/modelpipeline_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    19393 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipeline/v1/modelpipeline_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.179281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipelinerun/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipelinerun/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.179281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipelinerun/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipelinerun/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    24987 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipelinerun/v1/modelpipelinerun_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    24886 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipelinerun/v1/modelpipelinerun_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.179281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebook/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebook/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.179281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebook/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebook/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12816 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebook/v1/notebook_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11800 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebook/v1/notebook_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.179281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebookrun/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebookrun/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.179281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebookrun/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebookrun/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13543 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebookrun/v1/notebookrun_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12265 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebookrun/v1/notebookrun_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.179281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notifier/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notifier/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.179281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notifier/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12814 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11800 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.179281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/objectstored/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/objectstored/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.179281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/objectstored/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     5944 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     9814 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.179281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/offlinefeaturestored/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.199281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14122 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    15252 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.199281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/onlinefeaturestored/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.199281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13713 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14925 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.199281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/postmortem/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/postmortem/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.199281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/postmortem/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12447 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12110 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.199281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/prediction/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/prediction/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.199281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/prediction/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16220 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16389 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.199281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictionstore/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.199281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictionstore/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     3804 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     3486 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.199281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictor/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictor/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.199281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictor/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16835 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16147 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.199281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/publisherd/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/publisherd/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/publisherd/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14571 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     9701 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/recipe/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/recipe/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/recipe/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    15635 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    15629 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/reciperun/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/reciperun/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/reciperun/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12224 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11955 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/report/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/report/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/report/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/report/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13410 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13561 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/review/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/review/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/review/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/review/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13565 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11484 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/runbook/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/runbook/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/runbook/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11795 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11645 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/servingsite/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/servingsite/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.209281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/servingsite/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12694 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12265 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.219281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlquery/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-10-31 22:37:41.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.229281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlquery/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-10-31 22:37:47.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13739 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13906 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.229281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlqueryrun/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-11-09 23:34:25.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.229281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-11-09 23:34:29.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14535 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14465 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.229281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/study/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/study/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.229281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/study/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/study/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    22327 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    23824 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.229281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/system/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/system/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.229281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/system/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-02-10 00:17:26.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/system/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14859 2021-10-23 14:06:51.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     7442 2021-10-23 14:06:51.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.229281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/tenant/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/tenant/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.229281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/tenant/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    15643 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13629 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.229281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/todo/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/todo/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/todo/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11282 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    11180 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/trainerd/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/trainerd/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/trainerd/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    37187 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    17719 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/userroleclass/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-04-05 16:56:53.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/userroleclass/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-04-05 16:56:56.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    16143 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12588 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualbucket/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualbucket/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13015 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12575 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualcluster/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualcluster/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualcluster/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualcluster/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14210 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualcluster/v1/virtualcluster_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12730 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualcluster/v1/virtualcluster_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualvolume/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualvolume/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualvolume/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualvolume/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13877 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualvolume/v1/virtualvolume_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12575 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualvolume/v1/virtualvolume_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequest/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequest/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequest/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-09-06 18:34:35.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequest/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14244 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequest/v1/webrequest_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    14274 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequest/v1/webrequest_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.239281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequestrun/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-11-09 23:34:40.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequestrun/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.249281 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequestrun/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-11-09 23:34:44.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequestrun/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    13029 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequestrun/v1/webrequestrun_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    12575 2022-09-27 22:20:55.000000 modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequestrun/v1/webrequestrun_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.249281 modelaapi-0.5.99/google/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/google/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.249281 modelaapi-0.5.99/google/api/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/google/api/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1545 2022-09-27 22:20:55.000000 modelaapi-0.5.99/google/api/annotations_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     2997 2022-09-27 22:20:55.000000 modelaapi-0.5.99/google/api/http_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/google/api/http_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.249281 modelaapi-0.5.99/k8s/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.249281 modelaapi-0.5.99/k8s/io/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.249281 modelaapi-0.5.99/k8s/io/api/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/api/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.259281 modelaapi-0.5.99/k8s/io/api/apps/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2022-02-10 00:17:26.000000 modelaapi-0.5.99/k8s/io/api/apps/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.259281 modelaapi-0.5.99/k8s/io/api/apps/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2022-02-10 00:17:26.000000 modelaapi-0.5.99/k8s/io/api/apps/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    24763 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/api/apps/v1/generated_pb2.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.259281 modelaapi-0.5.99/k8s/io/api/core/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/api/core/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.259281 modelaapi-0.5.99/k8s/io/api/core/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/api/core/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)   183700 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/api/core/v1/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/api/core/v1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.259281 modelaapi-0.5.99/k8s/io/api/rbac/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/api/rbac/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.259281 modelaapi-0.5.99/k8s/io/api/rbac/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/api/rbac/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     9104 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/api/rbac/v1/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/api/rbac/v1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.259281 modelaapi-0.5.99/k8s/io/apimachinery/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.259281 modelaapi-0.5.99/k8s/io/apimachinery/pkg/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.259281 modelaapi-0.5.99/k8s/io/apimachinery/pkg/api/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/api/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.269281 modelaapi-0.5.99/k8s/io/apimachinery/pkg/api/resource/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/api/resource/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1971 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.269281 modelaapi-0.5.99/k8s/io/apimachinery/pkg/apis/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/apis/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.269281 modelaapi-0.5.99/k8s/io/apimachinery/pkg/apis/meta/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/apis/meta/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.269281 modelaapi-0.5.99/k8s/io/apimachinery/pkg/apis/meta/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    33000 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.279281 modelaapi-0.5.99/k8s/io/apimachinery/pkg/runtime/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/runtime/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     2609 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.289281 modelaapi-0.5.99/k8s/io/apimachinery/pkg/runtime/schema/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      950 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.289281 modelaapi-0.5.99/k8s/io/apimachinery/pkg/util/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/util/__init__.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.289281 modelaapi-0.5.99/k8s/io/apimachinery/pkg/util/intstr/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      170 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/util/intstr/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1525 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2021-09-06 18:34:35.000000 modelaapi-0.5.99/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.979281 modelaapi-0.5.99/k8s/io/apps/
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.289281 modelaapi-0.5.99/k8s/io/apps/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/apps/v1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.979281 modelaapi-0.5.99/k8s/io/core/
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.289281 modelaapi-0.5.99/k8s/io/core/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/core/v1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.979281 modelaapi-0.5.99/k8s/io/pkg/
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.979281 modelaapi-0.5.99/k8s/io/pkg/api/
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.289281 modelaapi-0.5.99/k8s/io/pkg/api/resource/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/pkg/api/resource/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.979281 modelaapi-0.5.99/k8s/io/pkg/apis/
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.979281 modelaapi-0.5.99/k8s/io/pkg/apis/meta/
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.289281 modelaapi-0.5.99/k8s/io/pkg/apis/meta/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.289281 modelaapi-0.5.99/k8s/io/pkg/runtime/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/pkg/runtime/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.289281 modelaapi-0.5.99/k8s/io/pkg/runtime/schema/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/pkg/runtime/schema/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.989281 modelaapi-0.5.99/k8s/io/pkg/util/
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.289281 modelaapi-0.5.99/k8s/io/pkg/util/intstr/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/pkg/util/intstr/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:23.989281 modelaapi-0.5.99/k8s/io/rbac/
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.289281 modelaapi-0.5.99/k8s/io/rbac/v1/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      159 2022-09-27 22:20:55.000000 modelaapi-0.5.99/k8s/io/rbac/v1/generated_pb2_grpc.py
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.299281 modelaapi-0.5.99/modelaapi/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      257 2021-09-06 18:34:35.000000 modelaapi-0.5.99/modelaapi/__init__.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     4077 2021-12-15 00:13:48.000000 modelaapi-0.5.99/modelaapi/custom_transformers.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1200 2022-09-29 13:45:12.000000 modelaapi-0.5.99/modelaapi/version.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        0 2021-09-06 18:34:35.000000 modelaapi-0.5.99/modelaapi/vim
+drwxr-xr-x   0 tsagi     (1000) tsagi     (1000)        0 2022-09-29 13:45:24.299281 modelaapi-0.5.99/modelaapi.egg-info/
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     1413 2022-09-29 13:45:23.000000 modelaapi-0.5.99/modelaapi.egg-info/PKG-INFO
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)    25319 2022-09-29 13:45:23.000000 modelaapi-0.5.99/modelaapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2022-09-29 13:45:23.000000 modelaapi-0.5.99/modelaapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        1 2021-10-29 15:43:24.000000 modelaapi-0.5.99/modelaapi.egg-info/not-zip-safe
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)       36 2022-09-29 13:45:23.000000 modelaapi-0.5.99/modelaapi.egg-info/requires.txt
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)       28 2022-09-29 13:45:23.000000 modelaapi-0.5.99/modelaapi.egg-info/top_level.txt
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      645 2021-10-29 15:36:30.000000 modelaapi-0.5.99/packagify.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)       36 2022-09-13 21:08:38.000000 modelaapi-0.5.99/requirements.txt
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)      790 2022-09-29 13:45:24.299281 modelaapi-0.5.99/setup.cfg
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)     5349 2021-10-29 15:41:47.000000 modelaapi-0.5.99/setup.py
+-rw-r--r--   0 tsagi     (1000) tsagi     (1000)        0 2022-08-04 00:22:23.000000 modelaapi-0.5.99/version.py
```

### Comparing `modelaapi-0.5.98/.gitignore` & `modelaapi-0.5.99/.gitignore`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/CONTRIBUTING.rst` & `modelaapi-0.5.99/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/LICENSE.txt` & `modelaapi-0.5.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/Makefile` & `modelaapi-0.5.99/Makefile`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/PKG-INFO` & `modelaapi-0.5.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.5.98
+Version: 0.5.99
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
-Download-URL: https://github.com/metaptov/modelaapi/tarball/v0.5.98
+Download-URL: https://github.com/metaptov/modelaapi/tarball/v0.5.99
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaptov/modelaapi/tarball/v0.5.98
+Project-URL: Download, https://github.com/metaptov/modelaapi/tarball/v0.5.99
 Project-URL: Source, https://github.com/metaptov/modelaapi
 Project-URL: Tracker, https://github.com/metaptov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `modelaapi-0.5.98/README.md` & `modelaapi-0.5.99/README.md`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/freeze.txt` & `modelaapi-0.5.99/freeze.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/gogo/protobuf/gogoproto/gogo_pb2.py` & `modelaapi-0.5.99/github/com/gogo/protobuf/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.api.resource import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_api_dot_resource_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x12\x37github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/api/resource/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\xa5\x01\n\tAlgorithm\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AlgorithmSpec\"\xa4\x01\n\rAlgorithmList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\x98\x03\n\rAlgorithmSpec\x12\x15\n\rframeworkName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\x12\x0e\n\x06sparse\x18\x05 \x01(\x08\x12`\n\x11integerParameters\x18\x06 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.IntParameter\x12`\n\x0f\x66loatParameters\x18\x07 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FloatParameter\x12l\n\x15\x63\x61tegoricalParameters\x18\x08 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CategoricalParameter\"I\n\x14\x43\x61tegoricalParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x02 \x01(\t\x12\r\n\x05\x65nums\x18\x03 \x03(\t\"\xf3\x01\n\x05\x43loud\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudStatus\"\x9c\x01\n\tCloudList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Cloud\"\xec\x02\n\tCloudSpec\x12\x19\n\x11\x64\x65\x66\x61ultRegionName\x18\x01 \x01(\t\x12\x1f\n\x17\x64\x65\x66\x61ultMachineClassName\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ultGpuClassName\x18\x03 \x01(\t\x12]\n\x0emachineClasses\x18\x04 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClass\x12U\n\ngpuClasses\x18\x05 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClass\x12P\n\x07regions\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Region\"\xc7\x01\n\x0b\x43loudStatus\x12_\n\x0cmachineCosts\x18\x01 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClassCost\x12W\n\x08gpuCosts\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClassCost\"A\n\x0c\x43ompilerSpec\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\x12\x10\n\x08\x63ompiler\x18\x02 \x01(\t\x12\x0f\n\x07targets\x18\x03 \x03(\t\"l\n\x0f\x43onfusionMatrix\x12Y\n\x04rows\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrixRow\"F\n\x12\x43onfusionMatrixRow\x12\t\n\x01t\x18\x01 \x01(\t\x12\t\n\x01p\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x05\x12\x0b\n\x03pct\x18\x04 \x01(\x01\";\n\x0c\x43ontainerLog\x12\x0b\n\x03job\x18\x01 \x01(\t\x12\x11\n\tcontainer\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\"\"\n\nCurvePoint\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"(\n\nDataCenter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"\xb1\x04\n\x0c\x44\x61taTestCase\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nassertThat\x18\x03 \x01(\t\x12\x36\n\tentityRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0c\x63ompareToRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\x12\x0c\n\x04type\x18\x07 \x01(\t\x12\x0e\n\x06metric\x18\x08 \x01(\t\x12\x15\n\rexpectedValue\x18\t \x01(\x01\x12\x18\n\x10\x65xpectedCategory\x18\n \x01(\t\x12\r\n\x05lower\x18\x0b \x01(\x01\x12\r\n\x05upper\x18\x0c \x01(\x01\x12\x13\n\x0b\x65xpectedSet\x18\r \x03(\t\x12\x16\n\x0elowerInclusive\x18\x0e \x01(\x08\x12\x16\n\x0eupperInclusive\x18\x0f \x01(\x08\x12\x11\n\tgenerated\x18\x10 \x01(\x08\x12\x0c\n\x04tags\x18\x11 \x03(\t\x12\x0f\n\x07\x63olumn2\x18\x12 \x01(\t\x12\x37\n\nentityRef2\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x63olumns\x18\x14 \x03(\t\x12\x15\n\rfeatureFilter\x18\x15 \x01(\t\x12\x15\n\rreferenceType\x18\x16 \x01(\t\x12\x0f\n\x07periods\x18\x17 \x01(\x05\"\xac\x01\n\x12\x44\x61taTestCaseResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12T\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x0f\n\x07\x66\x61ilure\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\"[\n\x0e\x46loatParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\x0b\n\x03max\x18\x04 \x01(\x01\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x05 \x01(\x01\x12\x0b\n\x03log\x18\x06 \x01(\x08\"t\n\x0cGithubEvents\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x15\n\rblobNameRegex\x18\x04 \x01(\t\x12\x0e\n\x06\x65vents\x18\x05 \x03(\t\"z\n\x08GpuClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12\x0c\n\x04vcpu\x18\x03 \x01(\x05\x12>\n\x06gpumem\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xb5\x01\n\x0cGpuClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"c\n\rHistogramData\x12\x0c\n\x04\x62ins\x18\x01 \x03(\x01\x12\x12\n\ncategories\x18\x02 \x03(\t\x12\x0e\n\x06\x63ounts\x18\x03 \x03(\x01\x12\x0f\n\x07missing\x18\x04 \x01(\x05\x12\x0f\n\x07invalid\x18\x05 \x01(\x05\"I\n\x06Images\x12\x14\n\x0ctrainerImage\x18\x01 \x01(\t\x12\x11\n\tdataImage\x18\x02 \x01(\t\x12\x16\n\x0epublisherImage\x18\x03 \x01(\t\"Z\n\x0cIntParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03min\x18\x03 \x01(\x05\x12\x0b\n\x03max\x18\x04 \x01(\x05\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x06 \x01(\x05\"\xb2\x01\n\rLastRunStatus\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x42\n\x0e\x63ompletionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08\x64uration\x18\x04 \x01(\x05\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\"*\n\x03Lib\x12\x12\n\nframeworks\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"u\n\x04Logs\x12\x12\n\nbucketName\x18\x01 \x01(\t\x12Y\n\ncontainers\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ContainerLog\"\xa9\x01\n\x0bMLFramework\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFrameworkSpec\"\xa8\x01\n\x0fMLFrameworkList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFramework\"R\n\x0fMLFrameworkSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0c\n\x04lang\x18\x04 \x01(\t\"\x8c\x01\n\x0cMachineClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12;\n\x03mem\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12\x0c\n\x04vcpu\x18\x04 \x01(\x05\x12\x0f\n\x07storage\x18\x05 \x01(\t\"\xb9\x01\n\x10MachineClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xab\x01\n\x0cManagedImage\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImageSpec\"\xaa\x01\n\x10ManagedImageList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImage\"\xbb\x03\n\x10ManagedImageSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x10\n\x08registry\x18\x02 \x01(\t\x12\x12\n\nrepository\x18\x03 \x01(\t\x12\x0b\n\x03tag\x18\x04 \x01(\t\x12\'\n\x03\x65nv\x18\x05 \x03(\x0b\x32\x1a.k8s.io.api.core.v1.EnvVar\x12\x0b\n\x03gpu\x18\x06 \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\x07 \x01(\x08\x12\x0f\n\x07preload\x18\x08 \x01(\x08\x12:\n\rconnectionRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04\x62\x61se\x18\n \x01(\t\x12\x0c\n\x04role\x18\x0b \x01(\t\x12\x13\n\x0bmantainedBy\x18\x0c \x01(\t\x12\x0b\n\x03uri\x18\r \x01(\t\x12\x12\n\nframeworks\x18\x0e \x03(\t\x12J\n\x04libs\x18\x0f \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Lib\x12\n\n\x02os\x18\x10 \x01(\t\x12\x11\n\tosVersion\x18\x11 \x01(\t\x12\x0f\n\x07private\x18\x12 \x01(\x08\"\xf5\x01\n\x0bMeasurement\x12\x33\n\x06\x65ntity\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0e\n\x06metric\x18\x03 \x01(\t\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0e\n\x06stddev\x18\x05 \x01(\x01\x12\x0f\n\x07\x62oolQty\x18\x06 \x01(\x08\x12\x10\n\x08\x63\x61tegory\x18\x07 \x01(\t\x12\x10\n\x08valueSet\x18\x08 \x03(\t\x12=\n\ttimePoint\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xb3\x02\n\x13ModelDeploymentSpec\x12\x35\n\x08modelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x14\n\x0cmodelVersion\x18\x03 \x01(\t\x12\x0f\n\x07traffic\x18\x04 \x01(\x05\x12\x0c\n\x04role\x18\x05 \x01(\t\x12\x10\n\x08mountTar\x18\t \x01(\x08\x12\x17\n\x0ftrafficSelector\x18\n \x01(\t\x12\x37\n\napprovedBy\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\r \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xea\x01\n\x10NotificationSpec\x12\x10\n\x08\x65rrorTTL\x18\x02 \x01(\x05\x12\x12\n\nsuccessTTL\x18\x04 \x01(\x05\x12\x14\n\x0cnotifierName\x18\x05 \x01(\t\x12i\n\x08selector\x18\x06 \x03(\x0b\x32W.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec.SelectorEntry\x1a/\n\rSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"^\n\x07PRCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"m\n\x0fPermissionsSpec\x12Z\n\x0cstakeholders\x18\x01 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Stakeholder\"\xb1\x01\n\x0fPretrainedModel\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModelSpec\"\xb0\x01\n\x13PretrainedModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModel\"$\n\x13PretrainedModelSpec\x12\r\n\x05image\x18\x01 \x01(\t\"\xad\x01\n\rPublicDataset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDatasetSpec\"\xac\x01\n\x11PublicDatasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDataset\"\xb6\x02\n\x11PublicDatasetSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\x10\n\x08openMLID\x18\x04 \x01(\t\x12\x0f\n\x07\x64\x61taUrl\x18\x05 \x01(\t\x12\x10\n\x08\x63itation\x18\x06 \x01(\t\x12\x0c\n\x04rows\x18\x07 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x08 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\t \x01(\x05\x12\x14\n\x0ctargetColumn\x18\n \x01(\t\x12\x10\n\x08industry\x18\x0b \x01(\t\x12\x12\n\nimbalanced\x18\x0c \x01(\x08\x12\x14\n\x0c\x64\x61tasourceCR\x18\r \x01(\t\x12\x11\n\tdatasetCR\x18\x0e \x01(\t\x12\x0f\n\x07studyCR\x18\x0f \x01(\t\x12\x15\n\rdataProductCR\x18\x10 \x01(\t\"\xb6\x01\n\x06Region\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x1d\n\x15\x64\x65\x66\x61ultDatacenterName\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x13\n\x0b\x62illingCode\x18\x04 \x01(\t\x12X\n\x0b\x64\x61tacenters\x18\x05 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataCenter\"\xe2\x01\n\x0cResourceSpec\x12\x14\n\x0cworkloadName\x18\x01 \x01(\t\x12\x0e\n\x06\x63ustom\x18\x02 \x01(\x08\x12\x35\n\x08\x63puImage\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x35\n\x08gpuImage\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\x0crequirements\x18\x05 \x01(\x0b\x32(.k8s.io.api.core.v1.ResourceRequirements\"b\n\x0bRocAucCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\xb6\x01\n\x0bRunSchedule\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12=\n\tstartTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04\x63ron\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\"R\n\x0bStakeholder\x12\x0f\n\x07\x61\x63\x63ount\x18\x01 \x01(\t\x12\x32\n\x05roles\x18\x02 \x03(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"r\n\tTestSuite\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12T\n\x05tests\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCase\"\xc4\x02\n\x0fTestSuiteResult\x12\x36\n\tentityRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08\x66\x61ilures\x18\x02 \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x03 \x01(\x05\x12=\n\tstartTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12<\n\x08stopTime\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Z\n\x05tests\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCaseResult\"#\n\x06VizUri\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\"\xad\x01\n\rWorkloadClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClassSpec\"\xac\x01\n\x11WorkloadClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClass\"u\n\x11WorkloadClassSpec\x12`\n\x11resourcesTemplate\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpecB9Z7github.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x12\x37github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/api/resource/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\xa5\x01\n\tAlgorithm\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AlgorithmSpec\"\xa4\x01\n\rAlgorithmList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\x98\x03\n\rAlgorithmSpec\x12\x15\n\rframeworkName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\x12\x0e\n\x06sparse\x18\x05 \x01(\x08\x12`\n\x11integerParameters\x18\x06 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.IntParameter\x12`\n\x0f\x66loatParameters\x18\x07 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FloatParameter\x12l\n\x15\x63\x61tegoricalParameters\x18\x08 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CategoricalParameter\"I\n\x14\x43\x61tegoricalParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x02 \x01(\t\x12\r\n\x05\x65nums\x18\x03 \x03(\t\"\xf3\x01\n\x05\x43loud\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudStatus\"\x9c\x01\n\tCloudList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Cloud\"\xec\x02\n\tCloudSpec\x12\x19\n\x11\x64\x65\x66\x61ultRegionName\x18\x01 \x01(\t\x12\x1f\n\x17\x64\x65\x66\x61ultMachineClassName\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ultGpuClassName\x18\x03 \x01(\t\x12]\n\x0emachineClasses\x18\x04 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClass\x12U\n\ngpuClasses\x18\x05 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClass\x12P\n\x07regions\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Region\"\xc7\x01\n\x0b\x43loudStatus\x12_\n\x0cmachineCosts\x18\x01 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClassCost\x12W\n\x08gpuCosts\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClassCost\"A\n\x0c\x43ompilerSpec\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\x12\x10\n\x08\x63ompiler\x18\x02 \x01(\t\x12\x0f\n\x07targets\x18\x03 \x03(\t\"l\n\x0f\x43onfusionMatrix\x12Y\n\x04rows\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrixRow\"F\n\x12\x43onfusionMatrixRow\x12\t\n\x01t\x18\x01 \x01(\t\x12\t\n\x01p\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x05\x12\x0b\n\x03pct\x18\x04 \x01(\x01\";\n\x0c\x43ontainerLog\x12\x0b\n\x03job\x18\x01 \x01(\t\x12\x11\n\tcontainer\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\"\"\n\nCurvePoint\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"(\n\nDataCenter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"\xb1\x04\n\x0c\x44\x61taTestCase\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nassertThat\x18\x03 \x01(\t\x12\x36\n\tentityRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0c\x63ompareToRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\x12\x0c\n\x04type\x18\x07 \x01(\t\x12\x0e\n\x06metric\x18\x08 \x01(\t\x12\x15\n\rexpectedValue\x18\t \x01(\x01\x12\x18\n\x10\x65xpectedCategory\x18\n \x01(\t\x12\r\n\x05lower\x18\x0b \x01(\x01\x12\r\n\x05upper\x18\x0c \x01(\x01\x12\x13\n\x0b\x65xpectedSet\x18\r \x03(\t\x12\x16\n\x0elowerInclusive\x18\x0e \x01(\x08\x12\x16\n\x0eupperInclusive\x18\x0f \x01(\x08\x12\x11\n\tgenerated\x18\x10 \x01(\x08\x12\x0c\n\x04tags\x18\x11 \x03(\t\x12\x0f\n\x07\x63olumn2\x18\x12 \x01(\t\x12\x37\n\nentityRef2\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x63olumns\x18\x14 \x03(\t\x12\x15\n\rfeatureFilter\x18\x15 \x01(\t\x12\x15\n\rreferenceType\x18\x16 \x01(\t\x12\x0f\n\x07periods\x18\x17 \x01(\x05\"\xac\x01\n\x12\x44\x61taTestCaseResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12T\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x0f\n\x07\x66\x61ilure\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\"[\n\x0e\x46loatParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\x0b\n\x03max\x18\x04 \x01(\x01\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x05 \x01(\x01\x12\x0b\n\x03log\x18\x06 \x01(\x08\"t\n\x0cGithubEvents\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x15\n\rblobNameRegex\x18\x04 \x01(\t\x12\x0e\n\x06\x65vents\x18\x05 \x03(\t\"z\n\x08GpuClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12\x0c\n\x04vcpu\x18\x03 \x01(\x05\x12>\n\x06gpumem\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xb5\x01\n\x0cGpuClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"c\n\rHistogramData\x12\x0c\n\x04\x62ins\x18\x01 \x03(\x01\x12\x12\n\ncategories\x18\x02 \x03(\t\x12\x0e\n\x06\x63ounts\x18\x03 \x03(\x01\x12\x0f\n\x07missing\x18\x04 \x01(\x05\x12\x0f\n\x07invalid\x18\x05 \x01(\x05\"I\n\x06Images\x12\x14\n\x0ctrainerImage\x18\x01 \x01(\t\x12\x11\n\tdataImage\x18\x02 \x01(\t\x12\x16\n\x0epublisherImage\x18\x03 \x01(\t\"Z\n\x0cIntParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03min\x18\x03 \x01(\x05\x12\x0b\n\x03max\x18\x04 \x01(\x05\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x06 \x01(\x05\"\xb2\x01\n\rLastRunStatus\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x42\n\x0e\x63ompletionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08\x64uration\x18\x04 \x01(\x05\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\"*\n\x03Lib\x12\x12\n\nframeworks\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"u\n\x04Logs\x12\x12\n\nbucketName\x18\x01 \x01(\t\x12Y\n\ncontainers\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ContainerLog\"\xa9\x01\n\x0bMLFramework\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFrameworkSpec\"\xa8\x01\n\x0fMLFrameworkList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFramework\"R\n\x0fMLFrameworkSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0c\n\x04lang\x18\x04 \x01(\t\"\x8c\x01\n\x0cMachineClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12;\n\x03mem\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12\x0c\n\x04vcpu\x18\x04 \x01(\x05\x12\x0f\n\x07storage\x18\x05 \x01(\t\"\xb9\x01\n\x10MachineClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xab\x01\n\x0cManagedImage\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImageSpec\"\xaa\x01\n\x10ManagedImageList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImage\"\xbb\x03\n\x10ManagedImageSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x10\n\x08registry\x18\x02 \x01(\t\x12\x12\n\nrepository\x18\x03 \x01(\t\x12\x0b\n\x03tag\x18\x04 \x01(\t\x12\'\n\x03\x65nv\x18\x05 \x03(\x0b\x32\x1a.k8s.io.api.core.v1.EnvVar\x12\x0b\n\x03gpu\x18\x06 \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\x07 \x01(\x08\x12\x0f\n\x07preload\x18\x08 \x01(\x08\x12:\n\rconnectionRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04\x62\x61se\x18\n \x01(\t\x12\x0c\n\x04role\x18\x0b \x01(\t\x12\x13\n\x0bmantainedBy\x18\x0c \x01(\t\x12\x0b\n\x03uri\x18\r \x01(\t\x12\x12\n\nframeworks\x18\x0e \x03(\t\x12J\n\x04libs\x18\x0f \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Lib\x12\n\n\x02os\x18\x10 \x01(\t\x12\x11\n\tosVersion\x18\x11 \x01(\t\x12\x0f\n\x07private\x18\x12 \x01(\x08\"\xf5\x01\n\x0bMeasurement\x12\x33\n\x06\x65ntity\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0e\n\x06metric\x18\x03 \x01(\t\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0e\n\x06stddev\x18\x05 \x01(\x01\x12\x0f\n\x07\x62oolQty\x18\x06 \x01(\x08\x12\x10\n\x08\x63\x61tegory\x18\x07 \x01(\t\x12\x10\n\x08valueSet\x18\x08 \x03(\t\x12=\n\ttimePoint\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xb3\x02\n\x13ModelDeploymentSpec\x12\x35\n\x08modelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x14\n\x0cmodelVersion\x18\x03 \x01(\t\x12\x0f\n\x07traffic\x18\x04 \x01(\x05\x12\x0c\n\x04role\x18\x05 \x01(\t\x12\x10\n\x08mountTar\x18\t \x01(\x08\x12\x17\n\x0ftrafficSelector\x18\n \x01(\t\x12\x37\n\napprovedBy\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\r \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xea\x01\n\x10NotificationSpec\x12\x10\n\x08\x65rrorTTL\x18\x02 \x01(\x05\x12\x12\n\nsuccessTTL\x18\x04 \x01(\x05\x12\x14\n\x0cnotifierName\x18\x05 \x01(\t\x12i\n\x08selector\x18\x06 \x03(\x0b\x32W.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec.SelectorEntry\x1a/\n\rSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"^\n\x07PRCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"m\n\x0fPermissionsSpec\x12Z\n\x0cstakeholders\x18\x01 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Stakeholder\"\xb1\x01\n\x0fPretrainedModel\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModelSpec\"\xb0\x01\n\x13PretrainedModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModel\"$\n\x13PretrainedModelSpec\x12\r\n\x05image\x18\x01 \x01(\t\"\xad\x01\n\rPublicDataset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDatasetSpec\"\xac\x01\n\x11PublicDatasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDataset\"\xb6\x02\n\x11PublicDatasetSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\x10\n\x08openMLID\x18\x04 \x01(\t\x12\x0f\n\x07\x64\x61taUrl\x18\x05 \x01(\t\x12\x10\n\x08\x63itation\x18\x06 \x01(\t\x12\x0c\n\x04rows\x18\x07 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x08 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\t \x01(\x05\x12\x14\n\x0ctargetColumn\x18\n \x01(\t\x12\x10\n\x08industry\x18\x0b \x01(\t\x12\x12\n\nimbalanced\x18\x0c \x01(\x08\x12\x14\n\x0c\x64\x61tasourceCR\x18\r \x01(\t\x12\x11\n\tdatasetCR\x18\x0e \x01(\t\x12\x0f\n\x07studyCR\x18\x0f \x01(\t\x12\x15\n\rdataProductCR\x18\x10 \x01(\t\"\xb6\x01\n\x06Region\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x1d\n\x15\x64\x65\x66\x61ultDatacenterName\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x13\n\x0b\x62illingCode\x18\x04 \x01(\t\x12X\n\x0b\x64\x61tacenters\x18\x05 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataCenter\"\xe2\x01\n\x0cResourceSpec\x12\x14\n\x0cworkloadName\x18\x01 \x01(\t\x12\x0e\n\x06\x63ustom\x18\x02 \x01(\x08\x12\x35\n\x08\x63puImage\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x35\n\x08gpuImage\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\x0crequirements\x18\x05 \x01(\x0b\x32(.k8s.io.api.core.v1.ResourceRequirements\"b\n\x0bRocAucCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\xb6\x01\n\x0bRunSchedule\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12=\n\tstartTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04\x63ron\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\"R\n\x0bStakeholder\x12\x0f\n\x07\x61\x63\x63ount\x18\x01 \x01(\t\x12\x32\n\x05roles\x18\x02 \x03(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"r\n\tTestSuite\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12T\n\x05tests\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCase\"\xc4\x02\n\x0fTestSuiteResult\x12\x36\n\tentityRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08\x66\x61ilures\x18\x02 \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x03 \x01(\x05\x12=\n\tstartTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12<\n\x08stopTime\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Z\n\x05tests\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCaseResult\"#\n\x06VizUri\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\"*\n\x0fWorkerRunResult\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0b\n\x03uri\x18\x02 \x01(\t\"\xad\x01\n\rWorkloadClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClassSpec\"\xac\x01\n\x11WorkloadClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClass\"u\n\x11WorkloadClassSpec\x12`\n\x11resourcesTemplate\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpecB9Z7github.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1')
 
 
 
 _ALGORITHM = DESCRIPTOR.message_types_by_name['Algorithm']
 _ALGORITHMLIST = DESCRIPTOR.message_types_by_name['AlgorithmList']
 _ALGORITHMSPEC = DESCRIPTOR.message_types_by_name['AlgorithmSpec']
 _CATEGORICALPARAMETER = DESCRIPTOR.message_types_by_name['CategoricalParameter']
@@ -73,14 +73,15 @@
 _RESOURCESPEC = DESCRIPTOR.message_types_by_name['ResourceSpec']
 _ROCAUCCURVE = DESCRIPTOR.message_types_by_name['RocAucCurve']
 _RUNSCHEDULE = DESCRIPTOR.message_types_by_name['RunSchedule']
 _STAKEHOLDER = DESCRIPTOR.message_types_by_name['Stakeholder']
 _TESTSUITE = DESCRIPTOR.message_types_by_name['TestSuite']
 _TESTSUITERESULT = DESCRIPTOR.message_types_by_name['TestSuiteResult']
 _VIZURI = DESCRIPTOR.message_types_by_name['VizUri']
+_WORKERRUNRESULT = DESCRIPTOR.message_types_by_name['WorkerRunResult']
 _WORKLOADCLASS = DESCRIPTOR.message_types_by_name['WorkloadClass']
 _WORKLOADCLASSLIST = DESCRIPTOR.message_types_by_name['WorkloadClassList']
 _WORKLOADCLASSSPEC = DESCRIPTOR.message_types_by_name['WorkloadClassSpec']
 Algorithm = _reflection.GeneratedProtocolMessageType('Algorithm', (_message.Message,), {
   'DESCRIPTOR' : _ALGORITHM,
   '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.generated_pb2'
   # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm)
@@ -455,14 +456,21 @@
 VizUri = _reflection.GeneratedProtocolMessageType('VizUri', (_message.Message,), {
   'DESCRIPTOR' : _VIZURI,
   '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.generated_pb2'
   # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.VizUri)
   })
 _sym_db.RegisterMessage(VizUri)
 
+WorkerRunResult = _reflection.GeneratedProtocolMessageType('WorkerRunResult', (_message.Message,), {
+  'DESCRIPTOR' : _WORKERRUNRESULT,
+  '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.generated_pb2'
+  # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult)
+  })
+_sym_db.RegisterMessage(WorkerRunResult)
+
 WorkloadClass = _reflection.GeneratedProtocolMessageType('WorkloadClass', (_message.Message,), {
   'DESCRIPTOR' : _WORKLOADCLASS,
   '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.generated_pb2'
   # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClass)
   })
 _sym_db.RegisterMessage(WorkloadClass)
 
@@ -590,14 +598,16 @@
   _STAKEHOLDER._serialized_end=8829
   _TESTSUITE._serialized_start=8831
   _TESTSUITE._serialized_end=8945
   _TESTSUITERESULT._serialized_start=8948
   _TESTSUITERESULT._serialized_end=9272
   _VIZURI._serialized_start=9274
   _VIZURI._serialized_end=9309
-  _WORKLOADCLASS._serialized_start=9312
-  _WORKLOADCLASS._serialized_end=9485
-  _WORKLOADCLASSLIST._serialized_start=9488
-  _WORKLOADCLASSLIST._serialized_end=9660
-  _WORKLOADCLASSSPEC._serialized_start=9662
-  _WORKLOADCLASSSPEC._serialized_end=9779
+  _WORKERRUNRESULT._serialized_start=9311
+  _WORKERRUNRESULT._serialized_end=9353
+  _WORKLOADCLASS._serialized_start=9356
+  _WORKLOADCLASS._serialized_end=9529
+  _WORKLOADCLASSLIST._serialized_start=9532
+  _WORKLOADCLASSLIST._serialized_end=9704
+  _WORKLOADCLASSSPEC._serialized_start=9706
+  _WORKLOADCLASSSPEC._serialized_end=9823
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_catalog_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nDgithub.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x12\x34github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x83\x01\n\x0f\x41ggregationSpec\x12\x13\n\x0bslidePeriod\x18\x01 \x01(\t\x12[\n\x0c\x61ggregations\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureAggrSpec\"W\n\x0c\x42\x61rChartSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\x12\x0e\n\x06legend\x18\x04 \x01(\x08\x12\x0c\n\x04sort\x18\x05 \x01(\x08\"\xa9\x07\n\x06\x43olumn\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x02 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x0e\n\x06ignore\x18\x06 \x01(\x08\x12\x0e\n\x06target\x18\x07 \x01(\x08\x12\x10\n\x08nullable\x18\x08 \x01(\x08\x12\n\n\x02pk\x18\t \x01(\x08\x12\n\n\x02\x66k\x18\n \x01(\x08\x12\x12\n\nmultipleOf\x18\x0b \x01(\x05\x12\x0f\n\x07maximum\x18\x0c \x01(\x01\x12\x18\n\x10\x65xclusiveMaximum\x18\r \x01(\x08\x12\x0f\n\x07minimum\x18\x0e \x01(\x01\x12\x18\n\x10\x65xclusiveMinimum\x18\x0f \x01(\x08\x12\x11\n\tmaxLength\x18\x10 \x01(\x05\x12\x11\n\tminLength\x18\x11 \x01(\x05\x12\x0f\n\x07pattern\x18\x12 \x01(\t\x12\x10\n\x08required\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xample\x18\x14 \x01(\t\x12\x14\n\x0c\x65xternalDocs\x18\x15 \x01(\t\x12\x0c\n\x04\x65num\x18\x16 \x03(\t\x12\x0f\n\x07ordinal\x18\x17 \x01(\x08\x12\x10\n\x08maxItems\x18\x18 \x01(\x05\x12\x10\n\x08minItems\x18\x19 \x01(\x05\x12\x13\n\x0buniqueItems\x18\x1a \x01(\x08\x12\x0b\n\x03pii\x18\x1c \x01(\x08\x12\x0b\n\x03phi\x18\x1d \x01(\x08\x12\x14\n\x0cpersonalData\x18\x1e \x01(\x08\x12\x11\n\tprotected\x18\x1f \x01(\x08\x12\x17\n\x0f\x64\x65\x66\x61ultValueNum\x18  \x01(\x01\x12\x0b\n\x03log\x18! \x01(\x08\x12\n\n\x02mu\x18\" \x01(\x01\x12\r\n\x05sigma\x18# \x01(\x01\x12\x15\n\rskewThreshold\x18$ \x01(\x01\x12\x16\n\x0e\x64riftThreshold\x18% \x01(\x01\x12\x0b\n\x03key\x18& \x01(\x08\x12\x0c\n\x04\x66old\x18\' \x01(\x08\x12\x0e\n\x06weight\x18( \x01(\x08\x12\x10\n\x08reserved\x18) \x01(\x08\x12\x12\n\nimputation\x18* \x01(\t\x12\x0f\n\x07scaling\x18+ \x01(\t\x12\x11\n\tgenerated\x18, \x01(\x08\x12\x0f\n\x07\x66ormula\x18- \x01(\t\x12\n\n\x02id\x18. \x01(\x08\x12\x0c\n\x04step\x18/ \x01(\x01\x12\x0b\n\x03loc\x18\x30 \x01(\x05\x12\x16\n\x0e\x64\x61tetimeFormat\x18\x31 \x01(\t\x12\x12\n\ntimeseries\x18\x32 \x01(\x08\x12\x11\n\tregressor\x18\x33 \x01(\x08\x12\x17\n\x0flaggedRegressor\x18\x34 \x01(\x08\x12\x11\n\ttimeIndex\x18\x35 \x01(\x08\"\xe0\x01\n\x0f\x43olumnHistogram\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Y\n\thistogram\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.HistogramData\x12U\n\x07metrics\x18\x03 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05\x64rift\x18\x04 \x01(\x08\"\x81\x01\n\nColumnSpec\x12\x0e\n\x06spacer\x18\x01 \x01(\x08\x12\r\n\x05width\x18\x02 \x01(\x05\x12T\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ComponentSpec\"\xae\x07\n\x10\x43olumnStatistics\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x01\x12\x10\n\x08\x64istinct\x18\x04 \x01(\x05\x12\x0f\n\x07missing\x18\x05 \x01(\x05\x12\x16\n\x0epercentMissing\x18\x06 \x01(\x01\x12\x0c\n\x04mean\x18\x07 \x01(\x01\x12\x0e\n\x06stddev\x18\x08 \x01(\x01\x12\x10\n\x08variance\x18\t \x01(\x01\x12\x0b\n\x03min\x18\n \x01(\x01\x12\x0b\n\x03max\x18\x0b \x01(\x01\x12\x10\n\x08kurtosis\x18\x0c \x01(\x01\x12\x10\n\x08skewness\x18\r \x01(\x01\x12\x0b\n\x03sum\x18\x0e \x01(\x01\x12\x0b\n\x03mad\x18\x0f \x01(\x01\x12\x0b\n\x03p25\x18\x10 \x01(\x01\x12\x0b\n\x03p50\x18\x11 \x01(\x01\x12\x0b\n\x03p75\x18\x12 \x01(\x01\x12\x0b\n\x03iqr\x18\x13 \x01(\x01\x12\x0c\n\x04mode\x18\x14 \x01(\t\x12\r\n\x05zeros\x18\x15 \x01(\x01\x12\x0f\n\x07invalid\x18\x16 \x01(\x05\x12\x12\n\nimportance\x18\x17 \x01(\x01\x12\x0e\n\x06target\x18\x18 \x01(\x08\x12\x0e\n\x06ignore\x18\x19 \x01(\x08\x12\x10\n\x08nullable\x18\x1a \x01(\x08\x12\x17\n\x0fhighCardinality\x18\x1b \x01(\x08\x12!\n\x19highCorrWithOtherFeatures\x18\x1c \x01(\x08\x12\x19\n\x11lowCorrWithTarget\x18\x1d \x01(\x08\x12\x16\n\x0ehighMissingPct\x18\x1e \x01(\x08\x12\x0e\n\x06skewed\x18\x1f \x01(\x08\x12\n\n\x02id\x18  \x01(\x08\x12\x10\n\x08\x63onstant\x18! \x01(\x08\x12\x11\n\tduplicate\x18\" \x01(\x08\x12\x10\n\x08reserved\x18# \x01(\x08\x12\x14\n\x0c\x63ompleteness\x18% \x01(\x01\x12\x1a\n\x12\x64istinctValueCount\x18& \x01(\x01\x12\x1b\n\x13mostFreqValuesRatio\x18\' \x01(\x01\x12\x1a\n\x12indexOfPeculiarity\x18( \x01(\x01\x12Y\n\thistogram\x18) \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.HistogramData\x12\x14\n\x0c\x63orrToTarget\x18* \x01(\x01\x12\r\n\x05index\x18+ \x01(\x05\x12S\n\x08outliers\x18, \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.OutlierStat\"\x96\x01\n\rComponentSpec\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x0e\n\x06\x66ooter\x18\x03 \x01(\t\x12T\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ComponentView\"\xe3\x04\n\rComponentView\x12P\n\x06metric\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.MetricSpec\x12N\n\x05gauge\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GaugeSpec\x12V\n\thistogram\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.HistogramSpec\x12N\n\x05table\x18\x04 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.TableSpec\x12V\n\tlineChart\x18\x05 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LineChartSpec\x12T\n\x08\x62\x61rChart\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.BarChartSpec\x12Z\n\x0bscatterPlot\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ScatterPlotSpec\"P\n\x0b\x43orrelation\x12\x10\n\x08\x66\x65\x61ture1\x18\x01 \x01(\t\x12\x10\n\x08\x66\x65\x61ture2\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\x12\x0e\n\x06method\x18\x04 \x01(\t\">\n\x0f\x43orrelationSpec\x12\x0e\n\x06\x63utoff\x18\x01 \x01(\x01\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0b\n\x03top\x18\x03 \x01(\x05\"\x8b\x02\n\x0b\x43svFileSpec\x12\x17\n\x0f\x63olumnDelimiter\x18\x01 \x01(\t\x12\x14\n\x0crowDelimiter\x18\x02 \x01(\t\x12\r\n\x05quote\x18\x03 \x01(\t\x12\x12\n\nescapeChar\x18\x04 \x01(\t\x12\x14\n\x0c\x63ommentChars\x18\x05 \x01(\t\x12\x0e\n\x06header\x18\x06 \x01(\x08\x12\x10\n\x08skipRows\x18\x07 \x01(\x05\x12\x12\n\nnullValues\x18\x08 \x01(\t\x12\x10\n\x08\x65ncoding\x18\t \x01(\t\x12\x0f\n\x07maxRows\x18\n \x01(\x05\x12\x0e\n\x06strict\x18\x0b \x01(\x08\x12\x13\n\x0b\x63ompression\x18\x0c \x01(\t\x12\x16\n\x0ehasIndexColumn\x18\r \x01(\x08\"u\n\rDataInputSpec\x12T\n\x08location\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\"\xda\x01\n\x0c\x44\x61taLocation\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x12\n\nbucketName\x18\x03 \x01(\t\x12\x0c\n\x04path\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x06 \x01(\t\x12\x0b\n\x03sql\x18\x07 \x01(\t\x12\r\n\x05topic\x18\x08 \x01(\t\x12\x0b\n\x03url\x18\t \x01(\t\x12\x38\n\x0bresourceRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xf8\x01\n\x0e\x44\x61taOutputSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12T\n\x08location\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\x12\x1d\n\x15\x63reateTableIfNotExist\x18\x05 \x01(\x08\x12\x17\n\x0fincludeFeatures\x18\x06 \x01(\x08\x12\x0b\n\x03xai\x18\x07 \x01(\x08\x12\x16\n\x0e\x64\x65tectOutliers\x18\x08 \x01(\x08\"\x82\x02\n\x0c\x44\x61taPipeline\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineStatus\"\x9e\x01\n\x15\x44\x61taPipelineCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xa7\x01\n\x10\x44\x61taPipelineList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"\x8b\x02\n\x0f\x44\x61taPipelineRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunStatus\"\xa1\x01\n\x18\x44\x61taPipelineRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xad\x01\n\x13\x44\x61taPipelineRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRun\"\x95\x02\n\x13\x44\x61taPipelineRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x18\n\x10\x64\x61tapipelineName\x18\x02 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xd9\x04\n\x15\x44\x61taPipelineRunStatus\x12\x12\n\nrecipeRuns\x18\x01 \x03(\t\x12R\n\x06output\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\r\n\x05phase\x18\x03 \x01(\t\x12=\n\tstartTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x06 \x01(\x03\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x10\n\x08progress\x18\t \x01(\x05\x12K\n\x04logs\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12?\n\x0blastUpdated\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x62\n\nconditions\x18\x0c \x03(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunCondition\"\xe8\x05\n\x10\x44\x61taPipelineSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12t\n\x0f\x64\x61tasetSelector\x18\x03 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineSpec.DatasetSelectorEntry\x12U\n\x07recipes\x18\x04 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipePartSpec\x12T\n\x06output\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12V\n\x08schedule\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12_\n\x0cnotification\x18\x07 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\x08 \x01(\t\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\n \x01(\t\x12\x0e\n\x06paused\x18\x0b \x01(\x08\x12\x0b\n\x03ttl\x18\x0c \x01(\x05\x1a\x36\n\x14\x44\x61tasetSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe8\x02\n\x12\x44\x61taPipelineStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12?\n\x0blastUpdated\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12W\n\x07lastRun\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12_\n\nconditions\x18\x05 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineCondition\"\xff\x01\n\x0b\x44\x61taProduct\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductStatus\"\x9d\x01\n\x14\x44\x61taProductCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xa5\x01\n\x0f\x44\x61taProductList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\"\xc4\t\n\x0f\x44\x61taProductSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x0e\n\x06public\x18\x02 \x01(\x08\x12\x36\n\ttenantRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12V\n\x0bgitLocation\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GitLocation\x12Z\n\rimageLocation\x18\x05 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ImageLocation\x12\x0f\n\x07labName\x18\x07 \x01(\t\x12\x17\n\x0fservingSiteName\x18\x08 \x01(\t\x12\x0c\n\x04task\x18\t \x01(\t\x12\x0f\n\x07subtask\x18\n \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12X\n\x0c\x64\x61taLocation\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12_\n\x0cnotification\x18\r \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12`\n\x11trainingResources\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12_\n\x10servingResources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x18\n\x10retriesOnFailure\x18\x10 \x01(\x05\x12G\n\x04kpis\x18\x11 \x03(\x0b\x32\x39.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.KPI\x12\x19\n\x11onCallAccountName\x18\x12 \x01(\t\x12Z\n\x0b\x63ompilation\x18\x13 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CompilerSpec\x12\x16\n\x0e\x63learanceLevel\x18\x14 \x01(\t\x12\x10\n\x08priority\x18\x15 \x01(\t\x12\r\n\x05\x63olor\x18\x16 \x01(\t\x12X\n\ngovernance\x18\x17 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GovernanceSpec\x12]\n\x0bpermissions\x18\x18 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PermissionsSpec\"\xfc\x04\n\x11\x44\x61taProductStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12?\n\x0blastUpdated\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x18\n\x10totalDatasources\x18\x03 \x01(\x05\x12\x15\n\rtotalDatasets\x18\x04 \x01(\x05\x12\x1a\n\x12totalDataPipelines\x18\x05 \x01(\x05\x12\x1d\n\x15totalDataPipelineRuns\x18\x06 \x01(\x05\x12\x14\n\x0ctotalStudies\x18\x07 \x01(\x05\x12\x13\n\x0btotalModels\x18\x08 \x01(\x05\x12\x1b\n\x13totalModelPipelines\x18\t \x01(\x05\x12\x1e\n\x16totalModelPipelineRuns\x18\n \x01(\x05\x12\x17\n\x0ftotalPredictors\x18\x0b \x01(\x05\x12\x15\n\rtotalBuilders\x18\x0c \x01(\x05\x12\x11\n\ttotalApps\x18\r \x01(\x05\x12\x18\n\x10totalPredictions\x18\x0e \x01(\x05\x12\x17\n\x0ftotalInfoAlerts\x18\x0f \x01(\x05\x12\x18\n\x10totalErrorAlerts\x18\x10 \x01(\x05\x12\x15\n\rfailureReason\x18\x11 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x12 \x01(\t\x12\x17\n\x0f\x62\x61selineVersion\x18\x13 \x01(\t\x12^\n\nconditions\x18\x14 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductCondition\"\x94\x02\n\x12\x44\x61taProductVersion\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionSpec\x12^\n\x06status\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionStatus\"\xa4\x01\n\x1b\x44\x61taProductVersionCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xb3\x01\n\x16\x44\x61taProductVersionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\"\xa0\x01\n\x16\x44\x61taProductVersionSpec\x12\x37\n\nproductRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x17\n\x0fprevVersionName\x18\x03 \x01(\t\x12\x10\n\x08\x62\x61seline\x18\x04 \x01(\x08\x12\r\n\x05owner\x18\x05 \x01(\t\"\x8d\x02\n\x18\x44\x61taProductVersionStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12?\n\x0blastUpdated\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x65\n\nconditions\x18\x05 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionCondition\"\xfc\x01\n\nDataSource\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceStatus\"\x9c\x01\n\x13\x44\x61taSourceCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xa3\x01\n\x0e\x44\x61taSourceList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\"\xf8\x05\n\x0e\x44\x61taSourceSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x61tasetType\x18\x04 \x01(\t\x12L\n\x06schema\x18\x05 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latfile\x18\x06 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x0f\n\x07labeled\x18\x07 \x01(\x08\x12P\n\x06sample\x18\t \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12\x0c\n\x04task\x18\n \x01(\t\x12\x0f\n\x07subtask\x18\x0b \x01(\t\x12]\n\rrelationships\x18\x0c \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RelationshipSpec\x12T\n\x08labeling\x18\r \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingSpec\x12X\n\x0cinferredFrom\x18\x0e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12]\n\x11unitTestsTemplate\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\xec\x02\n\x10\x44\x61taSourceStatus\x12\x0c\n\x04\x63ols\x18\x01 \x01(\x05\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12\x46\n\x12lastDatasetCreated\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0flastDatasetName\x18\x04 \x01(\t\x12?\n\x0blastUpdated\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x06 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12]\n\nconditions\x18\x08 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceCondition\"\xf3\x01\n\x07\x44\x61taset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSpec\x12S\n\x06status\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetStatus\"\x99\x01\n\x10\x44\x61tasetCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xab\x02\n\x14\x44\x61tasetGroupByStatus\x12\x13\n\x0b\x64\x61tasetsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x12\n\nreportsURI\x18\x03 \x01(\t\x12\x14\n\x0cunitTestsURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66\x65\x61turesURI\x18\x05 \x01(\t\x12t\n\rworkerResults\x18\x06 \x03(\x0b\x32].github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetGroupByStatus.WorkerResultsEntry\x1a\x34\n\x12WorkerResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9d\x01\n\x0b\x44\x61tasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12L\n\x05items\x18\x02 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x9f\n\n\x0b\x44\x61tasetSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0e\x64\x61tasourceName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x05 \x01(\t\x12\x0c\n\x04role\x18\x06 \x01(\t\x12\x10\n\x08reported\x18\x07 \x01(\x08\x12\x13\n\x0bsnapshotted\x18\x08 \x01(\x08\x12\x12\n\nunitTested\x18\t \x01(\x08\x12R\n\x06origin\x18\r \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12T\n\x08location\x18\x0e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12X\n\tresources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x10 \x01(\x03\x12\x0c\n\x04type\x18\x11 \x01(\t\x12P\n\x06sample\x18\x12 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12V\n\tsyntactic\x18\x13 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SyntheticSpec\x12\x0c\n\x04task\x18\x14 \x01(\t\x12\x0f\n\x07subtask\x18\x15 \x01(\t\x12_\n\x0cnotification\x18\x16 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12Z\n\x0b\x63orrelation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.CorrelationSpec\x12\x0c\n\x04\x66\x61st\x18\x18 \x01(\x08\x12\x12\n\nfeaturized\x18\x19 \x01(\x08\x12\x33\n\x06labRef\x18\x1a \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\x11servingDatasetRef\x18\x1b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cpredictorRef\x18\x1c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12 \n\x18generateFeatureHistogram\x18\x1d \x01(\x08\x12U\n\tunitTests\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12R\n\x07groupBy\x18\x1f \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GroupBySpec\x12\x0b\n\x03key\x18  \x03(\t\"\xd9\x02\n\x11\x44\x61tasetStatistics\x12W\n\x07\x63olumns\x18\x01 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnStatistics\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0c\n\x04\x63ols\x18\x04 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\x05 \x01(\x05\x12\x61\n\x16\x63orrelationsWithTarget\x18\x06 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18\x07 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\"\xe3\x08\n\rDatasetStatus\x12[\n\nstatistics\x18\x01 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetStatistics\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x12\n\nreportName\x18\x03 \x01(\t\x12\x11\n\treportUri\x18\x04 \x01(\t\x12\x12\n\nprofileUri\x18\x05 \x01(\t\x12\x12\n\nimbalanced\x18\x06 \x01(\x08\x12\x14\n\x0c\x61nomaliesUri\x18\x07 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x08 \x01(\x03\x12\x61\n\x0funitTestResults\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x41\n\rlastStudyTime\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\r \x01(\t\x12\x10\n\x08progress\x18\x0e \x01(\x05\x12\x0c\n\x04hash\x18\x0f \x01(\t\x12K\n\x04logs\x18\x10 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x1a\n\x12\x64\x65rivedFromDataset\x18\x11 \x01(\t\x12?\n\x0blastUpdated\x18\x12 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12O\n\x06images\x18\x13 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12=\n\tstartTime\x18\x14 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x15 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12@\n\x13\x66\x65\x61tureHistogramRef\x18\x16 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12[\n\x07groupby\x18\x17 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetGroupByStatus\x12Z\n\nconditions\x18\x18 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetCondition\"\xa6\x01\n\x0f\x44\x61tasetTemplate\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSpec\"/\n\x0e\x44riftThreshold\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"\xf0\x01\n\x06\x45ntity\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntitySpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntityStatus\"\x98\x01\n\x0f\x45ntityCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\x9b\x01\n\nEntityList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\"S\n\nEntitySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04keys\x18\x03 \x03(\t\x12\r\n\x05owner\x18\x04 \x01(\t\"\xc6\x01\n\x0c\x45ntityStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12?\n\x0blastUpdated\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Y\n\nconditions\x18\x03 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntityCondition\"\xc1\x01\n\x11\x45xcelNotebookSpec\x12\x1a\n\x12\x66irstSheetWithData\x18\x01 \x01(\x08\x12\x11\n\tsheetName\x18\x02 \x01(\t\x12\x12\n\nsheetIndex\x18\x03 \x01(\x05\x12\x15\n\rcolumnNameRow\x18\x04 \x01(\x05\x12R\n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ExcelSheetArea\"k\n\x0e\x45xcelSheetArea\x12\x13\n\x0b\x65ntireSheet\x18\x01 \x01(\x08\x12\x12\n\nfromColumn\x18\x02 \x01(\x05\x12\x10\n\x08toColumn\x18\x03 \x01(\x05\x12\x0f\n\x07\x66romRow\x18\x04 \x01(\x05\x12\r\n\x05toRow\x18\x05 \x01(\x05\"\xf3\x01\n\x07\x46\x65\x61ture\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureSpec\x12S\n\x06status\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureStatus\"E\n\x0f\x46\x65\x61tureAggrSpec\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x11\n\tfunctions\x18\x02 \x03(\t\x12\x0f\n\x07windows\x18\x03 \x03(\t\"\x99\x01\n\x10\x46\x65\x61tureCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\x8e\x02\n\x10\x46\x65\x61tureHistogram\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramSpec\x12\\\n\x06status\x18\x03 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramStatus\"\xa2\x01\n\x19\x46\x65\x61tureHistogramCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xaf\x01\n\x14\x46\x65\x61tureHistogramList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\"\xf5\x04\n\x14\x46\x65\x61tureHistogramSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x05 \x03(\t\x12\x36\n\tsourceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08training\x18\x07 \x01(\x08\x12\x0c\n\x04live\x18\t \x01(\x08\x12\x39\n\x05start\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x37\n\x03\x65nd\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x34\n\x07\x62\x61seRef\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12]\n\x0f\x64riftThresholds\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12\x17\n\x0fsyncIntervalSec\x18\x0e \x01(\x05\x12U\n\tunitTests\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x14\n\x0cgenUnitTests\x18\x10 \x01(\x08\x12\x15\n\rfeatureFilter\x18\x11 \x01(\t\x12\x15\n\rreferenceType\x18\x12 \x01(\t\"\xbf\x04\n\x16\x46\x65\x61tureHistogramStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12V\n\x07\x63olumns\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnHistogram\x12?\n\x0blastUpdated\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05total\x18\n \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x0b \x01(\x05\x12\x63\n\nconditions\x18\x0c \x03(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramCondition\"\x9d\x01\n\x0b\x46\x65\x61tureList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12L\n\x05items\x18\x02 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Feature\"\x8b\x02\n\x0f\x46\x65\x61turePipeline\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineStatus\"\xa1\x01\n\x18\x46\x65\x61turePipelineCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xad\x01\n\x13\x46\x65\x61turePipelineList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipeline\"\x94\x02\n\x12\x46\x65\x61turePipelineRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineRunSpec\x12^\n\x06status\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineRunStatus\"\xa4\x01\n\x1b\x46\x65\x61turePipelineRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xb3\x01\n\x16\x46\x65\x61turePipelineRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineRun\"\xc0\x01\n\x16\x46\x65\x61turePipelineRunSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x1b\n\x13\x66\x65\x61turePipelineName\x18\x03 \x01(\t\x12X\n\tresources\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03ttl\x18\x05 \x01(\x05\"\xfa\x03\n\x18\x46\x65\x61turePipelineRunStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x03 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x13\n\x0btriggeredBy\x18\x05 \x01(\t\x12K\n\x04logs\x18\x06 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12?\n\x0blastUpdated\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x08 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\t \x01(\t\x12\x65\n\nconditions\x18\n \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineRunCondition\"\xd1\x05\n\x13\x46\x65\x61turePipelineSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12w\n\x0f\x64\x61tasetSelector\x18\x02 \x03(\x0b\x32^.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineSpec.DatasetSelectorEntry\x12\x13\n\x0bversionName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12Z\n\x0b\x61ggregation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.AggregationSpec\x12\x62\n\x0fmaterialization\x18\x06 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.MaterializationSpec\x12\x0e\n\x06\x66\x61mily\x18\x07 \x01(\t\x12\x12\n\nentityName\x18\x08 \x01(\t\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12V\n\x08schedule\x18\n \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x0b \x01(\x03\x12\x0e\n\x06paused\x18\x0c \x01(\x08\x12\x0b\n\x03ttl\x18\r \x01(\x05\x1a\x36\n\x14\x44\x61tasetSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x03\n\x15\x46\x65\x61turePipelineStatus\x12W\n\x07lastRun\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0b\x61verageCost\x18\x03 \x01(\x01\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12?\n\x0blastUpdated\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x62\n\nconditions\x18\x06 \x03(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineCondition\"\xba\x01\n\x0b\x46\x65\x61tureSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x11\n\tkeyColumn\x18\x05 \x01(\t\x12\x17\n\x0ftimestampColumn\x18\x06 \x01(\t\x12\x15\n\rfeatureColumn\x18\x07 \x01(\t\x12\x12\n\nentityName\x18\x08 \x01(\t\x12\x1b\n\x13\x66\x65\x61turePipelineName\x18\t \x01(\t\"\xf1\x04\n\rFeatureStatus\x12\x0b\n\x03min\x18\x02 \x01(\x01\x12\x0b\n\x03max\x18\x03 \x01(\x01\x12\x0c\n\x04mean\x18\x04 \x01(\x01\x12\x0e\n\x06stddev\x18\x05 \x01(\x01\x12\x10\n\x08skewness\x18\x06 \x01(\x01\x12\x10\n\x08kurtosis\x18\x07 \x01(\x01\x12\r\n\x05zeros\x18\x08 \x01(\x01\x12\x0b\n\x03p25\x18\n \x01(\x01\x12\x0b\n\x03p50\x18\x0b \x01(\x01\x12\x0b\n\x03p75\x18\x0c \x01(\x01\x12\x0f\n\x07missing\x18\x0e \x01(\x05\x12\x0f\n\x07invalid\x18\x0f \x01(\x05\x12\x0e\n\x06target\x18\x10 \x01(\x08\x12\x12\n\nimportance\x18\x11 \x01(\x01\x12\x0f\n\x07\x64istinc\x18\x12 \x01(\x05\x12\x0f\n\x07ignored\x18\x13 \x01(\x08\x12\x10\n\x08nullable\x18\x14 \x01(\x08\x12\x10\n\x08highCred\x18\x15 \x01(\x08\x12\x10\n\x08highCorr\x18\x16 \x01(\x08\x12\x0c\n\x04skew\x18\x17 \x01(\x08\x12\x14\n\x0c\x63ompleteness\x18\x18 \x01(\x01\x12\x1a\n\x12\x64istinctValueCount\x18\x19 \x01(\x01\x12\x1b\n\x13mostFreqValuesRatio\x18\x1a \x01(\x01\x12\x1a\n\x12indexOfPeculiarity\x18\x1b \x01(\x01\x12\x1a\n\x12observedGeneration\x18\x1c \x01(\x03\x12?\n\x0blastUpdated\x18\x1d \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Z\n\nconditions\x18\x1e \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureCondition\"\xfc\x01\n\nFeatureset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturesetSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturesetStatus\"\x9c\x01\n\x13\x46\x65\x61turesetCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xa3\x01\n\x0e\x46\x65\x61turesetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Featureset\"[\n\x0e\x46\x65\x61turesetSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x10\n\x08\x66\x65\x61tures\x18\x03 \x03(\t\x12\r\n\x05owner\x18\x04 \x01(\t\"\xce\x01\n\x10\x46\x65\x61turesetStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12?\n\x0blastUpdated\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12]\n\nconditions\x18\x03 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturesetCondition\"\xa6\x02\n\x12\x46latFileFormatSpec\x12\x10\n\x08\x66ileType\x18\x01 \x01(\t\x12N\n\x03\x63sv\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.CsvFileSpec\x12V\n\x05\x65xcel\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ExcelNotebookSpec\x12V\n\x07parquet\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ParquetFileSpec\"M\n\tGaugeSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0b\n\x03row\x18\x03 \x01(\x05\x12\x0e\n\x06scalar\x18\x04 \x01(\t\"V\n\x0bGitLocation\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x0f\n\x07private\x18\x04 \x01(\x08\"y\n\x16GovernanceReviewStatus\x12\x0e\n\x06result\x18\x01 \x01(\t\x12@\n\x0c\x61pprovalDate\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05notes\x18\x03 \x01(\t\"\x8d\x01\n\x0eGovernanceSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x02 \x01(\t\x12\x12\n\nitReviewer\x18\x03 \x01(\t\x12\x1a\n\x12\x63omplianceReviewer\x18\x04 \x01(\t\x12\x18\n\x10\x62usinessReviewer\x18\x05 \x01(\t\x12\x0f\n\x07members\x18\x06 \x03(\t\"\xd2\x02\n\x10GovernanceStatus\x12\x64\n\x0eITReviewStatus\x18\x01 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GovernanceReviewStatus\x12l\n\x16\x63omplianceReviewStatus\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GovernanceReviewStatus\x12j\n\x14\x62usinessReviewStatus\x18\x03 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GovernanceReviewStatus\"]\n\x0bGroupBySpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07groupby\x18\x02 \x03(\t\x12\x0c\n\x04\x66req\x18\x03 \x01(\t\x12\x10\n\x08interval\x18\x04 \x01(\x05\x12\x0c\n\x04\x61ggr\x18\x05 \x01(\t\"=\n\rHistogramSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\x0c\n\x04\x62ins\x18\x03 \x01(\x05\"=\n\rImageLocation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\x16registryConnectionName\x18\x02 \x01(\t\"\"\n\x03KPI\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"\x8e\x02\n\x10LabelingPipeline\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineSpec\x12\\\n\x06status\x18\x03 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineStatus\"\xa2\x01\n\x19LabelingPipelineCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xaf\x01\n\x14LabelingPipelineList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipeline\"\x97\x02\n\x13LabelingPipelineRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12[\n\x04spec\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineRunSpec\x12_\n\x06status\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineRunStatus\"\xa5\x01\n\x1cLabelingPipelineRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xb5\x01\n\x17LabelingPipelineRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12X\n\x05items\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineRun\"\xbf\x01\n\x17LabelingPipelineRunSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x19\n\x11labelPipelineName\x18\x03 \x01(\t\x12X\n\tresources\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03ttl\x18\x05 \x01(\x05\"\xaf\x03\n\x19LabelingPipelineRunStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x13\n\x0btriggeredBy\x18\x05 \x01(\t\x12?\n\x0blastUpdated\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x66\n\nconditions\x18\t \x03(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineRunCondition\"\x9c\x04\n\x14LabelingPipelineSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12x\n\x0f\x64\x61tasetSelector\x18\x03 \x03(\x0b\x32_.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineSpec.DatasetSelectorEntry\x12\x13\n\x0brecipeNames\x18\x04 \x03(\t\x12\x16\n\x0eoutputLabelset\x18\x05 \x01(\t\x12V\n\x08schedule\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\r\n\x05owner\x18\x07 \x01(\t\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\t \x01(\x03\x12\x0e\n\x06paused\x18\n \x01(\x08\x12\x0b\n\x03ttl\x18\x0b \x01(\x05\x1a\x36\n\x14\x44\x61tasetSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xf0\x02\n\x16LabelingPipelineStatus\x12W\n\x07lastRun\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12?\n\x0blastUpdated\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x63\n\nconditions\x18\x05 \x03(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineCondition\"?\n\x0cLabelingRule\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x10\n\x08operator\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xe1\x01\n\x0cLabelingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x14\n\x0cresultColumn\x18\x02 \x01(\t\x12T\n\x08positive\x18\x03 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingRule\x12T\n\x08negative\x18\x04 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingRule\"J\n\rLineChartSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\x12\x0e\n\x06legend\x18\x04 \x01(\x08\"\xae\x01\n\x13MaterializationSpec\x12\x0e\n\x06online\x18\x01 \x01(\x08\x12\x0f\n\x07offline\x18\x02 \x01(\x08\x12=\n\tstartDate\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x18\n\x10scheduleInterval\x18\x04 \x01(\t\x12\x0b\n\x03ttl\x18\x05 \x01(\x05\x12\x10\n\x08\x62\x61\x63kfill\x18\x06 \x01(\x05\"N\n\nMetricSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0b\n\x03row\x18\x03 \x01(\x05\x12\x0e\n\x06scalar\x18\x04 \x01(\t\"<\n\x0bOutlierStat\x12\r\n\x05lower\x18\x01 \x01(\x05\x12\r\n\x05upper\x18\x02 \x01(\x05\x12\x0f\n\x07percent\x18\x03 \x01(\x02\"W\n\x08PageSpec\x12K\n\x04rows\x18\x01 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RowSpec\"!\n\x0fParquetFileSpec\x12\x0e\n\x06\x65ngine\x18\x01 \x01(\t\"\xf0\x01\n\x06Recipe\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeSpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStatus\"\x98\x01\n\x0fRecipeCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\x8c\x01\n\x0fRecipeInputSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12T\n\x08location\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\"\x9b\x01\n\nRecipeList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x94\x01\n\x10RecipeOutputSpec\x12\x15\n\rcreateDataset\x18\x01 \x01(\x08\x12\x13\n\x0b\x64\x61tasetName\x18\x02 \x01(\t\x12T\n\x08location\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\"8\n\x0eRecipePartSpec\x12\x12\n\nrecipeName\x18\x01 \x01(\t\x12\x12\n\ndependents\x18\x02 \x03(\t\"\xf9\x01\n\tRecipeRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRunSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRunStatus\"\x9b\x01\n\x12RecipeRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xa1\x01\n\rRecipeRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\"\xa8\x02\n\rRecipeRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x12\n\nrecipeName\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12R\n\x06output\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03ttl\x18\x06 \x01(\x05\"\xc8\x04\n\x0fRecipeRunStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x03 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x13\n\x0btriggeredBy\x18\x07 \x01(\t\x12K\n\x04logs\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12?\n\x0blastUpdated\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\n \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12Y\n\nconditions\x18\x0b \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeCondition\"\xfb\x04\n\nRecipeSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12T\n\x05input\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeInputSpec\x12O\n\x05steps\x18\x05 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStep\x12V\n\x06output\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeOutputSpec\x12P\n\x06sample\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\n \x01(\x03\x12\x0b\n\x03ttl\x18\x0b \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\xdc\x02\n\x0cRecipeStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12W\n\x07lastRun\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0blastUpdated\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Y\n\nconditions\x18\x07 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeCondition\"s\n\nRecipeStep\x12\n\n\x02op\x18\x01 \x01(\t\x12Y\n\nparameters\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStepParam\".\n\x0fRecipeStepParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"X\n\x14RecommendationSchema\x12\x14\n\x0cuserIDColumn\x18\x01 \x01(\t\x12\x14\n\x0citemIDColumn\x18\x02 \x01(\t\x12\x14\n\x0cratingColumn\x18\x03 \x01(\t\"R\n\x10RelationshipSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\r\n\x05\x61rity\x18\x03 \x01(\t\x12\x11\n\trelatesTo\x18\x04 \x01(\t\"Y\n\x07RowSpec\x12N\n\x04\x63ols\x18\x01 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnSpec\"j\n\nSampleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0f\n\x07percent\x18\x04 \x01(\x05\x12\x0e\n\x06\x66ilter\x18\x05 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\"<\n\x0fScatterPlotSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\"\xb0\x02\n\x06Schema\x12`\n\x10timeSeriesSchema\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.TimeSeriesSchema\x12h\n\x14recommendationSchema\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecommendationSchema\x12M\n\x07\x63olumns\x18\x03 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Column\x12\x0b\n\x03key\x18\x04 \x03(\t\"\xf6\x01\n\x08SqlQuery\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQuerySpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryStatus\"\x9a\x01\n\x11SqlQueryCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\x9f\x01\n\x0cSqlQueryList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQuery\"\xff\x01\n\x0bSqlQueryRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryRunSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryRunStatus\"\x9d\x01\n\x14SqlQueryRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xa5\x01\n\x0fSqlQueryRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryRun\"\xfd\x03\n\x0fSqlQueryRunSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\x08\x12\x12\n\nsqlOrTable\x18\x06 \x01(\t\x12\x16\n\x0e\x63onnectionName\x18\x07 \x01(\t\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\t \x01(\x03\x12\x10\n\x08priority\x18\n \x01(\t\x12\x0f\n\x07\x61\x62orted\x18\x0b \x01(\x08\x12\x14\n\x0cmaterialized\x18\x0c \x01(\x08\x12\x10\n\x08reported\x18\r \x01(\x08\x12\x14\n\x0csqlQueryName\x18\x0e \x01(\t\x12\x33\n\x06labRef\x18\x0f \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x10 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\xc7\x05\n\x11SqlQueryRunStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x03 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x13\n\x0btriggeredBy\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12T\n\x08location\x18\t \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x12\n\nreportName\x18\n \x01(\t\x12?\n\x0blastUpdated\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\r \x01(\t\x12\x61\n\x0funitTestsResult\x18\x10 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12^\n\nconditions\x18\x0e \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryRunCondition\"\xf8\x01\n\x0cSqlQuerySpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12W\n\x08template\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryRunSpec\x12V\n\x08schedule\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"\xe0\x02\n\x0eSqlQueryStatus\x12?\n\x0blastUpdated\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12W\n\x07lastRun\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12[\n\nconditions\x18\x07 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryCondition\".\n\rSyntheticSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04rows\x18\x02 \x01(\x05\"\x84\x01\n\tTableSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\x12\x0f\n\x07\x66ilters\x18\x03 \x03(\t\x12\x0f\n\x07groupby\x18\x04 \x03(\t\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x11\n\tshowIndex\x18\x06 \x01(\x08\x12\x0e\n\x06\x62order\x18\x07 \x01(\x08\"@\n\x10TimeSeriesSchema\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x66req\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\x05\"\xfc\x01\n\nWebRequest\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestStatus\"\x9c\x01\n\x13WebRequestCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xa3\x01\n\x0eWebRequestList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequest\"\x85\x02\n\rWebRequestRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12U\n\x04spec\x18\x02 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRunSpec\x12Y\n\x06status\x18\x03 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRunStatus\"\x9f\x01\n\x16WebRequestRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xa9\x01\n\x11WebRequestRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12R\n\x05items\x18\x02 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRun\"\xef\x05\n\x11WebRequestRunSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\x12\x0c\n\x04verb\x18\x05 \x01(\t\x12k\n\nparameters\x18\x06 \x03(\x0b\x32W.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRunSpec.ParametersEntry\x12\x65\n\x07headers\x18\x07 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRunSpec.HeadersEntry\x12\x16\n\x0e\x63onnectionName\x18\x08 \x01(\t\x12\x0f\n\x07timeout\x18\t \x01(\x05\x12\x14\n\x0cmaterialized\x18\n \x01(\x08\x12\x10\n\x08reported\x18\x0b \x01(\x08\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x16\n\x0ewebRequestName\x18\r \x01(\t\x12\x33\n\x06labRef\x18\x0e \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x1a\x31\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe9\x05\n\x13WebRequestRunStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x03 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x13\n\x0btriggeredBy\x18\x06 \x01(\t\x12\x16\n\x0ehttpResultCode\x18\x07 \x01(\x05\x12Z\n\x0eresultLocation\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x12\n\nreportName\x18\t \x01(\t\x12\x15\n\rfailureReason\x18\n \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0b \x01(\t\x12K\n\x04logs\x18\x0c \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12?\n\x0blastUpdated\x18\r \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12`\n\nconditions\x18\x0f \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRunCondition\"\xfc\x01\n\x0eWebRequestSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12Y\n\x08template\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRunSpec\x12V\n\x08schedule\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"\xe4\x02\n\x10WebRequestStatus\x12?\n\x0blastUpdated\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12W\n\x07lastRun\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12]\n\nconditions\x18\x07 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestConditionB6Z4github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nDgithub.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x12\x34github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x83\x01\n\x0f\x41ggregationSpec\x12\x13\n\x0bslidePeriod\x18\x01 \x01(\t\x12[\n\x0c\x61ggregations\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureAggrSpec\"W\n\x0c\x42\x61rChartSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\x12\x0e\n\x06legend\x18\x04 \x01(\x08\x12\x0c\n\x04sort\x18\x05 \x01(\x08\"\xa9\x07\n\x06\x43olumn\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x02 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x0e\n\x06ignore\x18\x06 \x01(\x08\x12\x0e\n\x06target\x18\x07 \x01(\x08\x12\x10\n\x08nullable\x18\x08 \x01(\x08\x12\n\n\x02pk\x18\t \x01(\x08\x12\n\n\x02\x66k\x18\n \x01(\x08\x12\x12\n\nmultipleOf\x18\x0b \x01(\x05\x12\x0f\n\x07maximum\x18\x0c \x01(\x01\x12\x18\n\x10\x65xclusiveMaximum\x18\r \x01(\x08\x12\x0f\n\x07minimum\x18\x0e \x01(\x01\x12\x18\n\x10\x65xclusiveMinimum\x18\x0f \x01(\x08\x12\x11\n\tmaxLength\x18\x10 \x01(\x05\x12\x11\n\tminLength\x18\x11 \x01(\x05\x12\x0f\n\x07pattern\x18\x12 \x01(\t\x12\x10\n\x08required\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xample\x18\x14 \x01(\t\x12\x14\n\x0c\x65xternalDocs\x18\x15 \x01(\t\x12\x0c\n\x04\x65num\x18\x16 \x03(\t\x12\x0f\n\x07ordinal\x18\x17 \x01(\x08\x12\x10\n\x08maxItems\x18\x18 \x01(\x05\x12\x10\n\x08minItems\x18\x19 \x01(\x05\x12\x13\n\x0buniqueItems\x18\x1a \x01(\x08\x12\x0b\n\x03pii\x18\x1c \x01(\x08\x12\x0b\n\x03phi\x18\x1d \x01(\x08\x12\x14\n\x0cpersonalData\x18\x1e \x01(\x08\x12\x11\n\tprotected\x18\x1f \x01(\x08\x12\x17\n\x0f\x64\x65\x66\x61ultValueNum\x18  \x01(\x01\x12\x0b\n\x03log\x18! \x01(\x08\x12\n\n\x02mu\x18\" \x01(\x01\x12\r\n\x05sigma\x18# \x01(\x01\x12\x15\n\rskewThreshold\x18$ \x01(\x01\x12\x16\n\x0e\x64riftThreshold\x18% \x01(\x01\x12\x0b\n\x03key\x18& \x01(\x08\x12\x0c\n\x04\x66old\x18\' \x01(\x08\x12\x0e\n\x06weight\x18( \x01(\x08\x12\x10\n\x08reserved\x18) \x01(\x08\x12\x12\n\nimputation\x18* \x01(\t\x12\x0f\n\x07scaling\x18+ \x01(\t\x12\x11\n\tgenerated\x18, \x01(\x08\x12\x0f\n\x07\x66ormula\x18- \x01(\t\x12\n\n\x02id\x18. \x01(\x08\x12\x0c\n\x04step\x18/ \x01(\x01\x12\x0b\n\x03loc\x18\x30 \x01(\x05\x12\x16\n\x0e\x64\x61tetimeFormat\x18\x31 \x01(\t\x12\x12\n\ntimeseries\x18\x32 \x01(\x08\x12\x11\n\tregressor\x18\x33 \x01(\x08\x12\x17\n\x0flaggedRegressor\x18\x34 \x01(\x08\x12\x11\n\ttimeIndex\x18\x35 \x01(\x08\"\xe0\x01\n\x0f\x43olumnHistogram\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Y\n\thistogram\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.HistogramData\x12U\n\x07metrics\x18\x03 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05\x64rift\x18\x04 \x01(\x08\"\x81\x01\n\nColumnSpec\x12\x0e\n\x06spacer\x18\x01 \x01(\x08\x12\r\n\x05width\x18\x02 \x01(\x05\x12T\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ComponentSpec\"\xae\x07\n\x10\x43olumnStatistics\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x01\x12\x10\n\x08\x64istinct\x18\x04 \x01(\x05\x12\x0f\n\x07missing\x18\x05 \x01(\x05\x12\x16\n\x0epercentMissing\x18\x06 \x01(\x01\x12\x0c\n\x04mean\x18\x07 \x01(\x01\x12\x0e\n\x06stddev\x18\x08 \x01(\x01\x12\x10\n\x08variance\x18\t \x01(\x01\x12\x0b\n\x03min\x18\n \x01(\x01\x12\x0b\n\x03max\x18\x0b \x01(\x01\x12\x10\n\x08kurtosis\x18\x0c \x01(\x01\x12\x10\n\x08skewness\x18\r \x01(\x01\x12\x0b\n\x03sum\x18\x0e \x01(\x01\x12\x0b\n\x03mad\x18\x0f \x01(\x01\x12\x0b\n\x03p25\x18\x10 \x01(\x01\x12\x0b\n\x03p50\x18\x11 \x01(\x01\x12\x0b\n\x03p75\x18\x12 \x01(\x01\x12\x0b\n\x03iqr\x18\x13 \x01(\x01\x12\x0c\n\x04mode\x18\x14 \x01(\t\x12\r\n\x05zeros\x18\x15 \x01(\x01\x12\x0f\n\x07invalid\x18\x16 \x01(\x05\x12\x12\n\nimportance\x18\x17 \x01(\x01\x12\x0e\n\x06target\x18\x18 \x01(\x08\x12\x0e\n\x06ignore\x18\x19 \x01(\x08\x12\x10\n\x08nullable\x18\x1a \x01(\x08\x12\x17\n\x0fhighCardinality\x18\x1b \x01(\x08\x12!\n\x19highCorrWithOtherFeatures\x18\x1c \x01(\x08\x12\x19\n\x11lowCorrWithTarget\x18\x1d \x01(\x08\x12\x16\n\x0ehighMissingPct\x18\x1e \x01(\x08\x12\x0e\n\x06skewed\x18\x1f \x01(\x08\x12\n\n\x02id\x18  \x01(\x08\x12\x10\n\x08\x63onstant\x18! \x01(\x08\x12\x11\n\tduplicate\x18\" \x01(\x08\x12\x10\n\x08reserved\x18# \x01(\x08\x12\x14\n\x0c\x63ompleteness\x18% \x01(\x01\x12\x1a\n\x12\x64istinctValueCount\x18& \x01(\x01\x12\x1b\n\x13mostFreqValuesRatio\x18\' \x01(\x01\x12\x1a\n\x12indexOfPeculiarity\x18( \x01(\x01\x12Y\n\thistogram\x18) \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.HistogramData\x12\x14\n\x0c\x63orrToTarget\x18* \x01(\x01\x12\r\n\x05index\x18+ \x01(\x05\x12S\n\x08outliers\x18, \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.OutlierStat\"\x96\x01\n\rComponentSpec\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x0e\n\x06\x66ooter\x18\x03 \x01(\t\x12T\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ComponentView\"\xe3\x04\n\rComponentView\x12P\n\x06metric\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.MetricSpec\x12N\n\x05gauge\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GaugeSpec\x12V\n\thistogram\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.HistogramSpec\x12N\n\x05table\x18\x04 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.TableSpec\x12V\n\tlineChart\x18\x05 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LineChartSpec\x12T\n\x08\x62\x61rChart\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.BarChartSpec\x12Z\n\x0bscatterPlot\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ScatterPlotSpec\"P\n\x0b\x43orrelation\x12\x10\n\x08\x66\x65\x61ture1\x18\x01 \x01(\t\x12\x10\n\x08\x66\x65\x61ture2\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\x12\x0e\n\x06method\x18\x04 \x01(\t\">\n\x0f\x43orrelationSpec\x12\x0e\n\x06\x63utoff\x18\x01 \x01(\x01\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0b\n\x03top\x18\x03 \x01(\x05\"\x8b\x02\n\x0b\x43svFileSpec\x12\x17\n\x0f\x63olumnDelimiter\x18\x01 \x01(\t\x12\x14\n\x0crowDelimiter\x18\x02 \x01(\t\x12\r\n\x05quote\x18\x03 \x01(\t\x12\x12\n\nescapeChar\x18\x04 \x01(\t\x12\x14\n\x0c\x63ommentChars\x18\x05 \x01(\t\x12\x0e\n\x06header\x18\x06 \x01(\x08\x12\x10\n\x08skipRows\x18\x07 \x01(\x05\x12\x12\n\nnullValues\x18\x08 \x01(\t\x12\x10\n\x08\x65ncoding\x18\t \x01(\t\x12\x0f\n\x07maxRows\x18\n \x01(\x05\x12\x0e\n\x06strict\x18\x0b \x01(\x08\x12\x13\n\x0b\x63ompression\x18\x0c \x01(\t\x12\x16\n\x0ehasIndexColumn\x18\r \x01(\x08\"u\n\rDataInputSpec\x12T\n\x08location\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\"\xda\x01\n\x0c\x44\x61taLocation\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x12\n\nbucketName\x18\x03 \x01(\t\x12\x0c\n\x04path\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x06 \x01(\t\x12\x0b\n\x03sql\x18\x07 \x01(\t\x12\r\n\x05topic\x18\x08 \x01(\t\x12\x0b\n\x03url\x18\t \x01(\t\x12\x38\n\x0bresourceRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xf8\x01\n\x0e\x44\x61taOutputSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12T\n\x08location\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\x12\x1d\n\x15\x63reateTableIfNotExist\x18\x05 \x01(\x08\x12\x17\n\x0fincludeFeatures\x18\x06 \x01(\x08\x12\x0b\n\x03xai\x18\x07 \x01(\x08\x12\x16\n\x0e\x64\x65tectOutliers\x18\x08 \x01(\x08\"\x82\x02\n\x0c\x44\x61taPipeline\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineStatus\"\x9e\x01\n\x15\x44\x61taPipelineCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xa7\x01\n\x10\x44\x61taPipelineList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"\x8b\x02\n\x0f\x44\x61taPipelineRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunStatus\"\xa1\x01\n\x18\x44\x61taPipelineRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xad\x01\n\x13\x44\x61taPipelineRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRun\"\x95\x02\n\x13\x44\x61taPipelineRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x18\n\x10\x64\x61tapipelineName\x18\x02 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xd9\x04\n\x15\x44\x61taPipelineRunStatus\x12\x12\n\nrecipeRuns\x18\x01 \x03(\t\x12R\n\x06output\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\r\n\x05phase\x18\x03 \x01(\t\x12=\n\tstartTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x06 \x01(\x03\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x10\n\x08progress\x18\t \x01(\x05\x12K\n\x04logs\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12?\n\x0blastUpdated\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x62\n\nconditions\x18\x0c \x03(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunCondition\"\xe8\x05\n\x10\x44\x61taPipelineSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12t\n\x0f\x64\x61tasetSelector\x18\x03 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineSpec.DatasetSelectorEntry\x12U\n\x07recipes\x18\x04 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipePartSpec\x12T\n\x06output\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12V\n\x08schedule\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12_\n\x0cnotification\x18\x07 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\x08 \x01(\t\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\n \x01(\t\x12\x0e\n\x06paused\x18\x0b \x01(\x08\x12\x0b\n\x03ttl\x18\x0c \x01(\x05\x1a\x36\n\x14\x44\x61tasetSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe8\x02\n\x12\x44\x61taPipelineStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12?\n\x0blastUpdated\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12W\n\x07lastRun\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12_\n\nconditions\x18\x05 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineCondition\"\xff\x01\n\x0b\x44\x61taProduct\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductStatus\"\x9d\x01\n\x14\x44\x61taProductCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xa5\x01\n\x0f\x44\x61taProductList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\"\xc4\t\n\x0f\x44\x61taProductSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x0e\n\x06public\x18\x02 \x01(\x08\x12\x36\n\ttenantRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12V\n\x0bgitLocation\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GitLocation\x12Z\n\rimageLocation\x18\x05 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ImageLocation\x12\x0f\n\x07labName\x18\x07 \x01(\t\x12\x17\n\x0fservingSiteName\x18\x08 \x01(\t\x12\x0c\n\x04task\x18\t \x01(\t\x12\x0f\n\x07subtask\x18\n \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12X\n\x0c\x64\x61taLocation\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12_\n\x0cnotification\x18\r \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12`\n\x11trainingResources\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12_\n\x10servingResources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x18\n\x10retriesOnFailure\x18\x10 \x01(\x05\x12G\n\x04kpis\x18\x11 \x03(\x0b\x32\x39.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.KPI\x12\x19\n\x11onCallAccountName\x18\x12 \x01(\t\x12Z\n\x0b\x63ompilation\x18\x13 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CompilerSpec\x12\x16\n\x0e\x63learanceLevel\x18\x14 \x01(\t\x12\x10\n\x08priority\x18\x15 \x01(\t\x12\r\n\x05\x63olor\x18\x16 \x01(\t\x12X\n\ngovernance\x18\x17 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GovernanceSpec\x12]\n\x0bpermissions\x18\x18 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PermissionsSpec\"\xfc\x04\n\x11\x44\x61taProductStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12?\n\x0blastUpdated\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x18\n\x10totalDatasources\x18\x03 \x01(\x05\x12\x15\n\rtotalDatasets\x18\x04 \x01(\x05\x12\x1a\n\x12totalDataPipelines\x18\x05 \x01(\x05\x12\x1d\n\x15totalDataPipelineRuns\x18\x06 \x01(\x05\x12\x14\n\x0ctotalStudies\x18\x07 \x01(\x05\x12\x13\n\x0btotalModels\x18\x08 \x01(\x05\x12\x1b\n\x13totalModelPipelines\x18\t \x01(\x05\x12\x1e\n\x16totalModelPipelineRuns\x18\n \x01(\x05\x12\x17\n\x0ftotalPredictors\x18\x0b \x01(\x05\x12\x15\n\rtotalBuilders\x18\x0c \x01(\x05\x12\x11\n\ttotalApps\x18\r \x01(\x05\x12\x18\n\x10totalPredictions\x18\x0e \x01(\x05\x12\x17\n\x0ftotalInfoAlerts\x18\x0f \x01(\x05\x12\x18\n\x10totalErrorAlerts\x18\x10 \x01(\x05\x12\x15\n\rfailureReason\x18\x11 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x12 \x01(\t\x12\x17\n\x0f\x62\x61selineVersion\x18\x13 \x01(\t\x12^\n\nconditions\x18\x14 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductCondition\"\x94\x02\n\x12\x44\x61taProductVersion\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionSpec\x12^\n\x06status\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionStatus\"\xa4\x01\n\x1b\x44\x61taProductVersionCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xb3\x01\n\x16\x44\x61taProductVersionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\"\xa0\x01\n\x16\x44\x61taProductVersionSpec\x12\x37\n\nproductRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x17\n\x0fprevVersionName\x18\x03 \x01(\t\x12\x10\n\x08\x62\x61seline\x18\x04 \x01(\x08\x12\r\n\x05owner\x18\x05 \x01(\t\"\x8d\x02\n\x18\x44\x61taProductVersionStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12?\n\x0blastUpdated\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x65\n\nconditions\x18\x05 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionCondition\"\xfc\x01\n\nDataSource\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceStatus\"\x9c\x01\n\x13\x44\x61taSourceCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xa3\x01\n\x0e\x44\x61taSourceList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\"\xf8\x05\n\x0e\x44\x61taSourceSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x61tasetType\x18\x04 \x01(\t\x12L\n\x06schema\x18\x05 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latfile\x18\x06 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x0f\n\x07labeled\x18\x07 \x01(\x08\x12P\n\x06sample\x18\t \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12\x0c\n\x04task\x18\n \x01(\t\x12\x0f\n\x07subtask\x18\x0b \x01(\t\x12]\n\rrelationships\x18\x0c \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RelationshipSpec\x12T\n\x08labeling\x18\r \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingSpec\x12X\n\x0cinferredFrom\x18\x0e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12]\n\x11unitTestsTemplate\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\xec\x02\n\x10\x44\x61taSourceStatus\x12\x0c\n\x04\x63ols\x18\x01 \x01(\x05\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12\x46\n\x12lastDatasetCreated\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0flastDatasetName\x18\x04 \x01(\t\x12?\n\x0blastUpdated\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x06 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12]\n\nconditions\x18\x08 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceCondition\"\xf3\x01\n\x07\x44\x61taset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSpec\x12S\n\x06status\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetStatus\"\x99\x01\n\x10\x44\x61tasetCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xe0\x01\n\x14\x44\x61tasetGroupByStatus\x12\x13\n\x0b\x64\x61tasetsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x12\n\nreportsURI\x18\x03 \x01(\t\x12\x14\n\x0cunitTestsURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66\x65\x61turesURI\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\x0b\x44\x61tasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12L\n\x05items\x18\x02 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x9f\n\n\x0b\x44\x61tasetSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0e\x64\x61tasourceName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x05 \x01(\t\x12\x0c\n\x04role\x18\x06 \x01(\t\x12\x10\n\x08reported\x18\x07 \x01(\x08\x12\x13\n\x0bsnapshotted\x18\x08 \x01(\x08\x12\x12\n\nunitTested\x18\t \x01(\x08\x12R\n\x06origin\x18\r \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12T\n\x08location\x18\x0e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12X\n\tresources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x10 \x01(\x03\x12\x0c\n\x04type\x18\x11 \x01(\t\x12P\n\x06sample\x18\x12 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12V\n\tsyntactic\x18\x13 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SyntheticSpec\x12\x0c\n\x04task\x18\x14 \x01(\t\x12\x0f\n\x07subtask\x18\x15 \x01(\t\x12_\n\x0cnotification\x18\x16 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12Z\n\x0b\x63orrelation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.CorrelationSpec\x12\x0c\n\x04\x66\x61st\x18\x18 \x01(\x08\x12\x12\n\nfeaturized\x18\x19 \x01(\x08\x12\x33\n\x06labRef\x18\x1a \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\x11servingDatasetRef\x18\x1b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cpredictorRef\x18\x1c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12 \n\x18generateFeatureHistogram\x18\x1d \x01(\x08\x12U\n\tunitTests\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12R\n\x07groupBy\x18\x1f \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GroupBySpec\x12\x0b\n\x03key\x18  \x03(\t\"\xd9\x02\n\x11\x44\x61tasetStatistics\x12W\n\x07\x63olumns\x18\x01 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnStatistics\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0c\n\x04\x63ols\x18\x04 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\x05 \x01(\x05\x12\x61\n\x16\x63orrelationsWithTarget\x18\x06 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18\x07 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\"\xe3\x08\n\rDatasetStatus\x12[\n\nstatistics\x18\x01 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetStatistics\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x12\n\nreportName\x18\x03 \x01(\t\x12\x11\n\treportUri\x18\x04 \x01(\t\x12\x12\n\nprofileUri\x18\x05 \x01(\t\x12\x12\n\nimbalanced\x18\x06 \x01(\x08\x12\x14\n\x0c\x61nomaliesUri\x18\x07 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x08 \x01(\x03\x12\x61\n\x0funitTestResults\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x41\n\rlastStudyTime\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\r \x01(\t\x12\x10\n\x08progress\x18\x0e \x01(\x05\x12\x0c\n\x04hash\x18\x0f \x01(\t\x12K\n\x04logs\x18\x10 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x1a\n\x12\x64\x65rivedFromDataset\x18\x11 \x01(\t\x12?\n\x0blastUpdated\x18\x12 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12O\n\x06images\x18\x13 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12=\n\tstartTime\x18\x14 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x15 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12@\n\x13\x66\x65\x61tureHistogramRef\x18\x16 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12[\n\x07groupby\x18\x17 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetGroupByStatus\x12Z\n\nconditions\x18\x18 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetCondition\"\xa6\x01\n\x0f\x44\x61tasetTemplate\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSpec\"/\n\x0e\x44riftThreshold\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"\xf0\x01\n\x06\x45ntity\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntitySpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntityStatus\"\x98\x01\n\x0f\x45ntityCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\x9b\x01\n\nEntityList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\"S\n\nEntitySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04keys\x18\x03 \x03(\t\x12\r\n\x05owner\x18\x04 \x01(\t\"\xc6\x01\n\x0c\x45ntityStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12?\n\x0blastUpdated\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Y\n\nconditions\x18\x03 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntityCondition\"\xc1\x01\n\x11\x45xcelNotebookSpec\x12\x1a\n\x12\x66irstSheetWithData\x18\x01 \x01(\x08\x12\x11\n\tsheetName\x18\x02 \x01(\t\x12\x12\n\nsheetIndex\x18\x03 \x01(\x05\x12\x15\n\rcolumnNameRow\x18\x04 \x01(\x05\x12R\n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ExcelSheetArea\"k\n\x0e\x45xcelSheetArea\x12\x13\n\x0b\x65ntireSheet\x18\x01 \x01(\x08\x12\x12\n\nfromColumn\x18\x02 \x01(\x05\x12\x10\n\x08toColumn\x18\x03 \x01(\x05\x12\x0f\n\x07\x66romRow\x18\x04 \x01(\x05\x12\r\n\x05toRow\x18\x05 \x01(\x05\"\xf3\x01\n\x07\x46\x65\x61ture\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureSpec\x12S\n\x06status\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureStatus\"E\n\x0f\x46\x65\x61tureAggrSpec\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x11\n\tfunctions\x18\x02 \x03(\t\x12\x0f\n\x07windows\x18\x03 \x03(\t\"\x99\x01\n\x10\x46\x65\x61tureCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\x8e\x02\n\x10\x46\x65\x61tureHistogram\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramSpec\x12\\\n\x06status\x18\x03 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramStatus\"\xa2\x01\n\x19\x46\x65\x61tureHistogramCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xaf\x01\n\x14\x46\x65\x61tureHistogramList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\"\xf5\x04\n\x14\x46\x65\x61tureHistogramSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x05 \x03(\t\x12\x36\n\tsourceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08training\x18\x07 \x01(\x08\x12\x0c\n\x04live\x18\t \x01(\x08\x12\x39\n\x05start\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x37\n\x03\x65nd\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x34\n\x07\x62\x61seRef\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12]\n\x0f\x64riftThresholds\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12\x17\n\x0fsyncIntervalSec\x18\x0e \x01(\x05\x12U\n\tunitTests\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x14\n\x0cgenUnitTests\x18\x10 \x01(\x08\x12\x15\n\rfeatureFilter\x18\x11 \x01(\t\x12\x15\n\rreferenceType\x18\x12 \x01(\t\"\xbf\x04\n\x16\x46\x65\x61tureHistogramStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12V\n\x07\x63olumns\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnHistogram\x12?\n\x0blastUpdated\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05total\x18\n \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x0b \x01(\x05\x12\x63\n\nconditions\x18\x0c \x03(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramCondition\"\x9d\x01\n\x0b\x46\x65\x61tureList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12L\n\x05items\x18\x02 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Feature\"\x8b\x02\n\x0f\x46\x65\x61turePipeline\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineStatus\"\xa1\x01\n\x18\x46\x65\x61turePipelineCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xad\x01\n\x13\x46\x65\x61turePipelineList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipeline\"\x94\x02\n\x12\x46\x65\x61turePipelineRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineRunSpec\x12^\n\x06status\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineRunStatus\"\xa4\x01\n\x1b\x46\x65\x61turePipelineRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xb3\x01\n\x16\x46\x65\x61turePipelineRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineRun\"\xc0\x01\n\x16\x46\x65\x61turePipelineRunSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x1b\n\x13\x66\x65\x61turePipelineName\x18\x03 \x01(\t\x12X\n\tresources\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03ttl\x18\x05 \x01(\x05\"\xfa\x03\n\x18\x46\x65\x61turePipelineRunStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x03 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x13\n\x0btriggeredBy\x18\x05 \x01(\t\x12K\n\x04logs\x18\x06 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12?\n\x0blastUpdated\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x08 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\t \x01(\t\x12\x65\n\nconditions\x18\n \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineRunCondition\"\xd1\x05\n\x13\x46\x65\x61turePipelineSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12w\n\x0f\x64\x61tasetSelector\x18\x02 \x03(\x0b\x32^.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineSpec.DatasetSelectorEntry\x12\x13\n\x0bversionName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12Z\n\x0b\x61ggregation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.AggregationSpec\x12\x62\n\x0fmaterialization\x18\x06 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.MaterializationSpec\x12\x0e\n\x06\x66\x61mily\x18\x07 \x01(\t\x12\x12\n\nentityName\x18\x08 \x01(\t\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12V\n\x08schedule\x18\n \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x0b \x01(\x03\x12\x0e\n\x06paused\x18\x0c \x01(\x08\x12\x0b\n\x03ttl\x18\r \x01(\x05\x1a\x36\n\x14\x44\x61tasetSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x03\n\x15\x46\x65\x61turePipelineStatus\x12W\n\x07lastRun\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0b\x61verageCost\x18\x03 \x01(\x01\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12?\n\x0blastUpdated\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x62\n\nconditions\x18\x06 \x03(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturePipelineCondition\"\xba\x01\n\x0b\x46\x65\x61tureSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x11\n\tkeyColumn\x18\x05 \x01(\t\x12\x17\n\x0ftimestampColumn\x18\x06 \x01(\t\x12\x15\n\rfeatureColumn\x18\x07 \x01(\t\x12\x12\n\nentityName\x18\x08 \x01(\t\x12\x1b\n\x13\x66\x65\x61turePipelineName\x18\t \x01(\t\"\xf1\x04\n\rFeatureStatus\x12\x0b\n\x03min\x18\x02 \x01(\x01\x12\x0b\n\x03max\x18\x03 \x01(\x01\x12\x0c\n\x04mean\x18\x04 \x01(\x01\x12\x0e\n\x06stddev\x18\x05 \x01(\x01\x12\x10\n\x08skewness\x18\x06 \x01(\x01\x12\x10\n\x08kurtosis\x18\x07 \x01(\x01\x12\r\n\x05zeros\x18\x08 \x01(\x01\x12\x0b\n\x03p25\x18\n \x01(\x01\x12\x0b\n\x03p50\x18\x0b \x01(\x01\x12\x0b\n\x03p75\x18\x0c \x01(\x01\x12\x0f\n\x07missing\x18\x0e \x01(\x05\x12\x0f\n\x07invalid\x18\x0f \x01(\x05\x12\x0e\n\x06target\x18\x10 \x01(\x08\x12\x12\n\nimportance\x18\x11 \x01(\x01\x12\x0f\n\x07\x64istinc\x18\x12 \x01(\x05\x12\x0f\n\x07ignored\x18\x13 \x01(\x08\x12\x10\n\x08nullable\x18\x14 \x01(\x08\x12\x10\n\x08highCred\x18\x15 \x01(\x08\x12\x10\n\x08highCorr\x18\x16 \x01(\x08\x12\x0c\n\x04skew\x18\x17 \x01(\x08\x12\x14\n\x0c\x63ompleteness\x18\x18 \x01(\x01\x12\x1a\n\x12\x64istinctValueCount\x18\x19 \x01(\x01\x12\x1b\n\x13mostFreqValuesRatio\x18\x1a \x01(\x01\x12\x1a\n\x12indexOfPeculiarity\x18\x1b \x01(\x01\x12\x1a\n\x12observedGeneration\x18\x1c \x01(\x03\x12?\n\x0blastUpdated\x18\x1d \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Z\n\nconditions\x18\x1e \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureCondition\"\xfc\x01\n\nFeatureset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturesetSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturesetStatus\"\x9c\x01\n\x13\x46\x65\x61turesetCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xa3\x01\n\x0e\x46\x65\x61turesetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Featureset\"[\n\x0e\x46\x65\x61turesetSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x10\n\x08\x66\x65\x61tures\x18\x03 \x03(\t\x12\r\n\x05owner\x18\x04 \x01(\t\"\xce\x01\n\x10\x46\x65\x61turesetStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12?\n\x0blastUpdated\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12]\n\nconditions\x18\x03 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeaturesetCondition\"\xa6\x02\n\x12\x46latFileFormatSpec\x12\x10\n\x08\x66ileType\x18\x01 \x01(\t\x12N\n\x03\x63sv\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.CsvFileSpec\x12V\n\x05\x65xcel\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ExcelNotebookSpec\x12V\n\x07parquet\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ParquetFileSpec\"M\n\tGaugeSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0b\n\x03row\x18\x03 \x01(\x05\x12\x0e\n\x06scalar\x18\x04 \x01(\t\"V\n\x0bGitLocation\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x0f\n\x07private\x18\x04 \x01(\x08\"y\n\x16GovernanceReviewStatus\x12\x0e\n\x06result\x18\x01 \x01(\t\x12@\n\x0c\x61pprovalDate\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05notes\x18\x03 \x01(\t\"\x8d\x01\n\x0eGovernanceSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x02 \x01(\t\x12\x12\n\nitReviewer\x18\x03 \x01(\t\x12\x1a\n\x12\x63omplianceReviewer\x18\x04 \x01(\t\x12\x18\n\x10\x62usinessReviewer\x18\x05 \x01(\t\x12\x0f\n\x07members\x18\x06 \x03(\t\"\xd2\x02\n\x10GovernanceStatus\x12\x64\n\x0eITReviewStatus\x18\x01 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GovernanceReviewStatus\x12l\n\x16\x63omplianceReviewStatus\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GovernanceReviewStatus\x12j\n\x14\x62usinessReviewStatus\x18\x03 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GovernanceReviewStatus\"]\n\x0bGroupBySpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07groupby\x18\x02 \x03(\t\x12\x0c\n\x04\x66req\x18\x03 \x01(\t\x12\x10\n\x08interval\x18\x04 \x01(\x05\x12\x0c\n\x04\x61ggr\x18\x05 \x01(\t\"=\n\rHistogramSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\x0c\n\x04\x62ins\x18\x03 \x01(\x05\"=\n\rImageLocation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\x16registryConnectionName\x18\x02 \x01(\t\"\"\n\x03KPI\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"\x8e\x02\n\x10LabelingPipeline\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineSpec\x12\\\n\x06status\x18\x03 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineStatus\"\xa2\x01\n\x19LabelingPipelineCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xaf\x01\n\x14LabelingPipelineList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipeline\"\x97\x02\n\x13LabelingPipelineRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12[\n\x04spec\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineRunSpec\x12_\n\x06status\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineRunStatus\"\xa5\x01\n\x1cLabelingPipelineRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xb5\x01\n\x17LabelingPipelineRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12X\n\x05items\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineRun\"\xbf\x01\n\x17LabelingPipelineRunSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x19\n\x11labelPipelineName\x18\x03 \x01(\t\x12X\n\tresources\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03ttl\x18\x05 \x01(\x05\"\xaf\x03\n\x19LabelingPipelineRunStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x13\n\x0btriggeredBy\x18\x05 \x01(\t\x12?\n\x0blastUpdated\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x66\n\nconditions\x18\t \x03(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineRunCondition\"\x9c\x04\n\x14LabelingPipelineSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12x\n\x0f\x64\x61tasetSelector\x18\x03 \x03(\x0b\x32_.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineSpec.DatasetSelectorEntry\x12\x13\n\x0brecipeNames\x18\x04 \x03(\t\x12\x16\n\x0eoutputLabelset\x18\x05 \x01(\t\x12V\n\x08schedule\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\r\n\x05owner\x18\x07 \x01(\t\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\t \x01(\x03\x12\x0e\n\x06paused\x18\n \x01(\x08\x12\x0b\n\x03ttl\x18\x0b \x01(\x05\x1a\x36\n\x14\x44\x61tasetSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xf0\x02\n\x16LabelingPipelineStatus\x12W\n\x07lastRun\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12?\n\x0blastUpdated\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x63\n\nconditions\x18\x05 \x03(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingPipelineCondition\"?\n\x0cLabelingRule\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x10\n\x08operator\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xe1\x01\n\x0cLabelingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x14\n\x0cresultColumn\x18\x02 \x01(\t\x12T\n\x08positive\x18\x03 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingRule\x12T\n\x08negative\x18\x04 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingRule\"J\n\rLineChartSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\x12\x0e\n\x06legend\x18\x04 \x01(\x08\"\xae\x01\n\x13MaterializationSpec\x12\x0e\n\x06online\x18\x01 \x01(\x08\x12\x0f\n\x07offline\x18\x02 \x01(\x08\x12=\n\tstartDate\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x18\n\x10scheduleInterval\x18\x04 \x01(\t\x12\x0b\n\x03ttl\x18\x05 \x01(\x05\x12\x10\n\x08\x62\x61\x63kfill\x18\x06 \x01(\x05\"N\n\nMetricSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0b\n\x03row\x18\x03 \x01(\x05\x12\x0e\n\x06scalar\x18\x04 \x01(\t\"<\n\x0bOutlierStat\x12\r\n\x05lower\x18\x01 \x01(\x05\x12\r\n\x05upper\x18\x02 \x01(\x05\x12\x0f\n\x07percent\x18\x03 \x01(\x02\"W\n\x08PageSpec\x12K\n\x04rows\x18\x01 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RowSpec\"!\n\x0fParquetFileSpec\x12\x0e\n\x06\x65ngine\x18\x01 \x01(\t\"\xf0\x01\n\x06Recipe\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeSpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStatus\"\x98\x01\n\x0fRecipeCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\x8c\x01\n\x0fRecipeInputSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12T\n\x08location\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\"\x9b\x01\n\nRecipeList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x94\x01\n\x10RecipeOutputSpec\x12\x15\n\rcreateDataset\x18\x01 \x01(\x08\x12\x13\n\x0b\x64\x61tasetName\x18\x02 \x01(\t\x12T\n\x08location\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\"8\n\x0eRecipePartSpec\x12\x12\n\nrecipeName\x18\x01 \x01(\t\x12\x12\n\ndependents\x18\x02 \x03(\t\"\xf9\x01\n\tRecipeRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRunSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRunStatus\"\x9b\x01\n\x12RecipeRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xa1\x01\n\rRecipeRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\"\xa8\x02\n\rRecipeRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x12\n\nrecipeName\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12R\n\x06output\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03ttl\x18\x06 \x01(\x05\"\xc8\x04\n\x0fRecipeRunStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x03 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x13\n\x0btriggeredBy\x18\x07 \x01(\t\x12K\n\x04logs\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12?\n\x0blastUpdated\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\n \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12Y\n\nconditions\x18\x0b \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeCondition\"\xfb\x04\n\nRecipeSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12T\n\x05input\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeInputSpec\x12O\n\x05steps\x18\x05 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStep\x12V\n\x06output\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeOutputSpec\x12P\n\x06sample\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\n \x01(\x03\x12\x0b\n\x03ttl\x18\x0b \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\xdc\x02\n\x0cRecipeStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12W\n\x07lastRun\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0blastUpdated\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Y\n\nconditions\x18\x07 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeCondition\"s\n\nRecipeStep\x12\n\n\x02op\x18\x01 \x01(\t\x12Y\n\nparameters\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStepParam\".\n\x0fRecipeStepParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"X\n\x14RecommendationSchema\x12\x14\n\x0cuserIDColumn\x18\x01 \x01(\t\x12\x14\n\x0citemIDColumn\x18\x02 \x01(\t\x12\x14\n\x0cratingColumn\x18\x03 \x01(\t\"R\n\x10RelationshipSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\r\n\x05\x61rity\x18\x03 \x01(\t\x12\x11\n\trelatesTo\x18\x04 \x01(\t\"Y\n\x07RowSpec\x12N\n\x04\x63ols\x18\x01 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnSpec\"j\n\nSampleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0f\n\x07percent\x18\x04 \x01(\x05\x12\x0e\n\x06\x66ilter\x18\x05 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\"<\n\x0fScatterPlotSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\"\xb0\x02\n\x06Schema\x12`\n\x10timeSeriesSchema\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.TimeSeriesSchema\x12h\n\x14recommendationSchema\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecommendationSchema\x12M\n\x07\x63olumns\x18\x03 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Column\x12\x0b\n\x03key\x18\x04 \x03(\t\"\xf6\x01\n\x08SqlQuery\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQuerySpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryStatus\"\x9a\x01\n\x11SqlQueryCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\x9f\x01\n\x0cSqlQueryList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQuery\"\xff\x01\n\x0bSqlQueryRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryRunSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryRunStatus\"\x9d\x01\n\x14SqlQueryRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xa5\x01\n\x0fSqlQueryRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryRun\"\xfd\x03\n\x0fSqlQueryRunSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\x08\x12\x12\n\nsqlOrTable\x18\x06 \x01(\t\x12\x16\n\x0e\x63onnectionName\x18\x07 \x01(\t\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\t \x01(\x03\x12\x10\n\x08priority\x18\n \x01(\t\x12\x0f\n\x07\x61\x62orted\x18\x0b \x01(\x08\x12\x14\n\x0cmaterialized\x18\x0c \x01(\x08\x12\x10\n\x08reported\x18\r \x01(\x08\x12\x14\n\x0csqlQueryName\x18\x0e \x01(\t\x12\x33\n\x06labRef\x18\x0f \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x10 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\xc7\x05\n\x11SqlQueryRunStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x03 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x13\n\x0btriggeredBy\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12T\n\x08location\x18\t \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x12\n\nreportName\x18\n \x01(\t\x12?\n\x0blastUpdated\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\r \x01(\t\x12\x61\n\x0funitTestsResult\x18\x10 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12^\n\nconditions\x18\x0e \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryRunCondition\"\xf8\x01\n\x0cSqlQuerySpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12W\n\x08template\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryRunSpec\x12V\n\x08schedule\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"\xe0\x02\n\x0eSqlQueryStatus\x12?\n\x0blastUpdated\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12W\n\x07lastRun\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12[\n\nconditions\x18\x07 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SqlQueryCondition\".\n\rSyntheticSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04rows\x18\x02 \x01(\x05\"\x84\x01\n\tTableSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\x12\x0f\n\x07\x66ilters\x18\x03 \x03(\t\x12\x0f\n\x07groupby\x18\x04 \x03(\t\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x11\n\tshowIndex\x18\x06 \x01(\x08\x12\x0e\n\x06\x62order\x18\x07 \x01(\x08\"@\n\x10TimeSeriesSchema\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x66req\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\x05\"\xfc\x01\n\nWebRequest\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestStatus\"\x9c\x01\n\x13WebRequestCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xa3\x01\n\x0eWebRequestList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequest\"\x85\x02\n\rWebRequestRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12U\n\x04spec\x18\x02 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRunSpec\x12Y\n\x06status\x18\x03 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRunStatus\"\x9f\x01\n\x16WebRequestRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xa9\x01\n\x11WebRequestRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12R\n\x05items\x18\x02 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRun\"\xef\x05\n\x11WebRequestRunSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\x12\x0c\n\x04verb\x18\x05 \x01(\t\x12k\n\nparameters\x18\x06 \x03(\x0b\x32W.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRunSpec.ParametersEntry\x12\x65\n\x07headers\x18\x07 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRunSpec.HeadersEntry\x12\x16\n\x0e\x63onnectionName\x18\x08 \x01(\t\x12\x0f\n\x07timeout\x18\t \x01(\x05\x12\x14\n\x0cmaterialized\x18\n \x01(\x08\x12\x10\n\x08reported\x18\x0b \x01(\x08\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x16\n\x0ewebRequestName\x18\r \x01(\t\x12\x33\n\x06labRef\x18\x0e \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x1a\x31\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe9\x05\n\x13WebRequestRunStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x03 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x13\n\x0btriggeredBy\x18\x06 \x01(\t\x12\x16\n\x0ehttpResultCode\x18\x07 \x01(\x05\x12Z\n\x0eresultLocation\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x12\n\nreportName\x18\t \x01(\t\x12\x15\n\rfailureReason\x18\n \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0b \x01(\t\x12K\n\x04logs\x18\x0c \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12?\n\x0blastUpdated\x18\r \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12`\n\nconditions\x18\x0f \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRunCondition\"\xfc\x01\n\x0eWebRequestSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12Y\n\x08template\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestRunSpec\x12V\n\x08schedule\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"\xe4\x02\n\x10WebRequestStatus\x12?\n\x0blastUpdated\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12W\n\x07lastRun\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12]\n\nconditions\x18\x07 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.WebRequestConditionB6Z4github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1')
 
 
 
 _AGGREGATIONSPEC = DESCRIPTOR.message_types_by_name['AggregationSpec']
 _BARCHARTSPEC = DESCRIPTOR.message_types_by_name['BarChartSpec']
 _COLUMN = DESCRIPTOR.message_types_by_name['Column']
 _COLUMNHISTOGRAM = DESCRIPTOR.message_types_by_name['ColumnHistogram']
@@ -62,15 +62,14 @@
 _DATASOURCECONDITION = DESCRIPTOR.message_types_by_name['DataSourceCondition']
 _DATASOURCELIST = DESCRIPTOR.message_types_by_name['DataSourceList']
 _DATASOURCESPEC = DESCRIPTOR.message_types_by_name['DataSourceSpec']
 _DATASOURCESTATUS = DESCRIPTOR.message_types_by_name['DataSourceStatus']
 _DATASET = DESCRIPTOR.message_types_by_name['Dataset']
 _DATASETCONDITION = DESCRIPTOR.message_types_by_name['DatasetCondition']
 _DATASETGROUPBYSTATUS = DESCRIPTOR.message_types_by_name['DatasetGroupByStatus']
-_DATASETGROUPBYSTATUS_WORKERRESULTSENTRY = _DATASETGROUPBYSTATUS.nested_types_by_name['WorkerResultsEntry']
 _DATASETLIST = DESCRIPTOR.message_types_by_name['DatasetList']
 _DATASETSPEC = DESCRIPTOR.message_types_by_name['DatasetSpec']
 _DATASETSTATISTICS = DESCRIPTOR.message_types_by_name['DatasetStatistics']
 _DATASETSTATUS = DESCRIPTOR.message_types_by_name['DatasetStatus']
 _DATASETTEMPLATE = DESCRIPTOR.message_types_by_name['DatasetTemplate']
 _DRIFTTHRESHOLD = DESCRIPTOR.message_types_by_name['DriftThreshold']
 _ENTITY = DESCRIPTOR.message_types_by_name['Entity']
@@ -474,27 +473,19 @@
   'DESCRIPTOR' : _DATASETCONDITION,
   '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.generated_pb2'
   # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetCondition)
   })
 _sym_db.RegisterMessage(DatasetCondition)
 
 DatasetGroupByStatus = _reflection.GeneratedProtocolMessageType('DatasetGroupByStatus', (_message.Message,), {
-
-  'WorkerResultsEntry' : _reflection.GeneratedProtocolMessageType('WorkerResultsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _DATASETGROUPBYSTATUS_WORKERRESULTSENTRY,
-    '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.generated_pb2'
-    # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetGroupByStatus.WorkerResultsEntry)
-    })
-  ,
   'DESCRIPTOR' : _DATASETGROUPBYSTATUS,
   '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.generated_pb2'
   # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetGroupByStatus)
   })
 _sym_db.RegisterMessage(DatasetGroupByStatus)
-_sym_db.RegisterMessage(DatasetGroupByStatus.WorkerResultsEntry)
 
 DatasetList = _reflection.GeneratedProtocolMessageType('DatasetList', (_message.Message,), {
   'DESCRIPTOR' : _DATASETLIST,
   '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.generated_pb2'
   # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetList)
   })
 _sym_db.RegisterMessage(DatasetList)
@@ -1303,16 +1294,14 @@
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z4github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1'
   _DATAPIPELINESPEC_DATASETSELECTORENTRY._options = None
   _DATAPIPELINESPEC_DATASETSELECTORENTRY._serialized_options = b'8\001'
-  _DATASETGROUPBYSTATUS_WORKERRESULTSENTRY._options = None
-  _DATASETGROUPBYSTATUS_WORKERRESULTSENTRY._serialized_options = b'8\001'
   _FEATUREPIPELINESPEC_DATASETSELECTORENTRY._options = None
   _FEATUREPIPELINESPEC_DATASETSELECTORENTRY._serialized_options = b'8\001'
   _LABELINGPIPELINESPEC_DATASETSELECTORENTRY._options = None
   _LABELINGPIPELINESPEC_DATASETSELECTORENTRY._serialized_options = b'8\001'
   _WEBREQUESTRUNSPEC_PARAMETERSENTRY._options = None
   _WEBREQUESTRUNSPEC_PARAMETERSENTRY._serialized_options = b'8\001'
   _WEBREQUESTRUNSPEC_HEADERSENTRY._options = None
@@ -1398,241 +1387,239 @@
   _DATASOURCESTATUS._serialized_start=12686
   _DATASOURCESTATUS._serialized_end=13050
   _DATASET._serialized_start=13053
   _DATASET._serialized_end=13296
   _DATASETCONDITION._serialized_start=13299
   _DATASETCONDITION._serialized_end=13452
   _DATASETGROUPBYSTATUS._serialized_start=13455
-  _DATASETGROUPBYSTATUS._serialized_end=13754
-  _DATASETGROUPBYSTATUS_WORKERRESULTSENTRY._serialized_start=13702
-  _DATASETGROUPBYSTATUS_WORKERRESULTSENTRY._serialized_end=13754
-  _DATASETLIST._serialized_start=13757
-  _DATASETLIST._serialized_end=13914
-  _DATASETSPEC._serialized_start=13917
-  _DATASETSPEC._serialized_end=15228
-  _DATASETSTATISTICS._serialized_start=15231
-  _DATASETSTATISTICS._serialized_end=15576
-  _DATASETSTATUS._serialized_start=15579
-  _DATASETSTATUS._serialized_end=16702
-  _DATASETTEMPLATE._serialized_start=16705
-  _DATASETTEMPLATE._serialized_end=16871
-  _DRIFTTHRESHOLD._serialized_start=16873
-  _DRIFTTHRESHOLD._serialized_end=16920
-  _ENTITY._serialized_start=16923
-  _ENTITY._serialized_end=17163
-  _ENTITYCONDITION._serialized_start=17166
-  _ENTITYCONDITION._serialized_end=17318
-  _ENTITYLIST._serialized_start=17321
-  _ENTITYLIST._serialized_end=17476
-  _ENTITYSPEC._serialized_start=17478
-  _ENTITYSPEC._serialized_end=17561
-  _ENTITYSTATUS._serialized_start=17564
-  _ENTITYSTATUS._serialized_end=17762
-  _EXCELNOTEBOOKSPEC._serialized_start=17765
-  _EXCELNOTEBOOKSPEC._serialized_end=17958
-  _EXCELSHEETAREA._serialized_start=17960
-  _EXCELSHEETAREA._serialized_end=18067
-  _FEATURE._serialized_start=18070
-  _FEATURE._serialized_end=18313
-  _FEATUREAGGRSPEC._serialized_start=18315
-  _FEATUREAGGRSPEC._serialized_end=18384
-  _FEATURECONDITION._serialized_start=18387
-  _FEATURECONDITION._serialized_end=18540
-  _FEATUREHISTOGRAM._serialized_start=18543
-  _FEATUREHISTOGRAM._serialized_end=18813
-  _FEATUREHISTOGRAMCONDITION._serialized_start=18816
-  _FEATUREHISTOGRAMCONDITION._serialized_end=18978
-  _FEATUREHISTOGRAMLIST._serialized_start=18981
-  _FEATUREHISTOGRAMLIST._serialized_end=19156
-  _FEATUREHISTOGRAMSPEC._serialized_start=19159
-  _FEATUREHISTOGRAMSPEC._serialized_end=19788
-  _FEATUREHISTOGRAMSTATUS._serialized_start=19791
-  _FEATUREHISTOGRAMSTATUS._serialized_end=20366
-  _FEATURELIST._serialized_start=20369
-  _FEATURELIST._serialized_end=20526
-  _FEATUREPIPELINE._serialized_start=20529
-  _FEATUREPIPELINE._serialized_end=20796
-  _FEATUREPIPELINECONDITION._serialized_start=20799
-  _FEATUREPIPELINECONDITION._serialized_end=20960
-  _FEATUREPIPELINELIST._serialized_start=20963
-  _FEATUREPIPELINELIST._serialized_end=21136
-  _FEATUREPIPELINERUN._serialized_start=21139
-  _FEATUREPIPELINERUN._serialized_end=21415
-  _FEATUREPIPELINERUNCONDITION._serialized_start=21418
-  _FEATUREPIPELINERUNCONDITION._serialized_end=21582
-  _FEATUREPIPELINERUNLIST._serialized_start=21585
-  _FEATUREPIPELINERUNLIST._serialized_end=21764
-  _FEATUREPIPELINERUNSPEC._serialized_start=21767
-  _FEATUREPIPELINERUNSPEC._serialized_end=21959
-  _FEATUREPIPELINERUNSTATUS._serialized_start=21962
-  _FEATUREPIPELINERUNSTATUS._serialized_end=22468
-  _FEATUREPIPELINESPEC._serialized_start=22471
-  _FEATUREPIPELINESPEC._serialized_end=23192
+  _DATASETGROUPBYSTATUS._serialized_end=13679
+  _DATASETLIST._serialized_start=13682
+  _DATASETLIST._serialized_end=13839
+  _DATASETSPEC._serialized_start=13842
+  _DATASETSPEC._serialized_end=15153
+  _DATASETSTATISTICS._serialized_start=15156
+  _DATASETSTATISTICS._serialized_end=15501
+  _DATASETSTATUS._serialized_start=15504
+  _DATASETSTATUS._serialized_end=16627
+  _DATASETTEMPLATE._serialized_start=16630
+  _DATASETTEMPLATE._serialized_end=16796
+  _DRIFTTHRESHOLD._serialized_start=16798
+  _DRIFTTHRESHOLD._serialized_end=16845
+  _ENTITY._serialized_start=16848
+  _ENTITY._serialized_end=17088
+  _ENTITYCONDITION._serialized_start=17091
+  _ENTITYCONDITION._serialized_end=17243
+  _ENTITYLIST._serialized_start=17246
+  _ENTITYLIST._serialized_end=17401
+  _ENTITYSPEC._serialized_start=17403
+  _ENTITYSPEC._serialized_end=17486
+  _ENTITYSTATUS._serialized_start=17489
+  _ENTITYSTATUS._serialized_end=17687
+  _EXCELNOTEBOOKSPEC._serialized_start=17690
+  _EXCELNOTEBOOKSPEC._serialized_end=17883
+  _EXCELSHEETAREA._serialized_start=17885
+  _EXCELSHEETAREA._serialized_end=17992
+  _FEATURE._serialized_start=17995
+  _FEATURE._serialized_end=18238
+  _FEATUREAGGRSPEC._serialized_start=18240
+  _FEATUREAGGRSPEC._serialized_end=18309
+  _FEATURECONDITION._serialized_start=18312
+  _FEATURECONDITION._serialized_end=18465
+  _FEATUREHISTOGRAM._serialized_start=18468
+  _FEATUREHISTOGRAM._serialized_end=18738
+  _FEATUREHISTOGRAMCONDITION._serialized_start=18741
+  _FEATUREHISTOGRAMCONDITION._serialized_end=18903
+  _FEATUREHISTOGRAMLIST._serialized_start=18906
+  _FEATUREHISTOGRAMLIST._serialized_end=19081
+  _FEATUREHISTOGRAMSPEC._serialized_start=19084
+  _FEATUREHISTOGRAMSPEC._serialized_end=19713
+  _FEATUREHISTOGRAMSTATUS._serialized_start=19716
+  _FEATUREHISTOGRAMSTATUS._serialized_end=20291
+  _FEATURELIST._serialized_start=20294
+  _FEATURELIST._serialized_end=20451
+  _FEATUREPIPELINE._serialized_start=20454
+  _FEATUREPIPELINE._serialized_end=20721
+  _FEATUREPIPELINECONDITION._serialized_start=20724
+  _FEATUREPIPELINECONDITION._serialized_end=20885
+  _FEATUREPIPELINELIST._serialized_start=20888
+  _FEATUREPIPELINELIST._serialized_end=21061
+  _FEATUREPIPELINERUN._serialized_start=21064
+  _FEATUREPIPELINERUN._serialized_end=21340
+  _FEATUREPIPELINERUNCONDITION._serialized_start=21343
+  _FEATUREPIPELINERUNCONDITION._serialized_end=21507
+  _FEATUREPIPELINERUNLIST._serialized_start=21510
+  _FEATUREPIPELINERUNLIST._serialized_end=21689
+  _FEATUREPIPELINERUNSPEC._serialized_start=21692
+  _FEATUREPIPELINERUNSPEC._serialized_end=21884
+  _FEATUREPIPELINERUNSTATUS._serialized_start=21887
+  _FEATUREPIPELINERUNSTATUS._serialized_end=22393
+  _FEATUREPIPELINESPEC._serialized_start=22396
+  _FEATUREPIPELINESPEC._serialized_end=23117
   _FEATUREPIPELINESPEC_DATASETSELECTORENTRY._serialized_start=7412
   _FEATUREPIPELINESPEC_DATASETSELECTORENTRY._serialized_end=7466
-  _FEATUREPIPELINESTATUS._serialized_start=23195
-  _FEATUREPIPELINESTATUS._serialized_end=23582
-  _FEATURESPEC._serialized_start=23585
-  _FEATURESPEC._serialized_end=23771
-  _FEATURESTATUS._serialized_start=23774
-  _FEATURESTATUS._serialized_end=24399
-  _FEATURESET._serialized_start=24402
-  _FEATURESET._serialized_end=24654
-  _FEATURESETCONDITION._serialized_start=24657
-  _FEATURESETCONDITION._serialized_end=24813
-  _FEATURESETLIST._serialized_start=24816
-  _FEATURESETLIST._serialized_end=24979
-  _FEATURESETSPEC._serialized_start=24981
-  _FEATURESETSPEC._serialized_end=25072
-  _FEATURESETSTATUS._serialized_start=25075
-  _FEATURESETSTATUS._serialized_end=25281
-  _FLATFILEFORMATSPEC._serialized_start=25284
-  _FLATFILEFORMATSPEC._serialized_end=25578
-  _GAUGESPEC._serialized_start=25580
-  _GAUGESPEC._serialized_end=25657
-  _GITLOCATION._serialized_start=25659
-  _GITLOCATION._serialized_end=25745
-  _GOVERNANCEREVIEWSTATUS._serialized_start=25747
-  _GOVERNANCEREVIEWSTATUS._serialized_end=25868
-  _GOVERNANCESPEC._serialized_start=25871
-  _GOVERNANCESPEC._serialized_end=26012
-  _GOVERNANCESTATUS._serialized_start=26015
-  _GOVERNANCESTATUS._serialized_end=26353
-  _GROUPBYSPEC._serialized_start=26355
-  _GROUPBYSPEC._serialized_end=26448
-  _HISTOGRAMSPEC._serialized_start=26450
-  _HISTOGRAMSPEC._serialized_end=26511
-  _IMAGELOCATION._serialized_start=26513
-  _IMAGELOCATION._serialized_end=26574
-  _KPI._serialized_start=26576
-  _KPI._serialized_end=26610
-  _LABELINGPIPELINE._serialized_start=26613
-  _LABELINGPIPELINE._serialized_end=26883
-  _LABELINGPIPELINECONDITION._serialized_start=26886
-  _LABELINGPIPELINECONDITION._serialized_end=27048
-  _LABELINGPIPELINELIST._serialized_start=27051
-  _LABELINGPIPELINELIST._serialized_end=27226
-  _LABELINGPIPELINERUN._serialized_start=27229
-  _LABELINGPIPELINERUN._serialized_end=27508
-  _LABELINGPIPELINERUNCONDITION._serialized_start=27511
-  _LABELINGPIPELINERUNCONDITION._serialized_end=27676
-  _LABELINGPIPELINERUNLIST._serialized_start=27679
-  _LABELINGPIPELINERUNLIST._serialized_end=27860
-  _LABELINGPIPELINERUNSPEC._serialized_start=27863
-  _LABELINGPIPELINERUNSPEC._serialized_end=28054
-  _LABELINGPIPELINERUNSTATUS._serialized_start=28057
-  _LABELINGPIPELINERUNSTATUS._serialized_end=28488
-  _LABELINGPIPELINESPEC._serialized_start=28491
-  _LABELINGPIPELINESPEC._serialized_end=29031
+  _FEATUREPIPELINESTATUS._serialized_start=23120
+  _FEATUREPIPELINESTATUS._serialized_end=23507
+  _FEATURESPEC._serialized_start=23510
+  _FEATURESPEC._serialized_end=23696
+  _FEATURESTATUS._serialized_start=23699
+  _FEATURESTATUS._serialized_end=24324
+  _FEATURESET._serialized_start=24327
+  _FEATURESET._serialized_end=24579
+  _FEATURESETCONDITION._serialized_start=24582
+  _FEATURESETCONDITION._serialized_end=24738
+  _FEATURESETLIST._serialized_start=24741
+  _FEATURESETLIST._serialized_end=24904
+  _FEATURESETSPEC._serialized_start=24906
+  _FEATURESETSPEC._serialized_end=24997
+  _FEATURESETSTATUS._serialized_start=25000
+  _FEATURESETSTATUS._serialized_end=25206
+  _FLATFILEFORMATSPEC._serialized_start=25209
+  _FLATFILEFORMATSPEC._serialized_end=25503
+  _GAUGESPEC._serialized_start=25505
+  _GAUGESPEC._serialized_end=25582
+  _GITLOCATION._serialized_start=25584
+  _GITLOCATION._serialized_end=25670
+  _GOVERNANCEREVIEWSTATUS._serialized_start=25672
+  _GOVERNANCEREVIEWSTATUS._serialized_end=25793
+  _GOVERNANCESPEC._serialized_start=25796
+  _GOVERNANCESPEC._serialized_end=25937
+  _GOVERNANCESTATUS._serialized_start=25940
+  _GOVERNANCESTATUS._serialized_end=26278
+  _GROUPBYSPEC._serialized_start=26280
+  _GROUPBYSPEC._serialized_end=26373
+  _HISTOGRAMSPEC._serialized_start=26375
+  _HISTOGRAMSPEC._serialized_end=26436
+  _IMAGELOCATION._serialized_start=26438
+  _IMAGELOCATION._serialized_end=26499
+  _KPI._serialized_start=26501
+  _KPI._serialized_end=26535
+  _LABELINGPIPELINE._serialized_start=26538
+  _LABELINGPIPELINE._serialized_end=26808
+  _LABELINGPIPELINECONDITION._serialized_start=26811
+  _LABELINGPIPELINECONDITION._serialized_end=26973
+  _LABELINGPIPELINELIST._serialized_start=26976
+  _LABELINGPIPELINELIST._serialized_end=27151
+  _LABELINGPIPELINERUN._serialized_start=27154
+  _LABELINGPIPELINERUN._serialized_end=27433
+  _LABELINGPIPELINERUNCONDITION._serialized_start=27436
+  _LABELINGPIPELINERUNCONDITION._serialized_end=27601
+  _LABELINGPIPELINERUNLIST._serialized_start=27604
+  _LABELINGPIPELINERUNLIST._serialized_end=27785
+  _LABELINGPIPELINERUNSPEC._serialized_start=27788
+  _LABELINGPIPELINERUNSPEC._serialized_end=27979
+  _LABELINGPIPELINERUNSTATUS._serialized_start=27982
+  _LABELINGPIPELINERUNSTATUS._serialized_end=28413
+  _LABELINGPIPELINESPEC._serialized_start=28416
+  _LABELINGPIPELINESPEC._serialized_end=28956
   _LABELINGPIPELINESPEC_DATASETSELECTORENTRY._serialized_start=7412
   _LABELINGPIPELINESPEC_DATASETSELECTORENTRY._serialized_end=7466
-  _LABELINGPIPELINESTATUS._serialized_start=29034
-  _LABELINGPIPELINESTATUS._serialized_end=29402
-  _LABELINGRULE._serialized_start=29404
-  _LABELINGRULE._serialized_end=29467
-  _LABELINGSPEC._serialized_start=29470
-  _LABELINGSPEC._serialized_end=29695
-  _LINECHARTSPEC._serialized_start=29697
-  _LINECHARTSPEC._serialized_end=29771
-  _MATERIALIZATIONSPEC._serialized_start=29774
-  _MATERIALIZATIONSPEC._serialized_end=29948
-  _METRICSPEC._serialized_start=29950
-  _METRICSPEC._serialized_end=30028
-  _OUTLIERSTAT._serialized_start=30030
-  _OUTLIERSTAT._serialized_end=30090
-  _PAGESPEC._serialized_start=30092
-  _PAGESPEC._serialized_end=30179
-  _PARQUETFILESPEC._serialized_start=30181
-  _PARQUETFILESPEC._serialized_end=30214
-  _RECIPE._serialized_start=30217
-  _RECIPE._serialized_end=30457
-  _RECIPECONDITION._serialized_start=30460
-  _RECIPECONDITION._serialized_end=30612
-  _RECIPEINPUTSPEC._serialized_start=30615
-  _RECIPEINPUTSPEC._serialized_end=30755
-  _RECIPELIST._serialized_start=30758
-  _RECIPELIST._serialized_end=30913
-  _RECIPEOUTPUTSPEC._serialized_start=30916
-  _RECIPEOUTPUTSPEC._serialized_end=31064
-  _RECIPEPARTSPEC._serialized_start=31066
-  _RECIPEPARTSPEC._serialized_end=31122
-  _RECIPERUN._serialized_start=31125
-  _RECIPERUN._serialized_end=31374
-  _RECIPERUNCONDITION._serialized_start=31377
-  _RECIPERUNCONDITION._serialized_end=31532
-  _RECIPERUNLIST._serialized_start=31535
-  _RECIPERUNLIST._serialized_end=31696
-  _RECIPERUNSPEC._serialized_start=31699
-  _RECIPERUNSPEC._serialized_end=31995
-  _RECIPERUNSTATUS._serialized_start=31998
-  _RECIPERUNSTATUS._serialized_end=32582
-  _RECIPESPEC._serialized_start=32585
-  _RECIPESPEC._serialized_end=33220
-  _RECIPESTATUS._serialized_start=33223
-  _RECIPESTATUS._serialized_end=33571
-  _RECIPESTEP._serialized_start=33573
-  _RECIPESTEP._serialized_end=33688
-  _RECIPESTEPPARAM._serialized_start=33690
-  _RECIPESTEPPARAM._serialized_end=33736
-  _RECOMMENDATIONSCHEMA._serialized_start=33738
-  _RECOMMENDATIONSCHEMA._serialized_end=33826
-  _RELATIONSHIPSPEC._serialized_start=33828
-  _RELATIONSHIPSPEC._serialized_end=33910
-  _ROWSPEC._serialized_start=33912
-  _ROWSPEC._serialized_end=34001
-  _SAMPLESPEC._serialized_start=34003
-  _SAMPLESPEC._serialized_end=34109
-  _SCATTERPLOTSPEC._serialized_start=34111
-  _SCATTERPLOTSPEC._serialized_end=34171
-  _SCHEMA._serialized_start=34174
-  _SCHEMA._serialized_end=34478
-  _SQLQUERY._serialized_start=34481
-  _SQLQUERY._serialized_end=34727
-  _SQLQUERYCONDITION._serialized_start=34730
-  _SQLQUERYCONDITION._serialized_end=34884
-  _SQLQUERYLIST._serialized_start=34887
-  _SQLQUERYLIST._serialized_end=35046
-  _SQLQUERYRUN._serialized_start=35049
-  _SQLQUERYRUN._serialized_end=35304
-  _SQLQUERYRUNCONDITION._serialized_start=35307
-  _SQLQUERYRUNCONDITION._serialized_end=35464
-  _SQLQUERYRUNLIST._serialized_start=35467
-  _SQLQUERYRUNLIST._serialized_end=35632
-  _SQLQUERYRUNSPEC._serialized_start=35635
-  _SQLQUERYRUNSPEC._serialized_end=36144
-  _SQLQUERYRUNSTATUS._serialized_start=36147
-  _SQLQUERYRUNSTATUS._serialized_end=36858
-  _SQLQUERYSPEC._serialized_start=36861
-  _SQLQUERYSPEC._serialized_end=37109
-  _SQLQUERYSTATUS._serialized_start=37112
-  _SQLQUERYSTATUS._serialized_end=37464
-  _SYNTHETICSPEC._serialized_start=37466
-  _SYNTHETICSPEC._serialized_end=37512
-  _TABLESPEC._serialized_start=37515
-  _TABLESPEC._serialized_end=37647
-  _TIMESERIESSCHEMA._serialized_start=37649
-  _TIMESERIESSCHEMA._serialized_end=37713
-  _WEBREQUEST._serialized_start=37716
-  _WEBREQUEST._serialized_end=37968
-  _WEBREQUESTCONDITION._serialized_start=37971
-  _WEBREQUESTCONDITION._serialized_end=38127
-  _WEBREQUESTLIST._serialized_start=38130
-  _WEBREQUESTLIST._serialized_end=38293
-  _WEBREQUESTRUN._serialized_start=38296
-  _WEBREQUESTRUN._serialized_end=38557
-  _WEBREQUESTRUNCONDITION._serialized_start=38560
-  _WEBREQUESTRUNCONDITION._serialized_end=38719
-  _WEBREQUESTRUNLIST._serialized_start=38722
-  _WEBREQUESTRUNLIST._serialized_end=38891
-  _WEBREQUESTRUNSPEC._serialized_start=38894
-  _WEBREQUESTRUNSPEC._serialized_end=39645
-  _WEBREQUESTRUNSPEC_PARAMETERSENTRY._serialized_start=39548
-  _WEBREQUESTRUNSPEC_PARAMETERSENTRY._serialized_end=39597
-  _WEBREQUESTRUNSPEC_HEADERSENTRY._serialized_start=39599
-  _WEBREQUESTRUNSPEC_HEADERSENTRY._serialized_end=39645
-  _WEBREQUESTRUNSTATUS._serialized_start=39648
-  _WEBREQUESTRUNSTATUS._serialized_end=40393
-  _WEBREQUESTSPEC._serialized_start=40396
-  _WEBREQUESTSPEC._serialized_end=40648
-  _WEBREQUESTSTATUS._serialized_start=40651
-  _WEBREQUESTSTATUS._serialized_end=41007
+  _LABELINGPIPELINESTATUS._serialized_start=28959
+  _LABELINGPIPELINESTATUS._serialized_end=29327
+  _LABELINGRULE._serialized_start=29329
+  _LABELINGRULE._serialized_end=29392
+  _LABELINGSPEC._serialized_start=29395
+  _LABELINGSPEC._serialized_end=29620
+  _LINECHARTSPEC._serialized_start=29622
+  _LINECHARTSPEC._serialized_end=29696
+  _MATERIALIZATIONSPEC._serialized_start=29699
+  _MATERIALIZATIONSPEC._serialized_end=29873
+  _METRICSPEC._serialized_start=29875
+  _METRICSPEC._serialized_end=29953
+  _OUTLIERSTAT._serialized_start=29955
+  _OUTLIERSTAT._serialized_end=30015
+  _PAGESPEC._serialized_start=30017
+  _PAGESPEC._serialized_end=30104
+  _PARQUETFILESPEC._serialized_start=30106
+  _PARQUETFILESPEC._serialized_end=30139
+  _RECIPE._serialized_start=30142
+  _RECIPE._serialized_end=30382
+  _RECIPECONDITION._serialized_start=30385
+  _RECIPECONDITION._serialized_end=30537
+  _RECIPEINPUTSPEC._serialized_start=30540
+  _RECIPEINPUTSPEC._serialized_end=30680
+  _RECIPELIST._serialized_start=30683
+  _RECIPELIST._serialized_end=30838
+  _RECIPEOUTPUTSPEC._serialized_start=30841
+  _RECIPEOUTPUTSPEC._serialized_end=30989
+  _RECIPEPARTSPEC._serialized_start=30991
+  _RECIPEPARTSPEC._serialized_end=31047
+  _RECIPERUN._serialized_start=31050
+  _RECIPERUN._serialized_end=31299
+  _RECIPERUNCONDITION._serialized_start=31302
+  _RECIPERUNCONDITION._serialized_end=31457
+  _RECIPERUNLIST._serialized_start=31460
+  _RECIPERUNLIST._serialized_end=31621
+  _RECIPERUNSPEC._serialized_start=31624
+  _RECIPERUNSPEC._serialized_end=31920
+  _RECIPERUNSTATUS._serialized_start=31923
+  _RECIPERUNSTATUS._serialized_end=32507
+  _RECIPESPEC._serialized_start=32510
+  _RECIPESPEC._serialized_end=33145
+  _RECIPESTATUS._serialized_start=33148
+  _RECIPESTATUS._serialized_end=33496
+  _RECIPESTEP._serialized_start=33498
+  _RECIPESTEP._serialized_end=33613
+  _RECIPESTEPPARAM._serialized_start=33615
+  _RECIPESTEPPARAM._serialized_end=33661
+  _RECOMMENDATIONSCHEMA._serialized_start=33663
+  _RECOMMENDATIONSCHEMA._serialized_end=33751
+  _RELATIONSHIPSPEC._serialized_start=33753
+  _RELATIONSHIPSPEC._serialized_end=33835
+  _ROWSPEC._serialized_start=33837
+  _ROWSPEC._serialized_end=33926
+  _SAMPLESPEC._serialized_start=33928
+  _SAMPLESPEC._serialized_end=34034
+  _SCATTERPLOTSPEC._serialized_start=34036
+  _SCATTERPLOTSPEC._serialized_end=34096
+  _SCHEMA._serialized_start=34099
+  _SCHEMA._serialized_end=34403
+  _SQLQUERY._serialized_start=34406
+  _SQLQUERY._serialized_end=34652
+  _SQLQUERYCONDITION._serialized_start=34655
+  _SQLQUERYCONDITION._serialized_end=34809
+  _SQLQUERYLIST._serialized_start=34812
+  _SQLQUERYLIST._serialized_end=34971
+  _SQLQUERYRUN._serialized_start=34974
+  _SQLQUERYRUN._serialized_end=35229
+  _SQLQUERYRUNCONDITION._serialized_start=35232
+  _SQLQUERYRUNCONDITION._serialized_end=35389
+  _SQLQUERYRUNLIST._serialized_start=35392
+  _SQLQUERYRUNLIST._serialized_end=35557
+  _SQLQUERYRUNSPEC._serialized_start=35560
+  _SQLQUERYRUNSPEC._serialized_end=36069
+  _SQLQUERYRUNSTATUS._serialized_start=36072
+  _SQLQUERYRUNSTATUS._serialized_end=36783
+  _SQLQUERYSPEC._serialized_start=36786
+  _SQLQUERYSPEC._serialized_end=37034
+  _SQLQUERYSTATUS._serialized_start=37037
+  _SQLQUERYSTATUS._serialized_end=37389
+  _SYNTHETICSPEC._serialized_start=37391
+  _SYNTHETICSPEC._serialized_end=37437
+  _TABLESPEC._serialized_start=37440
+  _TABLESPEC._serialized_end=37572
+  _TIMESERIESSCHEMA._serialized_start=37574
+  _TIMESERIESSCHEMA._serialized_end=37638
+  _WEBREQUEST._serialized_start=37641
+  _WEBREQUEST._serialized_end=37893
+  _WEBREQUESTCONDITION._serialized_start=37896
+  _WEBREQUESTCONDITION._serialized_end=38052
+  _WEBREQUESTLIST._serialized_start=38055
+  _WEBREQUESTLIST._serialized_end=38218
+  _WEBREQUESTRUN._serialized_start=38221
+  _WEBREQUESTRUN._serialized_end=38482
+  _WEBREQUESTRUNCONDITION._serialized_start=38485
+  _WEBREQUESTRUNCONDITION._serialized_end=38644
+  _WEBREQUESTRUNLIST._serialized_start=38647
+  _WEBREQUESTRUNLIST._serialized_end=38816
+  _WEBREQUESTRUNSPEC._serialized_start=38819
+  _WEBREQUESTRUNSPEC._serialized_end=39570
+  _WEBREQUESTRUNSPEC_PARAMETERSENTRY._serialized_start=39473
+  _WEBREQUESTRUNSPEC_PARAMETERSENTRY._serialized_end=39522
+  _WEBREQUESTRUNSPEC_HEADERSENTRY._serialized_start=39524
+  _WEBREQUESTRUNSPEC_HEADERSENTRY._serialized_end=39570
+  _WEBREQUESTRUNSTATUS._serialized_start=39573
+  _WEBREQUESTRUNSTATUS._serialized_end=40318
+  _WEBREQUESTSPEC._serialized_start=40321
+  _WEBREQUESTSPEC._serialized_end=40573
+  _WEBREQUESTSTATUS._serialized_start=40576
+  _WEBREQUESTSTATUS._serialized_end=40932
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_data_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x12\x38github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"-\n\x18\x41lgorithmSearchSpaceSpec\x12\x11\n\tallowlist\x18\x01 \x03(\t\"`\n\x07\x41nomaly\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x64jDeltaColumn\x18\x03 \x01(\t\x12\r\n\x05start\x18\x04 \x01(\t\x12\x0b\n\x03\x65nd\x18\x05 \x01(\t\"\'\n\x11\x41udioPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"M\n\x0c\x42\x61\x63ktestSpec\x12\x0f\n\x07sliding\x18\x01 \x01(\x08\x12\x0e\n\x06splits\x18\x02 \x01(\x05\x12\x0f\n\x07Initial\x18\x03 \x01(\x05\x12\x0b\n\x03gap\x18\x05 \x01(\x05\"?\n\x0c\x42\x61selineSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbaselines\x18\x02 \x03(\t\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"\xf4\x01\n\x11\x43\x61pacityStageSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\x0fservingSiteName\x18\x02 \x01(\t\x12[\n\tunitTests\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelTestSuite\x12X\n\tresources\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\"\r\n\x0b\x43hangePoint\"$\n\x14\x43hatbotEstimatorSpec\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"\x93\x01\n\x0e\x43heckpointSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12\x63heckpointInterval\x18\x02 \x01(\x05\x12T\n\x08location\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\"\x92\x01\n\x16\x43lassicalEstimatorSpec\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x61\n\nparameters\x18\x02 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperParameterValue\"\x84\x02\n\nCronReport\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CronReportSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CronReportStatus\"\x9c\x01\n\x13\x43ronReportCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xa7\x01\n\x0e\x43ronReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CronReport\"\xe8\x02\n\x0e\x43ronReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12V\n\x08schedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\r\n\x05range\x18\x04 \x01(\t\x12Z\n\x08template\x18\x05 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportTemplate\x12\x0e\n\x06paused\x18\x06 \x01(\x08\x12_\n\x0cnotification\x18\x07 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\"\x97\x03\n\x10\x43ronReportStatus\x12W\n\x07lastRun\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0blastUpdated\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x61\n\nconditions\x18\x07 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CronReportCondition\"a\n\x10\x43ustomReportSpec\x12M\n\x05pages\x18\x08 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"L\n\nDataHashes\x12\x11\n\ttrainHash\x18\x01 \x01(\t\x12\x13\n\x0btestingHash\x18\x02 \x01(\t\x12\x16\n\x0evalidationHash\x18\x03 \x01(\t\"\x84\x02\n\rDataSplitSpec\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\r\n\x05train\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x0c\n\x04test\x18\x04 \x01(\x05\x12\x13\n\x0bsplitColumn\x18\x05 \x01(\t\x12W\n\x08segments\x18\x06 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SegmentSpec\x12\x14\n\x0ctrainDataset\x18\x07 \x01(\t\x12\x13\n\x0btestDataset\x18\x08 \x01(\t\x12\x19\n\x11validationDataset\x18\t \x01(\t\"`\n\rDataStageSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07labName\x18\x02 \x01(\t\x12\x18\n\x10\x64\x61tapipelineName\x18\x03 \x01(\t\x12\x13\n\x0b\x64ockerImage\x18\x04 \x01(\t\"\xa5\x01\n\x12\x44\x65\x65pEstimatorLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12^\n\nparameters\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NNLayerParameter\x12\x13\n\x0binputLayers\x18\x04 \x03(\t\"\xe6\x01\n\x11\x44\x65\x65pEstimatorSpec\x12\\\n\x06layers\x18\x01 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorLayer\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x11\n\tbatchSize\x18\x03 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x04 \x01(\x05\x12\x17\n\x0fvalidationSplit\x18\x05 \x01(\x05\x12\r\n\x05isSeq\x18\x06 \x01(\x08\x12\x0c\n\x04gpus\x18\x07 \x01(\x05\x12\x0c\n\x04loss\x18\x08 \x01(\t\"\x8e\x02\n\x13\x44\x65ploymentStageSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\x0fservingSiteName\x18\x02 \x01(\t\x12\x16\n\x0emanualApproval\x18\x03 \x01(\x08\x12[\n\tunitTests\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelTestSuite\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\".\n\x13\x44riftDetectorStatus\x12\x17\n\x0foutlierModelURI\x18\x01 \x01(\t\";\n\x0e\x44riftModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10outlierAlgorithm\x18\x02 \x01(\t\"R\n\rEarlyStopSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07initial\x18\x02 \x01(\x05\x12\x1f\n\x17minModelsWithNoProgress\x18\x03 \x01(\x05\"\x0f\n\rEnsembleRules\"\xf3\x01\n\x0c\x45nsembleSpec\x12\x0e\n\x06models\x18\x01 \x03(\t\x12\x64\n\nestimators\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12_\n\x05\x66inal\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x0c\n\x04type\x18\x04 \x01(\t\"_\n\rEnsemblesSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0evotingEnsemble\x18\x02 \x01(\x08\x12\x18\n\x10stackingEnsemble\x18\x03 \x01(\x08\x12\x0b\n\x03top\x18\x04 \x01(\x05\"\x89\x01\n\x0b\x45valMetrics\x12\x11\n\tselection\x18\x01 \x01(\t\x12\x11\n\treporting\x18\x02 \x03(\t\x12\x0f\n\x07\x61ggFunc\x18\x03 \x01(\t\x12\x11\n\taggPeriod\x18\x04 \x01(\x05\x12\x17\n\x0fnullModelParams\x18\x05 \x01(\t\x12\x17\n\x0frelErrTolerance\x18\x06 \x01(\x01\"\xe0\x01\n\nEvalPeriod\x12\x13\n\x0btestHorizon\x18\x01 \x01(\x05\x12\x1f\n\x17periodsBetweenTrainTest\x18\x02 \x01(\x05\x12\x1e\n\x16\x63vPeriodsBetweenSplits\x18\x03 \x01(\x05\x12\x1a\n\x12\x63vExpandingWindows\x18\x04 \x01(\x08\x12\x11\n\tcvHorizon\x18\x05 \x01(\x05\x12\x19\n\x11\x63vMinTrainPeriods\x18\x06 \x01(\x05\x12\x13\n\x0b\x63vMaxSplits\x18\x07 \x01(\x05\x12\x1d\n\x15\x63vUseMostRecentSplits\x18\x08 \x01(\x08\"\xc7\x06\n\x1a\x46\x65\x61tureEngineeringPipeline\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\x12\x12\n\nimputation\x18\x04 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x05 \x01(\t\x12\x0f\n\x07scaling\x18\x06 \x01(\t\x12\x16\n\x0e\x64iscretisation\x18\x07 \x01(\t\x12\x1e\n\x16variableTransformation\x18\x08 \x01(\t\x12\x17\n\x0foutlierHandling\x18\t \x01(\t\x12\x1e\n\x16\x64\x61tetimeTransformation\x18\n \x01(\t\x12X\n\x04text\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TextPipelineSpec\x12Z\n\x05image\x18\x0c \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImagePipelineSpec\x12Z\n\x05\x61udio\x18\r \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AudioPipelineSpec\x12Z\n\x05video\x18\x0e \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.VideoPipelineSpec\x12`\n\tgenerated\x18\x10 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GeneratedColumnSpec\x12]\n\x06\x63ustom\x18\x11 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GeneratedColumnSpec\x12\x0c\n\x04\x64rop\x18\x12 \x01(\x08\x12\x13\n\x0bpassthrough\x18\x13 \x01(\x08\"\x9a\x03\n\x1c\x46\x65\x61tureEngineeringSearchSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x19\n\x11imbalancedHandler\x18\x02 \x01(\t\x12\x11\n\testimator\x18\x03 \x01(\t\x12\x11\n\tmaxModels\x18\x04 \x01(\x05\x12\x0f\n\x07maxTime\x18\x05 \x01(\x05\x12\x13\n\x0bmaxTrainers\x18\x06 \x01(\x05\x12\x11\n\tsamplePct\x18\x07 \x01(\x05\x12\x12\n\nautoRemove\x18\x08 \x01(\x08\x12\r\n\x05reuse\x18\t \x01(\x08\x12p\n\x18\x66\x65\x61tureSelectionTemplate\x18\n \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\"\x80\x01\n\x1e\x46\x65\x61tureEngineeringSearchStatus\x12^\n\x04\x62\x65st\x18\x01 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\"\xf7\x01\n\x16\x46\x65\x61tureEngineeringSpec\x12g\n\tpipelines\x18\x01 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringPipeline\x12\x11\n\timbalance\x18\x02 \x01(\t\x12\x61\n\tselection\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\"8\n\x11\x46\x65\x61tureImportance\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x01\":\n\x0b\x46\x65\x61tureInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"#\n\x0b\x46\x65\x61turePair\x12\t\n\x01x\x18\x01 \x01(\t\x12\t\n\x01y\x18\x02 \x01(\t\"\xdd\x01\n\x14\x46\x65\x61tureSelectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tembedding\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\x08\x12\x0f\n\x07wrapper\x18\x05 \x01(\x08\x12\x10\n\x08pipeline\x18\x06 \x03(\t\x12\x1c\n\x14varianceThresholdPct\x18\x07 \x01(\x05\x12\x15\n\rcorrThreshold\x18\x08 \x01(\x05\x12\x13\n\x0bmaxFeatures\x18\t \x01(\x05\x12\x12\n\npercentile\x18\n \x01(\x05\x12\x10\n\x08reserved\x18\x0c \x03(\t\"\xd4\x07\n\x0e\x46orecasterSpec\x12Y\n\x06\x65vents\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TimeSeriesEvent\x12R\n\x04past\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12T\n\x06\x66uture\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12\x10\n\x08\x63overage\x18\x06 \x01(\x01\x12Z\n\x0eoutputLocation\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x10\n\x08\x66\x65\x61tures\x18\x08 \x03(\t\x12\x0e\n\x06groups\x18\t \x03(\t\x12\x1a\n\x12predefinedTemplate\x18\n \x01(\t\x12T\n\tanomalies\x18\x0b \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Anomaly\x12\x14\n\x0ctrainEndData\x18\x0c \x01(\t\x12\x13\n\x0bvalueColumn\x18\r \x01(\t\x12\x11\n\thpoBudget\x18\x0e \x01(\x05\x12`\n\x11\x65valuationMetrics\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalMetrics\x12^\n\x10\x65valuationPeriod\x18\x10 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalPeriod\x12^\n\x0bseasonality\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalitySpec\x12\x12\n\nregressors\x18\x12 \x03(\t\x12\x18\n\x10laggedRegressors\x18\x13 \x03(\t\x12\x0e\n\x06growth\x18\x14 \x01(\t\x12\x0b\n\x03key\x18\x15 \x03(\t\"s\n\x15GarbageCollectionSpec\x12\x19\n\x11\x63ollectAtStudyEnd\x18\x01 \x01(\x08\x12%\n\x1dkeepOnlyBestModelPerAlgorithm\x18\x02 \x01(\x08\x12\x18\n\x10keepPrunedModels\x18\x03 \x01(\x08\"\x83\x01\n\x17GarbageCollectionStatus\x12\x11\n\tcollected\x18\x01 \x01(\x05\x12U\n\x06models\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelResult\"f\n\x13GeneratedColumnSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x66irst\x18\x03 \x01(\t\x12\x0e\n\x06second\x18\x04 \x01(\t\x12\x10\n\x08original\x18\x05 \x01(\t\"2\n\x13HyperParameterValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"o\n\x10HyperbandOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x14\n\x0cmaxResources\x18\x02 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"\'\n\x11ImagePipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\";\n\x15ImbalanceHandlingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\timbalance\x18\x02 \x01(\t\"\x9a\x02\n\x14InterpretabilitySpec\x12\x0b\n\x03ice\x18\x01 \x01(\x08\x12W\n\x08icepairs\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x0c\n\x04lime\x18\x03 \x01(\x08\x12\x0c\n\x04shap\x18\x04 \x01(\t\x12X\n\tshappairs\x18\x05 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x16\n\x0e\x63ounterfactual\x18\x06 \x01(\x08\x12\x0e\n\x06\x61nchor\x18\x07 \x01(\x08\"\xd2\x02\n\x16InterpretabilityStatus\x12\x45\n\x11trainingStartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x0ftrainingEndTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x14\n\x0c\x65xplainerURI\x18\x03 \x01(\t\x12\x1a\n\x12trainShapValuesURI\x18\x04 \x01(\t\x12\x19\n\x11testShapValuesURI\x18\x05 \x01(\t\x12_\n\nimportance\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\"V\n\x05Level\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05index\x18\x02 \x03(\t\x12\x0f\n\x07horizon\x18\x03 \x01(\x05\x12\x0c\n\x04\x66req\x18\x04 \x01(\t\x12\x11\n\taggregate\x18\x05 \x01(\t\"k\n\x13MedianPrunerOptions\x12\x15\n\rstartupTrials\x18\x01 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x02 \x01(\x05\x12\x15\n\rintervalSteps\x18\x03 \x01(\x05\x12\x11\n\tminTrials\x18\x04 \x01(\x05\"\xf5\x01\n\x05Model\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStatus\"\x96\x02\n\x10ModelAutobuilder\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12\\\n\x04spec\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelAutobuilderSpec\x12`\n\x06status\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelAutobuilderStatus\"\xa2\x01\n\x19ModelAutobuilderCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xb3\x01\n\x14ModelAutobuilderList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Y\n\x05items\x18\x02 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelAutobuilder\"\xbe\x06\n\x14ModelAutobuilderSpec\x12\x17\n\x0f\x64\x61taProductName\x18\x01 \x01(\t\x12\x1e\n\x16\x64\x61taProductVersionName\x18\x02 \x01(\t\x12\x16\n\x0e\x64\x61tasourceName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x04 \x01(\t\x12T\n\x08location\x18\x05 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x0c\n\x04task\x18\x06 \x01(\t\x12\x0f\n\x07subtask\x18\x07 \x01(\t\x12\x11\n\tobjective\x18\x08 \x01(\t\x12\x14\n\x0ctargetColumn\x18\t \x01(\t\x12\x0f\n\x07maxTime\x18\n \x01(\x05\x12\x11\n\tmaxModels\x18\x0b \x01(\x05\x12\x14\n\x0c\x61\x63\x63\x65ssMethod\x18\x0c \x01(\t\x12\x11\n\tautoScale\x18\r \x01(\x08\x12\x1a\n\x12\x66\x65\x61tureEngineering\x18\x0e \x01(\x08\x12\x18\n\x10\x66\x65\x61tureSelection\x18\x0f \x01(\x08\x12\x0f\n\x07\x64\x61taapp\x18\x10 \x01(\x08\x12\\\n\x0e\x64\x61taSourceSpec\x18\x11 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceSpec\x12\x10\n\x08trainers\x18\x12 \x01(\x05\x12\x0f\n\x07sampler\x18\x13 \x01(\t\x12\x0f\n\x07\x61\x62orted\x18\x14 \x01(\x08\x12\r\n\x05owner\x18\x15 \x01(\t\x12X\n\tresources\x18\x16 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x33\n\x06labRef\x18\x17 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12;\n\x0eservingSiteRef\x18\x18 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetType\x18\x19 \x01(\t\x12\x0c\n\x04\x66\x61st\x18\x1a \x01(\x08\"\x9a\x06\n\x16ModelAutobuilderStatus\x12\x14\n\x0c\x66latFileName\x18\x01 \x01(\t\x12\x16\n\x0e\x64\x61taSourceName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x11\n\tstudyName\x18\x04 \x01(\t\x12\x15\n\rbestModelName\x18\x06 \x01(\t\x12\x15\n\rpredictorName\x18\x07 \x01(\t\x12\x13\n\x0b\x64\x61taappName\x18\x08 \x01(\t\x12\x15\n\rimageRepoName\x18\t \x01(\t\x12\r\n\x05phase\x18\n \x01(\t\x12\x0c\n\x04rows\x18\x0b \x01(\x05\x12\x0c\n\x04\x63ols\x18\x0c \x01(\x05\x12\x10\n\x08\x66ileSize\x18\r \x01(\x05\x12\x0e\n\x06models\x18\x0e \x01(\x05\x12\x15\n\rtrainedModels\x18\x0f \x01(\x05\x12\x16\n\x0e\x62\x65stModelScore\x18\x10 \x01(\x01\x12\x63\n\testimator\x18\x11 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12=\n\tstartTime\x18\x12 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x13 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x15 \x01(\x03\x12\x15\n\rfailureReason\x18\x16 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x17 \x01(\t\x12?\n\x0blastUpdated\x18\x18 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12g\n\nconditions\x18\x19 \x03(\x0b\x32S.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelAutobuilderCondition\"\x96\x02\n\x10ModelCompilerRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12\\\n\x04spec\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelCompilerRunSpec\x12`\n\x06status\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelCompilerRunStatus\"\xa2\x01\n\x19ModelCompilerRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xb3\x01\n\x14ModelCompilerRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Y\n\x05items\x18\x02 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelCompilerRun\"\x96\x01\n\x14ModelCompilerRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x11\n\tmodelName\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12\x10\n\x08priority\x18\x05 \x01(\t\x12\x10\n\x08\x63ompiler\x18\x06 \x01(\t\x12\x0e\n\x06target\x18\x07 \x01(\t\"\xc6\x03\n\x16ModelCompilerRunStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x42\n\x0e\x63ompletionTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x03 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x05 \x01(\t\x12\x15\n\rfailureReason\x18\x06 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x10\n\x08progress\x18\x08 \x01(\x05\x12?\n\x0blastUpdated\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12g\n\nconditions\x18\n \x03(\x0b\x32S.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelCompilerRunCondition\"\x97\x01\n\x0eModelCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xfe\x01\n\x12ModelGroupByStatus\x12\x11\n\tmodelsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x12\n\nreportsURI\x18\x03 \x01(\t\x12v\n\rworkerResults\x18\x04 \x03(\x0b\x32_.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus.WorkerResultsEntry\x1a\x34\n\x12WorkerResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"R\n\x0eModelImageSpec\x12\r\n\x05\x65xist\x18\x01 \x01(\x08\x12\x11\n\timageName\x18\x02 \x01(\t\x12\x1e\n\x16registryConnectionName\x18\x03 \x01(\t\"\x9d\x01\n\tModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x8d\x02\n\rModelPipeline\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Y\n\x04spec\x18\x02 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineSpec\x12]\n\x06status\x18\x03 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineStatus\"\x9f\x01\n\x16ModelPipelineCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xad\x01\n\x11ModelPipelineList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12V\n\x05items\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipeline\"\x96\x02\n\x10ModelPipelineRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12\\\n\x04spec\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunSpec\x12`\n\x06status\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStatus\"\xa2\x01\n\x19ModelPipelineRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xb3\x01\n\x14ModelPipelineRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Y\n\x05items\x18\x02 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRun\"\xba\x01\n\x14ModelPipelineRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x14\n\x0cpipelineName\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x0b\n\x03ttl\x18\t \x01(\x05\"\x80\x03\n\x1bModelPipelineRunStageStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12\x10\n\x08\x61pproved\x18\x02 \x01(\x08\x12\x12\n\napprovedBy\x18\x03 \x01(\t\x12>\n\napprovedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\tstartTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05\x65rror\x18\n \x01(\t\"\xaa\x0b\n\x16ModelPipelineRunStatus\x12\r\n\x05stage\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x02 \x01(\t\x12\x11\n\tstudyName\x18\x03 \x01(\t\x12\x11\n\tmodelName\x18\x04 \x01(\t\x12\x63\n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12g\n\x08training\x18\x06 \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12\x62\n\x03uat\x18\x07 \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12g\n\x08\x63\x61pacity\x18\x08 \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12i\n\ndeployment\x18\t \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12\x66\n\x07release\x18\n \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12\x66\n\x07monitor\x18\x0b \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12g\n\x08labeling\x18\x0c \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12=\n\tstartTime\x18\r \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x0f \x01(\t\x12\x1a\n\x12observedGeneration\x18\x10 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x11 \x01(\t\x12\x15\n\rfailureReason\x18\x12 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x13 \x01(\t\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12\x13\n\x0btriggeredBy\x18\x15 \x01(\t\x12?\n\x0blastUpdated\x18\x16 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\x17 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12g\n\nconditions\x18\x18 \x03(\x0b\x32S.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunCondition\"\xbc\x08\n\x11ModelPipelineSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12y\n\x0f\x64\x61tasetSelector\x18\x03 \x03(\x0b\x32`.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineSpec.DatasetSelectorEntry\x12U\n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataStageSpec\x12]\n\x08training\x18\x05 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingStageSpec\x12S\n\x03uat\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.UATStageSpec\x12]\n\x08\x63\x61pacity\x18\x07 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CapacityStageSpec\x12\x61\n\ndeployment\x18\t \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeploymentStageSpec\x12[\n\x07release\x18\n \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReleaseStageSpec\x12V\n\x08schedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\r\n\x05owner\x18\r \x01(\t\x12\x1b\n\x13\x61pproverAccountName\x18\x0e \x01(\t\x12_\n\x0cnotification\x18\x0f \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\x19\n\x11\x62\x61selineModelName\x18\x10 \x01(\t\x12\x10\n\x08priority\x18\x11 \x01(\t\x12\x0e\n\x06paused\x18\x12 \x01(\x08\x1a\x36\n\x14\x44\x61tasetSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9d\x03\n\x13ModelPipelineStatus\x12W\n\x07lastRun\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12?\n\x0blastUpdated\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x64\n\nconditions\x18\x07 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineCondition\"W\n\x0bModelResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03\x61lg\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x01\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x0f\n\x07trialID\x18\x05 \x01(\x05\"\xca\x10\n\tModelSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x04 \x01(\t\x12\x11\n\tstudyName\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x06 \x01(\t\x12\x0c\n\x04task\x18\x07 \x01(\t\x12\x0f\n\x07subtask\x18\x08 \x01(\t\x12\x11\n\tobjective\x18\t \x01(\t\x12l\n\x12\x66\x65\x61tureEngineering\x18\n \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12\x63\n\testimator\x18\x0b \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12X\n\x03\x64nn\x18\x0c \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorSpec\x12_\n\x07\x63hatbot\x18\r \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ChatbotEstimatorSpec\x12`\n\x0cnlpEstimator\x18\x0e \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NLPEstimatorSpec\x12X\n\x08\x65nsemble\x18\x0f \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsembleSpec\x12X\n\x08training\x18\x10 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12V\n\x07serving\x18\x11 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12\x0e\n\x06tested\x18\x12 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x13 \x01(\x08\x12\x10\n\x08packaged\x18\x14 \x01(\x08\x12\x11\n\tpublished\x18\x15 \x01(\x08\x12\x0e\n\x06pushed\x18\x16 \x01(\x08\x12\x10\n\x08reported\x18\x17 \x01(\x08\x12\x0e\n\x06paused\x18\x18 \x01(\x08\x12\x10\n\x08profiled\x18\x19 \x01(\x08\x12\x10\n\x08\x61rchived\x18\x1a \x01(\x08\x12\x12\n\nforecasted\x18\x1b \x01(\x08\x12\x10\n\x08released\x18\x1c \x01(\x08\x12\x12\n\nregistered\x18\x1d \x01(\x08\x12\x0f\n\x07predict\x18\x1e \x01(\x08\x12\r\n\x05tuned\x18\x1f \x01(\x08\x12\x11\n\texplained\x18  \x01(\x08\x12\x15\n\rcodeGenerated\x18! \x01(\x08\x12\x10\n\x08\x62\x61seline\x18\" \x01(\x08\x12\x18\n\x10genDriftDetector\x18# \x01(\x08\x12\x0c\n\x04\x66\x61st\x18$ \x01(\x08\x12\x12\n\nunitTested\x18% \x01(\x08\x12?\n\x12\x66\x65\x65\x64\x62\x61\x63kDatasetRef\x18& \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x66lagged\x18\' \x01(\x08\x12T\n\x08location\x18( \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12]\n\x0b\x66orecasting\x18) \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12Z\n\x0b\x63ompilation\x18* \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CompilerSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18+ \x01(\x03\x12\x15\n\restimatorType\x18, \x01(\t\x12\x0b\n\x03ttl\x18- \x01(\x05\x12\x12\n\nmodelClass\x18. \x01(\t\x12\x0f\n\x07trialID\x18/ \x01(\x05\x12X\n\ngovernance\x18\x30 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GovernanceSpec\x12h\n\x10interpretability\x18\x31 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12U\n\tunitTests\x18\x32 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12Y\n\rfeedbackTests\x18\x33 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\xc3\x1f\n\x0bModelStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x45\n\x11trainingStartTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x0ftrainingEndTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x44\n\x10testingStartTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x42\n\x0etestingEndTime\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x0ftuningStartTime\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x41\n\rtuningEndTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0f\n\x07\x63vScore\x18\t \x01(\x01\x12\x15\n\rtrainingScore\x18\n \x01(\x01\x12\x11\n\ttestScore\x18\x0b \x01(\x01\x12\x0c\n\x04\x63ost\x18\x0c \x01(\x01\x12\x0c\n\x04\x62\x65st\x18\r \x01(\x08\x12P\n\x02\x63v\x18\x0e \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12S\n\x05train\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04test\x18\x10 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04tune\x18\x11 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12V\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x12 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x43\n\x16lastFeedbackDatasetRef\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\r\n\x05phase\x18\x14 \x01(\t\x12\x12\n\nreportName\x18\x15 \x01(\t\x12\x11\n\treportUri\x18\x16 \x01(\t\x12\x13\n\x0bmanifestUri\x18\x17 \x01(\t\x12\x12\n\nweightsUri\x18\x18 \x01(\t\x12\x17\n\x0flabelEncoderUri\x18\x19 \x01(\t\x12\x0f\n\x07logsUri\x18\x1a \x01(\t\x12\x12\n\nprofileUri\x18\x1b \x01(\t\x12\x1c\n\x14misclassificationUri\x18\x1c \x01(\t\x12\x0e\n\x06tarUri\x18\x1d \x01(\t\x12\x0e\n\x06\x61ppUri\x18\x1e \x01(\t\x12\x11\n\timageName\x18\x1f \x01(\t\x12_\n\nimportance\x18  \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12j\n\x15permutationImportance\x18! \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12\x13\n\x0b\x66orecastUri\x18\" \x01(\t\x12X\n\x07runtime\x18# \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus\x12X\n\x0ctrainDataset\x18$ \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12W\n\x0btestDataset\x18% \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12]\n\x11validationDataset\x18& \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x1a\n\x12observedGeneration\x18\' \x01(\x03\x12\x14\n\x0ctrainingRows\x18( \x01(\x05\x12\x13\n\x0btestingRows\x18) \x01(\x05\x12\x16\n\x0evalidationRows\x18* \x01(\x05\x12\x15\n\rfailureReason\x18+ \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18, \x01(\t\x12\x10\n\x08progress\x18- \x01(\x05\x12\x13\n\x0bsizeInBytes\x18. \x01(\x05\x12\x0f\n\x07latency\x18/ \x01(\x01\x12\x0b\n\x03url\x18\x30 \x01(\t\x12\x15\n\rpredictorName\x18\x31 \x01(\t\x12>\n\nreleasedAt\x18\x32 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0bpredictedAt\x18\x33 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0btarFileHash\x18\x34 \x01(\t\x12\x11\n\timageHash\x18\x35 \x01(\t\x12^\n\x10trainingDataHash\x18\x36 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12h\n\x11trainingResources\x18\x37 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ResourceConsumption\x12g\n\x10testingResources\x18\x38 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ResourceConsumption\x12\x11\n\ttrainedBy\x18\x39 \x01(\t\x12\x0c\n\x04team\x18: \x01(\t\x12\x10\n\x08\x65ndpoint\x18; \x01(\t\x12K\n\x04logs\x18< \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12V\n\x08rocCurve\x18= \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RocAucCurve\x12Q\n\x07prCurve\x18> \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PRCurve\x12\x66\n\x14trainConfusionMatrix\x18? \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18@ \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x61\n\x16\x63orrelationsWithTarget\x18\x41 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18\x42 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12?\n\x0blastUpdated\x18\x43 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x10governanceStatus\x18\x44 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GovernanceStatus\x12j\n\x10interpretability\x18\x45 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilityStatus\x12O\n\x06images\x18\x46 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12\x61\n\x0funitTestsResult\x18G \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x65\n\x13\x66\x65\x65\x64\x62\x61\x63kTestsResult\x18H \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x14\n\x0csubModelsURI\x18I \x01(\t\x12\\\n\nconditions\x18J \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelCondition\"\xdf\x01\n\x0eModelTestSuite\x12=\n\x10\x62\x61selineModelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\ndatasetRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\" \n\x10NLPEstimatorSpec\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"/\n\x10NNLayerParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xfe\x01\n\x08Notebook\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookStatus\"\x9a\x01\n\x11NotebookCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xa3\x01\n\x0cNotebookList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Notebook\"\x87\x02\n\x0bNotebookRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookRunSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookRunStatus\"\x9d\x01\n\x14NotebookRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xa9\x01\n\x0fNotebookRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookRun\"\xc3\x02\n\x0fNotebookRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x14\n\x0cnotebookName\x18\x02 \x01(\t\x12Z\n\x06values\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookVarValue\x12\r\n\x05owner\x18\x04 \x01(\t\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03ttl\x18\x06 \x01(\x05\x12\x33\n\x06labRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xf0\x03\n\x11NotebookRunStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x13\n\x0btriggeredBy\x18\x07 \x01(\t\x12K\n\x04logs\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12?\n\x0blastUpdated\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x62\n\nconditions\x18\n \x03(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookRunCondition\"\xeb\x04\n\x0cNotebookSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x36\n\tschemaRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x11\n\timageName\x18\x04 \x01(\t\x12\x14\n\x0crequirements\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65\x62Packages\x18\x06 \x01(\t\x12\x0c\n\x04vars\x18\x07 \x03(\t\x12T\n\x08location\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\r\n\x05owner\x18\t \x01(\t\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x0b \x01(\x03\x12V\n\x08schedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x10\n\x08priority\x18\r \x01(\t\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12U\n\tunitTests\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\xe3\x03\n\x0eNotebookStatus\x12\r\n\x05image\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12W\n\x07lastRun\x18\x04 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0blastUpdated\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\x07 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12_\n\nconditions\x18\t \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookCondition\"/\n\x10NotebookVarValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x84\x01\n\x17PercentilePrunerOptions\x12\x12\n\npercentile\x18\x01 \x01(\x05\x12\x15\n\rstartupTrials\x18\x02 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x16\n\x0eintervalTrials\x18\x04 \x01(\x05\x12\x11\n\tminTrials\x18\x05 \x01(\x05\"\x93\x04\n\nPrunerSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12]\n\x06median\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.MedianPrunerOptions\x12\x65\n\npercentile\x18\x03 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PercentilePrunerOptions\x12m\n\x11successiveHalving\x18\x04 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingOptions\x12]\n\thyperband\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperbandOptions\x12\x63\n\tthreshold\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ThresholdPrunerOptions\"\xd0\x01\n\x18RegressionForecasterSpec\x12\x10\n\x08\x65nsemble\x18\x01 \x01(\x08\x12\x12\n\nimputation\x18\x02 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x0f\n\x07scaling\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\x08\x12\x0f\n\x07windows\x18\x06 \x03(\x05\x12\x0c\n\x04lags\x18\x07 \x03(\x05\x12\x11\n\tfunctions\x18\x08 \x03(\t\x12\x0b\n\x03\x65ma\x18\t \x01(\x08\x12\x0b\n\x03log\x18\n \x01(\x08\x12\x11\n\treduction\x18\x0b \x01(\t\"\xa5\x02\n\x10ReleaseStageSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\x0fservingSiteName\x18\x02 \x01(\t\x12\x15\n\rpredictorName\x18\x03 \x01(\t\x12^\n\x08template\x18\x04 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ModelDeploymentSpec\x12\x16\n\x0emanualApproval\x18\x05 \x01(\x08\x12X\n\tresources\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\"\xf8\x01\n\x06Report\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportStatus\"\x98\x01\n\x0fReportCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\x9f\x01\n\nReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xa7\x04\n\nReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x36\n\tentityRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12T\n\x08location\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x12\n\nreportType\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x06 \x01(\t\x12\x14\n\x0cnotifierName\x18\x07 \x01(\t\x12\r\n\x05owner\x18\x08 \x01(\t\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\n \x01(\x03\x12Z\n\x06\x63ustom\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CustomReportSpec\x12\x16\n\x0e\x63ronReportName\x18\x0c \x01(\t\x12\x33\n\x06labRef\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03key\x18\x0e \x03(\t\"\xde\x03\n\x0cReportStatus\x12=\n\tstartTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x04 \x01(\t\x12\x0b\n\x03uri\x18\x05 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x06 \x01(\x03\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12K\n\x04logs\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12?\n\x0blastUpdated\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12]\n\nconditions\x18\x0b \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportCondition\"d\n\x0eReportTemplate\x12R\n\x04spec\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\"<\n\x13ResourceConsumption\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x01\x12\x0b\n\x03mem\x18\x02 \x01(\x01\x12\x0b\n\x03gpu\x18\x03 \x01(\x01\"\xf1\x01\n\rRuntimeStatus\x12\x15\n\rpythonVersion\x18\x01 \x01(\t\x12\x11\n\tpythonCmd\x18\x02 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12s\n\x0epythonPackages\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus.PythonPackagesEntry\x1a\x35\n\x13PythonPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x80\x04\n\nSearchSpec\x12\x0f\n\x07sampler\x18\x01 \x01(\t\x12T\n\x06pruner\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PrunerSpec\x12\x0f\n\x07maxCost\x18\x03 \x01(\x05\x12\x0f\n\x07maxTime\x18\x04 \x01(\x05\x12\x11\n\tmaxModels\x18\x05 \x01(\x05\x12\x14\n\x0cminBestScore\x18\x06 \x01(\x01\x12\x10\n\x08trainers\x18\x07 \x01(\x05\x12\x0c\n\x04test\x18\x08 \x01(\x05\x12\x11\n\tretainTop\x18\t \x01(\x05\x12\x13\n\x0bretainedFor\x18\n \x01(\x05\x12g\n\x0bsearchSpace\x18\x0b \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\x12\x11\n\tobjective\x18\x0e \x01(\t\x12\x12\n\nobjective2\x18\x0f \x01(\t\x12\x0c\n\x04tune\x18\x10 \x01(\x08\"L\n\x15SeasonalityPeriodSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x61uto\x18\x02 \x01(\x08\x12\x14\n\x0c\x66ourierOrder\x18\x03 \x01(\x05\"\x87\x04\n\x0fSeasonalitySpec\x12\x0c\n\x04\x61uto\x18\x01 \x01(\x08\x12_\n\x06yearly\x18\x02 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12\x62\n\tquarterly\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12`\n\x07monthly\x18\x04 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12_\n\x06weekly\x18\x05 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12^\n\x05\x64\x61ily\x18\x06 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\"<\n\x0bSegmentSpec\x12\x12\n\ncolumnName\x18\x01 \x01(\t\x12\n\n\x02op\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"w\n\x0bServingSpec\x12X\n\tresources\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"\xf5\x01\n\x05Study\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudySpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyStatus\"\x97\x01\n\x0eStudyCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\x9d\x01\n\tStudyList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\x84\x02\n\x10StudyPhaseStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0f\n\x07waiting\x18\x03 \x01(\x05\x12\x0f\n\x07running\x18\x04 \x01(\x05\x12\x0e\n\x06\x66\x61iled\x18\x05 \x01(\x05\x12\x11\n\tcompleted\x18\x06 \x01(\x05\x12\x11\n\tbestScore\x18\x07 \x01(\x01\x12\x1c\n\x14modelsWithNoProgress\x18\x08 \x01(\x05\"a\n\x11StudyScheduleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12;\n\x07startAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\x98\x10\n\tStudySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetName\x18\x04 \x01(\t\x12\x0c\n\x04task\x18\x05 \x01(\t\x12\x0f\n\x07subtask\x18\x06 \x01(\t\x12h\n\x08\x66\x65Search\x18\x07 \x01(\x0b\x32V.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSearchSpec\x12i\n\x10imbalanceHandler\x18\x08 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImbalanceHandlingSpec\x12X\n\x08\x62\x61seline\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.BaselineSpec\x12T\n\x06search\x18\n \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SearchSpec\x12Z\n\tensembles\x18\x0b \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsemblesSpec\x12`\n\x10trainingTemplate\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12^\n\x0fservingTemplate\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12]\n\x0b\x66\x63tTemplate\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12]\n\x08schedule\x18\x0f \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyScheduleSpec\x12h\n\x10interpretability\x18\x10 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12`\n\x0e\x64riftDetection\x18\x11 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftModelSpec\x12\x0f\n\x07\x61\x62orted\x18\x12 \x01(\x08\x12\x10\n\x08reported\x18\x13 \x01(\x08\x12\x0e\n\x06paused\x18\x14 \x01(\x08\x12\x10\n\x08profiled\x18\x15 \x01(\x08\x12\x16\n\x0emodelPublished\x18\x16 \x01(\x08\x12\x18\n\x10modelImagePushed\x18\x17 \x01(\x08\x12\x16\n\x0emodelExplained\x18\x18 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x19 \x01(\x08\x12T\n\x08location\x18\x1a \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\r\n\x05owner\x18\x1b \x01(\t\x12Z\n\x0b\x63ompilation\x18\x1c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CompilerSpec\x12\x10\n\x08template\x18\x1d \x01(\x08\x12\x0f\n\x07\x66lagged\x18\x1e \x01(\x08\x12_\n\x0cnotification\x18\x1f \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\nmodelImage\x18  \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelImageSpec\x12[\n\x02gc\x18! \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionSpec\x12\x0b\n\x03ttl\x18\" \x01(\x05\x12\x14\n\x0cmodelVersion\x18# \x01(\t\x12\x15\n\rtimeoutInSecs\x18$ \x01(\x05\x12\x15\n\rcodeGenerated\x18% \x01(\x08\x12]\n\x11unitTestsTemplate\x18& \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\x95\x0f\n\x0bStudyStatus\x12\x0e\n\x06models\x18\x01 \x01(\x05\x12=\n\tstartTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tbestModel\x18\x04 \x01(\t\x12\x16\n\x0e\x62\x65stModelScore\x18\x05 \x01(\x01\x12\x12\n\nprofileUri\x18\x06 \x01(\t\x12\x11\n\treportUri\x18\x07 \x01(\t\x12\x12\n\nreportName\x18\x08 \x01(\t\x12\r\n\x05phase\x18\t \x01(\t\x12\x1a\n\x12observedGeneration\x18\n \x01(\x03\x12X\n\x0ctrainDataset\x18\x0b \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12W\n\x0btestDataset\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12]\n\x11validationDataset\x18\r \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x13\n\x0blastModelID\x18\x0e \x01(\x03\x12\x15\n\rfailureReason\x18\x0f \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x10 \x01(\t\x12\x14\n\x0ctrainingRows\x18\x11 \x01(\x05\x12\x13\n\x0btestingRows\x18\x12 \x01(\x05\x12\x16\n\x0evalidationRows\x18\x13 \x01(\x05\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12^\n\x10trainingDataHash\x18\x16 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12\x13\n\x0btriggeredBy\x18\x17 \x01(\t\x12K\n\x04logs\x18\x18 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x66\n\x12\x66\x65\x61tureEngineering\x18\x19 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x62\x61seline\x18\x1a \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12Z\n\x06search\x18\x1b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x65nsemble\x18\x1c \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12X\n\x04test\x18\x1d \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12[\n\x07\x65xplain\x18\x1e \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\x65\n\x0e\x64riftDetection\x18\x1f \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftDetectorStatus\x12?\n\x0blastUpdated\x18  \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18! \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12]\n\x02gc\x18\" \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionStatus\x12\\\n\nconditions\x18# \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyCondition\"\x7f\n\x18SuccessiveHalvingOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x02 \x01(\x05\x12\x1c\n\x14minEarlyStoppingRate\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"h\n\x15SuccessiveHalvingSpec\x12\x0e\n\x06\x62udget\x18\x01 \x01(\x05\x12\x0f\n\x07\x62racket\x18\x02 \x01(\x05\x12\x0c\n\x04rung\x18\x03 \x01(\x05\x12\x0e\n\x06\x63onfID\x18\x04 \x01(\x05\x12\x10\n\x08modality\x18\x1a \x01(\t\"\xad\x01\n\x10TextPipelineSpec\x12\x0f\n\x07\x65ncoder\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x02 \x01(\t\x12\x11\n\tstopwords\x18\x03 \x01(\x08\x12\x0b\n\x03pos\x18\x04 \x01(\x08\x12\r\n\x05lemma\x18\x05 \x01(\x08\x12\x0c\n\x04stem\x18\x06 \x01(\x08\x12\x11\n\tembedding\x18\x07 \x01(\t\x12\x0b\n\x03svd\x18\x08 \x01(\x08\x12\x18\n\x10maxSvdComponents\x18\t \x01(\x05\"b\n\x16ThresholdPrunerOptions\x12\r\n\x05lower\x18\x01 \x01(\x01\x12\r\n\x05upper\x18\x02 \x01(\x01\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x15\n\rintervalSteps\x18\x04 \x01(\x05\"\x8a\x01\n\x0fTimeSeriesEvent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0f\n\x07holiday\x18\x03 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x10\n\x08preEvent\x18\x05 \x01(\x05\x12\x11\n\tpostEvent\x18\x06 \x01(\x05\x12\x12\n\ntimePoints\x18\x07 \x03(\t\"\x9c\x05\n\x0cTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08priority\x18\x02 \x01(\t\x12\x0e\n\x06\x63vtype\x18\x03 \x01(\t\x12\n\n\x02\x63V\x18\x04 \x01(\x08\x12\r\n\x05\x66olds\x18\x05 \x01(\x05\x12V\n\x05split\x18\x06 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataSplitSpec\x12\x13\n\x0b\x65valMetrics\x18\x07 \x03(\t\x12[\n\x02sh\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingSpec\x12\x0c\n\x04seed\x18\x0b \x01(\x01\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03gpu\x18\r \x01(\x08\x12\x13\n\x0b\x64istributed\x18\x0e \x01(\x08\x12\x19\n\x11\x66\x65\x61tureImportance\x18\x0f \x01(\x08\x12\x11\n\tnodeCount\x18\x10 \x01(\x05\x12\x11\n\tsamplePct\x18\x11 \x01(\x05\x12\\\n\ncheckpoint\x18\x12 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CheckpointSpec\x12\x10\n\x08logLevel\x18\x13 \x01(\t\x12\x15\n\rtimeoutInSecs\x18\x14 \x01(\x05\"f\n\x11TrainingStageSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x14\n\x0cnotebookName\x18\x02 \x01(\t\x12\x0f\n\x07labName\x18\x03 \x01(\t\x12\x19\n\x11studyTemplateName\x18\x04 \x01(\t\"\xef\x01\n\x0cUATStageSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\x0fservingSiteName\x18\x02 \x01(\t\x12[\n\tunitTests\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelTestSuite\x12X\n\tresources\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\"\xdc\x01\n\x18UnivariateForecastStatus\x12\x1b\n\x13gridSearchResultURI\x18\x01 \x01(\t\x12g\n\rbaseEstimator\x18\x02 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x10\n\x08modelURI\x18\x03 \x01(\t\x12\x13\n\x0b\x63vResultURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x05 \x01(\t\"\'\n\x11VideoPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"=\n\nWindowSpec\x12\x10\n\x08interval\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x0e\n\x06length\x18\x03 \x01(\x05\x42:Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x12\x38github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"-\n\x18\x41lgorithmSearchSpaceSpec\x12\x11\n\tallowlist\x18\x01 \x03(\t\"`\n\x07\x41nomaly\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x64jDeltaColumn\x18\x03 \x01(\t\x12\r\n\x05start\x18\x04 \x01(\t\x12\x0b\n\x03\x65nd\x18\x05 \x01(\t\"\'\n\x11\x41udioPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"M\n\x0c\x42\x61\x63ktestSpec\x12\x0f\n\x07sliding\x18\x01 \x01(\x08\x12\x0e\n\x06splits\x18\x02 \x01(\x05\x12\x0f\n\x07Initial\x18\x03 \x01(\x05\x12\x0b\n\x03gap\x18\x05 \x01(\x05\"?\n\x0c\x42\x61selineSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbaselines\x18\x02 \x03(\t\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"\xf4\x01\n\x11\x43\x61pacityStageSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\x0fservingSiteName\x18\x02 \x01(\t\x12[\n\tunitTests\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelTestSuite\x12X\n\tresources\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\"\r\n\x0b\x43hangePoint\"$\n\x14\x43hatbotEstimatorSpec\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"\x93\x01\n\x0e\x43heckpointSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12\x63heckpointInterval\x18\x02 \x01(\x05\x12T\n\x08location\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\"\x92\x01\n\x16\x43lassicalEstimatorSpec\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x61\n\nparameters\x18\x02 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperParameterValue\"\x84\x02\n\nCronReport\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CronReportSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CronReportStatus\"\x9c\x01\n\x13\x43ronReportCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xa7\x01\n\x0e\x43ronReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CronReport\"\xe8\x02\n\x0e\x43ronReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12V\n\x08schedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\r\n\x05range\x18\x04 \x01(\t\x12Z\n\x08template\x18\x05 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportTemplate\x12\x0e\n\x06paused\x18\x06 \x01(\x08\x12_\n\x0cnotification\x18\x07 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\"\x97\x03\n\x10\x43ronReportStatus\x12W\n\x07lastRun\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0blastUpdated\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x61\n\nconditions\x18\x07 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CronReportCondition\"a\n\x10\x43ustomReportSpec\x12M\n\x05pages\x18\x08 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"L\n\nDataHashes\x12\x11\n\ttrainHash\x18\x01 \x01(\t\x12\x13\n\x0btestingHash\x18\x02 \x01(\t\x12\x16\n\x0evalidationHash\x18\x03 \x01(\t\"\x84\x02\n\rDataSplitSpec\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\r\n\x05train\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x0c\n\x04test\x18\x04 \x01(\x05\x12\x13\n\x0bsplitColumn\x18\x05 \x01(\t\x12W\n\x08segments\x18\x06 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SegmentSpec\x12\x14\n\x0ctrainDataset\x18\x07 \x01(\t\x12\x13\n\x0btestDataset\x18\x08 \x01(\t\x12\x19\n\x11validationDataset\x18\t \x01(\t\"`\n\rDataStageSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07labName\x18\x02 \x01(\t\x12\x18\n\x10\x64\x61tapipelineName\x18\x03 \x01(\t\x12\x13\n\x0b\x64ockerImage\x18\x04 \x01(\t\"\xa5\x01\n\x12\x44\x65\x65pEstimatorLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12^\n\nparameters\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NNLayerParameter\x12\x13\n\x0binputLayers\x18\x04 \x03(\t\"\xe6\x01\n\x11\x44\x65\x65pEstimatorSpec\x12\\\n\x06layers\x18\x01 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorLayer\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x11\n\tbatchSize\x18\x03 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x04 \x01(\x05\x12\x17\n\x0fvalidationSplit\x18\x05 \x01(\x05\x12\r\n\x05isSeq\x18\x06 \x01(\x08\x12\x0c\n\x04gpus\x18\x07 \x01(\x05\x12\x0c\n\x04loss\x18\x08 \x01(\t\"\x8e\x02\n\x13\x44\x65ploymentStageSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\x0fservingSiteName\x18\x02 \x01(\t\x12\x16\n\x0emanualApproval\x18\x03 \x01(\x08\x12[\n\tunitTests\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelTestSuite\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\".\n\x13\x44riftDetectorStatus\x12\x17\n\x0foutlierModelURI\x18\x01 \x01(\t\";\n\x0e\x44riftModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10outlierAlgorithm\x18\x02 \x01(\t\"R\n\rEarlyStopSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07initial\x18\x02 \x01(\x05\x12\x1f\n\x17minModelsWithNoProgress\x18\x03 \x01(\x05\"\x0f\n\rEnsembleRules\"\xf3\x01\n\x0c\x45nsembleSpec\x12\x0e\n\x06models\x18\x01 \x03(\t\x12\x64\n\nestimators\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12_\n\x05\x66inal\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x0c\n\x04type\x18\x04 \x01(\t\"_\n\rEnsemblesSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0evotingEnsemble\x18\x02 \x01(\x08\x12\x18\n\x10stackingEnsemble\x18\x03 \x01(\x08\x12\x0b\n\x03top\x18\x04 \x01(\x05\"\x89\x01\n\x0b\x45valMetrics\x12\x11\n\tselection\x18\x01 \x01(\t\x12\x11\n\treporting\x18\x02 \x03(\t\x12\x0f\n\x07\x61ggFunc\x18\x03 \x01(\t\x12\x11\n\taggPeriod\x18\x04 \x01(\x05\x12\x17\n\x0fnullModelParams\x18\x05 \x01(\t\x12\x17\n\x0frelErrTolerance\x18\x06 \x01(\x01\"\xe0\x01\n\nEvalPeriod\x12\x13\n\x0btestHorizon\x18\x01 \x01(\x05\x12\x1f\n\x17periodsBetweenTrainTest\x18\x02 \x01(\x05\x12\x1e\n\x16\x63vPeriodsBetweenSplits\x18\x03 \x01(\x05\x12\x1a\n\x12\x63vExpandingWindows\x18\x04 \x01(\x08\x12\x11\n\tcvHorizon\x18\x05 \x01(\x05\x12\x19\n\x11\x63vMinTrainPeriods\x18\x06 \x01(\x05\x12\x13\n\x0b\x63vMaxSplits\x18\x07 \x01(\x05\x12\x1d\n\x15\x63vUseMostRecentSplits\x18\x08 \x01(\x08\"\xc7\x06\n\x1a\x46\x65\x61tureEngineeringPipeline\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\x12\x12\n\nimputation\x18\x04 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x05 \x01(\t\x12\x0f\n\x07scaling\x18\x06 \x01(\t\x12\x16\n\x0e\x64iscretisation\x18\x07 \x01(\t\x12\x1e\n\x16variableTransformation\x18\x08 \x01(\t\x12\x17\n\x0foutlierHandling\x18\t \x01(\t\x12\x1e\n\x16\x64\x61tetimeTransformation\x18\n \x01(\t\x12X\n\x04text\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TextPipelineSpec\x12Z\n\x05image\x18\x0c \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImagePipelineSpec\x12Z\n\x05\x61udio\x18\r \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AudioPipelineSpec\x12Z\n\x05video\x18\x0e \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.VideoPipelineSpec\x12`\n\tgenerated\x18\x10 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GeneratedColumnSpec\x12]\n\x06\x63ustom\x18\x11 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GeneratedColumnSpec\x12\x0c\n\x04\x64rop\x18\x12 \x01(\x08\x12\x13\n\x0bpassthrough\x18\x13 \x01(\x08\"\x9a\x03\n\x1c\x46\x65\x61tureEngineeringSearchSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x19\n\x11imbalancedHandler\x18\x02 \x01(\t\x12\x11\n\testimator\x18\x03 \x01(\t\x12\x11\n\tmaxModels\x18\x04 \x01(\x05\x12\x0f\n\x07maxTime\x18\x05 \x01(\x05\x12\x13\n\x0bmaxTrainers\x18\x06 \x01(\x05\x12\x11\n\tsamplePct\x18\x07 \x01(\x05\x12\x12\n\nautoRemove\x18\x08 \x01(\x08\x12\r\n\x05reuse\x18\t \x01(\x08\x12p\n\x18\x66\x65\x61tureSelectionTemplate\x18\n \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\"\x80\x01\n\x1e\x46\x65\x61tureEngineeringSearchStatus\x12^\n\x04\x62\x65st\x18\x01 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\"\xf7\x01\n\x16\x46\x65\x61tureEngineeringSpec\x12g\n\tpipelines\x18\x01 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringPipeline\x12\x11\n\timbalance\x18\x02 \x01(\t\x12\x61\n\tselection\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\"8\n\x11\x46\x65\x61tureImportance\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x01\":\n\x0b\x46\x65\x61tureInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"#\n\x0b\x46\x65\x61turePair\x12\t\n\x01x\x18\x01 \x01(\t\x12\t\n\x01y\x18\x02 \x01(\t\"\xdd\x01\n\x14\x46\x65\x61tureSelectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tembedding\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\x08\x12\x0f\n\x07wrapper\x18\x05 \x01(\x08\x12\x10\n\x08pipeline\x18\x06 \x03(\t\x12\x1c\n\x14varianceThresholdPct\x18\x07 \x01(\x05\x12\x15\n\rcorrThreshold\x18\x08 \x01(\x05\x12\x13\n\x0bmaxFeatures\x18\t \x01(\x05\x12\x12\n\npercentile\x18\n \x01(\x05\x12\x10\n\x08reserved\x18\x0c \x03(\t\"\xd4\x07\n\x0e\x46orecasterSpec\x12Y\n\x06\x65vents\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TimeSeriesEvent\x12R\n\x04past\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12T\n\x06\x66uture\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12\x10\n\x08\x63overage\x18\x06 \x01(\x01\x12Z\n\x0eoutputLocation\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x10\n\x08\x66\x65\x61tures\x18\x08 \x03(\t\x12\x0e\n\x06groups\x18\t \x03(\t\x12\x1a\n\x12predefinedTemplate\x18\n \x01(\t\x12T\n\tanomalies\x18\x0b \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Anomaly\x12\x14\n\x0ctrainEndData\x18\x0c \x01(\t\x12\x13\n\x0bvalueColumn\x18\r \x01(\t\x12\x11\n\thpoBudget\x18\x0e \x01(\x05\x12`\n\x11\x65valuationMetrics\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalMetrics\x12^\n\x10\x65valuationPeriod\x18\x10 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalPeriod\x12^\n\x0bseasonality\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalitySpec\x12\x12\n\nregressors\x18\x12 \x03(\t\x12\x18\n\x10laggedRegressors\x18\x13 \x03(\t\x12\x0e\n\x06growth\x18\x14 \x01(\t\x12\x0b\n\x03key\x18\x15 \x03(\t\"s\n\x15GarbageCollectionSpec\x12\x19\n\x11\x63ollectAtStudyEnd\x18\x01 \x01(\x08\x12%\n\x1dkeepOnlyBestModelPerAlgorithm\x18\x02 \x01(\x08\x12\x18\n\x10keepPrunedModels\x18\x03 \x01(\x08\"\x83\x01\n\x17GarbageCollectionStatus\x12\x11\n\tcollected\x18\x01 \x01(\x05\x12U\n\x06models\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelResult\"f\n\x13GeneratedColumnSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x66irst\x18\x03 \x01(\t\x12\x0e\n\x06second\x18\x04 \x01(\t\x12\x10\n\x08original\x18\x05 \x01(\t\"2\n\x13HyperParameterValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"o\n\x10HyperbandOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x14\n\x0cmaxResources\x18\x02 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"\'\n\x11ImagePipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\";\n\x15ImbalanceHandlingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\timbalance\x18\x02 \x01(\t\"\x9a\x02\n\x14InterpretabilitySpec\x12\x0b\n\x03ice\x18\x01 \x01(\x08\x12W\n\x08icepairs\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x0c\n\x04lime\x18\x03 \x01(\x08\x12\x0c\n\x04shap\x18\x04 \x01(\t\x12X\n\tshappairs\x18\x05 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x16\n\x0e\x63ounterfactual\x18\x06 \x01(\x08\x12\x0e\n\x06\x61nchor\x18\x07 \x01(\x08\"\xd2\x02\n\x16InterpretabilityStatus\x12\x45\n\x11trainingStartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x0ftrainingEndTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x14\n\x0c\x65xplainerURI\x18\x03 \x01(\t\x12\x1a\n\x12trainShapValuesURI\x18\x04 \x01(\t\x12\x19\n\x11testShapValuesURI\x18\x05 \x01(\t\x12_\n\nimportance\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\"V\n\x05Level\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05index\x18\x02 \x03(\t\x12\x0f\n\x07horizon\x18\x03 \x01(\x05\x12\x0c\n\x04\x66req\x18\x04 \x01(\t\x12\x11\n\taggregate\x18\x05 \x01(\t\"k\n\x13MedianPrunerOptions\x12\x15\n\rstartupTrials\x18\x01 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x02 \x01(\x05\x12\x15\n\rintervalSteps\x18\x03 \x01(\x05\x12\x11\n\tminTrials\x18\x04 \x01(\x05\"\xf5\x01\n\x05Model\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStatus\"\x96\x02\n\x10ModelAutobuilder\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12\\\n\x04spec\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelAutobuilderSpec\x12`\n\x06status\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelAutobuilderStatus\"\xa2\x01\n\x19ModelAutobuilderCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xb3\x01\n\x14ModelAutobuilderList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Y\n\x05items\x18\x02 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelAutobuilder\"\xbe\x06\n\x14ModelAutobuilderSpec\x12\x17\n\x0f\x64\x61taProductName\x18\x01 \x01(\t\x12\x1e\n\x16\x64\x61taProductVersionName\x18\x02 \x01(\t\x12\x16\n\x0e\x64\x61tasourceName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x04 \x01(\t\x12T\n\x08location\x18\x05 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x0c\n\x04task\x18\x06 \x01(\t\x12\x0f\n\x07subtask\x18\x07 \x01(\t\x12\x11\n\tobjective\x18\x08 \x01(\t\x12\x14\n\x0ctargetColumn\x18\t \x01(\t\x12\x0f\n\x07maxTime\x18\n \x01(\x05\x12\x11\n\tmaxModels\x18\x0b \x01(\x05\x12\x14\n\x0c\x61\x63\x63\x65ssMethod\x18\x0c \x01(\t\x12\x11\n\tautoScale\x18\r \x01(\x08\x12\x1a\n\x12\x66\x65\x61tureEngineering\x18\x0e \x01(\x08\x12\x18\n\x10\x66\x65\x61tureSelection\x18\x0f \x01(\x08\x12\x0f\n\x07\x64\x61taapp\x18\x10 \x01(\x08\x12\\\n\x0e\x64\x61taSourceSpec\x18\x11 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceSpec\x12\x10\n\x08trainers\x18\x12 \x01(\x05\x12\x0f\n\x07sampler\x18\x13 \x01(\t\x12\x0f\n\x07\x61\x62orted\x18\x14 \x01(\x08\x12\r\n\x05owner\x18\x15 \x01(\t\x12X\n\tresources\x18\x16 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x33\n\x06labRef\x18\x17 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12;\n\x0eservingSiteRef\x18\x18 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetType\x18\x19 \x01(\t\x12\x0c\n\x04\x66\x61st\x18\x1a \x01(\x08\"\x9a\x06\n\x16ModelAutobuilderStatus\x12\x14\n\x0c\x66latFileName\x18\x01 \x01(\t\x12\x16\n\x0e\x64\x61taSourceName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x11\n\tstudyName\x18\x04 \x01(\t\x12\x15\n\rbestModelName\x18\x06 \x01(\t\x12\x15\n\rpredictorName\x18\x07 \x01(\t\x12\x13\n\x0b\x64\x61taappName\x18\x08 \x01(\t\x12\x15\n\rimageRepoName\x18\t \x01(\t\x12\r\n\x05phase\x18\n \x01(\t\x12\x0c\n\x04rows\x18\x0b \x01(\x05\x12\x0c\n\x04\x63ols\x18\x0c \x01(\x05\x12\x10\n\x08\x66ileSize\x18\r \x01(\x05\x12\x0e\n\x06models\x18\x0e \x01(\x05\x12\x15\n\rtrainedModels\x18\x0f \x01(\x05\x12\x16\n\x0e\x62\x65stModelScore\x18\x10 \x01(\x01\x12\x63\n\testimator\x18\x11 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12=\n\tstartTime\x18\x12 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x13 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x15 \x01(\x03\x12\x15\n\rfailureReason\x18\x16 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x17 \x01(\t\x12?\n\x0blastUpdated\x18\x18 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12g\n\nconditions\x18\x19 \x03(\x0b\x32S.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelAutobuilderCondition\"\x96\x02\n\x10ModelCompilerRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12\\\n\x04spec\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelCompilerRunSpec\x12`\n\x06status\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelCompilerRunStatus\"\xa2\x01\n\x19ModelCompilerRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xb3\x01\n\x14ModelCompilerRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Y\n\x05items\x18\x02 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelCompilerRun\"\x96\x01\n\x14ModelCompilerRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x11\n\tmodelName\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12\x10\n\x08priority\x18\x05 \x01(\t\x12\x10\n\x08\x63ompiler\x18\x06 \x01(\t\x12\x0e\n\x06target\x18\x07 \x01(\t\"\xc6\x03\n\x16ModelCompilerRunStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x42\n\x0e\x63ompletionTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x03 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x05 \x01(\t\x12\x15\n\rfailureReason\x18\x06 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x10\n\x08progress\x18\x08 \x01(\x05\x12?\n\x0blastUpdated\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12g\n\nconditions\x18\n \x03(\x0b\x32S.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelCompilerRunCondition\"\x97\x01\n\x0eModelCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xb1\x01\n\x12ModelGroupByStatus\x12\x11\n\tmodelsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x12\n\nreportsURI\x18\x03 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"R\n\x0eModelImageSpec\x12\r\n\x05\x65xist\x18\x01 \x01(\x08\x12\x11\n\timageName\x18\x02 \x01(\t\x12\x1e\n\x16registryConnectionName\x18\x03 \x01(\t\"\x9d\x01\n\tModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x8d\x02\n\rModelPipeline\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Y\n\x04spec\x18\x02 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineSpec\x12]\n\x06status\x18\x03 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineStatus\"\x9f\x01\n\x16ModelPipelineCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x0f\n\x07message\x18\x05 \x01(\t\"\xad\x01\n\x11ModelPipelineList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12V\n\x05items\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipeline\"\x96\x02\n\x10ModelPipelineRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12\\\n\x04spec\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunSpec\x12`\n\x06status\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStatus\"\xa2\x01\n\x19ModelPipelineRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xb3\x01\n\x14ModelPipelineRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Y\n\x05items\x18\x02 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRun\"\xba\x01\n\x14ModelPipelineRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x14\n\x0cpipelineName\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x0b\n\x03ttl\x18\t \x01(\x05\"\x80\x03\n\x1bModelPipelineRunStageStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12\x10\n\x08\x61pproved\x18\x02 \x01(\x08\x12\x12\n\napprovedBy\x18\x03 \x01(\t\x12>\n\napprovedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\tstartTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05\x65rror\x18\n \x01(\t\"\xaa\x0b\n\x16ModelPipelineRunStatus\x12\r\n\x05stage\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x02 \x01(\t\x12\x11\n\tstudyName\x18\x03 \x01(\t\x12\x11\n\tmodelName\x18\x04 \x01(\t\x12\x63\n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12g\n\x08training\x18\x06 \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12\x62\n\x03uat\x18\x07 \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12g\n\x08\x63\x61pacity\x18\x08 \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12i\n\ndeployment\x18\t \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12\x66\n\x07release\x18\n \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12\x66\n\x07monitor\x18\x0b \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12g\n\x08labeling\x18\x0c \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunStageStatus\x12=\n\tstartTime\x18\r \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x0f \x01(\t\x12\x1a\n\x12observedGeneration\x18\x10 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x11 \x01(\t\x12\x15\n\rfailureReason\x18\x12 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x13 \x01(\t\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12\x13\n\x0btriggeredBy\x18\x15 \x01(\t\x12?\n\x0blastUpdated\x18\x16 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\x17 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12g\n\nconditions\x18\x18 \x03(\x0b\x32S.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineRunCondition\"\xbc\x08\n\x11ModelPipelineSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12y\n\x0f\x64\x61tasetSelector\x18\x03 \x03(\x0b\x32`.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineSpec.DatasetSelectorEntry\x12U\n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataStageSpec\x12]\n\x08training\x18\x05 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingStageSpec\x12S\n\x03uat\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.UATStageSpec\x12]\n\x08\x63\x61pacity\x18\x07 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CapacityStageSpec\x12\x61\n\ndeployment\x18\t \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeploymentStageSpec\x12[\n\x07release\x18\n \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReleaseStageSpec\x12V\n\x08schedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\r\n\x05owner\x18\r \x01(\t\x12\x1b\n\x13\x61pproverAccountName\x18\x0e \x01(\t\x12_\n\x0cnotification\x18\x0f \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\x19\n\x11\x62\x61selineModelName\x18\x10 \x01(\t\x12\x10\n\x08priority\x18\x11 \x01(\t\x12\x0e\n\x06paused\x18\x12 \x01(\x08\x1a\x36\n\x14\x44\x61tasetSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9d\x03\n\x13ModelPipelineStatus\x12W\n\x07lastRun\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12?\n\x0blastUpdated\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x64\n\nconditions\x18\x07 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelPipelineCondition\"W\n\x0bModelResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03\x61lg\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x01\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x0f\n\x07trialID\x18\x05 \x01(\x05\"\xca\x10\n\tModelSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x04 \x01(\t\x12\x11\n\tstudyName\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x06 \x01(\t\x12\x0c\n\x04task\x18\x07 \x01(\t\x12\x0f\n\x07subtask\x18\x08 \x01(\t\x12\x11\n\tobjective\x18\t \x01(\t\x12l\n\x12\x66\x65\x61tureEngineering\x18\n \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12\x63\n\testimator\x18\x0b \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12X\n\x03\x64nn\x18\x0c \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorSpec\x12_\n\x07\x63hatbot\x18\r \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ChatbotEstimatorSpec\x12`\n\x0cnlpEstimator\x18\x0e \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NLPEstimatorSpec\x12X\n\x08\x65nsemble\x18\x0f \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsembleSpec\x12X\n\x08training\x18\x10 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12V\n\x07serving\x18\x11 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12\x0e\n\x06tested\x18\x12 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x13 \x01(\x08\x12\x10\n\x08packaged\x18\x14 \x01(\x08\x12\x11\n\tpublished\x18\x15 \x01(\x08\x12\x0e\n\x06pushed\x18\x16 \x01(\x08\x12\x10\n\x08reported\x18\x17 \x01(\x08\x12\x0e\n\x06paused\x18\x18 \x01(\x08\x12\x10\n\x08profiled\x18\x19 \x01(\x08\x12\x10\n\x08\x61rchived\x18\x1a \x01(\x08\x12\x12\n\nforecasted\x18\x1b \x01(\x08\x12\x10\n\x08released\x18\x1c \x01(\x08\x12\x12\n\nregistered\x18\x1d \x01(\x08\x12\x0f\n\x07predict\x18\x1e \x01(\x08\x12\r\n\x05tuned\x18\x1f \x01(\x08\x12\x11\n\texplained\x18  \x01(\x08\x12\x15\n\rcodeGenerated\x18! \x01(\x08\x12\x10\n\x08\x62\x61seline\x18\" \x01(\x08\x12\x18\n\x10genDriftDetector\x18# \x01(\x08\x12\x0c\n\x04\x66\x61st\x18$ \x01(\x08\x12\x12\n\nunitTested\x18% \x01(\x08\x12?\n\x12\x66\x65\x65\x64\x62\x61\x63kDatasetRef\x18& \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x66lagged\x18\' \x01(\x08\x12T\n\x08location\x18( \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12]\n\x0b\x66orecasting\x18) \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12Z\n\x0b\x63ompilation\x18* \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CompilerSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18+ \x01(\x03\x12\x15\n\restimatorType\x18, \x01(\t\x12\x0b\n\x03ttl\x18- \x01(\x05\x12\x12\n\nmodelClass\x18. \x01(\t\x12\x0f\n\x07trialID\x18/ \x01(\x05\x12X\n\ngovernance\x18\x30 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GovernanceSpec\x12h\n\x10interpretability\x18\x31 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12U\n\tunitTests\x18\x32 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12Y\n\rfeedbackTests\x18\x33 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\xc3\x1f\n\x0bModelStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x45\n\x11trainingStartTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x0ftrainingEndTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x44\n\x10testingStartTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x42\n\x0etestingEndTime\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x0ftuningStartTime\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x41\n\rtuningEndTime\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0f\n\x07\x63vScore\x18\t \x01(\x01\x12\x15\n\rtrainingScore\x18\n \x01(\x01\x12\x11\n\ttestScore\x18\x0b \x01(\x01\x12\x0c\n\x04\x63ost\x18\x0c \x01(\x01\x12\x0c\n\x04\x62\x65st\x18\r \x01(\x08\x12P\n\x02\x63v\x18\x0e \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12S\n\x05train\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04test\x18\x10 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04tune\x18\x11 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12V\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x12 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x43\n\x16lastFeedbackDatasetRef\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\r\n\x05phase\x18\x14 \x01(\t\x12\x12\n\nreportName\x18\x15 \x01(\t\x12\x11\n\treportUri\x18\x16 \x01(\t\x12\x13\n\x0bmanifestUri\x18\x17 \x01(\t\x12\x12\n\nweightsUri\x18\x18 \x01(\t\x12\x17\n\x0flabelEncoderUri\x18\x19 \x01(\t\x12\x0f\n\x07logsUri\x18\x1a \x01(\t\x12\x12\n\nprofileUri\x18\x1b \x01(\t\x12\x1c\n\x14misclassificationUri\x18\x1c \x01(\t\x12\x0e\n\x06tarUri\x18\x1d \x01(\t\x12\x0e\n\x06\x61ppUri\x18\x1e \x01(\t\x12\x11\n\timageName\x18\x1f \x01(\t\x12_\n\nimportance\x18  \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12j\n\x15permutationImportance\x18! \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12\x13\n\x0b\x66orecastUri\x18\" \x01(\t\x12X\n\x07runtime\x18# \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus\x12X\n\x0ctrainDataset\x18$ \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12W\n\x0btestDataset\x18% \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12]\n\x11validationDataset\x18& \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x1a\n\x12observedGeneration\x18\' \x01(\x03\x12\x14\n\x0ctrainingRows\x18( \x01(\x05\x12\x13\n\x0btestingRows\x18) \x01(\x05\x12\x16\n\x0evalidationRows\x18* \x01(\x05\x12\x15\n\rfailureReason\x18+ \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18, \x01(\t\x12\x10\n\x08progress\x18- \x01(\x05\x12\x13\n\x0bsizeInBytes\x18. \x01(\x05\x12\x0f\n\x07latency\x18/ \x01(\x01\x12\x0b\n\x03url\x18\x30 \x01(\t\x12\x15\n\rpredictorName\x18\x31 \x01(\t\x12>\n\nreleasedAt\x18\x32 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0bpredictedAt\x18\x33 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0btarFileHash\x18\x34 \x01(\t\x12\x11\n\timageHash\x18\x35 \x01(\t\x12^\n\x10trainingDataHash\x18\x36 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12h\n\x11trainingResources\x18\x37 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ResourceConsumption\x12g\n\x10testingResources\x18\x38 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ResourceConsumption\x12\x11\n\ttrainedBy\x18\x39 \x01(\t\x12\x0c\n\x04team\x18: \x01(\t\x12\x10\n\x08\x65ndpoint\x18; \x01(\t\x12K\n\x04logs\x18< \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12V\n\x08rocCurve\x18= \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RocAucCurve\x12Q\n\x07prCurve\x18> \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PRCurve\x12\x66\n\x14trainConfusionMatrix\x18? \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18@ \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x61\n\x16\x63orrelationsWithTarget\x18\x41 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18\x42 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12?\n\x0blastUpdated\x18\x43 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x10governanceStatus\x18\x44 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GovernanceStatus\x12j\n\x10interpretability\x18\x45 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilityStatus\x12O\n\x06images\x18\x46 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12\x61\n\x0funitTestsResult\x18G \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x65\n\x13\x66\x65\x65\x64\x62\x61\x63kTestsResult\x18H \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x14\n\x0csubModelsURI\x18I \x01(\t\x12\\\n\nconditions\x18J \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelCondition\"\xdf\x01\n\x0eModelTestSuite\x12=\n\x10\x62\x61selineModelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\ndatasetRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\" \n\x10NLPEstimatorSpec\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"/\n\x10NNLayerParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xfe\x01\n\x08Notebook\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookStatus\"\x9a\x01\n\x11NotebookCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xa3\x01\n\x0cNotebookList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Notebook\"\x87\x02\n\x0bNotebookRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookRunSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookRunStatus\"\x9d\x01\n\x14NotebookRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xa9\x01\n\x0fNotebookRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookRun\"\xc3\x02\n\x0fNotebookRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x14\n\x0cnotebookName\x18\x02 \x01(\t\x12Z\n\x06values\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookVarValue\x12\r\n\x05owner\x18\x04 \x01(\t\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03ttl\x18\x06 \x01(\x05\x12\x33\n\x06labRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xf0\x03\n\x11NotebookRunStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x13\n\x0btriggeredBy\x18\x07 \x01(\t\x12K\n\x04logs\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12?\n\x0blastUpdated\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x62\n\nconditions\x18\n \x03(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookRunCondition\"\xeb\x04\n\x0cNotebookSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x36\n\tschemaRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x11\n\timageName\x18\x04 \x01(\t\x12\x14\n\x0crequirements\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65\x62Packages\x18\x06 \x01(\t\x12\x0c\n\x04vars\x18\x07 \x03(\t\x12T\n\x08location\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\r\n\x05owner\x18\t \x01(\t\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x0b \x01(\x03\x12V\n\x08schedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x10\n\x08priority\x18\r \x01(\t\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12U\n\tunitTests\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\xe3\x03\n\x0eNotebookStatus\x12\r\n\x05image\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12W\n\x07lastRun\x18\x04 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12;\n\x07nextRun\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0blastUpdated\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\x07 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12_\n\nconditions\x18\t \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NotebookCondition\"/\n\x10NotebookVarValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x84\x01\n\x17PercentilePrunerOptions\x12\x12\n\npercentile\x18\x01 \x01(\x05\x12\x15\n\rstartupTrials\x18\x02 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x16\n\x0eintervalTrials\x18\x04 \x01(\x05\x12\x11\n\tminTrials\x18\x05 \x01(\x05\"\x93\x04\n\nPrunerSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12]\n\x06median\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.MedianPrunerOptions\x12\x65\n\npercentile\x18\x03 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PercentilePrunerOptions\x12m\n\x11successiveHalving\x18\x04 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingOptions\x12]\n\thyperband\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperbandOptions\x12\x63\n\tthreshold\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ThresholdPrunerOptions\"\xd0\x01\n\x18RegressionForecasterSpec\x12\x10\n\x08\x65nsemble\x18\x01 \x01(\x08\x12\x12\n\nimputation\x18\x02 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x0f\n\x07scaling\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\x08\x12\x0f\n\x07windows\x18\x06 \x03(\x05\x12\x0c\n\x04lags\x18\x07 \x03(\x05\x12\x11\n\tfunctions\x18\x08 \x03(\t\x12\x0b\n\x03\x65ma\x18\t \x01(\x08\x12\x0b\n\x03log\x18\n \x01(\x08\x12\x11\n\treduction\x18\x0b \x01(\t\"\xa5\x02\n\x10ReleaseStageSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\x0fservingSiteName\x18\x02 \x01(\t\x12\x15\n\rpredictorName\x18\x03 \x01(\t\x12^\n\x08template\x18\x04 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ModelDeploymentSpec\x12\x16\n\x0emanualApproval\x18\x05 \x01(\x08\x12X\n\tresources\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\"\xf8\x01\n\x06Report\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportStatus\"\x98\x01\n\x0fReportCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\x9f\x01\n\nReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xa7\x04\n\nReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x36\n\tentityRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12T\n\x08location\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x12\n\nreportType\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x06 \x01(\t\x12\x14\n\x0cnotifierName\x18\x07 \x01(\t\x12\r\n\x05owner\x18\x08 \x01(\t\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\n \x01(\x03\x12Z\n\x06\x63ustom\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CustomReportSpec\x12\x16\n\x0e\x63ronReportName\x18\x0c \x01(\t\x12\x33\n\x06labRef\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03key\x18\x0e \x03(\t\"\xde\x03\n\x0cReportStatus\x12=\n\tstartTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x04 \x01(\t\x12\x0b\n\x03uri\x18\x05 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x06 \x01(\x03\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12K\n\x04logs\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12?\n\x0blastUpdated\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12]\n\nconditions\x18\x0b \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportCondition\"d\n\x0eReportTemplate\x12R\n\x04spec\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\"<\n\x13ResourceConsumption\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x01\x12\x0b\n\x03mem\x18\x02 \x01(\x01\x12\x0b\n\x03gpu\x18\x03 \x01(\x01\"\xf1\x01\n\rRuntimeStatus\x12\x15\n\rpythonVersion\x18\x01 \x01(\t\x12\x11\n\tpythonCmd\x18\x02 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12s\n\x0epythonPackages\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus.PythonPackagesEntry\x1a\x35\n\x13PythonPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x80\x04\n\nSearchSpec\x12\x0f\n\x07sampler\x18\x01 \x01(\t\x12T\n\x06pruner\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PrunerSpec\x12\x0f\n\x07maxCost\x18\x03 \x01(\x05\x12\x0f\n\x07maxTime\x18\x04 \x01(\x05\x12\x11\n\tmaxModels\x18\x05 \x01(\x05\x12\x14\n\x0cminBestScore\x18\x06 \x01(\x01\x12\x10\n\x08trainers\x18\x07 \x01(\x05\x12\x0c\n\x04test\x18\x08 \x01(\x05\x12\x11\n\tretainTop\x18\t \x01(\x05\x12\x13\n\x0bretainedFor\x18\n \x01(\x05\x12g\n\x0bsearchSpace\x18\x0b \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\x12\x11\n\tobjective\x18\x0e \x01(\t\x12\x12\n\nobjective2\x18\x0f \x01(\t\x12\x0c\n\x04tune\x18\x10 \x01(\x08\"L\n\x15SeasonalityPeriodSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x61uto\x18\x02 \x01(\x08\x12\x14\n\x0c\x66ourierOrder\x18\x03 \x01(\x05\"\x87\x04\n\x0fSeasonalitySpec\x12\x0c\n\x04\x61uto\x18\x01 \x01(\x08\x12_\n\x06yearly\x18\x02 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12\x62\n\tquarterly\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12`\n\x07monthly\x18\x04 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12_\n\x06weekly\x18\x05 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12^\n\x05\x64\x61ily\x18\x06 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\"<\n\x0bSegmentSpec\x12\x12\n\ncolumnName\x18\x01 \x01(\t\x12\n\n\x02op\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"w\n\x0bServingSpec\x12X\n\tresources\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"\xf5\x01\n\x05Study\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudySpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyStatus\"\x97\x01\n\x0eStudyCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\x89\x01\n\x12StudyGroupByStatus\x12\x12\n\nstudiesURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\tStudyList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\x84\x02\n\x10StudyPhaseStatus\x12=\n\tstartTime\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0f\n\x07waiting\x18\x03 \x01(\x05\x12\x0f\n\x07running\x18\x04 \x01(\x05\x12\x0e\n\x06\x66\x61iled\x18\x05 \x01(\x05\x12\x11\n\tcompleted\x18\x06 \x01(\x05\x12\x11\n\tbestScore\x18\x07 \x01(\x01\x12\x1c\n\x14modelsWithNoProgress\x18\x08 \x01(\x05\"a\n\x11StudyScheduleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12;\n\x07startAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\x98\x10\n\tStudySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetName\x18\x04 \x01(\t\x12\x0c\n\x04task\x18\x05 \x01(\t\x12\x0f\n\x07subtask\x18\x06 \x01(\t\x12h\n\x08\x66\x65Search\x18\x07 \x01(\x0b\x32V.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSearchSpec\x12i\n\x10imbalanceHandler\x18\x08 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImbalanceHandlingSpec\x12X\n\x08\x62\x61seline\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.BaselineSpec\x12T\n\x06search\x18\n \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SearchSpec\x12Z\n\tensembles\x18\x0b \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsemblesSpec\x12`\n\x10trainingTemplate\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12^\n\x0fservingTemplate\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12]\n\x0b\x66\x63tTemplate\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12]\n\x08schedule\x18\x0f \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyScheduleSpec\x12h\n\x10interpretability\x18\x10 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12`\n\x0e\x64riftDetection\x18\x11 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftModelSpec\x12\x0f\n\x07\x61\x62orted\x18\x12 \x01(\x08\x12\x10\n\x08reported\x18\x13 \x01(\x08\x12\x0e\n\x06paused\x18\x14 \x01(\x08\x12\x10\n\x08profiled\x18\x15 \x01(\x08\x12\x16\n\x0emodelPublished\x18\x16 \x01(\x08\x12\x18\n\x10modelImagePushed\x18\x17 \x01(\x08\x12\x16\n\x0emodelExplained\x18\x18 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x19 \x01(\x08\x12T\n\x08location\x18\x1a \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\r\n\x05owner\x18\x1b \x01(\t\x12Z\n\x0b\x63ompilation\x18\x1c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CompilerSpec\x12\x10\n\x08template\x18\x1d \x01(\x08\x12\x0f\n\x07\x66lagged\x18\x1e \x01(\x08\x12_\n\x0cnotification\x18\x1f \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\nmodelImage\x18  \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelImageSpec\x12[\n\x02gc\x18! \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionSpec\x12\x0b\n\x03ttl\x18\" \x01(\x05\x12\x14\n\x0cmodelVersion\x18# \x01(\t\x12\x15\n\rtimeoutInSecs\x18$ \x01(\x05\x12\x15\n\rcodeGenerated\x18% \x01(\x08\x12]\n\x11unitTestsTemplate\x18& \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\xf8\x0f\n\x0bStudyStatus\x12\x0e\n\x06models\x18\x01 \x01(\x05\x12=\n\tstartTime\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12;\n\x07\x65ndTime\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tbestModel\x18\x04 \x01(\t\x12\x16\n\x0e\x62\x65stModelScore\x18\x05 \x01(\x01\x12\x12\n\nprofileUri\x18\x06 \x01(\t\x12\x11\n\treportUri\x18\x07 \x01(\t\x12\x12\n\nreportName\x18\x08 \x01(\t\x12\r\n\x05phase\x18\t \x01(\t\x12\x1a\n\x12observedGeneration\x18\n \x01(\x03\x12X\n\x0ctrainDataset\x18\x0b \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12W\n\x0btestDataset\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12]\n\x11validationDataset\x18\r \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataLocation\x12\x13\n\x0blastModelID\x18\x0e \x01(\x03\x12\x15\n\rfailureReason\x18\x0f \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x10 \x01(\t\x12\x14\n\x0ctrainingRows\x18\x11 \x01(\x05\x12\x13\n\x0btestingRows\x18\x12 \x01(\x05\x12\x16\n\x0evalidationRows\x18\x13 \x01(\x05\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12^\n\x10trainingDataHash\x18\x16 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12\x13\n\x0btriggeredBy\x18\x17 \x01(\t\x12K\n\x04logs\x18\x18 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x66\n\x12\x66\x65\x61tureEngineering\x18\x19 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x62\x61seline\x18\x1a \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12Z\n\x06search\x18\x1b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x65nsemble\x18\x1c \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12X\n\x04test\x18\x1d \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12[\n\x07\x65xplain\x18\x1e \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\x65\n\x0e\x64riftDetection\x18\x1f \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftDetectorStatus\x12?\n\x0blastUpdated\x18  \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18! \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12]\n\x02gc\x18\" \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionStatus\x12\x61\n\x0bgroupStatus\x18# \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyGroupByStatus\x12\\\n\nconditions\x18$ \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyCondition\"\x7f\n\x18SuccessiveHalvingOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x02 \x01(\x05\x12\x1c\n\x14minEarlyStoppingRate\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"h\n\x15SuccessiveHalvingSpec\x12\x0e\n\x06\x62udget\x18\x01 \x01(\x05\x12\x0f\n\x07\x62racket\x18\x02 \x01(\x05\x12\x0c\n\x04rung\x18\x03 \x01(\x05\x12\x0e\n\x06\x63onfID\x18\x04 \x01(\x05\x12\x10\n\x08modality\x18\x1a \x01(\t\"\xad\x01\n\x10TextPipelineSpec\x12\x0f\n\x07\x65ncoder\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x02 \x01(\t\x12\x11\n\tstopwords\x18\x03 \x01(\x08\x12\x0b\n\x03pos\x18\x04 \x01(\x08\x12\r\n\x05lemma\x18\x05 \x01(\x08\x12\x0c\n\x04stem\x18\x06 \x01(\x08\x12\x11\n\tembedding\x18\x07 \x01(\t\x12\x0b\n\x03svd\x18\x08 \x01(\x08\x12\x18\n\x10maxSvdComponents\x18\t \x01(\x05\"b\n\x16ThresholdPrunerOptions\x12\r\n\x05lower\x18\x01 \x01(\x01\x12\r\n\x05upper\x18\x02 \x01(\x01\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x15\n\rintervalSteps\x18\x04 \x01(\x05\"\x8a\x01\n\x0fTimeSeriesEvent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0f\n\x07holiday\x18\x03 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x10\n\x08preEvent\x18\x05 \x01(\x05\x12\x11\n\tpostEvent\x18\x06 \x01(\x05\x12\x12\n\ntimePoints\x18\x07 \x03(\t\"\x9c\x05\n\x0cTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08priority\x18\x02 \x01(\t\x12\x0e\n\x06\x63vtype\x18\x03 \x01(\t\x12\n\n\x02\x63V\x18\x04 \x01(\x08\x12\r\n\x05\x66olds\x18\x05 \x01(\x05\x12V\n\x05split\x18\x06 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataSplitSpec\x12\x13\n\x0b\x65valMetrics\x18\x07 \x03(\t\x12[\n\x02sh\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingSpec\x12\x0c\n\x04seed\x18\x0b \x01(\x01\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03gpu\x18\r \x01(\x08\x12\x13\n\x0b\x64istributed\x18\x0e \x01(\x08\x12\x19\n\x11\x66\x65\x61tureImportance\x18\x0f \x01(\x08\x12\x11\n\tnodeCount\x18\x10 \x01(\x05\x12\x11\n\tsamplePct\x18\x11 \x01(\x05\x12\\\n\ncheckpoint\x18\x12 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CheckpointSpec\x12\x10\n\x08logLevel\x18\x13 \x01(\t\x12\x15\n\rtimeoutInSecs\x18\x14 \x01(\x05\"f\n\x11TrainingStageSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x14\n\x0cnotebookName\x18\x02 \x01(\t\x12\x0f\n\x07labName\x18\x03 \x01(\t\x12\x19\n\x11studyTemplateName\x18\x04 \x01(\t\"\xef\x01\n\x0cUATStageSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\x0fservingSiteName\x18\x02 \x01(\t\x12[\n\tunitTests\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelTestSuite\x12X\n\tresources\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\"\xdc\x01\n\x18UnivariateForecastStatus\x12\x1b\n\x13gridSearchResultURI\x18\x01 \x01(\t\x12g\n\rbaseEstimator\x18\x02 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x10\n\x08modelURI\x18\x03 \x01(\t\x12\x13\n\x0b\x63vResultURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x05 \x01(\t\"\'\n\x11VideoPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"=\n\nWindowSpec\x12\x10\n\x08interval\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x0e\n\x06length\x18\x03 \x01(\x05\x42:Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1')
 
 
 
 _ALGORITHMSEARCHSPACESPEC = DESCRIPTOR.message_types_by_name['AlgorithmSearchSpaceSpec']
 _ANOMALY = DESCRIPTOR.message_types_by_name['Anomaly']
 _AUDIOPIPELINESPEC = DESCRIPTOR.message_types_by_name['AudioPipelineSpec']
 _BACKTESTSPEC = DESCRIPTOR.message_types_by_name['BacktestSpec']
@@ -83,15 +83,14 @@
 _MODELCOMPILERRUN = DESCRIPTOR.message_types_by_name['ModelCompilerRun']
 _MODELCOMPILERRUNCONDITION = DESCRIPTOR.message_types_by_name['ModelCompilerRunCondition']
 _MODELCOMPILERRUNLIST = DESCRIPTOR.message_types_by_name['ModelCompilerRunList']
 _MODELCOMPILERRUNSPEC = DESCRIPTOR.message_types_by_name['ModelCompilerRunSpec']
 _MODELCOMPILERRUNSTATUS = DESCRIPTOR.message_types_by_name['ModelCompilerRunStatus']
 _MODELCONDITION = DESCRIPTOR.message_types_by_name['ModelCondition']
 _MODELGROUPBYSTATUS = DESCRIPTOR.message_types_by_name['ModelGroupByStatus']
-_MODELGROUPBYSTATUS_WORKERRESULTSENTRY = _MODELGROUPBYSTATUS.nested_types_by_name['WorkerResultsEntry']
 _MODELIMAGESPEC = DESCRIPTOR.message_types_by_name['ModelImageSpec']
 _MODELLIST = DESCRIPTOR.message_types_by_name['ModelList']
 _MODELPIPELINE = DESCRIPTOR.message_types_by_name['ModelPipeline']
 _MODELPIPELINECONDITION = DESCRIPTOR.message_types_by_name['ModelPipelineCondition']
 _MODELPIPELINELIST = DESCRIPTOR.message_types_by_name['ModelPipelineList']
 _MODELPIPELINERUN = DESCRIPTOR.message_types_by_name['ModelPipelineRun']
 _MODELPIPELINERUNCONDITION = DESCRIPTOR.message_types_by_name['ModelPipelineRunCondition']
@@ -135,14 +134,15 @@
 _SEARCHSPEC = DESCRIPTOR.message_types_by_name['SearchSpec']
 _SEASONALITYPERIODSPEC = DESCRIPTOR.message_types_by_name['SeasonalityPeriodSpec']
 _SEASONALITYSPEC = DESCRIPTOR.message_types_by_name['SeasonalitySpec']
 _SEGMENTSPEC = DESCRIPTOR.message_types_by_name['SegmentSpec']
 _SERVINGSPEC = DESCRIPTOR.message_types_by_name['ServingSpec']
 _STUDY = DESCRIPTOR.message_types_by_name['Study']
 _STUDYCONDITION = DESCRIPTOR.message_types_by_name['StudyCondition']
+_STUDYGROUPBYSTATUS = DESCRIPTOR.message_types_by_name['StudyGroupByStatus']
 _STUDYLIST = DESCRIPTOR.message_types_by_name['StudyList']
 _STUDYPHASESTATUS = DESCRIPTOR.message_types_by_name['StudyPhaseStatus']
 _STUDYSCHEDULESPEC = DESCRIPTOR.message_types_by_name['StudyScheduleSpec']
 _STUDYSPEC = DESCRIPTOR.message_types_by_name['StudySpec']
 _STUDYSTATUS = DESCRIPTOR.message_types_by_name['StudyStatus']
 _SUCCESSIVEHALVINGOPTIONS = DESCRIPTOR.message_types_by_name['SuccessiveHalvingOptions']
 _SUCCESSIVEHALVINGSPEC = DESCRIPTOR.message_types_by_name['SuccessiveHalvingSpec']
@@ -586,27 +586,19 @@
   'DESCRIPTOR' : _MODELCONDITION,
   '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.generated_pb2'
   # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelCondition)
   })
 _sym_db.RegisterMessage(ModelCondition)
 
 ModelGroupByStatus = _reflection.GeneratedProtocolMessageType('ModelGroupByStatus', (_message.Message,), {
-
-  'WorkerResultsEntry' : _reflection.GeneratedProtocolMessageType('WorkerResultsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _MODELGROUPBYSTATUS_WORKERRESULTSENTRY,
-    '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.generated_pb2'
-    # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus.WorkerResultsEntry)
-    })
-  ,
   'DESCRIPTOR' : _MODELGROUPBYSTATUS,
   '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.generated_pb2'
   # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus)
   })
 _sym_db.RegisterMessage(ModelGroupByStatus)
-_sym_db.RegisterMessage(ModelGroupByStatus.WorkerResultsEntry)
 
 ModelImageSpec = _reflection.GeneratedProtocolMessageType('ModelImageSpec', (_message.Message,), {
   'DESCRIPTOR' : _MODELIMAGESPEC,
   '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.generated_pb2'
   # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelImageSpec)
   })
 _sym_db.RegisterMessage(ModelImageSpec)
@@ -959,14 +951,21 @@
 StudyCondition = _reflection.GeneratedProtocolMessageType('StudyCondition', (_message.Message,), {
   'DESCRIPTOR' : _STUDYCONDITION,
   '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.generated_pb2'
   # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyCondition)
   })
 _sym_db.RegisterMessage(StudyCondition)
 
+StudyGroupByStatus = _reflection.GeneratedProtocolMessageType('StudyGroupByStatus', (_message.Message,), {
+  'DESCRIPTOR' : _STUDYGROUPBYSTATUS,
+  '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.generated_pb2'
+  # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyGroupByStatus)
+  })
+_sym_db.RegisterMessage(StudyGroupByStatus)
+
 StudyList = _reflection.GeneratedProtocolMessageType('StudyList', (_message.Message,), {
   'DESCRIPTOR' : _STUDYLIST,
   '__module__' : 'github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.generated_pb2'
   # @@protoc_insertion_point(class_scope:github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyList)
   })
 _sym_db.RegisterMessage(StudyList)
 
@@ -1075,16 +1074,14 @@
   })
 _sym_db.RegisterMessage(WindowSpec)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1'
-  _MODELGROUPBYSTATUS_WORKERRESULTSENTRY._options = None
-  _MODELGROUPBYSTATUS_WORKERRESULTSENTRY._serialized_options = b'8\001'
   _MODELPIPELINESPEC_DATASETSELECTORENTRY._options = None
   _MODELPIPELINESPEC_DATASETSELECTORENTRY._serialized_options = b'8\001'
   _RUNTIMESTATUS_PYTHONPACKAGESENTRY._options = None
   _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_options = b'8\001'
   _ALGORITHMSEARCHSPACESPEC._serialized_start=472
   _ALGORITHMSEARCHSPACESPEC._serialized_end=517
   _ANOMALY._serialized_start=519
@@ -1206,145 +1203,145 @@
   _MODELCOMPILERRUNSPEC._serialized_start=12476
   _MODELCOMPILERRUNSPEC._serialized_end=12626
   _MODELCOMPILERRUNSTATUS._serialized_start=12629
   _MODELCOMPILERRUNSTATUS._serialized_end=13083
   _MODELCONDITION._serialized_start=13086
   _MODELCONDITION._serialized_end=13237
   _MODELGROUPBYSTATUS._serialized_start=13240
-  _MODELGROUPBYSTATUS._serialized_end=13494
-  _MODELGROUPBYSTATUS_WORKERRESULTSENTRY._serialized_start=13442
-  _MODELGROUPBYSTATUS_WORKERRESULTSENTRY._serialized_end=13494
-  _MODELIMAGESPEC._serialized_start=13496
-  _MODELIMAGESPEC._serialized_end=13578
-  _MODELLIST._serialized_start=13581
-  _MODELLIST._serialized_end=13738
-  _MODELPIPELINE._serialized_start=13741
-  _MODELPIPELINE._serialized_end=14010
-  _MODELPIPELINECONDITION._serialized_start=14013
-  _MODELPIPELINECONDITION._serialized_end=14172
-  _MODELPIPELINELIST._serialized_start=14175
-  _MODELPIPELINELIST._serialized_end=14348
-  _MODELPIPELINERUN._serialized_start=14351
-  _MODELPIPELINERUN._serialized_end=14629
-  _MODELPIPELINERUNCONDITION._serialized_start=14632
-  _MODELPIPELINERUNCONDITION._serialized_end=14794
-  _MODELPIPELINERUNLIST._serialized_start=14797
-  _MODELPIPELINERUNLIST._serialized_end=14976
-  _MODELPIPELINERUNSPEC._serialized_start=14979
-  _MODELPIPELINERUNSPEC._serialized_end=15165
-  _MODELPIPELINERUNSTAGESTATUS._serialized_start=15168
-  _MODELPIPELINERUNSTAGESTATUS._serialized_end=15552
-  _MODELPIPELINERUNSTATUS._serialized_start=15555
-  _MODELPIPELINERUNSTATUS._serialized_end=17005
-  _MODELPIPELINESPEC._serialized_start=17008
-  _MODELPIPELINESPEC._serialized_end=18092
-  _MODELPIPELINESPEC_DATASETSELECTORENTRY._serialized_start=18038
-  _MODELPIPELINESPEC_DATASETSELECTORENTRY._serialized_end=18092
-  _MODELPIPELINESTATUS._serialized_start=18095
-  _MODELPIPELINESTATUS._serialized_end=18508
-  _MODELRESULT._serialized_start=18510
-  _MODELRESULT._serialized_end=18597
-  _MODELSPEC._serialized_start=18600
-  _MODELSPEC._serialized_end=20722
-  _MODELSTATUS._serialized_start=20725
-  _MODELSTATUS._serialized_end=24760
-  _MODELTESTSUITE._serialized_start=24763
-  _MODELTESTSUITE._serialized_end=24986
-  _NLPESTIMATORSPEC._serialized_start=24988
-  _NLPESTIMATORSPEC._serialized_end=25020
-  _NNLAYERPARAMETER._serialized_start=25022
-  _NNLAYERPARAMETER._serialized_end=25069
-  _NOTEBOOK._serialized_start=25072
-  _NOTEBOOK._serialized_end=25326
-  _NOTEBOOKCONDITION._serialized_start=25329
-  _NOTEBOOKCONDITION._serialized_end=25483
-  _NOTEBOOKLIST._serialized_start=25486
-  _NOTEBOOKLIST._serialized_end=25649
-  _NOTEBOOKRUN._serialized_start=25652
-  _NOTEBOOKRUN._serialized_end=25915
-  _NOTEBOOKRUNCONDITION._serialized_start=25918
-  _NOTEBOOKRUNCONDITION._serialized_end=26075
-  _NOTEBOOKRUNLIST._serialized_start=26078
-  _NOTEBOOKRUNLIST._serialized_end=26247
-  _NOTEBOOKRUNSPEC._serialized_start=26250
-  _NOTEBOOKRUNSPEC._serialized_end=26573
-  _NOTEBOOKRUNSTATUS._serialized_start=26576
-  _NOTEBOOKRUNSTATUS._serialized_end=27072
-  _NOTEBOOKSPEC._serialized_start=27075
-  _NOTEBOOKSPEC._serialized_end=27694
-  _NOTEBOOKSTATUS._serialized_start=27697
-  _NOTEBOOKSTATUS._serialized_end=28180
-  _NOTEBOOKVARVALUE._serialized_start=28182
-  _NOTEBOOKVARVALUE._serialized_end=28229
-  _PERCENTILEPRUNEROPTIONS._serialized_start=28232
-  _PERCENTILEPRUNEROPTIONS._serialized_end=28364
-  _PRUNERSPEC._serialized_start=28367
-  _PRUNERSPEC._serialized_end=28898
-  _REGRESSIONFORECASTERSPEC._serialized_start=28901
-  _REGRESSIONFORECASTERSPEC._serialized_end=29109
-  _RELEASESTAGESPEC._serialized_start=29112
-  _RELEASESTAGESPEC._serialized_end=29405
-  _REPORT._serialized_start=29408
-  _REPORT._serialized_end=29656
-  _REPORTCONDITION._serialized_start=29659
-  _REPORTCONDITION._serialized_end=29811
-  _REPORTLIST._serialized_start=29814
-  _REPORTLIST._serialized_end=29973
-  _REPORTSPEC._serialized_start=29976
-  _REPORTSPEC._serialized_end=30527
-  _REPORTSTATUS._serialized_start=30530
-  _REPORTSTATUS._serialized_end=31008
-  _REPORTTEMPLATE._serialized_start=31010
-  _REPORTTEMPLATE._serialized_end=31110
-  _RESOURCECONSUMPTION._serialized_start=31112
-  _RESOURCECONSUMPTION._serialized_end=31172
-  _RUNTIMESTATUS._serialized_start=31175
-  _RUNTIMESTATUS._serialized_end=31416
-  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_start=31363
-  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_end=31416
-  _SEARCHSPEC._serialized_start=31419
-  _SEARCHSPEC._serialized_end=31931
-  _SEASONALITYPERIODSPEC._serialized_start=31933
-  _SEASONALITYPERIODSPEC._serialized_end=32009
-  _SEASONALITYSPEC._serialized_start=32012
-  _SEASONALITYSPEC._serialized_end=32531
-  _SEGMENTSPEC._serialized_start=32533
-  _SEGMENTSPEC._serialized_end=32593
-  _SERVINGSPEC._serialized_start=32595
-  _SERVINGSPEC._serialized_end=32714
-  _STUDY._serialized_start=32717
-  _STUDY._serialized_end=32962
-  _STUDYCONDITION._serialized_start=32965
-  _STUDYCONDITION._serialized_end=33116
-  _STUDYLIST._serialized_start=33119
-  _STUDYLIST._serialized_end=33276
-  _STUDYPHASESTATUS._serialized_start=33279
-  _STUDYPHASESTATUS._serialized_end=33539
-  _STUDYSCHEDULESPEC._serialized_start=33541
-  _STUDYSCHEDULESPEC._serialized_end=33638
-  _STUDYSPEC._serialized_start=33641
-  _STUDYSPEC._serialized_end=35713
-  _STUDYSTATUS._serialized_start=35716
-  _STUDYSTATUS._serialized_end=37657
-  _SUCCESSIVEHALVINGOPTIONS._serialized_start=37659
-  _SUCCESSIVEHALVINGOPTIONS._serialized_end=37786
-  _SUCCESSIVEHALVINGSPEC._serialized_start=37788
-  _SUCCESSIVEHALVINGSPEC._serialized_end=37892
-  _TEXTPIPELINESPEC._serialized_start=37895
-  _TEXTPIPELINESPEC._serialized_end=38068
-  _THRESHOLDPRUNEROPTIONS._serialized_start=38070
-  _THRESHOLDPRUNEROPTIONS._serialized_end=38168
-  _TIMESERIESEVENT._serialized_start=38171
-  _TIMESERIESEVENT._serialized_end=38309
-  _TRAININGSPEC._serialized_start=38312
-  _TRAININGSPEC._serialized_end=38980
-  _TRAININGSTAGESPEC._serialized_start=38982
-  _TRAININGSTAGESPEC._serialized_end=39084
-  _UATSTAGESPEC._serialized_start=39087
-  _UATSTAGESPEC._serialized_end=39326
-  _UNIVARIATEFORECASTSTATUS._serialized_start=39329
-  _UNIVARIATEFORECASTSTATUS._serialized_end=39549
-  _VIDEOPIPELINESPEC._serialized_start=39551
-  _VIDEOPIPELINESPEC._serialized_end=39590
-  _WINDOWSPEC._serialized_start=39592
-  _WINDOWSPEC._serialized_end=39653
+  _MODELGROUPBYSTATUS._serialized_end=13417
+  _MODELIMAGESPEC._serialized_start=13419
+  _MODELIMAGESPEC._serialized_end=13501
+  _MODELLIST._serialized_start=13504
+  _MODELLIST._serialized_end=13661
+  _MODELPIPELINE._serialized_start=13664
+  _MODELPIPELINE._serialized_end=13933
+  _MODELPIPELINECONDITION._serialized_start=13936
+  _MODELPIPELINECONDITION._serialized_end=14095
+  _MODELPIPELINELIST._serialized_start=14098
+  _MODELPIPELINELIST._serialized_end=14271
+  _MODELPIPELINERUN._serialized_start=14274
+  _MODELPIPELINERUN._serialized_end=14552
+  _MODELPIPELINERUNCONDITION._serialized_start=14555
+  _MODELPIPELINERUNCONDITION._serialized_end=14717
+  _MODELPIPELINERUNLIST._serialized_start=14720
+  _MODELPIPELINERUNLIST._serialized_end=14899
+  _MODELPIPELINERUNSPEC._serialized_start=14902
+  _MODELPIPELINERUNSPEC._serialized_end=15088
+  _MODELPIPELINERUNSTAGESTATUS._serialized_start=15091
+  _MODELPIPELINERUNSTAGESTATUS._serialized_end=15475
+  _MODELPIPELINERUNSTATUS._serialized_start=15478
+  _MODELPIPELINERUNSTATUS._serialized_end=16928
+  _MODELPIPELINESPEC._serialized_start=16931
+  _MODELPIPELINESPEC._serialized_end=18015
+  _MODELPIPELINESPEC_DATASETSELECTORENTRY._serialized_start=17961
+  _MODELPIPELINESPEC_DATASETSELECTORENTRY._serialized_end=18015
+  _MODELPIPELINESTATUS._serialized_start=18018
+  _MODELPIPELINESTATUS._serialized_end=18431
+  _MODELRESULT._serialized_start=18433
+  _MODELRESULT._serialized_end=18520
+  _MODELSPEC._serialized_start=18523
+  _MODELSPEC._serialized_end=20645
+  _MODELSTATUS._serialized_start=20648
+  _MODELSTATUS._serialized_end=24683
+  _MODELTESTSUITE._serialized_start=24686
+  _MODELTESTSUITE._serialized_end=24909
+  _NLPESTIMATORSPEC._serialized_start=24911
+  _NLPESTIMATORSPEC._serialized_end=24943
+  _NNLAYERPARAMETER._serialized_start=24945
+  _NNLAYERPARAMETER._serialized_end=24992
+  _NOTEBOOK._serialized_start=24995
+  _NOTEBOOK._serialized_end=25249
+  _NOTEBOOKCONDITION._serialized_start=25252
+  _NOTEBOOKCONDITION._serialized_end=25406
+  _NOTEBOOKLIST._serialized_start=25409
+  _NOTEBOOKLIST._serialized_end=25572
+  _NOTEBOOKRUN._serialized_start=25575
+  _NOTEBOOKRUN._serialized_end=25838
+  _NOTEBOOKRUNCONDITION._serialized_start=25841
+  _NOTEBOOKRUNCONDITION._serialized_end=25998
+  _NOTEBOOKRUNLIST._serialized_start=26001
+  _NOTEBOOKRUNLIST._serialized_end=26170
+  _NOTEBOOKRUNSPEC._serialized_start=26173
+  _NOTEBOOKRUNSPEC._serialized_end=26496
+  _NOTEBOOKRUNSTATUS._serialized_start=26499
+  _NOTEBOOKRUNSTATUS._serialized_end=26995
+  _NOTEBOOKSPEC._serialized_start=26998
+  _NOTEBOOKSPEC._serialized_end=27617
+  _NOTEBOOKSTATUS._serialized_start=27620
+  _NOTEBOOKSTATUS._serialized_end=28103
+  _NOTEBOOKVARVALUE._serialized_start=28105
+  _NOTEBOOKVARVALUE._serialized_end=28152
+  _PERCENTILEPRUNEROPTIONS._serialized_start=28155
+  _PERCENTILEPRUNEROPTIONS._serialized_end=28287
+  _PRUNERSPEC._serialized_start=28290
+  _PRUNERSPEC._serialized_end=28821
+  _REGRESSIONFORECASTERSPEC._serialized_start=28824
+  _REGRESSIONFORECASTERSPEC._serialized_end=29032
+  _RELEASESTAGESPEC._serialized_start=29035
+  _RELEASESTAGESPEC._serialized_end=29328
+  _REPORT._serialized_start=29331
+  _REPORT._serialized_end=29579
+  _REPORTCONDITION._serialized_start=29582
+  _REPORTCONDITION._serialized_end=29734
+  _REPORTLIST._serialized_start=29737
+  _REPORTLIST._serialized_end=29896
+  _REPORTSPEC._serialized_start=29899
+  _REPORTSPEC._serialized_end=30450
+  _REPORTSTATUS._serialized_start=30453
+  _REPORTSTATUS._serialized_end=30931
+  _REPORTTEMPLATE._serialized_start=30933
+  _REPORTTEMPLATE._serialized_end=31033
+  _RESOURCECONSUMPTION._serialized_start=31035
+  _RESOURCECONSUMPTION._serialized_end=31095
+  _RUNTIMESTATUS._serialized_start=31098
+  _RUNTIMESTATUS._serialized_end=31339
+  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_start=31286
+  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_end=31339
+  _SEARCHSPEC._serialized_start=31342
+  _SEARCHSPEC._serialized_end=31854
+  _SEASONALITYPERIODSPEC._serialized_start=31856
+  _SEASONALITYPERIODSPEC._serialized_end=31932
+  _SEASONALITYSPEC._serialized_start=31935
+  _SEASONALITYSPEC._serialized_end=32454
+  _SEGMENTSPEC._serialized_start=32456
+  _SEGMENTSPEC._serialized_end=32516
+  _SERVINGSPEC._serialized_start=32518
+  _SERVINGSPEC._serialized_end=32637
+  _STUDY._serialized_start=32640
+  _STUDY._serialized_end=32885
+  _STUDYCONDITION._serialized_start=32888
+  _STUDYCONDITION._serialized_end=33039
+  _STUDYGROUPBYSTATUS._serialized_start=33042
+  _STUDYGROUPBYSTATUS._serialized_end=33179
+  _STUDYLIST._serialized_start=33182
+  _STUDYLIST._serialized_end=33339
+  _STUDYPHASESTATUS._serialized_start=33342
+  _STUDYPHASESTATUS._serialized_end=33602
+  _STUDYSCHEDULESPEC._serialized_start=33604
+  _STUDYSCHEDULESPEC._serialized_end=33701
+  _STUDYSPEC._serialized_start=33704
+  _STUDYSPEC._serialized_end=35776
+  _STUDYSTATUS._serialized_start=35779
+  _STUDYSTATUS._serialized_end=37819
+  _SUCCESSIVEHALVINGOPTIONS._serialized_start=37821
+  _SUCCESSIVEHALVINGOPTIONS._serialized_end=37948
+  _SUCCESSIVEHALVINGSPEC._serialized_start=37950
+  _SUCCESSIVEHALVINGSPEC._serialized_end=38054
+  _TEXTPIPELINESPEC._serialized_start=38057
+  _TEXTPIPELINESPEC._serialized_end=38230
+  _THRESHOLDPRUNEROPTIONS._serialized_start=38232
+  _THRESHOLDPRUNEROPTIONS._serialized_end=38330
+  _TIMESERIESEVENT._serialized_start=38333
+  _TIMESERIESEVENT._serialized_end=38471
+  _TRAININGSPEC._serialized_start=38474
+  _TRAININGSPEC._serialized_end=39142
+  _TRAININGSTAGESPEC._serialized_start=39144
+  _TRAININGSTAGESPEC._serialized_end=39246
+  _UATSTAGESPEC._serialized_start=39249
+  _UATSTAGESPEC._serialized_end=39488
+  _UNIVARIATEFORECASTSTATUS._serialized_start=39491
+  _UNIVARIATEFORECASTSTATUS._serialized_end=39711
+  _VIDEOPIPELINESPEC._serialized_start=39713
+  _VIDEOPIPELINESPEC._serialized_end=39752
+  _WINDOWSPEC._serialized_start=39754
+  _WINDOWSPEC._serialized_end=39815
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/apitoken/v1/apitoken_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/apitoken/v1/apitoken_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/apitoken/v1/apitoken_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/apitoken/v1/apitoken_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronprediction/v1/cronprediction_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronprediction/v1/cronprediction_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronprediction/v1/cronprediction_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronprediction/v1/cronprediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronreport/v1/cronreport_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronreport/v1/cronreport_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/cronreport/v1/cronreport_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/cronreport/v1/cronreport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/curtain/v1/curtain_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/curtain/v1/curtain_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/curtain/v1/curtain_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/curtain/v1/curtain_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/feature/v1/feature_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/feature/v1/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/feature/v1/feature_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/feature/v1/feature_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipeline/v1/featurepipeline_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipeline/v1/featurepipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipeline/v1/featurepipeline_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipeline/v1/featurepipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipelinerun/v1/featurepipelinerun_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipelinerun/v1/featurepipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featurepipelinerun/v1/featurepipelinerun_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featurepipelinerun/v1/featurepipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featureset/v1/featureset_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featureset/v1/featureset_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/featureset/v1/featureset_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/featureset/v1/featureset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipeline/v1/labelingpipeline_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipeline/v1/labelingpipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipeline/v1/labelingpipeline_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipeline/v1/labelingpipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipelinerun/v1/labelingpipelinerun_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipelinerun/v1/labelingpipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/labelingpipelinerun/v1/labelingpipelinerun_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/labelingpipelinerun/v1/labelingpipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/meeting/v1/meeting_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/meeting/v1/meeting_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/meeting/v1/meeting_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/meeting/v1/meeting_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelautobuilder/v1/modelautobuilder_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelautobuilder/v1/modelautobuilder_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelautobuilder/v1/modelautobuilder_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelautobuilder/v1/modelautobuilder_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelcompilerrun/v1/modelcompilerrun_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelcompilerrun/v1/modelcompilerrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelcompilerrun/v1/modelcompilerrun_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelcompilerrun/v1/modelcompilerrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipeline/v1/modelpipeline_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipeline/v1/modelpipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipeline/v1/modelpipeline_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipeline/v1/modelpipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipelinerun/v1/modelpipelinerun_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipelinerun/v1/modelpipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/modelpipelinerun/v1/modelpipelinerun_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/modelpipelinerun/v1/modelpipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebook/v1/notebook_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebook/v1/notebook_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebook/v1/notebook_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebook/v1/notebook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebookrun/v1/notebookrun_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebookrun/v1/notebookrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notebookrun/v1/notebookrun_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notebookrun/v1/notebookrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualcluster/v1/virtualcluster_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualcluster/v1/virtualcluster_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualcluster/v1/virtualcluster_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualcluster/v1/virtualcluster_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualvolume/v1/virtualvolume_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualvolume/v1/virtualvolume_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/virtualvolume/v1/virtualvolume_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/virtualvolume/v1/virtualvolume_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequest/v1/webrequest_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequest/v1/webrequest_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequest/v1/webrequest_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequest/v1/webrequest_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequestrun/v1/webrequestrun_pb2.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequestrun/v1/webrequestrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/github/com/metaprov/modelaapi/services/webrequestrun/v1/webrequestrun_pb2_grpc.py` & `modelaapi-0.5.99/github/com/metaprov/modelaapi/services/webrequestrun/v1/webrequestrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/google/api/annotations_pb2.py` & `modelaapi-0.5.99/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/google/api/http_pb2.py` & `modelaapi-0.5.99/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/k8s/io/api/apps/v1/generated_pb2.py` & `modelaapi-0.5.99/k8s/io/api/apps/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/k8s/io/api/core/v1/generated_pb2.py` & `modelaapi-0.5.99/k8s/io/api/core/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/k8s/io/api/rbac/v1/generated_pb2.py` & `modelaapi-0.5.99/k8s/io/api/rbac/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py` & `modelaapi-0.5.99/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py` & `modelaapi-0.5.99/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/k8s/io/apimachinery/pkg/runtime/generated_pb2.py` & `modelaapi-0.5.99/k8s/io/apimachinery/pkg/runtime/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py` & `modelaapi-0.5.99/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py` & `modelaapi-0.5.99/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/modelaapi/custom_transformers.py` & `modelaapi-0.5.99/modelaapi/custom_transformers.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/modelaapi/version.py` & `modelaapi-0.5.99/modelaapi/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
     "minor": 5,
-    "micro": 98,    
+    "micro": 99,    
     "releaselevel": "alpha",
     "post": 0,
     "serial": 1,
 }
 
 ##########################################################################
 ## Helper Functions
```

### Comparing `modelaapi-0.5.98/modelaapi.egg-info/PKG-INFO` & `modelaapi-0.5.99/modelaapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.5.98
+Version: 0.5.99
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
-Download-URL: https://github.com/metaptov/modelaapi/tarball/v0.5.98
+Download-URL: https://github.com/metaptov/modelaapi/tarball/v0.5.99
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaptov/modelaapi/tarball/v0.5.98
+Project-URL: Download, https://github.com/metaptov/modelaapi/tarball/v0.5.99
 Project-URL: Source, https://github.com/metaptov/modelaapi
 Project-URL: Tracker, https://github.com/metaptov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `modelaapi-0.5.98/modelaapi.egg-info/SOURCES.txt` & `modelaapi-0.5.99/modelaapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/packagify.py` & `modelaapi-0.5.99/packagify.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/setup.cfg` & `modelaapi-0.5.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelaapi-0.5.98/setup.py` & `modelaapi-0.5.99/setup.py`

 * *Files identical despite different names*

