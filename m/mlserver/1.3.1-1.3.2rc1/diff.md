# Comparing `tmp/mlserver-1.3.1.tar.gz` & `tmp/mlserver-1.3.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-1.3.1.tar", last modified: Fri Apr 14 18:06:37 2023, max compression
+gzip compressed data, was "mlserver-1.3.2rc1.tar", last modified: Thu Apr 20 16:08:57 2023, max compression
```

## Comparing `mlserver-1.3.1.tar` & `mlserver-1.3.2rc1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.578420 mlserver-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-14 18:05:57.000000 mlserver-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 18:05:57.000000 mlserver-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-14 18:06:37.578420 mlserver-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-14 18:05:57.000000 mlserver-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.566420 mlserver-1.3.1/mlserver/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/batch_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.570420 mlserver-1.3.1/mlserver/batching/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/batching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/batching/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/batching/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/batching/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/batching/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.570420 mlserver-1.3.1/mlserver/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cli/init_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cli/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cloudevents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.570420 mlserver-1.3.1/mlserver/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.574420 mlserver-1.3.1/mlserver/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    31033 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/dataplane_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/dataplane_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/interceptors.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/model_repository_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/model_repository_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/servicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.574420 mlserver-1.3.1/mlserver/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/handlers/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/handlers/dataplane.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/handlers/model_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.574420 mlserver-1.3.1/mlserver/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/kafka/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/kafka/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/kafka/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/kafka/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/kafka/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.574420 mlserver-1.3.1/mlserver/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.578420 mlserver-1.3.1/mlserver/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.578420 mlserver-1.3.1/mlserver/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/repository/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/repository/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/repository/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.578420 mlserver-1.3.1/mlserver/rest/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.578420 mlserver-1.3.1/mlserver/rest/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19065 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/openapi/dataplane.json
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/openapi/model_repository.json
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/openapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.578420 mlserver-1.3.1/mlserver/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/types/dataplane.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/types/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.566420 mlserver-1.3.1/mlserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-14 18:06:37.000000 mlserver-1.3.1/mlserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-14 18:06:37.000000 mlserver-1.3.1/mlserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:06:37.000000 mlserver-1.3.1/mlserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 18:06:37.000000 mlserver-1.3.1/mlserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-14 18:06:37.000000 mlserver-1.3.1/mlserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 18:06:37.000000 mlserver-1.3.1/mlserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-14 18:06:37.582420 mlserver-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-14 18:05:58.000000 mlserver-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.315351 mlserver-1.3.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-04-20 16:08:57.315351 mlserver-1.3.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.307350 mlserver-1.3.2rc1/mlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/batch_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.307350 mlserver-1.3.2rc1/mlserver/batching/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/batching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/batching/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/batching/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/batching/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/batching/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.307350 mlserver-1.3.2rc1/mlserver/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/cli/init_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/cli/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/cloudevents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.311351 mlserver-1.3.2rc1/mlserver/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/codecs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/codecs/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/codecs/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/codecs/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/codecs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/codecs/lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/codecs/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/codecs/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/codecs/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/codecs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.311351 mlserver-1.3.2rc1/mlserver/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/grpc/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31033 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/grpc/dataplane_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/grpc/dataplane_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/grpc/interceptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/grpc/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/grpc/model_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/grpc/model_repository_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/grpc/model_repository_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/grpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/grpc/servicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/grpc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.311351 mlserver-1.3.2rc1/mlserver/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/handlers/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/handlers/dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/handlers/model_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.311351 mlserver-1.3.2rc1/mlserver/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/kafka/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/kafka/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/kafka/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/kafka/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/kafka/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.311351 mlserver-1.3.2rc1/mlserver/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/metrics/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/metrics/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/metrics/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/metrics/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/metrics/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/metrics/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.315351 mlserver-1.3.2rc1/mlserver/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/parallel/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/parallel/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/parallel/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/parallel/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/parallel/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/parallel/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/parallel/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.315351 mlserver-1.3.2rc1/mlserver/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/repository/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/repository/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/repository/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.315351 mlserver-1.3.2rc1/mlserver/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.315351 mlserver-1.3.2rc1/mlserver/rest/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19065 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/openapi/dataplane.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/openapi/model_repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/openapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/rest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.315351 mlserver-1.3.2rc1/mlserver/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/types/dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/types/model_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/mlserver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:08:57.307350 mlserver-1.3.2rc1/mlserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-04-20 16:08:57.000000 mlserver-1.3.2rc1/mlserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-20 16:08:57.000000 mlserver-1.3.2rc1/mlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:08:57.000000 mlserver-1.3.2rc1/mlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 16:08:57.000000 mlserver-1.3.2rc1/mlserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-20 16:08:57.000000 mlserver-1.3.2rc1/mlserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 16:08:57.000000 mlserver-1.3.2rc1/mlserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-20 16:08:57.315351 mlserver-1.3.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-20 16:08:20.000000 mlserver-1.3.2rc1/setup.py
```

### Comparing `mlserver-1.3.1/LICENSE` & `mlserver-1.3.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/PKG-INFO` & `mlserver-1.3.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver
-Version: 1.3.1
+Version: 1.3.2rc1
 Summary: ML server
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # MLServer
```

### Comparing `mlserver-1.3.1/README.md` & `mlserver-1.3.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/batch_processing.py` & `mlserver-1.3.2rc1/mlserver/batch_processing.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/batching/adaptive.py` & `mlserver-1.3.2rc1/mlserver/batching/adaptive.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/batching/hooks.py` & `mlserver-1.3.2rc1/mlserver/batching/hooks.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Awaitable, Callable, Optional
 
 from ..errors import MLServerError
 from ..model import MLModel
 from ..types import InferenceRequest, InferenceResponse
 from ..utils import get_wrapped_method
 from .adaptive import AdaptiveBatcher
+from ..logging import logger
 
 _AdaptiveBatchingAttr = "__adaptive_batching__"
 
 
 class InvalidBatchingMethod(MLServerError):
     def __init__(self, method_name: str, reason: Optional[str] = None):
         msg = f"Method {method_name} can't be used for adaptive batching"
@@ -48,14 +49,22 @@
 async def load_batching(model: MLModel) -> MLModel:
     if model.settings.max_batch_size <= 1:
         return model
 
     if model.settings.max_batch_time <= 0:
         return model
 
+    if model.settings.max_batch_size > 1 and model.settings.max_batch_time <= 0:
+        logger.warning(
+            "Setting max_batch_time equal to zero will result"
+            " in batching having no effect, if you intend to "
+            "use batching try setting it to a value > 0 for"
+            " batching to take effect"
+        )
+
     batcher = AdaptiveBatcher(model)
     setattr(model, _AdaptiveBatchingAttr, batcher)
 
     # Decorate predict method
     setattr(model, "predict", adaptive_batching(model.predict))
 
     return model
```

### Comparing `mlserver-1.3.1/mlserver/batching/requests.py` & `mlserver-1.3.2rc1/mlserver/batching/requests.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/batching/shape.py` & `mlserver-1.3.2rc1/mlserver/batching/shape.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/cli/build.py` & `mlserver-1.3.2rc1/mlserver/cli/build.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/cli/constants.py` & `mlserver-1.3.2rc1/mlserver/cli/constants.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/cli/main.py` & `mlserver-1.3.2rc1/mlserver/cli/main.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/cli/serve.py` & `mlserver-1.3.2rc1/mlserver/cli/serve.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/cloudevents.py` & `mlserver-1.3.2rc1/mlserver/cloudevents.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/codecs/__init__.py` & `mlserver-1.3.2rc1/mlserver/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/codecs/base.py` & `mlserver-1.3.2rc1/mlserver/codecs/base.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/codecs/base64.py` & `mlserver-1.3.2rc1/mlserver/codecs/base64.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/codecs/datetime.py` & `mlserver-1.3.2rc1/mlserver/codecs/datetime.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/codecs/decorator.py` & `mlserver-1.3.2rc1/mlserver/codecs/decorator.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/codecs/errors.py` & `mlserver-1.3.2rc1/mlserver/codecs/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/codecs/lists.py` & `mlserver-1.3.2rc1/mlserver/codecs/lists.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/codecs/numpy.py` & `mlserver-1.3.2rc1/mlserver/codecs/numpy.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/codecs/pandas.py` & `mlserver-1.3.2rc1/mlserver/codecs/pandas.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/codecs/string.py` & `mlserver-1.3.2rc1/mlserver/codecs/string.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/codecs/utils.py` & `mlserver-1.3.2rc1/mlserver/codecs/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/env.py` & `mlserver-1.3.2rc1/mlserver/env.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/errors.py` & `mlserver-1.3.2rc1/mlserver/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/grpc/converters.py` & `mlserver-1.3.2rc1/mlserver/grpc/converters.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/grpc/dataplane_pb2.py` & `mlserver-1.3.2rc1/mlserver/grpc/dataplane_pb2.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/grpc/dataplane_pb2_grpc.py` & `mlserver-1.3.2rc1/mlserver/grpc/dataplane_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/grpc/interceptors.py` & `mlserver-1.3.2rc1/mlserver/grpc/interceptors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/grpc/model_repository.py` & `mlserver-1.3.2rc1/mlserver/grpc/model_repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/grpc/model_repository_pb2.py` & `mlserver-1.3.2rc1/mlserver/grpc/model_repository_pb2.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/grpc/model_repository_pb2_grpc.py` & `mlserver-1.3.2rc1/mlserver/grpc/model_repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/grpc/server.py` & `mlserver-1.3.2rc1/mlserver/grpc/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/grpc/servicers.py` & `mlserver-1.3.2rc1/mlserver/grpc/servicers.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/grpc/utils.py` & `mlserver-1.3.2rc1/mlserver/grpc/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/handlers/custom.py` & `mlserver-1.3.2rc1/mlserver/handlers/custom.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/handlers/dataplane.py` & `mlserver-1.3.2rc1/mlserver/handlers/dataplane.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/handlers/model_repository.py` & `mlserver-1.3.2rc1/mlserver/handlers/model_repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/kafka/handlers.py` & `mlserver-1.3.2rc1/mlserver/kafka/handlers.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/kafka/message.py` & `mlserver-1.3.2rc1/mlserver/kafka/message.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/kafka/server.py` & `mlserver-1.3.2rc1/mlserver/kafka/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/logging.py` & `mlserver-1.3.2rc1/mlserver/logging.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/metrics/context.py` & `mlserver-1.3.2rc1/mlserver/metrics/context.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/metrics/errors.py` & `mlserver-1.3.2rc1/mlserver/metrics/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/metrics/prometheus.py` & `mlserver-1.3.2rc1/mlserver/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/metrics/registry.py` & `mlserver-1.3.2rc1/mlserver/metrics/registry.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/metrics/server.py` & `mlserver-1.3.2rc1/mlserver/metrics/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/middleware.py` & `mlserver-1.3.2rc1/mlserver/middleware.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/model.py` & `mlserver-1.3.2rc1/mlserver/model.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/parallel/dispatcher.py` & `mlserver-1.3.2rc1/mlserver/parallel/dispatcher.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/parallel/errors.py` & `mlserver-1.3.2rc1/mlserver/parallel/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/parallel/messages.py` & `mlserver-1.3.2rc1/mlserver/parallel/messages.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/parallel/model.py` & `mlserver-1.3.2rc1/mlserver/parallel/model.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/parallel/pool.py` & `mlserver-1.3.2rc1/mlserver/parallel/pool.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/parallel/registry.py` & `mlserver-1.3.2rc1/mlserver/parallel/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,20 @@
         Used to initialise a model object in the ModelRegistry.
         """
         if not self._should_load_model(model_settings):
             # If parallel inference should not be used, instantiate the model
             # as normal.
             return model_initialiser(model_settings)
 
+        parameters = model_settings.parameters
+        if not parameters or not parameters.environment_tarball:
+            # If model is not using a custom environment, instantiate the model
+            # as normal.
+            return model_initialiser(model_settings)
+
         # Otherwise, return a dummy model for now and wait for the load_model
         # hook to create the actual thing.
         # This avoids instantiating the model's actual class within the
         # main process.
         return MLModel(model_settings)
 
     async def load_model(self, model: MLModel) -> MLModel:
```

### Comparing `mlserver-1.3.1/mlserver/parallel/utils.py` & `mlserver-1.3.2rc1/mlserver/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/parallel/worker.py` & `mlserver-1.3.2rc1/mlserver/parallel/worker.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/raw.py` & `mlserver-1.3.2rc1/mlserver/raw.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/registry.py` & `mlserver-1.3.2rc1/mlserver/registry.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/repository/factory.py` & `mlserver-1.3.2rc1/mlserver/repository/factory.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/repository/load.py` & `mlserver-1.3.2rc1/mlserver/repository/load.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/repository/repository.py` & `mlserver-1.3.2rc1/mlserver/repository/repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/rest/app.py` & `mlserver-1.3.2rc1/mlserver/rest/app.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/rest/endpoints.py` & `mlserver-1.3.2rc1/mlserver/rest/endpoints.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/rest/logging.py` & `mlserver-1.3.2rc1/mlserver/rest/logging.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/rest/openapi/dataplane.json` & `mlserver-1.3.2rc1/mlserver/rest/openapi/dataplane.json`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/rest/openapi/model_repository.json` & `mlserver-1.3.2rc1/mlserver/rest/openapi/model_repository.json`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/rest/openapi/schema.py` & `mlserver-1.3.2rc1/mlserver/rest/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/rest/requests.py` & `mlserver-1.3.2rc1/mlserver/rest/requests.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/rest/responses.py` & `mlserver-1.3.2rc1/mlserver/rest/responses.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/rest/server.py` & `mlserver-1.3.2rc1/mlserver/rest/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/rest/utils.py` & `mlserver-1.3.2rc1/mlserver/rest/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/server.py` & `mlserver-1.3.2rc1/mlserver/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/settings.py` & `mlserver-1.3.2rc1/mlserver/settings.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/types/__init__.py` & `mlserver-1.3.2rc1/mlserver/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/types/base.py` & `mlserver-1.3.2rc1/mlserver/types/base.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/types/dataplane.py` & `mlserver-1.3.2rc1/mlserver/types/dataplane.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/types/model_repository.py` & `mlserver-1.3.2rc1/mlserver/types/model_repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver/utils.py` & `mlserver-1.3.2rc1/mlserver/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/mlserver.egg-info/PKG-INFO` & `mlserver-1.3.2rc1/mlserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver
-Version: 1.3.1
+Version: 1.3.2rc1
 Summary: ML server
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # MLServer
```

### Comparing `mlserver-1.3.1/mlserver.egg-info/SOURCES.txt` & `mlserver-1.3.2rc1/mlserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.1/setup.cfg` & `mlserver-1.3.2rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -129,39 +129,46 @@
 	pip install \
 	-r{toxinidir}/runtimes/mlflow/requirements/dev.txt \
 	-r{toxinidir}/runtimes/alibi-explain/requirements/dev.txt \
 	-r{toxinidir}/runtimes/alibi-detect/requirements/dev.txt
 	pip install \
 	-e{toxinidir} \
 	-r{toxinidir}/requirements/docker.txt
+	pip install --upgrade setuptools pip wheel
 	python -m pytest {posargs} \
 	{toxinidir}/tests \
 	{toxinidir}/runtimes/alibi-explain \
 	{toxinidir}/runtimes/alibi-detect \
 	{toxinidir}/runtimes/sklearn \
 	{toxinidir}/runtimes/xgboost \
 	{toxinidir}/runtimes/mllib \
 	{toxinidir}/runtimes/lightgbm \
 	{toxinidir}/runtimes/mlflow \
 	{toxinidir}/runtimes/huggingface
 
 [testenv:licenses]
 deps = 
-	-e{toxinidir}
 	-e{toxinidir}/runtimes/alibi-explain
 	-e{toxinidir}/runtimes/alibi-detect
 	-e{toxinidir}/runtimes/sklearn
 	-e{toxinidir}/runtimes/xgboost
 	-e{toxinidir}/runtimes/mllib
 	-e{toxinidir}/runtimes/lightgbm
 	-e{toxinidir}/runtimes/mlflow
 	-e{toxinidir}/runtimes/huggingface
 	-r{toxinidir}/requirements/dev.txt
-	-r{toxinidir}/runtimes/mlflow/requirements/dev.txt
 commands = 
+	pip install \
+	-r{toxinidir}/runtimes/mlflow/requirements/dev.txt \
+	-r{toxinidir}/runtimes/alibi-explain/requirements/dev.txt \
+	-r{toxinidir}/runtimes/alibi-detect/requirements/dev.txt
+	pip install \
+	-e{toxinidir} \
+	-r{toxinidir}/requirements/docker.txt
+	pip install --upgrade setuptools pip wheel
 	pip-licenses \
 	--from=mixed \
 	--format=csv \
 	--output-file=./licenses/license_info.csv
 	pip-licenses \
 	--from=mixed \
 	--format=plain-vertical \
```

### Comparing `mlserver-1.3.1/setup.py` & `mlserver-1.3.2rc1/setup.py`

 * *Files identical despite different names*

