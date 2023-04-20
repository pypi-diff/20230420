# Comparing `tmp/kaskada-0.1.4.tar.gz` & `tmp/kaskada-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaskada-0.1.4.tar", max compression
+gzip compressed data, was "kaskada-0.1.5.tar", max compression
```

## Comparing `kaskada-0.1.4.tar` & `kaskada-0.1.5.tar`

### file list

```diff
@@ -1,83 +1,88 @@
--rw-r--r--   0        0        0     1098 2023-04-11 22:38:35.487057 kaskada-0.1.4/README.md
--rw-r--r--   0        0        0     3223 2023-04-11 23:54:13.671660 kaskada-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7084 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/fenlmagic/__init__.py
--rw-r--r--   0        0        0      401 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/fenlmagic/utils.py
--rw-r--r--   0        0        0     1546 2023-04-11 23:46:04.727618 kaskada-0.1.4/src/kaskada/api/__pycache__/api_utils.cpython-310.pyc
--rw-r--r--   0        0        0     5350 2023-04-11 23:46:04.731618 kaskada-0.1.4/src/kaskada/api/__pycache__/release.cpython-310.pyc
--rw-r--r--   0        0        0     8797 2023-04-11 23:46:04.727618 kaskada-0.1.4/src/kaskada/api/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0     1179 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/api/api_utils.py
--rw-r--r--   0        0        0     6381 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/api/release.py
--rw-r--r--   0        0        0     8961 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/api/session.py
--rw-r--r--   0        0        0     5688 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/client.py
--rw-r--r--   0        0        0     1500 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/formatters.css
--rw-r--r--   0        0        0      984 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/formatters.js
--rw-r--r--   0        0        0    26206 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/formatters.py
--rw-r--r--   0        0        0     7318 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/formatters_helpers.py
--rw-r--r--   0        0        0     9805 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/formatters_shared.py
--rw-r--r--   0        0        0     6457 2023-04-11 23:46:04.651619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/common_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     3499 2023-04-11 23:46:04.655619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/destinations_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2491 2023-04-11 23:46:04.651619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/fenl_diagnostics_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     7685 2023-04-11 23:46:04.655619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/materialization_service_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4932 2023-04-11 23:46:04.655619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/materialization_service_pb2_grpc.cpython-310.pyc
--rw-r--r--   0        0        0     1570 2023-04-11 23:46:03.995632 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/options_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2461 2023-04-11 23:46:04.647619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/pulsar_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     8772 2023-04-11 23:46:04.659619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/query_service_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     3917 2023-04-11 23:46:04.659619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/query_service_pb2_grpc.cpython-310.pyc
--rw-r--r--   0        0        0     3255 2023-04-11 23:46:04.651619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/schema_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2169 2023-04-11 23:46:04.651619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/sources_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     7592 2023-04-11 23:46:04.647619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/table_service_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4952 2023-04-11 23:46:04.659619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/table_service_pb2_grpc.cpython-310.pyc
--rw-r--r--   0        0        0     3806 2023-04-11 23:46:03.991632 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      425 2023-04-11 23:46:03.999632 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2_grpc.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     5783 2023-04-11 23:46:04.655619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/view_service_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4330 2023-04-11 23:46:04.659619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/view_service_pb2_grpc.cpython-310.pyc
--rw-r--r--   0        0        0    13053 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/common_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
--rw-r--r--   0        0        0    16901 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
--rw-r--r--   0        0        0     6628 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
--rw-r--r--   0        0        0     5994 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
--rw-r--r--   0        0        0     2938 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
--rw-r--r--   0        0        0     6043 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/destinations_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
--rw-r--r--   0        0        0     3526 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
--rw-r--r--   0        0        0     6348 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/file_service_pb2.py
--rw-r--r--   0        0        0     5054 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
--rw-r--r--   0        0        0    15562 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
--rw-r--r--   0        0        0     9283 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     1846 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/options_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
--rw-r--r--   0        0        0    21703 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/plan_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
--rw-r--r--   0        0        0     4981 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
--rw-r--r--   0        0        0     4894 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
--rw-r--r--   0        0        0     3561 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
--rw-r--r--   0        0        0    16795 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/query_service_pb2.py
--rw-r--r--   0        0        0     6542 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     4886 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/schema_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
--rw-r--r--   0        0        0     3258 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/sources_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
--rw-r--r--   0        0        0     2882 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/spec_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
--rw-r--r--   0        0        0    15322 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/table_service_pb2.py
--rw-r--r--   0        0        0    10053 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
--rw-r--r--   0        0        0     6835 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
--rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
--rw-r--r--   0        0        0    11387 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/view_service_pb2.py
--rw-r--r--   0        0        0     8153 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
--rw-r--r--   0        0        0    26185 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v2alpha/query_service_pb2.py
--rw-r--r--   0        0        0     8377 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     8594 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/materialization.py
--rw-r--r--   0        0        0     9232 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/query.py
--rw-r--r--   0        0        0     2564 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/slice_filters.py
--rw-r--r--   0        0        0    10098 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/table.py
--rw-r--r--   0        0        0     6690 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/utils.py
--rw-r--r--   0        0        0     4515 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/view.py
--rw-r--r--   0        0        0    29800 2023-04-11 22:38:35.491057 kaskada-0.1.4/vendor/validate/validate.proto
--rw-r--r--   0        0        0    13089 2023-04-11 22:38:35.491057 kaskada-0.1.4/vendor/validate/validate_pb2.py
--rw-r--r--   0        0        0    22952 2023-04-11 22:38:35.491057 kaskada-0.1.4/vendor/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-11 22:38:35.491057 kaskada-0.1.4/vendor/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 kaskada-0.1.4/setup.py
--rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 kaskada-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1646 2023-04-19 20:57:42.994947 kaskada-0.1.5/README.md
+-rw-r--r--   0        0        0     3874 2023-04-20 13:03:18.953835 kaskada-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7209 2023-04-19 20:57:42.996697 kaskada-0.1.5/src/fenlmagic/__init__.py
+-rw-r--r--   0        0        0      401 2023-03-16 21:27:38.249764 kaskada-0.1.5/src/fenlmagic/utils.py
+-rw-r--r--   0        0        0       33 2023-04-19 20:57:42.996774 kaskada-0.1.5/src/kaskada/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 20:57:42.996810 kaskada-0.1.5/src/kaskada/api/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-20 13:06:11.384170 kaskada-0.1.5/src/kaskada/api/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1476 2023-03-20 16:22:12.166889 kaskada-0.1.5/src/kaskada/api/__pycache__/api_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     5241 2023-03-20 16:22:12.171063 kaskada-0.1.5/src/kaskada/api/__pycache__/release.cpython-39.pyc
+-rw-r--r--   0        0        0     9143 2023-04-20 13:06:11.389501 kaskada-0.1.5/src/kaskada/api/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     1179 2023-03-16 21:27:38.250104 kaskada-0.1.5/src/kaskada/api/api_utils.py
+-rw-r--r--   0        0        0     6381 2023-03-16 21:27:38.250435 kaskada-0.1.5/src/kaskada/api/release.py
+-rw-r--r--   0        0        0     9503 2023-04-19 22:53:22.424816 kaskada-0.1.5/src/kaskada/api/session.py
+-rw-r--r--   0        0        0     5838 2023-04-19 21:28:57.311096 kaskada-0.1.5/src/kaskada/client.py
+-rw-r--r--   0        0        0     1500 2023-03-16 21:27:38.251034 kaskada-0.1.5/src/kaskada/formatters.css
+-rw-r--r--   0        0        0      984 2023-03-16 21:27:38.251117 kaskada-0.1.5/src/kaskada/formatters.js
+-rw-r--r--   0        0        0    26206 2023-03-16 21:27:38.251456 kaskada-0.1.5/src/kaskada/formatters.py
+-rw-r--r--   0        0        0     7318 2023-03-16 21:27:38.251739 kaskada-0.1.5/src/kaskada/formatters_helpers.py
+-rw-r--r--   0        0        0     9805 2023-04-05 15:54:29.951572 kaskada-0.1.5/src/kaskada/formatters_shared.py
+-rw-r--r--   0        0        0     6383 2023-04-20 13:06:11.210937 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/common_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     3427 2023-04-20 13:06:11.247588 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/destinations_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     2419 2023-04-20 13:06:11.215018 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/fenl_diagnostics_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     7611 2023-04-20 13:06:11.243268 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/materialization_service_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     5132 2023-04-20 13:06:11.238064 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/materialization_service_pb2_grpc.cpython-39.pyc
+-rw-r--r--   0        0        0     1496 2023-04-20 13:06:10.479718 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/options_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     2389 2023-04-20 13:06:11.198536 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/pulsar_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     8698 2023-04-20 13:06:11.257260 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/query_service_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     4020 2023-04-20 13:06:11.252307 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/query_service_pb2_grpc.cpython-39.pyc
+-rw-r--r--   0        0        0     3183 2023-04-20 13:06:11.219039 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/schema_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     2097 2023-04-20 13:06:11.223654 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/sources_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     7518 2023-04-20 13:06:11.204897 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/table_service_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     5249 2023-04-20 13:06:11.262515 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/table_service_pb2_grpc.cpython-39.pyc
+-rw-r--r--   0        0        0     3732 2023-03-28 20:07:39.942540 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2.cpython-39-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3732 2023-04-20 13:06:10.460690 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      357 2023-03-28 20:07:39.964989 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2_grpc.cpython-39-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      357 2023-04-20 13:06:10.485843 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2_grpc.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     5709 2023-04-20 13:06:11.232312 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/view_service_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     4530 2023-04-20 13:06:11.267104 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/view_service_pb2_grpc.cpython-39.pyc
+-rw-r--r--   0        0        0    13053 2023-04-20 13:03:28.003641 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/common_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-20 13:03:28.002913 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
+-rw-r--r--   0        0        0    16901 2023-04-20 13:03:28.002955 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
+-rw-r--r--   0        0        0     6628 2023-04-20 13:03:28.004505 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5994 2023-04-20 13:03:28.004483 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
+-rw-r--r--   0        0        0     2938 2023-04-20 13:03:28.005059 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6043 2023-04-20 13:03:28.005347 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/destinations_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-20 13:03:28.006106 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
+-rw-r--r--   0        0        0     3526 2023-04-20 13:03:28.006962 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-20 13:03:28.007312 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
+-rw-r--r--   0        0        0     6348 2023-04-20 13:03:28.007747 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/file_service_pb2.py
+-rw-r--r--   0        0        0     5054 2023-04-20 13:03:28.008449 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
+-rw-r--r--   0        0        0    15562 2023-04-20 13:03:28.009017 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
+-rw-r--r--   0        0        0     9283 2023-04-20 13:03:28.009595 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1846 2023-04-20 13:03:28.009925 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/options_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-20 13:03:28.010338 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
+-rw-r--r--   0        0        0    21703 2023-04-20 13:03:28.010880 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/plan_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-20 13:03:28.012058 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
+-rw-r--r--   0        0        0     4981 2023-04-20 13:03:28.012421 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
+-rw-r--r--   0        0        0     4894 2023-04-20 13:03:28.013248 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3561 2023-04-20 13:03:28.014281 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-20 13:03:28.014445 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
+-rw-r--r--   0        0        0    16795 2023-04-20 13:03:28.014973 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     6542 2023-04-20 13:03:28.015692 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4886 2023-04-20 13:03:28.015994 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/schema_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-20 13:03:28.016385 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     3258 2023-04-20 13:03:28.017021 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/sources_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-20 13:03:28.017508 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
+-rw-r--r--   0        0        0     2882 2023-04-20 13:03:28.017959 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/spec_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-20 13:03:28.018476 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
+-rw-r--r--   0        0        0    15322 2023-04-20 13:03:28.019199 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/table_service_pb2.py
+-rw-r--r--   0        0        0    10053 2023-04-20 13:03:28.019981 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6835 2023-04-20 13:03:28.020233 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-20 13:03:28.020617 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
+-rw-r--r--   0        0        0    11387 2023-04-20 13:03:28.021258 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/view_service_pb2.py
+-rw-r--r--   0        0        0     8153 2023-04-20 13:03:28.021701 kaskada-0.1.5/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
+-rw-r--r--   0        0        0    26185 2023-04-20 13:03:28.022708 kaskada-0.1.5/src/kaskada/kaskada/v2alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     8377 2023-04-20 13:03:28.023223 kaskada-0.1.5/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8594 2023-04-05 15:54:29.951770 kaskada-0.1.5/src/kaskada/materialization.py
+-rw-r--r--   0        0        0     9232 2023-04-05 15:54:29.952092 kaskada-0.1.5/src/kaskada/query.py
+-rw-r--r--   0        0        0     2564 2023-03-16 21:27:38.252438 kaskada-0.1.5/src/kaskada/slice_filters.py
+-rw-r--r--   0        0        0    10098 2023-04-05 15:54:29.952252 kaskada-0.1.5/src/kaskada/table.py
+-rw-r--r--   0        0        0     6725 2023-04-19 20:57:42.997805 kaskada-0.1.5/src/kaskada/utils.py
+-rw-r--r--   0        0        0     4515 2023-03-16 21:27:38.252722 kaskada-0.1.5/src/kaskada/view.py
+-rw-r--r--   0        0        0    29800 2023-03-16 21:27:38.254737 kaskada-0.1.5/vendor/validate/validate.proto
+-rw-r--r--   0        0        0    13089 2023-03-16 21:27:38.254889 kaskada-0.1.5/vendor/validate/validate_pb2.py
+-rw-r--r--   0        0        0    22952 2023-03-16 21:27:38.255015 kaskada-0.1.5/vendor/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-03-16 21:27:38.255097 kaskada-0.1.5/vendor/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 kaskada-0.1.5/setup.py
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 kaskada-0.1.5/PKG-INFO
```

### Comparing `kaskada-0.1.4/pyproject.toml` & `kaskada-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaskada"
-version = "0.1.4"
+version = "0.1.5"
 description = "A client library for the Kaskada time travel machine learning service"
 authors = ["Kaskada <maintainers@kaskada.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "kaskada", from = "src" },
     { include = "validate", from = "vendor" },
@@ -23,14 +23,15 @@
 grpcio-status = "^1.51.1"
 grpcio = "^1.51.1"
 tqdm = "^4.64.1"
 pygithub = "^1.57"
 pandas = "~1.3"
 ipython = "7.34.0"
 
+
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 pylint = "^2.15.10"
 pytest = "^7.2.0"
 mypy = "^0.991"
 poethepoet = "^0.18.0"
@@ -39,14 +40,18 @@
 types-requests = "^2.28.11.7"
 types-setuptools = "^65.7.0.1"
 types-six = "^1.16.21.4"
 types-typed-ast = "^1.5.8.3"
 autoflake = "^2.0.0"
 autopep8 = "^2.0.1"
 types-protobuf = "^4.21.0.5"
+Sphinx = "5.3.0"
+sphinx-rtd-theme = "1.2.0"
+sphinx-autodoc-typehints = "1.22"
+tomli = "2.0.1"
 
 [tool.poe.tasks]
 [tool.poe.tasks.clean]
 help = "Remove generated files"
 cmd = """
         # multiline commands including comments work too!
         rm -rf .coverage
@@ -105,20 +110,41 @@
 help = "Validate code style"
 sequence = ["style-isort", "style-black"]
 
 [tool.poe.tasks.remove-imports-vars]
 help = "Run to remove unused imports and variables"
 cmd = "autoflake -r --in-place --remove-unused-variables src/"
 
+[tool.poe.tasks.docs-build]
+help = "Build documentation into HTML"
+cmd = "sphinx-build -E -b html docs/source/. docs/build"
+
+[tool.poe.tasks.docs-generate]
+help = "Generates documentation from docstrings"
+cmd = "sphinx-apidoc -f -E  -M -o docs/source src/ src/clients/python/kaskada/kaskada"
+
+[tool.poe.tasks.docs]
+help = "Generated and build HTML docs"
+sequence = ["docs-generate", "docs-build"]
+
 [tool.isort]
 profile = "black"
 skip = ["src/kaskada/kaskada"]
 
 [tool.mypy]
 exclude = ["src/kaskada/kaskada"]
+implicit_optional = true
+
+[[tool.mypy.overrides]]
+follow_imports = "skip"
+
+
+module = ["kaskada.kaskada.*"]
+ignore_errors = true
+ignore_missing_imports = true
 
 [tool.pylint.format]
 max-line-length = "120"
 fail-under = "5"
 
 [tool.pylint.MASTER]
 ignore-paths = 'src/ksakada/kaskada'
```

### Comparing `kaskada-0.1.4/src/fenlmagic/__init__.py` & `kaskada-0.1.5/src/fenlmagic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Integration with IPython (Notebooks) for Fenl.
+
+    Raises:
+        UsageError: when improper arguments are provided
+"""
+
 from __future__ import print_function
 
 import os
 
 import IPython
 import pandas
 from google.protobuf import wrappers_pb2 as wrappers
```

### Comparing `kaskada-0.1.4/src/kaskada/api/__pycache__/release.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/api/__pycache__/release.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 22:38:35 2023 UTC, .py size: 6381 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,335 +1,328 @@
-00000000: 6f0d 0d0a 0000 0000 6be1 3564 ed18 0000  o.......k.5d....
+00000000: 610d 0d0a 0000 0000 ca89 1364 ed18 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6401 6c07 5a07 6400 6403 6c08  ..d.d.l.Z.d.d.l.
 00000070: 6d09 5a09 0100 6400 6401 6c0a 5a0b 6501  m.Z...d.d.l.Z.e.
 00000080: 6a0c 6504 6a0d 6501 6a0e 6404 8d02 0100  j.e.j.e.j.d.....
 00000090: 6501 a00f 6510 a101 5a11 4700 6405 6406  e...e...Z.G.d.d.
 000000a0: 8400 6406 6512 8303 5a13 4700 6407 6408  ..d.e...Z.G.d.d.
 000000b0: 8400 6408 6512 8303 5a14 6401 5300 2909  ..d.e...Z.d.S.).
 000000c0: e900 0000 004e 2901 da04 5061 7468 2901  .....N)...Path).
 000000d0: da06 4769 7468 7562 2902 da06 7374 7265  ..Github)...stre
 000000e0: 616d da05 6c65 7665 6c63 0000 0000 0000  am..levelc......
-000000f0: 0000 0000 0000 0000 0000 0800 0000 4000  ..............@.
-00000100: 0000 732a 0000 0065 005a 0164 005a 0264  ..s*...e.Z.d.Z.d
-00000110: 015a 0364 0265 0464 0365 0464 0465 0464  .Z.d.e.d.e.d.e.d
-00000120: 0564 0666 0864 0764 0884 045a 0564 0653  .d.f.d.d...Z.d.S
-00000130: 0029 09da 0c4c 6f63 616c 5265 6c65 6173  .)...LocalReleas
-00000140: 657a 4843 6f6e 6669 6775 7261 7469 6f6e  ezHConfiguration
-00000150: 2064 6574 6169 6c73 2066 6f72 2061 206c   details for a l
-00000160: 6f63 616c 2072 656c 6561 7365 2e20 4d6f  ocal release. Mo
-00000170: 7374 6c79 2075 7365 6420 666f 7220 6269  stly used for bi
-00000180: 6e61 7279 2070 6174 6873 2eda 0d64 6f77  nary paths...dow
-00000190: 6e6c 6f61 645f 7061 7468 da0c 6d61 6e61  nload_path..mana
-000001a0: 6765 725f 7061 7468 da0b 656e 6769 6e65  ger_path..engine
-000001b0: 5f70 6174 68da 0672 6574 7572 6e4e 6304  _path..returnNc.
-000001c0: 0000 0000 0000 0000 0000 0004 0000 0002  ................
-000001d0: 0000 0043 0000 0073 1600 0000 7c01 7c00  ...C...s....|.|.
-000001e0: 5f00 7c02 7c00 5f01 7c03 7c00 5f02 6400  _.|.|._.|.|._.d.
-000001f0: 5300 a901 4e29 03da 0e5f 646f 776e 6c6f  S...N)..._downlo
-00000200: 6164 5f70 6174 68da 0d5f 6d61 6e61 6765  ad_path.._manage
-00000210: 725f 7061 7468 da0c 5f65 6e67 696e 655f  r_path.._engine_
-00000220: 7061 7468 2904 da04 7365 6c66 7207 0000  path)...selfr...
-00000230: 0072 0800 0000 7209 0000 00a9 0072 1000  .r....r......r..
-00000240: 0000 fa61 2f68 6f6d 652f 7468 6572 6170  ...a/home/therap
-00000250: 6f6e 2f52 6570 6f73 2f47 6974 4875 622f  on/Repos/GitHub/
-00000260: 4b61 736b 6164 6141 492f 6b61 736b 6164  KaskadaAI/kaskad
-00000270: 612f 7265 6c65 6173 696e 672f 636c 6965  a/releasing/clie
-00000280: 6e74 732f 7079 7468 6f6e 2f73 7263 2f6b  nts/python/src/k
-00000290: 6173 6b61 6461 2f61 7069 2f72 656c 6561  askada/api/relea
-000002a0: 7365 2e70 79da 085f 5f69 6e69 745f 5f14  se.py..__init__.
-000002b0: 0000 0073 0600 0000 0603 0601 0a01 7a15  ...s..........z.
-000002c0: 4c6f 6361 6c52 656c 6561 7365 2e5f 5f69  LocalRelease.__i
-000002d0: 6e69 745f 5f29 06da 085f 5f6e 616d 655f  nit__)...__name_
-000002e0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000002f0: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-00000300: 6f63 5f5f 7202 0000 0072 1200 0000 7210  oc__r....r....r.
-00000310: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
-00000320: 0000 7206 0000 0011 0000 0073 1600 0000  ..r........s....
-00000330: 0800 0401 0202 0201 02ff 0201 02ff 0201  ................
-00000340: 02ff 0202 0efe 7206 0000 0063 0000 0000  ......r....c....
-00000350: 0000 0000 0000 0000 0000 0000 0d00 0000  ................
-00000360: 0000 0000 7378 0000 0065 005a 0164 005a  ....sx...e.Z.d.Z
-00000370: 0264 015a 0364 025a 0464 035a 0564 04a0  .d.Z.d.Z.d.Z.d..
-00000380: 0665 0365 04a1 025a 0764 1587 0066 0164  .e.e...Z.d...f.d
-00000390: 0764 0884 0c5a 0864 0965 0964 0a65 0a64  .d...Z.d.e.d.e.d
-000003a0: 0b65 0a64 0565 0b66 0864 0c64 0d84 045a  .e.d.e.f.d.d...Z
-000003b0: 0c09 0e64 1664 0f65 0d6a 0e64 1065 0a64  ...d.d.e.j.d.e.d
-000003c0: 0965 0964 1165 0a64 1265 0f64 0565 0966  .e.d.e.d.e.d.e.f
-000003d0: 0c64 1364 1484 055a 1087 0004 005a 1153  .d.d...Z.....Z.S
-000003e0: 0029 17da 0d52 656c 6561 7365 436c 6965  .)...ReleaseClie
-000003f0: 6e74 7a0a 6b61 736b 6164 612d 6169 da07  ntz.kaskada-ai..
-00000400: 6b61 736b 6164 61da 1347 4954 4855 425f  kaskada..GITHUB_
-00000410: 4143 4345 5353 5f54 4f4b 454e 7a32 6874  ACCESS_TOKENz2ht
-00000420: 7470 733a 2f2f 6170 692e 6769 7468 7562  tps://api.github
-00000430: 2e63 6f6d 2f72 6570 6f73 2f7b 7d2f 7b7d  .com/repos/{}/{}
-00000440: 2f72 656c 6561 7365 732f 6173 7365 7473  /releases/assets
-00000450: 720a 0000 004e 6301 0000 0000 0000 0000  r....Nc.........
-00000460: 0000 0002 0000 0003 0000 0003 0000 0073  ...............s
-00000470: 3200 0000 7400 8300 a001 a100 0100 7402  2...t.........t.
-00000480: 6a03 6a04 a005 a100 7c00 5f06 7407 a008  j.j.....|._.t...
-00000490: 7c00 6a09 a101 7d01 740a 7c01 8301 7c00  |.j...}.t.|...|.
-000004a0: 5f0b 6400 5300 720b 0000 0029 0cda 0573  _.d.S.r....)...s
-000004b0: 7570 6572 7212 0000 0072 1800 0000 da03  uperr....r......
-000004c0: 6170 69da 0961 7069 5f75 7469 6c73 da14  api..api_utils..
-000004d0: 6765 745f 706c 6174 666f 726d 5f64 6574  get_platform_det
-000004e0: 6169 6c73 da11 5f70 6c61 7466 6f72 6d5f  ails.._platform_
-000004f0: 6465 7461 696c 73da 026f 73da 0667 6574  details..os..get
-00000500: 656e 76da 1747 4954 4855 425f 4143 4345  env..GITHUB_ACCE
-00000510: 5353 5f54 4f4b 454e 5f45 4e56 7203 0000  SS_TOKEN_ENVr...
-00000520: 00da 075f 6769 7468 7562 2902 720f 0000  ..._github).r...
-00000530: 00da 0c61 6363 6573 735f 746f 6b65 6ea9  ...access_token.
-00000540: 01da 095f 5f63 6c61 7373 5f5f 7210 0000  ...__class__r...
-00000550: 0072 1100 0000 7212 0000 0025 0000 0073  .r....r....%...s
-00000560: 0800 0000 0a01 0e01 0c02 0e01 7a16 5265  ............z.Re
-00000570: 6c65 6173 6543 6c69 656e 742e 5f5f 696e  leaseClient.__in
-00000580: 6974 5f5f 7207 0000 00da 106d 616e 6167  it__r......manag
-00000590: 6572 5f62 696e 5f6e 616d 65da 0f65 6e67  er_bin_name..eng
-000005a0: 696e 655f 6269 6e5f 6e61 6d65 6304 0000  ine_bin_namec...
-000005b0: 0000 0000 0000 0000 000f 0000 0008 0000  ................
-000005c0: 0043 0000 0073 7c01 0000 6401 7c00 6a00  .C...s|...d.|.j.
-000005d0: 9b00 9d02 7d04 7401 a002 6402 7c04 9b00  ....}.t...d.|...
-000005e0: 9d02 a101 0100 6403 7c00 6a00 9b00 9d02  ......d.|.j.....
-000005f0: 7d05 7401 a002 6404 7c05 9b00 9d02 a101  }.t...d.|.......
-00000600: 0100 7403 a004 a100 7d06 7405 a006 7c00  ..t.....}.t...|.
-00000610: 6a07 a101 7d07 7c07 6405 7501 7237 7401  j...}.|.d.u.r7t.
-00000620: a002 6406 a101 0100 6407 7c07 9b00 9d02  ..d.....d.|.....
-00000630: 7c06 6a08 6408 3c00 7c00 6a09 a00a 7c00  |.j.d.<.|.j...|.
-00000640: 6a0b 9b00 6409 7c00 6a0c 9b00 9d03 a101  j...d.|.j.......
-00000650: 7d08 7c08 a00d a100 7d09 7401 a00e 640a  }.|.....}.t...d.
-00000660: 7c09 6a0f 9b00 9d02 a101 0100 7c01 7c09  |.j.........|.|.
-00000670: 6a0f 1b00 7d01 7c01 6a10 640b 640b 640c  j...}.|.j.d.d.d.
-00000680: 8d02 0100 7401 a002 640d 7c01 9b00 9d02  ....t...d.|.....
-00000690: a101 0100 7c09 a011 a100 7d0a 640e 5c02  ....|.....}.d.\.
-000006a0: 7d0b 7d0c 7c0a 4400 5d32 7d0d 7c00 6a12  }.}.|.D.]2}.|.j.
-000006b0: 9b00 6409 7c0d 6a13 9b00 9d03 7d0e 7c0d  ..d.|.j.....}.|.
-000006c0: 6a14 7c04 6b02 728e 7c00 6a15 7c06 7c0e  j.|.k.r.|.j.|.|.
-000006d0: 7c01 7c02 1b00 7c0d 6a14 7c0d 6a16 640f  |.|...|.j.|.j.d.
-000006e0: 8d05 7d0b 716f 7c0d 6a14 7c05 6b02 72a1  ..}.qo|.j.|.k.r.
-000006f0: 7c00 6a15 7c06 7c0e 7c01 7c03 1b00 7c0d  |.j.|.|.|.|...|.
-00000700: 6a14 7c0d 6a16 640f 8d05 7d0c 716f 7c0b  j.|.j.d...}.qo|.
-00000710: 6405 7500 72ad 7417 6410 7c04 9b00 9d02  d.u.r.t.d.|.....
-00000720: 8301 8201 7c0c 6405 7500 72b8 7417 6411  ....|.d.u.r.t.d.
-00000730: 7c05 9b00 9d02 8301 8201 7418 7c01 7c0b  |.........t.|.|.
-00000740: 7c0c 8303 5300 2912 61ec 0100 0044 6f77  |...S.).a....Dow
-00000750: 6e6c 6f61 6473 2074 6865 206c 6174 6573  nloads the lates
-00000760: 7420 7665 7273 696f 6e20 6f66 2074 6865  t version of the
-00000770: 206b 6173 6b61 6461 2d6d 616e 6167 6572   kaskada-manager
-00000780: 2061 6e64 206b 6173 6b61 6461 2d65 6e67   and kaskada-eng
-00000790: 696e 6520 7365 7276 6963 6573 2e0a 0a20  ine services... 
-000007a0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-000007b0: 2020 2020 2020 2020 2064 6f77 6e6c 6f61           downloa
-000007c0: 645f 7061 7468 2028 5061 7468 293a 2054  d_path (Path): T
-000007d0: 6865 206c 6f63 616c 2064 6f77 6e6c 6f61  he local downloa
-000007e0: 6420 7061 7468 0a20 2020 2020 2020 2020  d path.         
-000007f0: 2020 206d 616e 6167 6572 5f62 696e 5f6e     manager_bin_n
-00000800: 616d 6520 2873 7472 293a 2054 6865 206e  ame (str): The n
-00000810: 616d 6520 6f66 2074 6865 206d 616e 6167  ame of the manag
-00000820: 6572 2062 696e 6172 7920 746f 2073 6176  er binary to sav
-00000830: 6520 696e 2064 6f77 6e6c 6f61 6420 7061  e in download pa
-00000840: 7468 0a20 2020 2020 2020 2020 2020 2065  th.            e
-00000850: 6e67 696e 655f 6269 6e5f 6e61 6d65 2028  ngine_bin_name (
-00000860: 7374 7229 3a20 5468 6520 6e61 6d65 206f  str): The name o
-00000870: 6620 7468 6520 656e 6769 6e65 2062 696e  f the engine bin
-00000880: 6172 7920 746f 2073 6176 6520 696e 2064  ary to save in d
-00000890: 6f77 6e6c 6f61 6420 7061 7468 0a0a 2020  ownload path..  
-000008a0: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
-000008b0: 2020 2020 2020 2020 2020 5275 6e74 696d            Runtim
-000008c0: 6545 7272 6f72 3a20 756e 6162 6c65 2074  eError: unable t
-000008d0: 6f20 6765 7420 7265 6c65 6173 6520 6173  o get release as
-000008e0: 7365 7473 0a0a 2020 2020 2020 2020 5265  sets..        Re
-000008f0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00000900: 2020 2054 7570 6c65 5b73 7472 2c20 7374     Tuple[str, st
-00000910: 725d 3a20 6d61 6e61 6765 7220 7061 7468  r]: manager path
-00000920: 2061 6e64 2065 6e67 696e 6520 7061 7468   and engine path
-00000930: 0a20 2020 2020 2020 207a 106b 6173 6b61  .        z.kaska
-00000940: 6461 2d6d 616e 6167 6572 2d7a 214c 6f6f  da-manager-z!Loo
-00000950: 6b69 6e67 2066 6f72 206d 616e 6167 6572  king for manager
-00000960: 2062 696e 6172 7920 6e61 6d65 3a20 7a0f   binary name: z.
-00000970: 6b61 736b 6164 612d 656e 6769 6e65 2d7a  kaskada-engine-z
-00000980: 204c 6f6f 6b69 6e67 2066 6f72 2065 6e67   Looking for eng
-00000990: 696e 6520 6269 6e61 7279 206e 616d 653a  ine binary name:
-000009a0: 204e 7a2c 4163 6365 7373 2074 6f6b 656e   Nz,Access token
-000009b0: 2073 6574 2e20 5573 696e 6720 4769 7468   set. Using Gith
-000009c0: 7562 2041 6363 6573 7320 746f 6b65 6e2e  ub Access token.
-000009d0: 7a06 746f 6b65 6e20 da0d 4175 7468 6f72  z.token ..Author
-000009e0: 697a 6174 696f 6efa 012f 7a1e 5573 696e  ization../z.Usin
-000009f0: 6720 6c61 7465 7374 2072 656c 6561 7365  g latest release
-00000a00: 2076 6572 7369 6f6e 3a20 5429 02da 0770   version: T)...p
-00000a10: 6172 656e 7473 da08 6578 6973 745f 6f6b  arents..exist_ok
-00000a20: 7a0f 446f 776e 6c6f 6164 2070 6174 683a  z.Download path:
-00000a30: 2029 024e 4e29 01da 0966 696c 655f 7369   ).NN)...file_si
-00000a40: 7a65 7a23 756e 6162 6c65 2074 6f20 646f  zez#unable to do
-00000a50: 776e 6c6f 6164 206d 616e 6167 6572 2062  wnload manager b
-00000a60: 696e 6172 793a 207a 2275 6e61 626c 6520  inary: z"unable 
-00000a70: 746f 2064 6f77 6e6c 6f61 6420 656e 6769  to download engi
-00000a80: 6e65 2062 696e 6172 793a 2029 1972 1e00  ne binary: ).r..
-00000a90: 0000 da06 6c6f 6767 6572 da05 6465 6275  ....logger..debu
-00000aa0: 67da 0872 6571 7565 7374 73da 0753 6573  g..requests..Ses
-00000ab0: 7369 6f6e 721f 0000 0072 2000 0000 7221  sionr....r ...r!
-00000ac0: 0000 00da 0768 6561 6465 7273 7222 0000  .....headersr"..
-00000ad0: 00da 0867 6574 5f72 6570 6fda 0c4f 5247  ...get_repo..ORG
-00000ae0: 414e 495a 4154 494f 4eda 0952 4550 4f5f  ANIZATION..REPO_
-00000af0: 4e41 4d45 da12 6765 745f 6c61 7465 7374  NAME..get_latest
-00000b00: 5f72 656c 6561 7365 da04 696e 666f da08  _release..info..
-00000b10: 7461 675f 6e61 6d65 da05 6d6b 6469 72da  tag_name..mkdir.
-00000b20: 0a67 6574 5f61 7373 6574 73da 1341 5353  .get_assets..ASS
-00000b30: 4554 535f 4150 495f 454e 4450 4f49 4e54  ETS_API_ENDPOINT
-00000b40: da02 6964 da04 6e61 6d65 da18 5f52 656c  ..id..name.._Rel
-00000b50: 6561 7365 436c 6965 6e74 5f5f 646f 776e  easeClient__down
-00000b60: 6c6f 6164 da04 7369 7a65 da0c 5275 6e74  load..size..Runt
-00000b70: 696d 6545 7272 6f72 7206 0000 0029 0f72  imeErrorr....).r
-00000b80: 0f00 0000 7207 0000 0072 2600 0000 7227  ....r....r&...r'
-00000b90: 0000 00da 0c6d 616e 6167 6572 5f6e 616d  .....manager_nam
-00000ba0: 65da 0b65 6e67 696e 655f 6e61 6d65 da07  e..engine_name..
-00000bb0: 7365 7373 696f 6e72 2300 0000 da04 7265  sessionr#.....re
-00000bc0: 706f da0e 6c61 7465 7374 5f72 656c 6561  po..latest_relea
-00000bd0: 7365 da06 6173 7365 7473 7208 0000 0072  se..assetsr....r
-00000be0: 0900 0000 da05 6173 7365 74da 0375 726c  ......asset..url
-00000bf0: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-00000c00: 1764 6f77 6e6c 6f61 645f 6c61 7465 7374  .download_latest
-00000c10: 5f72 656c 6561 7365 2c00 0000 7352 0000  _release,...sR..
-00000c20: 000c 1010 010c 0110 0108 010c 0108 010a  ................
-00000c30: 0110 011a 0208 0112 010a 010e 0110 0108  ................
-00000c40: 0108 0208 0112 010a 0104 0102 0102 0106  ................
-00000c50: 0104 0104 0108 fb0a 0704 0102 0102 0106  ................
-00000c60: 0104 0104 0106 fb02 8008 080e 0108 010e  ................
-00000c70: 010c 017a 2552 656c 6561 7365 436c 6965  ...z%ReleaseClie
-00000c80: 6e74 2e64 6f77 6e6c 6f61 645f 6c61 7465  nt.download_late
-00000c90: 7374 5f72 656c 6561 7365 7201 0000 00da  st_releaser.....
-00000ca0: 0172 7247 0000 00da 0b64 6573 6372 6970  .rrG.....descrip
-00000cb0: 7469 6f6e 722c 0000 0063 0600 0000 0000  tionr,...c......
-00000cc0: 0000 0000 0000 0b00 0000 0900 0000 4300  ..............C.
-00000cd0: 0000 734c 0100 0074 00a0 0164 017c 029b  ..sL...t...d.|..
-00000ce0: 0064 027c 039b 0064 037c 059b 009d 06a1  .d.|...d.|......
-00000cf0: 0101 007c 03a0 02a1 0072 237c 03a0 03a1  ...|.....r#|....
-00000d00: 006a 047c 056b 0272 2374 00a0 0564 047c  .j.|.k.r#t...d.|
-00000d10: 039b 009d 02a1 0101 007c 0353 0064 057c  .........|.S.d.|
-00000d20: 016a 0664 063c 007c 016a 077c 0264 0764  .j.d.<.|.j.|.d.d
-00000d30: 0764 088d 037d 067c 066a 0864 096b 0372  .d...}.|.j.d.k.r
-00000d40: 417c 06a0 09a1 0001 0074 0a64 0a7c 066a  A|.......t.d.|.j
-00000d50: 089b 009d 0283 0182 017c 0564 0b6b 0272  .........|.d.k.r
-00000d60: 4e74 0b7c 016a 06a0 0764 0c64 0ba1 0283  Nt.|.j...d.d....
-00000d70: 017d 057c 0564 0b6b 0272 5464 0d6e 017c  .}.|.d.k.rTd.n.|
-00000d80: 047d 0774 0c6a 0d7c 066a 0e6a 0f64 0764  .}.t.j.|.j.j.d.d
-00000d90: 0e8d 027c 066a 0e5f 0f64 0b64 0f6c 106d  ...|.j._.d.d.l.m
-00000da0: 117d 0801 007c 086a 127c 066a 0e64 107c  .}...|.j.|.j.d.|
-00000db0: 057c 0764 118d 048f 237d 097c 03a0 1364  .|.d....#}.|...d
-00000dc0: 12a1 018f 0e7d 0a74 14a0 157c 097c 0aa1  .....}.t...|.|..
-00000dd0: 0201 0057 0064 1304 0004 0083 0301 006e  ...W.d.........n
-00000de0: 0831 0073 8877 0101 0001 0001 0059 0001  .1.s.w.......Y..
-00000df0: 0057 0064 1304 0004 0083 0301 006e 0831  .W.d.........n.1
-00000e00: 0073 9777 0101 0001 0001 0059 0001 0074  .s.w.......Y...t
-00000e10: 00a0 0164 147c 039b 009d 02a1 0101 007c  ...d.|.........|
-00000e20: 0353 0029 1561 4f02 0000 446f 776e 6c6f  .S.).aO...Downlo
-00000e30: 6164 7320 6120 5552 4c20 6173 2061 6e20  ads a URL as an 
-00000e40: 6170 706c 6963 6174 696f 6e2f 6f63 7465  application/octe
-00000e50: 742d 7374 7265 616d 0a0a 2020 2020 2020  t-stream..      
-00000e60: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00000e70: 2020 2020 7220 2872 6571 7565 7374 732e      r (requests.
-00000e80: 5365 7373 696f 6e29 3a20 5468 6520 7265  Session): The re
-00000e90: 7175 6573 7420 7365 7373 696f 6e0a 2020  quest session.  
-00000ea0: 2020 2020 2020 2020 2020 7572 6c20 2873            url (s
-00000eb0: 7472 293a 2054 6865 2074 6172 6767 6574  tr): The targget
-00000ec0: 2055 524c 0a20 2020 2020 2020 2020 2020   URL.           
-00000ed0: 2064 6f77 6e6c 6f61 645f 7061 7468 2028   download_path (
-00000ee0: 5061 7468 293a 2054 6865 206c 6f63 616c  Path): The local
-00000ef0: 2070 6174 6820 746f 2073 7472 6561 6d20   path to stream 
-00000f00: 7772 6974 6520 7468 6520 6669 6c65 0a20  write the file. 
-00000f10: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-00000f20: 6970 7469 6f6e 2028 7374 7229 3a20 5468  iption (str): Th
-00000f30: 6520 6465 7363 7269 7074 696f 6e20 746f  e description to
-00000f40: 2072 656e 6465 7220 6475 7269 6e67 2064   render during d
-00000f50: 6f77 6e6c 6f61 640a 2020 2020 2020 2020  ownload.        
-00000f60: 2020 2020 6669 6c65 5f73 697a 6520 2869      file_size (i
-00000f70: 6e74 2c20 6f70 7469 6f6e 616c 293a 2054  nt, optional): T
-00000f80: 6865 2066 696c 6520 7369 7a65 2069 6620  he file size if 
-00000f90: 6b6e 6f77 6e20 6168 6561 6420 6f66 2074  known ahead of t
-00000fa0: 696d 652e 2044 6566 6175 6c74 7320 746f  ime. Defaults to
-00000fb0: 2072 6573 706f 6e73 6520 636f 6e74 656e   response conten
-00000fc0: 7420 7369 7a65 206f 7220 302e 0a0a 2020  t size or 0...  
-00000fd0: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
-00000fe0: 2020 2020 2020 2020 2020 5275 6e74 696d            Runtim
-00000ff0: 6545 7272 6f72 3a20 556e 6162 6c65 2074  eError: Unable t
-00001000: 6f20 646f 776e 6c6f 6164 2074 6865 2074  o download the t
-00001010: 6172 6765 7420 5552 4c20 6475 6520 746f  arget URL due to
-00001020: 206e 6f6e 2032 3030 2065 7272 6f72 2063   non 200 error c
-00001030: 6f64 652e 0a0a 2020 2020 2020 2020 5265  ode...        Re
-00001040: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00001050: 2020 2050 6174 683a 2054 6865 206c 6f63     Path: The loc
-00001060: 616c 2064 6f77 6e6c 6f61 6420 7061 7468  al download path
-00001070: 0a20 2020 2020 2020 207a 0d44 6f77 6e6c  .        z.Downl
-00001080: 6f61 6469 6e67 3a20 7a04 2074 6f20 7a10  oading: z. to z.
-00001090: 2e20 436f 6e74 656e 7420 5369 7a65 3a20  . Content Size: 
-000010a0: 7a21 536b 6970 7069 6e67 2064 6f77 6e6c  z!Skipping downl
-000010b0: 6f61 642e 2055 7369 6e67 2062 696e 6172  oad. Using binar
-000010c0: 793a 207a 1861 7070 6c69 6361 7469 6f6e  y: z.application
-000010d0: 2f6f 6374 6574 2d73 7472 6561 6dda 0641  /octet-stream..A
-000010e0: 6363 6570 7454 2902 7204 0000 00da 0f61  cceptT).r......a
-000010f0: 6c6c 6f77 5f72 6564 6972 6563 7473 e9c8  llow_redirects..
-00001100: 0000 007a 3472 6571 7565 7374 2074 6f20  ...z4request to 
-00001110: 646f 776e 6c6f 6164 2062 696e 6172 7920  download binary 
-00001120: 6661 696c 6564 2077 6974 6820 7374 6174  failed with stat
-00001130: 7573 2063 6f64 653a 2072 0100 0000 7a0e  us code: r....z.
-00001140: 436f 6e74 656e 742d 4c65 6e67 7468 7a19  Content-Lengthz.
-00001150: 2855 6e6b 6e6f 776e 2074 6f74 616c 2066  (Unknown total f
-00001160: 696c 6520 7369 7a65 2929 01da 0e64 6563  ile size))...dec
-00001170: 6f64 655f 636f 6e74 656e 7429 01da 0474  ode_content)...t
-00001180: 7164 6dda 0472 6561 6429 02da 0574 6f74  qdm..read)...tot
-00001190: 616c da04 6465 7363 da02 7762 4e7a 1c53  al..desc..wbNz.S
-000011a0: 7563 6365 7373 6675 6c6c 7920 646f 776e  uccessfully down
-000011b0: 6c6f 6164 6564 2074 6f3a 2029 1672 2d00  loaded to: ).r-.
-000011c0: 0000 722e 0000 00da 0665 7869 7374 73da  ..r......exists.
-000011d0: 0473 7461 74da 0773 745f 7369 7a65 7236  .stat..st_sizer6
-000011e0: 0000 0072 3100 0000 da03 6765 74da 0b73  ...r1.....get..s
-000011f0: 7461 7475 735f 636f 6465 da10 7261 6973  tatus_code..rais
-00001200: 655f 666f 725f 7374 6174 7573 723f 0000  e_for_statusr?..
-00001210: 00da 0369 6e74 da09 6675 6e63 746f 6f6c  ...int..functool
-00001220: 73da 0770 6172 7469 616c da03 7261 7772  s..partial..rawr
-00001230: 5000 0000 da09 7471 646d 2e61 7574 6f72  P.....tqdm.autor
-00001240: 4f00 0000 da08 7772 6170 6174 7472 da04  O.....wrapattr..
-00001250: 6f70 656e da06 7368 7574 696c da0b 636f  open..shutil..co
-00001260: 7079 6669 6c65 6f62 6a29 0b72 0f00 0000  pyfileobj).r....
-00001270: 7249 0000 0072 4700 0000 7207 0000 0072  rI...rG...r....r
-00001280: 4a00 0000 722c 0000 00da 0872 6573 706f  J...r,.....respo
-00001290: 6e73 6572 5200 0000 724f 0000 00da 0572  nserR...rO.....r
-000012a0: 5f72 6177 da01 6672 1000 0000 7210 0000  _raw..fr....r...
-000012b0: 0072 1100 0000 da0a 5f5f 646f 776e 6c6f  .r......__downlo
-000012c0: 6164 6800 0000 7346 0000 0004 1714 0104  adh...sF........
-000012d0: ff16 0410 0104 010a 0210 010a 0108 0102  ................
-000012e0: 010a 0104 ff06 0402 ff12 0310 0104 0108  ................
-000012f0: 010a ff0c 0304 020a 0106 ff02 0204 0102  ................
-00001300: 0104 ff02 020e 011c fd02 801c fd10 0704  ................
-00001310: 017a 1852 656c 6561 7365 436c 6965 6e74  .z.ReleaseClient
-00001320: 2e5f 5f64 6f77 6e6c 6f61 6429 0272 0a00  .__download).r..
-00001330: 0000 4e29 0172 0100 0000 2912 7213 0000  ..N).r....).r...
-00001340: 0072 1400 0000 7215 0000 0072 3300 0000  .r....r....r3...
-00001350: 7234 0000 0072 2100 0000 da06 666f 726d  r4...r!.....form
-00001360: 6174 723a 0000 0072 1200 0000 7202 0000  atr:...r....r...
-00001370: 00da 0373 7472 7206 0000 0072 4800 0000  ...strr....rH...
-00001380: 722f 0000 0072 3000 0000 725a 0000 0072  r/...r0...rZ...r
-00001390: 3d00 0000 da0d 5f5f 636c 6173 7363 656c  =.....__classcel
-000013a0: 6c5f 5f72 1000 0000 7210 0000 0072 2400  l__r....r....r$.
-000013b0: 0000 7211 0000 0072 1700 0000 1c00 0000  ..r....r........
-000013c0: 733e 0000 0008 0004 0104 0104 0204 0104  s>..............
-000013d0: 0104 ff0e 0402 0702 0102 ff02 0102 ff02  ................
-000013e0: 0102 ff02 020a fe02 4204 fa04 0202 fe02  ........B.......
-000013f0: 0302 fd02 0402 fc02 0502 fb02 0602 fa02  ................
-00001400: 0712 f972 1700 0000 2915 725b 0000 00da  ...r....).r[....
-00001410: 076c 6f67 6769 6e67 721f 0000 0072 6100  .loggingr....ra.
-00001420: 0000 da03 7379 73da 0770 6174 686c 6962  ....sys..pathlib
-00001430: 7202 0000 0072 2f00 0000 da06 6769 7468  r....r/.....gith
-00001440: 7562 7203 0000 00da 156b 6173 6b61 6461  ubr......kaskada
-00001450: 2e61 7069 2e61 7069 5f75 7469 6c73 7218  .api.api_utilsr.
-00001460: 0000 00da 0b62 6173 6963 436f 6e66 6967  .....basicConfig
-00001470: da06 7374 646f 7574 da04 494e 464f da09  ..stdout..INFO..
-00001480: 6765 744c 6f67 6765 7272 1300 0000 722d  getLoggerr....r-
-00001490: 0000 00da 066f 626a 6563 7472 0600 0000  .....objectr....
-000014a0: 7217 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-000014b0: 1000 0000 7211 0000 00da 083c 6d6f 6475  ....r......<modu
-000014c0: 6c65 3e01 0000 0073 1a00 0000 0800 0801  le>....s........
-000014d0: 0801 0801 0801 0c01 0802 0c01 0802 1202  ................
-000014e0: 0a01 1003 140b                           ......
+000000f0: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
+00000100: 0000 7324 0000 0065 005a 0164 005a 0264  ..s$...e.Z.d.Z.d
+00000110: 015a 0365 0465 0465 0464 0264 039c 0464  .Z.e.e.e.d.d...d
+00000120: 0464 0584 045a 0564 0253 0029 06da 0c4c  .d...Z.d.S.)...L
+00000130: 6f63 616c 5265 6c65 6173 657a 4843 6f6e  ocalReleasezHCon
+00000140: 6669 6775 7261 7469 6f6e 2064 6574 6169  figuration detai
+00000150: 6c73 2066 6f72 2061 206c 6f63 616c 2072  ls for a local r
+00000160: 656c 6561 7365 2e20 4d6f 7374 6c79 2075  elease. Mostly u
+00000170: 7365 6420 666f 7220 6269 6e61 7279 2070  sed for binary p
+00000180: 6174 6873 2e4e 2904 da0d 646f 776e 6c6f  aths.N)...downlo
+00000190: 6164 5f70 6174 68da 0c6d 616e 6167 6572  ad_path..manager
+000001a0: 5f70 6174 68da 0b65 6e67 696e 655f 7061  _path..engine_pa
+000001b0: 7468 da06 7265 7475 726e 6304 0000 0000  th..returnc.....
+000001c0: 0000 0000 0000 0004 0000 0002 0000 0043  ...............C
+000001d0: 0000 0073 1600 0000 7c01 7c00 5f00 7c02  ...s....|.|._.|.
+000001e0: 7c00 5f01 7c03 7c00 5f02 6400 5300 a901  |._.|.|._.d.S...
+000001f0: 4e29 03da 0e5f 646f 776e 6c6f 6164 5f70  N)..._download_p
+00000200: 6174 68da 0d5f 6d61 6e61 6765 725f 7061  ath.._manager_pa
+00000210: 7468 da0c 5f65 6e67 696e 655f 7061 7468  th.._engine_path
+00000220: 2904 da04 7365 6c66 7207 0000 0072 0800  )...selfr....r..
+00000230: 0000 7209 0000 00a9 0072 1000 0000 fa1f  ..r......r......
+00000240: 2f73 7263 2f73 7263 2f6b 6173 6b61 6461  /src/src/kaskada
+00000250: 2f61 7069 2f72 656c 6561 7365 2e70 79da  /api/release.py.
+00000260: 085f 5f69 6e69 745f 5f14 0000 0073 0600  .__init__....s..
+00000270: 0000 0003 0601 0601 7a15 4c6f 6361 6c52  ........z.LocalR
+00000280: 656c 6561 7365 2e5f 5f69 6e69 745f 5f29  elease.__init__)
+00000290: 06da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000002a0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000002b0: 616d 655f 5fda 075f 5f64 6f63 5f5f 7202  ame__..__doc__r.
+000002c0: 0000 0072 1200 0000 7210 0000 0072 1000  ...r....r....r..
+000002d0: 0000 7210 0000 0072 1100 0000 7206 0000  ..r....r....r...
+000002e0: 0011 0000 0073 0800 0000 0801 0403 0601  .....s..........
+000002f0: 02fe 7206 0000 0063 0000 0000 0000 0000  ..r....c........
+00000300: 0000 0000 0000 0000 0800 0000 0000 0000  ................
+00000310: 736a 0000 0065 005a 0164 005a 0264 015a  sj...e.Z.d.Z.d.Z
+00000320: 0364 025a 0464 035a 0564 04a0 0665 0365  .d.Z.d.Z.d...e.e
+00000330: 04a1 025a 0764 0564 069c 0187 0066 0164  ...Z.d.d.....f.d
+00000340: 0764 0884 0c5a 0865 0965 0a65 0a65 0b64  .d...Z.e.e.e.e.d
+00000350: 099c 0464 0a64 0b84 045a 0c64 1065 0d6a  ...d.d...Z.d.e.j
+00000360: 0e65 0a65 0965 0a65 0f65 0964 0d9c 0664  .e.e.e.e.e.d...d
+00000370: 0e64 0f84 055a 1087 0004 005a 1153 0029  .d...Z.....Z.S.)
+00000380: 11da 0d52 656c 6561 7365 436c 6965 6e74  ...ReleaseClient
+00000390: 7a0a 6b61 736b 6164 612d 6169 da07 6b61  z.kaskada-ai..ka
+000003a0: 736b 6164 615a 1347 4954 4855 425f 4143  skadaZ.GITHUB_AC
+000003b0: 4345 5353 5f54 4f4b 454e 7a32 6874 7470  CESS_TOKENz2http
+000003c0: 733a 2f2f 6170 692e 6769 7468 7562 2e63  s://api.github.c
+000003d0: 6f6d 2f72 6570 6f73 2f7b 7d2f 7b7d 2f72  om/repos/{}/{}/r
+000003e0: 656c 6561 7365 732f 6173 7365 7473 4e29  eleases/assetsN)
+000003f0: 0172 0a00 0000 6301 0000 0000 0000 0000  .r....c.........
+00000400: 0000 0002 0000 0003 0000 0003 0000 0073  ...............s
+00000410: 3200 0000 7400 8300 a001 a100 0100 7402  2...t.........t.
+00000420: 6a03 6a04 a005 a100 7c00 5f06 7407 a008  j.j.....|._.t...
+00000430: 7c00 6a09 a101 7d01 740a 7c01 8301 7c00  |.j...}.t.|...|.
+00000440: 5f0b 6400 5300 720b 0000 0029 0cda 0573  _.d.S.r....)...s
+00000450: 7570 6572 7212 0000 0072 1800 0000 da03  uperr....r......
+00000460: 6170 69da 0961 7069 5f75 7469 6c73 da14  api..api_utils..
+00000470: 6765 745f 706c 6174 666f 726d 5f64 6574  get_platform_det
+00000480: 6169 6c73 da11 5f70 6c61 7466 6f72 6d5f  ails.._platform_
+00000490: 6465 7461 696c 73da 026f 73da 0667 6574  details..os..get
+000004a0: 656e 76da 1747 4954 4855 425f 4143 4345  env..GITHUB_ACCE
+000004b0: 5353 5f54 4f4b 454e 5f45 4e56 7203 0000  SS_TOKEN_ENVr...
+000004c0: 00da 075f 6769 7468 7562 2902 720f 0000  ..._github).r...
+000004d0: 00da 0c61 6363 6573 735f 746f 6b65 6ea9  ...access_token.
+000004e0: 01da 095f 5f63 6c61 7373 5f5f 7210 0000  ...__class__r...
+000004f0: 0072 1100 0000 7212 0000 0025 0000 0073  .r....r....%...s
+00000500: 0800 0000 0001 0a01 0e02 0c01 7a16 5265  ............z.Re
+00000510: 6c65 6173 6543 6c69 656e 742e 5f5f 696e  leaseClient.__in
+00000520: 6974 5f5f 2904 7207 0000 00da 106d 616e  it__).r......man
+00000530: 6167 6572 5f62 696e 5f6e 616d 65da 0f65  ager_bin_name..e
+00000540: 6e67 696e 655f 6269 6e5f 6e61 6d65 720a  ngine_bin_namer.
+00000550: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
+00000560: 0f00 0000 0800 0000 4300 0000 7382 0100  ........C...s...
+00000570: 0064 017c 006a 009b 009d 027d 0474 01a0  .d.|.j.....}.t..
+00000580: 0264 027c 049b 009d 02a1 0101 0064 037c  .d.|.........d.|
+00000590: 006a 009b 009d 027d 0574 01a0 0264 047c  .j.....}.t...d.|
+000005a0: 059b 009d 02a1 0101 0074 03a0 04a1 007d  .........t.....}
+000005b0: 0674 05a0 067c 006a 07a1 017d 077c 0764  .t...|.j...}.|.d
+000005c0: 0575 0172 6e74 01a0 0264 06a1 0101 0064  .u.rnt...d.....d
+000005d0: 077c 079b 009d 027c 066a 0864 083c 007c  .|.....|.j.d.<.|
+000005e0: 006a 09a0 0a7c 006a 0b9b 0064 097c 006a  .j...|.j...d.|.j
+000005f0: 0c9b 009d 03a1 017d 087c 08a0 0da1 007d  .......}.|.....}
+00000600: 0974 01a0 0e64 0a7c 096a 0f9b 009d 02a1  .t...d.|.j......
+00000610: 0101 007c 017c 096a 0f1b 007d 017c 016a  ...|.|.j...}.|.j
+00000620: 1064 0b64 0b64 0c8d 0201 0074 01a0 0264  .d.d.d.....t...d
+00000630: 0d7c 019b 009d 02a1 0101 007c 09a0 11a1  .|.........|....
+00000640: 007d 0a64 0e5c 027d 0b7d 0c7c 0a44 005d  .}.d.\.}.}.|.D.]
+00000650: 667d 0d7c 006a 129b 0064 097c 0d6a 139b  f}.|.j...d.|.j..
+00000660: 009d 037d 0e7c 0d6a 147c 046b 0290 0172  ...}.|.j.|.k...r
+00000670: 1e7c 006a 157c 067c 0e7c 017c 021b 007c  .|.j.|.|.|.|...|
+00000680: 0d6a 147c 0d6a 1664 0f8d 057d 0b71 de7c  .j.|.j.d...}.q.|
+00000690: 0d6a 147c 056b 0272 de7c 006a 157c 067c  .j.|.k.r.|.j.|.|
+000006a0: 0e7c 017c 031b 007c 0d6a 147c 0d6a 1664  .|.|...|.j.|.j.d
+000006b0: 0f8d 057d 0c71 de7c 0b64 0575 0090 0172  ...}.q.|.d.u...r
+000006c0: 5e74 1764 107c 049b 009d 0283 0182 017c  ^t.d.|.........|
+000006d0: 0c64 0575 0090 0172 7674 1764 117c 059b  .d.u...rvt.d.|..
+000006e0: 009d 0283 0182 0174 187c 017c 0b7c 0c83  .......t.|.|.|..
+000006f0: 0353 0029 1261 ec01 0000 446f 776e 6c6f  .S.).a....Downlo
+00000700: 6164 7320 7468 6520 6c61 7465 7374 2076  ads the latest v
+00000710: 6572 7369 6f6e 206f 6620 7468 6520 6b61  ersion of the ka
+00000720: 736b 6164 612d 6d61 6e61 6765 7220 616e  skada-manager an
+00000730: 6420 6b61 736b 6164 612d 656e 6769 6e65  d kaskada-engine
+00000740: 2073 6572 7669 6365 732e 0a0a 2020 2020   services...    
+00000750: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00000760: 2020 2020 2020 646f 776e 6c6f 6164 5f70        download_p
+00000770: 6174 6820 2850 6174 6829 3a20 5468 6520  ath (Path): The 
+00000780: 6c6f 6361 6c20 646f 776e 6c6f 6164 2070  local download p
+00000790: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+000007a0: 6d61 6e61 6765 725f 6269 6e5f 6e61 6d65  manager_bin_name
+000007b0: 2028 7374 7229 3a20 5468 6520 6e61 6d65   (str): The name
+000007c0: 206f 6620 7468 6520 6d61 6e61 6765 7220   of the manager 
+000007d0: 6269 6e61 7279 2074 6f20 7361 7665 2069  binary to save i
+000007e0: 6e20 646f 776e 6c6f 6164 2070 6174 680a  n download path.
+000007f0: 2020 2020 2020 2020 2020 2020 656e 6769              engi
+00000800: 6e65 5f62 696e 5f6e 616d 6520 2873 7472  ne_bin_name (str
+00000810: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
+00000820: 6865 2065 6e67 696e 6520 6269 6e61 7279  he engine binary
+00000830: 2074 6f20 7361 7665 2069 6e20 646f 776e   to save in down
+00000840: 6c6f 6164 2070 6174 680a 0a20 2020 2020  load path..     
+00000850: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+00000860: 2020 2020 2020 2052 756e 7469 6d65 4572         RuntimeEr
+00000870: 726f 723a 2075 6e61 626c 6520 746f 2067  ror: unable to g
+00000880: 6574 2072 656c 6561 7365 2061 7373 6574  et release asset
+00000890: 730a 0a20 2020 2020 2020 2052 6574 7572  s..        Retur
+000008a0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+000008b0: 5475 706c 655b 7374 722c 2073 7472 5d3a  Tuple[str, str]:
+000008c0: 206d 616e 6167 6572 2070 6174 6820 616e   manager path an
+000008d0: 6420 656e 6769 6e65 2070 6174 680a 2020  d engine path.  
+000008e0: 2020 2020 2020 7a10 6b61 736b 6164 612d        z.kaskada-
+000008f0: 6d61 6e61 6765 722d 7a21 4c6f 6f6b 696e  manager-z!Lookin
+00000900: 6720 666f 7220 6d61 6e61 6765 7220 6269  g for manager bi
+00000910: 6e61 7279 206e 616d 653a 207a 0f6b 6173  nary name: z.kas
+00000920: 6b61 6461 2d65 6e67 696e 652d 7a20 4c6f  kada-engine-z Lo
+00000930: 6f6b 696e 6720 666f 7220 656e 6769 6e65  oking for engine
+00000940: 2062 696e 6172 7920 6e61 6d65 3a20 4e7a   binary name: Nz
+00000950: 2c41 6363 6573 7320 746f 6b65 6e20 7365  ,Access token se
+00000960: 742e 2055 7369 6e67 2047 6974 6875 6220  t. Using Github 
+00000970: 4163 6365 7373 2074 6f6b 656e 2e7a 0674  Access token.z.t
+00000980: 6f6b 656e 20da 0d41 7574 686f 7269 7a61  oken ..Authoriza
+00000990: 7469 6f6e fa01 2f7a 1e55 7369 6e67 206c  tion../z.Using l
+000009a0: 6174 6573 7420 7265 6c65 6173 6520 7665  atest release ve
+000009b0: 7273 696f 6e3a 2054 2902 da07 7061 7265  rsion: T)...pare
+000009c0: 6e74 73da 0865 7869 7374 5f6f 6b7a 0f44  nts..exist_okz.D
+000009d0: 6f77 6e6c 6f61 6420 7061 7468 3a20 2902  ownload path: ).
+000009e0: 4e4e 2901 da09 6669 6c65 5f73 697a 657a  NN)...file_sizez
+000009f0: 2375 6e61 626c 6520 746f 2064 6f77 6e6c  #unable to downl
+00000a00: 6f61 6420 6d61 6e61 6765 7220 6269 6e61  oad manager bina
+00000a10: 7279 3a20 7a22 756e 6162 6c65 2074 6f20  ry: z"unable to 
+00000a20: 646f 776e 6c6f 6164 2065 6e67 696e 6520  download engine 
+00000a30: 6269 6e61 7279 3a20 2919 721d 0000 00da  binary: ).r.....
+00000a40: 066c 6f67 6765 72da 0564 6562 7567 da08  .logger..debug..
+00000a50: 7265 7175 6573 7473 da07 5365 7373 696f  requests..Sessio
+00000a60: 6e72 1e00 0000 721f 0000 0072 2000 0000  nr....r....r ...
+00000a70: da07 6865 6164 6572 7372 2100 0000 5a08  ..headersr!...Z.
+00000a80: 6765 745f 7265 706f da0c 4f52 4741 4e49  get_repo..ORGANI
+00000a90: 5a41 5449 4f4e da09 5245 504f 5f4e 414d  ZATION..REPO_NAM
+00000aa0: 455a 1267 6574 5f6c 6174 6573 745f 7265  EZ.get_latest_re
+00000ab0: 6c65 6173 65da 0469 6e66 6f5a 0874 6167  lease..infoZ.tag
+00000ac0: 5f6e 616d 65da 056d 6b64 6972 5a0a 6765  _name..mkdirZ.ge
+00000ad0: 745f 6173 7365 7473 da13 4153 5345 5453  t_assets..ASSETS
+00000ae0: 5f41 5049 5f45 4e44 504f 494e 54da 0269  _API_ENDPOINT..i
+00000af0: 64da 046e 616d 65da 185f 5265 6c65 6173  d..name.._Releas
+00000b00: 6543 6c69 656e 745f 5f64 6f77 6e6c 6f61  eClient__downloa
+00000b10: 64da 0473 697a 65da 0c52 756e 7469 6d65  d..size..Runtime
+00000b20: 4572 726f 7272 0600 0000 290f 720f 0000  Errorr....).r...
+00000b30: 0072 0700 0000 7225 0000 0072 2600 0000  .r....r%...r&...
+00000b40: 5a0c 6d61 6e61 6765 725f 6e61 6d65 da0b  Z.manager_name..
+00000b50: 656e 6769 6e65 5f6e 616d 65da 0773 6573  engine_name..ses
+00000b60: 7369 6f6e 7222 0000 005a 0472 6570 6f5a  sionr"...Z.repoZ
+00000b70: 0e6c 6174 6573 745f 7265 6c65 6173 65da  .latest_release.
+00000b80: 0661 7373 6574 7372 0800 0000 7209 0000  .assetsr....r...
+00000b90: 005a 0561 7373 6574 da03 7572 6c72 1000  .Z.asset..urlr..
+00000ba0: 0000 7210 0000 0072 1100 0000 da17 646f  ..r....r......do
+00000bb0: 776e 6c6f 6164 5f6c 6174 6573 745f 7265  wnload_latest_re
+00000bc0: 6c65 6173 652c 0000 0073 5000 0000 0010  lease,...sP.....
+00000bd0: 0c01 1001 0c01 1001 0801 0c01 0801 0a01  ................
+00000be0: 1002 1a01 0801 1201 0a01 0e01 1001 0802  ................
+00000bf0: 0801 0801 1201 0c01 0401 0201 0201 0601  ................
+00000c00: 0401 04fb 0807 0a01 0401 0201 0201 0601  ................
+00000c10: 0401 04fb 0808 0a01 0e01 0a01 0e01 7a25  ..............z%
+00000c20: 5265 6c65 6173 6543 6c69 656e 742e 646f  ReleaseClient.do
+00000c30: 776e 6c6f 6164 5f6c 6174 6573 745f 7265  wnload_latest_re
+00000c40: 6c65 6173 6572 0100 0000 2906 da01 7272  leaser....)...rr
+00000c50: 3e00 0000 7207 0000 00da 0b64 6573 6372  >...r......descr
+00000c60: 6970 7469 6f6e 722b 0000 0072 0a00 0000  iptionr+...r....
+00000c70: 6306 0000 0000 0000 0000 0000 000b 0000  c...............
+00000c80: 0009 0000 0043 0000 0073 5001 0000 7400  .....C...sP...t.
+00000c90: a001 6401 7c02 9b00 6402 7c03 9b00 6403  ..d.|...d.|...d.
+00000ca0: 7c05 9b00 9d06 a101 0100 7c03 a002 a100  |.........|.....
+00000cb0: 7246 7c03 a003 a100 6a04 7c05 6b02 7246  rF|.....j.|.k.rF
+00000cc0: 7400 a005 6404 7c03 9b00 9d02 a101 0100  t...d.|.........
+00000cd0: 7c03 5300 6405 7c01 6a06 6406 3c00 7c01  |.S.d.|.j.d.<.|.
+00000ce0: 6a07 7c02 6407 6407 6408 8d03 7d06 7c06  j.|.d.d.d...}.|.
+00000cf0: 6a08 6409 6b03 7282 7c06 a009 a100 0100  j.d.k.r.|.......
+00000d00: 740a 640a 7c06 6a08 9b00 9d02 8301 8201  t.d.|.j.........
+00000d10: 7c05 640b 6b02 729c 740b 7c01 6a06 a007  |.d.k.r.t.|.j...
+00000d20: 640c 640b a102 8301 7d05 7c05 640b 6b02  d.d.....}.|.d.k.
+00000d30: 72a8 640d 6e02 7c04 7d07 740c 6a0d 7c06  r.d.n.|.}.t.j.|.
+00000d40: 6a0e 6a0f 6407 640e 8d02 7c06 6a0e 5f0f  j.j.d.d...|.j._.
+00000d50: 640b 640f 6c10 6d11 7d08 0100 7c08 6a12  d.d.l.m.}...|.j.
+00000d60: 7c06 6a0e 6410 7c05 7c07 6411 8d04 8f48  |.j.d.|.|.d....H
+00000d70: 7d09 7c03 a013 6412 a101 8f1c 7d0a 7414  }.|...d.....}.t.
+00000d80: a015 7c09 7c0a a102 0100 5700 6413 0400  ..|.|.....W.d...
+00000d90: 0400 8303 0100 6e12 3100 9001 7312 3000  ......n.1...s.0.
+00000da0: 0100 0100 0100 5900 0100 5700 6413 0400  ......Y...W.d...
+00000db0: 0400 8303 0100 6e12 3100 9001 7332 3000  ......n.1...s20.
+00000dc0: 0100 0100 0100 5900 0100 7400 a001 6414  ......Y...t...d.
+00000dd0: 7c03 9b00 9d02 a101 0100 7c03 5300 2915  |.........|.S.).
+00000de0: 614f 0200 0044 6f77 6e6c 6f61 6473 2061  aO...Downloads a
+00000df0: 2055 524c 2061 7320 616e 2061 7070 6c69   URL as an appli
+00000e00: 6361 7469 6f6e 2f6f 6374 6574 2d73 7472  cation/octet-str
+00000e10: 6561 6d0a 0a20 2020 2020 2020 2041 7267  eam..        Arg
+00000e20: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+00000e30: 2028 7265 7175 6573 7473 2e53 6573 7369   (requests.Sessi
+00000e40: 6f6e 293a 2054 6865 2072 6571 7565 7374  on): The request
+00000e50: 2073 6573 7369 6f6e 0a20 2020 2020 2020   session.       
+00000e60: 2020 2020 2075 726c 2028 7374 7229 3a20       url (str): 
+00000e70: 5468 6520 7461 7267 6765 7420 5552 4c0a  The targget URL.
+00000e80: 2020 2020 2020 2020 2020 2020 646f 776e              down
+00000e90: 6c6f 6164 5f70 6174 6820 2850 6174 6829  load_path (Path)
+00000ea0: 3a20 5468 6520 6c6f 6361 6c20 7061 7468  : The local path
+00000eb0: 2074 6f20 7374 7265 616d 2077 7269 7465   to stream write
+00000ec0: 2074 6865 2066 696c 650a 2020 2020 2020   the file.      
+00000ed0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00000ee0: 6e20 2873 7472 293a 2054 6865 2064 6573  n (str): The des
+00000ef0: 6372 6970 7469 6f6e 2074 6f20 7265 6e64  cription to rend
+00000f00: 6572 2064 7572 696e 6720 646f 776e 6c6f  er during downlo
+00000f10: 6164 0a20 2020 2020 2020 2020 2020 2066  ad.            f
+00000f20: 696c 655f 7369 7a65 2028 696e 742c 206f  ile_size (int, o
+00000f30: 7074 696f 6e61 6c29 3a20 5468 6520 6669  ptional): The fi
+00000f40: 6c65 2073 697a 6520 6966 206b 6e6f 776e  le size if known
+00000f50: 2061 6865 6164 206f 6620 7469 6d65 2e20   ahead of time. 
+00000f60: 4465 6661 756c 7473 2074 6f20 7265 7370  Defaults to resp
+00000f70: 6f6e 7365 2063 6f6e 7465 6e74 2073 697a  onse content siz
+00000f80: 6520 6f72 2030 2e0a 0a20 2020 2020 2020  e or 0...       
+00000f90: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+00000fa0: 2020 2020 2052 756e 7469 6d65 4572 726f       RuntimeErro
+00000fb0: 723a 2055 6e61 626c 6520 746f 2064 6f77  r: Unable to dow
+00000fc0: 6e6c 6f61 6420 7468 6520 7461 7267 6574  nload the target
+00000fd0: 2055 524c 2064 7565 2074 6f20 6e6f 6e20   URL due to non 
+00000fe0: 3230 3020 6572 726f 7220 636f 6465 2e0a  200 error code..
+00000ff0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00001000: 3a0a 2020 2020 2020 2020 2020 2020 5061  :.            Pa
+00001010: 7468 3a20 5468 6520 6c6f 6361 6c20 646f  th: The local do
+00001020: 776e 6c6f 6164 2070 6174 680a 2020 2020  wnload path.    
+00001030: 2020 2020 7a0d 446f 776e 6c6f 6164 696e      z.Downloadin
+00001040: 673a 207a 0420 746f 207a 102e 2043 6f6e  g: z. to z.. Con
+00001050: 7465 6e74 2053 697a 653a 207a 2153 6b69  tent Size: z!Ski
+00001060: 7070 696e 6720 646f 776e 6c6f 6164 2e20  pping download. 
+00001070: 5573 696e 6720 6269 6e61 7279 3a20 7a18  Using binary: z.
+00001080: 6170 706c 6963 6174 696f 6e2f 6f63 7465  application/octe
+00001090: 742d 7374 7265 616d da06 4163 6365 7074  t-stream..Accept
+000010a0: 5429 0272 0400 0000 da0f 616c 6c6f 775f  T).r......allow_
+000010b0: 7265 6469 7265 6374 73e9 c800 0000 7a34  redirects.....z4
+000010c0: 7265 7175 6573 7420 746f 2064 6f77 6e6c  request to downl
+000010d0: 6f61 6420 6269 6e61 7279 2066 6169 6c65  oad binary faile
+000010e0: 6420 7769 7468 2073 7461 7475 7320 636f  d with status co
+000010f0: 6465 3a20 7201 0000 007a 0e43 6f6e 7465  de: r....z.Conte
+00001100: 6e74 2d4c 656e 6774 687a 1928 556e 6b6e  nt-Lengthz.(Unkn
+00001110: 6f77 6e20 746f 7461 6c20 6669 6c65 2073  own total file s
+00001120: 697a 6529 2901 da0e 6465 636f 6465 5f63  ize))...decode_c
+00001130: 6f6e 7465 6e74 2901 da04 7471 646d da04  ontent)...tqdm..
+00001140: 7265 6164 2902 da05 746f 7461 6cda 0464  read)...total..d
+00001150: 6573 63da 0277 624e 7a1c 5375 6363 6573  esc..wbNz.Succes
+00001160: 7366 756c 6c79 2064 6f77 6e6c 6f61 6465  sfully downloade
+00001170: 6420 746f 3a20 2916 722c 0000 0072 2d00  d to: ).r,...r-.
+00001180: 0000 da06 6578 6973 7473 da04 7374 6174  ....exists..stat
+00001190: da07 7374 5f73 697a 6572 3300 0000 7230  ..st_sizer3...r0
+000011a0: 0000 00da 0367 6574 da0b 7374 6174 7573  .....get..status
+000011b0: 5f63 6f64 65da 1072 6169 7365 5f66 6f72  _code..raise_for
+000011c0: 5f73 7461 7475 7372 3a00 0000 da03 696e  _statusr:.....in
+000011d0: 74da 0966 756e 6374 6f6f 6c73 da07 7061  t..functools..pa
+000011e0: 7274 6961 6cda 0372 6177 7247 0000 005a  rtial..rawrG...Z
+000011f0: 0974 7164 6d2e 6175 746f 7246 0000 005a  .tqdm.autorF...Z
+00001200: 0877 7261 7061 7474 72da 046f 7065 6eda  .wrapattr..open.
+00001210: 0673 6875 7469 6cda 0b63 6f70 7966 696c  .shutil..copyfil
+00001220: 656f 626a 290b 720f 0000 0072 4000 0000  eobj).r....r@...
+00001230: 723e 0000 0072 0700 0000 7241 0000 0072  r>...r....rA...r
+00001240: 2b00 0000 da08 7265 7370 6f6e 7365 7249  +.....responserI
+00001250: 0000 0072 4600 0000 5a05 725f 7261 77da  ...rF...Z.r_raw.
+00001260: 0166 7210 0000 0072 1000 0000 7211 0000  .fr....r....r...
+00001270: 005a 0a5f 5f64 6f77 6e6c 6f61 6468 0000  .Z.__downloadh..
+00001280: 0073 4000 0000 0017 0401 14ff 0404 1601  .s@.............
+00001290: 1001 0402 0a01 1001 0a01 0801 0201 0aff  ................
+000012a0: 0404 06ff 0203 1201 1001 0401 08ff 0a03  ................
+000012b0: 0c02 0401 0aff 0602 0201 0401 02ff 0402  ................
+000012c0: 0201 4c01 1001 7a18 5265 6c65 6173 6543  ..L...z.ReleaseC
+000012d0: 6c69 656e 742e 5f5f 646f 776e 6c6f 6164  lient.__download
+000012e0: 2901 7201 0000 0029 1272 1300 0000 7214  ).r....).r....r.
+000012f0: 0000 0072 1500 0000 7231 0000 0072 3200  ...r....r1...r2.
+00001300: 0000 7220 0000 00da 0666 6f72 6d61 7472  ..r .....formatr
+00001310: 3500 0000 7212 0000 0072 0200 0000 da03  5...r....r......
+00001320: 7374 7272 0600 0000 723f 0000 0072 2e00  strr....r?...r..
+00001330: 0000 722f 0000 0072 5100 0000 7238 0000  ..r/...rQ...r8..
+00001340: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00001350: 7210 0000 0072 1000 0000 7223 0000 0072  r....r....r#...r
+00001360: 1100 0000 7217 0000 001c 0000 0073 2600  ....r........s&.
+00001370: 0000 0801 0401 0402 0401 0401 04ff 0404  ................
+00001380: 1208 0601 02fe 0c42 00fa 0202 0401 0201  .......B........
+00001390: 0201 0201 0201 02f9 7217 0000 0029 1572  ........r....).r
+000013a0: 5200 0000 da07 6c6f 6767 696e 6772 1e00  R.....loggingr..
+000013b0: 0000 7256 0000 00da 0373 7973 da07 7061  ..rV.....sys..pa
+000013c0: 7468 6c69 6272 0200 0000 722e 0000 005a  thlibr....r....Z
+000013d0: 0667 6974 6875 6272 0300 0000 5a15 6b61  .githubr....Z.ka
+000013e0: 736b 6164 612e 6170 692e 6170 695f 7574  skada.api.api_ut
+000013f0: 696c 7372 1800 0000 da0b 6261 7369 6343  ilsr......basicC
+00001400: 6f6e 6669 67da 0673 7464 6f75 74da 0449  onfig..stdout..I
+00001410: 4e46 4fda 0967 6574 4c6f 6767 6572 7213  NFO..getLoggerr.
+00001420: 0000 0072 2c00 0000 da06 6f62 6a65 6374  ...r,.....object
+00001430: 7206 0000 0072 1700 0000 7210 0000 0072  r....r....r....r
+00001440: 1000 0000 7210 0000 0072 1100 0000 da08  ....r....r......
+00001450: 3c6d 6f64 756c 653e 0100 0000 7318 0000  <module>....s...
+00001460: 0008 0108 0108 0108 0108 010c 0208 010c  ................
+00001470: 0208 0212 010a 0310 0b                   .........
```

### Comparing `kaskada-0.1.4/src/kaskada/api/__pycache__/session.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/api/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 22:38:35 2023 UTC, .py size: 8961 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6be1 3564 0123 0000  o.......k.5d.#..
+00000000: 610d 0d0a 0000 0000 e270 4064 1f25 0000  a........p@d.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
@@ -18,533 +18,555 @@
 00000110: 2912 e900 0000 004e 2901 da03 4142 4329  )......N)...ABC)
 00000120: 01da 0450 6174 6829 01da 0550 6f70 656e  ...Path)...Popen
 00000130: 2904 da03 416e 79da 0444 6963 74da 084f  )...Any..Dict..O
 00000140: 7074 696f 6e61 6cda 0554 7570 6c65 2902  ptional..Tuple).
 00000150: da09 6170 695f 7574 696c 73da 0772 656c  ..api_utils..rel
 00000160: 6561 7365 2902 da06 7374 7265 616d da05  ease)...stream..
 00000170: 6c65 7665 6c63 0000 0000 0000 0000 0000  levelc..........
-00000180: 0000 0000 0000 0f00 0000 4000 0000 7356  ..........@...sV
-00000190: 0000 0065 005a 0164 005a 0209 0109 0109  ...e.Z.d.Z......
-000001a0: 0164 0f64 0265 0364 0365 0464 0465 0364  .d.d.e.d.e.d.e.d
-000001b0: 0565 0565 0319 0064 0665 0565 0619 0064  .e.e...d.e.e...d
-000001c0: 0765 0565 0619 0064 0864 0166 0e64 0964  .e.e...d.d.f.d.d
-000001d0: 0a84 055a 0764 0b64 0c84 005a 0864 0d64  ...Z.d.d...Z.d.d
-000001e0: 0e84 005a 0964 0153 0029 10da 0753 6573  ...Z.d.S.)...Ses
-000001f0: 7369 6f6e 4eda 0865 6e64 706f 696e 74da  sionN..endpoint.
-00000200: 0969 735f 7365 6375 7265 da04 6e61 6d65  .is_secure..name
-00000210: da09 636c 6965 6e74 5f69 64da 0f6d 616e  ..client_id..man
-00000220: 6167 6572 5f70 726f 6365 7373 da0e 656e  ager_process..en
-00000230: 6769 6e65 5f70 726f 6365 7373 da06 7265  gine_process..re
-00000240: 7475 726e 6307 0000 0000 0000 0000 0000  turnc...........
-00000250: 0007 0000 0002 0000 0043 0000 0073 3200  .........C...s2.
-00000260: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7c03  ..|.|._.|.|._.|.
-00000270: 7c00 5f02 7c04 7c00 5f03 7c00 a004 a100  |._.|.|._.|.....
-00000280: 7c00 5f05 7c05 7c00 5f06 7c06 7c00 5f07  |._.|.|._.|.|._.
-00000290: 6400 5300 a901 4e29 08da 095f 656e 6470  d.S...N)..._endp
-000002a0: 6f69 6e74 da0a 5f69 735f 7365 6375 7265  oint.._is_secure
-000002b0: da05 5f6e 616d 65da 0a5f 636c 6965 6e74  .._name.._client
-000002c0: 5f69 64da 0763 6f6e 6e65 6374 da07 5f63  _id..connect.._c
-000002d0: 6c69 656e 74da 105f 6d61 6e61 6765 725f  lient.._manager_
-000002e0: 7072 6f63 6573 73da 0f5f 656e 6769 6e65  process.._engine
-000002f0: 5f70 726f 6365 7373 2907 da04 7365 6c66  _process)...self
-00000300: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00000310: 1100 0000 7212 0000 0072 1300 0000 a900  ....r....r......
-00000320: 721f 0000 00fa 612f 686f 6d65 2f74 6865  r.....a/home/the
-00000330: 7261 706f 6e2f 5265 706f 732f 4769 7448  rapon/Repos/GitH
-00000340: 7562 2f4b 6173 6b61 6461 4149 2f6b 6173  ub/KaskadaAI/kas
-00000350: 6b61 6461 2f72 656c 6561 7369 6e67 2f63  kada/releasing/c
-00000360: 6c69 656e 7473 2f70 7974 686f 6e2f 7372  lients/python/sr
-00000370: 632f 6b61 736b 6164 612f 6170 692f 7365  c/kaskada/api/se
-00000380: 7373 696f 6e2e 7079 da08 5f5f 696e 6974  ssion.py..__init
-00000390: 5f5f 1300 0000 730e 0000 0006 0906 0106  __....s.........
-000003a0: 0106 010a 0106 010a 017a 1053 6573 7369  .........z.Sessi
-000003b0: 6f6e 2e5f 5f69 6e69 745f 5f63 0100 0000  on.__init__c....
-000003c0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000003d0: 4300 0000 7344 0000 007c 006a 0064 0075  C...sD...|.j.d.u
-000003e0: 0172 0f74 01a0 0264 01a1 0101 007c 006a  .r.t...d.....|.j
-000003f0: 00a0 03a1 0001 007c 006a 0464 0075 0172  .......|.j.d.u.r
-00000400: 2074 01a0 0264 02a1 0101 007c 006a 04a0   t...d.....|.j..
-00000410: 03a1 0001 0064 0053 0064 0053 0029 034e  .....d.S.d.S.).N
-00000420: 7a20 5374 6f70 7069 6e67 204b 6173 6b61  z Stopping Kaska
-00000430: 6461 204d 616e 6167 6572 2073 6572 7669  da Manager servi
-00000440: 6365 7a1f 5374 6f70 7069 6e67 204b 6173  cez.Stopping Kas
-00000450: 6b61 6461 2045 6e67 696e 6520 7365 7276  kada Engine serv
-00000460: 6963 6529 0572 1c00 0000 da06 6c6f 6767  ice).r......logg
-00000470: 6572 da04 696e 666f da04 6b69 6c6c 721d  er..info..killr.
-00000480: 0000 00a9 0172 1e00 0000 721f 0000 0072  .....r....r....r
-00000490: 1f00 0000 7220 0000 00da 075f 5f64 656c  ....r .....__del
-000004a0: 5f5f 2400 0000 730e 0000 000a 010a 010a  __$...s.........
-000004b0: 010a 020a 010e 0104 fe7a 0f53 6573 7369  .........z.Sessi
-000004c0: 6f6e 2e5f 5f64 656c 5f5f 6301 0000 0000  on.__del__c.....
-000004d0: 0000 0000 0000 0003 0000 0006 0000 0043  ...............C
-000004e0: 0000 0073 9400 0000 6401 7d01 6402 7d02  ...s....d.}.d.}.
-000004f0: 7c01 6403 6b00 7234 7c02 7334 7400 a001  |.d.k.r4|.s4t...
-00000500: 6404 7c01 9b00 6405 7c00 6a02 9b00 9d04  d.|...d.|.j.....
-00000510: a101 0100 7403 a004 7c00 6a02 a101 7223  ....t...|.j...r#
-00000520: 7400 a005 6406 a101 0100 6407 7d02 7c01  t...d.....d.}.|.
-00000530: 6408 3700 7d01 7406 a007 6409 7c01 1300  d.7.}.t...d.|...
-00000540: a101 0100 7c01 6403 6b00 7234 7c02 720a  ....|.d.k.r4|.r.
-00000550: 7c02 6402 6b02 723f 7408 640a a009 7c01  |.d.k.r?t.d...|.
-00000560: a101 8301 8201 740a 6a0b a00c 7c00 6a0d  ......t.j...|.j.
-00000570: 7c00 6a02 7c00 6a0e a103 5300 290b 4e72  |.j.|.j...S.).Nr
-00000580: 0100 0000 46e9 0300 0000 7a11 4174 7465  ....F.....z.Atte
-00000590: 6d70 7469 6e67 2028 7472 7920 237a 1029  mpting (try #z.)
-000005a0: 2074 6f20 636f 6e6e 6563 7420 746f 207a   to connect to z
-000005b0: 2253 7563 6365 7373 6675 6c6c 7920 636f  "Successfully co
-000005c0: 6e6e 6563 7465 6420 746f 2073 6573 7369  nnected to sessi
-000005d0: 6f6e 2e54 e901 0000 0067 0000 0000 0000  on.T.....g......
-000005e0: f83f 7a38 756e 6162 6c65 2074 6f20 636f  .?z8unable to co
-000005f0: 6e6e 6563 7420 746f 204d 616e 6167 6572  nnect to Manager
-00000600: 206f 7220 456e 6769 6e65 2061 6674 6572   or Engine after
-00000610: 207b 7d20 6174 7465 6d70 7473 290f 7222   {} attempts).r"
-00000620: 0000 00da 0564 6562 7567 7216 0000 0072  .....debugr....r
-00000630: 0900 0000 da0c 6368 6563 6b5f 736f 636b  ......check_sock
-00000640: 6574 7223 0000 00da 0474 696d 65da 0573  etr#.....time..s
-00000650: 6c65 6570 da0f 436f 6e6e 6563 7469 6f6e  leep..Connection
-00000660: 4572 726f 72da 0666 6f72 6d61 74da 076b  Error..format..k
-00000670: 6173 6b61 6461 da06 636c 6965 6e74 da04  askada..client..
-00000680: 696e 6974 7219 0000 0072 1700 0000 2903  initr....r....).
-00000690: 721e 0000 00da 0761 7474 656d 7074 da10  r......attempt..
-000006a0: 6973 5f76 616c 6964 5f73 6573 7369 6f6e  is_valid_session
-000006b0: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-000006c0: 1a00 0000 2d00 0000 7322 0000 0004 0104  ....-...s"......
-000006d0: 010c 0118 010c 010a 0104 0108 010e 020c  ................
-000006e0: f908 0802 0104 0102 0102 ff04 ff16 057a  ...............z
-000006f0: 0f53 6573 7369 6f6e 2e63 6f6e 6e65 6374  .Session.connect
-00000700: 2903 4e4e 4e29 0ada 085f 5f6e 616d 655f  ).NNN)...__name_
-00000710: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000720: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
-00000730: da04 626f 6f6c 7207 0000 0072 0400 0000  ..boolr....r....
-00000740: 7221 0000 0072 2600 0000 721a 0000 0072  r!...r&...r....r
-00000750: 1f00 0000 721f 0000 0072 1f00 0000 7220  ....r....r....r 
-00000760: 0000 0072 0d00 0000 1200 0000 732a 0000  ...r........s*..
-00000770: 0008 0002 0602 0102 0104 f902 0202 fe02  ................
-00000780: 0302 fd02 0402 fc06 0502 fb06 0602 fa06  ................
-00000790: 0702 f902 080a f808 110c 0972 0d00 0000  ...........r....
-000007a0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000007b0: 000b 0000 0000 0000 0073 7e00 0000 6500  .........s~...e.
-000007c0: 5a01 6400 5a02 6401 6401 6503 6504 a005  Z.d.Z.d.d.e.e...
-000007d0: a100 8301 6401 6604 6402 6506 6503 1900  ....d.f.d.e.e...
-000007e0: 6403 6506 6507 1900 6404 6503 6405 6506  d.e.e...d.e.d.e.
-000007f0: 6503 1900 6406 6401 660a 8700 6601 6407  e...d.d.f...f.d.
-00000800: 6408 840d 5a08 6402 6503 6403 6507 6604  d...Z.d.e.d.e.f.
-00000810: 6409 640a 8404 5a09 6404 6503 6602 640b  d.d...Z.d.e.f.d.
-00000820: 640c 8404 5a0a 6405 6503 6602 640d 640e  d...Z.d.e.f.d.d.
-00000830: 8404 5a0b 8700 0400 5a0c 5300 290f da07  ..Z.....Z.S.)...
-00000840: 4275 696c 6465 724e 720e 0000 0072 0f00  BuilderNr....r..
-00000850: 0000 7210 0000 0072 1100 0000 7214 0000  ..r....r....r...
-00000860: 0063 0500 0000 0000 0000 0000 0000 0500  .c..............
-00000870: 0000 0200 0000 0300 0000 7326 0000 0074  ..........s&...t
-00000880: 0083 00a0 01a1 0001 007c 017c 005f 027c  .........|.|._.|
-00000890: 027c 005f 037c 037c 005f 047c 047c 005f  .|._.|.|._.|.|._
-000008a0: 0564 0053 0072 1500 0000 2906 da05 7375  .d.S.r....)...su
-000008b0: 7065 7272 2100 0000 7216 0000 0072 1700  perr!...r....r..
-000008c0: 0000 7218 0000 0072 1900 0000 2905 721e  ..r....r....).r.
-000008d0: 0000 0072 0e00 0000 720f 0000 0072 1000  ...r....r....r..
-000008e0: 0000 7211 0000 00a9 01da 095f 5f63 6c61  ..r........__cla
-000008f0: 7373 5f5f 721f 0000 0072 2000 0000 7221  ss__r....r ...r!
-00000900: 0000 0042 0000 0073 0a00 0000 0a07 0601  ...B...s........
-00000910: 0601 0601 0a01 7a10 4275 696c 6465 722e  ......z.Builder.
-00000920: 5f5f 696e 6974 5f5f 6303 0000 0000 0000  __init__c.......
-00000930: 0000 0000 0003 0000 0002 0000 0043 0000  .............C..
-00000940: 0073 1000 0000 7c01 7c00 5f00 7c02 7c00  .s....|.|._.|.|.
-00000950: 5f01 7c00 5300 7215 0000 0029 0272 1600  _.|.S.r....).r..
-00000960: 0000 7217 0000 00a9 0372 1e00 0000 720e  ..r......r....r.
-00000970: 0000 0072 0f00 0000 721f 0000 0072 1f00  ...r....r....r..
-00000980: 0000 7220 0000 0072 0e00 0000 4f00 0000  ..r ...r....O...
-00000990: 7306 0000 0006 0106 0104 017a 1042 7569  s..........z.Bui
-000009a0: 6c64 6572 2e65 6e64 706f 696e 7463 0200  lder.endpointc..
-000009b0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-000009c0: 0000 4300 0000 f30a 0000 007c 017c 005f  ..C........|.|._
-000009d0: 007c 0053 0072 1500 0000 2901 7218 0000  .|.S.r....).r...
-000009e0: 0029 0272 1e00 0000 7210 0000 0072 1f00  .).r....r....r..
-000009f0: 0000 721f 0000 0072 2000 0000 7210 0000  ..r....r ...r...
-00000a00: 0054 0000 00f3 0400 0000 0601 0401 7a0c  .T............z.
-00000a10: 4275 696c 6465 722e 6e61 6d65 6302 0000  Builder.namec...
-00000a20: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00000a30: 0043 0000 0072 3e00 0000 7215 0000 0029  .C...r>...r....)
-00000a40: 0172 1900 0000 2902 721e 0000 0072 1100  .r....).r....r..
-00000a50: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00000a60: 0072 1100 0000 5800 0000 723f 0000 007a  .r....X...r?...z
-00000a70: 1142 7569 6c64 6572 2e63 6c69 656e 745f  .Builder.client_
-00000a80: 6964 290d 7234 0000 0072 3500 0000 7236  id).r4...r5...r6
-00000a90: 0000 0072 3700 0000 da04 7575 6964 da05  ...r7.....uuid..
-00000aa0: 7575 6964 3472 0700 0000 7238 0000 0072  uuid4r....r8...r
-00000ab0: 2100 0000 720e 0000 0072 1000 0000 7211  !...r....r....r.
-00000ac0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00000ad0: 5f5f 721f 0000 0072 1f00 0000 723b 0000  __r....r....r;..
-00000ae0: 0072 2000 0000 7239 0000 0041 0000 0073  .r ...r9...A...s
-00000af0: 2600 0000 0800 0203 0201 0a01 0201 04fb  &...............
-00000b00: 0602 02fe 0603 02fd 0204 02fc 0605 02fb  ................
-00000b10: 0206 0efa 120d 0e05 1604 7239 0000 007a  ..........r9...z
-00000b20: 0f6c 6f63 616c 686f 7374 3a35 3030 3531  .localhost:50051
-00000b30: 4663 0000 0000 0000 0000 0000 0000 0000  Fc..............
-00000b40: 0000 0700 0000 0000 0000 7304 0100 0065  ..........s....e
-00000b50: 005a 0164 005a 0264 015a 0364 025a 0464  .Z.d.Z.d.Z.d.Z.d
-00000b60: 035a 0564 045a 0664 055a 0764 065a 0864  .Z.d.Z.d.Z.d.Z.d
-00000b70: 075a 0964 085a 0a65 0b65 0c66 0264 0965  .Z.d.Z.e.e.f.d.e
-00000b80: 0d64 0a65 0e64 0b64 0c66 0687 0066 0164  .d.e.d.d.f...f.d
-00000b90: 0d64 0e84 0d5a 0f64 0f65 0d66 0264 1064  .d...Z.d.e.f.d.d
-00000ba0: 1184 045a 1064 0f65 0d66 0264 1264 1384  ...Z.d.e.f.d.d..
-00000bb0: 045a 1164 0f65 0d66 0264 1464 1584 045a  .Z.d.e.f.d.d...Z
-00000bc0: 1264 1665 0e66 0264 1764 1884 045a 1364  .d.e.f.d.d...Z.d
-00000bd0: 1965 1466 0264 1a64 1b84 045a 1564 1965  .e.f.d.d...Z.d.e
-00000be0: 1466 0264 1c64 1d84 045a 1664 1e64 1f84  .f.d.d...Z.d.d..
-00000bf0: 005a 1764 2065 0d64 0b65 1866 0464 2164  .Z.d e.d.e.f.d!d
-00000c00: 2284 045a 1964 2365 0d64 0b65 1a65 1865  "..Z.d#e.d.e.e.e
-00000c10: 1866 0219 0066 0464 2464 2584 045a 1b64  .f...f.d$d%..Z.d
-00000c20: 0b65 1866 0264 2664 2784 045a 1c64 2864  .e.f.d&d'..Z.d(d
-00000c30: 2984 005a 1d64 2a64 2b84 005a 1e64 0b65  )..Z.d*d+..Z.d.e
-00000c40: 1f66 0264 2c64 2d84 045a 2087 0004 005a  .f.d,d-..Z ....Z
-00000c50: 2153 0029 2eda 0c4c 6f63 616c 4275 696c  !S.)...LocalBuil
-00000c60: 6465 72da 0c4b 4153 4b41 4441 5f50 4154  der..KASKADA_PAT
-00000c70: 487a 107e 2f2e 6361 6368 652f 6b61 736b  Hz.~/.cache/kask
-00000c80: 6164 61da 046c 6f67 73da 104b 4153 4b41  ada..logs..KASKA
-00000c90: 4441 5f4c 4f47 5f50 4154 48da 0362 696e  DA_LOG_PATH..bin
-00000ca0: da10 4b41 534b 4144 415f 4249 4e5f 5041  ..KASKADA_BIN_PA
-00000cb0: 5448 7a0f 6b61 736b 6164 612d 6d61 6e61  THz.kaskada-mana
-00000cc0: 6765 727a 0e6b 6173 6b61 6461 2d65 6e67  gerz.kaskada-eng
-00000cd0: 696e 6572 0e00 0000 720f 0000 0072 1400  iner....r....r..
-00000ce0: 0000 4e63 0300 0000 0000 0000 0000 0000  ..Nc............
-00000cf0: 0300 0000 0400 0000 0300 0000 735c 0000  ............s\..
-00000d00: 0074 0083 00a0 01a1 0001 0074 02a0 0374  .t.........t...t
-00000d10: 046a 0574 046a 06a1 027c 005f 0774 02a0  .j.t.j...|._.t..
-00000d20: 0374 046a 0874 046a 09a1 027c 005f 0a74  .t.j.t.j...|._.t
-00000d30: 02a0 0374 046a 0b74 046a 0ca1 027c 005f  ...t.j.t.j...|._
-00000d40: 0d7c 00a0 0e7c 017c 02a1 0201 0064 017c  .|...|.|.....d.|
-00000d50: 005f 0f69 007c 005f 1064 0053 0029 024e  ._.i.|._.d.S.).N
-00000d60: 5429 1172 3a00 0000 7221 0000 00da 026f  T).r:...r!.....o
-00000d70: 73da 0667 6574 656e 7672 4300 0000 da10  s..getenvrC.....
-00000d80: 4b41 534b 4144 415f 5041 5448 5f45 4e56  KASKADA_PATH_ENV
-00000d90: da14 4b41 534b 4144 415f 5041 5448 5f44  ..KASKADA_PATH_D
-00000da0: 4546 4155 4c54 da05 5f70 6174 68da 144b  EFAULT.._path..K
-00000db0: 4153 4b41 4441 5f42 494e 5f50 4154 485f  ASKADA_BIN_PATH_
-00000dc0: 454e 56da 184b 4153 4b41 4441 5f42 494e  ENV..KASKADA_BIN
-00000dd0: 5f50 4154 485f 4445 4641 554c 54da 095f  _PATH_DEFAULT.._
-00000de0: 6269 6e5f 7061 7468 da14 4b41 534b 4144  bin_path..KASKAD
-00000df0: 415f 4c4f 475f 5041 5448 5f45 4e56 da18  A_LOG_PATH_ENV..
-00000e00: 4b41 534b 4144 415f 4c4f 475f 5041 5448  KASKADA_LOG_PATH
-00000e10: 5f44 4546 4155 4c54 da09 5f6c 6f67 5f70  _DEFAULT.._log_p
-00000e20: 6174 6872 0e00 0000 da09 5f64 6f77 6e6c  athr......_downl
-00000e30: 6f61 64da 105f 6d61 6e61 6765 725f 636f  oad.._manager_co
-00000e40: 6e66 6967 7372 3d00 0000 723b 0000 0072  nfigsr=...r;...r
-00000e50: 1f00 0000 7220 0000 0072 2100 0000 6c00  ....r ...r!...l.
-00000e60: 0000 731a 0000 000a 0504 0108 0106 ff04  ..s.............
-00000e70: 0308 0106 ff04 0308 0106 ff0c 0306 010a  ................
-00000e80: 017a 154c 6f63 616c 4275 696c 6465 722e  .z.LocalBuilder.
-00000e90: 5f5f 696e 6974 5f5f da04 7061 7468 6302  __init__..pathc.
-00000ea0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000eb0: 0000 0043 0000 0072 3e00 0000 7215 0000  ...C...r>...r...
-00000ec0: 0029 0172 4d00 0000 a902 721e 0000 0072  .).rM.....r....r
-00000ed0: 5600 0000 721f 0000 0072 1f00 0000 7220  V...r....r....r 
-00000ee0: 0000 0072 5600 0000 7f00 0000 723f 0000  ...rV.......r?..
-00000ef0: 007a 114c 6f63 616c 4275 696c 6465 722e  .z.LocalBuilder.
-00000f00: 7061 7468 6302 0000 0000 0000 0000 0000  pathc...........
-00000f10: 0002 0000 0002 0000 0043 0000 0072 3e00  .........C...r>.
-00000f20: 0000 7215 0000 0029 0172 5300 0000 7257  ..r....).rS...rW
-00000f30: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
-00000f40: 0000 da08 6c6f 675f 7061 7468 8300 0000  ....log_path....
-00000f50: 723f 0000 007a 154c 6f63 616c 4275 696c  r?...z.LocalBuil
-00000f60: 6465 722e 6c6f 675f 7061 7468 6302 0000  der.log_pathc...
-00000f70: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00000f80: 0043 0000 0072 3e00 0000 7215 0000 0029  .C...r>...r....)
-00000f90: 0172 5000 0000 7257 0000 0072 1f00 0000  .rP...rW...r....
-00000fa0: 721f 0000 0072 2000 0000 da08 6269 6e5f  r....r .....bin_
-00000fb0: 7061 7468 8700 0000 723f 0000 007a 154c  path....r?...z.L
-00000fc0: 6f63 616c 4275 696c 6465 722e 6269 6e5f  ocalBuilder.bin_
-00000fd0: 7061 7468 da08 646f 776e 6c6f 6164 6302  path..downloadc.
-00000fe0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000ff0: 0000 0043 0000 0072 3e00 0000 7215 0000  ...C...r>...r...
-00001000: 0029 0172 5400 0000 2902 721e 0000 0072  .).rT...).r....r
-00001010: 5a00 0000 721f 0000 0072 1f00 0000 7220  Z...r....r....r 
-00001020: 0000 0072 5a00 0000 8b00 0000 723f 0000  ...rZ.......r?..
-00001030: 007a 154c 6f63 616c 4275 696c 6465 722e  .z.LocalBuilder.
-00001040: 646f 776e 6c6f 6164 da04 706f 7274 6302  download..portc.
-00001050: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00001060: 0000 0043 0000 00f3 0e00 0000 7c01 7c00  ...C........|.|.
-00001070: 6a00 6401 3c00 7c00 5300 2902 4e7a 0a2d  j.d.<.|.S.).Nz.-
-00001080: 7265 7374 2d70 6f72 74a9 0172 5500 0000  rest-port..rU...
-00001090: a902 721e 0000 0072 5b00 0000 721f 0000  ..r....r[...r...
-000010a0: 0072 1f00 0000 7220 0000 00da 116d 616e  .r....r .....man
-000010b0: 6167 6572 5f72 6573 745f 706f 7274 8f00  ager_rest_port..
-000010c0: 0000 f304 0000 000a 0104 017a 1e4c 6f63  ...........z.Loc
-000010d0: 616c 4275 696c 6465 722e 6d61 6e61 6765  alBuilder.manage
-000010e0: 725f 7265 7374 5f70 6f72 7463 0200 0000  r_rest_portc....
-000010f0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00001100: 4300 0000 725c 0000 0029 024e 7a0a 2d67  C...r\...).Nz.-g
-00001110: 7270 632d 706f 7274 725d 0000 0072 5e00  rpc-portr]...r^.
-00001120: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00001130: 00da 116d 616e 6167 6572 5f67 7270 635f  ...manager_grpc_
-00001140: 706f 7274 9300 0000 7260 0000 007a 1e4c  port....r`...z.L
-00001150: 6f63 616c 4275 696c 6465 722e 6d61 6e61  ocalBuilder.mana
-00001160: 6765 725f 6772 7063 5f70 6f72 7463 0100  ger_grpc_portc..
-00001170: 0000 0000 0000 0000 0000 0400 0000 0600  ................
-00001180: 0000 4300 0000 7330 0000 0067 007d 017c  ..C...s0...g.}.|
-00001190: 006a 00a0 01a1 0044 005d 0e5c 027d 027d  .j.....D.].\.}.}
-000011a0: 037c 01a0 027c 029b 0064 017c 039b 009d  .|...|...d.|....
-000011b0: 03a1 0101 0071 077c 0153 0029 024e da01  .....q.|.S.).N..
-000011c0: 3d29 0372 5500 0000 da05 6974 656d 73da  =).rU.....items.
-000011d0: 0661 7070 656e 6429 0472 1e00 0000 da07  .append).r......
-000011e0: 636f 6e66 6967 73da 036b 6579 da05 7661  configs..key..va
-000011f0: 6c75 6572 1f00 0000 721f 0000 0072 2000  luer....r....r .
-00001200: 0000 da1d 5f5f 6765 745f 6d61 6e61 6765  ....__get_manage
-00001210: 725f 636f 6e66 6967 735f 6173 5f61 7267  r_configs_as_arg
-00001220: 7397 0000 0073 0800 0000 0401 1201 1601  s....s..........
-00001230: 0401 7a2a 4c6f 6361 6c42 7569 6c64 6572  ..z*LocalBuilder
-00001240: 2e5f 5f67 6574 5f6d 616e 6167 6572 5f63  .__get_manager_c
-00001250: 6f6e 6669 6773 5f61 735f 6172 6773 da09  onfigs_as_args..
-00001260: 6669 6c65 5f6e 616d 6563 0200 0000 0000  file_namec......
-00001270: 0000 0000 0000 0300 0000 0600 0000 4300  ..............C.
-00001280: 0000 7356 0000 007c 006a 0064 0075 0072  ..sV...|.j.d.u.r
-00001290: 0974 0164 0183 0182 017c 006a 0264 0075  .t.d.....|.j.d.u
-000012a0: 0072 1274 0164 0283 0182 0174 0364 03a0  .r.t.d.....t.d..
-000012b0: 047c 006a 007c 006a 027c 006a 05a1 0383  .|.j.|.j.|.j....
-000012c0: 01a0 06a1 007d 027c 026a 0764 0464 0464  .....}.|.j.d.d.d
-000012d0: 058d 0201 007c 027c 011b 0053 0029 064e  .....|.|...S.).N
-000012e0: fa2d 6e6f 2070 6174 6820 7072 6f76 6964  .-no path provid
-000012f0: 6564 2061 6e64 204b 4153 4b41 4441 5f50  ed and KASKADA_P
-00001300: 4154 4820 7761 7320 6e6f 7420 7365 747a  ATH was not setz
-00001310: 356e 6f20 6c6f 6720 7061 7468 2070 726f  5no log path pro
-00001320: 7669 6465 6420 616e 6420 4b41 534b 4144  vided and KASKAD
-00001330: 415f 4c4f 475f 5041 5448 2077 6173 206e  A_LOG_PATH was n
-00001340: 6f74 2073 6574 7a08 7b7d 2f7b 7d2f 7b7d  ot setz.{}/{}/{}
-00001350: 54a9 02da 0770 6172 656e 7473 da08 6578  T....parents..ex
-00001360: 6973 745f 6f6b 2908 724d 0000 00da 0a56  ist_ok).rM.....V
-00001370: 616c 7565 4572 726f 7272 5300 0000 7203  alueErrorrS...r.
-00001380: 0000 0072 2e00 0000 7218 0000 00da 0a65  ...r....r......e
-00001390: 7870 616e 6475 7365 72da 056d 6b64 6972  xpanduser..mkdir
-000013a0: 2903 721e 0000 0072 6900 0000 7258 0000  ).r....ri...rX..
-000013b0: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-000013c0: da0e 5f5f 6765 745f 6c6f 675f 7061 7468  ..__get_log_path
-000013d0: 9d00 0000 7316 0000 000a 0108 010a 0108  ....s...........
-000013e0: 0102 0112 0102 ff04 0202 fe0e 0308 017a  ...............z
-000013f0: 1b4c 6f63 616c 4275 696c 6465 722e 5f5f  .LocalBuilder.__
-00001400: 6765 745f 6c6f 675f 7061 7468 da06 7072  get_log_path..pr
-00001410: 6566 6978 6302 0000 0000 0000 0000 0000  efixc...........
-00001420: 0004 0000 0004 0000 0043 0000 0073 2800  .........C...s(.
-00001430: 0000 7c00 a000 7c01 9b00 6401 9d02 a101  ..|...|...d.....
-00001440: 7d02 7c00 a000 7c01 9b00 6402 9d02 a101  }.|...|...d.....
-00001450: 7d03 7c02 7c03 6602 5300 2903 4e7a 0b5f  }.|.|.f.S.).Nz._
-00001460: 7374 6465 7272 2e74 7874 7a0b 5f73 7464  stderr.txtz._std
-00001470: 6f75 742e 7478 7429 01da 1b5f 4c6f 6361  out.txt)..._Loca
-00001480: 6c42 7569 6c64 6572 5f5f 6765 745f 6c6f  lBuilder__get_lo
-00001490: 675f 7061 7468 2904 721e 0000 0072 7200  g_path).r....rr.
-000014a0: 0000 da06 7374 6465 7272 da06 7374 646f  ....stderr..stdo
-000014b0: 7574 721f 0000 0072 1f00 0000 7220 0000  utr....r....r ..
-000014c0: 00da 0f5f 5f67 6574 5f73 7464 5f70 6174  ...__get_std_pat
-000014d0: 6873 a800 0000 7306 0000 0010 0110 0108  hs....s.........
-000014e0: 017a 1c4c 6f63 616c 4275 696c 6465 722e  .z.LocalBuilder.
-000014f0: 5f5f 6765 745f 7374 645f 7061 7468 7363  __get_std_pathsc
-00001500: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001510: 0500 0000 4300 0000 734e 0000 007c 006a  ....C...sN...|.j
-00001520: 0064 0075 0072 0974 0164 0183 0182 017c  .d.u.r.t.d.....|
-00001530: 006a 0264 0075 0072 1274 0164 0283 0182  .j.d.u.r.t.d....
-00001540: 0174 0364 03a0 047c 006a 007c 006a 02a1  .t.d...|.j.|.j..
-00001550: 0283 01a0 05a1 007d 017c 016a 0664 0464  .......}.|.j.d.d
-00001560: 0464 058d 0201 007c 0153 0029 064e 726a  .d.....|.S.).Nrj
-00001570: 0000 007a 356e 6f20 6269 6e20 7061 7468  ...z5no bin path
-00001580: 2070 726f 7669 6465 6420 616e 6420 4b41   provided and KA
-00001590: 534b 4144 415f 4249 4e5f 5041 5448 2077  SKADA_BIN_PATH w
-000015a0: 6173 206e 6f74 2073 6574 7a05 7b7d 2f7b  as not setz.{}/{
-000015b0: 7d54 726b 0000 0029 0772 4d00 0000 726e  }Trk...).rM...rn
-000015c0: 0000 0072 5000 0000 7203 0000 0072 2e00  ...rP...r....r..
-000015d0: 0000 726f 0000 0072 7000 0000 2902 721e  ..ro...rp...).r.
-000015e0: 0000 0072 5900 0000 721f 0000 0072 1f00  ...rY...r....r..
-000015f0: 0000 7220 0000 00da 115f 5f67 6574 5f62  ..r .....__get_b
-00001600: 696e 6172 795f 7061 7468 ad00 0000 730e  inary_path....s.
-00001610: 0000 000a 0108 010a 0108 0118 010e 0104  ................
-00001620: 017a 1e4c 6f63 616c 4275 696c 6465 722e  .z.LocalBuilder.
-00001630: 5f5f 6765 745f 6269 6e61 7279 5f70 6174  __get_binary_pat
-00001640: 6863 0100 0000 0000 0000 0000 0000 0c00  hc..............
-00001650: 0000 0500 0000 4300 0000 73ae 0000 007c  ......C...s....|
-00001660: 00a0 00a1 007c 006a 011b 007d 017c 00a0  .....|.j...}.|..
-00001670: 0264 01a1 015c 027d 027d 037c 00a0 00a1  .d...\.}.}.|....
-00001680: 007c 006a 031b 007d 047c 00a0 0264 02a1  .|.j...}.|...d..
-00001690: 015c 027d 057d 0664 037d 0774 047c 0183  .\.}.}.d.}.t.|..
-000016a0: 0167 017c 00a0 05a1 0017 007d 0874 06a0  .g.|.......}.t..
-000016b0: 0764 047c 089b 009d 02a1 0101 007c 047c  .d.|.........|.|
-000016c0: 0767 027d 0974 06a0 0764 057c 099b 009d  .g.}.t...d.|....
-000016d0: 02a1 0101 0074 06a0 0864 06a1 0101 0074  .....t...d.....t
-000016e0: 09a0 0a7c 087c 027c 03a1 037d 0a74 06a0  ...|.|.|...}.t..
-000016f0: 0864 07a1 0101 0074 09a0 0a7c 097c 057c  .d.....t...|.|.|
-00001700: 06a1 037d 0b7c 0a7c 0b66 0253 0029 084e  ...}.|.|.f.S.).N
-00001710: da07 6d61 6e61 6765 72da 0665 6e67 696e  ..manager..engin
-00001720: 65da 0573 6572 7665 7a17 4d61 6e61 6765  e..servez.Manage
-00001730: 7220 7374 6172 7420 636f 6d6d 616e 643a  r start command:
-00001740: 207a 1645 6e67 696e 6520 7374 6172 7420   z.Engine start 
-00001750: 636f 6d6d 616e 643a 207a 1c49 6e69 7469  command: z.Initi
-00001760: 616c 697a 696e 6720 6d61 6e61 6765 7220  alizing manager 
-00001770: 7072 6f63 6573 737a 1b49 6e69 7469 616c  processz.Initial
-00001780: 697a 696e 6720 656e 6769 6e65 2070 726f  izing engine pro
-00001790: 6365 7373 290b da1e 5f4c 6f63 616c 4275  cess)..._LocalBu
-000017a0: 696c 6465 725f 5f67 6574 5f62 696e 6172  ilder__get_binar
-000017b0: 795f 7061 7468 da20 4b41 534b 4144 415f  y_path. KASKADA_
-000017c0: 4d41 4e41 4745 525f 4249 4e5f 4e41 4d45  MANAGER_BIN_NAME
-000017d0: 5f44 4546 4155 4c54 da1c 5f4c 6f63 616c  _DEFAULT.._Local
-000017e0: 4275 696c 6465 725f 5f67 6574 5f73 7464  Builder__get_std
-000017f0: 5f70 6174 6873 da1f 4b41 534b 4144 415f  _paths..KASKADA_
-00001800: 454e 4749 4e45 5f42 494e 5f4e 414d 455f  ENGINE_BIN_NAME_
-00001810: 4445 4641 554c 5472 3700 0000 da2a 5f4c  DEFAULTr7....*_L
-00001820: 6f63 616c 4275 696c 6465 725f 5f67 6574  ocalBuilder__get
-00001830: 5f6d 616e 6167 6572 5f63 6f6e 6669 6773  _manager_configs
-00001840: 5f61 735f 6172 6773 7222 0000 0072 2900  _as_argsr"...r).
-00001850: 0000 7223 0000 0072 0900 0000 da0e 7275  ..r#...r......ru
-00001860: 6e5f 7375 6270 726f 6365 7373 290c 721e  n_subprocess).r.
-00001870: 0000 00da 136d 616e 6167 6572 5f62 696e  .....manager_bin
-00001880: 6172 795f 7061 7468 da0f 6d61 6e61 6765  ary_path..manage
-00001890: 725f 7374 645f 6572 72da 0f6d 616e 6167  r_std_err..manag
-000018a0: 6572 5f73 7464 5f6f 7574 da12 656e 6769  er_std_out..engi
-000018b0: 6e65 5f62 696e 6172 795f 7061 7468 da0e  ne_binary_path..
-000018c0: 656e 6769 6e65 5f73 7464 5f65 7272 da0e  engine_std_err..
-000018d0: 656e 6769 6e65 5f73 7464 5f6f 7574 da0e  engine_std_out..
-000018e0: 656e 6769 6e65 5f63 6f6d 6d61 6e64 da0b  engine_command..
-000018f0: 6d61 6e61 6765 725f 636d 64da 0a65 6e67  manager_cmd..eng
-00001900: 696e 655f 636d 6472 1200 0000 7213 0000  ine_cmdr....r...
-00001910: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00001920: da07 5f5f 7374 6172 74b6 0000 0073 2800  ..__start....s(.
-00001930: 0000 0c02 02ff 0e03 0c02 02ff 0e03 0401  ................
-00001940: 1202 1001 0801 1001 0a01 0401 0601 04ff  ................
-00001950: 0a03 0401 0601 04ff 0803 7a14 4c6f 6361  ..........z.Loca
-00001960: 6c42 7569 6c64 6572 2e5f 5f73 7461 7274  lBuilder.__start
-00001970: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
-00001980: 0006 0000 0043 0000 0073 aa00 0000 7400  .....C...s....t.
-00001990: a001 a100 7d01 7c00 a002 a100 7d02 7c02  ....}.|.....}.|.
-000019a0: 6a03 6401 6401 6402 8d02 0100 7c01 a004  j.d.d.d.....|...
-000019b0: 7c02 7c00 6a05 7c00 6a06 a103 7d03 7407  |.|.j.|.j...}.t.
-000019c0: a008 6403 7c03 6a09 9b00 9d02 a101 0100  ..d.|.j.........
-000019d0: 7407 a008 6404 7c03 6a0a 9b00 9d02 a101  t...d.|.j.......
-000019e0: 0100 7407 a008 6405 7c03 6a0b 9b00 9d02  ..t...d.|.j.....
-000019f0: a101 0100 7c00 a00c 7c03 6a09 a00d a100  ....|...|.j.....
-00001a00: a00e 740f 7c00 6a10 8301 a011 a100 a00d  ..t.|.j.........
-00001a10: a100 a101 a101 0100 7412 a013 7c03 6a0a  ........t...|.j.
-00001a20: 6406 a102 0100 7412 a013 7c03 6a0b 6406  d.....t...|.j.d.
-00001a30: a102 0100 6407 5300 2908 7a38 446f 776e  ....d.S.).z8Down
-00001a40: 6c6f 6164 7320 7468 6520 6c61 7465 7374  loads the latest
-00001a50: 2072 656c 6561 7365 2076 6572 7369 6f6e   release version
-00001a60: 2074 6f20 7468 6520 6269 6e61 7279 2070   to the binary p
-00001a70: 6174 682e 5472 6b00 0000 7a0f 446f 776e  ath.Trk...z.Down
-00001a80: 6c6f 6164 2050 6174 683a 207a 0e4d 616e  load Path: z.Man
-00001a90: 6167 6572 2050 6174 683a 207a 0d45 6e67  ager Path: z.Eng
-00001aa0: 696e 6520 5061 7468 3a20 69ed 0100 004e  ine Path: i....N
-00001ab0: 2914 720a 0000 00da 0d52 656c 6561 7365  ).r......Release
-00001ac0: 436c 6965 6e74 727b 0000 0072 7000 0000  Clientr{...rp...
-00001ad0: da17 646f 776e 6c6f 6164 5f6c 6174 6573  ..download_lates
-00001ae0: 745f 7265 6c65 6173 6572 7c00 0000 727e  t_releaser|...r~
-00001af0: 0000 0072 2200 0000 7229 0000 00da 0e5f  ...r"...r)....._
-00001b00: 646f 776e 6c6f 6164 5f70 6174 68da 0d5f  download_path.._
-00001b10: 6d61 6e61 6765 725f 7061 7468 da0c 5f65  manager_path.._e
-00001b20: 6e67 696e 655f 7061 7468 7259 0000 00da  ngine_pathrY....
-00001b30: 0861 6273 6f6c 7574 65da 0b72 656c 6174  .absolute..relat
-00001b40: 6976 655f 746f 7203 0000 0072 4d00 0000  ive_tor....rM...
-00001b50: 726f 0000 0072 4900 0000 da05 6368 6d6f  ro...rI.....chmo
-00001b60: 6429 0472 1e00 0000 7230 0000 00da 0d64  d).r....r0.....d
-00001b70: 6f77 6e6c 6f61 645f 7061 7468 da0d 6c6f  ownload_path..lo
-00001b80: 6361 6c5f 7265 6c65 6173 6572 1f00 0000  cal_releaser....
-00001b90: 721f 0000 0072 2000 0000 da19 5f5f 646f  r....r .....__do
-00001ba0: 776e 6c6f 6164 5f6c 6174 6573 745f 7265  wnload_latest_re
-00001bb0: 6c65 6173 65cf 0000 0073 2400 0000 0802  lease....s$.....
-00001bc0: 0801 0e01 0401 0201 0401 0401 04fd 1205  ................
-00001bd0: 1201 1201 0402 0a01 1001 02ff 04ff 0e05  ................
-00001be0: 1201 7a26 4c6f 6361 6c42 7569 6c64 6572  ..z&LocalBuilder
-00001bf0: 2e5f 5f64 6f77 6e6c 6f61 645f 6c61 7465  .__download_late
-00001c00: 7374 5f72 656c 6561 7365 6301 0000 0000  st_releasec.....
-00001c10: 0000 0000 0000 0003 0000 0008 0000 0043  ...............C
-00001c20: 0000 0073 5a00 0000 7c00 6a00 7207 7c00  ...sZ...|.j.r.|.
-00001c30: a001 a100 0100 7c00 a002 a100 5c02 7d01  ......|.....\.}.
-00001c40: 7d02 7c00 6a03 6401 7500 7216 7404 6402  }.|.j.d.u.r.t.d.
-00001c50: 8301 8201 7c00 6a05 6401 7500 721f 7404  ....|.j.d.u.r.t.
-00001c60: 6403 8301 8201 7406 7c00 6a03 7c00 6a05  d.....t.|.j.|.j.
-00001c70: 7c00 6a07 7c00 6a08 7c01 7c02 6404 8d06  |.j.|.j.|.|.d...
-00001c80: 5300 2905 7aac 4275 696c 6473 2074 6865  S.).z.Builds the
-00001c90: 206c 6f63 616c 2073 6573 7369 6f6e 2e20   local session. 
-00001ca0: 5374 6172 7473 2062 7920 646f 776e 6c6f  Starts by downlo
-00001cb0: 6164 696e 6720 7468 6520 6c61 7465 7374  ading the latest
-00001cc0: 2072 656c 6561 7365 2061 6e64 2073 7461   release and sta
-00001cd0: 7274 696e 6720 7468 6520 6c6f 6361 6c20  rting the local 
-00001ce0: 6269 6e61 7269 6573 2e0a 0a20 2020 2020  binaries...     
-00001cf0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00001d00: 2020 2020 2020 2020 5365 7373 696f 6e3a          Session:
-00001d10: 2054 6865 206c 6f63 616c 2073 6573 7369   The local sessi
-00001d20: 6f6e 206f 626a 6563 740a 2020 2020 2020  on object.      
-00001d30: 2020 4e7a 1465 6e64 706f 696e 7420 7761    Nz.endpoint wa
-00001d40: 7320 6e6f 7420 7365 747a 1569 735f 7365  s not setz.is_se
-00001d50: 6375 7265 2077 6173 206e 6f74 2073 6574  cure was not set
-00001d60: 2903 7211 0000 0072 1200 0000 7213 0000  ).r....r....r...
-00001d70: 0029 0972 5400 0000 da26 5f4c 6f63 616c  .).rT....&_Local
-00001d80: 4275 696c 6465 725f 5f64 6f77 6e6c 6f61  Builder__downloa
-00001d90: 645f 6c61 7465 7374 5f72 656c 6561 7365  d_latest_release
-00001da0: da14 5f4c 6f63 616c 4275 696c 6465 725f  .._LocalBuilder_
-00001db0: 5f73 7461 7274 7216 0000 0072 6e00 0000  _startr....rn...
-00001dc0: 7217 0000 0072 0d00 0000 7218 0000 0072  r....r....r....r
-00001dd0: 1900 0000 2903 721e 0000 0072 1200 0000  ....).r....r....
-00001de0: 7213 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
-00001df0: 2000 0000 da05 6275 696c 64e5 0000 0073   .....build....s
-00001e00: 1e00 0000 0606 0801 0c01 0a01 0801 0a01  ................
-00001e10: 0801 0202 0401 0401 0401 0401 0201 0201  ................
-00001e20: 06fa 7a12 4c6f 6361 6c42 7569 6c64 6572  ..z.LocalBuilder
-00001e30: 2e62 7569 6c64 2922 7234 0000 0072 3500  .build)"r4...r5.
-00001e40: 0000 7236 0000 0072 4b00 0000 724c 0000  ..r6...rK...rL..
-00001e50: 0072 5200 0000 7251 0000 0072 4f00 0000  .rR...rQ...rO...
-00001e60: 724e 0000 0072 7c00 0000 727e 0000 00da  rN...r|...r~....
-00001e70: 184b 4153 4b41 4441 5f45 4e44 504f 494e  .KASKADA_ENDPOIN
-00001e80: 545f 4445 4641 554c 54da 194b 4153 4b41  T_DEFAULT..KASKA
-00001e90: 4441 5f49 535f 5345 4355 5245 5f44 4546  DA_IS_SECURE_DEF
-00001ea0: 4155 4c54 7237 0000 0072 3800 0000 7221  AULTr7...r8...r!
-00001eb0: 0000 0072 5600 0000 7258 0000 0072 5900  ...rV...rX...rY.
-00001ec0: 0000 725a 0000 00da 0369 6e74 725f 0000  ..rZ.....intr_..
-00001ed0: 0072 6100 0000 727f 0000 0072 0300 0000  .ra...r....r....
-00001ee0: 7273 0000 0072 0800 0000 727d 0000 0072  rs...r....r}...r
-00001ef0: 7b00 0000 7297 0000 0072 9600 0000 720d  {...r....r....r.
-00001f00: 0000 0072 9800 0000 7242 0000 0072 1f00  ...r....rB...r..
-00001f10: 0000 721f 0000 0072 3b00 0000 7220 0000  ..r....r;...r ..
-00001f20: 0072 4300 0000 6100 0000 733e 0000 0008  .rC...a...s>....
-00001f30: 0004 0104 0104 0104 0104 0104 0104 0204  ................
-00001f40: 0102 0402 0104 fd02 0202 fe02 0302 fd02  ................
-00001f50: 040e fc0e 130e 040e 040e 040e 040e 0408  ................
-00001f60: 0412 061a 0b0e 0508 0908 1916 1672 4300  .............rC.
-00001f70: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00001f80: 0000 0004 0000 0000 0000 0073 2600 0000  ...........s&...
-00001f90: 6500 5a01 6400 5a02 6407 8700 6601 6403  e.Z.d.Z.d...f.d.
-00001fa0: 6404 840c 5a03 6405 6406 8400 5a04 8700  d...Z.d.d...Z...
-00001fb0: 0400 5a05 5300 2908 da0d 5265 6d6f 7465  ..Z.S.)...Remote
-00001fc0: 4275 696c 6465 7272 1400 0000 4e63 0100  Builderr....Nc..
-00001fd0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00001fe0: 0000 0300 0000 730e 0000 0074 0083 00a0  ......s....t....
-00001ff0: 01a1 0001 0064 0053 0072 1500 0000 2902  .....d.S.r....).
-00002000: 723a 0000 0072 2100 0000 7225 0000 0072  r:...r!...r%...r
-00002010: 3b00 0000 721f 0000 0072 2000 0000 7221  ;...r....r ...r!
-00002020: 0000 00fe 0000 0073 0200 0000 0e01 7a16  .......s......z.
-00002030: 5265 6d6f 7465 4275 696c 6465 722e 5f5f  RemoteBuilder.__
-00002040: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00002050: 0000 0001 0000 0006 0000 0043 0000 0073  ...........C...s
-00002060: 1800 0000 7400 7c00 6a01 7c00 6a02 7c00  ....t.|.j.|.j.|.
-00002070: 6a03 7c00 6a04 6401 8d04 5300 2902 4e29  j.|.j.d...S.).N)
-00002080: 0172 1100 0000 2905 720d 0000 0072 1600  .r....).r....r..
-00002090: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
-000020a0: 0072 2500 0000 721f 0000 0072 1f00 0000  .r%...r....r....
-000020b0: 7220 0000 0072 9800 0000 0101 0000 7306  r ...r........s.
-000020c0: 0000 0002 0110 0106 ff7a 1352 656d 6f74  .........z.Remot
-000020d0: 6542 7569 6c64 6572 2e62 7569 6c64 2902  eBuilder.build).
-000020e0: 7214 0000 004e 2906 7234 0000 0072 3500  r....N).r4...r5.
-000020f0: 0000 7236 0000 0072 2100 0000 7298 0000  ..r6...r!...r...
-00002100: 0072 4200 0000 721f 0000 0072 1f00 0000  .rB...r....r....
-00002110: 723b 0000 0072 2000 0000 729c 0000 00fd  r;...r ...r.....
-00002120: 0000 0073 0600 0000 0800 0e01 1003 729c  ...s..........r.
-00002130: 0000 0029 21da 076c 6f67 6769 6e67 7249  ...)!..loggingrI
-00002140: 0000 00da 0373 7973 722b 0000 0072 4000  .....sysr+...r@.
-00002150: 0000 da03 6162 6372 0200 0000 da07 7061  ....abcr......pa
-00002160: 7468 6c69 6272 0300 0000 da0a 7375 6270  thlibr......subp
-00002170: 726f 6365 7373 7204 0000 00da 0674 7970  rocessr......typ
-00002180: 696e 6772 0500 0000 7206 0000 0072 0700  ingr....r....r..
-00002190: 0000 7208 0000 00da 0e6b 6173 6b61 6461  ..r......kaskada
-000021a0: 2e63 6c69 656e 7472 2f00 0000 da0b 6b61  .clientr/.....ka
-000021b0: 736b 6164 612e 6170 6972 0900 0000 720a  skada.apir....r.
-000021c0: 0000 00da 0b62 6173 6963 436f 6e66 6967  .....basicConfig
-000021d0: 7275 0000 00da 0449 4e46 4fda 0967 6574  ru.....INFO..get
-000021e0: 4c6f 6767 6572 7234 0000 0072 2200 0000  Loggerr4...r"...
-000021f0: 720d 0000 0072 3900 0000 7299 0000 0072  r....r9...r....r
-00002200: 9a00 0000 7243 0000 0072 9c00 0000 721f  ....rC...r....r.
-00002210: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
-00002220: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00002230: 7328 0000 0008 0008 0108 0108 0108 010c  s(..............
-00002240: 010c 010c 0118 0108 0210 0112 020a 010e  ................
-00002250: 0310 2f04 1c04 0110 0300 7f14 1d         ../..........
+00000180: 0000 0000 0000 0900 0000 4000 0000 7344  ..........@...sD
+00000190: 0000 0065 005a 0164 005a 0264 0965 0365  ...e.Z.d.Z.d.e.e
+000001a0: 0465 0365 0565 0319 0065 0565 0619 0065  .e.e.e...e.e...e
+000001b0: 0565 0619 0064 0164 029c 0764 0364 0484  .e...d.d...d.d..
+000001c0: 055a 0764 0564 0684 005a 0864 0764 0884  .Z.d.d...Z.d.d..
+000001d0: 005a 0964 0153 0029 0ada 0753 6573 7369  .Z.d.S.)...Sessi
+000001e0: 6f6e 4e29 07da 0865 6e64 706f 696e 74da  onN)...endpoint.
+000001f0: 0969 735f 7365 6375 7265 da04 6e61 6d65  .is_secure..name
+00000200: da09 636c 6965 6e74 5f69 64da 0f6d 616e  ..client_id..man
+00000210: 6167 6572 5f70 726f 6365 7373 da0e 656e  ager_process..en
+00000220: 6769 6e65 5f70 726f 6365 7373 da06 7265  gine_process..re
+00000230: 7475 726e 6307 0000 0000 0000 0000 0000  turnc...........
+00000240: 0007 0000 0002 0000 0043 0000 0073 3200  .........C...s2.
+00000250: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7c03  ..|.|._.|.|._.|.
+00000260: 7c00 5f02 7c04 7c00 5f03 7c00 a004 a100  |._.|.|._.|.....
+00000270: 7c00 5f05 7c05 7c00 5f06 7c06 7c00 5f07  |._.|.|._.|.|._.
+00000280: 6400 5300 a901 4e29 08da 095f 656e 6470  d.S...N)..._endp
+00000290: 6f69 6e74 da0a 5f69 735f 7365 6375 7265  oint.._is_secure
+000002a0: da05 5f6e 616d 65da 0a5f 636c 6965 6e74  .._name.._client
+000002b0: 5f69 64da 0763 6f6e 6e65 6374 5a07 5f63  _id..connectZ._c
+000002c0: 6c69 656e 74da 105f 6d61 6e61 6765 725f  lient.._manager_
+000002d0: 7072 6f63 6573 73da 0f5f 656e 6769 6e65  process.._engine
+000002e0: 5f70 726f 6365 7373 2907 da04 7365 6c66  _process)...self
+000002f0: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00000300: 1100 0000 7212 0000 0072 1300 0000 a900  ....r....r......
+00000310: 721e 0000 00fa 1f2f 7372 632f 7372 632f  r....../src/src/
+00000320: 6b61 736b 6164 612f 6170 692f 7365 7373  kaskada/api/sess
+00000330: 696f 6e2e 7079 da08 5f5f 696e 6974 5f5f  ion.py..__init__
+00000340: 1300 0000 730e 0000 0000 0906 0106 0106  ....s...........
+00000350: 0106 010a 0106 017a 1053 6573 7369 6f6e  .......z.Session
+00000360: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+00000370: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00000380: 0000 7358 0000 007c 006a 0064 0075 0172  ..sX...|.j.d.u.r
+00000390: 2a74 0164 0075 0172 1c74 01a0 0264 01a1  *t.d.u.r.t...d..
+000003a0: 016e 0264 0001 007c 006a 00a0 03a1 0001  .n.d...|.j......
+000003b0: 007c 006a 0464 0075 0172 5474 0164 0075  .|.j.d.u.rTt.d.u
+000003c0: 0172 4674 01a0 0264 02a1 016e 0264 0001  .rFt...d...n.d..
+000003d0: 007c 006a 04a0 03a1 0001 0064 0053 0029  .|.j.......d.S.)
+000003e0: 034e 7a20 5374 6f70 7069 6e67 204b 6173  .Nz Stopping Kas
+000003f0: 6b61 6461 204d 616e 6167 6572 2073 6572  kada Manager ser
+00000400: 7669 6365 7a1f 5374 6f70 7069 6e67 204b  vicez.Stopping K
+00000410: 6173 6b61 6461 2045 6e67 696e 6520 7365  askada Engine se
+00000420: 7276 6963 6529 0572 1b00 0000 da06 6c6f  rvice).r......lo
+00000430: 6767 6572 da04 696e 666f da04 6b69 6c6c  gger..info..kill
+00000440: 721c 0000 00a9 0172 1d00 0000 721e 0000  r......r....r...
+00000450: 0072 1e00 0000 721f 0000 00da 075f 5f64  .r....r......__d
+00000460: 656c 5f5f 2400 0000 7320 0000 0000 010a  el__$...s ......
+00000470: 0306 fe06 0102 ff04 0202 fe02 030a 020a  ................
+00000480: 0306 fe06 0102 ff04 0202 fe02 037a 0f53  .............z.S
+00000490: 6573 7369 6f6e 2e5f 5f64 656c 5f5f 6301  ession.__del__c.
+000004a0: 0000 0000 0000 0000 0000 0003 0000 0006  ................
+000004b0: 0000 0043 0000 0073 8a00 0000 6401 7d01  ...C...s....d.}.
+000004c0: 6402 7d02 7c01 6403 6b00 725e 7c02 735e  d.}.|.d.k.r^|.s^
+000004d0: 7400 a001 6404 7c01 9b00 6405 7c00 6a02  t...d.|...d.|.j.
+000004e0: 9b00 9d04 a101 0100 7403 a004 7c00 6a02  ........t...|.j.
+000004f0: a101 7246 7400 a005 6406 a101 0100 6407  ..rFt...d.....d.
+00000500: 7d02 7c01 6408 3700 7d01 7406 a007 6409  }.|.d.7.}.t...d.
+00000510: 7c01 1300 a101 0100 7108 7c02 6402 6b02  |.......q.|.d.k.
+00000520: 7274 7408 640a a009 7c01 a101 8301 8201  rtt.d...|.......
+00000530: 740a 6a0b a00c 7c00 6a0d 7c00 6a02 7c00  t.j...|.j.|.j.|.
+00000540: 6a0e a103 5300 290b 4e72 0100 0000 46e9  j...S.).Nr....F.
+00000550: 0300 0000 7a11 4174 7465 6d70 7469 6e67  ....z.Attempting
+00000560: 2028 7472 7920 237a 1029 2074 6f20 636f   (try #z.) to co
+00000570: 6e6e 6563 7420 746f 207a 2253 7563 6365  nnect to z"Succe
+00000580: 7373 6675 6c6c 7920 636f 6e6e 6563 7465  ssfully connecte
+00000590: 6420 746f 2073 6573 7369 6f6e 2e54 e901  d to session.T..
+000005a0: 0000 0067 0000 0000 0000 f83f 7a38 756e  ...g.......?z8un
+000005b0: 6162 6c65 2074 6f20 636f 6e6e 6563 7420  able to connect 
+000005c0: 746f 204d 616e 6167 6572 206f 7220 456e  to Manager or En
+000005d0: 6769 6e65 2061 6674 6572 207b 7d20 6174  gine after {} at
+000005e0: 7465 6d70 7473 290f 7221 0000 00da 0564  tempts).r!.....d
+000005f0: 6562 7567 7216 0000 0072 0900 0000 5a0c  ebugr....r....Z.
+00000600: 6368 6563 6b5f 736f 636b 6574 7222 0000  check_socketr"..
+00000610: 00da 0474 696d 65da 0573 6c65 6570 da0f  ...time..sleep..
+00000620: 436f 6e6e 6563 7469 6f6e 4572 726f 72da  ConnectionError.
+00000630: 0666 6f72 6d61 74da 076b 6173 6b61 6461  .format..kaskada
+00000640: da06 636c 6965 6e74 da04 696e 6974 7219  ..client..initr.
+00000650: 0000 0072 1700 0000 2903 721d 0000 00da  ...r....).r.....
+00000660: 0761 7474 656d 7074 5a10 6973 5f76 616c  .attemptZ.is_val
+00000670: 6964 5f73 6573 7369 6f6e 721e 0000 0072  id_sessionr....r
+00000680: 1e00 0000 721f 0000 0072 1a00 0000 3100  ....r....r....1.
+00000690: 0000 7320 0000 0000 0104 0104 010c 0118  ..s ............
+000006a0: 010c 010a 0104 0108 0210 0108 0102 0104  ................
+000006b0: 0102 ff02 ff04 057a 0f53 6573 7369 6f6e  .......z.Session
+000006c0: 2e63 6f6e 6e65 6374 2903 4e4e 4e29 0ada  .connect).NNN)..
+000006d0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000006e0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000006f0: 655f 5fda 0373 7472 da04 626f 6f6c 7207  e__..str..boolr.
+00000700: 0000 0072 0400 0000 7220 0000 0072 2500  ...r....r ...r%.
+00000710: 0000 721a 0000 0072 1e00 0000 721e 0000  ..r....r....r...
+00000720: 0072 1e00 0000 721f 0000 0072 0d00 0000  .r....r....r....
+00000730: 1200 0000 731c 0000 0008 0600 0100 0100  ....s...........
+00000740: f902 0202 0102 0102 0106 0106 0106 0102  ................
+00000750: f80c 1108 0d72 0d00 0000 6300 0000 0000  .....r....c.....
+00000760: 0000 0000 0000 0000 0000 0007 0000 0000  ................
+00000770: 0000 0073 7400 0000 6500 5a01 6400 5a02  ...st...e.Z.d.Z.
+00000780: 6401 6401 6503 6504 a005 a100 8301 6401  d.d.e.e.......d.
+00000790: 6604 6506 6503 1900 6506 6507 1900 6503  f.e.e...e.e...e.
+000007a0: 6506 6503 1900 6401 6402 9c05 8700 6601  e.e...d.d.....f.
+000007b0: 6403 6404 840d 5a08 6503 6507 6405 9c02  d.d...Z.e.e.d...
+000007c0: 6406 6407 8404 5a09 6503 6408 9c01 6409  d.d...Z.e.d...d.
+000007d0: 640a 8404 5a0a 6503 640b 9c01 640c 640d  d...Z.e.d...d.d.
+000007e0: 8404 5a0b 8700 0400 5a0c 5300 290e da07  ..Z.....Z.S.)...
+000007f0: 4275 696c 6465 724e 2905 720e 0000 0072  BuilderN).r....r
+00000800: 0f00 0000 7210 0000 0072 1100 0000 7214  ....r....r....r.
+00000810: 0000 0063 0500 0000 0000 0000 0000 0000  ...c............
+00000820: 0500 0000 0200 0000 0300 0000 7326 0000  ............s&..
+00000830: 0074 0083 00a0 01a1 0001 007c 017c 005f  .t.........|.|._
+00000840: 027c 027c 005f 037c 037c 005f 047c 047c  .|.|._.|.|._.|.|
+00000850: 005f 0564 0053 0072 1500 0000 2906 da05  ._.d.S.r....)...
+00000860: 7375 7065 7272 2000 0000 7216 0000 0072  superr ...r....r
+00000870: 1700 0000 7218 0000 0072 1900 0000 2905  ....r....r....).
+00000880: 721d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+00000890: 1000 0000 7211 0000 00a9 01da 095f 5f63  ....r........__c
+000008a0: 6c61 7373 5f5f 721e 0000 0072 1f00 0000  lass__r....r....
+000008b0: 7220 0000 0046 0000 0073 0a00 0000 0007  r ...F...s......
+000008c0: 0a01 0601 0601 0601 7a10 4275 696c 6465  ........z.Builde
+000008d0: 722e 5f5f 696e 6974 5f5f 2902 720e 0000  r.__init__).r...
+000008e0: 0072 0f00 0000 6303 0000 0000 0000 0000  .r....c.........
+000008f0: 0000 0003 0000 0002 0000 0043 0000 0073  ...........C...s
+00000900: 1000 0000 7c01 7c00 5f00 7c02 7c00 5f01  ....|.|._.|.|._.
+00000910: 7c00 5300 7215 0000 0029 0272 1600 0000  |.S.r....).r....
+00000920: 7217 0000 00a9 0372 1d00 0000 720e 0000  r......r....r...
+00000930: 0072 0f00 0000 721e 0000 0072 1e00 0000  .r....r....r....
+00000940: 721f 0000 0072 0e00 0000 5300 0000 7306  r....r....S...s.
+00000950: 0000 0000 0106 0106 017a 1042 7569 6c64  .........z.Build
+00000960: 6572 2e65 6e64 706f 696e 7429 0172 1000  er.endpoint).r..
+00000970: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
+00000980: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+00000990: 7c01 7c00 5f00 7c00 5300 7215 0000 0029  |.|._.|.S.r....)
+000009a0: 0172 1800 0000 2902 721d 0000 0072 1000  .r....).r....r..
+000009b0: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+000009c0: 0072 1000 0000 5800 0000 7304 0000 0000  .r....X...s.....
+000009d0: 0106 017a 0c42 7569 6c64 6572 2e6e 616d  ...z.Builder.nam
+000009e0: 65a9 0172 1100 0000 6302 0000 0000 0000  e..r....c.......
+000009f0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00000a00: 0073 0a00 0000 7c01 7c00 5f00 7c00 5300  .s....|.|._.|.S.
+00000a10: 7215 0000 0029 0172 1900 0000 2902 721d  r....).r....).r.
+00000a20: 0000 0072 1100 0000 721e 0000 0072 1e00  ...r....r....r..
+00000a30: 0000 721f 0000 0072 1100 0000 5c00 0000  ..r....r....\...
+00000a40: 7304 0000 0000 0106 017a 1142 7569 6c64  s........z.Build
+00000a50: 6572 2e63 6c69 656e 745f 6964 290d 7231  er.client_id).r1
+00000a60: 0000 0072 3200 0000 7233 0000 0072 3400  ...r2...r3...r4.
+00000a70: 0000 da04 7575 6964 da05 7575 6964 3472  ....uuid..uuid4r
+00000a80: 0700 0000 7235 0000 0072 2000 0000 720e  ....r5...r ...r.
+00000a90: 0000 0072 1000 0000 7211 0000 00da 0d5f  ...r....r......_
+00000aa0: 5f63 6c61 7373 6365 6c6c 5f5f 721e 0000  _classcell__r...
+00000ab0: 0072 1e00 0000 7238 0000 0072 1f00 0000  .r....r8...r....
+00000ac0: 7236 0000 0045 0000 0073 1c00 0000 0803  r6...E...s......
+00000ad0: 0201 0201 0a01 02fb 0202 0601 0601 0201  ................
+00000ae0: 0601 02fa 100d 1005 0e04 7236 0000 007a  ..........r6...z
+00000af0: 0f6c 6f63 616c 686f 7374 3a35 3030 3531  .localhost:50051
+00000b00: 4663 0000 0000 0000 0000 0000 0000 0000  Fc..............
+00000b10: 0000 0500 0000 0000 0000 7300 0100 0065  ..........s....e
+00000b20: 005a 0164 005a 0264 015a 0364 025a 0464  .Z.d.Z.d.Z.d.Z.d
+00000b30: 035a 0564 045a 0664 055a 0764 065a 0864  .Z.d.Z.d.Z.d.Z.d
+00000b40: 075a 0964 085a 0a64 095a 0b65 0c65 0d66  .Z.d.Z.d.Z.e.e.f
+00000b50: 0265 0e65 0f64 0a64 0b9c 0387 0066 0164  .e.e.d.d.....f.d
+00000b60: 0c64 0d84 0d5a 1065 0e64 0e9c 0164 0f64  .d...Z.e.d...d.d
+00000b70: 1084 045a 1165 0e64 0e9c 0164 1164 1284  ...Z.e.d...d.d..
+00000b80: 045a 1265 0e64 0e9c 0164 1364 1484 045a  .Z.e.d...d.d...Z
+00000b90: 1365 0f64 159c 0164 1664 1784 045a 1465  .e.d...d.d...Z.e
+00000ba0: 1564 189c 0164 1964 1a84 045a 1665 1564  .d...d.d...Z.e.d
+00000bb0: 189c 0164 1b64 1c84 045a 1764 1d64 1e84  ...d.d...Z.d.d..
+00000bc0: 005a 1865 0e65 1964 1f9c 0264 2064 2184  .Z.e.e.d...d d!.
+00000bd0: 045a 1a65 0e65 1b65 1965 1966 0219 0064  .Z.e.e.e.e.f...d
+00000be0: 229c 0264 2364 2484 045a 1c65 1964 259c  "..d#d$..Z.e.d%.
+00000bf0: 0164 2664 2784 045a 1d64 2864 2984 005a  .d&d'..Z.d(d)..Z
+00000c00: 1e64 2a64 2b84 005a 1f65 2064 259c 0164  .d*d+..Z.e d%..d
+00000c10: 2c64 2d84 045a 2187 0004 005a 2253 0029  ,d-..Z!....Z"S.)
+00000c20: 2eda 0c4c 6f63 616c 4275 696c 6465 725a  ...LocalBuilderZ
+00000c30: 0c4b 4153 4b41 4441 5f50 4154 487a 107e  .KASKADA_PATHz.~
+00000c40: 2f2e 6361 6368 652f 6b61 736b 6164 615a  /.cache/kaskadaZ
+00000c50: 046c 6f67 735a 104b 4153 4b41 4441 5f4c  .logsZ.KASKADA_L
+00000c60: 4f47 5f50 4154 48da 0362 696e 5a10 4b41  OG_PATH..binZ.KA
+00000c70: 534b 4144 415f 4249 4e5f 5041 5448 7a0f  SKADA_BIN_PATHz.
+00000c80: 6b61 736b 6164 612d 6d61 6e61 6765 727a  kaskada-managerz
+00000c90: 0e6b 6173 6b61 6461 2d65 6e67 696e 655a  .kaskada-engineZ
+00000ca0: 184b 4153 4b41 4441 5f44 4953 4142 4c45  .KASKADA_DISABLE
+00000cb0: 5f44 4f57 4e4c 4f41 444e 2903 720e 0000  _DOWNLOADN).r...
+00000cc0: 0072 0f00 0000 7214 0000 0063 0300 0000  .r....r....c....
+00000cd0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00000ce0: 0300 0000 736a 0000 0074 0083 00a0 01a1  ....sj...t......
+00000cf0: 0001 0074 02a0 0374 046a 0574 046a 06a1  ...t...t.j.t.j..
+00000d00: 027c 005f 0774 02a0 0374 046a 0874 046a  .|._.t...t.j.t.j
+00000d10: 09a1 027c 005f 0a74 02a0 0374 046a 0b74  ...|._.t...t.j.t
+00000d20: 046a 0ca1 027c 005f 0d7c 00a0 0e7c 017c  .j...|._.|...|.|
+00000d30: 02a1 0201 0074 02a0 0374 046a 0f64 01a1  .....t...t.j.d..
+00000d40: 0264 026b 037c 005f 1069 007c 005f 1164  .d.k.|._.i.|._.d
+00000d50: 0053 0029 034e da05 6661 6c73 65da 0474  .S.).N..false..t
+00000d60: 7275 6529 1272 3700 0000 7220 0000 00da  rue).r7...r ....
+00000d70: 026f 73da 0667 6574 656e 7672 3f00 0000  .os..getenvr?...
+00000d80: da10 4b41 534b 4144 415f 5041 5448 5f45  ..KASKADA_PATH_E
+00000d90: 4e56 da14 4b41 534b 4144 415f 5041 5448  NV..KASKADA_PATH
+00000da0: 5f44 4546 4155 4c54 da05 5f70 6174 68da  _DEFAULT.._path.
+00000db0: 144b 4153 4b41 4441 5f42 494e 5f50 4154  .KASKADA_BIN_PAT
+00000dc0: 485f 454e 56da 184b 4153 4b41 4441 5f42  H_ENV..KASKADA_B
+00000dd0: 494e 5f50 4154 485f 4445 4641 554c 54da  IN_PATH_DEFAULT.
+00000de0: 095f 6269 6e5f 7061 7468 da14 4b41 534b  ._bin_path..KASK
+00000df0: 4144 415f 4c4f 475f 5041 5448 5f45 4e56  ADA_LOG_PATH_ENV
+00000e00: da18 4b41 534b 4144 415f 4c4f 475f 5041  ..KASKADA_LOG_PA
+00000e10: 5448 5f44 4546 4155 4c54 da09 5f6c 6f67  TH_DEFAULT.._log
+00000e20: 5f70 6174 6872 0e00 0000 da1c 4b41 534b  _pathr......KASK
+00000e30: 4144 415f 4449 5341 424c 455f 444f 574e  ADA_DISABLE_DOWN
+00000e40: 4c4f 4144 5f45 4e56 da09 5f64 6f77 6e6c  LOAD_ENV.._downl
+00000e50: 6f61 64da 105f 6d61 6e61 6765 725f 636f  oad.._manager_co
+00000e60: 6e66 6967 7372 3a00 0000 7238 0000 0072  nfigsr:...r8...r
+00000e70: 1e00 0000 721f 0000 0072 2000 0000 7200  ....r....r ...r.
+00000e80: 0000 731c 0000 0000 050a 0104 0108 ff06  ..s.............
+00000e90: 0304 0108 ff06 0304 0108 ff06 030c 0210  ................
+00000ea0: ff04 037a 154c 6f63 616c 4275 696c 6465  ...z.LocalBuilde
+00000eb0: 722e 5f5f 696e 6974 5f5f 2901 da04 7061  r.__init__)...pa
+00000ec0: 7468 6302 0000 0000 0000 0000 0000 0002  thc.............
+00000ed0: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+00000ee0: 7c01 7c00 5f00 7c00 5300 7215 0000 0029  |.|._.|.S.r....)
+00000ef0: 0172 4700 0000 a902 721d 0000 0072 5100  .rG.....r....rQ.
+00000f00: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00000f10: 0072 5100 0000 8700 0000 7304 0000 0000  .rQ.......s.....
+00000f20: 0106 017a 114c 6f63 616c 4275 696c 6465  ...z.LocalBuilde
+00000f30: 722e 7061 7468 6302 0000 0000 0000 0000  r.pathc.........
+00000f40: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00000f50: 0a00 0000 7c01 7c00 5f00 7c00 5300 7215  ....|.|._.|.S.r.
+00000f60: 0000 0029 0172 4d00 0000 7252 0000 0072  ...).rM...rR...r
+00000f70: 1e00 0000 721e 0000 0072 1f00 0000 da08  ....r....r......
+00000f80: 6c6f 675f 7061 7468 8b00 0000 7304 0000  log_path....s...
+00000f90: 0000 0106 017a 154c 6f63 616c 4275 696c  .....z.LocalBuil
+00000fa0: 6465 722e 6c6f 675f 7061 7468 6302 0000  der.log_pathc...
+00000fb0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00000fc0: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
+00000fd0: 7c00 5300 7215 0000 0029 0172 4a00 0000  |.S.r....).rJ...
+00000fe0: 7252 0000 0072 1e00 0000 721e 0000 0072  rR...r....r....r
+00000ff0: 1f00 0000 da08 6269 6e5f 7061 7468 8f00  ......bin_path..
+00001000: 0000 7304 0000 0000 0106 017a 154c 6f63  ..s........z.Loc
+00001010: 616c 4275 696c 6465 722e 6269 6e5f 7061  alBuilder.bin_pa
+00001020: 7468 2901 da08 646f 776e 6c6f 6164 6302  th)...downloadc.
+00001030: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00001040: 0000 0043 0000 0073 0a00 0000 7c01 7c00  ...C...s....|.|.
+00001050: 5f00 7c00 5300 7215 0000 0029 0172 4f00  _.|.S.r....).rO.
+00001060: 0000 2902 721d 0000 0072 5500 0000 721e  ..).r....rU...r.
+00001070: 0000 0072 1e00 0000 721f 0000 0072 5500  ...r....r....rU.
+00001080: 0000 9300 0000 7304 0000 0000 0106 017a  ......s........z
+00001090: 154c 6f63 616c 4275 696c 6465 722e 646f  .LocalBuilder.do
+000010a0: 776e 6c6f 6164 2901 da04 706f 7274 6302  wnload)...portc.
+000010b0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000010c0: 0000 0043 0000 0073 0e00 0000 7c01 7c00  ...C...s....|.|.
+000010d0: 6a00 6401 3c00 7c00 5300 2902 4e7a 0a2d  j.d.<.|.S.).Nz.-
+000010e0: 7265 7374 2d70 6f72 74a9 0172 5000 0000  rest-port..rP...
+000010f0: a902 721d 0000 0072 5600 0000 721e 0000  ..r....rV...r...
+00001100: 0072 1e00 0000 721f 0000 00da 116d 616e  .r....r......man
+00001110: 6167 6572 5f72 6573 745f 706f 7274 9700  ager_rest_port..
+00001120: 0000 7304 0000 0000 010a 017a 1e4c 6f63  ..s........z.Loc
+00001130: 616c 4275 696c 6465 722e 6d61 6e61 6765  alBuilder.manage
+00001140: 725f 7265 7374 5f70 6f72 7463 0200 0000  r_rest_portc....
+00001150: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00001160: 4300 0000 730e 0000 007c 017c 006a 0064  C...s....|.|.j.d
+00001170: 013c 007c 0053 0029 024e 7a0a 2d67 7270  .<.|.S.).Nz.-grp
+00001180: 632d 706f 7274 7257 0000 0072 5800 0000  c-portrW...rX...
+00001190: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
+000011a0: 116d 616e 6167 6572 5f67 7270 635f 706f  .manager_grpc_po
+000011b0: 7274 9b00 0000 7304 0000 0000 010a 017a  rt....s........z
+000011c0: 1e4c 6f63 616c 4275 696c 6465 722e 6d61  .LocalBuilder.ma
+000011d0: 6e61 6765 725f 6772 7063 5f70 6f72 7463  nager_grpc_portc
+000011e0: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+000011f0: 0600 0000 4300 0000 7330 0000 0067 007d  ....C...s0...g.}
+00001200: 017c 006a 00a0 01a1 0044 005d 1c5c 027d  .|.j.....D.].\.}
+00001210: 027d 037c 01a0 027c 029b 0064 017c 039b  .}.|...|...d.|..
+00001220: 009d 03a1 0101 0071 0e7c 0153 0029 024e  .......q.|.S.).N
+00001230: da01 3d29 0372 5000 0000 da05 6974 656d  ..=).rP.....item
+00001240: 73da 0661 7070 656e 6429 0472 1d00 0000  s..append).r....
+00001250: 5a07 636f 6e66 6967 73da 036b 6579 da05  Z.configs..key..
+00001260: 7661 6c75 6572 1e00 0000 721e 0000 0072  valuer....r....r
+00001270: 1f00 0000 5a1d 5f5f 6765 745f 6d61 6e61  ....Z.__get_mana
+00001280: 6765 725f 636f 6e66 6967 735f 6173 5f61  ger_configs_as_a
+00001290: 7267 739f 0000 0073 0800 0000 0001 0401  rgs....s........
+000012a0: 1201 1601 7a2a 4c6f 6361 6c42 7569 6c64  ....z*LocalBuild
+000012b0: 6572 2e5f 5f67 6574 5f6d 616e 6167 6572  er.__get_manager
+000012c0: 5f63 6f6e 6669 6773 5f61 735f 6172 6773  _configs_as_args
+000012d0: 2902 da09 6669 6c65 5f6e 616d 6572 1400  )...file_namer..
+000012e0: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
+000012f0: 0000 0006 0000 0043 0000 0073 5600 0000  .......C...sV...
+00001300: 7c00 6a00 6400 7500 7212 7401 6401 8301  |.j.d.u.r.t.d...
+00001310: 8201 7c00 6a02 6400 7500 7224 7401 6402  ..|.j.d.u.r$t.d.
+00001320: 8301 8201 7403 6403 a004 7c00 6a00 7c00  ....t.d...|.j.|.
+00001330: 6a02 7c00 6a05 a103 8301 a006 a100 7d02  j.|.j.........}.
+00001340: 7c02 6a07 6404 6404 6405 8d02 0100 7c02  |.j.d.d.d.....|.
+00001350: 7c01 1b00 5300 2906 4efa 2d6e 6f20 7061  |...S.).N.-no pa
+00001360: 7468 2070 726f 7669 6465 6420 616e 6420  th provided and 
+00001370: 4b41 534b 4144 415f 5041 5448 2077 6173  KASKADA_PATH was
+00001380: 206e 6f74 2073 6574 7a35 6e6f 206c 6f67   not setz5no log
+00001390: 2070 6174 6820 7072 6f76 6964 6564 2061   path provided a
+000013a0: 6e64 204b 4153 4b41 4441 5f4c 4f47 5f50  nd KASKADA_LOG_P
+000013b0: 4154 4820 7761 7320 6e6f 7420 7365 747a  ATH was not setz
+000013c0: 087b 7d2f 7b7d 2f7b 7d54 a902 da07 7061  .{}/{}/{}T....pa
+000013d0: 7265 6e74 73da 0865 7869 7374 5f6f 6b29  rents..exist_ok)
+000013e0: 0872 4700 0000 da0a 5661 6c75 6545 7272  .rG.....ValueErr
+000013f0: 6f72 724d 0000 0072 0300 0000 722c 0000  orrM...r....r,..
+00001400: 0072 1800 0000 da0a 6578 7061 6e64 7573  .r......expandus
+00001410: 6572 da05 6d6b 6469 7229 0372 1d00 0000  er..mkdir).r....
+00001420: 7260 0000 0072 5300 0000 721e 0000 0072  r`...rS...r....r
+00001430: 1e00 0000 721f 0000 005a 0e5f 5f67 6574  ....r....Z.__get
+00001440: 5f6c 6f67 5f70 6174 68a5 0000 0073 1200  _log_path....s..
+00001450: 0000 0001 0a01 0801 0a01 0801 0201 12ff  ................
+00001460: 0803 0e01 7a1b 4c6f 6361 6c42 7569 6c64  ....z.LocalBuild
+00001470: 6572 2e5f 5f67 6574 5f6c 6f67 5f70 6174  er.__get_log_pat
+00001480: 6829 02da 0670 7265 6669 7872 1400 0000  h)...prefixr....
+00001490: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+000014a0: 0004 0000 0043 0000 0073 2800 0000 7c00  .....C...s(...|.
+000014b0: a000 7c01 9b00 6401 9d02 a101 7d02 7c00  ..|...d.....}.|.
+000014c0: a000 7c01 9b00 6402 9d02 a101 7d03 7c02  ..|...d.....}.|.
+000014d0: 7c03 6602 5300 2903 4e7a 0b5f 7374 6465  |.f.S.).Nz._stde
+000014e0: 7272 2e74 7874 7a0b 5f73 7464 6f75 742e  rr.txtz._stdout.
+000014f0: 7478 7429 01da 1b5f 4c6f 6361 6c42 7569  txt)..._LocalBui
+00001500: 6c64 6572 5f5f 6765 745f 6c6f 675f 7061  lder__get_log_pa
+00001510: 7468 2904 721d 0000 0072 6800 0000 da06  th).r....rh.....
+00001520: 7374 6465 7272 da06 7374 646f 7574 721e  stderr..stdoutr.
+00001530: 0000 0072 1e00 0000 721f 0000 005a 0f5f  ...r....r....Z._
+00001540: 5f67 6574 5f73 7464 5f70 6174 6873 b000  _get_std_paths..
+00001550: 0000 7306 0000 0000 0110 0110 017a 1c4c  ..s..........z.L
+00001560: 6f63 616c 4275 696c 6465 722e 5f5f 6765  ocalBuilder.__ge
+00001570: 745f 7374 645f 7061 7468 73a9 0172 1400  t_std_paths..r..
+00001580: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00001590: 0000 0005 0000 0043 0000 0073 4e00 0000  .......C...sN...
+000015a0: 7c00 6a00 6400 7500 7212 7401 6401 8301  |.j.d.u.r.t.d...
+000015b0: 8201 7c00 6a02 6400 7500 7224 7401 6402  ..|.j.d.u.r$t.d.
+000015c0: 8301 8201 7403 6403 a004 7c00 6a00 7c00  ....t.d...|.j.|.
+000015d0: 6a02 a102 8301 a005 a100 7d01 7c01 6a06  j.........}.|.j.
+000015e0: 6404 6404 6405 8d02 0100 7c01 5300 2906  d.d.d.....|.S.).
+000015f0: 4e72 6100 0000 7a35 6e6f 2062 696e 2070  Nra...z5no bin p
+00001600: 6174 6820 7072 6f76 6964 6564 2061 6e64  ath provided and
+00001610: 204b 4153 4b41 4441 5f42 494e 5f50 4154   KASKADA_BIN_PAT
+00001620: 4820 7761 7320 6e6f 7420 7365 747a 057b  H was not setz.{
+00001630: 7d2f 7b7d 5472 6200 0000 2907 7247 0000  }/{}Trb...).rG..
+00001640: 0072 6500 0000 724a 0000 0072 0300 0000  .re...rJ...r....
+00001650: 722c 0000 0072 6600 0000 7267 0000 0029  r,...rf...rg...)
+00001660: 0272 1d00 0000 7254 0000 0072 1e00 0000  .r....rT...r....
+00001670: 721e 0000 0072 1f00 0000 5a11 5f5f 6765  r....r....Z.__ge
+00001680: 745f 6269 6e61 7279 5f70 6174 68b5 0000  t_binary_path...
+00001690: 0073 0e00 0000 0001 0a01 0801 0a01 0801  .s..............
+000016a0: 1801 0e01 7a1e 4c6f 6361 6c42 7569 6c64  ....z.LocalBuild
+000016b0: 6572 2e5f 5f67 6574 5f62 696e 6172 795f  er.__get_binary_
+000016c0: 7061 7468 6301 0000 0000 0000 0000 0000  pathc...........
+000016d0: 000c 0000 0005 0000 0043 0000 0073 d600  .........C...s..
+000016e0: 0000 7c00 a000 a100 7c00 6a01 1b00 7d01  ..|.....|.j...}.
+000016f0: 7c00 a002 6401 a101 5c02 7d02 7d03 7c00  |...d...\.}.}.|.
+00001700: a000 a100 7c00 6a03 1b00 7d04 7c00 a002  ....|.j...}.|...
+00001710: 6402 a101 5c02 7d05 7d06 6403 7d07 7404  d...\.}.}.d.}.t.
+00001720: 7c01 8301 6701 7c00 a005 a100 1700 7d08  |...g.|.......}.
+00001730: 7406 a007 6404 7c08 9b00 9d02 a101 0100  t...d.|.........
+00001740: 7c04 7c07 6702 7d09 7406 a007 6405 7c09  |.|.g.}.t...d.|.
+00001750: 9b00 9d02 a101 0100 7406 a008 6406 a101  ........t...d...
+00001760: 0100 7406 a008 6407 a101 0100 7406 a008  ..t...d.....t...
+00001770: 6408 a101 0100 7409 a00a 7c08 7c02 7c03  d.....t...|.|.|.
+00001780: a103 7d0a 7406 a008 6409 a101 0100 7406  ..}.t...d.....t.
+00001790: a008 640a a101 0100 7406 a008 640b a101  ..d.....t...d...
+000017a0: 0100 7409 a00a 7c09 7c05 7c06 a103 7d0b  ..t...|.|.|...}.
+000017b0: 7c0a 7c0b 6602 5300 290c 4eda 076d 616e  |.|.f.S.).N..man
+000017c0: 6167 6572 da06 656e 6769 6e65 5a05 7365  ager..engineZ.se
+000017d0: 7276 657a 174d 616e 6167 6572 2073 7461  rvez.Manager sta
+000017e0: 7274 2063 6f6d 6d61 6e64 3a20 7a16 456e  rt command: z.En
+000017f0: 6769 6e65 2073 7461 7274 2063 6f6d 6d61  gine start comma
+00001800: 6e64 3a20 7a1c 496e 6974 6961 6c69 7a69  nd: z.Initializi
+00001810: 6e67 206d 616e 6167 6572 2070 726f 6365  ng manager proce
+00001820: 7373 7a2b 4c6f 6767 696e 6720 6d61 6e61  ssz+Logging mana
+00001830: 6765 7220 5354 444f 5554 2074 6f20 7b6d  ger STDOUT to {m
+00001840: 616e 6167 6572 5f73 7464 5f6f 7574 7d7a  anager_std_out}z
+00001850: 2b4c 6f67 6769 6e67 206d 616e 6167 6572  +Logging manager
+00001860: 2053 5444 4552 5220 746f 207b 6d61 6e61   STDERR to {mana
+00001870: 6765 725f 7374 645f 6572 727d 7a1b 496e  ger_std_err}z.In
+00001880: 6974 6961 6c69 7a69 6e67 2065 6e67 696e  itializing engin
+00001890: 6520 7072 6f63 6573 737a 294c 6f67 6769  e processz)Loggi
+000018a0: 6e67 2065 6e67 696e 6520 5354 444f 5554  ng engine STDOUT
+000018b0: 2074 6f20 7b65 6e67 696e 655f 7374 645f   to {engine_std_
+000018c0: 6f75 747d 7a29 4c6f 6767 696e 6720 656e  out}z)Logging en
+000018d0: 6769 6e65 2053 5444 4552 5220 746f 207b  gine STDERR to {
+000018e0: 656e 6769 6e65 5f73 7464 5f65 7272 7d29  engine_std_err})
+000018f0: 0bda 1e5f 4c6f 6361 6c42 7569 6c64 6572  ..._LocalBuilder
+00001900: 5f5f 6765 745f 6269 6e61 7279 5f70 6174  __get_binary_pat
+00001910: 68da 204b 4153 4b41 4441 5f4d 414e 4147  h. KASKADA_MANAG
+00001920: 4552 5f42 494e 5f4e 414d 455f 4445 4641  ER_BIN_NAME_DEFA
+00001930: 554c 54da 1c5f 4c6f 6361 6c42 7569 6c64  ULT.._LocalBuild
+00001940: 6572 5f5f 6765 745f 7374 645f 7061 7468  er__get_std_path
+00001950: 73da 1f4b 4153 4b41 4441 5f45 4e47 494e  s..KASKADA_ENGIN
+00001960: 455f 4249 4e5f 4e41 4d45 5f44 4546 4155  E_BIN_NAME_DEFAU
+00001970: 4c54 7234 0000 00da 2a5f 4c6f 6361 6c42  LTr4....*_LocalB
+00001980: 7569 6c64 6572 5f5f 6765 745f 6d61 6e61  uilder__get_mana
+00001990: 6765 725f 636f 6e66 6967 735f 6173 5f61  ger_configs_as_a
+000019a0: 7267 7372 2100 0000 7228 0000 0072 2200  rgsr!...r(...r".
+000019b0: 0000 7209 0000 005a 0e72 756e 5f73 7562  ..r....Z.run_sub
+000019c0: 7072 6f63 6573 7329 0c72 1d00 0000 5a13  process).r....Z.
+000019d0: 6d61 6e61 6765 725f 6269 6e61 7279 5f70  manager_binary_p
+000019e0: 6174 685a 0f6d 616e 6167 6572 5f73 7464  athZ.manager_std
+000019f0: 5f65 7272 5a0f 6d61 6e61 6765 725f 7374  _errZ.manager_st
+00001a00: 645f 6f75 745a 1265 6e67 696e 655f 6269  d_outZ.engine_bi
+00001a10: 6e61 7279 5f70 6174 685a 0e65 6e67 696e  nary_pathZ.engin
+00001a20: 655f 7374 645f 6572 725a 0e65 6e67 696e  e_std_errZ.engin
+00001a30: 655f 7374 645f 6f75 745a 0e65 6e67 696e  e_std_outZ.engin
+00001a40: 655f 636f 6d6d 616e 645a 0b6d 616e 6167  e_commandZ.manag
+00001a50: 6572 5f63 6d64 5a0a 656e 6769 6e65 5f63  er_cmdZ.engine_c
+00001a60: 6d64 7212 0000 0072 1300 0000 721e 0000  mdr....r....r...
+00001a70: 0072 1e00 0000 721f 0000 005a 075f 5f73  .r....r....Z.__s
+00001a80: 7461 7274 be00 0000 7330 0000 0000 020c  tart....s0......
+00001a90: ff02 030e 020c ff02 030e 0104 0212 0110  ................
+00001aa0: 0108 0110 010a 010a 010a 0104 0106 ff04  ................
+00001ab0: 030a 010a 010a 0104 0106 ff04 037a 144c  .............z.L
+00001ac0: 6f63 616c 4275 696c 6465 722e 5f5f 7374  ocalBuilder.__st
+00001ad0: 6172 7463 0100 0000 0000 0000 0000 0000  artc............
+00001ae0: 0400 0000 0600 0000 4300 0000 73aa 0000  ........C...s...
+00001af0: 0074 00a0 01a1 007d 017c 00a0 02a1 007d  .t.....}.|.....}
+00001b00: 027c 026a 0364 0164 0164 028d 0201 007c  .|.j.d.d.d.....|
+00001b10: 01a0 047c 027c 006a 057c 006a 06a1 037d  ...|.|.j.|.j...}
+00001b20: 0374 07a0 0864 037c 036a 099b 009d 02a1  .t...d.|.j......
+00001b30: 0101 0074 07a0 0864 047c 036a 0a9b 009d  ...t...d.|.j....
+00001b40: 02a1 0101 0074 07a0 0864 057c 036a 0b9b  .....t...d.|.j..
+00001b50: 009d 02a1 0101 007c 00a0 0c7c 036a 09a0  .......|...|.j..
+00001b60: 0da1 00a0 0e74 0f7c 006a 1083 01a0 11a1  .....t.|.j......
+00001b70: 00a0 0da1 00a1 01a1 0101 0074 12a0 137c  ...........t...|
+00001b80: 036a 0a64 06a1 0201 0074 12a0 137c 036a  .j.d.....t...|.j
+00001b90: 0b64 06a1 0201 0064 0753 0029 087a 3844  .d.....d.S.).z8D
+00001ba0: 6f77 6e6c 6f61 6473 2074 6865 206c 6174  ownloads the lat
+00001bb0: 6573 7420 7265 6c65 6173 6520 7665 7273  est release vers
+00001bc0: 696f 6e20 746f 2074 6865 2062 696e 6172  ion to the binar
+00001bd0: 7920 7061 7468 2e54 7262 0000 007a 0f44  y path.Trb...z.D
+00001be0: 6f77 6e6c 6f61 6420 5061 7468 3a20 7a0e  ownload Path: z.
+00001bf0: 4d61 6e61 6765 7220 5061 7468 3a20 7a0d  Manager Path: z.
+00001c00: 456e 6769 6e65 2050 6174 683a 2069 ed01  Engine Path: i..
+00001c10: 0000 4e29 1472 0a00 0000 5a0d 5265 6c65  ..N).r....Z.Rele
+00001c20: 6173 6543 6c69 656e 7472 6f00 0000 7267  aseClientro...rg
+00001c30: 0000 005a 1764 6f77 6e6c 6f61 645f 6c61  ...Z.download_la
+00001c40: 7465 7374 5f72 656c 6561 7365 7270 0000  test_releaserp..
+00001c50: 0072 7200 0000 7221 0000 0072 2800 0000  .rr...r!...r(...
+00001c60: 5a0e 5f64 6f77 6e6c 6f61 645f 7061 7468  Z._download_path
+00001c70: 5a0d 5f6d 616e 6167 6572 5f70 6174 685a  Z._manager_pathZ
+00001c80: 0c5f 656e 6769 6e65 5f70 6174 6872 5400  ._engine_pathrT.
+00001c90: 0000 da08 6162 736f 6c75 7465 da0b 7265  ....absolute..re
+00001ca0: 6c61 7469 7665 5f74 6f72 0300 0000 7247  lative_tor....rG
+00001cb0: 0000 0072 6600 0000 7243 0000 00da 0563  ...rf...rC.....c
+00001cc0: 686d 6f64 2904 721d 0000 0072 2e00 0000  hmod).r....r....
+00001cd0: 5a0d 646f 776e 6c6f 6164 5f70 6174 685a  Z.download_pathZ
+00001ce0: 0d6c 6f63 616c 5f72 656c 6561 7365 721e  .local_releaser.
+00001cf0: 0000 0072 1e00 0000 721f 0000 005a 195f  ...r....r....Z._
+00001d00: 5f64 6f77 6e6c 6f61 645f 6c61 7465 7374  _download_latest
+00001d10: 5f72 656c 6561 7365 db00 0000 7324 0000  _release....s$..
+00001d20: 0000 0208 0108 010e 0104 0102 0104 0104  ................
+00001d30: fd04 0512 0112 0112 0204 010a 0110 ff02  ................
+00001d40: ff04 050e 017a 264c 6f63 616c 4275 696c  .....z&LocalBuil
+00001d50: 6465 722e 5f5f 646f 776e 6c6f 6164 5f6c  der.__download_l
+00001d60: 6174 6573 745f 7265 6c65 6173 6563 0100  atest_releasec..
+00001d70: 0000 0000 0000 0000 0000 0300 0000 0800  ................
+00001d80: 0000 4300 0000 735a 0000 007c 006a 0072  ..C...sZ...|.j.r
+00001d90: 0e7c 00a0 01a1 0001 007c 00a0 02a1 005c  .|.......|.....\
+00001da0: 027d 017d 027c 006a 0364 0175 0072 2c74  .}.}.|.j.d.u.r,t
+00001db0: 0464 0283 0182 017c 006a 0564 0175 0072  .d.....|.j.d.u.r
+00001dc0: 3e74 0464 0383 0182 0174 067c 006a 037c  >t.d.....t.|.j.|
+00001dd0: 006a 057c 006a 077c 006a 087c 017c 0264  .j.|.j.|.j.|.|.d
+00001de0: 048d 0653 0029 057a ac42 7569 6c64 7320  ...S.).z.Builds 
+00001df0: 7468 6520 6c6f 6361 6c20 7365 7373 696f  the local sessio
+00001e00: 6e2e 2053 7461 7274 7320 6279 2064 6f77  n. Starts by dow
+00001e10: 6e6c 6f61 6469 6e67 2074 6865 206c 6174  nloading the lat
+00001e20: 6573 7420 7265 6c65 6173 6520 616e 6420  est release and 
+00001e30: 7374 6172 7469 6e67 2074 6865 206c 6f63  starting the loc
+00001e40: 616c 2062 696e 6172 6965 732e 0a0a 2020  al binaries...  
+00001e50: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00001e60: 2020 2020 2020 2020 2020 2053 6573 7369             Sessi
+00001e70: 6f6e 3a20 5468 6520 6c6f 6361 6c20 7365  on: The local se
+00001e80: 7373 696f 6e20 6f62 6a65 6374 0a20 2020  ssion object.   
+00001e90: 2020 2020 204e 7a14 656e 6470 6f69 6e74       Nz.endpoint
+00001ea0: 2077 6173 206e 6f74 2073 6574 7a15 6973   was not setz.is
+00001eb0: 5f73 6563 7572 6520 7761 7320 6e6f 7420  _secure was not 
+00001ec0: 7365 7429 0372 1100 0000 7212 0000 0072  set).r....r....r
+00001ed0: 1300 0000 2909 724f 0000 00da 265f 4c6f  ....).rO....&_Lo
+00001ee0: 6361 6c42 7569 6c64 6572 5f5f 646f 776e  calBuilder__down
+00001ef0: 6c6f 6164 5f6c 6174 6573 745f 7265 6c65  load_latest_rele
+00001f00: 6173 65da 145f 4c6f 6361 6c42 7569 6c64  ase.._LocalBuild
+00001f10: 6572 5f5f 7374 6172 7472 1600 0000 7265  er__startr....re
+00001f20: 0000 0072 1700 0000 720d 0000 0072 1800  ...r....r....r..
+00001f30: 0000 7219 0000 0029 0372 1d00 0000 7212  ..r....).r....r.
+00001f40: 0000 0072 1300 0000 721e 0000 0072 1e00  ...r....r....r..
+00001f50: 0000 721f 0000 00da 0562 7569 6c64 f100  ..r......build..
+00001f60: 0000 731e 0000 0000 0606 0108 010c 010a  ..s.............
+00001f70: 0108 010a 0108 0202 0104 0104 0104 0104  ................
+00001f80: 0102 0102 fa7a 124c 6f63 616c 4275 696c  .....z.LocalBuil
+00001f90: 6465 722e 6275 696c 6429 2372 3100 0000  der.build)#r1...
+00001fa0: 7232 0000 0072 3300 0000 7245 0000 0072  r2...r3...rE...r
+00001fb0: 4600 0000 724c 0000 0072 4b00 0000 7249  F...rL...rK...rI
+00001fc0: 0000 0072 4800 0000 7270 0000 0072 7200  ...rH...rp...rr.
+00001fd0: 0000 724e 0000 00da 184b 4153 4b41 4441  ..rN.....KASKADA
+00001fe0: 5f45 4e44 504f 494e 545f 4445 4641 554c  _ENDPOINT_DEFAUL
+00001ff0: 54da 194b 4153 4b41 4441 5f49 535f 5345  T..KASKADA_IS_SE
+00002000: 4355 5245 5f44 4546 4155 4c54 7234 0000  CURE_DEFAULTr4..
+00002010: 0072 3500 0000 7220 0000 0072 5100 0000  .r5...r ...rQ...
+00002020: 7253 0000 0072 5400 0000 7255 0000 00da  rS...rT...rU....
+00002030: 0369 6e74 7259 0000 0072 5a00 0000 7273  .intrY...rZ...rs
+00002040: 0000 0072 0300 0000 7269 0000 0072 0800  ...r....ri...r..
+00002050: 0000 7271 0000 0072 6f00 0000 7278 0000  ..rq...ro...rx..
+00002060: 0072 7700 0000 720d 0000 0072 7900 0000  .rw...r....ry...
+00002070: 723e 0000 0072 1e00 0000 721e 0000 0072  r>...r....r....r
+00002080: 3800 0000 721f 0000 0072 3f00 0000 6500  8...r....r?...e.
+00002090: 0000 733a 0000 0008 0104 0104 0104 0104  ..s:............
+000020a0: 0104 0104 0204 0104 0204 0402 0102 fd02  ................
+000020b0: 0202 0102 0102 fc10 150e 040e 040e 040e  ................
+000020c0: 040e 040e 0408 0610 0b18 050e 0908 1d08  ................
+000020d0: 1672 3f00 0000 6300 0000 0000 0000 0000  .r?...c.........
+000020e0: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
+000020f0: 2a00 0000 6500 5a01 6400 5a02 6401 6402  *...e.Z.d.Z.d.d.
+00002100: 9c01 8700 6601 6403 6404 840c 5a03 6405  ....f.d.d...Z.d.
+00002110: 6406 8400 5a04 8700 0400 5a05 5300 2907  d...Z.....Z.S.).
+00002120: da0d 5265 6d6f 7465 4275 696c 6465 724e  ..RemoteBuilderN
+00002130: 726c 0000 0063 0100 0000 0000 0000 0000  rl...c..........
+00002140: 0000 0100 0000 0200 0000 0300 0000 730e  ..............s.
+00002150: 0000 0074 0083 00a0 01a1 0001 0064 0053  ...t.........d.S
+00002160: 0072 1500 0000 2902 7237 0000 0072 2000  .r....).r7...r .
+00002170: 0000 7224 0000 0072 3800 0000 721e 0000  ..r$...r8...r...
+00002180: 0072 1f00 0000 7220 0000 000a 0100 0073  .r....r .......s
+00002190: 0200 0000 0001 7a16 5265 6d6f 7465 4275  ......z.RemoteBu
+000021a0: 696c 6465 722e 5f5f 696e 6974 5f5f 6301  ilder.__init__c.
+000021b0: 0000 0000 0000 0000 0000 0001 0000 0006  ................
+000021c0: 0000 0043 0000 0073 1800 0000 7400 7c00  ...C...s....t.|.
+000021d0: 6a01 7c00 6a02 7c00 6a03 7c00 6a04 6401  j.|.j.|.j.|.j.d.
+000021e0: 8d04 5300 2902 4e72 3b00 0000 2905 720d  ..S.).Nr;...).r.
+000021f0: 0000 0072 1600 0000 7217 0000 0072 1800  ...r....r....r..
+00002200: 0000 7219 0000 0072 2400 0000 721e 0000  ..r....r$...r...
+00002210: 0072 1e00 0000 721f 0000 0072 7900 0000  .r....r....ry...
+00002220: 0d01 0000 7306 0000 0000 0102 0110 ff7a  ....s..........z
+00002230: 1352 656d 6f74 6542 7569 6c64 6572 2e62  .RemoteBuilder.b
+00002240: 7569 6c64 2906 7231 0000 0072 3200 0000  uild).r1...r2...
+00002250: 7233 0000 0072 2000 0000 7279 0000 0072  r3...r ...ry...r
+00002260: 3e00 0000 721e 0000 0072 1e00 0000 7238  >...r....r....r8
+00002270: 0000 0072 1f00 0000 727d 0000 0009 0100  ...r....r}......
+00002280: 0073 0400 0000 0801 1203 727d 0000 0029  .s........r}...)
+00002290: 21da 076c 6f67 6769 6e67 7243 0000 00da  !..loggingrC....
+000022a0: 0373 7973 7229 0000 0072 3c00 0000 da03  .sysr)...r<.....
+000022b0: 6162 6372 0200 0000 da07 7061 7468 6c69  abcr......pathli
+000022c0: 6272 0300 0000 da0a 7375 6270 726f 6365  br......subproce
+000022d0: 7373 7204 0000 00da 0674 7970 696e 6772  ssr......typingr
+000022e0: 0500 0000 7206 0000 0072 0700 0000 7208  ....r....r....r.
+000022f0: 0000 00da 0e6b 6173 6b61 6461 2e63 6c69  .....kaskada.cli
+00002300: 656e 7472 2d00 0000 5a0b 6b61 736b 6164  entr-...Z.kaskad
+00002310: 612e 6170 6972 0900 0000 720a 0000 00da  a.apir....r.....
+00002320: 0b62 6173 6963 436f 6e66 6967 726b 0000  .basicConfigrk..
+00002330: 00da 0449 4e46 4fda 0967 6574 4c6f 6767  ...INFO..getLogg
+00002340: 6572 7231 0000 0072 2100 0000 720d 0000  err1...r!...r...
+00002350: 0072 3600 0000 727a 0000 0072 7b00 0000  .r6...rz...r{...
+00002360: 723f 0000 0072 7d00 0000 721e 0000 0072  r?...r}...r....r
+00002370: 1e00 0000 721e 0000 0072 1f00 0000 da08  ....r....r......
+00002380: 3c6d 6f64 756c 653e 0100 0000 7326 0000  <module>....s&..
+00002390: 0008 0108 0108 0108 0108 010c 010c 010c  ................
+000023a0: 0118 0208 0110 0212 010a 030e 3310 1c04  ............3...
+000023b0: 0104 0310 7f00 25                        ......%
```

### Comparing `kaskada-0.1.4/src/kaskada/api/api_utils.py` & `kaskada-0.1.5/src/kaskada/api/api_utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/api/release.py` & `kaskada-0.1.5/src/kaskada/api/release.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/api/session.py` & `kaskada-0.1.5/src/kaskada/api/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,19 +31,23 @@
         self._client_id = client_id
         self._client = self.connect()
         self._manager_process = manager_process
         self._engine_process = engine_process
 
     def __del__(self):
         if self._manager_process is not None:
-            logger.info("Stopping Kaskada Manager service")
+            logger.info(
+                "Stopping Kaskada Manager service"
+            ) if logger is not None else None
             self._manager_process.kill()
 
         if self._engine_process is not None:
-            logger.info("Stopping Kaskada Engine service")
+            logger.info(
+                "Stopping Kaskada Engine service"
+            ) if logger is not None else None
             self._engine_process.kill()
 
     def connect(self):
         attempt = 0
         is_valid_session = False
         while attempt < 3 and not is_valid_session:
             logger.debug(f"Attempting (try #{attempt}) to connect to {self._endpoint}")
@@ -101,14 +105,16 @@
     KASKADA_LOG_PATH_ENV = "KASKADA_LOG_PATH"
     KASKADA_BIN_PATH_DEFAULT = "bin"
     KASKADA_BIN_PATH_ENV = "KASKADA_BIN_PATH"
 
     KASKADA_MANAGER_BIN_NAME_DEFAULT = "kaskada-manager"
     KASKADA_ENGINE_BIN_NAME_DEFAULT = "kaskada-engine"
 
+    KASKADA_DISABLE_DOWNLOAD_ENV = "KASKADA_DISABLE_DOWNLOAD"
+
     def __init__(
         self,
         endpoint: str = KASKADA_ENDPOINT_DEFAULT,
         is_secure: bool = KASKADA_IS_SECURE_DEFAULT,
     ) -> None:
         super().__init__()
         self._path: str = os.getenv(
@@ -117,15 +123,17 @@
         self._bin_path: str = os.getenv(
             LocalBuilder.KASKADA_BIN_PATH_ENV, LocalBuilder.KASKADA_BIN_PATH_DEFAULT
         )
         self._log_path: str = os.getenv(
             LocalBuilder.KASKADA_LOG_PATH_ENV, LocalBuilder.KASKADA_LOG_PATH_DEFAULT
         )
         self.endpoint(endpoint, is_secure)
-        self._download = True
+        self._download = (
+            os.getenv(LocalBuilder.KASKADA_DISABLE_DOWNLOAD_ENV, "false") != "true"
+        )
         self._manager_configs: Dict[str, Any] = {}
 
     def path(self, path: str):
         self._path = path
         return self
 
     def log_path(self, path: str):
@@ -191,18 +199,22 @@
         engine_command = "serve"
 
         manager_cmd = [str(manager_binary_path)] + self.__get_manager_configs_as_args()
         logger.debug(f"Manager start command: {manager_cmd}")
         engine_cmd = [engine_binary_path, engine_command]
         logger.debug(f"Engine start command: {engine_cmd}")
         logger.info("Initializing manager process")
+        logger.info("Logging manager STDOUT to {manager_std_out}")
+        logger.info("Logging manager STDERR to {manager_std_err}")
         manager_process = api_utils.run_subprocess(
             manager_cmd, manager_std_err, manager_std_out
         )
         logger.info("Initializing engine process")
+        logger.info("Logging engine STDOUT to {engine_std_out}")
+        logger.info("Logging engine STDERR to {engine_std_err}")
         engine_process = api_utils.run_subprocess(
             engine_cmd, engine_std_err, engine_std_out
         )
         return (manager_process, engine_process)
 
     def __download_latest_release(self):
         """Downloads the latest release version to the binary path."""
```

### Comparing `kaskada-0.1.4/src/kaskada/client.py` & `kaskada-0.1.5/src/kaskada/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         metadata: List[Tuple[str, str]] = []
         if self.client_id is not None:
             metadata.append(("client-id", self.client_id))
         return metadata
 
 
 def validate_client(client: Client):
-    """Valides the client by checking the service stubs
+    """Validates the client by checking the service stubs
 
     Args:
         client (Client): The client to validate
 
     Raises:
         ValueError: View service stub was not initialized properly.
         ValueError: Table service stubs was not initialized properly.
@@ -155,15 +155,16 @@
     Raises:
         ValueError: No client is initialized or client is improperly initialized
 
     Returns:
         Client: The provided client argument or the global client.
     """
     if client is None and KASKADA_DEFAULT_CLIENT is None:
-        raise ValueError("Client must be provided")
+        raise ValueError(
+            "No client was provided, and no global client is configured. Consider setting the global client by creating a session, for example 'kaskada.api.session.LocalBuilder().build()`."
+        )
     elif client is None:
         client = KASKADA_DEFAULT_CLIENT
 
-    if client is None:
-        raise ValueError("Client must be provided")
+    assert client is not None  # make mypy happy
     validate_client(client)
     return client
```

### Comparing `kaskada-0.1.4/src/kaskada/formatters.css` & `kaskada-0.1.5/src/kaskada/formatters.css`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/formatters.js` & `kaskada-0.1.5/src/kaskada/formatters.js`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/formatters.py` & `kaskada-0.1.5/src/kaskada/formatters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/formatters_helpers.py` & `kaskada-0.1.5/src/kaskada/formatters_helpers.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/formatters_shared.py` & `kaskada-0.1.5/src/kaskada/formatters_shared.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/common_pb2.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/common_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 13053 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 fd32 0000  o.........5d.2..
+00000000: 610d 0d0a 0000 0000 2038 4164 fd32 0000  a....... 8Ad.2..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000c 0000 0040 0000 0073 6204 0000 6400  .....@...sb...d.
+00000020: 000c 0000 0040 0000 0073 5e04 0000 6400  .....@...s^...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a05 0100 6401 6404 6c03  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c03 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c03 6d0a 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c03 6d0c 5a0d 0100 650d a00e a100  d.l.m.Z...e.....
 00000080: 5a0f 6401 6408 6c03 6d10 5a11 0100 6401  Z.d.d.l.m.Z...d.
 00000090: 6409 6c03 6d12 5a13 0100 6401 640a 6c14  d.l.m.Z...d.d.l.
@@ -52,353 +52,348 @@
 00000330: a103 6536 6420 6422 9c04 a103 5a48 650f  ..e6d d"....ZHe.
 00000340: a03e 6548 a101 0100 650f a03e 6548 6a45  .>eH....e..>eHjE
 00000350: a101 0100 650f a03e 6548 6a46 a101 0100  ....e..>eHjF....
 00000360: 650b a03b 641e 6509 6a3c 6601 6539 6420  e..;d.e.j<f.e9d 
 00000370: 6421 9c02 a103 5a49 650f a03e 6549 a101  d!....ZIe..>eI..
 00000380: 0100 650b a03b 641f 6509 6a3c 6601 653a  ..e..;d.e.j<f.e:
 00000390: 6420 6421 9c02 a103 5a4a 650f a03e 654a  d d!....ZJe..>eJ
-000003a0: a101 0100 6505 6a4b 6423 6b02 9002 722f  ....e.jKd#k...r/
+000003a0: a101 0100 6505 6a4b 6423 6b02 9004 725a  ....e.jKd#k...rZ
 000003b0: 6424 651c 5f4c 6425 651c 5f4d 6426 651e  d$e._Ld%e._Md&e.
 000003c0: 5f4e 6427 651e 5f4f 6428 6521 5f4e 6429  _Nd'e._Od(e!_Nd)
 000003d0: 6521 5f4f 642a 652b 5f4e 642b 652b 5f4f  e!_Od*e+_Nd+e+_O
 000003e0: 642c 652c 5f4e 642d 652c 5f4f 642e 652d  d,e,_Nd-e,_Od.e-
 000003f0: 5f4e 642f 652d 5f4f 6430 652e 5f4e 6431  _Nd/e-_Od0e._Nd1
 00000400: 652e 5f4f 6432 652f 5f4e 6433 652f 5f4f  e._Od2e/_Nd3e/_O
 00000410: 6434 6530 5f4e 6435 6530 5f4f 6436 6531  d4e0_Nd5e0_Od6e1
 00000420: 5f4e 6437 6531 5f4f 6438 6533 5f4e 6439  _Nd7e1_Od8e3_Nd9
 00000430: 6533 5f4f 643a 6534 5f4e 643b 6534 5f4f  e3_Od:e4_Nd;e4_O
 00000440: 643c 6535 5f4e 643d 6535 5f4f 643e 6536  d<e5_Nd=e5_Od>e6
 00000450: 5f4e 643f 6536 5f4f 6438 6537 5f4e 6439  _Nd?e6_Od8e7_Nd9
 00000460: 6537 5f4f 6440 6538 5f4e 6441 6538 5f4f  e7_Od@e8_NdAe8_O
 00000470: 6442 6539 5f4e 6443 6539 5f4f 6444 653a  dBe9_NdCe9_OdDe:
-00000480: 5f4e 6445 653a 5f4f 6424 5300 6424 5300  _NdEe:_Od$S.d$S.
-00000490: 2946 7a1f 4765 6e65 7261 7465 6420 7072  )Fz.Generated pr
-000004a0: 6f74 6f63 6f6c 2062 7566 6665 7220 636f  otocol buffer co
-000004b0: 6465 2ee9 0000 0000 2901 da11 656e 756d  de......)...enum
-000004c0: 5f74 7970 655f 7772 6170 7065 7229 01da  _type_wrapper)..
-000004d0: 0a64 6573 6372 6970 746f 7229 01da 0f64  .descriptor)...d
-000004e0: 6573 6372 6970 746f 725f 706f 6f6c 2901  escriptor_pool).
-000004f0: da07 6d65 7373 6167 6529 01da 0a72 6566  ..message)...ref
-00000500: 6c65 6374 696f 6e29 01da 0f73 796d 626f  lection)...symbo
-00000510: 6c5f 6461 7461 6261 7365 2901 da0d 7469  l_database)...ti
-00000520: 6d65 7374 616d 705f 7062 3229 01da 0c77  mestamp_pb2)...w
-00000530: 7261 7070 6572 735f 7062 3229 01da 1466  rappers_pb2)...f
-00000540: 656e 6c5f 6469 6167 6e6f 7374 6963 735f  enl_diagnostics_
-00000550: 7062 3229 01da 0a70 756c 7361 725f 7062  pb2)...pulsar_pb
-00000560: 3229 01da 0a73 6368 656d 615f 7062 3273  2)...schema_pb2s
-00000570: 570a 0000 0a24 6b61 736b 6164 612f 6b61  W....$kaskada/ka
-00000580: 736b 6164 612f 7631 616c 7068 612f 636f  skada/v1alpha/co
-00000590: 6d6d 6f6e 2e70 726f 746f 1217 6b61 736b  mmon.proto..kask
-000005a0: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-000005b0: 7068 611a 1f67 6f6f 676c 652f 7072 6f74  pha..google/prot
-000005c0: 6f62 7566 2f74 696d 6573 7461 6d70 2e70  obuf/timestamp.p
-000005d0: 726f 746f 1a1e 676f 6f67 6c65 2f70 726f  roto..google/pro
-000005e0: 746f 6275 662f 7772 6170 7065 7273 2e70  tobuf/wrappers.p
-000005f0: 726f 746f 1a2e 6b61 736b 6164 612f 6b61  roto..kaskada/ka
-00000600: 736b 6164 612f 7631 616c 7068 612f 6665  skada/v1alpha/fe
-00000610: 6e6c 5f64 6961 676e 6f73 7469 6373 2e70  nl_diagnostics.p
-00000620: 726f 746f 1a24 6b61 736b 6164 612f 6b61  roto.$kaskada/ka
-00000630: 736b 6164 612f 7631 616c 7068 612f 7075  skada/v1alpha/pu
-00000640: 6c73 6172 2e70 726f 746f 1a24 6b61 736b  lsar.proto.$kask
-00000650: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
-00000660: 7068 612f 7363 6865 6d61 2e70 726f 746f  pha/schema.proto
-00000670: 22d5 010a 0a53 6f75 7263 6544 6174 6112  "....SourceData.
-00000680: 230a 0c70 6172 7175 6574 5f70 6174 6818  #..parquet_path.
-00000690: 0120 0128 0948 0052 0b70 6172 7175 6574  . .(.H.R.parquet
-000006a0: 5061 7468 121b 0a08 6373 765f 7061 7468  Path....csv_path
-000006b0: 1802 2001 2809 4800 5207 6373 7650 6174  .. .(.H.R.csvPat
-000006c0: 6812 1b0a 0863 7376 5f64 6174 6118 0320  h....csv_data.. 
-000006d0: 0128 0948 0052 0763 7376 4461 7461 125e  .(.H.R.csvData.^
-000006e0: 0a13 7075 6c73 6172 5f73 7562 7363 7269  ..pulsar_subscri
-000006f0: 7074 696f 6e18 0420 0128 0b32 2b2e 6b61  ption.. .(.2+.ka
-00000700: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
-00000710: 616c 7068 612e 5075 6c73 6172 5375 6273  alpha.PulsarSubs
-00000720: 6372 6970 7469 6f6e 4800 5212 7075 6c73  criptionH.R.puls
-00000730: 6172 5375 6273 6372 6970 7469 6f6e 4208  arSubscriptionB.
-00000740: 0a06 736f 7572 6365 225d 0a09 4669 6c65  ..source"]..File
-00000750: 496e 7075 7412 3e0a 0966 696c 655f 7479  Input.>..file_ty
-00000760: 7065 1801 2001 280e 3221 2e6b 6173 6b61  pe.. .(.2!.kaska
-00000770: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-00000780: 6861 2e46 696c 6554 7970 6552 0866 696c  ha.FileTypeR.fil
-00000790: 6554 7970 6512 100a 0375 7269 1802 2001  eType....uri.. .
-000007a0: 2809 5203 7572 6922 630a 0b46 696c 6552  (.R.uri"c..FileR
-000007b0: 6573 756c 7473 123e 0a09 6669 6c65 5f74  esults.>..file_t
-000007c0: 7970 6518 0120 0128 0e32 212e 6b61 736b  ype.. .(.2!.kask
-000007d0: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-000007e0: 7068 612e 4669 6c65 5479 7065 5208 6669  pha.FileTypeR.fi
-000007f0: 6c65 5479 7065 1214 0a05 7061 7468 7318  leType....paths.
-00000800: 0220 0328 0952 0570 6174 6873 22f5 010a  . .(.R.paths"...
-00000810: 0b54 6162 6c65 436f 6e66 6967 1212 0a04  .TableConfig....
-00000820: 6e61 6d65 1801 2001 2809 5204 6e61 6d65  name.. .(.R.name
-00000830: 1212 0a04 7575 6964 1806 2001 2809 5204  ....uuid.. .(.R.
-00000840: 7575 6964 1228 0a10 7469 6d65 5f63 6f6c  uuid.(..time_col
-00000850: 756d 6e5f 6e61 6d65 1802 2001 2809 520e  umn_name.. .(.R.
-00000860: 7469 6d65 436f 6c75 6d6e 4e61 6d65 124c  timeColumnName.L
-00000870: 0a13 7375 6273 6f72 745f 636f 6c75 6d6e  ..subsort_column
-00000880: 5f6e 616d 6518 0320 0128 0b32 1c2e 676f  _name.. .(.2..go
-00000890: 6f67 6c65 2e70 726f 746f 6275 662e 5374  ogle.protobuf.St
-000008a0: 7269 6e67 5661 6c75 6552 1173 7562 736f  ringValueR.subso
-000008b0: 7274 436f 6c75 6d6e 4e61 6d65 122a 0a11  rtColumnName.*..
-000008c0: 6772 6f75 705f 636f 6c75 6d6e 5f6e 616d  group_column_nam
-000008d0: 6518 0420 0128 0952 0f67 726f 7570 436f  e.. .(.R.groupCo
-000008e0: 6c75 6d6e 4e61 6d65 121a 0a08 6772 6f75  lumnName....grou
-000008f0: 7069 6e67 1805 2001 2809 5208 6772 6f75  ping.. .(.R.grou
-00000900: 7069 6e67 2267 0a0d 5461 626c 654d 6574  ping"g..TableMet
-00000910: 6164 6174 6112 370a 0673 6368 656d 6118  adata.7..schema.
-00000920: 0120 0128 0b32 1f2e 6b61 736b 6164 612e  . .(.2..kaskada.
-00000930: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
-00000940: 5363 6865 6d61 5206 7363 6865 6d61 121d  SchemaR.schema..
-00000950: 0a0a 6669 6c65 5f63 6f75 6e74 1802 2001  ..file_count.. .
-00000960: 2803 5209 6669 6c65 436f 756e 7422 e601  (.R.fileCount"..
-00000970: 0a0c 5072 6570 6172 6564 4669 6c65 1212  ..PreparedFile..
-00000980: 0a04 7061 7468 1801 2001 2809 5204 7061  ..path.. .(.R.pa
-00000990: 7468 1240 0a0e 6d69 6e5f 6576 656e 745f  th.@..min_event_
-000009a0: 7469 6d65 1802 2001 280b 321a 2e67 6f6f  time.. .(.2..goo
-000009b0: 676c 652e 7072 6f74 6f62 7566 2e54 696d  gle.protobuf.Tim
-000009c0: 6573 7461 6d70 520c 6d69 6e45 7665 6e74  estampR.minEvent
-000009d0: 5469 6d65 1240 0a0e 6d61 785f 6576 656e  Time.@..max_even
-000009e0: 745f 7469 6d65 1803 2001 280b 321a 2e67  t_time.. .(.2..g
-000009f0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e54  oogle.protobuf.T
-00000a00: 696d 6573 7461 6d70 520c 6d61 7845 7665  imestampR.maxEve
-00000a10: 6e74 5469 6d65 1219 0a08 6e75 6d5f 726f  ntTime....num_ro
-00000a20: 7773 1804 2001 2803 5207 6e75 6d52 6f77  ws.. .(.R.numRow
-00000a30: 7312 230a 0d6d 6574 6164 6174 615f 7061  s.#..metadata_pa
-00000a40: 7468 1805 2001 2809 520c 6d65 7461 6461  th.. .(.R.metada
-00000a50: 7461 5061 7468 22b5 020a 0953 6c69 6365  taPath"....Slice
-00000a60: 506c 616e 121d 0a0a 7461 626c 655f 6e61  Plan....table_na
-00000a70: 6d65 1801 2001 2809 5209 7461 626c 654e  me.. .(.R.tableN
-00000a80: 616d 6512 4b0a 0770 6572 6365 6e74 1802  ame.K..percent..
-00000a90: 2001 280b 322f 2e6b 6173 6b61 6461 2e6b   .(.2/.kaskada.k
-00000aa0: 6173 6b61 6461 2e76 3161 6c70 6861 2e53  askada.v1alpha.S
-00000ab0: 6c69 6365 506c 616e 2e50 6572 6365 6e74  licePlan.Percent
-00000ac0: 536c 6963 6548 0052 0770 6572 6365 6e74  SliceH.R.percent
-00000ad0: 1255 0a0b 656e 7469 7479 5f6b 6579 7318  .U..entity_keys.
-00000ae0: 0320 0128 0b32 322e 6b61 736b 6164 612e  . .(.22.kaskada.
-00000af0: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
-00000b00: 536c 6963 6550 6c61 6e2e 456e 7469 7479  SlicePlan.Entity
-00000b10: 4b65 7973 536c 6963 6548 0052 0a65 6e74  KeysSliceH.R.ent
-00000b20: 6974 794b 6579 731a 280a 0c50 6572 6365  ityKeys.(..Perce
-00000b30: 6e74 536c 6963 6512 180a 0770 6572 6365  ntSlice....perce
-00000b40: 6e74 1801 2001 2801 5207 7065 7263 656e  nt.. .(.R.percen
-00000b50: 741a 320a 0f45 6e74 6974 794b 6579 7353  t.2..EntityKeysS
-00000b60: 6c69 6365 121f 0a0b 656e 7469 7479 5f6b  lice....entity_k
-00000b70: 6579 7318 0120 0328 0952 0a65 6e74 6974  eys.. .(.R.entit
-00000b80: 794b 6579 7342 070a 0573 6c69 6365 222c  yKeysB...slice",
-00000b90: 0a04 5575 6964 1212 0a04 6869 6768 1801  ..Uuid....high..
-00000ba0: 2001 2804 5204 6869 6768 1210 0a03 6c6f   .(.R.high....lo
-00000bb0: 7718 0220 0128 0452 036c 6f77 229f 020a  w.. .(.R.low"...
-00000bc0: 0c53 6c69 6365 5265 7175 6573 7412 4e0a  .SliceRequest.N.
-00000bd0: 0770 6572 6365 6e74 1801 2001 280b 3232  .percent.. .(.22
-00000be0: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
-00000bf0: 2e76 3161 6c70 6861 2e53 6c69 6365 5265  .v1alpha.SliceRe
-00000c00: 7175 6573 742e 5065 7263 656e 7453 6c69  quest.PercentSli
-00000c10: 6365 4800 5207 7065 7263 656e 7412 580a  ceH.R.percent.X.
-00000c20: 0b65 6e74 6974 795f 6b65 7973 1802 2001  .entity_keys.. .
-00000c30: 280b 3235 2e6b 6173 6b61 6461 2e6b 6173  (.25.kaskada.kas
-00000c40: 6b61 6461 2e76 3161 6c70 6861 2e53 6c69  kada.v1alpha.Sli
-00000c50: 6365 5265 7175 6573 742e 456e 7469 7479  ceRequest.Entity
-00000c60: 4b65 7973 536c 6963 6548 0052 0a65 6e74  KeysSliceH.R.ent
-00000c70: 6974 794b 6579 731a 280a 0c50 6572 6365  ityKeys.(..Perce
-00000c80: 6e74 536c 6963 6512 180a 0770 6572 6365  ntSlice....perce
-00000c90: 6e74 1801 2001 2801 5207 7065 7263 656e  nt.. .(.R.percen
-00000ca0: 741a 320a 0f45 6e74 6974 794b 6579 7353  t.2..EntityKeysS
-00000cb0: 6c69 6365 121f 0a0b 656e 7469 7479 5f6b  lice....entity_k
-00000cc0: 6579 7318 0220 0328 0952 0a65 6e74 6974  eys.. .(.R.entit
-00000cd0: 794b 6579 7342 070a 0573 6c69 6365 22c4  yKeysB...slice".
-00000ce0: 010a 0841 6e61 6c79 7369 7312 230a 0d6d  ...Analysis.#..m
-00000cf0: 6973 7369 6e67 5f6e 616d 6573 1801 2003  issing_names.. .
-00000d00: 2809 520c 6d69 7373 696e 674e 616d 6573  (.R.missingNames
-00000d10: 1253 0a10 6665 6e6c 5f64 6961 676e 6f73  .S..fenl_diagnos
-00000d20: 7469 6373 1802 2001 280b 3228 2e6b 6173  tics.. .(.2(.kas
-00000d30: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-00000d40: 6c70 6861 2e46 656e 6c44 6961 676e 6f73  lpha.FenlDiagnos
-00000d50: 7469 6373 520f 6665 6e6c 4469 6167 6e6f  ticsR.fenlDiagno
-00000d60: 7374 6963 7312 1f0a 0b63 616e 5f65 7865  stics....can_exe
-00000d70: 6375 7465 1803 2001 2808 520a 6361 6e45  cute.. .(.R.canE
-00000d80: 7865 6375 7465 121d 0a0a 6672 6565 5f6e  xecute....free_n
-00000d90: 616d 6573 1804 2003 2809 5209 6672 6565  ames.. .(.R.free
-00000da0: 4e61 6d65 7322 2f0a 0e52 6571 7565 7374  Names"/..Request
-00000db0: 4465 7461 696c 7312 1d0a 0a72 6571 7565  Details....reque
-00000dc0: 7374 5f69 6418 0120 0128 0952 0972 6571  st_id.. .(.R.req
-00000dd0: 7565 7374 4964 2a4f 0a08 4669 6c65 5479  uestId*O..FileTy
-00000de0: 7065 1219 0a15 4649 4c45 5f54 5950 455f  pe....FILE_TYPE_
-00000df0: 554e 5350 4543 4946 4945 4410 0012 150a  UNSPECIFIED.....
-00000e00: 1146 494c 455f 5459 5045 5f50 4152 5155  .FILE_TYPE_PARQU
-00000e10: 4554 1001 1211 0a0d 4649 4c45 5f54 5950  ET......FILE_TYP
-00000e20: 455f 4353 5610 022a 9b01 0a11 5065 7245  E_CSV..*....PerE
-00000e30: 6e74 6974 7942 6568 6176 696f 7212 230a  ntityBehavior.#.
-00000e40: 1f50 4552 5f45 4e54 4954 595f 4245 4841  .PER_ENTITY_BEHA
-00000e50: 5649 4f52 5f55 4e53 5045 4349 4649 4544  VIOR_UNSPECIFIED
-00000e60: 1000 121b 0a17 5045 525f 454e 5449 5459  ......PER_ENTITY
-00000e70: 5f42 4548 4156 494f 525f 414c 4c10 0112  _BEHAVIOR_ALL...
-00000e80: 1d0a 1950 4552 5f45 4e54 4954 595f 4245  ...PER_ENTITY_BE
-00000e90: 4841 5649 4f52 5f46 494e 414c 1002 1225  HAVIOR_FINAL...%
-00000ea0: 0a21 5045 525f 454e 5449 5459 5f42 4548  .!PER_ENTITY_BEH
-00000eb0: 4156 494f 525f 4649 4e41 4c5f 4154 5f54  AVIOR_FINAL_AT_T
-00000ec0: 494d 4510 0342 fb01 0a1b 636f 6d2e 6b61  IME..B....com.ka
-00000ed0: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
-00000ee0: 616c 7068 6142 0b43 6f6d 6d6f 6e50 726f  alphaB.CommonPro
-00000ef0: 746f 5001 5a51 6769 7468 7562 2e63 6f6d  toP.ZQgithub.com
-00000f00: 2f6b 6173 6b61 6461 2d61 692f 6b61 736b  /kaskada-ai/kask
-00000f10: 6164 612f 6765 6e2f 7072 6f74 6f2f 676f  ada/gen/proto/go
-00000f20: 2f6b 6173 6b61 6461 2f6b 6173 6b61 6461  /kaskada/kaskada
-00000f30: 2f76 3161 6c70 6861 3b6b 6173 6b61 6461  /v1alpha;kaskada
-00000f40: 7631 616c 7068 61a2 0203 4b4b 58aa 0217  v1alpha...KKX...
-00000f50: 4b61 736b 6164 612e 4b61 736b 6164 612e  Kaskada.Kaskada.
-00000f60: 5631 616c 7068 61ca 0217 4b61 736b 6164  V1alpha...Kaskad
-00000f70: 615c 4b61 736b 6164 615c 5631 616c 7068  a\Kaskada\V1alph
-00000f80: 61e2 0223 4b61 736b 6164 615c 4b61 736b  a..#Kaskada\Kask
-00000f90: 6164 615c 5631 616c 7068 615c 4750 424d  ada\V1alpha\GPBM
-00000fa0: 6574 6164 6174 61ea 0219 4b61 736b 6164  etadata...Kaskad
-00000fb0: 613a 3a4b 6173 6b61 6461 3a3a 5631 616c  a::Kaskada::V1al
-00000fc0: 7068 6162 0670 726f 746f 33da 0846 696c  phab.proto3..Fil
-00000fd0: 6554 7970 65da 1150 6572 456e 7469 7479  eType..PerEntity
-00000fe0: 4265 6861 7669 6f72 e901 0000 00e9 0200  Behavior........
-00000ff0: 0000 e903 0000 00da 0a53 6f75 7263 6544  .........SourceD
-00001000: 6174 61da 0946 696c 6549 6e70 7574 da0b  ata..FileInput..
-00001010: 4669 6c65 5265 7375 6c74 73da 0b54 6162  FileResults..Tab
-00001020: 6c65 436f 6e66 6967 da0d 5461 626c 654d  leConfig..TableM
-00001030: 6574 6164 6174 61da 0c50 7265 7061 7265  etadata..Prepare
-00001040: 6446 696c 65da 0953 6c69 6365 506c 616e  dFile..SlicePlan
-00001050: da0c 5065 7263 656e 7453 6c69 6365 da0f  ..PercentSlice..
-00001060: 456e 7469 7479 4b65 7973 536c 6963 65da  EntityKeysSlice.
-00001070: 0455 7569 64da 0c53 6c69 6365 5265 7175  .Uuid..SliceRequ
-00001080: 6573 74da 0841 6e61 6c79 7369 73da 0e52  est..Analysis..R
-00001090: 6571 7565 7374 4465 7461 696c 737a 226b  equestDetailsz"k
-000010a0: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
-000010b0: 3161 6c70 6861 2e63 6f6d 6d6f 6e5f 7062  1alpha.common_pb
-000010c0: 3229 02da 0a44 4553 4352 4950 544f 52da  2)...DESCRIPTOR.
-000010d0: 0a5f 5f6d 6f64 756c 655f 5f29 0472 1900  .__module__).r..
-000010e0: 0000 721a 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-000010f0: 0046 4e73 fb00 0000 0a1b 636f 6d2e 6b61  .FNs......com.ka
-00001100: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
-00001110: 616c 7068 6142 0b43 6f6d 6d6f 6e50 726f  alphaB.CommonPro
-00001120: 746f 5001 5a51 6769 7468 7562 2e63 6f6d  toP.ZQgithub.com
-00001130: 2f6b 6173 6b61 6461 2d61 692f 6b61 736b  /kaskada-ai/kask
-00001140: 6164 612f 6765 6e2f 7072 6f74 6f2f 676f  ada/gen/proto/go
-00001150: 2f6b 6173 6b61 6461 2f6b 6173 6b61 6461  /kaskada/kaskada
-00001160: 2f76 3161 6c70 6861 3b6b 6173 6b61 6461  /v1alpha;kaskada
-00001170: 7631 616c 7068 61a2 0203 4b4b 58aa 0217  v1alpha...KKX...
-00001180: 4b61 736b 6164 612e 4b61 736b 6164 612e  Kaskada.Kaskada.
-00001190: 5631 616c 7068 61ca 0217 4b61 736b 6164  V1alpha...Kaskad
-000011a0: 615c 4b61 736b 6164 615c 5631 616c 7068  a\Kaskada\V1alph
-000011b0: 61e2 0223 4b61 736b 6164 615c 4b61 736b  a..#Kaskada\Kask
-000011c0: 6164 615c 5631 616c 7068 615c 4750 424d  ada\V1alpha\GPBM
-000011d0: 6574 6164 6174 61ea 0219 4b61 736b 6164  etadata...Kaskad
-000011e0: 613a 3a4b 6173 6b61 6461 3a3a 5631 616c  a::Kaskada::V1al
-000011f0: 7068 6169 6408 0000 69b3 0800 0069 b608  phaid...i....i..
-00001200: 0000 6951 0900 00e9 ff00 0000 69d4 0100  ..iQ........i...
-00001210: 0069 d601 0000 6933 0200 0069 3502 0000  .i....i3...i5...
-00001220: 6998 0200 0069 9b02 0000 6990 0300 0069  i....i....i....i
-00001230: 9203 0000 69f9 0300 0069 fc03 0000 69e2  ....i....i....i.
-00001240: 0400 0069 e504 0000 691a 0600 0069 b505  ...i....i....i..
-00001250: 0000 69dd 0500 0069 df05 0000 6911 0600  ..i....i....i...
-00001260: 0069 1c06 0000 6948 0600 0069 4b06 0000  .i....iH...iK...
-00001270: 696a 0700 0069 2f07 0000 6961 0700 0069  ij...i/...ia...i
-00001280: 6d07 0000 6931 0800 0069 3308 0000 6962  m...i1...i3...ib
-00001290: 0800 0029 50da 075f 5f64 6f63 5f5f da18  ...)P..__doc__..
-000012a0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-000012b0: 696e 7465 726e 616c 7202 0000 00da 0f67  internalr......g
-000012c0: 6f6f 676c 652e 7072 6f74 6f62 7566 7203  oogle.protobufr.
-000012d0: 0000 00da 0b5f 6465 7363 7269 7074 6f72  ....._descriptor
-000012e0: 7204 0000 00da 105f 6465 7363 7269 7074  r......_descript
-000012f0: 6f72 5f70 6f6f 6c72 0500 0000 da08 5f6d  or_poolr......_m
-00001300: 6573 7361 6765 7206 0000 00da 0b5f 7265  essager......_re
-00001310: 666c 6563 7469 6f6e 7207 0000 00da 105f  flectionr......_
-00001320: 7379 6d62 6f6c 5f64 6174 6162 6173 65da  symbol_database.
-00001330: 0744 6566 6175 6c74 da07 5f73 796d 5f64  .Default.._sym_d
-00001340: 6272 0800 0000 da26 676f 6f67 6c65 5f64  br.....&google_d
-00001350: 6f74 5f70 726f 746f 6275 665f 646f 745f  ot_protobuf_dot_
-00001360: 7469 6d65 7374 616d 705f 5f70 6232 7209  timestamp__pb2r.
-00001370: 0000 00da 2567 6f6f 676c 655f 646f 745f  ....%google_dot_
-00001380: 7072 6f74 6f62 7566 5f64 6f74 5f77 7261  protobuf_dot_wra
-00001390: 7070 6572 735f 5f70 6232 da17 6b61 736b  ppers__pb2..kask
-000013a0: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-000013b0: 7068 6172 0a00 0000 da3a 6b61 736b 6164  phar.....:kaskad
-000013c0: 615f 646f 745f 6b61 736b 6164 615f 646f  a_dot_kaskada_do
-000013d0: 745f 7631 616c 7068 615f 646f 745f 6665  t_v1alpha_dot_fe
-000013e0: 6e6c 5f5f 6469 6167 6e6f 7374 6963 735f  nl__diagnostics_
-000013f0: 5f70 6232 720b 0000 00da 2f6b 6173 6b61  _pb2r...../kaska
-00001400: 6461 5f64 6f74 5f6b 6173 6b61 6461 5f64  da_dot_kaskada_d
-00001410: 6f74 5f76 3161 6c70 6861 5f64 6f74 5f70  ot_v1alpha_dot_p
-00001420: 756c 7361 725f 5f70 6232 720c 0000 00da  ulsar__pb2r.....
-00001430: 2f6b 6173 6b61 6461 5f64 6f74 5f6b 6173  /kaskada_dot_kas
-00001440: 6b61 6461 5f64 6f74 5f76 3161 6c70 6861  kada_dot_v1alpha
-00001450: 5f64 6f74 5f73 6368 656d 615f 5f70 6232  _dot_schema__pb2
-00001460: da11 4164 6453 6572 6961 6c69 7a65 6446  ..AddSerializedF
-00001470: 696c 6572 1f00 0000 da12 656e 756d 5f74  iler......enum_t
-00001480: 7970 6573 5f62 795f 6e61 6d65 da09 5f46  ypes_by_name.._F
-00001490: 494c 4554 5950 45da 0f45 6e75 6d54 7970  ILETYPE..EnumTyp
-000014a0: 6557 7261 7070 6572 720d 0000 00da 125f  eWrapperr......_
-000014b0: 5045 5245 4e54 4954 5942 4548 4156 494f  PERENTITYBEHAVIO
-000014c0: 5272 0e00 0000 da15 4649 4c45 5f54 5950  Rr......FILE_TYP
-000014d0: 455f 554e 5350 4543 4946 4945 44da 1146  E_UNSPECIFIED..F
-000014e0: 494c 455f 5459 5045 5f50 4152 5155 4554  ILE_TYPE_PARQUET
-000014f0: da0d 4649 4c45 5f54 5950 455f 4353 56da  ..FILE_TYPE_CSV.
-00001500: 1f50 4552 5f45 4e54 4954 595f 4245 4841  .PER_ENTITY_BEHA
-00001510: 5649 4f52 5f55 4e53 5045 4349 4649 4544  VIOR_UNSPECIFIED
-00001520: da17 5045 525f 454e 5449 5459 5f42 4548  ..PER_ENTITY_BEH
-00001530: 4156 494f 525f 414c 4cda 1950 4552 5f45  AVIOR_ALL..PER_E
-00001540: 4e54 4954 595f 4245 4841 5649 4f52 5f46  NTITY_BEHAVIOR_F
-00001550: 494e 414c da21 5045 525f 454e 5449 5459  INAL.!PER_ENTITY
-00001560: 5f42 4548 4156 494f 525f 4649 4e41 4c5f  _BEHAVIOR_FINAL_
-00001570: 4154 5f54 494d 45da 156d 6573 7361 6765  AT_TIME..message
-00001580: 5f74 7970 6573 5f62 795f 6e61 6d65 da0b  _types_by_name..
-00001590: 5f53 4f55 5243 4544 4154 41da 0a5f 4649  _SOURCEDATA.._FI
-000015a0: 4c45 494e 5055 54da 0c5f 4649 4c45 5245  LEINPUT.._FILERE
-000015b0: 5355 4c54 53da 0c5f 5441 424c 4543 4f4e  SULTS.._TABLECON
-000015c0: 4649 47da 0e5f 5441 424c 454d 4554 4144  FIG.._TABLEMETAD
-000015d0: 4154 41da 0d5f 5052 4550 4152 4544 4649  ATA.._PREPAREDFI
-000015e0: 4c45 da0a 5f53 4c49 4345 504c 414e da14  LE.._SLICEPLAN..
-000015f0: 6e65 7374 6564 5f74 7970 6573 5f62 795f  nested_types_by_
-00001600: 6e61 6d65 da17 5f53 4c49 4345 504c 414e  name.._SLICEPLAN
-00001610: 5f50 4552 4345 4e54 534c 4943 45da 1a5f  _PERCENTSLICE.._
-00001620: 534c 4943 4550 4c41 4e5f 454e 5449 5459  SLICEPLAN_ENTITY
-00001630: 4b45 5953 534c 4943 45da 055f 5555 4944  KEYSSLICE.._UUID
-00001640: da0d 5f53 4c49 4345 5245 5155 4553 54da  .._SLICEREQUEST.
-00001650: 1a5f 534c 4943 4552 4551 5545 5354 5f50  ._SLICEREQUEST_P
-00001660: 4552 4345 4e54 534c 4943 45da 1d5f 534c  ERCENTSLICE.._SL
-00001670: 4943 4552 4551 5545 5354 5f45 4e54 4954  ICEREQUEST_ENTIT
-00001680: 594b 4559 5353 4c49 4345 da09 5f41 4e41  YKEYSSLICE.._ANA
-00001690: 4c59 5349 53da 0f5f 5245 5155 4553 5444  LYSIS.._REQUESTD
-000016a0: 4554 4149 4c53 da1c 4765 6e65 7261 7465  ETAILS..Generate
-000016b0: 6450 726f 746f 636f 6c4d 6573 7361 6765  dProtocolMessage
-000016c0: 5479 7065 da07 4d65 7373 6167 6572 1200  Type..Messager..
-000016d0: 0000 da0f 5265 6769 7374 6572 4d65 7373  ....RegisterMess
-000016e0: 6167 6572 1300 0000 7214 0000 0072 1500  ager....r....r..
-000016f0: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00001700: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00001710: 721c 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
-00001720: 125f 5553 455f 435f 4445 5343 5249 5054  ._USE_C_DESCRIPT
-00001730: 4f52 53da 085f 6f70 7469 6f6e 73da 135f  ORS.._options.._
-00001740: 7365 7269 616c 697a 6564 5f6f 7074 696f  serialized_optio
-00001750: 6e73 da11 5f73 6572 6961 6c69 7a65 645f  ns.._serialized_
-00001760: 7374 6172 74da 0f5f 7365 7269 616c 697a  start.._serializ
-00001770: 6564 5f65 6e64 a900 7257 0000 0072 5700  ed_end..rW...rW.
-00001780: 0000 fa70 2f68 6f6d 652f 7468 6572 6170  ...p/home/therap
-00001790: 6f6e 2f52 6570 6f73 2f47 6974 4875 622f  on/Repos/GitHub/
-000017a0: 4b61 736b 6164 6141 492f 6b61 736b 6164  KaskadaAI/kaskad
-000017b0: 612f 7265 6c65 6173 696e 672f 636c 6965  a/releasing/clie
-000017c0: 6e74 732f 7079 7468 6f6e 2f73 7263 2f6b  nts/python/src/k
-000017d0: 6173 6b61 6461 2f6b 6173 6b61 6461 2f76  askada/kaskada/v
-000017e0: 3161 6c70 6861 2f63 6f6d 6d6f 6e5f 7062  1alpha/common_pb
-000017f0: 322e 7079 da08 3c6d 6f64 756c 653e 0100  2.py..<module>..
-00001800: 0000 7332 0100 0004 030c 010c 010c 010c  ..s2............
-00001810: 010c 010c 0108 030c 030c 010c 010c 010c  ................
-00001820: 010e 030a 020a 010a 010a 0104 0104 0104  ................
-00001830: 0104 0104 0104 0104 010a 030a 010a 010a  ................
-00001840: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00001850: 010a 010a 010a 010c 0102 0102 0108 fe0a  ................
-00001860: 050c 0202 0102 0108 fe0a 050c 0202 0102  ................
-00001870: 0108 fe0a 050c 0202 0102 0108 fe0a 050c  ................
-00001880: 0202 0102 0108 fe0a 050c 0202 0102 0108  ................
-00001890: fe0a 050c 020c 0202 0102 0106 fe0c 0702  ................
-000018a0: 0102 0106 fe02 0602 0108 f00a 130c 010c  ................
-000018b0: 010c 0202 0102 0108 fe0a 050c 020c 0202  ................
-000018c0: 0102 0106 fe0c 0702 0102 0106 fe02 0602  ................
-000018d0: 0108 f00a 130c 010c 010c 0202 0102 0108  ................
-000018e0: fe0a 050c 0202 0102 0108 fe0a 050c 0206  ................
-000018f0: 0206 0106 0106 0106 0106 0106 0106 0106  ................
-00001900: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00001910: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00001920: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00001930: 0106 0106 010a 0104 db                   .........
+00000480: 5f4e 6445 653a 5f4f 6424 5300 2946 7a1f  _NdEe:_Od$S.)Fz.
+00000490: 4765 6e65 7261 7465 6420 7072 6f74 6f63  Generated protoc
+000004a0: 6f6c 2062 7566 6665 7220 636f 6465 2ee9  ol buffer code..
+000004b0: 0000 0000 2901 da11 656e 756d 5f74 7970  ....)...enum_typ
+000004c0: 655f 7772 6170 7065 7229 01da 0a64 6573  e_wrapper)...des
+000004d0: 6372 6970 746f 7229 01da 0f64 6573 6372  criptor)...descr
+000004e0: 6970 746f 725f 706f 6f6c 2901 da07 6d65  iptor_pool)...me
+000004f0: 7373 6167 6529 01da 0a72 6566 6c65 6374  ssage)...reflect
+00000500: 696f 6e29 01da 0f73 796d 626f 6c5f 6461  ion)...symbol_da
+00000510: 7461 6261 7365 2901 da0d 7469 6d65 7374  tabase)...timest
+00000520: 616d 705f 7062 3229 01da 0c77 7261 7070  amp_pb2)...wrapp
+00000530: 6572 735f 7062 3229 01da 1466 656e 6c5f  ers_pb2)...fenl_
+00000540: 6469 6167 6e6f 7374 6963 735f 7062 3229  diagnostics_pb2)
+00000550: 01da 0a70 756c 7361 725f 7062 3229 01da  ...pulsar_pb2)..
+00000560: 0a73 6368 656d 615f 7062 3273 570a 0000  .schema_pb2sW...
+00000570: 0a24 6b61 736b 6164 612f 6b61 736b 6164  .$kaskada/kaskad
+00000580: 612f 7631 616c 7068 612f 636f 6d6d 6f6e  a/v1alpha/common
+00000590: 2e70 726f 746f 1217 6b61 736b 6164 612e  .proto..kaskada.
+000005a0: 6b61 736b 6164 612e 7631 616c 7068 611a  kaskada.v1alpha.
+000005b0: 1f67 6f6f 676c 652f 7072 6f74 6f62 7566  .google/protobuf
+000005c0: 2f74 696d 6573 7461 6d70 2e70 726f 746f  /timestamp.proto
+000005d0: 1a1e 676f 6f67 6c65 2f70 726f 746f 6275  ..google/protobu
+000005e0: 662f 7772 6170 7065 7273 2e70 726f 746f  f/wrappers.proto
+000005f0: 1a2e 6b61 736b 6164 612f 6b61 736b 6164  ..kaskada/kaskad
+00000600: 612f 7631 616c 7068 612f 6665 6e6c 5f64  a/v1alpha/fenl_d
+00000610: 6961 676e 6f73 7469 6373 2e70 726f 746f  iagnostics.proto
+00000620: 1a24 6b61 736b 6164 612f 6b61 736b 6164  .$kaskada/kaskad
+00000630: 612f 7631 616c 7068 612f 7075 6c73 6172  a/v1alpha/pulsar
+00000640: 2e70 726f 746f 1a24 6b61 736b 6164 612f  .proto.$kaskada/
+00000650: 6b61 736b 6164 612f 7631 616c 7068 612f  kaskada/v1alpha/
+00000660: 7363 6865 6d61 2e70 726f 746f 22d5 010a  schema.proto"...
+00000670: 0a53 6f75 7263 6544 6174 6112 230a 0c70  .SourceData.#..p
+00000680: 6172 7175 6574 5f70 6174 6818 0120 0128  arquet_path.. .(
+00000690: 0948 0052 0b70 6172 7175 6574 5061 7468  .H.R.parquetPath
+000006a0: 121b 0a08 6373 765f 7061 7468 1802 2001  ....csv_path.. .
+000006b0: 2809 4800 5207 6373 7650 6174 6812 1b0a  (.H.R.csvPath...
+000006c0: 0863 7376 5f64 6174 6118 0320 0128 0948  .csv_data.. .(.H
+000006d0: 0052 0763 7376 4461 7461 125e 0a13 7075  .R.csvData.^..pu
+000006e0: 6c73 6172 5f73 7562 7363 7269 7074 696f  lsar_subscriptio
+000006f0: 6e18 0420 0128 0b32 2b2e 6b61 736b 6164  n.. .(.2+.kaskad
+00000700: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00000710: 612e 5075 6c73 6172 5375 6273 6372 6970  a.PulsarSubscrip
+00000720: 7469 6f6e 4800 5212 7075 6c73 6172 5375  tionH.R.pulsarSu
+00000730: 6273 6372 6970 7469 6f6e 4208 0a06 736f  bscriptionB...so
+00000740: 7572 6365 225d 0a09 4669 6c65 496e 7075  urce"]..FileInpu
+00000750: 7412 3e0a 0966 696c 655f 7479 7065 1801  t.>..file_type..
+00000760: 2001 280e 3221 2e6b 6173 6b61 6461 2e6b   .(.2!.kaskada.k
+00000770: 6173 6b61 6461 2e76 3161 6c70 6861 2e46  askada.v1alpha.F
+00000780: 696c 6554 7970 6552 0866 696c 6554 7970  ileTypeR.fileTyp
+00000790: 6512 100a 0375 7269 1802 2001 2809 5203  e....uri.. .(.R.
+000007a0: 7572 6922 630a 0b46 696c 6552 6573 756c  uri"c..FileResul
+000007b0: 7473 123e 0a09 6669 6c65 5f74 7970 6518  ts.>..file_type.
+000007c0: 0120 0128 0e32 212e 6b61 736b 6164 612e  . .(.2!.kaskada.
+000007d0: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
+000007e0: 4669 6c65 5479 7065 5208 6669 6c65 5479  FileTypeR.fileTy
+000007f0: 7065 1214 0a05 7061 7468 7318 0220 0328  pe....paths.. .(
+00000800: 0952 0570 6174 6873 22f5 010a 0b54 6162  .R.paths"....Tab
+00000810: 6c65 436f 6e66 6967 1212 0a04 6e61 6d65  leConfig....name
+00000820: 1801 2001 2809 5204 6e61 6d65 1212 0a04  .. .(.R.name....
+00000830: 7575 6964 1806 2001 2809 5204 7575 6964  uuid.. .(.R.uuid
+00000840: 1228 0a10 7469 6d65 5f63 6f6c 756d 6e5f  .(..time_column_
+00000850: 6e61 6d65 1802 2001 2809 520e 7469 6d65  name.. .(.R.time
+00000860: 436f 6c75 6d6e 4e61 6d65 124c 0a13 7375  ColumnName.L..su
+00000870: 6273 6f72 745f 636f 6c75 6d6e 5f6e 616d  bsort_column_nam
+00000880: 6518 0320 0128 0b32 1c2e 676f 6f67 6c65  e.. .(.2..google
+00000890: 2e70 726f 746f 6275 662e 5374 7269 6e67  .protobuf.String
+000008a0: 5661 6c75 6552 1173 7562 736f 7274 436f  ValueR.subsortCo
+000008b0: 6c75 6d6e 4e61 6d65 122a 0a11 6772 6f75  lumnName.*..grou
+000008c0: 705f 636f 6c75 6d6e 5f6e 616d 6518 0420  p_column_name.. 
+000008d0: 0128 0952 0f67 726f 7570 436f 6c75 6d6e  .(.R.groupColumn
+000008e0: 4e61 6d65 121a 0a08 6772 6f75 7069 6e67  Name....grouping
+000008f0: 1805 2001 2809 5208 6772 6f75 7069 6e67  .. .(.R.grouping
+00000900: 2267 0a0d 5461 626c 654d 6574 6164 6174  "g..TableMetadat
+00000910: 6112 370a 0673 6368 656d 6118 0120 0128  a.7..schema.. .(
+00000920: 0b32 1f2e 6b61 736b 6164 612e 6b61 736b  .2..kaskada.kask
+00000930: 6164 612e 7631 616c 7068 612e 5363 6865  ada.v1alpha.Sche
+00000940: 6d61 5206 7363 6865 6d61 121d 0a0a 6669  maR.schema....fi
+00000950: 6c65 5f63 6f75 6e74 1802 2001 2803 5209  le_count.. .(.R.
+00000960: 6669 6c65 436f 756e 7422 e601 0a0c 5072  fileCount"....Pr
+00000970: 6570 6172 6564 4669 6c65 1212 0a04 7061  eparedFile....pa
+00000980: 7468 1801 2001 2809 5204 7061 7468 1240  th.. .(.R.path.@
+00000990: 0a0e 6d69 6e5f 6576 656e 745f 7469 6d65  ..min_event_time
+000009a0: 1802 2001 280b 321a 2e67 6f6f 676c 652e  .. .(.2..google.
+000009b0: 7072 6f74 6f62 7566 2e54 696d 6573 7461  protobuf.Timesta
+000009c0: 6d70 520c 6d69 6e45 7665 6e74 5469 6d65  mpR.minEventTime
+000009d0: 1240 0a0e 6d61 785f 6576 656e 745f 7469  .@..max_event_ti
+000009e0: 6d65 1803 2001 280b 321a 2e67 6f6f 676c  me.. .(.2..googl
+000009f0: 652e 7072 6f74 6f62 7566 2e54 696d 6573  e.protobuf.Times
+00000a00: 7461 6d70 520c 6d61 7845 7665 6e74 5469  tampR.maxEventTi
+00000a10: 6d65 1219 0a08 6e75 6d5f 726f 7773 1804  me....num_rows..
+00000a20: 2001 2803 5207 6e75 6d52 6f77 7312 230a   .(.R.numRows.#.
+00000a30: 0d6d 6574 6164 6174 615f 7061 7468 1805  .metadata_path..
+00000a40: 2001 2809 520c 6d65 7461 6461 7461 5061   .(.R.metadataPa
+00000a50: 7468 22b5 020a 0953 6c69 6365 506c 616e  th"....SlicePlan
+00000a60: 121d 0a0a 7461 626c 655f 6e61 6d65 1801  ....table_name..
+00000a70: 2001 2809 5209 7461 626c 654e 616d 6512   .(.R.tableName.
+00000a80: 4b0a 0770 6572 6365 6e74 1802 2001 280b  K..percent.. .(.
+00000a90: 322f 2e6b 6173 6b61 6461 2e6b 6173 6b61  2/.kaskada.kaska
+00000aa0: 6461 2e76 3161 6c70 6861 2e53 6c69 6365  da.v1alpha.Slice
+00000ab0: 506c 616e 2e50 6572 6365 6e74 536c 6963  Plan.PercentSlic
+00000ac0: 6548 0052 0770 6572 6365 6e74 1255 0a0b  eH.R.percent.U..
+00000ad0: 656e 7469 7479 5f6b 6579 7318 0320 0128  entity_keys.. .(
+00000ae0: 0b32 322e 6b61 736b 6164 612e 6b61 736b  .22.kaskada.kask
+00000af0: 6164 612e 7631 616c 7068 612e 536c 6963  ada.v1alpha.Slic
+00000b00: 6550 6c61 6e2e 456e 7469 7479 4b65 7973  ePlan.EntityKeys
+00000b10: 536c 6963 6548 0052 0a65 6e74 6974 794b  SliceH.R.entityK
+00000b20: 6579 731a 280a 0c50 6572 6365 6e74 536c  eys.(..PercentSl
+00000b30: 6963 6512 180a 0770 6572 6365 6e74 1801  ice....percent..
+00000b40: 2001 2801 5207 7065 7263 656e 741a 320a   .(.R.percent.2.
+00000b50: 0f45 6e74 6974 794b 6579 7353 6c69 6365  .EntityKeysSlice
+00000b60: 121f 0a0b 656e 7469 7479 5f6b 6579 7318  ....entity_keys.
+00000b70: 0120 0328 0952 0a65 6e74 6974 794b 6579  . .(.R.entityKey
+00000b80: 7342 070a 0573 6c69 6365 222c 0a04 5575  sB...slice",..Uu
+00000b90: 6964 1212 0a04 6869 6768 1801 2001 2804  id....high.. .(.
+00000ba0: 5204 6869 6768 1210 0a03 6c6f 7718 0220  R.high....low.. 
+00000bb0: 0128 0452 036c 6f77 229f 020a 0c53 6c69  .(.R.low"....Sli
+00000bc0: 6365 5265 7175 6573 7412 4e0a 0770 6572  ceRequest.N..per
+00000bd0: 6365 6e74 1801 2001 280b 3232 2e6b 6173  cent.. .(.22.kas
+00000be0: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
+00000bf0: 6c70 6861 2e53 6c69 6365 5265 7175 6573  lpha.SliceReques
+00000c00: 742e 5065 7263 656e 7453 6c69 6365 4800  t.PercentSliceH.
+00000c10: 5207 7065 7263 656e 7412 580a 0b65 6e74  R.percent.X..ent
+00000c20: 6974 795f 6b65 7973 1802 2001 280b 3235  ity_keys.. .(.25
+00000c30: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00000c40: 2e76 3161 6c70 6861 2e53 6c69 6365 5265  .v1alpha.SliceRe
+00000c50: 7175 6573 742e 456e 7469 7479 4b65 7973  quest.EntityKeys
+00000c60: 536c 6963 6548 0052 0a65 6e74 6974 794b  SliceH.R.entityK
+00000c70: 6579 731a 280a 0c50 6572 6365 6e74 536c  eys.(..PercentSl
+00000c80: 6963 6512 180a 0770 6572 6365 6e74 1801  ice....percent..
+00000c90: 2001 2801 5207 7065 7263 656e 741a 320a   .(.R.percent.2.
+00000ca0: 0f45 6e74 6974 794b 6579 7353 6c69 6365  .EntityKeysSlice
+00000cb0: 121f 0a0b 656e 7469 7479 5f6b 6579 7318  ....entity_keys.
+00000cc0: 0220 0328 0952 0a65 6e74 6974 794b 6579  . .(.R.entityKey
+00000cd0: 7342 070a 0573 6c69 6365 22c4 010a 0841  sB...slice"....A
+00000ce0: 6e61 6c79 7369 7312 230a 0d6d 6973 7369  nalysis.#..missi
+00000cf0: 6e67 5f6e 616d 6573 1801 2003 2809 520c  ng_names.. .(.R.
+00000d00: 6d69 7373 696e 674e 616d 6573 1253 0a10  missingNames.S..
+00000d10: 6665 6e6c 5f64 6961 676e 6f73 7469 6373  fenl_diagnostics
+00000d20: 1802 2001 280b 3228 2e6b 6173 6b61 6461  .. .(.2(.kaskada
+00000d30: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00000d40: 2e46 656e 6c44 6961 676e 6f73 7469 6373  .FenlDiagnostics
+00000d50: 520f 6665 6e6c 4469 6167 6e6f 7374 6963  R.fenlDiagnostic
+00000d60: 7312 1f0a 0b63 616e 5f65 7865 6375 7465  s....can_execute
+00000d70: 1803 2001 2808 520a 6361 6e45 7865 6375  .. .(.R.canExecu
+00000d80: 7465 121d 0a0a 6672 6565 5f6e 616d 6573  te....free_names
+00000d90: 1804 2003 2809 5209 6672 6565 4e61 6d65  .. .(.R.freeName
+00000da0: 7322 2f0a 0e52 6571 7565 7374 4465 7461  s"/..RequestDeta
+00000db0: 696c 7312 1d0a 0a72 6571 7565 7374 5f69  ils....request_i
+00000dc0: 6418 0120 0128 0952 0972 6571 7565 7374  d.. .(.R.request
+00000dd0: 4964 2a4f 0a08 4669 6c65 5479 7065 1219  Id*O..FileType..
+00000de0: 0a15 4649 4c45 5f54 5950 455f 554e 5350  ..FILE_TYPE_UNSP
+00000df0: 4543 4946 4945 4410 0012 150a 1146 494c  ECIFIED......FIL
+00000e00: 455f 5459 5045 5f50 4152 5155 4554 1001  E_TYPE_PARQUET..
+00000e10: 1211 0a0d 4649 4c45 5f54 5950 455f 4353  ....FILE_TYPE_CS
+00000e20: 5610 022a 9b01 0a11 5065 7245 6e74 6974  V..*....PerEntit
+00000e30: 7942 6568 6176 696f 7212 230a 1f50 4552  yBehavior.#..PER
+00000e40: 5f45 4e54 4954 595f 4245 4841 5649 4f52  _ENTITY_BEHAVIOR
+00000e50: 5f55 4e53 5045 4349 4649 4544 1000 121b  _UNSPECIFIED....
+00000e60: 0a17 5045 525f 454e 5449 5459 5f42 4548  ..PER_ENTITY_BEH
+00000e70: 4156 494f 525f 414c 4c10 0112 1d0a 1950  AVIOR_ALL......P
+00000e80: 4552 5f45 4e54 4954 595f 4245 4841 5649  ER_ENTITY_BEHAVI
+00000e90: 4f52 5f46 494e 414c 1002 1225 0a21 5045  OR_FINAL...%.!PE
+00000ea0: 525f 454e 5449 5459 5f42 4548 4156 494f  R_ENTITY_BEHAVIO
+00000eb0: 525f 4649 4e41 4c5f 4154 5f54 494d 4510  R_FINAL_AT_TIME.
+00000ec0: 0342 fb01 0a1b 636f 6d2e 6b61 736b 6164  .B....com.kaskad
+00000ed0: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00000ee0: 6142 0b43 6f6d 6d6f 6e50 726f 746f 5001  aB.CommonProtoP.
+00000ef0: 5a51 6769 7468 7562 2e63 6f6d 2f6b 6173  ZQgithub.com/kas
+00000f00: 6b61 6461 2d61 692f 6b61 736b 6164 612f  kada-ai/kaskada/
+00000f10: 6765 6e2f 7072 6f74 6f2f 676f 2f6b 6173  gen/proto/go/kas
+00000f20: 6b61 6461 2f6b 6173 6b61 6461 2f76 3161  kada/kaskada/v1a
+00000f30: 6c70 6861 3b6b 6173 6b61 6461 7631 616c  lpha;kaskadav1al
+00000f40: 7068 61a2 0203 4b4b 58aa 0217 4b61 736b  pha...KKX...Kask
+00000f50: 6164 612e 4b61 736b 6164 612e 5631 616c  ada.Kaskada.V1al
+00000f60: 7068 61ca 0217 4b61 736b 6164 615c 4b61  pha...Kaskada\Ka
+00000f70: 736b 6164 615c 5631 616c 7068 61e2 0223  skada\V1alpha..#
+00000f80: 4b61 736b 6164 615c 4b61 736b 6164 615c  Kaskada\Kaskada\
+00000f90: 5631 616c 7068 615c 4750 424d 6574 6164  V1alpha\GPBMetad
+00000fa0: 6174 61ea 0219 4b61 736b 6164 613a 3a4b  ata...Kaskada::K
+00000fb0: 6173 6b61 6461 3a3a 5631 616c 7068 6162  askada::V1alphab
+00000fc0: 0670 726f 746f 33da 0846 696c 6554 7970  .proto3..FileTyp
+00000fd0: 65da 1150 6572 456e 7469 7479 4265 6861  e..PerEntityBeha
+00000fe0: 7669 6f72 e901 0000 00e9 0200 0000 e903  vior............
+00000ff0: 0000 00da 0a53 6f75 7263 6544 6174 61da  .....SourceData.
+00001000: 0946 696c 6549 6e70 7574 da0b 4669 6c65  .FileInput..File
+00001010: 5265 7375 6c74 73da 0b54 6162 6c65 436f  Results..TableCo
+00001020: 6e66 6967 da0d 5461 626c 654d 6574 6164  nfig..TableMetad
+00001030: 6174 61da 0c50 7265 7061 7265 6446 696c  ata..PreparedFil
+00001040: 65da 0953 6c69 6365 506c 616e da0c 5065  e..SlicePlan..Pe
+00001050: 7263 656e 7453 6c69 6365 da0f 456e 7469  rcentSlice..Enti
+00001060: 7479 4b65 7973 536c 6963 65da 0455 7569  tyKeysSlice..Uui
+00001070: 64da 0c53 6c69 6365 5265 7175 6573 74da  d..SliceRequest.
+00001080: 0841 6e61 6c79 7369 73da 0e52 6571 7565  .Analysis..Reque
+00001090: 7374 4465 7461 696c 737a 226b 6173 6b61  stDetailsz"kaska
+000010a0: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
+000010b0: 6861 2e63 6f6d 6d6f 6e5f 7062 3229 02da  ha.common_pb2)..
+000010c0: 0a44 4553 4352 4950 544f 52da 0a5f 5f6d  .DESCRIPTOR..__m
+000010d0: 6f64 756c 655f 5f29 0472 1900 0000 721a  odule__).r....r.
+000010e0: 0000 0072 1f00 0000 7220 0000 0046 4e73  ...r....r ...FNs
+000010f0: fb00 0000 0a1b 636f 6d2e 6b61 736b 6164  ......com.kaskad
+00001100: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00001110: 6142 0b43 6f6d 6d6f 6e50 726f 746f 5001  aB.CommonProtoP.
+00001120: 5a51 6769 7468 7562 2e63 6f6d 2f6b 6173  ZQgithub.com/kas
+00001130: 6b61 6461 2d61 692f 6b61 736b 6164 612f  kada-ai/kaskada/
+00001140: 6765 6e2f 7072 6f74 6f2f 676f 2f6b 6173  gen/proto/go/kas
+00001150: 6b61 6461 2f6b 6173 6b61 6461 2f76 3161  kada/kaskada/v1a
+00001160: 6c70 6861 3b6b 6173 6b61 6461 7631 616c  lpha;kaskadav1al
+00001170: 7068 61a2 0203 4b4b 58aa 0217 4b61 736b  pha...KKX...Kask
+00001180: 6164 612e 4b61 736b 6164 612e 5631 616c  ada.Kaskada.V1al
+00001190: 7068 61ca 0217 4b61 736b 6164 615c 4b61  pha...Kaskada\Ka
+000011a0: 736b 6164 615c 5631 616c 7068 61e2 0223  skada\V1alpha..#
+000011b0: 4b61 736b 6164 615c 4b61 736b 6164 615c  Kaskada\Kaskada\
+000011c0: 5631 616c 7068 615c 4750 424d 6574 6164  V1alpha\GPBMetad
+000011d0: 6174 61ea 0219 4b61 736b 6164 613a 3a4b  ata...Kaskada::K
+000011e0: 6173 6b61 6461 3a3a 5631 616c 7068 6169  askada::V1alphai
+000011f0: 6408 0000 69b3 0800 0069 b608 0000 6951  d...i....i....iQ
+00001200: 0900 00e9 ff00 0000 69d4 0100 0069 d601  ........i....i..
+00001210: 0000 6933 0200 0069 3502 0000 6998 0200  ..i3...i5...i...
+00001220: 0069 9b02 0000 6990 0300 0069 9203 0000  .i....i....i....
+00001230: 69f9 0300 0069 fc03 0000 69e2 0400 0069  i....i....i....i
+00001240: e504 0000 691a 0600 0069 b505 0000 69dd  ....i....i....i.
+00001250: 0500 0069 df05 0000 6911 0600 0069 1c06  ...i....i....i..
+00001260: 0000 6948 0600 0069 4b06 0000 696a 0700  ..iH...iK...ij..
+00001270: 0069 2f07 0000 6961 0700 0069 6d07 0000  .i/...ia...im...
+00001280: 6931 0800 0069 3308 0000 6962 0800 0029  i1...i3...ib...)
+00001290: 50da 075f 5f64 6f63 5f5f da18 676f 6f67  P..__doc__..goog
+000012a0: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
+000012b0: 726e 616c 7202 0000 00da 0f67 6f6f 676c  rnalr......googl
+000012c0: 652e 7072 6f74 6f62 7566 7203 0000 00da  e.protobufr.....
+000012d0: 0b5f 6465 7363 7269 7074 6f72 7204 0000  ._descriptorr...
+000012e0: 00da 105f 6465 7363 7269 7074 6f72 5f70  ..._descriptor_p
+000012f0: 6f6f 6c72 0500 0000 da08 5f6d 6573 7361  oolr......_messa
+00001300: 6765 7206 0000 00da 0b5f 7265 666c 6563  ger......_reflec
+00001310: 7469 6f6e 7207 0000 00da 105f 7379 6d62  tionr......_symb
+00001320: 6f6c 5f64 6174 6162 6173 65da 0744 6566  ol_database..Def
+00001330: 6175 6c74 da07 5f73 796d 5f64 6272 0800  ault.._sym_dbr..
+00001340: 0000 da26 676f 6f67 6c65 5f64 6f74 5f70  ...&google_dot_p
+00001350: 726f 746f 6275 665f 646f 745f 7469 6d65  rotobuf_dot_time
+00001360: 7374 616d 705f 5f70 6232 7209 0000 00da  stamp__pb2r.....
+00001370: 2567 6f6f 676c 655f 646f 745f 7072 6f74  %google_dot_prot
+00001380: 6f62 7566 5f64 6f74 5f77 7261 7070 6572  obuf_dot_wrapper
+00001390: 735f 5f70 6232 da17 6b61 736b 6164 612e  s__pb2..kaskada.
+000013a0: 6b61 736b 6164 612e 7631 616c 7068 6172  kaskada.v1alphar
+000013b0: 0a00 0000 5a3a 6b61 736b 6164 615f 646f  ....Z:kaskada_do
+000013c0: 745f 6b61 736b 6164 615f 646f 745f 7631  t_kaskada_dot_v1
+000013d0: 616c 7068 615f 646f 745f 6665 6e6c 5f5f  alpha_dot_fenl__
+000013e0: 6469 6167 6e6f 7374 6963 735f 5f70 6232  diagnostics__pb2
+000013f0: 720b 0000 005a 2f6b 6173 6b61 6461 5f64  r....Z/kaskada_d
+00001400: 6f74 5f6b 6173 6b61 6461 5f64 6f74 5f76  ot_kaskada_dot_v
+00001410: 3161 6c70 6861 5f64 6f74 5f70 756c 7361  1alpha_dot_pulsa
+00001420: 725f 5f70 6232 720c 0000 00da 2f6b 6173  r__pb2r...../kas
+00001430: 6b61 6461 5f64 6f74 5f6b 6173 6b61 6461  kada_dot_kaskada
+00001440: 5f64 6f74 5f76 3161 6c70 6861 5f64 6f74  _dot_v1alpha_dot
+00001450: 5f73 6368 656d 615f 5f70 6232 da11 4164  _schema__pb2..Ad
+00001460: 6453 6572 6961 6c69 7a65 6446 696c 6572  dSerializedFiler
+00001470: 1f00 0000 da12 656e 756d 5f74 7970 6573  ......enum_types
+00001480: 5f62 795f 6e61 6d65 5a09 5f46 494c 4554  _by_nameZ._FILET
+00001490: 5950 45da 0f45 6e75 6d54 7970 6557 7261  YPE..EnumTypeWra
+000014a0: 7070 6572 720d 0000 005a 125f 5045 5245  pperr....Z._PERE
+000014b0: 4e54 4954 5942 4548 4156 494f 5272 0e00  NTITYBEHAVIORr..
+000014c0: 0000 5a15 4649 4c45 5f54 5950 455f 554e  ..Z.FILE_TYPE_UN
+000014d0: 5350 4543 4946 4945 445a 1146 494c 455f  SPECIFIEDZ.FILE_
+000014e0: 5459 5045 5f50 4152 5155 4554 5a0d 4649  TYPE_PARQUETZ.FI
+000014f0: 4c45 5f54 5950 455f 4353 565a 1f50 4552  LE_TYPE_CSVZ.PER
+00001500: 5f45 4e54 4954 595f 4245 4841 5649 4f52  _ENTITY_BEHAVIOR
+00001510: 5f55 4e53 5045 4349 4649 4544 5a17 5045  _UNSPECIFIEDZ.PE
+00001520: 525f 454e 5449 5459 5f42 4548 4156 494f  R_ENTITY_BEHAVIO
+00001530: 525f 414c 4c5a 1950 4552 5f45 4e54 4954  R_ALLZ.PER_ENTIT
+00001540: 595f 4245 4841 5649 4f52 5f46 494e 414c  Y_BEHAVIOR_FINAL
+00001550: 5a21 5045 525f 454e 5449 5459 5f42 4548  Z!PER_ENTITY_BEH
+00001560: 4156 494f 525f 4649 4e41 4c5f 4154 5f54  AVIOR_FINAL_AT_T
+00001570: 494d 45da 156d 6573 7361 6765 5f74 7970  IME..message_typ
+00001580: 6573 5f62 795f 6e61 6d65 5a0b 5f53 4f55  es_by_nameZ._SOU
+00001590: 5243 4544 4154 415a 0a5f 4649 4c45 494e  RCEDATAZ._FILEIN
+000015a0: 5055 545a 0c5f 4649 4c45 5245 5355 4c54  PUTZ._FILERESULT
+000015b0: 535a 0c5f 5441 424c 4543 4f4e 4649 475a  SZ._TABLECONFIGZ
+000015c0: 0e5f 5441 424c 454d 4554 4144 4154 415a  ._TABLEMETADATAZ
+000015d0: 0d5f 5052 4550 4152 4544 4649 4c45 5a0a  ._PREPAREDFILEZ.
+000015e0: 5f53 4c49 4345 504c 414e da14 6e65 7374  _SLICEPLAN..nest
+000015f0: 6564 5f74 7970 6573 5f62 795f 6e61 6d65  ed_types_by_name
+00001600: 5a17 5f53 4c49 4345 504c 414e 5f50 4552  Z._SLICEPLAN_PER
+00001610: 4345 4e54 534c 4943 455a 1a5f 534c 4943  CENTSLICEZ._SLIC
+00001620: 4550 4c41 4e5f 454e 5449 5459 4b45 5953  EPLAN_ENTITYKEYS
+00001630: 534c 4943 455a 055f 5555 4944 5a0d 5f53  SLICEZ._UUIDZ._S
+00001640: 4c49 4345 5245 5155 4553 545a 1a5f 534c  LICEREQUESTZ._SL
+00001650: 4943 4552 4551 5545 5354 5f50 4552 4345  ICEREQUEST_PERCE
+00001660: 4e54 534c 4943 455a 1d5f 534c 4943 4552  NTSLICEZ._SLICER
+00001670: 4551 5545 5354 5f45 4e54 4954 594b 4559  EQUEST_ENTITYKEY
+00001680: 5353 4c49 4345 5a09 5f41 4e41 4c59 5349  SSLICEZ._ANALYSI
+00001690: 535a 0f5f 5245 5155 4553 5444 4554 4149  SZ._REQUESTDETAI
+000016a0: 4c53 da1c 4765 6e65 7261 7465 6450 726f  LS..GeneratedPro
+000016b0: 746f 636f 6c4d 6573 7361 6765 5479 7065  tocolMessageType
+000016c0: da07 4d65 7373 6167 6572 1200 0000 da0f  ..Messager......
+000016d0: 5265 6769 7374 6572 4d65 7373 6167 6572  RegisterMessager
+000016e0: 1300 0000 7214 0000 0072 1500 0000 7216  ....r....r....r.
+000016f0: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
+00001700: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00001710: 0072 1d00 0000 721e 0000 00da 125f 5553  .r....r......_US
+00001720: 455f 435f 4445 5343 5249 5054 4f52 53da  E_C_DESCRIPTORS.
+00001730: 085f 6f70 7469 6f6e 73da 135f 7365 7269  ._options.._seri
+00001740: 616c 697a 6564 5f6f 7074 696f 6e73 da11  alized_options..
+00001750: 5f73 6572 6961 6c69 7a65 645f 7374 6172  _serialized_star
+00001760: 74da 0f5f 7365 7269 616c 697a 6564 5f65  t.._serialized_e
+00001770: 6e64 a900 723d 0000 0072 3d00 0000 fa2e  nd..r=...r=.....
+00001780: 2f73 7263 2f73 7263 2f6b 6173 6b61 6461  /src/src/kaskada
+00001790: 2f6b 6173 6b61 6461 2f76 3161 6c70 6861  /kaskada/v1alpha
+000017a0: 2f63 6f6d 6d6f 6e5f 7062 322e 7079 da08  /common_pb2.py..
+000017b0: 3c6d 6f64 756c 653e 0400 0000 732e 0100  <module>....s...
+000017c0: 0004 010c 010c 010c 010c 010c 010c 0308  ................
+000017d0: 030c 010c 010c 010c 010c 030e 020a 010a  ................
+000017e0: 010a 010a 0104 0104 0104 0104 0104 0104  ................
+000017f0: 0104 030a 010a 010a 010a 010a 010a 010a  ................
+00001800: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00001810: 010c 0102 0102 fe08 050a 020c 0102 0102  ................
+00001820: fe08 050a 020c 0102 0102 fe08 050a 020c  ................
+00001830: 0102 0102 fe08 050a 020c 0102 0102 fe08  ................
+00001840: 050a 020c 0102 0102 fe08 050a 020c 020c  ................
+00001850: 0102 0102 fe06 070c 0102 0102 fe06 0602  ................
+00001860: 0102 f008 130a 010c 010c 020c 0102 0102  ................
+00001870: fe08 050a 020c 020c 0102 0102 fe06 070c  ................
+00001880: 0102 0102 fe06 0602 0102 f008 130a 010c  ................
+00001890: 010c 020c 0102 0102 fe08 050a 020c 0102  ................
+000018a0: 0102 fe08 050a 020c 0206 0106 0106 0106  ................
+000018b0: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+000018c0: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+000018d0: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+000018e0: 0106 0106 0106 0106 0106 0106 0106 01    ...............
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/destinations_pb2.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/destinations_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 6043 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 9b17 0000  o.........5d....
+00000000: 610d 0d0a 0000 0000 2038 4164 9b17 0000  a....... 8Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000b 0000 0040 0000 0073 c801 0000 6400  .....@...s....d.
+00000020: 000b 0000 0040 0000 0073 c601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
 00000070: a00c a100 5a0d 6401 6407 6c0e 6d0f 5a10  ....Z.d.d.l.m.Z.
 00000080: 0100 6401 6408 6c11 6d12 5a13 0100 6401  ..d.d.l.m.Z...d.
 00000090: 6409 6c11 6d14 5a15 0100 6505 a00c a100  d.l.m.Z...e.....
@@ -18,202 +18,198 @@
 00000110: 6a20 6601 651c 6410 6411 9c02 a103 651a  j f.e.d.d.....e.
 00000120: 6410 6412 9c03 a103 5a23 650d a022 6523  d.d.....Z#e.."e#
 00000130: a101 0100 650d a022 6523 6a24 a101 0100  ....e.."e#j$....
 00000140: 6509 a01f 640e 6507 6a20 6601 651d 6410  e...d.e.j f.e.d.
 00000150: 6411 9c02 a103 5a25 650d a022 6525 a101  d.....Z%e.."e%..
 00000160: 0100 6509 a01f 640f 6507 6a20 6601 651e  ..e...d.e.j f.e.
 00000170: 6410 6411 9c02 a103 5a26 650d a022 6526  d.d.....Z&e.."e&
-00000180: a101 0100 6503 6a27 6413 6b02 72e2 6414  ....e.j'd.k.r.d.
-00000190: 6517 5f28 6415 6517 5f29 6414 651a 6a2a  e._(d.e._)d.e.j*
-000001a0: 6416 1900 5f28 6417 651a 6a2a 6416 1900  d..._(d.e.j*d...
-000001b0: 5f29 6418 6519 5f2b 6419 6519 5f2c 641a  _)d.e._+d.e._,d.
-000001c0: 651a 5f2b 641b 651a 5f2c 641c 651c 5f2b  e._+d.e._,d.e._+
-000001d0: 641b 651c 5f2c 641d 651d 5f2b 641e 651d  d.e._,d.e._+d.e.
-000001e0: 5f2c 641f 651e 5f2b 6420 651e 5f2c 6414  _,d.e._+d e._,d.
-000001f0: 5300 6414 5300 2921 7a1f 4765 6e65 7261  S.d.S.)!z.Genera
-00000200: 7465 6420 7072 6f74 6f63 6f6c 2062 7566  ted protocol buf
-00000210: 6665 7220 636f 6465 2ee9 0000 0000 2901  fer code......).
-00000220: da0a 6465 7363 7269 7074 6f72 2901 da0f  ..descriptor)...
-00000230: 6465 7363 7269 7074 6f72 5f70 6f6f 6c29  descriptor_pool)
-00000240: 01da 076d 6573 7361 6765 2901 da0a 7265  ...message)...re
-00000250: 666c 6563 7469 6f6e 2901 da0f 7379 6d62  flection)...symb
-00000260: 6f6c 5f64 6174 6162 6173 6529 01da 1266  ol_database)...f
-00000270: 6965 6c64 5f62 6568 6176 696f 725f 7062  ield_behavior_pb
-00000280: 3229 01da 0a63 6f6d 6d6f 6e5f 7062 3229  2)...common_pb2)
-00000290: 01da 0a70 756c 7361 725f 7062 3273 4b05  ...pulsar_pb2sK.
-000002a0: 0000 0a2a 6b61 736b 6164 612f 6b61 736b  ...*kaskada/kask
-000002b0: 6164 612f 7631 616c 7068 612f 6465 7374  ada/v1alpha/dest
-000002c0: 696e 6174 696f 6e73 2e70 726f 746f 1217  inations.proto..
-000002d0: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
-000002e0: 7631 616c 7068 611a 1f67 6f6f 676c 652f  v1alpha..google/
-000002f0: 6170 692f 6669 656c 645f 6265 6861 7669  api/field_behavi
-00000300: 6f72 2e70 726f 746f 1a24 6b61 736b 6164  or.proto.$kaskad
-00000310: 612f 6b61 736b 6164 612f 7631 616c 7068  a/kaskada/v1alph
-00000320: 612f 636f 6d6d 6f6e 2e70 726f 746f 1a24  a/common.proto.$
-00000330: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
-00000340: 7631 616c 7068 612f 7075 6c73 6172 2e70  v1alpha/pulsar.p
-00000350: 726f 746f 22fb 010a 0b44 6573 7469 6e61  roto"....Destina
-00000360: 7469 6f6e 1254 0a0c 6f62 6a65 6374 5f73  tion.T..object_s
-00000370: 746f 7265 1801 2001 280b 322f 2e6b 6173  tore.. .(.2/.kas
-00000380: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-00000390: 6c70 6861 2e4f 626a 6563 7453 746f 7265  lpha.ObjectStore
-000003a0: 4465 7374 696e 6174 696f 6e48 0052 0b6f  DestinationH.R.o
-000003b0: 626a 6563 7453 746f 7265 1241 0a05 7265  bjectStore.A..re
-000003c0: 6469 7318 0220 0128 0b32 292e 6b61 736b  dis.. .(.2).kask
-000003d0: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-000003e0: 7068 612e 5265 6469 7344 6573 7469 6e61  pha.RedisDestina
-000003f0: 7469 6f6e 4800 5205 7265 6469 7312 440a  tionH.R.redis.D.
-00000400: 0670 756c 7361 7218 0320 0128 0b32 2a2e  .pulsar.. .(.2*.
-00000410: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
-00000420: 7631 616c 7068 612e 5075 6c73 6172 4465  v1alpha.PulsarDe
-00000430: 7374 696e 6174 696f 6e48 0052 0670 756c  stinationH.R.pul
-00000440: 7361 7242 0d0a 0b64 6573 7469 6e61 7469  sarB...destinati
-00000450: 6f6e 228e 020a 164f 626a 6563 7453 746f  on"....ObjectSto
-00000460: 7265 4465 7374 696e 6174 696f 6e12 3e0a  reDestination.>.
-00000470: 0966 696c 655f 7479 7065 1801 2001 280e  .file_type.. .(.
-00000480: 3221 2e6b 6173 6b61 6461 2e6b 6173 6b61  2!.kaskada.kaska
-00000490: 6461 2e76 3161 6c70 6861 2e46 696c 6554  da.v1alpha.FileT
-000004a0: 7970 6552 0866 696c 6554 7970 6512 2a0a  ypeR.fileType.*.
-000004b0: 116f 7574 7075 745f 7072 6566 6978 5f75  .output_prefix_u
-000004c0: 7269 1802 2001 2809 520f 6f75 7470 7574  ri.. .(.R.output
-000004d0: 5072 6566 6978 5572 6912 630a 0c6f 7574  PrefixUri.c..out
-000004e0: 7075 745f 7061 7468 7318 0320 0128 0b32  put_paths.. .(.2
-000004f0: 3b2e 6b61 736b 6164 612e 6b61 736b 6164  ;.kaskada.kaskad
-00000500: 612e 7631 616c 7068 612e 4f62 6a65 6374  a.v1alpha.Object
-00000510: 5374 6f72 6544 6573 7469 6e61 7469 6f6e  StoreDestination
-00000520: 2e52 6573 756c 7450 6174 6873 4203 e041  .ResultPathsB..A
-00000530: 0352 0b6f 7574 7075 7450 6174 6873 1a23  .R.outputPaths.#
-00000540: 0a0b 5265 7375 6c74 5061 7468 7312 140a  ..ResultPaths...
-00000550: 0570 6174 6873 1801 2003 2809 5205 7061  .paths.. .(.R.pa
-00000560: 7468 7322 a702 0a10 5265 6469 7344 6573  ths"....RedisDes
-00000570: 7469 6e61 7469 6f6e 121b 0a09 686f 7374  tination....host
-00000580: 5f6e 616d 6518 0120 0128 0952 0868 6f73  _name.. .(.R.hos
-00000590: 744e 616d 6512 120a 0470 6f72 7418 0220  tName....port.. 
-000005a0: 0128 0552 0470 6f72 7412 170a 0775 7365  .(.R.port....use
-000005b0: 5f74 6c73 1803 2001 2808 5206 7573 6554  _tls.. .(.R.useT
-000005c0: 6c73 1227 0a0f 6461 7461 6261 7365 5f6e  ls.'..database_n
-000005d0: 756d 6265 7218 0420 0128 0552 0e64 6174  umber.. .(.R.dat
-000005e0: 6162 6173 654e 756d 6265 7212 1a0a 0870  abaseNumber....p
-000005f0: 6173 7377 6f72 6418 0520 0128 0952 0870  assword.. .(.R.p
-00000600: 6173 7377 6f72 6412 190a 0874 6c73 5f63  assword....tls_c
-00000610: 6572 7418 0620 0128 0952 0774 6c73 4365  ert.. .(.R.tlsCe
-00000620: 7274 1217 0a07 746c 735f 6b65 7918 0720  rt....tls_key.. 
-00000630: 0128 0952 0674 6c73 4b65 7912 1e0a 0b74  .(.R.tlsKey....t
-00000640: 6c73 5f63 615f 6365 7274 1808 2001 2809  ls_ca_cert.. .(.
-00000650: 5209 746c 7343 6143 6572 7412 300a 1469  R.tlsCaCert.0..i
-00000660: 6e73 6563 7572 655f 736b 6970 5f76 6572  nsecure_skip_ver
-00000670: 6966 7918 0920 0128 0852 1269 6e73 6563  ify.. .(.R.insec
-00000680: 7572 6553 6b69 7056 6572 6966 7922 520a  ureSkipVerify"R.
-00000690: 1150 756c 7361 7244 6573 7469 6e61 7469  .PulsarDestinati
-000006a0: 6f6e 123d 0a06 636f 6e66 6967 1801 2001  on.=..config.. .
-000006b0: 280b 3225 2e6b 6173 6b61 6461 2e6b 6173  (.2%.kaskada.kas
-000006c0: 6b61 6461 2e76 3161 6c70 6861 2e50 756c  kada.v1alpha.Pul
-000006d0: 7361 7243 6f6e 6669 6752 0663 6f6e 6669  sarConfigR.confi
-000006e0: 6742 8102 0a1b 636f 6d2e 6b61 736b 6164  gB....com.kaskad
-000006f0: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
-00000700: 6142 1144 6573 7469 6e61 7469 6f6e 7350  aB.DestinationsP
-00000710: 726f 746f 5001 5a51 6769 7468 7562 2e63  rotoP.ZQgithub.c
-00000720: 6f6d 2f6b 6173 6b61 6461 2d61 692f 6b61  om/kaskada-ai/ka
-00000730: 736b 6164 612f 6765 6e2f 7072 6f74 6f2f  skada/gen/proto/
-00000740: 676f 2f6b 6173 6b61 6461 2f6b 6173 6b61  go/kaskada/kaska
-00000750: 6461 2f76 3161 6c70 6861 3b6b 6173 6b61  da/v1alpha;kaska
-00000760: 6461 7631 616c 7068 61a2 0203 4b4b 58aa  dav1alpha...KKX.
-00000770: 0217 4b61 736b 6164 612e 4b61 736b 6164  ..Kaskada.Kaskad
-00000780: 612e 5631 616c 7068 61ca 0217 4b61 736b  a.V1alpha...Kask
-00000790: 6164 615c 4b61 736b 6164 615c 5631 616c  ada\Kaskada\V1al
-000007a0: 7068 61e2 0223 4b61 736b 6164 615c 4b61  pha..#Kaskada\Ka
-000007b0: 736b 6164 615c 5631 616c 7068 615c 4750  skada\V1alpha\GP
-000007c0: 424d 6574 6164 6174 61ea 0219 4b61 736b  BMetadata...Kask
-000007d0: 6164 613a 3a4b 6173 6b61 6461 3a3a 5631  ada::Kaskada::V1
-000007e0: 616c 7068 6162 0670 726f 746f 33da 0b44  alphab.proto3..D
-000007f0: 6573 7469 6e61 7469 6f6e da16 4f62 6a65  estination..Obje
-00000800: 6374 5374 6f72 6544 6573 7469 6e61 7469  ctStoreDestinati
-00000810: 6f6e da0b 5265 7375 6c74 5061 7468 73da  on..ResultPaths.
-00000820: 1052 6564 6973 4465 7374 696e 6174 696f  .RedisDestinatio
-00000830: 6eda 1150 756c 7361 7244 6573 7469 6e61  n..PulsarDestina
-00000840: 7469 6f6e 7a28 6b61 736b 6164 612e 6b61  tionz(kaskada.ka
-00000850: 736b 6164 612e 7631 616c 7068 612e 6465  skada.v1alpha.de
-00000860: 7374 696e 6174 696f 6e73 5f70 6232 2902  stinations_pb2).
-00000870: da0a 4445 5343 5249 5054 4f52 da0a 5f5f  ..DESCRIPTOR..__
-00000880: 6d6f 6475 6c65 5f5f 2903 720c 0000 0072  module__).r....r
-00000890: 0f00 0000 7210 0000 0046 4e73 0101 0000  ....r....FNs....
-000008a0: 0a1b 636f 6d2e 6b61 736b 6164 612e 6b61  ..com.kaskada.ka
-000008b0: 736b 6164 612e 7631 616c 7068 6142 1144  skada.v1alphaB.D
-000008c0: 6573 7469 6e61 7469 6f6e 7350 726f 746f  estinationsProto
-000008d0: 5001 5a51 6769 7468 7562 2e63 6f6d 2f6b  P.ZQgithub.com/k
-000008e0: 6173 6b61 6461 2d61 692f 6b61 736b 6164  askada-ai/kaskad
-000008f0: 612f 6765 6e2f 7072 6f74 6f2f 676f 2f6b  a/gen/proto/go/k
-00000900: 6173 6b61 6461 2f6b 6173 6b61 6461 2f76  askada/kaskada/v
-00000910: 3161 6c70 6861 3b6b 6173 6b61 6461 7631  1alpha;kaskadav1
-00000920: 616c 7068 61a2 0203 4b4b 58aa 0217 4b61  alpha...KKX...Ka
-00000930: 736b 6164 612e 4b61 736b 6164 612e 5631  skada.Kaskada.V1
-00000940: 616c 7068 61ca 0217 4b61 736b 6164 615c  alpha...Kaskada\
-00000950: 4b61 736b 6164 615c 5631 616c 7068 61e2  Kaskada\V1alpha.
-00000960: 0223 4b61 736b 6164 615c 4b61 736b 6164  .#Kaskada\Kaskad
-00000970: 615c 5631 616c 7068 615c 4750 424d 6574  a\V1alpha\GPBMet
-00000980: 6164 6174 61ea 0219 4b61 736b 6164 613a  adata...Kaskada:
-00000990: 3a4b 6173 6b61 6461 3a3a 5631 616c 7068  :Kaskada::V1alph
-000009a0: 61da 0c6f 7574 7075 745f 7061 7468 7373  a..output_pathss
-000009b0: 0300 0000 e041 03e9 b500 0000 69b0 0100  .....A......i...
-000009c0: 0069 b301 0000 69c1 0200 0069 9e02 0000  .i....i....i....
-000009d0: 69c4 0200 0069 eb03 0000 69ed 0300 0069  i....i....i....i
-000009e0: 3f04 0000 292d da07 5f5f 646f 635f 5fda  ?...)-..__doc__.
-000009f0: 0f67 6f6f 676c 652e 7072 6f74 6f62 7566  .google.protobuf
-00000a00: 7202 0000 00da 0b5f 6465 7363 7269 7074  r......_descript
-00000a10: 6f72 7203 0000 00da 105f 6465 7363 7269  orr......_descri
-00000a20: 7074 6f72 5f70 6f6f 6c72 0400 0000 da08  ptor_poolr......
-00000a30: 5f6d 6573 7361 6765 7205 0000 00da 0b5f  _messager......_
-00000a40: 7265 666c 6563 7469 6f6e 7206 0000 00da  reflectionr.....
-00000a50: 105f 7379 6d62 6f6c 5f64 6174 6162 6173  ._symbol_databas
-00000a60: 65da 0744 6566 6175 6c74 da07 5f73 796d  e..Default.._sym
-00000a70: 5f64 62da 0a67 6f6f 676c 652e 6170 6972  _db..google.apir
-00000a80: 0700 0000 da27 676f 6f67 6c65 5f64 6f74  .....'google_dot
-00000a90: 5f61 7069 5f64 6f74 5f66 6965 6c64 5f5f  _api_dot_field__
-00000aa0: 6265 6861 7669 6f72 5f5f 7062 32da 176b  behavior__pb2..k
-00000ab0: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
-00000ac0: 3161 6c70 6861 7208 0000 00da 2f6b 6173  1alphar...../kas
-00000ad0: 6b61 6461 5f64 6f74 5f6b 6173 6b61 6461  kada_dot_kaskada
-00000ae0: 5f64 6f74 5f76 3161 6c70 6861 5f64 6f74  _dot_v1alpha_dot
-00000af0: 5f63 6f6d 6d6f 6e5f 5f70 6232 7209 0000  _common__pb2r...
-00000b00: 00da 2f6b 6173 6b61 6461 5f64 6f74 5f6b  ../kaskada_dot_k
-00000b10: 6173 6b61 6461 5f64 6f74 5f76 3161 6c70  askada_dot_v1alp
-00000b20: 6861 5f64 6f74 5f70 756c 7361 725f 5f70  ha_dot_pulsar__p
-00000b30: 6232 da11 4164 6453 6572 6961 6c69 7a65  b2..AddSerialize
-00000b40: 6446 696c 6572 0f00 0000 da15 6d65 7373  dFiler......mess
-00000b50: 6167 655f 7479 7065 735f 6279 5f6e 616d  age_types_by_nam
-00000b60: 65da 0c5f 4445 5354 494e 4154 494f 4eda  e.._DESTINATION.
-00000b70: 175f 4f42 4a45 4354 5354 4f52 4544 4553  ._OBJECTSTOREDES
-00000b80: 5449 4e41 5449 4f4e da14 6e65 7374 6564  TINATION..nested
-00000b90: 5f74 7970 6573 5f62 795f 6e61 6d65 da23  _types_by_name.#
-00000ba0: 5f4f 424a 4543 5453 544f 5245 4445 5354  _OBJECTSTOREDEST
-00000bb0: 494e 4154 494f 4e5f 5245 5355 4c54 5041  INATION_RESULTPA
-00000bc0: 5448 53da 115f 5245 4449 5344 4553 5449  THS.._REDISDESTI
-00000bd0: 4e41 5449 4f4e da12 5f50 554c 5341 5244  NATION.._PULSARD
-00000be0: 4553 5449 4e41 5449 4f4e da1c 4765 6e65  ESTINATION..Gene
-00000bf0: 7261 7465 6450 726f 746f 636f 6c4d 6573  ratedProtocolMes
-00000c00: 7361 6765 5479 7065 da07 4d65 7373 6167  sageType..Messag
-00000c10: 6572 0a00 0000 da0f 5265 6769 7374 6572  er......Register
-00000c20: 4d65 7373 6167 6572 0b00 0000 720c 0000  Messager....r...
-00000c30: 0072 0d00 0000 720e 0000 00da 125f 5553  .r....r......_US
-00000c40: 455f 435f 4445 5343 5249 5054 4f52 53da  E_C_DESCRIPTORS.
-00000c50: 085f 6f70 7469 6f6e 73da 135f 7365 7269  ._options.._seri
-00000c60: 616c 697a 6564 5f6f 7074 696f 6e73 da0e  alized_options..
-00000c70: 6669 656c 6473 5f62 795f 6e61 6d65 da11  fields_by_name..
-00000c80: 5f73 6572 6961 6c69 7a65 645f 7374 6172  _serialized_star
-00000c90: 74da 0f5f 7365 7269 616c 697a 6564 5f65  t.._serialized_e
-00000ca0: 6e64 a900 7232 0000 0072 3200 0000 fa76  nd..r2...r2....v
-00000cb0: 2f68 6f6d 652f 7468 6572 6170 6f6e 2f52  /home/therapon/R
-00000cc0: 6570 6f73 2f47 6974 4875 622f 4b61 736b  epos/GitHub/Kask
-00000cd0: 6164 6141 492f 6b61 736b 6164 612f 7265  adaAI/kaskada/re
-00000ce0: 6c65 6173 696e 672f 636c 6965 6e74 732f  leasing/clients/
-00000cf0: 7079 7468 6f6e 2f73 7263 2f6b 6173 6b61  python/src/kaska
-00000d00: 6461 2f6b 6173 6b61 6461 2f76 3161 6c70  da/kaskada/v1alp
-00000d10: 6861 2f64 6573 7469 6e61 7469 6f6e 735f  ha/destinations_
-00000d20: 7062 322e 7079 da08 3c6d 6f64 756c 653e  pb2.py..<module>
-00000d30: 0100 0000 7372 0000 0004 030c 010c 010c  ....sr..........
-00000d40: 010c 010c 0108 030c 030c 010c 010e 030a  ................
-00000d50: 040a 010a 010a 010a 010c 0102 0102 0108  ................
-00000d60: fe0a 050c 020c 0202 0102 0106 fe02 0602  ................
-00000d70: 0108 f70a 0c0c 010c 0202 0102 0108 fe0a  ................
-00000d80: 050c 0202 0102 0108 fe0a 050a 0206 0206  ................
-00000d90: 010c 010c 0106 0106 0106 0106 0106 0106  ................
-00000da0: 0106 0106 0106 010a 0104 f1              ...........
+00000180: a101 0100 6503 6a27 6413 6b02 9001 72c2  ....e.j'd.k...r.
+00000190: 6414 6517 5f28 6415 6517 5f29 6414 651a  d.e._(d.e._)d.e.
+000001a0: 6a2a 6416 1900 5f28 6417 651a 6a2a 6416  j*d..._(d.e.j*d.
+000001b0: 1900 5f29 6418 6519 5f2b 6419 6519 5f2c  .._)d.e._+d.e._,
+000001c0: 641a 651a 5f2b 641b 651a 5f2c 641c 651c  d.e._+d.e._,d.e.
+000001d0: 5f2b 641b 651c 5f2c 641d 651d 5f2b 641e  _+d.e._,d.e._+d.
+000001e0: 651d 5f2c 641f 651e 5f2b 6420 651e 5f2c  e._,d.e._+d e._,
+000001f0: 6414 5300 2921 7a1f 4765 6e65 7261 7465  d.S.)!z.Generate
+00000200: 6420 7072 6f74 6f63 6f6c 2062 7566 6665  d protocol buffe
+00000210: 7220 636f 6465 2ee9 0000 0000 2901 da0a  r code......)...
+00000220: 6465 7363 7269 7074 6f72 2901 da0f 6465  descriptor)...de
+00000230: 7363 7269 7074 6f72 5f70 6f6f 6c29 01da  scriptor_pool)..
+00000240: 076d 6573 7361 6765 2901 da0a 7265 666c  .message)...refl
+00000250: 6563 7469 6f6e 2901 da0f 7379 6d62 6f6c  ection)...symbol
+00000260: 5f64 6174 6162 6173 6529 01da 1266 6965  _database)...fie
+00000270: 6c64 5f62 6568 6176 696f 725f 7062 3229  ld_behavior_pb2)
+00000280: 01da 0a63 6f6d 6d6f 6e5f 7062 3229 01da  ...common_pb2)..
+00000290: 0a70 756c 7361 725f 7062 3273 4b05 0000  .pulsar_pb2sK...
+000002a0: 0a2a 6b61 736b 6164 612f 6b61 736b 6164  .*kaskada/kaskad
+000002b0: 612f 7631 616c 7068 612f 6465 7374 696e  a/v1alpha/destin
+000002c0: 6174 696f 6e73 2e70 726f 746f 1217 6b61  ations.proto..ka
+000002d0: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
+000002e0: 616c 7068 611a 1f67 6f6f 676c 652f 6170  alpha..google/ap
+000002f0: 692f 6669 656c 645f 6265 6861 7669 6f72  i/field_behavior
+00000300: 2e70 726f 746f 1a24 6b61 736b 6164 612f  .proto.$kaskada/
+00000310: 6b61 736b 6164 612f 7631 616c 7068 612f  kaskada/v1alpha/
+00000320: 636f 6d6d 6f6e 2e70 726f 746f 1a24 6b61  common.proto.$ka
+00000330: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
+00000340: 616c 7068 612f 7075 6c73 6172 2e70 726f  alpha/pulsar.pro
+00000350: 746f 22fb 010a 0b44 6573 7469 6e61 7469  to"....Destinati
+00000360: 6f6e 1254 0a0c 6f62 6a65 6374 5f73 746f  on.T..object_sto
+00000370: 7265 1801 2001 280b 322f 2e6b 6173 6b61  re.. .(.2/.kaska
+00000380: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
+00000390: 6861 2e4f 626a 6563 7453 746f 7265 4465  ha.ObjectStoreDe
+000003a0: 7374 696e 6174 696f 6e48 0052 0b6f 626a  stinationH.R.obj
+000003b0: 6563 7453 746f 7265 1241 0a05 7265 6469  ectStore.A..redi
+000003c0: 7318 0220 0128 0b32 292e 6b61 736b 6164  s.. .(.2).kaskad
+000003d0: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+000003e0: 612e 5265 6469 7344 6573 7469 6e61 7469  a.RedisDestinati
+000003f0: 6f6e 4800 5205 7265 6469 7312 440a 0670  onH.R.redis.D..p
+00000400: 756c 7361 7218 0320 0128 0b32 2a2e 6b61  ulsar.. .(.2*.ka
+00000410: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
+00000420: 616c 7068 612e 5075 6c73 6172 4465 7374  alpha.PulsarDest
+00000430: 696e 6174 696f 6e48 0052 0670 756c 7361  inationH.R.pulsa
+00000440: 7242 0d0a 0b64 6573 7469 6e61 7469 6f6e  rB...destination
+00000450: 228e 020a 164f 626a 6563 7453 746f 7265  "....ObjectStore
+00000460: 4465 7374 696e 6174 696f 6e12 3e0a 0966  Destination.>..f
+00000470: 696c 655f 7479 7065 1801 2001 280e 3221  ile_type.. .(.2!
+00000480: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00000490: 2e76 3161 6c70 6861 2e46 696c 6554 7970  .v1alpha.FileTyp
+000004a0: 6552 0866 696c 6554 7970 6512 2a0a 116f  eR.fileType.*..o
+000004b0: 7574 7075 745f 7072 6566 6978 5f75 7269  utput_prefix_uri
+000004c0: 1802 2001 2809 520f 6f75 7470 7574 5072  .. .(.R.outputPr
+000004d0: 6566 6978 5572 6912 630a 0c6f 7574 7075  efixUri.c..outpu
+000004e0: 745f 7061 7468 7318 0320 0128 0b32 3b2e  t_paths.. .(.2;.
+000004f0: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000500: 7631 616c 7068 612e 4f62 6a65 6374 5374  v1alpha.ObjectSt
+00000510: 6f72 6544 6573 7469 6e61 7469 6f6e 2e52  oreDestination.R
+00000520: 6573 756c 7450 6174 6873 4203 e041 0352  esultPathsB..A.R
+00000530: 0b6f 7574 7075 7450 6174 6873 1a23 0a0b  .outputPaths.#..
+00000540: 5265 7375 6c74 5061 7468 7312 140a 0570  ResultPaths....p
+00000550: 6174 6873 1801 2003 2809 5205 7061 7468  aths.. .(.R.path
+00000560: 7322 a702 0a10 5265 6469 7344 6573 7469  s"....RedisDesti
+00000570: 6e61 7469 6f6e 121b 0a09 686f 7374 5f6e  nation....host_n
+00000580: 616d 6518 0120 0128 0952 0868 6f73 744e  ame.. .(.R.hostN
+00000590: 616d 6512 120a 0470 6f72 7418 0220 0128  ame....port.. .(
+000005a0: 0552 0470 6f72 7412 170a 0775 7365 5f74  .R.port....use_t
+000005b0: 6c73 1803 2001 2808 5206 7573 6554 6c73  ls.. .(.R.useTls
+000005c0: 1227 0a0f 6461 7461 6261 7365 5f6e 756d  .'..database_num
+000005d0: 6265 7218 0420 0128 0552 0e64 6174 6162  ber.. .(.R.datab
+000005e0: 6173 654e 756d 6265 7212 1a0a 0870 6173  aseNumber....pas
+000005f0: 7377 6f72 6418 0520 0128 0952 0870 6173  sword.. .(.R.pas
+00000600: 7377 6f72 6412 190a 0874 6c73 5f63 6572  sword....tls_cer
+00000610: 7418 0620 0128 0952 0774 6c73 4365 7274  t.. .(.R.tlsCert
+00000620: 1217 0a07 746c 735f 6b65 7918 0720 0128  ....tls_key.. .(
+00000630: 0952 0674 6c73 4b65 7912 1e0a 0b74 6c73  .R.tlsKey....tls
+00000640: 5f63 615f 6365 7274 1808 2001 2809 5209  _ca_cert.. .(.R.
+00000650: 746c 7343 6143 6572 7412 300a 1469 6e73  tlsCaCert.0..ins
+00000660: 6563 7572 655f 736b 6970 5f76 6572 6966  ecure_skip_verif
+00000670: 7918 0920 0128 0852 1269 6e73 6563 7572  y.. .(.R.insecur
+00000680: 6553 6b69 7056 6572 6966 7922 520a 1150  eSkipVerify"R..P
+00000690: 756c 7361 7244 6573 7469 6e61 7469 6f6e  ulsarDestination
+000006a0: 123d 0a06 636f 6e66 6967 1801 2001 280b  .=..config.. .(.
+000006b0: 3225 2e6b 6173 6b61 6461 2e6b 6173 6b61  2%.kaskada.kaska
+000006c0: 6461 2e76 3161 6c70 6861 2e50 756c 7361  da.v1alpha.Pulsa
+000006d0: 7243 6f6e 6669 6752 0663 6f6e 6669 6742  rConfigR.configB
+000006e0: 8102 0a1b 636f 6d2e 6b61 736b 6164 612e  ....com.kaskada.
+000006f0: 6b61 736b 6164 612e 7631 616c 7068 6142  kaskada.v1alphaB
+00000700: 1144 6573 7469 6e61 7469 6f6e 7350 726f  .DestinationsPro
+00000710: 746f 5001 5a51 6769 7468 7562 2e63 6f6d  toP.ZQgithub.com
+00000720: 2f6b 6173 6b61 6461 2d61 692f 6b61 736b  /kaskada-ai/kask
+00000730: 6164 612f 6765 6e2f 7072 6f74 6f2f 676f  ada/gen/proto/go
+00000740: 2f6b 6173 6b61 6461 2f6b 6173 6b61 6461  /kaskada/kaskada
+00000750: 2f76 3161 6c70 6861 3b6b 6173 6b61 6461  /v1alpha;kaskada
+00000760: 7631 616c 7068 61a2 0203 4b4b 58aa 0217  v1alpha...KKX...
+00000770: 4b61 736b 6164 612e 4b61 736b 6164 612e  Kaskada.Kaskada.
+00000780: 5631 616c 7068 61ca 0217 4b61 736b 6164  V1alpha...Kaskad
+00000790: 615c 4b61 736b 6164 615c 5631 616c 7068  a\Kaskada\V1alph
+000007a0: 61e2 0223 4b61 736b 6164 615c 4b61 736b  a..#Kaskada\Kask
+000007b0: 6164 615c 5631 616c 7068 615c 4750 424d  ada\V1alpha\GPBM
+000007c0: 6574 6164 6174 61ea 0219 4b61 736b 6164  etadata...Kaskad
+000007d0: 613a 3a4b 6173 6b61 6461 3a3a 5631 616c  a::Kaskada::V1al
+000007e0: 7068 6162 0670 726f 746f 33da 0b44 6573  phab.proto3..Des
+000007f0: 7469 6e61 7469 6f6e da16 4f62 6a65 6374  tination..Object
+00000800: 5374 6f72 6544 6573 7469 6e61 7469 6f6e  StoreDestination
+00000810: da0b 5265 7375 6c74 5061 7468 73da 1052  ..ResultPaths..R
+00000820: 6564 6973 4465 7374 696e 6174 696f 6eda  edisDestination.
+00000830: 1150 756c 7361 7244 6573 7469 6e61 7469  .PulsarDestinati
+00000840: 6f6e 7a28 6b61 736b 6164 612e 6b61 736b  onz(kaskada.kask
+00000850: 6164 612e 7631 616c 7068 612e 6465 7374  ada.v1alpha.dest
+00000860: 696e 6174 696f 6e73 5f70 6232 2902 da0a  inations_pb2)...
+00000870: 4445 5343 5249 5054 4f52 da0a 5f5f 6d6f  DESCRIPTOR..__mo
+00000880: 6475 6c65 5f5f 2903 720c 0000 0072 0f00  dule__).r....r..
+00000890: 0000 7210 0000 0046 4e73 0101 0000 0a1b  ..r....FNs......
+000008a0: 636f 6d2e 6b61 736b 6164 612e 6b61 736b  com.kaskada.kask
+000008b0: 6164 612e 7631 616c 7068 6142 1144 6573  ada.v1alphaB.Des
+000008c0: 7469 6e61 7469 6f6e 7350 726f 746f 5001  tinationsProtoP.
+000008d0: 5a51 6769 7468 7562 2e63 6f6d 2f6b 6173  ZQgithub.com/kas
+000008e0: 6b61 6461 2d61 692f 6b61 736b 6164 612f  kada-ai/kaskada/
+000008f0: 6765 6e2f 7072 6f74 6f2f 676f 2f6b 6173  gen/proto/go/kas
+00000900: 6b61 6461 2f6b 6173 6b61 6461 2f76 3161  kada/kaskada/v1a
+00000910: 6c70 6861 3b6b 6173 6b61 6461 7631 616c  lpha;kaskadav1al
+00000920: 7068 61a2 0203 4b4b 58aa 0217 4b61 736b  pha...KKX...Kask
+00000930: 6164 612e 4b61 736b 6164 612e 5631 616c  ada.Kaskada.V1al
+00000940: 7068 61ca 0217 4b61 736b 6164 615c 4b61  pha...Kaskada\Ka
+00000950: 736b 6164 615c 5631 616c 7068 61e2 0223  skada\V1alpha..#
+00000960: 4b61 736b 6164 615c 4b61 736b 6164 615c  Kaskada\Kaskada\
+00000970: 5631 616c 7068 615c 4750 424d 6574 6164  V1alpha\GPBMetad
+00000980: 6174 61ea 0219 4b61 736b 6164 613a 3a4b  ata...Kaskada::K
+00000990: 6173 6b61 6461 3a3a 5631 616c 7068 615a  askada::V1alphaZ
+000009a0: 0c6f 7574 7075 745f 7061 7468 7373 0300  .output_pathss..
+000009b0: 0000 e041 03e9 b500 0000 69b0 0100 0069  ...A......i....i
+000009c0: b301 0000 69c1 0200 0069 9e02 0000 69c4  ....i....i....i.
+000009d0: 0200 0069 eb03 0000 69ed 0300 0069 3f04  ...i....i....i?.
+000009e0: 0000 292d da07 5f5f 646f 635f 5fda 0f67  ..)-..__doc__..g
+000009f0: 6f6f 676c 652e 7072 6f74 6f62 7566 7202  oogle.protobufr.
+00000a00: 0000 00da 0b5f 6465 7363 7269 7074 6f72  ....._descriptor
+00000a10: 7203 0000 00da 105f 6465 7363 7269 7074  r......_descript
+00000a20: 6f72 5f70 6f6f 6c72 0400 0000 da08 5f6d  or_poolr......_m
+00000a30: 6573 7361 6765 7205 0000 00da 0b5f 7265  essager......_re
+00000a40: 666c 6563 7469 6f6e 7206 0000 00da 105f  flectionr......_
+00000a50: 7379 6d62 6f6c 5f64 6174 6162 6173 65da  symbol_database.
+00000a60: 0744 6566 6175 6c74 da07 5f73 796d 5f64  .Default.._sym_d
+00000a70: 62da 0a67 6f6f 676c 652e 6170 6972 0700  b..google.apir..
+00000a80: 0000 da27 676f 6f67 6c65 5f64 6f74 5f61  ...'google_dot_a
+00000a90: 7069 5f64 6f74 5f66 6965 6c64 5f5f 6265  pi_dot_field__be
+00000aa0: 6861 7669 6f72 5f5f 7062 32da 176b 6173  havior__pb2..kas
+00000ab0: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
+00000ac0: 6c70 6861 7208 0000 00da 2f6b 6173 6b61  lphar...../kaska
+00000ad0: 6461 5f64 6f74 5f6b 6173 6b61 6461 5f64  da_dot_kaskada_d
+00000ae0: 6f74 5f76 3161 6c70 6861 5f64 6f74 5f63  ot_v1alpha_dot_c
+00000af0: 6f6d 6d6f 6e5f 5f70 6232 7209 0000 00da  ommon__pb2r.....
+00000b00: 2f6b 6173 6b61 6461 5f64 6f74 5f6b 6173  /kaskada_dot_kas
+00000b10: 6b61 6461 5f64 6f74 5f76 3161 6c70 6861  kada_dot_v1alpha
+00000b20: 5f64 6f74 5f70 756c 7361 725f 5f70 6232  _dot_pulsar__pb2
+00000b30: da11 4164 6453 6572 6961 6c69 7a65 6446  ..AddSerializedF
+00000b40: 696c 6572 0f00 0000 da15 6d65 7373 6167  iler......messag
+00000b50: 655f 7479 7065 735f 6279 5f6e 616d 655a  e_types_by_nameZ
+00000b60: 0c5f 4445 5354 494e 4154 494f 4e5a 175f  ._DESTINATIONZ._
+00000b70: 4f42 4a45 4354 5354 4f52 4544 4553 5449  OBJECTSTOREDESTI
+00000b80: 4e41 5449 4f4e da14 6e65 7374 6564 5f74  NATION..nested_t
+00000b90: 7970 6573 5f62 795f 6e61 6d65 5a23 5f4f  ypes_by_nameZ#_O
+00000ba0: 424a 4543 5453 544f 5245 4445 5354 494e  BJECTSTOREDESTIN
+00000bb0: 4154 494f 4e5f 5245 5355 4c54 5041 5448  ATION_RESULTPATH
+00000bc0: 535a 115f 5245 4449 5344 4553 5449 4e41  SZ._REDISDESTINA
+00000bd0: 5449 4f4e 5a12 5f50 554c 5341 5244 4553  TIONZ._PULSARDES
+00000be0: 5449 4e41 5449 4f4e da1c 4765 6e65 7261  TINATION..Genera
+00000bf0: 7465 6450 726f 746f 636f 6c4d 6573 7361  tedProtocolMessa
+00000c00: 6765 5479 7065 da07 4d65 7373 6167 6572  geType..Messager
+00000c10: 0a00 0000 da0f 5265 6769 7374 6572 4d65  ......RegisterMe
+00000c20: 7373 6167 6572 0b00 0000 720c 0000 0072  ssager....r....r
+00000c30: 0d00 0000 720e 0000 00da 125f 5553 455f  ....r......_USE_
+00000c40: 435f 4445 5343 5249 5054 4f52 53da 085f  C_DESCRIPTORS.._
+00000c50: 6f70 7469 6f6e 73da 135f 7365 7269 616c  options.._serial
+00000c60: 697a 6564 5f6f 7074 696f 6e73 da0e 6669  ized_options..fi
+00000c70: 656c 6473 5f62 795f 6e61 6d65 da11 5f73  elds_by_name.._s
+00000c80: 6572 6961 6c69 7a65 645f 7374 6172 74da  erialized_start.
+00000c90: 0f5f 7365 7269 616c 697a 6564 5f65 6e64  ._serialized_end
+00000ca0: a900 722c 0000 0072 2c00 0000 fa34 2f73  ..r,...r,....4/s
+00000cb0: 7263 2f73 7263 2f6b 6173 6b61 6461 2f6b  rc/src/kaskada/k
+00000cc0: 6173 6b61 6461 2f76 3161 6c70 6861 2f64  askada/v1alpha/d
+00000cd0: 6573 7469 6e61 7469 6f6e 735f 7062 322e  estinations_pb2.
+00000ce0: 7079 da08 3c6d 6f64 756c 653e 0400 0000  py..<module>....
+00000cf0: 736e 0000 0004 010c 010c 010c 010c 010c  sn..............
+00000d00: 0308 030c 010c 010c 030e 040a 010a 010a  ................
+00000d10: 010a 010a 010c 0102 0102 fe08 050a 020c  ................
+00000d20: 020c 0102 0102 fe06 0602 0102 f708 0c0a  ................
+00000d30: 010c 020c 0102 0102 fe08 050a 020c 0102  ................
+00000d40: 0102 fe08 050a 020c 0206 0106 010c 010c  ................
+00000d50: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00000d60: 0106 01                                  ...
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/fenl_diagnostics_pb2.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/fenl_diagnostics_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 3526 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,156 +1,152 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 c60d 0000  o.........5d....
+00000000: 610d 0d0a 0000 0000 2038 4164 c60d 0000  a....... 8Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
+00000020: 0007 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a05 0100 6401 6404 6c03  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c03 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c03 6d0a 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c03 6d0c 5a0d 0100 650d a00e a100  d.l.m.Z...e.....
 00000080: 5a0f 6507 a00e a100 a010 6408 a101 5a11  Z.e.......d...Z.
 00000090: 6511 6a12 6409 1900 5a13 6502 a014 6513  e.j.d...Z.e...e.
 000000a0: a101 5a15 6401 5a16 640a 5a17 640b 5a18  ..Z.d.Z.d.Z.d.Z.
 000000b0: 640c 5a19 640d 5a1a 640e 5a1b 6511 6a1c  d.Z.d.Z.d.Z.e.j.
 000000c0: 640f 1900 5a1d 6511 6a1c 6410 1900 5a1e  d...Z.e.j.d...Z.
 000000d0: 650b a01f 640f 6509 6a20 6601 651d 6411  e...d.e.j f.e.d.
 000000e0: 6412 9c02 a103 5a21 650f a022 6521 a101  d.....Z!e.."e!..
 000000f0: 0100 650b a01f 6410 6509 6a20 6601 651e  ..e...d.e.j f.e.
 00000100: 6411 6412 9c02 a103 5a23 650f a022 6523  d.d.....Z#e.."e#
-00000110: a101 0100 6505 6a24 6413 6b02 7292 6414  ....e.j$d.k.r.d.
-00000120: 6511 5f25 6415 6511 5f26 6416 6513 5f27  e._%d.e._&d.e._'
-00000130: 6417 6513 5f28 6418 651d 5f27 6419 651d  d.e._(d.e._'d.e.
-00000140: 5f28 641a 651e 5f27 641b 651e 5f28 6414  _(d.e._'d.e._(d.
-00000150: 5300 6414 5300 291c 7a1f 4765 6e65 7261  S.d.S.).z.Genera
-00000160: 7465 6420 7072 6f74 6f63 6f6c 2062 7566  ted protocol buf
-00000170: 6665 7220 636f 6465 2ee9 0000 0000 2901  fer code......).
-00000180: da11 656e 756d 5f74 7970 655f 7772 6170  ..enum_type_wrap
-00000190: 7065 7229 01da 0a64 6573 6372 6970 746f  per)...descripto
-000001a0: 7229 01da 0f64 6573 6372 6970 746f 725f  r)...descriptor_
-000001b0: 706f 6f6c 2901 da07 6d65 7373 6167 6529  pool)...message)
-000001c0: 01da 0a72 6566 6c65 6374 696f 6e29 01da  ...reflection)..
-000001d0: 0f73 796d 626f 6c5f 6461 7461 6261 7365  .symbol_database
-000001e0: 7306 0300 000a 2e6b 6173 6b61 6461 2f6b  s......kaskada/k
-000001f0: 6173 6b61 6461 2f76 3161 6c70 6861 2f66  askada/v1alpha/f
-00000200: 656e 6c5f 6469 6167 6e6f 7374 6963 732e  enl_diagnostics.
-00000210: 7072 6f74 6f12 176b 6173 6b61 6461 2e6b  proto..kaskada.k
-00000220: 6173 6b61 6461 2e76 3161 6c70 6861 2284  askada.v1alpha".
-00000230: 010a 0f46 656e 6c44 6961 676e 6f73 7469  ...FenlDiagnosti
-00000240: 6373 1252 0a10 6665 6e6c 5f64 6961 676e  cs.R..fenl_diagn
-00000250: 6f73 7469 6373 1801 2003 280b 3227 2e6b  ostics.. .(.2'.k
-00000260: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
-00000270: 3161 6c70 6861 2e46 656e 6c44 6961 676e  1alpha.FenlDiagn
-00000280: 6f73 7469 6352 0f66 656e 6c44 6961 676e  osticR.fenlDiagn
-00000290: 6f73 7469 6373 121d 0a0a 6e75 6d5f 6572  ostics....num_er
-000002a0: 726f 7273 1802 2001 2803 5209 6e75 6d45  rors.. .(.R.numE
-000002b0: 7272 6f72 7322 9b01 0a0e 4665 6e6c 4469  rrors"....FenlDi
-000002c0: 6167 6e6f 7374 6963 123d 0a08 7365 7665  agnostic.=..seve
-000002d0: 7269 7479 1801 2001 280e 3221 2e6b 6173  rity.. .(.2!.kas
-000002e0: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-000002f0: 6c70 6861 2e53 6576 6572 6974 7952 0873  lpha.SeverityR.s
-00000300: 6576 6572 6974 7912 120a 0463 6f64 6518  everity....code.
-00000310: 0220 0128 0952 0463 6f64 6512 180a 076d  . .(.R.code....m
-00000320: 6573 7361 6765 1803 2001 2809 5207 6d65  essage.. .(.R.me
-00000330: 7373 6167 6512 1c0a 0966 6f72 6d61 7474  ssage....formatt
-00000340: 6564 1804 2001 2809 5209 666f 726d 6174  ed.. .(.R.format
-00000350: 7465 642a 8601 0a08 5365 7665 7269 7479  ted*....Severity
-00000360: 1218 0a14 5345 5645 5249 5459 5f55 4e53  ....SEVERITY_UNS
-00000370: 5045 4349 4649 4544 1000 1210 0a0c 5345  PECIFIED......SE
-00000380: 5645 5249 5459 5f42 5547 1001 1212 0a0e  VERITY_BUG......
-00000390: 5345 5645 5249 5459 5f45 5252 4f52 1002  SEVERITY_ERROR..
-000003a0: 1214 0a10 5345 5645 5249 5459 5f57 4152  ....SEVERITY_WAR
-000003b0: 4e49 4e47 1003 1211 0a0d 5345 5645 5249  NING......SEVERI
-000003c0: 5459 5f4e 4f54 4510 0412 110a 0d53 4556  TY_NOTE......SEV
-000003d0: 4552 4954 595f 4845 4c50 1005 4284 020a  ERITY_HELP..B...
-000003e0: 1b63 6f6d 2e6b 6173 6b61 6461 2e6b 6173  .com.kaskada.kas
-000003f0: 6b61 6461 2e76 3161 6c70 6861 4214 4665  kada.v1alphaB.Fe
-00000400: 6e6c 4469 6167 6e6f 7374 6963 7350 726f  nlDiagnosticsPro
-00000410: 746f 5001 5a51 6769 7468 7562 2e63 6f6d  toP.ZQgithub.com
-00000420: 2f6b 6173 6b61 6461 2d61 692f 6b61 736b  /kaskada-ai/kask
-00000430: 6164 612f 6765 6e2f 7072 6f74 6f2f 676f  ada/gen/proto/go
-00000440: 2f6b 6173 6b61 6461 2f6b 6173 6b61 6461  /kaskada/kaskada
-00000450: 2f76 3161 6c70 6861 3b6b 6173 6b61 6461  /v1alpha;kaskada
-00000460: 7631 616c 7068 61a2 0203 4b4b 58aa 0217  v1alpha...KKX...
-00000470: 4b61 736b 6164 612e 4b61 736b 6164 612e  Kaskada.Kaskada.
-00000480: 5631 616c 7068 61ca 0217 4b61 736b 6164  V1alpha...Kaskad
-00000490: 615c 4b61 736b 6164 615c 5631 616c 7068  a\Kaskada\V1alph
-000004a0: 61e2 0223 4b61 736b 6164 615c 4b61 736b  a..#Kaskada\Kask
-000004b0: 6164 615c 5631 616c 7068 615c 4750 424d  ada\V1alpha\GPBM
-000004c0: 6574 6164 6174 61ea 0219 4b61 736b 6164  etadata...Kaskad
-000004d0: 613a 3a4b 6173 6b61 6461 3a3a 5631 616c  a::Kaskada::V1al
-000004e0: 7068 6162 0670 726f 746f 33da 0853 6576  phab.proto3..Sev
-000004f0: 6572 6974 79e9 0100 0000 e902 0000 00e9  erity...........
-00000500: 0300 0000 e904 0000 00e9 0500 0000 da0f  ................
-00000510: 4665 6e6c 4469 6167 6e6f 7374 6963 73da  FenlDiagnostics.
-00000520: 0e46 656e 6c44 6961 676e 6f73 7469 637a  .FenlDiagnosticz
-00000530: 2c6b 6173 6b61 6461 2e6b 6173 6b61 6461  ,kaskada.kaskada
-00000540: 2e76 3161 6c70 6861 2e66 656e 6c5f 6469  .v1alpha.fenl_di
-00000550: 6167 6e6f 7374 6963 735f 7062 3229 02da  agnostics_pb2)..
-00000560: 0a44 4553 4352 4950 544f 52da 0a5f 5f6d  .DESCRIPTOR..__m
-00000570: 6f64 756c 655f 5f46 4e73 0401 0000 0a1b  odule__FNs......
-00000580: 636f 6d2e 6b61 736b 6164 612e 6b61 736b  com.kaskada.kask
-00000590: 6164 612e 7631 616c 7068 6142 1446 656e  ada.v1alphaB.Fen
-000005a0: 6c44 6961 676e 6f73 7469 6373 5072 6f74  lDiagnosticsProt
-000005b0: 6f50 015a 5167 6974 6875 622e 636f 6d2f  oP.ZQgithub.com/
-000005c0: 6b61 736b 6164 612d 6169 2f6b 6173 6b61  kaskada-ai/kaska
-000005d0: 6461 2f67 656e 2f70 726f 746f 2f67 6f2f  da/gen/proto/go/
-000005e0: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
-000005f0: 7631 616c 7068 613b 6b61 736b 6164 6176  v1alpha;kaskadav
-00000600: 3161 6c70 6861 a202 034b 4b58 aa02 174b  1alpha...KKX...K
-00000610: 6173 6b61 6461 2e4b 6173 6b61 6461 2e56  askada.Kaskada.V
-00000620: 3161 6c70 6861 ca02 174b 6173 6b61 6461  1alpha...Kaskada
-00000630: 5c4b 6173 6b61 6461 5c56 3161 6c70 6861  \Kaskada\V1alpha
-00000640: e202 234b 6173 6b61 6461 5c4b 6173 6b61  ..#Kaskada\Kaska
-00000650: 6461 5c56 3161 6c70 6861 5c47 5042 4d65  da\V1alpha\GPBMe
-00000660: 7461 6461 7461 ea02 194b 6173 6b61 6461  tadata...Kaskada
-00000670: 3a3a 4b61 736b 6164 613a 3a56 3161 6c70  ::Kaskada::V1alp
-00000680: 6861 6971 0100 0069 f701 0000 e94c 0000  haiq...i.....L..
-00000690: 00e9 d000 0000 e9d3 0000 0069 6e01 0000  ...........in...
-000006a0: 2929 da07 5f5f 646f 635f 5fda 1867 6f6f  ))..__doc__..goo
-000006b0: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
-000006c0: 6572 6e61 6c72 0200 0000 da0f 676f 6f67  ernalr......goog
-000006d0: 6c65 2e70 726f 746f 6275 6672 0300 0000  le.protobufr....
-000006e0: da0b 5f64 6573 6372 6970 746f 7272 0400  .._descriptorr..
-000006f0: 0000 da10 5f64 6573 6372 6970 746f 725f  ...._descriptor_
-00000700: 706f 6f6c 7205 0000 00da 085f 6d65 7373  poolr......_mess
-00000710: 6167 6572 0600 0000 da0b 5f72 6566 6c65  ager......_refle
-00000720: 6374 696f 6e72 0700 0000 da10 5f73 796d  ctionr......_sym
-00000730: 626f 6c5f 6461 7461 6261 7365 da07 4465  bol_database..De
-00000740: 6661 756c 74da 075f 7379 6d5f 6462 da11  fault.._sym_db..
-00000750: 4164 6453 6572 6961 6c69 7a65 6446 696c  AddSerializedFil
-00000760: 6572 1000 0000 da12 656e 756d 5f74 7970  er......enum_typ
-00000770: 6573 5f62 795f 6e61 6d65 da09 5f53 4556  es_by_name.._SEV
-00000780: 4552 4954 59da 0f45 6e75 6d54 7970 6557  ERITY..EnumTypeW
-00000790: 7261 7070 6572 7208 0000 00da 1453 4556  rapperr......SEV
-000007a0: 4552 4954 595f 554e 5350 4543 4946 4945  ERITY_UNSPECIFIE
-000007b0: 44da 0c53 4556 4552 4954 595f 4255 47da  D..SEVERITY_BUG.
-000007c0: 0e53 4556 4552 4954 595f 4552 524f 52da  .SEVERITY_ERROR.
-000007d0: 1053 4556 4552 4954 595f 5741 524e 494e  .SEVERITY_WARNIN
-000007e0: 47da 0d53 4556 4552 4954 595f 4e4f 5445  G..SEVERITY_NOTE
-000007f0: da0d 5345 5645 5249 5459 5f48 454c 50da  ..SEVERITY_HELP.
-00000800: 156d 6573 7361 6765 5f74 7970 6573 5f62  .message_types_b
-00000810: 795f 6e61 6d65 da10 5f46 454e 4c44 4941  y_name.._FENLDIA
-00000820: 474e 4f53 5449 4353 da0f 5f46 454e 4c44  GNOSTICS.._FENLD
-00000830: 4941 474e 4f53 5449 43da 1c47 656e 6572  IAGNOSTIC..Gener
-00000840: 6174 6564 5072 6f74 6f63 6f6c 4d65 7373  atedProtocolMess
-00000850: 6167 6554 7970 65da 074d 6573 7361 6765  ageType..Message
-00000860: 720e 0000 00da 0f52 6567 6973 7465 724d  r......RegisterM
-00000870: 6573 7361 6765 720f 0000 00da 125f 5553  essager......_US
-00000880: 455f 435f 4445 5343 5249 5054 4f52 53da  E_C_DESCRIPTORS.
-00000890: 085f 6f70 7469 6f6e 73da 135f 7365 7269  ._options.._seri
-000008a0: 616c 697a 6564 5f6f 7074 696f 6e73 da11  alized_options..
-000008b0: 5f73 6572 6961 6c69 7a65 645f 7374 6172  _serialized_star
-000008c0: 74da 0f5f 7365 7269 616c 697a 6564 5f65  t.._serialized_e
-000008d0: 6e64 a900 7234 0000 0072 3400 0000 fa7a  nd..r4...r4....z
-000008e0: 2f68 6f6d 652f 7468 6572 6170 6f6e 2f52  /home/therapon/R
-000008f0: 6570 6f73 2f47 6974 4875 622f 4b61 736b  epos/GitHub/Kask
-00000900: 6164 6141 492f 6b61 736b 6164 612f 7265  adaAI/kaskada/re
-00000910: 6c65 6173 696e 672f 636c 6965 6e74 732f  leasing/clients/
-00000920: 7079 7468 6f6e 2f73 7263 2f6b 6173 6b61  python/src/kaska
-00000930: 6461 2f6b 6173 6b61 6461 2f76 3161 6c70  da/kaskada/v1alp
-00000940: 6861 2f66 656e 6c5f 6469 6167 6e6f 7374  ha/fenl_diagnost
-00000950: 6963 735f 7062 322e 7079 da08 3c6d 6f64  ics_pb2.py..<mod
-00000960: 756c 653e 0100 0000 734e 0000 0004 030c  ule>....sN......
-00000970: 010c 010c 010c 010c 010c 0108 030e 050a  ................
-00000980: 020a 0104 0104 0104 0104 0104 0104 010a  ................
-00000990: 030a 010c 0102 0102 0108 fe0a 050c 0202  ................
-000009a0: 0102 0108 fe0a 050a 0206 0206 0106 0106  ................
-000009b0: 0106 0106 0106 010a 0104 f7              ...........
+00000110: a101 0100 6505 6a24 6413 6b02 9001 7222  ....e.j$d.k...r"
+00000120: 6414 6511 5f25 6415 6511 5f26 6416 6513  d.e._%d.e._&d.e.
+00000130: 5f27 6417 6513 5f28 6418 651d 5f27 6419  _'d.e._(d.e._'d.
+00000140: 651d 5f28 641a 651e 5f27 641b 651e 5f28  e._(d.e._'d.e._(
+00000150: 6414 5300 291c 7a1f 4765 6e65 7261 7465  d.S.).z.Generate
+00000160: 6420 7072 6f74 6f63 6f6c 2062 7566 6665  d protocol buffe
+00000170: 7220 636f 6465 2ee9 0000 0000 2901 da11  r code......)...
+00000180: 656e 756d 5f74 7970 655f 7772 6170 7065  enum_type_wrappe
+00000190: 7229 01da 0a64 6573 6372 6970 746f 7229  r)...descriptor)
+000001a0: 01da 0f64 6573 6372 6970 746f 725f 706f  ...descriptor_po
+000001b0: 6f6c 2901 da07 6d65 7373 6167 6529 01da  ol)...message)..
+000001c0: 0a72 6566 6c65 6374 696f 6e29 01da 0f73  .reflection)...s
+000001d0: 796d 626f 6c5f 6461 7461 6261 7365 7306  ymbol_databases.
+000001e0: 0300 000a 2e6b 6173 6b61 6461 2f6b 6173  .....kaskada/kas
+000001f0: 6b61 6461 2f76 3161 6c70 6861 2f66 656e  kada/v1alpha/fen
+00000200: 6c5f 6469 6167 6e6f 7374 6963 732e 7072  l_diagnostics.pr
+00000210: 6f74 6f12 176b 6173 6b61 6461 2e6b 6173  oto..kaskada.kas
+00000220: 6b61 6461 2e76 3161 6c70 6861 2284 010a  kada.v1alpha"...
+00000230: 0f46 656e 6c44 6961 676e 6f73 7469 6373  .FenlDiagnostics
+00000240: 1252 0a10 6665 6e6c 5f64 6961 676e 6f73  .R..fenl_diagnos
+00000250: 7469 6373 1801 2003 280b 3227 2e6b 6173  tics.. .(.2'.kas
+00000260: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
+00000270: 6c70 6861 2e46 656e 6c44 6961 676e 6f73  lpha.FenlDiagnos
+00000280: 7469 6352 0f66 656e 6c44 6961 676e 6f73  ticR.fenlDiagnos
+00000290: 7469 6373 121d 0a0a 6e75 6d5f 6572 726f  tics....num_erro
+000002a0: 7273 1802 2001 2803 5209 6e75 6d45 7272  rs.. .(.R.numErr
+000002b0: 6f72 7322 9b01 0a0e 4665 6e6c 4469 6167  ors"....FenlDiag
+000002c0: 6e6f 7374 6963 123d 0a08 7365 7665 7269  nostic.=..severi
+000002d0: 7479 1801 2001 280e 3221 2e6b 6173 6b61  ty.. .(.2!.kaska
+000002e0: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
+000002f0: 6861 2e53 6576 6572 6974 7952 0873 6576  ha.SeverityR.sev
+00000300: 6572 6974 7912 120a 0463 6f64 6518 0220  erity....code.. 
+00000310: 0128 0952 0463 6f64 6512 180a 076d 6573  .(.R.code....mes
+00000320: 7361 6765 1803 2001 2809 5207 6d65 7373  sage.. .(.R.mess
+00000330: 6167 6512 1c0a 0966 6f72 6d61 7474 6564  age....formatted
+00000340: 1804 2001 2809 5209 666f 726d 6174 7465  .. .(.R.formatte
+00000350: 642a 8601 0a08 5365 7665 7269 7479 1218  d*....Severity..
+00000360: 0a14 5345 5645 5249 5459 5f55 4e53 5045  ..SEVERITY_UNSPE
+00000370: 4349 4649 4544 1000 1210 0a0c 5345 5645  CIFIED......SEVE
+00000380: 5249 5459 5f42 5547 1001 1212 0a0e 5345  RITY_BUG......SE
+00000390: 5645 5249 5459 5f45 5252 4f52 1002 1214  VERITY_ERROR....
+000003a0: 0a10 5345 5645 5249 5459 5f57 4152 4e49  ..SEVERITY_WARNI
+000003b0: 4e47 1003 1211 0a0d 5345 5645 5249 5459  NG......SEVERITY
+000003c0: 5f4e 4f54 4510 0412 110a 0d53 4556 4552  _NOTE......SEVER
+000003d0: 4954 595f 4845 4c50 1005 4284 020a 1b63  ITY_HELP..B....c
+000003e0: 6f6d 2e6b 6173 6b61 6461 2e6b 6173 6b61  om.kaskada.kaska
+000003f0: 6461 2e76 3161 6c70 6861 4214 4665 6e6c  da.v1alphaB.Fenl
+00000400: 4469 6167 6e6f 7374 6963 7350 726f 746f  DiagnosticsProto
+00000410: 5001 5a51 6769 7468 7562 2e63 6f6d 2f6b  P.ZQgithub.com/k
+00000420: 6173 6b61 6461 2d61 692f 6b61 736b 6164  askada-ai/kaskad
+00000430: 612f 6765 6e2f 7072 6f74 6f2f 676f 2f6b  a/gen/proto/go/k
+00000440: 6173 6b61 6461 2f6b 6173 6b61 6461 2f76  askada/kaskada/v
+00000450: 3161 6c70 6861 3b6b 6173 6b61 6461 7631  1alpha;kaskadav1
+00000460: 616c 7068 61a2 0203 4b4b 58aa 0217 4b61  alpha...KKX...Ka
+00000470: 736b 6164 612e 4b61 736b 6164 612e 5631  skada.Kaskada.V1
+00000480: 616c 7068 61ca 0217 4b61 736b 6164 615c  alpha...Kaskada\
+00000490: 4b61 736b 6164 615c 5631 616c 7068 61e2  Kaskada\V1alpha.
+000004a0: 0223 4b61 736b 6164 615c 4b61 736b 6164  .#Kaskada\Kaskad
+000004b0: 615c 5631 616c 7068 615c 4750 424d 6574  a\V1alpha\GPBMet
+000004c0: 6164 6174 61ea 0219 4b61 736b 6164 613a  adata...Kaskada:
+000004d0: 3a4b 6173 6b61 6461 3a3a 5631 616c 7068  :Kaskada::V1alph
+000004e0: 6162 0670 726f 746f 33da 0853 6576 6572  ab.proto3..Sever
+000004f0: 6974 79e9 0100 0000 e902 0000 00e9 0300  ity.............
+00000500: 0000 e904 0000 00e9 0500 0000 da0f 4665  ..............Fe
+00000510: 6e6c 4469 6167 6e6f 7374 6963 73da 0e46  nlDiagnostics..F
+00000520: 656e 6c44 6961 676e 6f73 7469 637a 2c6b  enlDiagnosticz,k
+00000530: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
+00000540: 3161 6c70 6861 2e66 656e 6c5f 6469 6167  1alpha.fenl_diag
+00000550: 6e6f 7374 6963 735f 7062 3229 02da 0a44  nostics_pb2)...D
+00000560: 4553 4352 4950 544f 52da 0a5f 5f6d 6f64  ESCRIPTOR..__mod
+00000570: 756c 655f 5f46 4e73 0401 0000 0a1b 636f  ule__FNs......co
+00000580: 6d2e 6b61 736b 6164 612e 6b61 736b 6164  m.kaskada.kaskad
+00000590: 612e 7631 616c 7068 6142 1446 656e 6c44  a.v1alphaB.FenlD
+000005a0: 6961 676e 6f73 7469 6373 5072 6f74 6f50  iagnosticsProtoP
+000005b0: 015a 5167 6974 6875 622e 636f 6d2f 6b61  .ZQgithub.com/ka
+000005c0: 736b 6164 612d 6169 2f6b 6173 6b61 6461  skada-ai/kaskada
+000005d0: 2f67 656e 2f70 726f 746f 2f67 6f2f 6b61  /gen/proto/go/ka
+000005e0: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
+000005f0: 616c 7068 613b 6b61 736b 6164 6176 3161  alpha;kaskadav1a
+00000600: 6c70 6861 a202 034b 4b58 aa02 174b 6173  lpha...KKX...Kas
+00000610: 6b61 6461 2e4b 6173 6b61 6461 2e56 3161  kada.Kaskada.V1a
+00000620: 6c70 6861 ca02 174b 6173 6b61 6461 5c4b  lpha...Kaskada\K
+00000630: 6173 6b61 6461 5c56 3161 6c70 6861 e202  askada\V1alpha..
+00000640: 234b 6173 6b61 6461 5c4b 6173 6b61 6461  #Kaskada\Kaskada
+00000650: 5c56 3161 6c70 6861 5c47 5042 4d65 7461  \V1alpha\GPBMeta
+00000660: 6461 7461 ea02 194b 6173 6b61 6461 3a3a  data...Kaskada::
+00000670: 4b61 736b 6164 613a 3a56 3161 6c70 6861  Kaskada::V1alpha
+00000680: 6971 0100 0069 f701 0000 e94c 0000 00e9  iq...i.....L....
+00000690: d000 0000 e9d3 0000 0069 6e01 0000 2929  .........in...))
+000006a0: da07 5f5f 646f 635f 5fda 1867 6f6f 676c  ..__doc__..googl
+000006b0: 652e 7072 6f74 6f62 7566 2e69 6e74 6572  e.protobuf.inter
+000006c0: 6e61 6c72 0200 0000 da0f 676f 6f67 6c65  nalr......google
+000006d0: 2e70 726f 746f 6275 6672 0300 0000 da0b  .protobufr......
+000006e0: 5f64 6573 6372 6970 746f 7272 0400 0000  _descriptorr....
+000006f0: da10 5f64 6573 6372 6970 746f 725f 706f  .._descriptor_po
+00000700: 6f6c 7205 0000 00da 085f 6d65 7373 6167  olr......_messag
+00000710: 6572 0600 0000 da0b 5f72 6566 6c65 6374  er......_reflect
+00000720: 696f 6e72 0700 0000 da10 5f73 796d 626f  ionr......_symbo
+00000730: 6c5f 6461 7461 6261 7365 da07 4465 6661  l_database..Defa
+00000740: 756c 74da 075f 7379 6d5f 6462 da11 4164  ult.._sym_db..Ad
+00000750: 6453 6572 6961 6c69 7a65 6446 696c 6572  dSerializedFiler
+00000760: 1000 0000 da12 656e 756d 5f74 7970 6573  ......enum_types
+00000770: 5f62 795f 6e61 6d65 5a09 5f53 4556 4552  _by_nameZ._SEVER
+00000780: 4954 59da 0f45 6e75 6d54 7970 6557 7261  ITY..EnumTypeWra
+00000790: 7070 6572 7208 0000 005a 1453 4556 4552  pperr....Z.SEVER
+000007a0: 4954 595f 554e 5350 4543 4946 4945 445a  ITY_UNSPECIFIEDZ
+000007b0: 0c53 4556 4552 4954 595f 4255 475a 0e53  .SEVERITY_BUGZ.S
+000007c0: 4556 4552 4954 595f 4552 524f 525a 1053  EVERITY_ERRORZ.S
+000007d0: 4556 4552 4954 595f 5741 524e 494e 475a  EVERITY_WARNINGZ
+000007e0: 0d53 4556 4552 4954 595f 4e4f 5445 5a0d  .SEVERITY_NOTEZ.
+000007f0: 5345 5645 5249 5459 5f48 454c 50da 156d  SEVERITY_HELP..m
+00000800: 6573 7361 6765 5f74 7970 6573 5f62 795f  essage_types_by_
+00000810: 6e61 6d65 5a10 5f46 454e 4c44 4941 474e  nameZ._FENLDIAGN
+00000820: 4f53 5449 4353 5a0f 5f46 454e 4c44 4941  OSTICSZ._FENLDIA
+00000830: 474e 4f53 5449 43da 1c47 656e 6572 6174  GNOSTIC..Generat
+00000840: 6564 5072 6f74 6f63 6f6c 4d65 7373 6167  edProtocolMessag
+00000850: 6554 7970 65da 074d 6573 7361 6765 720e  eType..Messager.
+00000860: 0000 00da 0f52 6567 6973 7465 724d 6573  .....RegisterMes
+00000870: 7361 6765 720f 0000 00da 125f 5553 455f  sager......_USE_
+00000880: 435f 4445 5343 5249 5054 4f52 53da 085f  C_DESCRIPTORS.._
+00000890: 6f70 7469 6f6e 73da 135f 7365 7269 616c  options.._serial
+000008a0: 697a 6564 5f6f 7074 696f 6e73 da11 5f73  ized_options.._s
+000008b0: 6572 6961 6c69 7a65 645f 7374 6172 74da  erialized_start.
+000008c0: 0f5f 7365 7269 616c 697a 6564 5f65 6e64  ._serialized_end
+000008d0: a900 722b 0000 0072 2b00 0000 fa38 2f73  ..r+...r+....8/s
+000008e0: 7263 2f73 7263 2f6b 6173 6b61 6461 2f6b  rc/src/kaskada/k
+000008f0: 6173 6b61 6461 2f76 3161 6c70 6861 2f66  askada/v1alpha/f
+00000900: 656e 6c5f 6469 6167 6e6f 7374 6963 735f  enl_diagnostics_
+00000910: 7062 322e 7079 da08 3c6d 6f64 756c 653e  pb2.py..<module>
+00000920: 0400 0000 734a 0000 0004 010c 010c 010c  ....sJ..........
+00000930: 010c 010c 010c 0308 050e 020a 010a 0104  ................
+00000940: 0104 0104 0104 0104 0104 030a 010a 010c  ................
+00000950: 0102 0102 fe08 050a 020c 0102 0102 fe08  ................
+00000960: 050a 020c 0206 0106 0106 0106 0106 0106  ................
+00000970: 0106 01                                  ...
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/materialization_service_pb2.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/materialization_service_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 15562 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 ca3c 0000  o.........5d.<..
+00000000: 610d 0d0a 0000 0000 2038 4164 ca3c 0000  a....... 8Ad.<..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 b004 0000 6400  .....@...s....d.
+00000020: 0007 0000 0040 0000 0073 ac04 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
 00000070: a00c a100 5a0d 6401 6407 6c0e 6d0f 5a10  ....Z.d.d.l.m.Z.
 00000080: 0100 6401 6408 6c0e 6d11 5a12 0100 6401  ..d.d.l.m.Z...d.
 00000090: 6409 6c01 6d13 5a14 0100 6401 640a 6c15  d.l.m.Z...d.d.l.
@@ -38,16 +38,16 @@
 00000250: 6537 a101 0100 6509 a02d 6417 6507 6a2e  e7....e..-d.e.j.
 00000260: 6601 652a 641a 641b 9c02 a103 5a38 650d  f.e*d.d.....Z8e.
 00000270: a030 6538 a101 0100 6509 a02d 6418 6507  .0e8....e..-d.e.
 00000280: 6a2e 6601 652b 641a 641b 9c02 a103 5a39  j.f.e+d.d.....Z9
 00000290: 650d a030 6539 a101 0100 6509 a02d 6419  e..0e9....e..-d.
 000002a0: 6507 6a2e 6601 652c 641a 641b 9c02 a103  e.j.f.e,d.d.....
 000002b0: 5a3a 650d a030 653a a101 0100 6520 6a3b  Z:e..0e:....e j;
-000002c0: 641c 1900 5a3c 6503 6a3d 641d 6b02 9002  d...Z<e.j=d.k...
-000002d0: 7256 641e 6520 5f3e 641f 6520 5f3f 641e  rVd.e _>d.e _?d.
+000002c0: 641c 1900 5a3c 6503 6a3d 641d 6b02 9004  d...Z<e.j=d.k...
+000002d0: 72a8 641e 6520 5f3e 641f 6520 5f3f 641e  r.d.e _>d.e _?d.
 000002e0: 6522 6a40 6420 1900 5f3e 6421 6522 6a40  e"j@d .._>d!e"j@
 000002f0: 6420 1900 5f3f 641e 6522 6a40 6422 1900  d .._?d.e"j@d"..
 00000300: 5f3e 6421 6522 6a40 6422 1900 5f3f 641e  _>d!e"j@d".._?d.
 00000310: 6524 6a40 6423 1900 5f3e 6424 6524 6a40  e$j@d#.._>d$e$j@
 00000320: 6423 1900 5f3f 641e 6524 6a40 6425 1900  d#.._?d.e$j@d%..
 00000330: 5f3e 6421 6524 6a40 6425 1900 5f3f 641e  _>d!e$j@d%.._?d.
 00000340: 6524 6a40 6426 1900 5f3e 6424 6524 6a40  e$j@d&.._>d$e$j@
@@ -71,411 +71,406 @@
 00000460: 6524 5f42 6439 6524 5f43 643a 6525 5f42  e$_Bd9e$_Cd:e%_B
 00000470: 643b 6525 5f43 643c 6526 5f42 643d 6526  d;e%_Cd<e&_Bd=e&
 00000480: 5f43 643e 6527 5f42 643f 6527 5f43 6440  _Cd>e'_Bd?e'_Cd@
 00000490: 6528 5f42 6441 6528 5f43 6442 6529 5f42  e(_BdAe(_CdBe)_B
 000004a0: 6443 6529 5f43 6444 652a 5f42 6445 652a  dCe)_CdDe*_BdEe*
 000004b0: 5f43 6446 652b 5f42 6447 652b 5f43 6448  _CdFe+_BdGe+_CdH
 000004c0: 652c 5f42 6449 652c 5f43 644a 653c 5f42  e,_BdIe,_CdJe<_B
-000004d0: 644b 653c 5f43 641e 5300 641e 5300 294c  dKe<_Cd.S.d.S.)L
-000004e0: 7a1f 4765 6e65 7261 7465 6420 7072 6f74  z.Generated prot
-000004f0: 6f63 6f6c 2062 7566 6665 7220 636f 6465  ocol buffer code
-00000500: 2ee9 0000 0000 2901 da0a 6465 7363 7269  ......)...descri
-00000510: 7074 6f72 2901 da0f 6465 7363 7269 7074  ptor)...descript
-00000520: 6f72 5f70 6f6f 6c29 01da 076d 6573 7361  or_pool)...messa
-00000530: 6765 2901 da0a 7265 666c 6563 7469 6f6e  ge)...reflection
-00000540: 2901 da0f 7379 6d62 6f6c 5f64 6174 6162  )...symbol_datab
-00000550: 6173 6529 01da 0f61 6e6e 6f74 6174 696f  ase)...annotatio
-00000560: 6e73 5f70 6232 2901 da12 6669 656c 645f  ns_pb2)...field_
-00000570: 6265 6861 7669 6f72 5f70 6232 2901 da0d  behavior_pb2)...
-00000580: 7469 6d65 7374 616d 705f 7062 3229 01da  timestamp_pb2)..
-00000590: 0a63 6f6d 6d6f 6e5f 7062 3229 01da 1064  .common_pb2)...d
-000005a0: 6573 7469 6e61 7469 6f6e 735f 7062 3229  estinations_pb2)
-000005b0: 01da 0a73 6368 656d 615f 7062 3229 01da  ...schema_pb2)..
-000005c0: 0c76 616c 6964 6174 655f 7062 3273 410d  .validate_pb2sA.
-000005d0: 0000 0a35 6b61 736b 6164 612f 6b61 736b  ...5kaskada/kask
-000005e0: 6164 612f 7631 616c 7068 612f 6d61 7465  ada/v1alpha/mate
-000005f0: 7269 616c 697a 6174 696f 6e5f 7365 7276  rialization_serv
-00000600: 6963 652e 7072 6f74 6f12 176b 6173 6b61  ice.proto..kaska
-00000610: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-00000620: 6861 1a1c 676f 6f67 6c65 2f61 7069 2f61  ha..google/api/a
-00000630: 6e6e 6f74 6174 696f 6e73 2e70 726f 746f  nnotations.proto
-00000640: 1a1f 676f 6f67 6c65 2f61 7069 2f66 6965  ..google/api/fie
-00000650: 6c64 5f62 6568 6176 696f 722e 7072 6f74  ld_behavior.prot
-00000660: 6f1a 1f67 6f6f 676c 652f 7072 6f74 6f62  o..google/protob
-00000670: 7566 2f74 696d 6573 7461 6d70 2e70 726f  uf/timestamp.pro
-00000680: 746f 1a24 6b61 736b 6164 612f 6b61 736b  to.$kaskada/kask
-00000690: 6164 612f 7631 616c 7068 612f 636f 6d6d  ada/v1alpha/comm
-000006a0: 6f6e 2e70 726f 746f 1a2a 6b61 736b 6164  on.proto.*kaskad
-000006b0: 612f 6b61 736b 6164 612f 7631 616c 7068  a/kaskada/v1alph
-000006c0: 612f 6465 7374 696e 6174 696f 6e73 2e70  a/destinations.p
-000006d0: 726f 746f 1a24 6b61 736b 6164 612f 6b61  roto.$kaskada/ka
-000006e0: 736b 6164 612f 7631 616c 7068 612f 7363  skada/v1alpha/sc
-000006f0: 6865 6d61 2e70 726f 746f 1a17 7661 6c69  hema.proto..vali
-00000700: 6461 7465 2f76 616c 6964 6174 652e 7072  date/validate.pr
-00000710: 6f74 6f22 500a 0857 6974 6856 6965 7712  oto"P..WithView.
-00000720: 1b0a 046e 616d 6518 0120 0128 0942 07fa  ...name.. .(.B..
-00000730: 4204 7202 1001 5204 6e61 6d65 1227 0a0a  B.r...R.name.'..
-00000740: 6578 7072 6573 7369 6f6e 1802 2001 2809  expression.. .(.
-00000750: 4207 fa42 0472 0210 0152 0a65 7870 7265  B..B.r...R.expre
-00000760: 7373 696f 6e22 440a 0957 6974 6856 6965  ssion"D..WithVie
-00000770: 7773 1237 0a05 7669 6577 7318 0120 0328  ws.7..views.. .(
-00000780: 0b32 212e 6b61 736b 6164 612e 6b61 736b  .2!.kaskada.kask
-00000790: 6164 612e 7631 616c 7068 612e 5769 7468  ada.v1alpha.With
-000007a0: 5669 6577 5205 7669 6577 7322 db04 0a0f  ViewR.views"....
-000007b0: 4d61 7465 7269 616c 697a 6174 696f 6e12  Materialization.
-000007c0: 320a 126d 6174 6572 6961 6c69 7a61 7469  2..materializati
-000007d0: 6f6e 5f69 6418 0120 0128 0942 03e0 4103  on_id.. .(.B..A.
-000007e0: 5211 6d61 7465 7269 616c 697a 6174 696f  R.materializatio
-000007f0: 6e49 6412 3a0a 146d 6174 6572 6961 6c69  nId.:..materiali
-00000800: 7a61 7469 6f6e 5f6e 616d 6518 0220 0128  zation_name.. .(
-00000810: 0942 07fa 4204 7202 1001 5213 6d61 7465  .B..B.r...R.mate
-00000820: 7269 616c 697a 6174 696f 6e4e 616d 6512  rializationName.
-00000830: 400a 0b63 7265 6174 655f 7469 6d65 1803  @..create_time..
-00000840: 2001 280b 321a 2e67 6f6f 676c 652e 7072   .(.2..google.pr
-00000850: 6f74 6f62 7566 2e54 696d 6573 7461 6d70  otobuf.Timestamp
-00000860: 4203 e041 0352 0a63 7265 6174 6554 696d  B..A.R.createTim
-00000870: 6512 1e0a 0a65 7870 7265 7373 696f 6e18  e....expression.
-00000880: 0b20 0128 0952 0a65 7870 7265 7373 696f  . .(.R.expressio
-00000890: 6e12 400a 0a77 6974 685f 7669 6577 7318  n.@..with_views.
-000008a0: 0520 0328 0b32 212e 6b61 736b 6164 612e  . .(.2!.kaskada.
-000008b0: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
-000008c0: 5769 7468 5669 6577 5209 7769 7468 5669  WithViewR.withVi
-000008d0: 6577 7312 460a 0b64 6573 7469 6e61 7469  ews.F..destinati
-000008e0: 6f6e 1806 2001 280b 3224 2e6b 6173 6b61  on.. .(.2$.kaska
-000008f0: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-00000900: 6861 2e44 6573 7469 6e61 7469 6f6e 520b  ha.DestinationR.
-00000910: 6465 7374 696e 6174 696f 6e12 3c0a 0673  destination.<..s
-00000920: 6368 656d 6118 0720 0128 0b32 1f2e 6b61  chema.. .(.2..ka
-00000930: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
-00000940: 616c 7068 612e 5363 6865 6d61 4203 e041  alpha.SchemaB..A
-00000950: 0352 0673 6368 656d 6112 3b0a 0573 6c69  .R.schema.;..sli
-00000960: 6365 1808 2001 280b 3225 2e6b 6173 6b61  ce.. .(.2%.kaska
-00000970: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-00000980: 6861 2e53 6c69 6365 5265 7175 6573 7452  ha.SliceRequestR
-00000990: 0573 6c69 6365 1242 0a08 616e 616c 7973  .slice.B..analys
-000009a0: 6973 1809 2001 280b 3221 2e6b 6173 6b61  is.. .(.2!.kaska
-000009b0: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-000009c0: 6861 2e41 6e61 6c79 7369 7342 03e0 4103  ha.AnalysisB..A.
-000009d0: 5208 616e 616c 7973 6973 1227 0a0d 6461  R.analysis.'..da
-000009e0: 7461 5f74 6f6b 656e 5f69 6418 0a20 0128  ta_token_id.. .(
-000009f0: 0942 03e0 4103 520b 6461 7461 546f 6b65  .B..A.R.dataToke
-00000a00: 6e49 644a 0408 0410 0522 7d0a 1b4c 6973  nIdJ....."}..Lis
-00000a10: 744d 6174 6572 6961 6c69 7a61 7469 6f6e  tMaterialization
-00000a20: 7352 6571 7565 7374 1216 0a06 7365 6172  sRequest....sear
-00000a30: 6368 1801 2001 2809 5206 7365 6172 6368  ch.. .(.R.search
-00000a40: 1227 0a09 7061 6765 5f73 697a 6518 0220  .'..page_size.. 
-00000a50: 0128 0542 0afa 4207 1a05 18e8 0728 0052  .(.B..B......(.R
-00000a60: 0870 6167 6553 697a 6512 1d0a 0a70 6167  .pageSize....pag
-00000a70: 655f 746f 6b65 6e18 0320 0128 0952 0970  e_token.. .(.R.p
-00000a80: 6167 6554 6f6b 656e 22ee 010a 1c4c 6973  ageToken"....Lis
-00000a90: 744d 6174 6572 6961 6c69 7a61 7469 6f6e  tMaterialization
-00000aa0: 7352 6573 706f 6e73 6512 540a 106d 6174  sResponse.T..mat
-00000ab0: 6572 6961 6c69 7a61 7469 6f6e 7318 0120  erializations.. 
-00000ac0: 0328 0b32 282e 6b61 736b 6164 612e 6b61  .(.2(.kaskada.ka
-00000ad0: 736b 6164 612e 7631 616c 7068 612e 4d61  skada.v1alpha.Ma
-00000ae0: 7465 7269 616c 697a 6174 696f 6e52 106d  terializationR.m
-00000af0: 6174 6572 6961 6c69 7a61 7469 6f6e 7312  aterializations.
-00000b00: 260a 0f6e 6578 745f 7061 6765 5f74 6f6b  &..next_page_tok
-00000b10: 656e 1802 2001 2809 520d 6e65 7874 5061  en.. .(.R.nextPa
-00000b20: 6765 546f 6b65 6e12 500a 0f72 6571 7565  geToken.P..reque
-00000b30: 7374 5f64 6574 6169 6c73 1803 2001 280b  st_details.. .(.
-00000b40: 3227 2e6b 6173 6b61 6461 2e6b 6173 6b61  2'.kaskada.kaska
-00000b50: 6461 2e76 3161 6c70 6861 2e52 6571 7565  da.v1alpha.Reque
-00000b60: 7374 4465 7461 696c 7352 0e72 6571 7565  stDetailsR.reque
-00000b70: 7374 4465 7461 696c 7322 570a 1947 6574  stDetails"W..Get
-00000b80: 4d61 7465 7269 616c 697a 6174 696f 6e52  MaterializationR
-00000b90: 6571 7565 7374 123a 0a14 6d61 7465 7269  equest.:..materi
-00000ba0: 616c 697a 6174 696f 6e5f 6e61 6d65 1801  alization_name..
-00000bb0: 2001 2809 4207 fa42 0472 0210 0152 136d   .(.B..B.r...R.m
-00000bc0: 6174 6572 6961 6c69 7a61 7469 6f6e 4e61  aterializationNa
-00000bd0: 6d65 22c2 010a 1a47 6574 4d61 7465 7269  me"....GetMateri
-00000be0: 616c 697a 6174 696f 6e52 6573 706f 6e73  alizationRespons
-00000bf0: 6512 520a 0f6d 6174 6572 6961 6c69 7a61  e.R..materializa
-00000c00: 7469 6f6e 1801 2001 280b 3228 2e6b 6173  tion.. .(.2(.kas
-00000c10: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-00000c20: 6c70 6861 2e4d 6174 6572 6961 6c69 7a61  lpha.Materializa
-00000c30: 7469 6f6e 520f 6d61 7465 7269 616c 697a  tionR.materializ
-00000c40: 6174 696f 6e12 500a 0f72 6571 7565 7374  ation.P..request
-00000c50: 5f64 6574 6169 6c73 1802 2001 280b 3227  _details.. .(.2'
-00000c60: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
-00000c70: 2e76 3161 6c70 6861 2e52 6571 7565 7374  .v1alpha.Request
-00000c80: 4465 7461 696c 7352 0e72 6571 7565 7374  DetailsR.request
-00000c90: 4465 7461 696c 7322 8b01 0a1c 4372 6561  Details"....Crea
-00000ca0: 7465 4d61 7465 7269 616c 697a 6174 696f  teMaterializatio
-00000cb0: 6e52 6571 7565 7374 1252 0a0f 6d61 7465  nRequest.R..mate
-00000cc0: 7269 616c 697a 6174 696f 6e18 0120 0128  rialization.. .(
-00000cd0: 0b32 282e 6b61 736b 6164 612e 6b61 736b  .2(.kaskada.kask
-00000ce0: 6164 612e 7631 616c 7068 612e 4d61 7465  ada.v1alpha.Mate
-00000cf0: 7269 616c 697a 6174 696f 6e52 0f6d 6174  rializationR.mat
-00000d00: 6572 6961 6c69 7a61 7469 6f6e 1217 0a07  erialization....
-00000d10: 6472 795f 7275 6e18 0220 0128 0852 0664  dry_run.. .(.R.d
-00000d20: 7279 5275 6e22 8402 0a1d 4372 6561 7465  ryRun"....Create
-00000d30: 4d61 7465 7269 616c 697a 6174 696f 6e52  MaterializationR
-00000d40: 6573 706f 6e73 6512 520a 0f6d 6174 6572  esponse.R..mater
-00000d50: 6961 6c69 7a61 7469 6f6e 1801 2001 280b  ialization.. .(.
-00000d60: 3228 2e6b 6173 6b61 6461 2e6b 6173 6b61  2(.kaskada.kaska
-00000d70: 6461 2e76 3161 6c70 6861 2e4d 6174 6572  da.v1alpha.Mater
-00000d80: 6961 6c69 7a61 7469 6f6e 520f 6d61 7465  ializationR.mate
-00000d90: 7269 616c 697a 6174 696f 6e12 500a 0f72  rialization.P..r
-00000da0: 6571 7565 7374 5f64 6574 6169 6c73 1802  equest_details..
-00000db0: 2001 280b 3227 2e6b 6173 6b61 6461 2e6b   .(.2'.kaskada.k
-00000dc0: 6173 6b61 6461 2e76 3161 6c70 6861 2e52  askada.v1alpha.R
-00000dd0: 6571 7565 7374 4465 7461 696c 7352 0e72  equestDetailsR.r
-00000de0: 6571 7565 7374 4465 7461 696c 7312 3d0a  equestDetails.=.
-00000df0: 0861 6e61 6c79 7369 7318 0320 0128 0b32  .analysis.. .(.2
-00000e00: 212e 6b61 736b 6164 612e 6b61 736b 6164  !.kaskada.kaskad
-00000e10: 612e 7631 616c 7068 612e 416e 616c 7973  a.v1alpha.Analys
-00000e20: 6973 5208 616e 616c 7973 6973 225a 0a1c  isR.analysis"Z..
-00000e30: 4465 6c65 7465 4d61 7465 7269 616c 697a  DeleteMaterializ
-00000e40: 6174 696f 6e52 6571 7565 7374 123a 0a14  ationRequest.:..
-00000e50: 6d61 7465 7269 616c 697a 6174 696f 6e5f  materialization_
-00000e60: 6e61 6d65 1801 2001 2809 4207 fa42 0472  name.. .(.B..B.r
-00000e70: 0210 0152 136d 6174 6572 6961 6c69 7a61  ...R.materializa
-00000e80: 7469 6f6e 4e61 6d65 2271 0a1d 4465 6c65  tionName"q..Dele
-00000e90: 7465 4d61 7465 7269 616c 697a 6174 696f  teMaterializatio
-00000ea0: 6e52 6573 706f 6e73 6512 500a 0f72 6571  nResponse.P..req
-00000eb0: 7565 7374 5f64 6574 6169 6c73 1801 2001  uest_details.. .
-00000ec0: 280b 3227 2e6b 6173 6b61 6461 2e6b 6173  (.2'.kaskada.kas
-00000ed0: 6b61 6461 2e76 3161 6c70 6861 2e52 6571  kada.v1alpha.Req
-00000ee0: 7565 7374 4465 7461 696c 7352 0e72 6571  uestDetailsR.req
-00000ef0: 7565 7374 4465 7461 696c 7332 ff05 0a16  uestDetails2....
-00000f00: 4d61 7465 7269 616c 697a 6174 696f 6e53  MaterializationS
-00000f10: 6572 7669 6365 12a6 010a 144c 6973 744d  ervice.....ListM
-00000f20: 6174 6572 6961 6c69 7a61 7469 6f6e 7312  aterializations.
-00000f30: 342e 6b61 736b 6164 612e 6b61 736b 6164  4.kaskada.kaskad
-00000f40: 612e 7631 616c 7068 612e 4c69 7374 4d61  a.v1alpha.ListMa
-00000f50: 7465 7269 616c 697a 6174 696f 6e73 5265  terializationsRe
-00000f60: 7175 6573 741a 352e 6b61 736b 6164 612e  quest.5.kaskada.
-00000f70: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
-00000f80: 4c69 7374 4d61 7465 7269 616c 697a 6174  ListMaterializat
-00000f90: 696f 6e73 5265 7370 6f6e 7365 2221 82d3  ionsResponse"!..
-00000fa0: e493 021b 1219 2f76 3161 6c70 6861 2f6d  ....../v1alpha/m
-00000fb0: 6174 6572 6961 6c69 7a61 7469 6f6e 7312  aterializations.
-00000fc0: b901 0a12 4765 744d 6174 6572 6961 6c69  ....GetMateriali
-00000fd0: 7a61 7469 6f6e 1232 2e6b 6173 6b61 6461  zation.2.kaskada
-00000fe0: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
-00000ff0: 2e47 6574 4d61 7465 7269 616c 697a 6174  .GetMaterializat
-00001000: 696f 6e52 6571 7565 7374 1a33 2e6b 6173  ionRequest.3.kas
-00001010: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-00001020: 6c70 6861 2e47 6574 4d61 7465 7269 616c  lpha.GetMaterial
-00001030: 697a 6174 696f 6e52 6573 706f 6e73 6522  izationResponse"
-00001040: 3a82 d3e4 9302 3412 322f 7631 616c 7068  :.....4.2/v1alph
-00001050: 612f 6d61 7465 7269 616c 697a 6174 696f  a/materializatio
-00001060: 6e73 2f7b 6d61 7465 7269 616c 697a 6174  ns/{materializat
-00001070: 696f 6e5f 6e61 6d65 3d2a 7d12 ba01 0a15  ion_name=*}.....
-00001080: 4372 6561 7465 4d61 7465 7269 616c 697a  CreateMaterializ
-00001090: 6174 696f 6e12 352e 6b61 736b 6164 612e  ation.5.kaskada.
-000010a0: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
-000010b0: 4372 6561 7465 4d61 7465 7269 616c 697a  CreateMaterializ
-000010c0: 6174 696f 6e52 6571 7565 7374 1a36 2e6b  ationRequest.6.k
-000010d0: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
-000010e0: 3161 6c70 6861 2e43 7265 6174 654d 6174  1alpha.CreateMat
-000010f0: 6572 6961 6c69 7a61 7469 6f6e 5265 7370  erializationResp
-00001100: 6f6e 7365 2232 82d3 e493 022c 3a0f 6d61  onse"2.....,:.ma
-00001110: 7465 7269 616c 697a 6174 696f 6e22 192f  terialization"./
-00001120: 7631 616c 7068 612f 6d61 7465 7269 616c  v1alpha/material
-00001130: 697a 6174 696f 6e73 12c2 010a 1544 656c  izations.....Del
-00001140: 6574 654d 6174 6572 6961 6c69 7a61 7469  eteMaterializati
-00001150: 6f6e 1235 2e6b 6173 6b61 6461 2e6b 6173  on.5.kaskada.kas
-00001160: 6b61 6461 2e76 3161 6c70 6861 2e44 656c  kada.v1alpha.Del
-00001170: 6574 654d 6174 6572 6961 6c69 7a61 7469  eteMaterializati
-00001180: 6f6e 5265 7175 6573 741a 362e 6b61 736b  onRequest.6.kask
-00001190: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-000011a0: 7068 612e 4465 6c65 7465 4d61 7465 7269  pha.DeleteMateri
-000011b0: 616c 697a 6174 696f 6e52 6573 706f 6e73  alizationRespons
-000011c0: 6522 3a82 d3e4 9302 342a 322f 7631 616c  e":.....4*2/v1al
-000011d0: 7068 612f 6d61 7465 7269 616c 697a 6174  pha/materializat
-000011e0: 696f 6e73 2f7b 6d61 7465 7269 616c 697a  ions/{materializ
-000011f0: 6174 696f 6e5f 6e61 6d65 3d2a 7d42 8b02  ation_name=*}B..
-00001200: 0a1b 636f 6d2e 6b61 736b 6164 612e 6b61  ..com.kaskada.ka
-00001210: 736b 6164 612e 7631 616c 7068 6142 1b4d  skada.v1alphaB.M
-00001220: 6174 6572 6961 6c69 7a61 7469 6f6e 5365  aterializationSe
-00001230: 7276 6963 6550 726f 746f 5001 5a51 6769  rviceProtoP.ZQgi
-00001240: 7468 7562 2e63 6f6d 2f6b 6173 6b61 6461  thub.com/kaskada
-00001250: 2d61 692f 6b61 736b 6164 612f 6765 6e2f  -ai/kaskada/gen/
-00001260: 7072 6f74 6f2f 676f 2f6b 6173 6b61 6461  proto/go/kaskada
-00001270: 2f6b 6173 6b61 6461 2f76 3161 6c70 6861  /kaskada/v1alpha
-00001280: 3b6b 6173 6b61 6461 7631 616c 7068 61a2  ;kaskadav1alpha.
-00001290: 0203 4b4b 58aa 0217 4b61 736b 6164 612e  ..KKX...Kaskada.
-000012a0: 4b61 736b 6164 612e 5631 616c 7068 61ca  Kaskada.V1alpha.
-000012b0: 0217 4b61 736b 6164 615c 4b61 736b 6164  ..Kaskada\Kaskad
-000012c0: 615c 5631 616c 7068 61e2 0223 4b61 736b  a\V1alpha..#Kask
-000012d0: 6164 615c 4b61 736b 6164 615c 5631 616c  ada\Kaskada\V1al
-000012e0: 7068 615c 4750 424d 6574 6164 6174 61ea  pha\GPBMetadata.
-000012f0: 0219 4b61 736b 6164 613a 3a4b 6173 6b61  ..Kaskada::Kaska
-00001300: 6461 3a3a 5631 616c 7068 6162 0670 726f  da::V1alphab.pro
-00001310: 746f 33da 0857 6974 6856 6965 77da 0957  to3..WithView..W
-00001320: 6974 6856 6965 7773 da0f 4d61 7465 7269  ithViews..Materi
-00001330: 616c 697a 6174 696f 6eda 1b4c 6973 744d  alization..ListM
-00001340: 6174 6572 6961 6c69 7a61 7469 6f6e 7352  aterializationsR
-00001350: 6571 7565 7374 da1c 4c69 7374 4d61 7465  equest..ListMate
-00001360: 7269 616c 697a 6174 696f 6e73 5265 7370  rializationsResp
-00001370: 6f6e 7365 da19 4765 744d 6174 6572 6961  onse..GetMateria
-00001380: 6c69 7a61 7469 6f6e 5265 7175 6573 74da  lizationRequest.
-00001390: 1a47 6574 4d61 7465 7269 616c 697a 6174  .GetMaterializat
-000013a0: 696f 6e52 6573 706f 6e73 65da 1c43 7265  ionResponse..Cre
-000013b0: 6174 654d 6174 6572 6961 6c69 7a61 7469  ateMaterializati
-000013c0: 6f6e 5265 7175 6573 74da 1d43 7265 6174  onRequest..Creat
-000013d0: 654d 6174 6572 6961 6c69 7a61 7469 6f6e  eMaterialization
-000013e0: 5265 7370 6f6e 7365 da1c 4465 6c65 7465  Response..Delete
-000013f0: 4d61 7465 7269 616c 697a 6174 696f 6e52  MaterializationR
-00001400: 6571 7565 7374 da1d 4465 6c65 7465 4d61  equest..DeleteMa
-00001410: 7465 7269 616c 697a 6174 696f 6e52 6573  terializationRes
-00001420: 706f 6e73 657a 336b 6173 6b61 6461 2e6b  ponsez3kaskada.k
-00001430: 6173 6b61 6461 2e76 3161 6c70 6861 2e6d  askada.v1alpha.m
-00001440: 6174 6572 6961 6c69 7a61 7469 6f6e 5f73  aterialization_s
-00001450: 6572 7669 6365 5f70 6232 2902 da0a 4445  ervice_pb2)...DE
-00001460: 5343 5249 5054 4f52 da0a 5f5f 6d6f 6475  SCRIPTOR..__modu
-00001470: 6c65 5f5f da16 4d61 7465 7269 616c 697a  le__..Materializ
-00001480: 6174 696f 6e53 6572 7669 6365 464e 730b  ationServiceFNs.
-00001490: 0100 000a 1b63 6f6d 2e6b 6173 6b61 6461  .....com.kaskada
-000014a0: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
-000014b0: 421b 4d61 7465 7269 616c 697a 6174 696f  B.Materializatio
-000014c0: 6e53 6572 7669 6365 5072 6f74 6f50 015a  nServiceProtoP.Z
-000014d0: 5167 6974 6875 622e 636f 6d2f 6b61 736b  Qgithub.com/kask
-000014e0: 6164 612d 6169 2f6b 6173 6b61 6461 2f67  ada-ai/kaskada/g
-000014f0: 656e 2f70 726f 746f 2f67 6f2f 6b61 736b  en/proto/go/kask
-00001500: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
-00001510: 7068 613b 6b61 736b 6164 6176 3161 6c70  pha;kaskadav1alp
-00001520: 6861 a202 034b 4b58 aa02 174b 6173 6b61  ha...KKX...Kaska
-00001530: 6461 2e4b 6173 6b61 6461 2e56 3161 6c70  da.Kaskada.V1alp
-00001540: 6861 ca02 174b 6173 6b61 6461 5c4b 6173  ha...Kaskada\Kas
-00001550: 6b61 6461 5c56 3161 6c70 6861 e202 234b  kada\V1alpha..#K
-00001560: 6173 6b61 6461 5c4b 6173 6b61 6461 5c56  askada\Kaskada\V
-00001570: 3161 6c70 6861 5c47 5042 4d65 7461 6461  1alpha\GPBMetada
-00001580: 7461 ea02 194b 6173 6b61 6461 3a3a 4b61  ta...Kaskada::Ka
-00001590: 736b 6164 613a 3a56 3161 6c70 6861 da04  skada::V1alpha..
-000015a0: 6e61 6d65 7307 0000 00fa 4204 7202 1001  names.....B.r...
-000015b0: da0a 6578 7072 6573 7369 6f6e da12 6d61  ..expression..ma
-000015c0: 7465 7269 616c 697a 6174 696f 6e5f 6964  terialization_id
-000015d0: 7303 0000 00e0 4103 da14 6d61 7465 7269  s.....A...materi
-000015e0: 616c 697a 6174 696f 6e5f 6e61 6d65 da0b  alization_name..
-000015f0: 6372 6561 7465 5f74 696d 65da 0673 6368  create_time..sch
-00001600: 656d 61da 0861 6e61 6c79 7369 73da 0d64  ema..analysis..d
-00001610: 6174 615f 746f 6b65 6e5f 6964 da09 7061  ata_token_id..pa
-00001620: 6765 5f73 697a 6573 0a00 0000 fa42 071a  ge_sizes.....B..
-00001630: 0518 e807 2800 da14 4c69 7374 4d61 7465  ....(...ListMate
-00001640: 7269 616c 697a 6174 696f 6e73 7321 0000  rializationss!..
-00001650: 0082 d3e4 9302 1b12 192f 7631 616c 7068  ........./v1alph
-00001660: 612f 6d61 7465 7269 616c 697a 6174 696f  a/materializatio
-00001670: 6e73 da12 4765 744d 6174 6572 6961 6c69  ns..GetMateriali
-00001680: 7a61 7469 6f6e 733a 0000 0082 d3e4 9302  zations:........
-00001690: 3412 322f 7631 616c 7068 612f 6d61 7465  4.2/v1alpha/mate
-000016a0: 7269 616c 697a 6174 696f 6e73 2f7b 6d61  rializations/{ma
-000016b0: 7465 7269 616c 697a 6174 696f 6e5f 6e61  terialization_na
-000016c0: 6d65 3d2a 7dda 1543 7265 6174 654d 6174  me=*}..CreateMat
-000016d0: 6572 6961 6c69 7a61 7469 6f6e 7332 0000  erializations2..
-000016e0: 0082 d3e4 9302 2c3a 0f6d 6174 6572 6961  ......,:.materia
-000016f0: 6c69 7a61 7469 6f6e 2219 2f76 3161 6c70  lization"./v1alp
-00001700: 6861 2f6d 6174 6572 6961 6c69 7a61 7469  ha/materializati
-00001710: 6f6e 73da 1544 656c 6574 654d 6174 6572  ons..DeleteMater
-00001720: 6961 6c69 7a61 7469 6f6e 733a 0000 0082  ializations:....
-00001730: d3e4 9302 342a 322f 7631 616c 7068 612f  ....4*2/v1alpha/
-00001740: 6d61 7465 7269 616c 697a 6174 696f 6e73  materializations
-00001750: 2f7b 6d61 7465 7269 616c 697a 6174 696f  /{materializatio
-00001760: 6e5f 6e61 6d65 3d2a 7d69 4301 0000 6993  n_name=*}iC...i.
-00001770: 0100 0069 9501 0000 69d9 0100 0069 dc01  ...i....i....i..
-00001780: 0000 6937 0400 0069 3904 0000 69b6 0400  ..i7...i9...i...
-00001790: 0069 b904 0000 69a7 0500 0069 a905 0000  .i....i....i....
-000017a0: 6900 0600 0069 0306 0000 69c5 0600 0069  i....i....i....i
-000017b0: c806 0000 6953 0700 0069 5607 0000 695a  ....iS...iV...iZ
-000017c0: 0800 0069 5c08 0000 69b6 0800 0069 b808  ...i\...i....i..
-000017d0: 0000 6929 0900 0069 2c09 0000 692b 0c00  ..i)...i,...i+..
-000017e0: 0029 44da 075f 5f64 6f63 5f5f da0f 676f  .)D..__doc__..go
-000017f0: 6f67 6c65 2e70 726f 746f 6275 6672 0200  ogle.protobufr..
-00001800: 0000 da0b 5f64 6573 6372 6970 746f 7272  ...._descriptorr
-00001810: 0300 0000 da10 5f64 6573 6372 6970 746f  ......_descripto
-00001820: 725f 706f 6f6c 7204 0000 00da 085f 6d65  r_poolr......_me
-00001830: 7373 6167 6572 0500 0000 da0b 5f72 6566  ssager......_ref
-00001840: 6c65 6374 696f 6e72 0600 0000 da10 5f73  lectionr......_s
-00001850: 796d 626f 6c5f 6461 7461 6261 7365 da07  ymbol_database..
-00001860: 4465 6661 756c 74da 075f 7379 6d5f 6462  Default.._sym_db
-00001870: da0a 676f 6f67 6c65 2e61 7069 7207 0000  ..google.apir...
-00001880: 00da 2367 6f6f 676c 655f 646f 745f 6170  ..#google_dot_ap
-00001890: 695f 646f 745f 616e 6e6f 7461 7469 6f6e  i_dot_annotation
-000018a0: 735f 5f70 6232 7208 0000 00da 2767 6f6f  s__pb2r.....'goo
-000018b0: 676c 655f 646f 745f 6170 695f 646f 745f  gle_dot_api_dot_
-000018c0: 6669 656c 645f 5f62 6568 6176 696f 725f  field__behavior_
-000018d0: 5f70 6232 7209 0000 00da 2667 6f6f 676c  _pb2r.....&googl
-000018e0: 655f 646f 745f 7072 6f74 6f62 7566 5f64  e_dot_protobuf_d
-000018f0: 6f74 5f74 696d 6573 7461 6d70 5f5f 7062  ot_timestamp__pb
-00001900: 32da 176b 6173 6b61 6461 2e6b 6173 6b61  2..kaskada.kaska
-00001910: 6461 2e76 3161 6c70 6861 720a 0000 00da  da.v1alphar.....
-00001920: 2f6b 6173 6b61 6461 5f64 6f74 5f6b 6173  /kaskada_dot_kas
-00001930: 6b61 6461 5f64 6f74 5f76 3161 6c70 6861  kada_dot_v1alpha
-00001940: 5f64 6f74 5f63 6f6d 6d6f 6e5f 5f70 6232  _dot_common__pb2
-00001950: 720b 0000 00da 356b 6173 6b61 6461 5f64  r.....5kaskada_d
-00001960: 6f74 5f6b 6173 6b61 6461 5f64 6f74 5f76  ot_kaskada_dot_v
-00001970: 3161 6c70 6861 5f64 6f74 5f64 6573 7469  1alpha_dot_desti
-00001980: 6e61 7469 6f6e 735f 5f70 6232 720c 0000  nations__pb2r...
-00001990: 00da 2f6b 6173 6b61 6461 5f64 6f74 5f6b  ../kaskada_dot_k
-000019a0: 6173 6b61 6461 5f64 6f74 5f76 3161 6c70  askada_dot_v1alp
-000019b0: 6861 5f64 6f74 5f73 6368 656d 615f 5f70  ha_dot_schema__p
-000019c0: 6232 da08 7661 6c69 6461 7465 720d 0000  b2..validater...
-000019d0: 00da 1a76 616c 6964 6174 655f 646f 745f  ...validate_dot_
-000019e0: 7661 6c69 6461 7465 5f5f 7062 32da 1141  validate__pb2..A
-000019f0: 6464 5365 7269 616c 697a 6564 4669 6c65  ddSerializedFile
-00001a00: 7219 0000 00da 156d 6573 7361 6765 5f74  r......message_t
-00001a10: 7970 6573 5f62 795f 6e61 6d65 da09 5f57  ypes_by_name.._W
-00001a20: 4954 4856 4945 57da 0a5f 5749 5448 5649  ITHVIEW.._WITHVI
-00001a30: 4557 53da 105f 4d41 5445 5249 414c 495a  EWS.._MATERIALIZ
-00001a40: 4154 494f 4eda 1c5f 4c49 5354 4d41 5445  ATION.._LISTMATE
-00001a50: 5249 414c 495a 4154 494f 4e53 5245 5155  RIALIZATIONSREQU
-00001a60: 4553 54da 1d5f 4c49 5354 4d41 5445 5249  EST.._LISTMATERI
-00001a70: 414c 495a 4154 494f 4e53 5245 5350 4f4e  ALIZATIONSRESPON
-00001a80: 5345 da1a 5f47 4554 4d41 5445 5249 414c  SE.._GETMATERIAL
-00001a90: 495a 4154 494f 4e52 4551 5545 5354 da1b  IZATIONREQUEST..
-00001aa0: 5f47 4554 4d41 5445 5249 414c 495a 4154  _GETMATERIALIZAT
-00001ab0: 494f 4e52 4553 504f 4e53 45da 1d5f 4352  IONRESPONSE.._CR
-00001ac0: 4541 5445 4d41 5445 5249 414c 495a 4154  EATEMATERIALIZAT
-00001ad0: 494f 4e52 4551 5545 5354 da1e 5f43 5245  IONREQUEST.._CRE
-00001ae0: 4154 454d 4154 4552 4941 4c49 5a41 5449  ATEMATERIALIZATI
-00001af0: 4f4e 5245 5350 4f4e 5345 da1d 5f44 454c  ONRESPONSE.._DEL
-00001b00: 4554 454d 4154 4552 4941 4c49 5a41 5449  ETEMATERIALIZATI
-00001b10: 4f4e 5245 5155 4553 54da 1e5f 4445 4c45  ONREQUEST.._DELE
-00001b20: 5445 4d41 5445 5249 414c 495a 4154 494f  TEMATERIALIZATIO
-00001b30: 4e52 4553 504f 4e53 45da 1c47 656e 6572  NRESPONSE..Gener
-00001b40: 6174 6564 5072 6f74 6f63 6f6c 4d65 7373  atedProtocolMess
-00001b50: 6167 6554 7970 65da 074d 6573 7361 6765  ageType..Message
-00001b60: 720e 0000 00da 0f52 6567 6973 7465 724d  r......RegisterM
-00001b70: 6573 7361 6765 720f 0000 0072 1000 0000  essager....r....
-00001b80: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00001b90: 1400 0000 7215 0000 0072 1600 0000 7217  ....r....r....r.
-00001ba0: 0000 0072 1800 0000 da10 7365 7276 6963  ...r......servic
-00001bb0: 6573 5f62 795f 6e61 6d65 da17 5f4d 4154  es_by_name.._MAT
-00001bc0: 4552 4941 4c49 5a41 5449 4f4e 5345 5256  ERIALIZATIONSERV
-00001bd0: 4943 45da 125f 5553 455f 435f 4445 5343  ICE.._USE_C_DESC
-00001be0: 5249 5054 4f52 53da 085f 6f70 7469 6f6e  RIPTORS.._option
-00001bf0: 73da 135f 7365 7269 616c 697a 6564 5f6f  s.._serialized_o
-00001c00: 7074 696f 6e73 da0e 6669 656c 6473 5f62  ptions..fields_b
-00001c10: 795f 6e61 6d65 da0f 6d65 7468 6f64 735f  y_name..methods_
-00001c20: 6279 5f6e 616d 65da 115f 7365 7269 616c  by_name.._serial
-00001c30: 697a 6564 5f73 7461 7274 da0f 5f73 6572  ized_start.._ser
-00001c40: 6961 6c69 7a65 645f 656e 64a9 0072 5500  ialized_end..rU.
-00001c50: 0000 7255 0000 00fa 812f 686f 6d65 2f74  ..rU...../home/t
-00001c60: 6865 7261 706f 6e2f 5265 706f 732f 4769  herapon/Repos/Gi
-00001c70: 7448 7562 2f4b 6173 6b61 6461 4149 2f6b  tHub/KaskadaAI/k
-00001c80: 6173 6b61 6461 2f72 656c 6561 7369 6e67  askada/releasing
-00001c90: 2f63 6c69 656e 7473 2f70 7974 686f 6e2f  /clients/python/
-00001ca0: 7372 632f 6b61 736b 6164 612f 6b61 736b  src/kaskada/kask
-00001cb0: 6164 612f 7631 616c 7068 612f 6d61 7465  ada/v1alpha/mate
-00001cc0: 7269 616c 697a 6174 696f 6e5f 7365 7276  rialization_serv
-00001cd0: 6963 655f 7062 322e 7079 da08 3c6d 6f64  ice_pb2.py..<mod
-00001ce0: 756c 653e 0100 0000 7318 0100 0004 030c  ule>....s.......
-00001cf0: 010c 010c 010c 010c 0108 030c 030c 010c  ................
-00001d00: 010c 010c 010c 010c 010e 030a 040a 010a  ................
-00001d10: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00001d20: 010c 0102 0102 0108 fe0a 050c 0202 0102  ................
-00001d30: 0108 fe0a 050c 0202 0102 0108 fe0a 050c  ................
-00001d40: 0202 0102 0108 fe0a 050c 0202 0102 0108  ................
-00001d50: fe0a 050c 0202 0102 0108 fe0a 050c 0202  ................
-00001d60: 0102 0108 fe0a 050c 0202 0102 0108 fe0a  ................
-00001d70: 050c 0202 0102 0108 fe0a 050c 0202 0102  ................
-00001d80: 0108 fe0a 050c 0202 0102 0108 fe0a 050a  ................
-00001d90: 020c 0106 0206 010c 010c 010c 010c 010c  ................
-00001da0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00001db0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00001dc0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00001dd0: 010c 0106 0106 0106 0106 0106 0106 0106  ................
-00001de0: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00001df0: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00001e00: 010a 0104 c7                             .....
+000004d0: 644b 653c 5f43 641e 5300 294c 7a1f 4765  dKe<_Cd.S.)Lz.Ge
+000004e0: 6e65 7261 7465 6420 7072 6f74 6f63 6f6c  nerated protocol
+000004f0: 2062 7566 6665 7220 636f 6465 2ee9 0000   buffer code....
+00000500: 0000 2901 da0a 6465 7363 7269 7074 6f72  ..)...descriptor
+00000510: 2901 da0f 6465 7363 7269 7074 6f72 5f70  )...descriptor_p
+00000520: 6f6f 6c29 01da 076d 6573 7361 6765 2901  ool)...message).
+00000530: da0a 7265 666c 6563 7469 6f6e 2901 da0f  ..reflection)...
+00000540: 7379 6d62 6f6c 5f64 6174 6162 6173 6529  symbol_database)
+00000550: 01da 0f61 6e6e 6f74 6174 696f 6e73 5f70  ...annotations_p
+00000560: 6232 2901 da12 6669 656c 645f 6265 6861  b2)...field_beha
+00000570: 7669 6f72 5f70 6232 2901 da0d 7469 6d65  vior_pb2)...time
+00000580: 7374 616d 705f 7062 3229 01da 0a63 6f6d  stamp_pb2)...com
+00000590: 6d6f 6e5f 7062 3229 01da 1064 6573 7469  mon_pb2)...desti
+000005a0: 6e61 7469 6f6e 735f 7062 3229 01da 0a73  nations_pb2)...s
+000005b0: 6368 656d 615f 7062 3229 01da 0c76 616c  chema_pb2)...val
+000005c0: 6964 6174 655f 7062 3273 410d 0000 0a35  idate_pb2sA....5
+000005d0: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
+000005e0: 7631 616c 7068 612f 6d61 7465 7269 616c  v1alpha/material
+000005f0: 697a 6174 696f 6e5f 7365 7276 6963 652e  ization_service.
+00000600: 7072 6f74 6f12 176b 6173 6b61 6461 2e6b  proto..kaskada.k
+00000610: 6173 6b61 6461 2e76 3161 6c70 6861 1a1c  askada.v1alpha..
+00000620: 676f 6f67 6c65 2f61 7069 2f61 6e6e 6f74  google/api/annot
+00000630: 6174 696f 6e73 2e70 726f 746f 1a1f 676f  ations.proto..go
+00000640: 6f67 6c65 2f61 7069 2f66 6965 6c64 5f62  ogle/api/field_b
+00000650: 6568 6176 696f 722e 7072 6f74 6f1a 1f67  ehavior.proto..g
+00000660: 6f6f 676c 652f 7072 6f74 6f62 7566 2f74  oogle/protobuf/t
+00000670: 696d 6573 7461 6d70 2e70 726f 746f 1a24  imestamp.proto.$
+00000680: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
+00000690: 7631 616c 7068 612f 636f 6d6d 6f6e 2e70  v1alpha/common.p
+000006a0: 726f 746f 1a2a 6b61 736b 6164 612f 6b61  roto.*kaskada/ka
+000006b0: 736b 6164 612f 7631 616c 7068 612f 6465  skada/v1alpha/de
+000006c0: 7374 696e 6174 696f 6e73 2e70 726f 746f  stinations.proto
+000006d0: 1a24 6b61 736b 6164 612f 6b61 736b 6164  .$kaskada/kaskad
+000006e0: 612f 7631 616c 7068 612f 7363 6865 6d61  a/v1alpha/schema
+000006f0: 2e70 726f 746f 1a17 7661 6c69 6461 7465  .proto..validate
+00000700: 2f76 616c 6964 6174 652e 7072 6f74 6f22  /validate.proto"
+00000710: 500a 0857 6974 6856 6965 7712 1b0a 046e  P..WithView....n
+00000720: 616d 6518 0120 0128 0942 07fa 4204 7202  ame.. .(.B..B.r.
+00000730: 1001 5204 6e61 6d65 1227 0a0a 6578 7072  ..R.name.'..expr
+00000740: 6573 7369 6f6e 1802 2001 2809 4207 fa42  ession.. .(.B..B
+00000750: 0472 0210 0152 0a65 7870 7265 7373 696f  .r...R.expressio
+00000760: 6e22 440a 0957 6974 6856 6965 7773 1237  n"D..WithViews.7
+00000770: 0a05 7669 6577 7318 0120 0328 0b32 212e  ..views.. .(.2!.
+00000780: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000790: 7631 616c 7068 612e 5769 7468 5669 6577  v1alpha.WithView
+000007a0: 5205 7669 6577 7322 db04 0a0f 4d61 7465  R.views"....Mate
+000007b0: 7269 616c 697a 6174 696f 6e12 320a 126d  rialization.2..m
+000007c0: 6174 6572 6961 6c69 7a61 7469 6f6e 5f69  aterialization_i
+000007d0: 6418 0120 0128 0942 03e0 4103 5211 6d61  d.. .(.B..A.R.ma
+000007e0: 7465 7269 616c 697a 6174 696f 6e49 6412  terializationId.
+000007f0: 3a0a 146d 6174 6572 6961 6c69 7a61 7469  :..materializati
+00000800: 6f6e 5f6e 616d 6518 0220 0128 0942 07fa  on_name.. .(.B..
+00000810: 4204 7202 1001 5213 6d61 7465 7269 616c  B.r...R.material
+00000820: 697a 6174 696f 6e4e 616d 6512 400a 0b63  izationName.@..c
+00000830: 7265 6174 655f 7469 6d65 1803 2001 280b  reate_time.. .(.
+00000840: 321a 2e67 6f6f 676c 652e 7072 6f74 6f62  2..google.protob
+00000850: 7566 2e54 696d 6573 7461 6d70 4203 e041  uf.TimestampB..A
+00000860: 0352 0a63 7265 6174 6554 696d 6512 1e0a  .R.createTime...
+00000870: 0a65 7870 7265 7373 696f 6e18 0b20 0128  .expression.. .(
+00000880: 0952 0a65 7870 7265 7373 696f 6e12 400a  .R.expression.@.
+00000890: 0a77 6974 685f 7669 6577 7318 0520 0328  .with_views.. .(
+000008a0: 0b32 212e 6b61 736b 6164 612e 6b61 736b  .2!.kaskada.kask
+000008b0: 6164 612e 7631 616c 7068 612e 5769 7468  ada.v1alpha.With
+000008c0: 5669 6577 5209 7769 7468 5669 6577 7312  ViewR.withViews.
+000008d0: 460a 0b64 6573 7469 6e61 7469 6f6e 1806  F..destination..
+000008e0: 2001 280b 3224 2e6b 6173 6b61 6461 2e6b   .(.2$.kaskada.k
+000008f0: 6173 6b61 6461 2e76 3161 6c70 6861 2e44  askada.v1alpha.D
+00000900: 6573 7469 6e61 7469 6f6e 520b 6465 7374  estinationR.dest
+00000910: 696e 6174 696f 6e12 3c0a 0673 6368 656d  ination.<..schem
+00000920: 6118 0720 0128 0b32 1f2e 6b61 736b 6164  a.. .(.2..kaskad
+00000930: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00000940: 612e 5363 6865 6d61 4203 e041 0352 0673  a.SchemaB..A.R.s
+00000950: 6368 656d 6112 3b0a 0573 6c69 6365 1808  chema.;..slice..
+00000960: 2001 280b 3225 2e6b 6173 6b61 6461 2e6b   .(.2%.kaskada.k
+00000970: 6173 6b61 6461 2e76 3161 6c70 6861 2e53  askada.v1alpha.S
+00000980: 6c69 6365 5265 7175 6573 7452 0573 6c69  liceRequestR.sli
+00000990: 6365 1242 0a08 616e 616c 7973 6973 1809  ce.B..analysis..
+000009a0: 2001 280b 3221 2e6b 6173 6b61 6461 2e6b   .(.2!.kaskada.k
+000009b0: 6173 6b61 6461 2e76 3161 6c70 6861 2e41  askada.v1alpha.A
+000009c0: 6e61 6c79 7369 7342 03e0 4103 5208 616e  nalysisB..A.R.an
+000009d0: 616c 7973 6973 1227 0a0d 6461 7461 5f74  alysis.'..data_t
+000009e0: 6f6b 656e 5f69 6418 0a20 0128 0942 03e0  oken_id.. .(.B..
+000009f0: 4103 520b 6461 7461 546f 6b65 6e49 644a  A.R.dataTokenIdJ
+00000a00: 0408 0410 0522 7d0a 1b4c 6973 744d 6174  ....."}..ListMat
+00000a10: 6572 6961 6c69 7a61 7469 6f6e 7352 6571  erializationsReq
+00000a20: 7565 7374 1216 0a06 7365 6172 6368 1801  uest....search..
+00000a30: 2001 2809 5206 7365 6172 6368 1227 0a09   .(.R.search.'..
+00000a40: 7061 6765 5f73 697a 6518 0220 0128 0542  page_size.. .(.B
+00000a50: 0afa 4207 1a05 18e8 0728 0052 0870 6167  ..B......(.R.pag
+00000a60: 6553 697a 6512 1d0a 0a70 6167 655f 746f  eSize....page_to
+00000a70: 6b65 6e18 0320 0128 0952 0970 6167 6554  ken.. .(.R.pageT
+00000a80: 6f6b 656e 22ee 010a 1c4c 6973 744d 6174  oken"....ListMat
+00000a90: 6572 6961 6c69 7a61 7469 6f6e 7352 6573  erializationsRes
+00000aa0: 706f 6e73 6512 540a 106d 6174 6572 6961  ponse.T..materia
+00000ab0: 6c69 7a61 7469 6f6e 7318 0120 0328 0b32  lizations.. .(.2
+00000ac0: 282e 6b61 736b 6164 612e 6b61 736b 6164  (.kaskada.kaskad
+00000ad0: 612e 7631 616c 7068 612e 4d61 7465 7269  a.v1alpha.Materi
+00000ae0: 616c 697a 6174 696f 6e52 106d 6174 6572  alizationR.mater
+00000af0: 6961 6c69 7a61 7469 6f6e 7312 260a 0f6e  ializations.&..n
+00000b00: 6578 745f 7061 6765 5f74 6f6b 656e 1802  ext_page_token..
+00000b10: 2001 2809 520d 6e65 7874 5061 6765 546f   .(.R.nextPageTo
+00000b20: 6b65 6e12 500a 0f72 6571 7565 7374 5f64  ken.P..request_d
+00000b30: 6574 6169 6c73 1803 2001 280b 3227 2e6b  etails.. .(.2'.k
+00000b40: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
+00000b50: 3161 6c70 6861 2e52 6571 7565 7374 4465  1alpha.RequestDe
+00000b60: 7461 696c 7352 0e72 6571 7565 7374 4465  tailsR.requestDe
+00000b70: 7461 696c 7322 570a 1947 6574 4d61 7465  tails"W..GetMate
+00000b80: 7269 616c 697a 6174 696f 6e52 6571 7565  rializationReque
+00000b90: 7374 123a 0a14 6d61 7465 7269 616c 697a  st.:..materializ
+00000ba0: 6174 696f 6e5f 6e61 6d65 1801 2001 2809  ation_name.. .(.
+00000bb0: 4207 fa42 0472 0210 0152 136d 6174 6572  B..B.r...R.mater
+00000bc0: 6961 6c69 7a61 7469 6f6e 4e61 6d65 22c2  ializationName".
+00000bd0: 010a 1a47 6574 4d61 7465 7269 616c 697a  ...GetMaterializ
+00000be0: 6174 696f 6e52 6573 706f 6e73 6512 520a  ationResponse.R.
+00000bf0: 0f6d 6174 6572 6961 6c69 7a61 7469 6f6e  .materialization
+00000c00: 1801 2001 280b 3228 2e6b 6173 6b61 6461  .. .(.2(.kaskada
+00000c10: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00000c20: 2e4d 6174 6572 6961 6c69 7a61 7469 6f6e  .Materialization
+00000c30: 520f 6d61 7465 7269 616c 697a 6174 696f  R.materializatio
+00000c40: 6e12 500a 0f72 6571 7565 7374 5f64 6574  n.P..request_det
+00000c50: 6169 6c73 1802 2001 280b 3227 2e6b 6173  ails.. .(.2'.kas
+00000c60: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
+00000c70: 6c70 6861 2e52 6571 7565 7374 4465 7461  lpha.RequestDeta
+00000c80: 696c 7352 0e72 6571 7565 7374 4465 7461  ilsR.requestDeta
+00000c90: 696c 7322 8b01 0a1c 4372 6561 7465 4d61  ils"....CreateMa
+00000ca0: 7465 7269 616c 697a 6174 696f 6e52 6571  terializationReq
+00000cb0: 7565 7374 1252 0a0f 6d61 7465 7269 616c  uest.R..material
+00000cc0: 697a 6174 696f 6e18 0120 0128 0b32 282e  ization.. .(.2(.
+00000cd0: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000ce0: 7631 616c 7068 612e 4d61 7465 7269 616c  v1alpha.Material
+00000cf0: 697a 6174 696f 6e52 0f6d 6174 6572 6961  izationR.materia
+00000d00: 6c69 7a61 7469 6f6e 1217 0a07 6472 795f  lization....dry_
+00000d10: 7275 6e18 0220 0128 0852 0664 7279 5275  run.. .(.R.dryRu
+00000d20: 6e22 8402 0a1d 4372 6561 7465 4d61 7465  n"....CreateMate
+00000d30: 7269 616c 697a 6174 696f 6e52 6573 706f  rializationRespo
+00000d40: 6e73 6512 520a 0f6d 6174 6572 6961 6c69  nse.R..materiali
+00000d50: 7a61 7469 6f6e 1801 2001 280b 3228 2e6b  zation.. .(.2(.k
+00000d60: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
+00000d70: 3161 6c70 6861 2e4d 6174 6572 6961 6c69  1alpha.Materiali
+00000d80: 7a61 7469 6f6e 520f 6d61 7465 7269 616c  zationR.material
+00000d90: 697a 6174 696f 6e12 500a 0f72 6571 7565  ization.P..reque
+00000da0: 7374 5f64 6574 6169 6c73 1802 2001 280b  st_details.. .(.
+00000db0: 3227 2e6b 6173 6b61 6461 2e6b 6173 6b61  2'.kaskada.kaska
+00000dc0: 6461 2e76 3161 6c70 6861 2e52 6571 7565  da.v1alpha.Reque
+00000dd0: 7374 4465 7461 696c 7352 0e72 6571 7565  stDetailsR.reque
+00000de0: 7374 4465 7461 696c 7312 3d0a 0861 6e61  stDetails.=..ana
+00000df0: 6c79 7369 7318 0320 0128 0b32 212e 6b61  lysis.. .(.2!.ka
+00000e00: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
+00000e10: 616c 7068 612e 416e 616c 7973 6973 5208  alpha.AnalysisR.
+00000e20: 616e 616c 7973 6973 225a 0a1c 4465 6c65  analysis"Z..Dele
+00000e30: 7465 4d61 7465 7269 616c 697a 6174 696f  teMaterializatio
+00000e40: 6e52 6571 7565 7374 123a 0a14 6d61 7465  nRequest.:..mate
+00000e50: 7269 616c 697a 6174 696f 6e5f 6e61 6d65  rialization_name
+00000e60: 1801 2001 2809 4207 fa42 0472 0210 0152  .. .(.B..B.r...R
+00000e70: 136d 6174 6572 6961 6c69 7a61 7469 6f6e  .materialization
+00000e80: 4e61 6d65 2271 0a1d 4465 6c65 7465 4d61  Name"q..DeleteMa
+00000e90: 7465 7269 616c 697a 6174 696f 6e52 6573  terializationRes
+00000ea0: 706f 6e73 6512 500a 0f72 6571 7565 7374  ponse.P..request
+00000eb0: 5f64 6574 6169 6c73 1801 2001 280b 3227  _details.. .(.2'
+00000ec0: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00000ed0: 2e76 3161 6c70 6861 2e52 6571 7565 7374  .v1alpha.Request
+00000ee0: 4465 7461 696c 7352 0e72 6571 7565 7374  DetailsR.request
+00000ef0: 4465 7461 696c 7332 ff05 0a16 4d61 7465  Details2....Mate
+00000f00: 7269 616c 697a 6174 696f 6e53 6572 7669  rializationServi
+00000f10: 6365 12a6 010a 144c 6973 744d 6174 6572  ce.....ListMater
+00000f20: 6961 6c69 7a61 7469 6f6e 7312 342e 6b61  ializations.4.ka
+00000f30: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
+00000f40: 616c 7068 612e 4c69 7374 4d61 7465 7269  alpha.ListMateri
+00000f50: 616c 697a 6174 696f 6e73 5265 7175 6573  alizationsReques
+00000f60: 741a 352e 6b61 736b 6164 612e 6b61 736b  t.5.kaskada.kask
+00000f70: 6164 612e 7631 616c 7068 612e 4c69 7374  ada.v1alpha.List
+00000f80: 4d61 7465 7269 616c 697a 6174 696f 6e73  Materializations
+00000f90: 5265 7370 6f6e 7365 2221 82d3 e493 021b  Response"!......
+00000fa0: 1219 2f76 3161 6c70 6861 2f6d 6174 6572  ../v1alpha/mater
+00000fb0: 6961 6c69 7a61 7469 6f6e 7312 b901 0a12  ializations.....
+00000fc0: 4765 744d 6174 6572 6961 6c69 7a61 7469  GetMaterializati
+00000fd0: 6f6e 1232 2e6b 6173 6b61 6461 2e6b 6173  on.2.kaskada.kas
+00000fe0: 6b61 6461 2e76 3161 6c70 6861 2e47 6574  kada.v1alpha.Get
+00000ff0: 4d61 7465 7269 616c 697a 6174 696f 6e52  MaterializationR
+00001000: 6571 7565 7374 1a33 2e6b 6173 6b61 6461  equest.3.kaskada
+00001010: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00001020: 2e47 6574 4d61 7465 7269 616c 697a 6174  .GetMaterializat
+00001030: 696f 6e52 6573 706f 6e73 6522 3a82 d3e4  ionResponse":...
+00001040: 9302 3412 322f 7631 616c 7068 612f 6d61  ..4.2/v1alpha/ma
+00001050: 7465 7269 616c 697a 6174 696f 6e73 2f7b  terializations/{
+00001060: 6d61 7465 7269 616c 697a 6174 696f 6e5f  materialization_
+00001070: 6e61 6d65 3d2a 7d12 ba01 0a15 4372 6561  name=*}.....Crea
+00001080: 7465 4d61 7465 7269 616c 697a 6174 696f  teMaterializatio
+00001090: 6e12 352e 6b61 736b 6164 612e 6b61 736b  n.5.kaskada.kask
+000010a0: 6164 612e 7631 616c 7068 612e 4372 6561  ada.v1alpha.Crea
+000010b0: 7465 4d61 7465 7269 616c 697a 6174 696f  teMaterializatio
+000010c0: 6e52 6571 7565 7374 1a36 2e6b 6173 6b61  nRequest.6.kaska
+000010d0: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
+000010e0: 6861 2e43 7265 6174 654d 6174 6572 6961  ha.CreateMateria
+000010f0: 6c69 7a61 7469 6f6e 5265 7370 6f6e 7365  lizationResponse
+00001100: 2232 82d3 e493 022c 3a0f 6d61 7465 7269  "2.....,:.materi
+00001110: 616c 697a 6174 696f 6e22 192f 7631 616c  alization"./v1al
+00001120: 7068 612f 6d61 7465 7269 616c 697a 6174  pha/materializat
+00001130: 696f 6e73 12c2 010a 1544 656c 6574 654d  ions.....DeleteM
+00001140: 6174 6572 6961 6c69 7a61 7469 6f6e 1235  aterialization.5
+00001150: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00001160: 2e76 3161 6c70 6861 2e44 656c 6574 654d  .v1alpha.DeleteM
+00001170: 6174 6572 6961 6c69 7a61 7469 6f6e 5265  aterializationRe
+00001180: 7175 6573 741a 362e 6b61 736b 6164 612e  quest.6.kaskada.
+00001190: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
+000011a0: 4465 6c65 7465 4d61 7465 7269 616c 697a  DeleteMaterializ
+000011b0: 6174 696f 6e52 6573 706f 6e73 6522 3a82  ationResponse":.
+000011c0: d3e4 9302 342a 322f 7631 616c 7068 612f  ....4*2/v1alpha/
+000011d0: 6d61 7465 7269 616c 697a 6174 696f 6e73  materializations
+000011e0: 2f7b 6d61 7465 7269 616c 697a 6174 696f  /{materializatio
+000011f0: 6e5f 6e61 6d65 3d2a 7d42 8b02 0a1b 636f  n_name=*}B....co
+00001200: 6d2e 6b61 736b 6164 612e 6b61 736b 6164  m.kaskada.kaskad
+00001210: 612e 7631 616c 7068 6142 1b4d 6174 6572  a.v1alphaB.Mater
+00001220: 6961 6c69 7a61 7469 6f6e 5365 7276 6963  ializationServic
+00001230: 6550 726f 746f 5001 5a51 6769 7468 7562  eProtoP.ZQgithub
+00001240: 2e63 6f6d 2f6b 6173 6b61 6461 2d61 692f  .com/kaskada-ai/
+00001250: 6b61 736b 6164 612f 6765 6e2f 7072 6f74  kaskada/gen/prot
+00001260: 6f2f 676f 2f6b 6173 6b61 6461 2f6b 6173  o/go/kaskada/kas
+00001270: 6b61 6461 2f76 3161 6c70 6861 3b6b 6173  kada/v1alpha;kas
+00001280: 6b61 6461 7631 616c 7068 61a2 0203 4b4b  kadav1alpha...KK
+00001290: 58aa 0217 4b61 736b 6164 612e 4b61 736b  X...Kaskada.Kask
+000012a0: 6164 612e 5631 616c 7068 61ca 0217 4b61  ada.V1alpha...Ka
+000012b0: 736b 6164 615c 4b61 736b 6164 615c 5631  skada\Kaskada\V1
+000012c0: 616c 7068 61e2 0223 4b61 736b 6164 615c  alpha..#Kaskada\
+000012d0: 4b61 736b 6164 615c 5631 616c 7068 615c  Kaskada\V1alpha\
+000012e0: 4750 424d 6574 6164 6174 61ea 0219 4b61  GPBMetadata...Ka
+000012f0: 736b 6164 613a 3a4b 6173 6b61 6461 3a3a  skada::Kaskada::
+00001300: 5631 616c 7068 6162 0670 726f 746f 33da  V1alphab.proto3.
+00001310: 0857 6974 6856 6965 77da 0957 6974 6856  .WithView..WithV
+00001320: 6965 7773 da0f 4d61 7465 7269 616c 697a  iews..Materializ
+00001330: 6174 696f 6eda 1b4c 6973 744d 6174 6572  ation..ListMater
+00001340: 6961 6c69 7a61 7469 6f6e 7352 6571 7565  ializationsReque
+00001350: 7374 da1c 4c69 7374 4d61 7465 7269 616c  st..ListMaterial
+00001360: 697a 6174 696f 6e73 5265 7370 6f6e 7365  izationsResponse
+00001370: da19 4765 744d 6174 6572 6961 6c69 7a61  ..GetMaterializa
+00001380: 7469 6f6e 5265 7175 6573 74da 1a47 6574  tionRequest..Get
+00001390: 4d61 7465 7269 616c 697a 6174 696f 6e52  MaterializationR
+000013a0: 6573 706f 6e73 65da 1c43 7265 6174 654d  esponse..CreateM
+000013b0: 6174 6572 6961 6c69 7a61 7469 6f6e 5265  aterializationRe
+000013c0: 7175 6573 74da 1d43 7265 6174 654d 6174  quest..CreateMat
+000013d0: 6572 6961 6c69 7a61 7469 6f6e 5265 7370  erializationResp
+000013e0: 6f6e 7365 da1c 4465 6c65 7465 4d61 7465  onse..DeleteMate
+000013f0: 7269 616c 697a 6174 696f 6e52 6571 7565  rializationReque
+00001400: 7374 da1d 4465 6c65 7465 4d61 7465 7269  st..DeleteMateri
+00001410: 616c 697a 6174 696f 6e52 6573 706f 6e73  alizationRespons
+00001420: 657a 336b 6173 6b61 6461 2e6b 6173 6b61  ez3kaskada.kaska
+00001430: 6461 2e76 3161 6c70 6861 2e6d 6174 6572  da.v1alpha.mater
+00001440: 6961 6c69 7a61 7469 6f6e 5f73 6572 7669  ialization_servi
+00001450: 6365 5f70 6232 2902 da0a 4445 5343 5249  ce_pb2)...DESCRI
+00001460: 5054 4f52 da0a 5f5f 6d6f 6475 6c65 5f5f  PTOR..__module__
+00001470: da16 4d61 7465 7269 616c 697a 6174 696f  ..Materializatio
+00001480: 6e53 6572 7669 6365 464e 730b 0100 000a  nServiceFNs.....
+00001490: 1b63 6f6d 2e6b 6173 6b61 6461 2e6b 6173  .com.kaskada.kas
+000014a0: 6b61 6461 2e76 3161 6c70 6861 421b 4d61  kada.v1alphaB.Ma
+000014b0: 7465 7269 616c 697a 6174 696f 6e53 6572  terializationSer
+000014c0: 7669 6365 5072 6f74 6f50 015a 5167 6974  viceProtoP.ZQgit
+000014d0: 6875 622e 636f 6d2f 6b61 736b 6164 612d  hub.com/kaskada-
+000014e0: 6169 2f6b 6173 6b61 6461 2f67 656e 2f70  ai/kaskada/gen/p
+000014f0: 726f 746f 2f67 6f2f 6b61 736b 6164 612f  roto/go/kaskada/
+00001500: 6b61 736b 6164 612f 7631 616c 7068 613b  kaskada/v1alpha;
+00001510: 6b61 736b 6164 6176 3161 6c70 6861 a202  kaskadav1alpha..
+00001520: 034b 4b58 aa02 174b 6173 6b61 6461 2e4b  .KKX...Kaskada.K
+00001530: 6173 6b61 6461 2e56 3161 6c70 6861 ca02  askada.V1alpha..
+00001540: 174b 6173 6b61 6461 5c4b 6173 6b61 6461  .Kaskada\Kaskada
+00001550: 5c56 3161 6c70 6861 e202 234b 6173 6b61  \V1alpha..#Kaska
+00001560: 6461 5c4b 6173 6b61 6461 5c56 3161 6c70  da\Kaskada\V1alp
+00001570: 6861 5c47 5042 4d65 7461 6461 7461 ea02  ha\GPBMetadata..
+00001580: 194b 6173 6b61 6461 3a3a 4b61 736b 6164  .Kaskada::Kaskad
+00001590: 613a 3a56 3161 6c70 6861 da04 6e61 6d65  a::V1alpha..name
+000015a0: 7307 0000 00fa 4204 7202 1001 da0a 6578  s.....B.r.....ex
+000015b0: 7072 6573 7369 6f6e 5a12 6d61 7465 7269  pressionZ.materi
+000015c0: 616c 697a 6174 696f 6e5f 6964 7303 0000  alization_ids...
+000015d0: 00e0 4103 da14 6d61 7465 7269 616c 697a  ..A...materializ
+000015e0: 6174 696f 6e5f 6e61 6d65 da0b 6372 6561  ation_name..crea
+000015f0: 7465 5f74 696d 65da 0673 6368 656d 61da  te_time..schema.
+00001600: 0861 6e61 6c79 7369 73da 0d64 6174 615f  .analysis..data_
+00001610: 746f 6b65 6e5f 6964 da09 7061 6765 5f73  token_id..page_s
+00001620: 697a 6573 0a00 0000 fa42 071a 0518 e807  izes.....B......
+00001630: 2800 da14 4c69 7374 4d61 7465 7269 616c  (...ListMaterial
+00001640: 697a 6174 696f 6e73 7321 0000 0082 d3e4  izationss!......
+00001650: 9302 1b12 192f 7631 616c 7068 612f 6d61  ...../v1alpha/ma
+00001660: 7465 7269 616c 697a 6174 696f 6e73 da12  terializations..
+00001670: 4765 744d 6174 6572 6961 6c69 7a61 7469  GetMaterializati
+00001680: 6f6e 733a 0000 0082 d3e4 9302 3412 322f  ons:........4.2/
+00001690: 7631 616c 7068 612f 6d61 7465 7269 616c  v1alpha/material
+000016a0: 697a 6174 696f 6e73 2f7b 6d61 7465 7269  izations/{materi
+000016b0: 616c 697a 6174 696f 6e5f 6e61 6d65 3d2a  alization_name=*
+000016c0: 7dda 1543 7265 6174 654d 6174 6572 6961  }..CreateMateria
+000016d0: 6c69 7a61 7469 6f6e 7332 0000 0082 d3e4  lizations2......
+000016e0: 9302 2c3a 0f6d 6174 6572 6961 6c69 7a61  ..,:.materializa
+000016f0: 7469 6f6e 2219 2f76 3161 6c70 6861 2f6d  tion"./v1alpha/m
+00001700: 6174 6572 6961 6c69 7a61 7469 6f6e 73da  aterializations.
+00001710: 1544 656c 6574 654d 6174 6572 6961 6c69  .DeleteMateriali
+00001720: 7a61 7469 6f6e 733a 0000 0082 d3e4 9302  zations:........
+00001730: 342a 322f 7631 616c 7068 612f 6d61 7465  4*2/v1alpha/mate
+00001740: 7269 616c 697a 6174 696f 6e73 2f7b 6d61  rializations/{ma
+00001750: 7465 7269 616c 697a 6174 696f 6e5f 6e61  terialization_na
+00001760: 6d65 3d2a 7d69 4301 0000 6993 0100 0069  me=*}iC...i....i
+00001770: 9501 0000 69d9 0100 0069 dc01 0000 6937  ....i....i....i7
+00001780: 0400 0069 3904 0000 69b6 0400 0069 b904  ...i9...i....i..
+00001790: 0000 69a7 0500 0069 a905 0000 6900 0600  ..i....i....i...
+000017a0: 0069 0306 0000 69c5 0600 0069 c806 0000  .i....i....i....
+000017b0: 6953 0700 0069 5607 0000 695a 0800 0069  iS...iV...iZ...i
+000017c0: 5c08 0000 69b6 0800 0069 b808 0000 6929  \...i....i....i)
+000017d0: 0900 0069 2c09 0000 692b 0c00 0029 44da  ...i,...i+...)D.
+000017e0: 075f 5f64 6f63 5f5f da0f 676f 6f67 6c65  .__doc__..google
+000017f0: 2e70 726f 746f 6275 6672 0200 0000 da0b  .protobufr......
+00001800: 5f64 6573 6372 6970 746f 7272 0300 0000  _descriptorr....
+00001810: da10 5f64 6573 6372 6970 746f 725f 706f  .._descriptor_po
+00001820: 6f6c 7204 0000 00da 085f 6d65 7373 6167  olr......_messag
+00001830: 6572 0500 0000 da0b 5f72 6566 6c65 6374  er......_reflect
+00001840: 696f 6e72 0600 0000 da10 5f73 796d 626f  ionr......_symbo
+00001850: 6c5f 6461 7461 6261 7365 da07 4465 6661  l_database..Defa
+00001860: 756c 74da 075f 7379 6d5f 6462 da0a 676f  ult.._sym_db..go
+00001870: 6f67 6c65 2e61 7069 7207 0000 00da 2367  ogle.apir.....#g
+00001880: 6f6f 676c 655f 646f 745f 6170 695f 646f  oogle_dot_api_do
+00001890: 745f 616e 6e6f 7461 7469 6f6e 735f 5f70  t_annotations__p
+000018a0: 6232 7208 0000 00da 2767 6f6f 676c 655f  b2r.....'google_
+000018b0: 646f 745f 6170 695f 646f 745f 6669 656c  dot_api_dot_fiel
+000018c0: 645f 5f62 6568 6176 696f 725f 5f70 6232  d__behavior__pb2
+000018d0: 7209 0000 00da 2667 6f6f 676c 655f 646f  r.....&google_do
+000018e0: 745f 7072 6f74 6f62 7566 5f64 6f74 5f74  t_protobuf_dot_t
+000018f0: 696d 6573 7461 6d70 5f5f 7062 32da 176b  imestamp__pb2..k
+00001900: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
+00001910: 3161 6c70 6861 720a 0000 00da 2f6b 6173  1alphar...../kas
+00001920: 6b61 6461 5f64 6f74 5f6b 6173 6b61 6461  kada_dot_kaskada
+00001930: 5f64 6f74 5f76 3161 6c70 6861 5f64 6f74  _dot_v1alpha_dot
+00001940: 5f63 6f6d 6d6f 6e5f 5f70 6232 720b 0000  _common__pb2r...
+00001950: 005a 356b 6173 6b61 6461 5f64 6f74 5f6b  .Z5kaskada_dot_k
+00001960: 6173 6b61 6461 5f64 6f74 5f76 3161 6c70  askada_dot_v1alp
+00001970: 6861 5f64 6f74 5f64 6573 7469 6e61 7469  ha_dot_destinati
+00001980: 6f6e 735f 5f70 6232 720c 0000 00da 2f6b  ons__pb2r...../k
+00001990: 6173 6b61 6461 5f64 6f74 5f6b 6173 6b61  askada_dot_kaska
+000019a0: 6461 5f64 6f74 5f76 3161 6c70 6861 5f64  da_dot_v1alpha_d
+000019b0: 6f74 5f73 6368 656d 615f 5f70 6232 da08  ot_schema__pb2..
+000019c0: 7661 6c69 6461 7465 720d 0000 00da 1a76  validater......v
+000019d0: 616c 6964 6174 655f 646f 745f 7661 6c69  alidate_dot_vali
+000019e0: 6461 7465 5f5f 7062 32da 1141 6464 5365  date__pb2..AddSe
+000019f0: 7269 616c 697a 6564 4669 6c65 7219 0000  rializedFiler...
+00001a00: 00da 156d 6573 7361 6765 5f74 7970 6573  ...message_types
+00001a10: 5f62 795f 6e61 6d65 5a09 5f57 4954 4856  _by_nameZ._WITHV
+00001a20: 4945 575a 0a5f 5749 5448 5649 4557 535a  IEWZ._WITHVIEWSZ
+00001a30: 105f 4d41 5445 5249 414c 495a 4154 494f  ._MATERIALIZATIO
+00001a40: 4e5a 1c5f 4c49 5354 4d41 5445 5249 414c  NZ._LISTMATERIAL
+00001a50: 495a 4154 494f 4e53 5245 5155 4553 545a  IZATIONSREQUESTZ
+00001a60: 1d5f 4c49 5354 4d41 5445 5249 414c 495a  ._LISTMATERIALIZ
+00001a70: 4154 494f 4e53 5245 5350 4f4e 5345 5a1a  ATIONSRESPONSEZ.
+00001a80: 5f47 4554 4d41 5445 5249 414c 495a 4154  _GETMATERIALIZAT
+00001a90: 494f 4e52 4551 5545 5354 5a1b 5f47 4554  IONREQUESTZ._GET
+00001aa0: 4d41 5445 5249 414c 495a 4154 494f 4e52  MATERIALIZATIONR
+00001ab0: 4553 504f 4e53 455a 1d5f 4352 4541 5445  ESPONSEZ._CREATE
+00001ac0: 4d41 5445 5249 414c 495a 4154 494f 4e52  MATERIALIZATIONR
+00001ad0: 4551 5545 5354 5a1e 5f43 5245 4154 454d  EQUESTZ._CREATEM
+00001ae0: 4154 4552 4941 4c49 5a41 5449 4f4e 5245  ATERIALIZATIONRE
+00001af0: 5350 4f4e 5345 5a1d 5f44 454c 4554 454d  SPONSEZ._DELETEM
+00001b00: 4154 4552 4941 4c49 5a41 5449 4f4e 5245  ATERIALIZATIONRE
+00001b10: 5155 4553 545a 1e5f 4445 4c45 5445 4d41  QUESTZ._DELETEMA
+00001b20: 5445 5249 414c 495a 4154 494f 4e52 4553  TERIALIZATIONRES
+00001b30: 504f 4e53 45da 1c47 656e 6572 6174 6564  PONSE..Generated
+00001b40: 5072 6f74 6f63 6f6c 4d65 7373 6167 6554  ProtocolMessageT
+00001b50: 7970 65da 074d 6573 7361 6765 720e 0000  ype..Messager...
+00001b60: 00da 0f52 6567 6973 7465 724d 6573 7361  ...RegisterMessa
+00001b70: 6765 720f 0000 0072 1000 0000 7211 0000  ger....r....r...
+00001b80: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+00001b90: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00001ba0: 1800 0000 da10 7365 7276 6963 6573 5f62  ......services_b
+00001bb0: 795f 6e61 6d65 5a17 5f4d 4154 4552 4941  y_nameZ._MATERIA
+00001bc0: 4c49 5a41 5449 4f4e 5345 5256 4943 45da  LIZATIONSERVICE.
+00001bd0: 125f 5553 455f 435f 4445 5343 5249 5054  ._USE_C_DESCRIPT
+00001be0: 4f52 53da 085f 6f70 7469 6f6e 73da 135f  ORS.._options.._
+00001bf0: 7365 7269 616c 697a 6564 5f6f 7074 696f  serialized_optio
+00001c00: 6e73 da0e 6669 656c 6473 5f62 795f 6e61  ns..fields_by_na
+00001c10: 6d65 da0f 6d65 7468 6f64 735f 6279 5f6e  me..methods_by_n
+00001c20: 616d 65da 115f 7365 7269 616c 697a 6564  ame.._serialized
+00001c30: 5f73 7461 7274 da0f 5f73 6572 6961 6c69  _start.._seriali
+00001c40: 7a65 645f 656e 64a9 0072 4700 0000 7247  zed_end..rG...rG
+00001c50: 0000 00fa 3f2f 7372 632f 7372 632f 6b61  ....?/src/src/ka
+00001c60: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
+00001c70: 616c 7068 612f 6d61 7465 7269 616c 697a  alpha/materializ
+00001c80: 6174 696f 6e5f 7365 7276 6963 655f 7062  ation_service_pb
+00001c90: 322e 7079 da08 3c6d 6f64 756c 653e 0400  2.py..<module>..
+00001ca0: 0000 7314 0100 0004 010c 010c 010c 010c  ..s.............
+00001cb0: 010c 0308 030c 010c 010c 010c 010c 010c  ................
+00001cc0: 010c 030e 040a 010a 010a 010a 010a 010a  ................
+00001cd0: 010a 010a 010a 010a 010a 010c 0102 0102  ................
+00001ce0: fe08 050a 020c 0102 0102 fe08 050a 020c  ................
+00001cf0: 0102 0102 fe08 050a 020c 0102 0102 fe08  ................
+00001d00: 050a 020c 0102 0102 fe08 050a 020c 0102  ................
+00001d10: 0102 fe08 050a 020c 0102 0102 fe08 050a  ................
+00001d20: 020c 0102 0102 fe08 050a 020c 0102 0102  ................
+00001d30: fe08 050a 020c 0102 0102 fe08 050a 020c  ................
+00001d40: 0102 0102 fe08 050a 020a 010c 0206 0106  ................
+00001d50: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00001d60: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00001d70: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00001d80: 010c 010c 010c 010c 010c 010c 0106 0106  ................
+00001d90: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00001da0: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00001db0: 0106 0106 0106 0106 0106 01              ...........
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/materialization_service_pb2_grpc.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/materialization_service_pb2_grpc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 9283 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 4324 0000  o.........5dC$..
+00000000: 610d 0d0a 0000 0000 2038 4164 4324 0000  a....... 8AdC$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a04 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000050: 6505 8303 5a06 4700 6406 6407 8400 6407  e...Z.G.d.d...d.
 00000060: 6505 8303 5a07 6408 6409 8400 5a08 4700  e...Z.d.d...Z.G.
 00000070: 640a 640b 8400 640b 6505 8303 5a09 6402  d.d...d.e...Z.d.
@@ -79,231 +79,243 @@
 000004e0: 7465 4d61 7465 7269 616c 697a 6174 696f  teMaterializatio
 000004f0: 6eda 1c44 656c 6574 654d 6174 6572 6961  n..DeleteMateria
 00000500: 6c69 7a61 7469 6f6e 5265 7175 6573 74da  lizationRequest.
 00000510: 1d44 656c 6574 654d 6174 6572 6961 6c69  .DeleteMateriali
 00000520: 7a61 7469 6f6e 5265 7370 6f6e 7365 da15  zationResponse..
 00000530: 4465 6c65 7465 4d61 7465 7269 616c 697a  DeleteMaterializ
 00000540: 6174 696f 6e29 02da 0473 656c 66da 0763  ation)...self..c
-00000550: 6861 6e6e 656c a900 721d 0000 00fa 862f  hannel..r....../
-00000560: 686f 6d65 2f74 6865 7261 706f 6e2f 5265  home/therapon/Re
-00000570: 706f 732f 4769 7448 7562 2f4b 6173 6b61  pos/GitHub/Kaska
-00000580: 6461 4149 2f6b 6173 6b61 6461 2f72 656c  daAI/kaskada/rel
-00000590: 6561 7369 6e67 2f63 6c69 656e 7473 2f70  easing/clients/p
-000005a0: 7974 686f 6e2f 7372 632f 6b61 736b 6164  ython/src/kaskad
-000005b0: 612f 6b61 736b 6164 612f 7631 616c 7068  a/kaskada/v1alph
-000005c0: 612f 6d61 7465 7269 616c 697a 6174 696f  a/materializatio
-000005d0: 6e5f 7365 7276 6963 655f 7062 325f 6772  n_service_pb2_gr
-000005e0: 7063 2e70 79da 085f 5f69 6e69 745f 5f0c  pc.py..__init__.
-000005f0: 0000 0073 2800 0000 0406 0201 0601 0601  ...s(...........
-00000600: 08fd 0405 0201 0601 0601 08fd 0405 0201  ................
-00000610: 0601 0601 08fd 0405 0201 0601 0601 0cfd  ................
-00000620: 7a23 4d61 7465 7269 616c 697a 6174 696f  z#Materializatio
-00000630: 6e53 6572 7669 6365 5374 7562 2e5f 5f69  nServiceStub.__i
-00000640: 6e69 745f 5f4e 2905 da08 5f5f 6e61 6d65  nit__N)...__name
-00000650: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000660: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
-00000670: 646f 635f 5f72 1f00 0000 721d 0000 0072  doc__r....r....r
-00000680: 1d00 0000 721d 0000 0072 1e00 0000 7203  ....r....r....r.
-00000690: 0000 0008 0000 0073 0600 0000 0800 0401  .......s........
-000006a0: 0c03 7203 0000 0063 0000 0000 0000 0000  ..r....c........
-000006b0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-000006c0: 7330 0000 0065 005a 0164 005a 0264 015a  s0...e.Z.d.Z.d.Z
-000006d0: 0364 0264 0384 005a 0464 0464 0584 005a  .d.d...Z.d.d...Z
-000006e0: 0564 0664 0784 005a 0664 0864 0984 005a  .d.d...Z.d.d...Z
-000006f0: 0764 0a53 0029 0bda 1e4d 6174 6572 6961  .d.S.)...Materia
-00000700: 6c69 7a61 7469 6f6e 5365 7276 6963 6553  lizationServiceS
-00000710: 6572 7669 6365 7272 0400 0000 6303 0000  ervicerr....c...
-00000720: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00000730: 0043 0000 00f3 2000 0000 7c02 a000 7401  .C.... ...|...t.
-00000740: 6a02 6a03 a101 0100 7c02 a004 6401 a101  j.j.....|...d...
-00000750: 0100 7405 6401 8301 8201 2902 7ae4 4c69  ..t.d.....).z.Li
-00000760: 7374 7320 6d61 7465 7269 616c 697a 6174  sts materializat
-00000770: 696f 6e73 2e0a 0a20 2020 2020 2020 2054  ions...        T
-00000780: 6865 2072 6573 706f 6e73 6520 696e 636c  he response incl
-00000790: 7564 6573 2061 6c6c 204d 6174 6572 6961  udes all Materia
-000007a0: 6c69 7a61 7469 6f6e 7320 6465 6669 6e65  lizations define
-000007b0: 6420 666f 7220 7468 6520 4b61 736b 6164  d for the Kaskad
-000007c0: 610a 2020 2020 2020 2020 6163 636f 756e  a.        accoun
-000007d0: 742e 2049 6620 6120 7365 6172 6368 2073  t. If a search s
-000007e0: 7472 696e 6720 6973 2070 726f 7669 6465  tring is provide
-000007f0: 642c 206f 6e6c 7920 4d61 7465 7269 616c  d, only Material
-00000800: 697a 6174 696f 6e73 0a20 2020 2020 2020  izations.       
-00000810: 206d 6174 6368 696e 6720 7468 6520 7365   matching the se
-00000820: 6172 6368 2073 7472 696e 6720 6172 6520  arch string are 
-00000830: 7265 7475 726e 6564 2e0a 2020 2020 2020  returned..      
-00000840: 2020 fa17 4d65 7468 6f64 206e 6f74 2069    ..Method not i
-00000850: 6d70 6c65 6d65 6e74 6564 21a9 06da 0873  mplemented!....s
-00000860: 6574 5f63 6f64 65da 0467 7270 63da 0a53  et_code..grpc..S
-00000870: 7461 7475 7343 6f64 65da 0d55 4e49 4d50  tatusCode..UNIMP
-00000880: 4c45 4d45 4e54 4544 da0b 7365 745f 6465  LEMENTED..set_de
-00000890: 7461 696c 73da 134e 6f74 496d 706c 656d  tails..NotImplem
-000008a0: 656e 7465 6445 7272 6f72 a903 721b 0000  entedError..r...
-000008b0: 00da 0772 6571 7565 7374 da07 636f 6e74  ...request..cont
-000008c0: 6578 7472 1d00 0000 721d 0000 0072 1e00  extr....r....r..
-000008d0: 0000 7211 0000 002c 0000 0073 0600 0000  ..r....,...s....
-000008e0: 0e07 0a01 0801 7a33 4d61 7465 7269 616c  ......z3Material
-000008f0: 697a 6174 696f 6e53 6572 7669 6365 5365  izationServiceSe
-00000900: 7276 6963 6572 2e4c 6973 744d 6174 6572  rvicer.ListMater
-00000910: 6961 6c69 7a61 7469 6f6e 7363 0300 0000  ializationsc....
-00000920: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00000930: 4300 0000 7225 0000 0029 027a 2047 6574  C...r%...).z Get
-00000940: 7320 6120 6d61 7465 7269 616c 697a 6174  s a materializat
-00000950: 696f 6e2e 0a20 2020 2020 2020 2072 2600  ion..        r&.
-00000960: 0000 7227 0000 0072 2e00 0000 721d 0000  ..r'...r....r...
-00000970: 0072 1d00 0000 721e 0000 0072 1400 0000  .r....r....r....
-00000980: 3700 0000 f306 0000 000e 030a 0108 017a  7..............z
-00000990: 314d 6174 6572 6961 6c69 7a61 7469 6f6e  1Materialization
-000009a0: 5365 7276 6963 6553 6572 7669 6365 722e  ServiceServicer.
-000009b0: 4765 744d 6174 6572 6961 6c69 7a61 7469  GetMaterializati
-000009c0: 6f6e 6303 0000 0000 0000 0000 0000 0003  onc.............
-000009d0: 0000 0003 0000 0043 0000 0072 2500 0000  .......C...r%...
-000009e0: 2902 7a23 4372 6561 7465 7320 6120 6d61  ).z#Creates a ma
-000009f0: 7465 7269 616c 697a 6174 696f 6e2e 0a20  terialization.. 
-00000a00: 2020 2020 2020 2072 2600 0000 7227 0000         r&...r'..
-00000a10: 0072 2e00 0000 721d 0000 0072 1d00 0000  .r....r....r....
-00000a20: 721e 0000 0072 1700 0000 3e00 0000 7231  r....r....>...r1
-00000a30: 0000 007a 344d 6174 6572 6961 6c69 7a61  ...z4Materializa
-00000a40: 7469 6f6e 5365 7276 6963 6553 6572 7669  tionServiceServi
-00000a50: 6365 722e 4372 6561 7465 4d61 7465 7269  cer.CreateMateri
-00000a60: 616c 697a 6174 696f 6e63 0300 0000 0000  alizationc......
-00000a70: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00000a80: 0000 7225 0000 0029 027a 4144 656c 6574  ..r%...).zADelet
-00000a90: 6573 2061 206d 6174 6572 6961 6c69 7a61  es a materializa
-00000aa0: 7469 6f6e 2061 6e64 2061 6e79 2065 7665  tion and any eve
-00000ab0: 6e74 7320 6c6f 6164 6564 2069 6e74 6f20  nts loaded into 
-00000ac0: 6974 2e0a 2020 2020 2020 2020 7226 0000  it..        r&..
-00000ad0: 0072 2700 0000 722e 0000 0072 1d00 0000  .r'...r....r....
-00000ae0: 721d 0000 0072 1e00 0000 721a 0000 0045  r....r....r....E
-00000af0: 0000 0072 3100 0000 7a34 4d61 7465 7269  ...r1...z4Materi
-00000b00: 616c 697a 6174 696f 6e53 6572 7669 6365  alizationService
-00000b10: 5365 7276 6963 6572 2e44 656c 6574 654d  Servicer.DeleteM
-00000b20: 6174 6572 6961 6c69 7a61 7469 6f6e 4e29  aterializationN)
-00000b30: 0872 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
-00000b40: 7223 0000 0072 1100 0000 7214 0000 0072  r#...r....r....r
-00000b50: 1700 0000 721a 0000 0072 1d00 0000 721d  ....r....r....r.
-00000b60: 0000 0072 1d00 0000 721e 0000 0072 2400  ...r....r....r$.
-00000b70: 0000 2800 0000 730c 0000 0008 0004 0108  ..(...s.........
-00000b80: 0308 0b08 070c 0772 2400 0000 6302 0000  .......r$...c...
-00000b90: 0000 0000 0000 0000 0004 0000 0008 0000  ................
-00000ba0: 0043 0000 0073 8200 0000 7400 6a01 7c00  .C...s....t.j.|.
-00000bb0: 6a02 7403 6a04 6a05 7403 6a06 6a07 6401  j.t.j.j.t.j.j.d.
-00000bc0: 8d03 7400 6a01 7c00 6a08 7403 6a09 6a05  ..t.j.|.j.t.j.j.
-00000bd0: 7403 6a0a 6a07 6401 8d03 7400 6a01 7c00  t.j.j.d...t.j.|.
-00000be0: 6a0b 7403 6a0c 6a05 7403 6a0d 6a07 6401  j.t.j.j.t.j.j.d.
-00000bf0: 8d03 7400 6a01 7c00 6a0e 7403 6a0f 6a05  ..t.j.|.j.t.j.j.
-00000c00: 7403 6a10 6a07 6401 8d03 6402 9c04 7d02  t.j.j.d...d...}.
-00000c10: 7400 a011 6403 7c02 a102 7d03 7c01 a012  t...d.|...}.|...
-00000c20: 7c03 6601 a101 0100 6400 5300 2904 4e29  |.f.....d.S.).N)
-00000c30: 02da 1472 6571 7565 7374 5f64 6573 6572  ...request_deser
-00000c40: 6961 6c69 7a65 72da 1372 6573 706f 6e73  ializer..respons
-00000c50: 655f 7365 7269 616c 697a 6572 2904 7211  e_serializer).r.
-00000c60: 0000 0072 1400 0000 7217 0000 0072 1a00  ...r....r....r..
-00000c70: 0000 7a2e 6b61 736b 6164 612e 6b61 736b  ..z.kaskada.kask
-00000c80: 6164 612e 7631 616c 7068 612e 4d61 7465  ada.v1alpha.Mate
-00000c90: 7269 616c 697a 6174 696f 6e53 6572 7669  rializationServi
-00000ca0: 6365 2913 7229 0000 00da 1e75 6e61 7279  ce).r).....unary
-00000cb0: 5f75 6e61 7279 5f72 7063 5f6d 6574 686f  _unary_rpc_metho
-00000cc0: 645f 6861 6e64 6c65 7272 1100 0000 720c  d_handlerr....r.
-00000cd0: 0000 0072 0d00 0000 7210 0000 0072 0f00  ...r....r....r..
-00000ce0: 0000 720e 0000 0072 1400 0000 7212 0000  ..r....r....r...
-00000cf0: 0072 1300 0000 7217 0000 0072 1500 0000  .r....r....r....
-00000d00: 7216 0000 0072 1a00 0000 7218 0000 0072  r....r....r....r
-00000d10: 1900 0000 da1f 6d65 7468 6f64 5f68 616e  ......method_han
-00000d20: 646c 6572 735f 6765 6e65 7269 635f 6861  dlers_generic_ha
-00000d30: 6e64 6c65 72da 1861 6464 5f67 656e 6572  ndler..add_gener
-00000d40: 6963 5f72 7063 5f68 616e 646c 6572 7329  ic_rpc_handlers)
-00000d50: 04da 0873 6572 7669 6365 72da 0673 6572  ...servicer..ser
-00000d60: 7665 72da 1372 7063 5f6d 6574 686f 645f  ver..rpc_method_
-00000d70: 6861 6e64 6c65 7273 da0f 6765 6e65 7269  handlers..generi
-00000d80: 635f 6861 6e64 6c65 7272 1d00 0000 721d  c_handlerr....r.
-00000d90: 0000 0072 1e00 0000 da2c 6164 645f 4d61  ...r.....,add_Ma
-00000da0: 7465 7269 616c 697a 6174 696f 6e53 6572  terializationSer
-00000db0: 7669 6365 5365 7276 6963 6572 5f74 6f5f  viceServicer_to_
-00000dc0: 7365 7276 6572 4d00 0000 7332 0000 0004  serverM...s2....
-00000dd0: 0204 0106 0106 0104 fd04 0504 0106 0106  ................
-00000de0: 0104 fd04 0504 0106 0106 0104 fd04 0504  ................
-00000df0: 0106 0106 0104 fd06 f004 1604 0104 ff10  ................
-00000e00: 0272 3b00 0000 6300 0000 0000 0000 0000  .r;...c.........
-00000e10: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-00000e20: 8800 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00000e30: 6504 0902 0903 0903 0904 0903 0903 0903  e...............
-00000e40: 0903 640d 6405 6406 8401 8301 5a05 6504  ..d.d.d.....Z.e.
-00000e50: 0902 0903 0903 0904 0903 0903 0903 0903  ................
-00000e60: 640d 6407 6408 8401 8301 5a06 6504 0902  d.d.d.....Z.e...
-00000e70: 0903 0903 0904 0903 0903 0903 0903 640d  ..............d.
-00000e80: 6409 640a 8401 8301 5a07 6504 0902 0903  d.d.....Z.e.....
-00000e90: 0903 0904 0903 0903 0903 0903 640d 640b  ............d.d.
-00000ea0: 640c 8401 8301 5a08 6403 5300 290e da16  d.....Z.d.S.)...
-00000eb0: 4d61 7465 7269 616c 697a 6174 696f 6e53  MaterializationS
-00000ec0: 6572 7669 6365 7204 0000 0072 1d00 0000  ervicer....r....
-00000ed0: 4e46 630a 0000 0000 0000 0000 0000 000a  NFc.............
-00000ee0: 0000 000f 0000 0043 0000 00f3 2c00 0000  .......C....,...
-00000ef0: 7400 6a01 a002 7c00 7c01 6401 7403 6a04  t.j...|.|.d.t.j.
-00000f00: 6a05 7403 6a06 6a07 7c02 7c03 7c05 7c04  j.t.j.j.|.|.|.|.
-00000f10: 7c06 7c07 7c08 7c09 a10d 5300 2902 4e72  |.|.|.|...S.).Nr
-00000f20: 0500 0000 2908 7229 0000 00da 0c65 7870  ....).r).....exp
-00000f30: 6572 696d 656e 7461 6c72 0b00 0000 720c  erimentalr....r.
-00000f40: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
-00000f50: 0000 7210 0000 00a9 0a72 2f00 0000 da06  ..r......r/.....
-00000f60: 7461 7267 6574 da07 6f70 7469 6f6e 73da  target..options.
-00000f70: 1363 6861 6e6e 656c 5f63 7265 6465 6e74  .channel_credent
-00000f80: 6961 6c73 da10 6361 6c6c 5f63 7265 6465  ials..call_crede
-00000f90: 6e74 6961 6c73 da08 696e 7365 6375 7265  ntials..insecure
-00000fa0: da0b 636f 6d70 7265 7373 696f 6eda 0e77  ..compression..w
-00000fb0: 6169 745f 666f 725f 7265 6164 79da 0774  ait_for_ready..t
-00000fc0: 696d 656f 7574 da08 6d65 7461 6461 7461  imeout..metadata
-00000fd0: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000fe0: 1100 0000 6e00 0000 f30c 0000 000c 0b06  ....n...........
-00000ff0: 0106 0104 010c 0104 fc7a 2b4d 6174 6572  .........z+Mater
-00001000: 6961 6c69 7a61 7469 6f6e 5365 7276 6963  ializationServic
-00001010: 652e 4c69 7374 4d61 7465 7269 616c 697a  e.ListMaterializ
-00001020: 6174 696f 6e73 630a 0000 0000 0000 0000  ationsc.........
-00001030: 0000 000a 0000 000f 0000 0043 0000 0072  ...........C...r
-00001040: 3d00 0000 2902 4e72 0800 0000 2908 7229  =...).Nr....).r)
-00001050: 0000 0072 3e00 0000 720b 0000 0072 0c00  ...r>...r....r..
-00001060: 0000 7212 0000 0072 0e00 0000 7213 0000  ..r....r....r...
-00001070: 0072 1000 0000 723f 0000 0072 1d00 0000  .r....r?...r....
-00001080: 721d 0000 0072 1e00 0000 7214 0000 007f  r....r....r.....
-00001090: 0000 0072 4900 0000 7a29 4d61 7465 7269  ...rI...z)Materi
-000010a0: 616c 697a 6174 696f 6e53 6572 7669 6365  alizationService
-000010b0: 2e47 6574 4d61 7465 7269 616c 697a 6174  .GetMaterializat
-000010c0: 696f 6e63 0a00 0000 0000 0000 0000 0000  ionc............
-000010d0: 0a00 0000 0f00 0000 4300 0000 723d 0000  ........C...r=..
-000010e0: 0029 024e 7209 0000 0029 0872 2900 0000  .).Nr....).r)...
-000010f0: 723e 0000 0072 0b00 0000 720c 0000 0072  r>...r....r....r
-00001100: 1500 0000 720e 0000 0072 1600 0000 7210  ....r....r....r.
-00001110: 0000 0072 3f00 0000 721d 0000 0072 1d00  ...r?...r....r..
-00001120: 0000 721e 0000 0072 1700 0000 9000 0000  ..r....r........
-00001130: 7249 0000 007a 2c4d 6174 6572 6961 6c69  rI...z,Materiali
-00001140: 7a61 7469 6f6e 5365 7276 6963 652e 4372  zationService.Cr
-00001150: 6561 7465 4d61 7465 7269 616c 697a 6174  eateMaterializat
-00001160: 696f 6e63 0a00 0000 0000 0000 0000 0000  ionc............
-00001170: 0a00 0000 0f00 0000 4300 0000 723d 0000  ........C...r=..
-00001180: 0029 024e 720a 0000 0029 0872 2900 0000  .).Nr....).r)...
-00001190: 723e 0000 0072 0b00 0000 720c 0000 0072  r>...r....r....r
-000011a0: 1800 0000 720e 0000 0072 1900 0000 7210  ....r....r....r.
-000011b0: 0000 0072 3f00 0000 721d 0000 0072 1d00  ...r?...r....r..
-000011c0: 0000 721e 0000 0072 1a00 0000 a100 0000  ..r....r........
-000011d0: 7249 0000 007a 2c4d 6174 6572 6961 6c69  rI...z,Materiali
-000011e0: 7a61 7469 6f6e 5365 7276 6963 652e 4465  zationService.De
-000011f0: 6c65 7465 4d61 7465 7269 616c 697a 6174  leteMaterializat
-00001200: 696f 6e29 0872 1d00 0000 4e4e 464e 4e4e  ion).r....NNFNNN
-00001210: 4e29 0972 2000 0000 7221 0000 0072 2200  N).r ...r!...r".
-00001220: 0000 7223 0000 00da 0c73 7461 7469 636d  ..r#.....staticm
-00001230: 6574 686f 6472 1100 0000 7214 0000 0072  ethodr....r....r
-00001240: 1700 0000 721a 0000 0072 1d00 0000 721d  ....r....r....r.
-00001250: 0000 0072 1d00 0000 721e 0000 0072 3c00  ...r....r....r<.
-00001260: 0000 6a00 0000 7354 0000 0008 0004 0102  ..j...sT........
-00001270: 0302 0302 0102 0102 0102 0102 0102 0102  ................
-00001280: 010c f702 1002 0302 0102 0102 0102 0102  ................
-00001290: 0102 0102 010c f702 1002 0302 0102 0102  ................
-000012a0: 0102 0102 0102 0102 010c f702 1002 0302  ................
-000012b0: 0102 0102 0102 0102 0102 0102 0110 f772  ...............r
-000012c0: 3c00 0000 290a 7223 0000 0072 2900 0000  <...).r#...r)...
-000012d0: da17 6b61 736b 6164 612e 6b61 736b 6164  ..kaskada.kaskad
-000012e0: 612e 7631 616c 7068 6172 0200 0000 720c  a.v1alphar....r.
-000012f0: 0000 00da 066f 626a 6563 7472 0300 0000  .....objectr....
-00001300: 7224 0000 0072 3b00 0000 723c 0000 0072  r$...r;...r<...r
-00001310: 1d00 0000 721d 0000 0072 1d00 0000 721e  ....r....r....r.
-00001320: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001330: 0073 0e00 0000 0401 0801 0c02 1003 1020  .s............. 
-00001340: 0825 141d                                .%..
+00000550: 6861 6e6e 656c a900 721d 0000 00fa 442f  hannel..r.....D/
+00000560: 7372 632f 7372 632f 6b61 736b 6164 612f  src/src/kaskada/
+00000570: 6b61 736b 6164 612f 7631 616c 7068 612f  kaskada/v1alpha/
+00000580: 6d61 7465 7269 616c 697a 6174 696f 6e5f  materialization_
+00000590: 7365 7276 6963 655f 7062 325f 6772 7063  service_pb2_grpc
+000005a0: 2e70 79da 085f 5f69 6e69 745f 5f0c 0000  .py..__init__...
+000005b0: 0073 2800 0000 0006 0401 0201 0601 06fd  .s(.............
+000005c0: 0805 0401 0201 0601 06fd 0805 0401 0201  ................
+000005d0: 0601 06fd 0805 0401 0201 0601 06fd 7a23  ..............z#
+000005e0: 4d61 7465 7269 616c 697a 6174 696f 6e53  MaterializationS
+000005f0: 6572 7669 6365 5374 7562 2e5f 5f69 6e69  erviceStub.__ini
+00000600: 745f 5f4e 2905 da08 5f5f 6e61 6d65 5f5f  t__N)...__name__
+00000610: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000620: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00000630: 635f 5f72 1f00 0000 721d 0000 0072 1d00  c__r....r....r..
+00000640: 0000 721d 0000 0072 1e00 0000 7203 0000  ..r....r....r...
+00000650: 0008 0000 0073 0400 0000 0801 0403 7203  .....s........r.
+00000660: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000670: 0000 0000 0200 0000 4000 0000 7330 0000  ........@...s0..
+00000680: 0065 005a 0164 005a 0264 015a 0364 0264  .e.Z.d.Z.d.Z.d.d
+00000690: 0384 005a 0464 0464 0584 005a 0564 0664  ...Z.d.d...Z.d.d
+000006a0: 0784 005a 0664 0864 0984 005a 0764 0a53  ...Z.d.d...Z.d.S
+000006b0: 0029 0bda 1e4d 6174 6572 6961 6c69 7a61  .)...Materializa
+000006c0: 7469 6f6e 5365 7276 6963 6553 6572 7669  tionServiceServi
+000006d0: 6365 7272 0400 0000 6303 0000 0000 0000  cerr....c.......
+000006e0: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
+000006f0: 0073 2400 0000 7c02 a000 7401 6a02 6a03  .s$...|...t.j.j.
+00000700: a101 0100 7c02 a004 6401 a101 0100 7405  ....|...d.....t.
+00000710: 6401 8301 8201 6402 5300 2903 7ae4 4c69  d.....d.S.).z.Li
+00000720: 7374 7320 6d61 7465 7269 616c 697a 6174  sts materializat
+00000730: 696f 6e73 2e0a 0a20 2020 2020 2020 2054  ions...        T
+00000740: 6865 2072 6573 706f 6e73 6520 696e 636c  he response incl
+00000750: 7564 6573 2061 6c6c 204d 6174 6572 6961  udes all Materia
+00000760: 6c69 7a61 7469 6f6e 7320 6465 6669 6e65  lizations define
+00000770: 6420 666f 7220 7468 6520 4b61 736b 6164  d for the Kaskad
+00000780: 610a 2020 2020 2020 2020 6163 636f 756e  a.        accoun
+00000790: 742e 2049 6620 6120 7365 6172 6368 2073  t. If a search s
+000007a0: 7472 696e 6720 6973 2070 726f 7669 6465  tring is provide
+000007b0: 642c 206f 6e6c 7920 4d61 7465 7269 616c  d, only Material
+000007c0: 697a 6174 696f 6e73 0a20 2020 2020 2020  izations.       
+000007d0: 206d 6174 6368 696e 6720 7468 6520 7365   matching the se
+000007e0: 6172 6368 2073 7472 696e 6720 6172 6520  arch string are 
+000007f0: 7265 7475 726e 6564 2e0a 2020 2020 2020  returned..      
+00000800: 2020 fa17 4d65 7468 6f64 206e 6f74 2069    ..Method not i
+00000810: 6d70 6c65 6d65 6e74 6564 214e a906 da08  mplemented!N....
+00000820: 7365 745f 636f 6465 da04 6772 7063 da0a  set_code..grpc..
+00000830: 5374 6174 7573 436f 6465 da0d 554e 494d  StatusCode..UNIM
+00000840: 504c 454d 454e 5445 44da 0b73 6574 5f64  PLEMENTED..set_d
+00000850: 6574 6169 6c73 da13 4e6f 7449 6d70 6c65  etails..NotImple
+00000860: 6d65 6e74 6564 4572 726f 72a9 0372 1b00  mentedError..r..
+00000870: 0000 da07 7265 7175 6573 74da 0763 6f6e  ....request..con
+00000880: 7465 7874 721d 0000 0072 1d00 0000 721e  textr....r....r.
+00000890: 0000 0072 1100 0000 2c00 0000 7306 0000  ...r....,...s...
+000008a0: 0000 070e 010a 017a 334d 6174 6572 6961  .......z3Materia
+000008b0: 6c69 7a61 7469 6f6e 5365 7276 6963 6553  lizationServiceS
+000008c0: 6572 7669 6365 722e 4c69 7374 4d61 7465  ervicer.ListMate
+000008d0: 7269 616c 697a 6174 696f 6e73 6303 0000  rializationsc...
+000008e0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+000008f0: 0043 0000 0073 2400 0000 7c02 a000 7401  .C...s$...|...t.
+00000900: 6a02 6a03 a101 0100 7c02 a004 6401 a101  j.j.....|...d...
+00000910: 0100 7405 6401 8301 8201 6402 5300 2903  ..t.d.....d.S.).
+00000920: 7a20 4765 7473 2061 206d 6174 6572 6961  z Gets a materia
+00000930: 6c69 7a61 7469 6f6e 2e0a 2020 2020 2020  lization..      
+00000940: 2020 7225 0000 004e 7226 0000 0072 2d00    r%...Nr&...r-.
+00000950: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00000960: 0072 1400 0000 3700 0000 7306 0000 0000  .r....7...s.....
+00000970: 030e 010a 017a 314d 6174 6572 6961 6c69  .....z1Materiali
+00000980: 7a61 7469 6f6e 5365 7276 6963 6553 6572  zationServiceSer
+00000990: 7669 6365 722e 4765 744d 6174 6572 6961  vicer.GetMateria
+000009a0: 6c69 7a61 7469 6f6e 6303 0000 0000 0000  lizationc.......
+000009b0: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
+000009c0: 0073 2400 0000 7c02 a000 7401 6a02 6a03  .s$...|...t.j.j.
+000009d0: a101 0100 7c02 a004 6401 a101 0100 7405  ....|...d.....t.
+000009e0: 6401 8301 8201 6402 5300 2903 7a23 4372  d.....d.S.).z#Cr
+000009f0: 6561 7465 7320 6120 6d61 7465 7269 616c  eates a material
+00000a00: 697a 6174 696f 6e2e 0a20 2020 2020 2020  ization..       
+00000a10: 2072 2500 0000 4e72 2600 0000 722d 0000   r%...Nr&...r-..
+00000a20: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00000a30: 7217 0000 003e 0000 0073 0600 0000 0003  r....>...s......
+00000a40: 0e01 0a01 7a34 4d61 7465 7269 616c 697a  ....z4Materializ
+00000a50: 6174 696f 6e53 6572 7669 6365 5365 7276  ationServiceServ
+00000a60: 6963 6572 2e43 7265 6174 654d 6174 6572  icer.CreateMater
+00000a70: 6961 6c69 7a61 7469 6f6e 6303 0000 0000  ializationc.....
+00000a80: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
+00000a90: 0000 0073 2400 0000 7c02 a000 7401 6a02  ...s$...|...t.j.
+00000aa0: 6a03 a101 0100 7c02 a004 6401 a101 0100  j.....|...d.....
+00000ab0: 7405 6401 8301 8201 6402 5300 2903 7a41  t.d.....d.S.).zA
+00000ac0: 4465 6c65 7465 7320 6120 6d61 7465 7269  Deletes a materi
+00000ad0: 616c 697a 6174 696f 6e20 616e 6420 616e  alization and an
+00000ae0: 7920 6576 656e 7473 206c 6f61 6465 6420  y events loaded 
+00000af0: 696e 746f 2069 742e 0a20 2020 2020 2020  into it..       
+00000b00: 2072 2500 0000 4e72 2600 0000 722d 0000   r%...Nr&...r-..
+00000b10: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00000b20: 721a 0000 0045 0000 0073 0600 0000 0003  r....E...s......
+00000b30: 0e01 0a01 7a34 4d61 7465 7269 616c 697a  ....z4Materializ
+00000b40: 6174 696f 6e53 6572 7669 6365 5365 7276  ationServiceServ
+00000b50: 6963 6572 2e44 656c 6574 654d 6174 6572  icer.DeleteMater
+00000b60: 6961 6c69 7a61 7469 6f6e 4e29 0872 2000  ializationN).r .
+00000b70: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
+00000b80: 0072 1100 0000 7214 0000 0072 1700 0000  .r....r....r....
+00000b90: 721a 0000 0072 1d00 0000 721d 0000 0072  r....r....r....r
+00000ba0: 1d00 0000 721e 0000 0072 2400 0000 2800  ....r....r$...(.
+00000bb0: 0000 730a 0000 0008 0104 0308 0b08 0708  ..s.............
+00000bc0: 0772 2400 0000 6302 0000 0000 0000 0000  .r$...c.........
+00000bd0: 0000 0004 0000 0008 0000 0043 0000 0073  ...........C...s
+00000be0: 8200 0000 7400 6a01 7c00 6a02 7403 6a04  ....t.j.|.j.t.j.
+00000bf0: 6a05 7403 6a06 6a07 6401 8d03 7400 6a01  j.t.j.j.d...t.j.
+00000c00: 7c00 6a08 7403 6a09 6a05 7403 6a0a 6a07  |.j.t.j.j.t.j.j.
+00000c10: 6401 8d03 7400 6a01 7c00 6a0b 7403 6a0c  d...t.j.|.j.t.j.
+00000c20: 6a05 7403 6a0d 6a07 6401 8d03 7400 6a01  j.t.j.j.d...t.j.
+00000c30: 7c00 6a0e 7403 6a0f 6a05 7403 6a10 6a07  |.j.t.j.j.t.j.j.
+00000c40: 6401 8d03 6402 9c04 7d02 7400 a011 6403  d...d...}.t...d.
+00000c50: 7c02 a102 7d03 7c01 a012 7c03 6601 a101  |...}.|...|.f...
+00000c60: 0100 6400 5300 2904 4e29 02da 1472 6571  ..d.S.).N)...req
+00000c70: 7565 7374 5f64 6573 6572 6961 6c69 7a65  uest_deserialize
+00000c80: 72da 1372 6573 706f 6e73 655f 7365 7269  r..response_seri
+00000c90: 616c 697a 6572 2904 7211 0000 0072 1400  alizer).r....r..
+00000ca0: 0000 7217 0000 0072 1a00 0000 7a2e 6b61  ..r....r....z.ka
+00000cb0: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
+00000cc0: 616c 7068 612e 4d61 7465 7269 616c 697a  alpha.Materializ
+00000cd0: 6174 696f 6e53 6572 7669 6365 2913 7228  ationService).r(
+00000ce0: 0000 00da 1e75 6e61 7279 5f75 6e61 7279  .....unary_unary
+00000cf0: 5f72 7063 5f6d 6574 686f 645f 6861 6e64  _rpc_method_hand
+00000d00: 6c65 7272 1100 0000 720c 0000 0072 0d00  lerr....r....r..
+00000d10: 0000 7210 0000 0072 0f00 0000 720e 0000  ..r....r....r...
+00000d20: 0072 1400 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000d30: 7217 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000d40: 1a00 0000 7218 0000 0072 1900 0000 da1f  ....r....r......
+00000d50: 6d65 7468 6f64 5f68 616e 646c 6572 735f  method_handlers_
+00000d60: 6765 6e65 7269 635f 6861 6e64 6c65 72da  generic_handler.
+00000d70: 1861 6464 5f67 656e 6572 6963 5f72 7063  .add_generic_rpc
+00000d80: 5f68 616e 646c 6572 7329 045a 0873 6572  _handlers).Z.ser
+00000d90: 7669 6365 72da 0673 6572 7665 725a 1372  vicer..serverZ.r
+00000da0: 7063 5f6d 6574 686f 645f 6861 6e64 6c65  pc_method_handle
+00000db0: 7273 da0f 6765 6e65 7269 635f 6861 6e64  rs..generic_hand
+00000dc0: 6c65 7272 1d00 0000 721d 0000 0072 1e00  lerr....r....r..
+00000dd0: 0000 da2c 6164 645f 4d61 7465 7269 616c  ...,add_Material
+00000de0: 697a 6174 696f 6e53 6572 7669 6365 5365  izationServiceSe
+00000df0: 7276 6963 6572 5f74 6f5f 7365 7276 6572  rvicer_to_server
+00000e00: 4d00 0000 7332 0000 0000 0204 0104 0106  M...s2..........
+00000e10: 0106 fd04 0504 0104 0106 0106 fd04 0504  ................
+00000e20: 0104 0106 0106 fd04 0504 0104 0106 0106  ................
+00000e30: fd04 f006 1604 0104 ff04 0272 3700 0000  ...........r7...
+00000e40: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000e50: 0009 0000 0040 0000 0073 4800 0000 6500  .....@...sH...e.
+00000e60: 5a01 6400 5a02 6401 5a03 6504 640d 6405  Z.d.Z.d.Z.e.d.d.
+00000e70: 6406 8401 8301 5a05 6504 640e 6407 6408  d.....Z.e.d.d.d.
+00000e80: 8401 8301 5a06 6504 640f 6409 640a 8401  ....Z.e.d.d.d...
+00000e90: 8301 5a07 6504 6410 640b 640c 8401 8301  ..Z.e.d.d.d.....
+00000ea0: 5a08 6403 5300 2911 da16 4d61 7465 7269  Z.d.S.)...Materi
+00000eb0: 616c 697a 6174 696f 6e53 6572 7669 6365  alizationService
+00000ec0: 7204 0000 0072 1d00 0000 4e46 630a 0000  r....r....NFc...
+00000ed0: 0000 0000 0000 0000 000a 0000 000f 0000  ................
+00000ee0: 0043 0000 0073 2c00 0000 7400 6a01 a002  .C...s,...t.j...
+00000ef0: 7c00 7c01 6401 7403 6a04 6a05 7403 6a06  |.|.d.t.j.j.t.j.
+00000f00: 6a07 7c02 7c03 7c05 7c04 7c06 7c07 7c08  j.|.|.|.|.|.|.|.
+00000f10: 7c09 a10d 5300 2902 4e72 0500 0000 2908  |...S.).Nr....).
+00000f20: 7228 0000 00da 0c65 7870 6572 696d 656e  r(.....experimen
+00000f30: 7461 6c72 0b00 0000 720c 0000 0072 0d00  talr....r....r..
+00000f40: 0000 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00000f50: 00a9 0a72 2e00 0000 da06 7461 7267 6574  ...r......target
+00000f60: da07 6f70 7469 6f6e 73da 1363 6861 6e6e  ..options..chann
+00000f70: 656c 5f63 7265 6465 6e74 6961 6c73 da10  el_credentials..
+00000f80: 6361 6c6c 5f63 7265 6465 6e74 6961 6c73  call_credentials
+00000f90: 5a08 696e 7365 6375 7265 da0b 636f 6d70  Z.insecure..comp
+00000fa0: 7265 7373 696f 6eda 0e77 6169 745f 666f  ression..wait_fo
+00000fb0: 725f 7265 6164 79da 0774 696d 656f 7574  r_ready..timeout
+00000fc0: da08 6d65 7461 6461 7461 721d 0000 0072  ..metadatar....r
+00000fd0: 1d00 0000 721e 0000 0072 1100 0000 6e00  ....r....r....n.
+00000fe0: 0000 730c 0000 0000 0b0c 0106 0106 0104  ..s.............
+00000ff0: 010c fc7a 2b4d 6174 6572 6961 6c69 7a61  ...z+Materializa
+00001000: 7469 6f6e 5365 7276 6963 652e 4c69 7374  tionService.List
+00001010: 4d61 7465 7269 616c 697a 6174 696f 6e73  Materializations
+00001020: 630a 0000 0000 0000 0000 0000 000a 0000  c...............
+00001030: 000f 0000 0043 0000 0073 2c00 0000 7400  .....C...s,...t.
+00001040: 6a01 a002 7c00 7c01 6401 7403 6a04 6a05  j...|.|.d.t.j.j.
+00001050: 7403 6a06 6a07 7c02 7c03 7c05 7c04 7c06  t.j.j.|.|.|.|.|.
+00001060: 7c07 7c08 7c09 a10d 5300 2902 4e72 0800  |.|.|...S.).Nr..
+00001070: 0000 2908 7228 0000 0072 3900 0000 720b  ..).r(...r9...r.
+00001080: 0000 0072 0c00 0000 7212 0000 0072 0e00  ...r....r....r..
+00001090: 0000 7213 0000 0072 1000 0000 723a 0000  ..r....r....r:..
+000010a0: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+000010b0: 7214 0000 007f 0000 0073 0c00 0000 000b  r........s......
+000010c0: 0c01 0601 0601 0401 0cfc 7a29 4d61 7465  ..........z)Mate
+000010d0: 7269 616c 697a 6174 696f 6e53 6572 7669  rializationServi
+000010e0: 6365 2e47 6574 4d61 7465 7269 616c 697a  ce.GetMaterializ
+000010f0: 6174 696f 6e63 0a00 0000 0000 0000 0000  ationc..........
+00001100: 0000 0a00 0000 0f00 0000 4300 0000 732c  ..........C...s,
+00001110: 0000 0074 006a 01a0 027c 007c 0164 0174  ...t.j...|.|.d.t
+00001120: 036a 046a 0574 036a 066a 077c 027c 037c  .j.j.t.j.j.|.|.|
+00001130: 057c 047c 067c 077c 087c 09a1 0d53 0029  .|.|.|.|.|...S.)
+00001140: 024e 7209 0000 0029 0872 2800 0000 7239  .Nr....).r(...r9
+00001150: 0000 0072 0b00 0000 720c 0000 0072 1500  ...r....r....r..
+00001160: 0000 720e 0000 0072 1600 0000 7210 0000  ..r....r....r...
+00001170: 0072 3a00 0000 721d 0000 0072 1d00 0000  .r:...r....r....
+00001180: 721e 0000 0072 1700 0000 9000 0000 730c  r....r........s.
+00001190: 0000 0000 0b0c 0106 0106 0104 010c fc7a  ...............z
+000011a0: 2c4d 6174 6572 6961 6c69 7a61 7469 6f6e  ,Materialization
+000011b0: 5365 7276 6963 652e 4372 6561 7465 4d61  Service.CreateMa
+000011c0: 7465 7269 616c 697a 6174 696f 6e63 0a00  terializationc..
+000011d0: 0000 0000 0000 0000 0000 0a00 0000 0f00  ................
+000011e0: 0000 4300 0000 732c 0000 0074 006a 01a0  ..C...s,...t.j..
+000011f0: 027c 007c 0164 0174 036a 046a 0574 036a  .|.|.d.t.j.j.t.j
+00001200: 066a 077c 027c 037c 057c 047c 067c 077c  .j.|.|.|.|.|.|.|
+00001210: 087c 09a1 0d53 0029 024e 720a 0000 0029  .|...S.).Nr....)
+00001220: 0872 2800 0000 7239 0000 0072 0b00 0000  .r(...r9...r....
+00001230: 720c 0000 0072 1800 0000 720e 0000 0072  r....r....r....r
+00001240: 1900 0000 7210 0000 0072 3a00 0000 721d  ....r....r:...r.
+00001250: 0000 0072 1d00 0000 721e 0000 0072 1a00  ...r....r....r..
+00001260: 0000 a100 0000 730c 0000 0000 0b0c 0106  ......s.........
+00001270: 0106 0104 010c fc7a 2c4d 6174 6572 6961  .......z,Materia
+00001280: 6c69 7a61 7469 6f6e 5365 7276 6963 652e  lizationService.
+00001290: 4465 6c65 7465 4d61 7465 7269 616c 697a  DeleteMaterializ
+000012a0: 6174 696f 6e29 0872 1d00 0000 4e4e 464e  ation).r....NNFN
+000012b0: 4e4e 4e29 0872 1d00 0000 4e4e 464e 4e4e  NNN).r....NNFNNN
+000012c0: 4e29 0872 1d00 0000 4e4e 464e 4e4e 4e29  N).r....NNFNNNN)
+000012d0: 0872 1d00 0000 4e4e 464e 4e4e 4e29 0972  .r....NNFNNNN).r
+000012e0: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
+000012f0: 0000 00da 0c73 7461 7469 636d 6574 686f  .....staticmetho
+00001300: 6472 1100 0000 7214 0000 0072 1700 0000  dr....r....r....
+00001310: 721a 0000 0072 1d00 0000 721d 0000 0072  r....r....r....r
+00001320: 1d00 0000 721e 0000 0072 3800 0000 6a00  ....r....r8...j.
+00001330: 0000 7352 0000 0008 0104 0302 0300 0100  ..sR............
+00001340: 0100 0100 0100 0100 0100 0100 f70c 1002  ................
+00001350: 0300 0100 0100 0100 0100 0100 0100 0100  ................
+00001360: f70c 1002 0300 0100 0100 0100 0100 0100  ................
+00001370: 0100 0100 f70c 1002 0300 0100 0100 0100  ................
+00001380: 0100 0100 0100 0100 f772 3800 0000 290a  .........r8...).
+00001390: 7223 0000 0072 2800 0000 da17 6b61 736b  r#...r(.....kask
+000013a0: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
+000013b0: 7068 6172 0200 0000 720c 0000 00da 066f  phar....r......o
+000013c0: 626a 6563 7472 0300 0000 7224 0000 0072  bjectr....r$...r
+000013d0: 3700 0000 7238 0000 0072 1d00 0000 721d  7...r8...r....r.
+000013e0: 0000 0072 1d00 0000 721e 0000 00da 083c  ...r....r......<
+000013f0: 6d6f 6475 6c65 3e02 0000 0073 0c00 0000  module>....s....
+00001400: 0401 0802 0c03 1020 1025 081d            ....... .%..
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/options_pb2.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/options_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 1846 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,94 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 3607 0000  o.........5d6...
+00000000: 610d 0d0a 0000 0000 2038 4164 3607 0000  a....... 8Ad6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
 00000070: a00c a100 5a0d 6401 6407 6c01 6d0e 5a0f  ....Z.d.d.l.m.Z.
 00000080: 0100 6505 a00c a100 a010 6408 a101 5a11  ..e.......d...Z.
 00000090: 6409 5a12 6511 6a13 640a 1900 5a14 6503  d.Z.e.j.d...Z.e.
-000000a0: 6a15 640b 6b02 724b 650f 6a16 a017 6514  j.d.k.rKe.j...e.
+000000a0: 6a15 640b 6b02 7292 650f 6a16 a017 6514  j.d.k.r.e.j...e.
 000000b0: a101 0100 640c 6511 5f18 640d 6511 5f19  ....d.e._.d.e._.
-000000c0: 640c 5300 640c 5300 290e 7a1f 4765 6e65  d.S.d.S.).z.Gene
-000000d0: 7261 7465 6420 7072 6f74 6f63 6f6c 2062  rated protocol b
-000000e0: 7566 6665 7220 636f 6465 2ee9 0000 0000  uffer code......
-000000f0: 2901 da0a 6465 7363 7269 7074 6f72 2901  )...descriptor).
-00000100: da0f 6465 7363 7269 7074 6f72 5f70 6f6f  ..descriptor_poo
-00000110: 6c29 01da 076d 6573 7361 6765 2901 da0a  l)...message)...
-00000120: 7265 666c 6563 7469 6f6e 2901 da0f 7379  reflection)...sy
-00000130: 6d62 6f6c 5f64 6174 6162 6173 6529 01da  mbol_database)..
-00000140: 0e64 6573 6372 6970 746f 725f 7062 3273  .descriptor_pb2s
-00000150: a801 0000 0a25 6b61 736b 6164 612f 6b61  .....%kaskada/ka
-00000160: 736b 6164 612f 7631 616c 7068 612f 6f70  skada/v1alpha/op
-00000170: 7469 6f6e 732e 7072 6f74 6f12 176b 6173  tions.proto..kas
-00000180: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-00000190: 6c70 6861 1a20 676f 6f67 6c65 2f70 726f  lpha. google/pro
-000001a0: 746f 6275 662f 6465 7363 7269 7074 6f72  tobuf/descriptor
-000001b0: 2e70 726f 746f 3a3d 0a09 7365 6e73 6974  .proto:=..sensit
-000001c0: 6976 6512 1d2e 676f 6f67 6c65 2e70 726f  ive...google.pro
-000001d0: 746f 6275 662e 4669 656c 644f 7074 696f  tobuf.FieldOptio
-000001e0: 6e73 18d0 8603 2001 2808 5209 7365 6e73  ns.... .(.R.sens
-000001f0: 6974 6976 6542 fc01 0a1b 636f 6d2e 6b61  itiveB....com.ka
-00000200: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
-00000210: 616c 7068 6142 0c4f 7074 696f 6e73 5072  alphaB.OptionsPr
-00000220: 6f74 6f50 015a 5167 6974 6875 622e 636f  otoP.ZQgithub.co
-00000230: 6d2f 6b61 736b 6164 612d 6169 2f6b 6173  m/kaskada-ai/kas
-00000240: 6b61 6461 2f67 656e 2f70 726f 746f 2f67  kada/gen/proto/g
-00000250: 6f2f 6b61 736b 6164 612f 6b61 736b 6164  o/kaskada/kaskad
-00000260: 612f 7631 616c 7068 613b 6b61 736b 6164  a/v1alpha;kaskad
-00000270: 6176 3161 6c70 6861 a202 034b 4b58 aa02  av1alpha...KKX..
-00000280: 174b 6173 6b61 6461 2e4b 6173 6b61 6461  .Kaskada.Kaskada
-00000290: 2e56 3161 6c70 6861 ca02 174b 6173 6b61  .V1alpha...Kaska
-000002a0: 6461 5c4b 6173 6b61 6461 5c56 3161 6c70  da\Kaskada\V1alp
-000002b0: 6861 e202 234b 6173 6b61 6461 5c4b 6173  ha..#Kaskada\Kas
-000002c0: 6b61 6461 5c56 3161 6c70 6861 5c47 5042  kada\V1alpha\GPB
-000002d0: 4d65 7461 6461 7461 ea02 194b 6173 6b61  Metadata...Kaska
-000002e0: 6461 3a3a 4b61 736b 6164 613a 3a56 3161  da::Kaskada::V1a
-000002f0: 6c70 6861 6206 7072 6f74 6f33 6950 c300  lphab.proto3iP..
-00000300: 00da 0973 656e 7369 7469 7665 464e 73fc  ...sensitiveFNs.
-00000310: 0000 000a 1b63 6f6d 2e6b 6173 6b61 6461  .....com.kaskada
-00000320: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
-00000330: 420c 4f70 7469 6f6e 7350 726f 746f 5001  B.OptionsProtoP.
-00000340: 5a51 6769 7468 7562 2e63 6f6d 2f6b 6173  ZQgithub.com/kas
-00000350: 6b61 6461 2d61 692f 6b61 736b 6164 612f  kada-ai/kaskada/
-00000360: 6765 6e2f 7072 6f74 6f2f 676f 2f6b 6173  gen/proto/go/kas
-00000370: 6b61 6461 2f6b 6173 6b61 6461 2f76 3161  kada/kaskada/v1a
-00000380: 6c70 6861 3b6b 6173 6b61 6461 7631 616c  lpha;kaskadav1al
-00000390: 7068 61a2 0203 4b4b 58aa 0217 4b61 736b  pha...KKX...Kask
-000003a0: 6164 612e 4b61 736b 6164 612e 5631 616c  ada.Kaskada.V1al
-000003b0: 7068 61ca 0217 4b61 736b 6164 615c 4b61  pha...Kaskada\Ka
-000003c0: 736b 6164 615c 5631 616c 7068 61e2 0223  skada\V1alpha..#
-000003d0: 4b61 736b 6164 615c 4b61 736b 6164 615c  Kaskada\Kaskada\
-000003e0: 5631 616c 7068 615c 4750 424d 6574 6164  V1alpha\GPBMetad
-000003f0: 6174 61ea 0219 4b61 736b 6164 613a 3a4b  ata...Kaskada::K
-00000400: 6173 6b61 6461 3a3a 5631 616c 7068 6129  askada::V1alpha)
-00000410: 1ada 075f 5f64 6f63 5f5f da0f 676f 6f67  ...__doc__..goog
-00000420: 6c65 2e70 726f 746f 6275 6672 0200 0000  le.protobufr....
-00000430: da0b 5f64 6573 6372 6970 746f 7272 0300  .._descriptorr..
-00000440: 0000 da10 5f64 6573 6372 6970 746f 725f  ...._descriptor_
-00000450: 706f 6f6c 7204 0000 00da 085f 6d65 7373  poolr......_mess
-00000460: 6167 6572 0500 0000 da0b 5f72 6566 6c65  ager......_refle
-00000470: 6374 696f 6e72 0600 0000 da10 5f73 796d  ctionr......_sym
-00000480: 626f 6c5f 6461 7461 6261 7365 da07 4465  bol_database..De
-00000490: 6661 756c 74da 075f 7379 6d5f 6462 7207  fault.._sym_dbr.
-000004a0: 0000 00da 2767 6f6f 676c 655f 646f 745f  ....'google_dot_
-000004b0: 7072 6f74 6f62 7566 5f64 6f74 5f64 6573  protobuf_dot_des
-000004c0: 6372 6970 746f 725f 5f70 6232 da11 4164  criptor__pb2..Ad
-000004d0: 6453 6572 6961 6c69 7a65 6446 696c 65da  dSerializedFile.
-000004e0: 0a44 4553 4352 4950 544f 52da 1653 454e  .DESCRIPTOR..SEN
-000004f0: 5349 5449 5645 5f46 4945 4c44 5f4e 554d  SITIVE_FIELD_NUM
-00000500: 4245 52da 1265 7874 656e 7369 6f6e 735f  BER..extensions_
-00000510: 6279 5f6e 616d 6572 0800 0000 da12 5f55  by_namer......_U
-00000520: 5345 5f43 5f44 4553 4352 4950 544f 5253  SE_C_DESCRIPTORS
-00000530: da0c 4669 656c 644f 7074 696f 6e73 da11  ..FieldOptions..
-00000540: 5265 6769 7374 6572 4578 7465 6e73 696f  RegisterExtensio
-00000550: 6eda 085f 6f70 7469 6f6e 73da 135f 7365  n.._options.._se
-00000560: 7269 616c 697a 6564 5f6f 7074 696f 6e73  rialized_options
-00000570: a900 721c 0000 0072 1c00 0000 fa71 2f68  ..r....r.....q/h
-00000580: 6f6d 652f 7468 6572 6170 6f6e 2f52 6570  ome/therapon/Rep
-00000590: 6f73 2f47 6974 4875 622f 4b61 736b 6164  os/GitHub/Kaskad
-000005a0: 6141 492f 6b61 736b 6164 612f 7265 6c65  aAI/kaskada/rele
-000005b0: 6173 696e 672f 636c 6965 6e74 732f 7079  asing/clients/py
-000005c0: 7468 6f6e 2f73 7263 2f6b 6173 6b61 6461  thon/src/kaskada
-000005d0: 2f6b 6173 6b61 6461 2f76 3161 6c70 6861  /kaskada/v1alpha
-000005e0: 2f6f 7074 696f 6e73 5f70 6232 2e70 79da  /options_pb2.py.
-000005f0: 083c 6d6f 6475 6c65 3e01 0000 0073 2000  .<module>....s .
-00000600: 0000 0403 0c01 0c01 0c01 0c01 0c01 0803  ................
-00000610: 0c03 0e03 0403 0a01 0a02 0c01 0602 0a01  ................
-00000620: 04fc                                     ..
+000000c0: 640c 5300 290e 7a1f 4765 6e65 7261 7465  d.S.).z.Generate
+000000d0: 6420 7072 6f74 6f63 6f6c 2062 7566 6665  d protocol buffe
+000000e0: 7220 636f 6465 2ee9 0000 0000 2901 da0a  r code......)...
+000000f0: 6465 7363 7269 7074 6f72 2901 da0f 6465  descriptor)...de
+00000100: 7363 7269 7074 6f72 5f70 6f6f 6c29 01da  scriptor_pool)..
+00000110: 076d 6573 7361 6765 2901 da0a 7265 666c  .message)...refl
+00000120: 6563 7469 6f6e 2901 da0f 7379 6d62 6f6c  ection)...symbol
+00000130: 5f64 6174 6162 6173 6529 01da 0e64 6573  _database)...des
+00000140: 6372 6970 746f 725f 7062 3273 a801 0000  criptor_pb2s....
+00000150: 0a25 6b61 736b 6164 612f 6b61 736b 6164  .%kaskada/kaskad
+00000160: 612f 7631 616c 7068 612f 6f70 7469 6f6e  a/v1alpha/option
+00000170: 732e 7072 6f74 6f12 176b 6173 6b61 6461  s.proto..kaskada
+00000180: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00000190: 1a20 676f 6f67 6c65 2f70 726f 746f 6275  . google/protobu
+000001a0: 662f 6465 7363 7269 7074 6f72 2e70 726f  f/descriptor.pro
+000001b0: 746f 3a3d 0a09 7365 6e73 6974 6976 6512  to:=..sensitive.
+000001c0: 1d2e 676f 6f67 6c65 2e70 726f 746f 6275  ..google.protobu
+000001d0: 662e 4669 656c 644f 7074 696f 6e73 18d0  f.FieldOptions..
+000001e0: 8603 2001 2808 5209 7365 6e73 6974 6976  .. .(.R.sensitiv
+000001f0: 6542 fc01 0a1b 636f 6d2e 6b61 736b 6164  eB....com.kaskad
+00000200: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00000210: 6142 0c4f 7074 696f 6e73 5072 6f74 6f50  aB.OptionsProtoP
+00000220: 015a 5167 6974 6875 622e 636f 6d2f 6b61  .ZQgithub.com/ka
+00000230: 736b 6164 612d 6169 2f6b 6173 6b61 6461  skada-ai/kaskada
+00000240: 2f67 656e 2f70 726f 746f 2f67 6f2f 6b61  /gen/proto/go/ka
+00000250: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
+00000260: 616c 7068 613b 6b61 736b 6164 6176 3161  alpha;kaskadav1a
+00000270: 6c70 6861 a202 034b 4b58 aa02 174b 6173  lpha...KKX...Kas
+00000280: 6b61 6461 2e4b 6173 6b61 6461 2e56 3161  kada.Kaskada.V1a
+00000290: 6c70 6861 ca02 174b 6173 6b61 6461 5c4b  lpha...Kaskada\K
+000002a0: 6173 6b61 6461 5c56 3161 6c70 6861 e202  askada\V1alpha..
+000002b0: 234b 6173 6b61 6461 5c4b 6173 6b61 6461  #Kaskada\Kaskada
+000002c0: 5c56 3161 6c70 6861 5c47 5042 4d65 7461  \V1alpha\GPBMeta
+000002d0: 6461 7461 ea02 194b 6173 6b61 6461 3a3a  data...Kaskada::
+000002e0: 4b61 736b 6164 613a 3a56 3161 6c70 6861  Kaskada::V1alpha
+000002f0: 6206 7072 6f74 6f33 6950 c300 00da 0973  b.proto3iP.....s
+00000300: 656e 7369 7469 7665 464e 73fc 0000 000a  ensitiveFNs.....
+00000310: 1b63 6f6d 2e6b 6173 6b61 6461 2e6b 6173  .com.kaskada.kas
+00000320: 6b61 6461 2e76 3161 6c70 6861 420c 4f70  kada.v1alphaB.Op
+00000330: 7469 6f6e 7350 726f 746f 5001 5a51 6769  tionsProtoP.ZQgi
+00000340: 7468 7562 2e63 6f6d 2f6b 6173 6b61 6461  thub.com/kaskada
+00000350: 2d61 692f 6b61 736b 6164 612f 6765 6e2f  -ai/kaskada/gen/
+00000360: 7072 6f74 6f2f 676f 2f6b 6173 6b61 6461  proto/go/kaskada
+00000370: 2f6b 6173 6b61 6461 2f76 3161 6c70 6861  /kaskada/v1alpha
+00000380: 3b6b 6173 6b61 6461 7631 616c 7068 61a2  ;kaskadav1alpha.
+00000390: 0203 4b4b 58aa 0217 4b61 736b 6164 612e  ..KKX...Kaskada.
+000003a0: 4b61 736b 6164 612e 5631 616c 7068 61ca  Kaskada.V1alpha.
+000003b0: 0217 4b61 736b 6164 615c 4b61 736b 6164  ..Kaskada\Kaskad
+000003c0: 615c 5631 616c 7068 61e2 0223 4b61 736b  a\V1alpha..#Kask
+000003d0: 6164 615c 4b61 736b 6164 615c 5631 616c  ada\Kaskada\V1al
+000003e0: 7068 615c 4750 424d 6574 6164 6174 61ea  pha\GPBMetadata.
+000003f0: 0219 4b61 736b 6164 613a 3a4b 6173 6b61  ..Kaskada::Kaska
+00000400: 6461 3a3a 5631 616c 7068 6129 1ada 075f  da::V1alpha)..._
+00000410: 5f64 6f63 5f5f da0f 676f 6f67 6c65 2e70  _doc__..google.p
+00000420: 726f 746f 6275 6672 0200 0000 da0b 5f64  rotobufr......_d
+00000430: 6573 6372 6970 746f 7272 0300 0000 da10  escriptorr......
+00000440: 5f64 6573 6372 6970 746f 725f 706f 6f6c  _descriptor_pool
+00000450: 7204 0000 00da 085f 6d65 7373 6167 6572  r......_messager
+00000460: 0500 0000 da0b 5f72 6566 6c65 6374 696f  ......_reflectio
+00000470: 6e72 0600 0000 da10 5f73 796d 626f 6c5f  nr......_symbol_
+00000480: 6461 7461 6261 7365 da07 4465 6661 756c  database..Defaul
+00000490: 74da 075f 7379 6d5f 6462 7207 0000 005a  t.._sym_dbr....Z
+000004a0: 2767 6f6f 676c 655f 646f 745f 7072 6f74  'google_dot_prot
+000004b0: 6f62 7566 5f64 6f74 5f64 6573 6372 6970  obuf_dot_descrip
+000004c0: 746f 725f 5f70 6232 da11 4164 6453 6572  tor__pb2..AddSer
+000004d0: 6961 6c69 7a65 6446 696c 65da 0a44 4553  ializedFile..DES
+000004e0: 4352 4950 544f 525a 1653 454e 5349 5449  CRIPTORZ.SENSITI
+000004f0: 5645 5f46 4945 4c44 5f4e 554d 4245 52da  VE_FIELD_NUMBER.
+00000500: 1265 7874 656e 7369 6f6e 735f 6279 5f6e  .extensions_by_n
+00000510: 616d 6572 0800 0000 da12 5f55 5345 5f43  amer......_USE_C
+00000520: 5f44 4553 4352 4950 544f 5253 da0c 4669  _DESCRIPTORS..Fi
+00000530: 656c 644f 7074 696f 6e73 da11 5265 6769  eldOptions..Regi
+00000540: 7374 6572 4578 7465 6e73 696f 6eda 085f  sterExtension.._
+00000550: 6f70 7469 6f6e 73da 135f 7365 7269 616c  options.._serial
+00000560: 697a 6564 5f6f 7074 696f 6e73 a900 721a  ized_options..r.
+00000570: 0000 0072 1a00 0000 fa2f 2f73 7263 2f73  ...r.....//src/s
+00000580: 7263 2f6b 6173 6b61 6461 2f6b 6173 6b61  rc/kaskada/kaska
+00000590: 6461 2f76 3161 6c70 6861 2f6f 7074 696f  da/v1alpha/optio
+000005a0: 6e73 5f70 6232 2e70 79da 083c 6d6f 6475  ns_pb2.py..<modu
+000005b0: 6c65 3e04 0000 0073 1c00 0000 0401 0c01  le>....s........
+000005c0: 0c01 0c01 0c01 0c03 0803 0c03 0e03 0401  ................
+000005d0: 0a02 0a01 0c02 0601                      ........
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/pulsar_pb2.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/pulsar_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 3561 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,154 +1,150 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 e90d 0000  o.........5d....
+00000000: 610d 0d0a 0000 0000 2038 4164 e90d 0000  a....... 8Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 1401 0000 6400  .....@...s....d.
+00000020: 0007 0000 0040 0000 0073 1201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
 00000070: a00c a100 5a0d 6401 6407 6c01 6d0e 5a0f  ....Z.d.d.l.m.Z.
 00000080: 0100 6401 6408 6c10 6d11 5a12 0100 6505  ..d.d.l.m.Z...e.
 00000090: a00c a100 a013 6409 a101 5a14 6514 6a15  ......d...Z.e.j.
 000000a0: 640a 1900 5a16 6514 6a15 640b 1900 5a17  d...Z.e.j.d...Z.
 000000b0: 6509 a018 640a 6507 6a19 6601 6516 640c  e...d.e.j.f.e.d.
 000000c0: 640d 9c02 a103 5a1a 650d a01b 651a a101  d.....Z.e...e...
 000000d0: 0100 6509 a018 640b 6507 6a19 6601 6517  ..e...d.e.j.f.e.
 000000e0: 640c 640d 9c02 a103 5a1c 650d a01b 651c  d.d.....Z.e...e.
-000000f0: a101 0100 6503 6a1d 640e 6b02 7288 640f  ....e.j.d.k.r.d.
-00000100: 6514 5f1e 6410 6514 5f1f 640f 6516 6a20  e._.d.e._.d.e.j 
-00000110: 6411 1900 5f1e 6412 6516 6a20 6411 1900  d..._.d.e.j d...
-00000120: 5f1f 6413 6516 5f21 6414 6516 5f22 6415  _.d.e._!d.e._"d.
-00000130: 6517 5f21 6416 6517 5f22 640f 5300 640f  e._!d.e._"d.S.d.
-00000140: 5300 2917 7a1f 4765 6e65 7261 7465 6420  S.).z.Generated 
-00000150: 7072 6f74 6f63 6f6c 2062 7566 6665 7220  protocol buffer 
-00000160: 636f 6465 2ee9 0000 0000 2901 da0a 6465  code......)...de
-00000170: 7363 7269 7074 6f72 2901 da0f 6465 7363  scriptor)...desc
-00000180: 7269 7074 6f72 5f70 6f6f 6c29 01da 076d  riptor_pool)...m
-00000190: 6573 7361 6765 2901 da0a 7265 666c 6563  essage)...reflec
-000001a0: 7469 6f6e 2901 da0f 7379 6d62 6f6c 5f64  tion)...symbol_d
-000001b0: 6174 6162 6173 6529 01da 0d74 696d 6573  atabase)...times
-000001c0: 7461 6d70 5f70 6232 2901 da0b 6f70 7469  tamp_pb2)...opti
-000001d0: 6f6e 735f 7062 3273 5c03 0000 0a24 6b61  ons_pb2s\....$ka
-000001e0: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
-000001f0: 616c 7068 612f 7075 6c73 6172 2e70 726f  alpha/pulsar.pro
-00000200: 746f 1217 6b61 736b 6164 612e 6b61 736b  to..kaskada.kask
-00000210: 6164 612e 7631 616c 7068 611a 1f67 6f6f  ada.v1alpha..goo
-00000220: 676c 652f 7072 6f74 6f62 7566 2f74 696d  gle/protobuf/tim
-00000230: 6573 7461 6d70 2e70 726f 746f 1a25 6b61  estamp.proto.%ka
-00000240: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
-00000250: 616c 7068 612f 6f70 7469 6f6e 732e 7072  alpha/options.pr
-00000260: 6f74 6f22 8502 0a0c 5075 6c73 6172 436f  oto"....PulsarCo
-00000270: 6e66 6967 122c 0a12 6272 6f6b 6572 5f73  nfig.,..broker_s
-00000280: 6572 7669 6365 5f75 726c 1801 2001 2809  ervice_url.. .(.
-00000290: 5210 6272 6f6b 6572 5365 7276 6963 6555  R.brokerServiceU
-000002a0: 726c 122a 0a11 6164 6d69 6e5f 7365 7276  rl.*..admin_serv
-000002b0: 6963 655f 7572 6c18 0220 0128 0952 0f61  ice_url.. .(.R.a
-000002c0: 646d 696e 5365 7276 6963 6555 726c 121f  dminServiceUrl..
-000002d0: 0a0b 6175 7468 5f70 6c75 6769 6e18 0320  ..auth_plugin.. 
-000002e0: 0128 0952 0a61 7574 6850 6c75 6769 6e12  .(.R.authPlugin.
-000002f0: 250a 0b61 7574 685f 7061 7261 6d73 1804  %..auth_params..
-00000300: 2001 2809 4204 80b5 1801 520a 6175 7468   .(.B.....R.auth
-00000310: 5061 7261 6d73 1216 0a06 7465 6e61 6e74  Params....tenant
-00000320: 1805 2001 2809 5206 7465 6e61 6e74 121c  .. .(.R.tenant..
-00000330: 0a09 6e61 6d65 7370 6163 6518 0620 0128  ..namespace.. .(
-00000340: 0952 096e 616d 6573 7061 6365 121d 0a0a  .R.namespace....
-00000350: 746f 7069 635f 6e61 6d65 1807 2001 2809  topic_name.. .(.
-00000360: 5209 746f 7069 634e 616d 6522 c401 0a12  R.topicName"....
-00000370: 5075 6c73 6172 5375 6273 6372 6970 7469  PulsarSubscripti
-00000380: 6f6e 123d 0a06 636f 6e66 6967 1801 2001  on.=..config.. .
-00000390: 280b 3225 2e6b 6173 6b61 6461 2e6b 6173  (.2%.kaskada.kas
-000003a0: 6b61 6461 2e76 3161 6c70 6861 2e50 756c  kada.v1alpha.Pul
-000003b0: 7361 7243 6f6e 6669 6752 0663 6f6e 6669  sarConfigR.confi
-000003c0: 6712 270a 0f73 7562 7363 7269 7074 696f  g.'..subscriptio
-000003d0: 6e5f 6964 1802 2001 2809 520e 7375 6273  n_id.. .(.R.subs
-000003e0: 6372 6970 7469 6f6e 4964 1246 0a11 6c61  criptionId.F..la
-000003f0: 7374 5f70 7562 6c69 7368 5f74 696d 6518  st_publish_time.
-00000400: 0320 0128 0b32 1a2e 676f 6f67 6c65 2e70  . .(.2..google.p
-00000410: 726f 746f 6275 662e 5469 6d65 7374 616d  rotobuf.Timestam
-00000420: 7052 0f6c 6173 7450 7562 6c69 7368 5469  pR.lastPublishTi
-00000430: 6d65 42fb 010a 1b63 6f6d 2e6b 6173 6b61  meB....com.kaska
-00000440: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-00000450: 6861 420b 5075 6c73 6172 5072 6f74 6f50  haB.PulsarProtoP
-00000460: 015a 5167 6974 6875 622e 636f 6d2f 6b61  .ZQgithub.com/ka
-00000470: 736b 6164 612d 6169 2f6b 6173 6b61 6461  skada-ai/kaskada
-00000480: 2f67 656e 2f70 726f 746f 2f67 6f2f 6b61  /gen/proto/go/ka
-00000490: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
-000004a0: 616c 7068 613b 6b61 736b 6164 6176 3161  alpha;kaskadav1a
-000004b0: 6c70 6861 a202 034b 4b58 aa02 174b 6173  lpha...KKX...Kas
-000004c0: 6b61 6461 2e4b 6173 6b61 6461 2e56 3161  kada.Kaskada.V1a
-000004d0: 6c70 6861 ca02 174b 6173 6b61 6461 5c4b  lpha...Kaskada\K
-000004e0: 6173 6b61 6461 5c56 3161 6c70 6861 e202  askada\V1alpha..
-000004f0: 234b 6173 6b61 6461 5c4b 6173 6b61 6461  #Kaskada\Kaskada
-00000500: 5c56 3161 6c70 6861 5c47 5042 4d65 7461  \V1alpha\GPBMeta
-00000510: 6461 7461 ea02 194b 6173 6b61 6461 3a3a  data...Kaskada::
-00000520: 4b61 736b 6164 613a 3a56 3161 6c70 6861  Kaskada::V1alpha
-00000530: 6206 7072 6f74 6f33 da0c 5075 6c73 6172  b.proto3..Pulsar
-00000540: 436f 6e66 6967 da12 5075 6c73 6172 5375  Config..PulsarSu
-00000550: 6273 6372 6970 7469 6f6e 7a22 6b61 736b  bscriptionz"kask
-00000560: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-00000570: 7068 612e 7075 6c73 6172 5f70 6232 2902  pha.pulsar_pb2).
-00000580: da0a 4445 5343 5249 5054 4f52 da0a 5f5f  ..DESCRIPTOR..__
-00000590: 6d6f 6475 6c65 5f5f 464e 73fb 0000 000a  module__FNs.....
-000005a0: 1b63 6f6d 2e6b 6173 6b61 6461 2e6b 6173  .com.kaskada.kas
-000005b0: 6b61 6461 2e76 3161 6c70 6861 420b 5075  kada.v1alphaB.Pu
-000005c0: 6c73 6172 5072 6f74 6f50 015a 5167 6974  lsarProtoP.ZQgit
-000005d0: 6875 622e 636f 6d2f 6b61 736b 6164 612d  hub.com/kaskada-
-000005e0: 6169 2f6b 6173 6b61 6461 2f67 656e 2f70  ai/kaskada/gen/p
-000005f0: 726f 746f 2f67 6f2f 6b61 736b 6164 612f  roto/go/kaskada/
-00000600: 6b61 736b 6164 612f 7631 616c 7068 613b  kaskada/v1alpha;
-00000610: 6b61 736b 6164 6176 3161 6c70 6861 a202  kaskadav1alpha..
-00000620: 034b 4b58 aa02 174b 6173 6b61 6461 2e4b  .KKX...Kaskada.K
-00000630: 6173 6b61 6461 2e56 3161 6c70 6861 ca02  askada.V1alpha..
-00000640: 174b 6173 6b61 6461 5c4b 6173 6b61 6461  .Kaskada\Kaskada
-00000650: 5c56 3161 6c70 6861 e202 234b 6173 6b61  \V1alpha..#Kaska
-00000660: 6461 5c4b 6173 6b61 6461 5c56 3161 6c70  da\Kaskada\V1alp
-00000670: 6861 5c47 5042 4d65 7461 6461 7461 ea02  ha\GPBMetadata..
-00000680: 194b 6173 6b61 6461 3a3a 4b61 736b 6164  .Kaskada::Kaskad
-00000690: 613a 3a56 3161 6c70 6861 da0b 6175 7468  a::V1alpha..auth
-000006a0: 5f70 6172 616d 7373 0400 0000 80b5 1801  _paramss........
-000006b0: e98a 0000 0069 8f01 0000 6992 0100 0069  .....i....i....i
-000006c0: 5602 0000 2923 da07 5f5f 646f 635f 5fda  V...)#..__doc__.
-000006d0: 0f67 6f6f 676c 652e 7072 6f74 6f62 7566  .google.protobuf
-000006e0: 7202 0000 00da 0b5f 6465 7363 7269 7074  r......_descript
-000006f0: 6f72 7203 0000 00da 105f 6465 7363 7269  orr......_descri
-00000700: 7074 6f72 5f70 6f6f 6c72 0400 0000 da08  ptor_poolr......
-00000710: 5f6d 6573 7361 6765 7205 0000 00da 0b5f  _messager......_
-00000720: 7265 666c 6563 7469 6f6e 7206 0000 00da  reflectionr.....
-00000730: 105f 7379 6d62 6f6c 5f64 6174 6162 6173  ._symbol_databas
-00000740: 65da 0744 6566 6175 6c74 da07 5f73 796d  e..Default.._sym
-00000750: 5f64 6272 0700 0000 da26 676f 6f67 6c65  _dbr.....&google
-00000760: 5f64 6f74 5f70 726f 746f 6275 665f 646f  _dot_protobuf_do
-00000770: 745f 7469 6d65 7374 616d 705f 5f70 6232  t_timestamp__pb2
-00000780: da17 6b61 736b 6164 612e 6b61 736b 6164  ..kaskada.kaskad
-00000790: 612e 7631 616c 7068 6172 0800 0000 da30  a.v1alphar.....0
-000007a0: 6b61 736b 6164 615f 646f 745f 6b61 736b  kaskada_dot_kask
-000007b0: 6164 615f 646f 745f 7631 616c 7068 615f  ada_dot_v1alpha_
-000007c0: 646f 745f 6f70 7469 6f6e 735f 5f70 6232  dot_options__pb2
-000007d0: da11 4164 6453 6572 6961 6c69 7a65 6446  ..AddSerializedF
-000007e0: 696c 6572 0b00 0000 da15 6d65 7373 6167  iler......messag
-000007f0: 655f 7479 7065 735f 6279 5f6e 616d 65da  e_types_by_name.
-00000800: 0d5f 5055 4c53 4152 434f 4e46 4947 da13  ._PULSARCONFIG..
-00000810: 5f50 554c 5341 5253 5542 5343 5249 5054  _PULSARSUBSCRIPT
-00000820: 494f 4eda 1c47 656e 6572 6174 6564 5072  ION..GeneratedPr
-00000830: 6f74 6f63 6f6c 4d65 7373 6167 6554 7970  otocolMessageTyp
-00000840: 65da 074d 6573 7361 6765 7209 0000 00da  e..Messager.....
-00000850: 0f52 6567 6973 7465 724d 6573 7361 6765  .RegisterMessage
-00000860: 720a 0000 00da 125f 5553 455f 435f 4445  r......_USE_C_DE
-00000870: 5343 5249 5054 4f52 53da 085f 6f70 7469  SCRIPTORS.._opti
-00000880: 6f6e 73da 135f 7365 7269 616c 697a 6564  ons.._serialized
-00000890: 5f6f 7074 696f 6e73 da0e 6669 656c 6473  _options..fields
-000008a0: 5f62 795f 6e61 6d65 da11 5f73 6572 6961  _by_name.._seria
-000008b0: 6c69 7a65 645f 7374 6172 74da 0f5f 7365  lized_start.._se
-000008c0: 7269 616c 697a 6564 5f65 6e64 a900 7228  rialized_end..r(
-000008d0: 0000 0072 2800 0000 fa70 2f68 6f6d 652f  ...r(....p/home/
-000008e0: 7468 6572 6170 6f6e 2f52 6570 6f73 2f47  therapon/Repos/G
-000008f0: 6974 4875 622f 4b61 736b 6164 6141 492f  itHub/KaskadaAI/
-00000900: 6b61 736b 6164 612f 7265 6c65 6173 696e  kaskada/releasin
-00000910: 672f 636c 6965 6e74 732f 7079 7468 6f6e  g/clients/python
-00000920: 2f73 7263 2f6b 6173 6b61 6461 2f6b 6173  /src/kaskada/kas
-00000930: 6b61 6461 2f76 3161 6c70 6861 2f70 756c  kada/v1alpha/pul
-00000940: 7361 725f 7062 322e 7079 da08 3c6d 6f64  sar_pb2.py..<mod
-00000950: 756c 653e 0100 0000 7340 0000 0004 030c  ule>....s@......
-00000960: 010c 010c 010c 010c 0108 030c 030c 010e  ................
-00000970: 030a 040a 010c 0102 0102 0108 fe0a 050c  ................
-00000980: 0202 0102 0108 fe0a 050a 0206 0206 010c  ................
-00000990: 010c 0106 0106 0106 010a 0104 f7         .............
+000000f0: a101 0100 6503 6a1d 640e 6b02 9001 720e  ....e.j.d.k...r.
+00000100: 640f 6514 5f1e 6410 6514 5f1f 640f 6516  d.e._.d.e._.d.e.
+00000110: 6a20 6411 1900 5f1e 6412 6516 6a20 6411  j d..._.d.e.j d.
+00000120: 1900 5f1f 6413 6516 5f21 6414 6516 5f22  .._.d.e._!d.e._"
+00000130: 6415 6517 5f21 6416 6517 5f22 640f 5300  d.e._!d.e._"d.S.
+00000140: 2917 7a1f 4765 6e65 7261 7465 6420 7072  ).z.Generated pr
+00000150: 6f74 6f63 6f6c 2062 7566 6665 7220 636f  otocol buffer co
+00000160: 6465 2ee9 0000 0000 2901 da0a 6465 7363  de......)...desc
+00000170: 7269 7074 6f72 2901 da0f 6465 7363 7269  riptor)...descri
+00000180: 7074 6f72 5f70 6f6f 6c29 01da 076d 6573  ptor_pool)...mes
+00000190: 7361 6765 2901 da0a 7265 666c 6563 7469  sage)...reflecti
+000001a0: 6f6e 2901 da0f 7379 6d62 6f6c 5f64 6174  on)...symbol_dat
+000001b0: 6162 6173 6529 01da 0d74 696d 6573 7461  abase)...timesta
+000001c0: 6d70 5f70 6232 2901 da0b 6f70 7469 6f6e  mp_pb2)...option
+000001d0: 735f 7062 3273 5c03 0000 0a24 6b61 736b  s_pb2s\....$kask
+000001e0: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
+000001f0: 7068 612f 7075 6c73 6172 2e70 726f 746f  pha/pulsar.proto
+00000200: 1217 6b61 736b 6164 612e 6b61 736b 6164  ..kaskada.kaskad
+00000210: 612e 7631 616c 7068 611a 1f67 6f6f 676c  a.v1alpha..googl
+00000220: 652f 7072 6f74 6f62 7566 2f74 696d 6573  e/protobuf/times
+00000230: 7461 6d70 2e70 726f 746f 1a25 6b61 736b  tamp.proto.%kask
+00000240: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
+00000250: 7068 612f 6f70 7469 6f6e 732e 7072 6f74  pha/options.prot
+00000260: 6f22 8502 0a0c 5075 6c73 6172 436f 6e66  o"....PulsarConf
+00000270: 6967 122c 0a12 6272 6f6b 6572 5f73 6572  ig.,..broker_ser
+00000280: 7669 6365 5f75 726c 1801 2001 2809 5210  vice_url.. .(.R.
+00000290: 6272 6f6b 6572 5365 7276 6963 6555 726c  brokerServiceUrl
+000002a0: 122a 0a11 6164 6d69 6e5f 7365 7276 6963  .*..admin_servic
+000002b0: 655f 7572 6c18 0220 0128 0952 0f61 646d  e_url.. .(.R.adm
+000002c0: 696e 5365 7276 6963 6555 726c 121f 0a0b  inServiceUrl....
+000002d0: 6175 7468 5f70 6c75 6769 6e18 0320 0128  auth_plugin.. .(
+000002e0: 0952 0a61 7574 6850 6c75 6769 6e12 250a  .R.authPlugin.%.
+000002f0: 0b61 7574 685f 7061 7261 6d73 1804 2001  .auth_params.. .
+00000300: 2809 4204 80b5 1801 520a 6175 7468 5061  (.B.....R.authPa
+00000310: 7261 6d73 1216 0a06 7465 6e61 6e74 1805  rams....tenant..
+00000320: 2001 2809 5206 7465 6e61 6e74 121c 0a09   .(.R.tenant....
+00000330: 6e61 6d65 7370 6163 6518 0620 0128 0952  namespace.. .(.R
+00000340: 096e 616d 6573 7061 6365 121d 0a0a 746f  .namespace....to
+00000350: 7069 635f 6e61 6d65 1807 2001 2809 5209  pic_name.. .(.R.
+00000360: 746f 7069 634e 616d 6522 c401 0a12 5075  topicName"....Pu
+00000370: 6c73 6172 5375 6273 6372 6970 7469 6f6e  lsarSubscription
+00000380: 123d 0a06 636f 6e66 6967 1801 2001 280b  .=..config.. .(.
+00000390: 3225 2e6b 6173 6b61 6461 2e6b 6173 6b61  2%.kaskada.kaska
+000003a0: 6461 2e76 3161 6c70 6861 2e50 756c 7361  da.v1alpha.Pulsa
+000003b0: 7243 6f6e 6669 6752 0663 6f6e 6669 6712  rConfigR.config.
+000003c0: 270a 0f73 7562 7363 7269 7074 696f 6e5f  '..subscription_
+000003d0: 6964 1802 2001 2809 520e 7375 6273 6372  id.. .(.R.subscr
+000003e0: 6970 7469 6f6e 4964 1246 0a11 6c61 7374  iptionId.F..last
+000003f0: 5f70 7562 6c69 7368 5f74 696d 6518 0320  _publish_time.. 
+00000400: 0128 0b32 1a2e 676f 6f67 6c65 2e70 726f  .(.2..google.pro
+00000410: 746f 6275 662e 5469 6d65 7374 616d 7052  tobuf.TimestampR
+00000420: 0f6c 6173 7450 7562 6c69 7368 5469 6d65  .lastPublishTime
+00000430: 42fb 010a 1b63 6f6d 2e6b 6173 6b61 6461  B....com.kaskada
+00000440: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00000450: 420b 5075 6c73 6172 5072 6f74 6f50 015a  B.PulsarProtoP.Z
+00000460: 5167 6974 6875 622e 636f 6d2f 6b61 736b  Qgithub.com/kask
+00000470: 6164 612d 6169 2f6b 6173 6b61 6461 2f67  ada-ai/kaskada/g
+00000480: 656e 2f70 726f 746f 2f67 6f2f 6b61 736b  en/proto/go/kask
+00000490: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
+000004a0: 7068 613b 6b61 736b 6164 6176 3161 6c70  pha;kaskadav1alp
+000004b0: 6861 a202 034b 4b58 aa02 174b 6173 6b61  ha...KKX...Kaska
+000004c0: 6461 2e4b 6173 6b61 6461 2e56 3161 6c70  da.Kaskada.V1alp
+000004d0: 6861 ca02 174b 6173 6b61 6461 5c4b 6173  ha...Kaskada\Kas
+000004e0: 6b61 6461 5c56 3161 6c70 6861 e202 234b  kada\V1alpha..#K
+000004f0: 6173 6b61 6461 5c4b 6173 6b61 6461 5c56  askada\Kaskada\V
+00000500: 3161 6c70 6861 5c47 5042 4d65 7461 6461  1alpha\GPBMetada
+00000510: 7461 ea02 194b 6173 6b61 6461 3a3a 4b61  ta...Kaskada::Ka
+00000520: 736b 6164 613a 3a56 3161 6c70 6861 6206  skada::V1alphab.
+00000530: 7072 6f74 6f33 da0c 5075 6c73 6172 436f  proto3..PulsarCo
+00000540: 6e66 6967 da12 5075 6c73 6172 5375 6273  nfig..PulsarSubs
+00000550: 6372 6970 7469 6f6e 7a22 6b61 736b 6164  criptionz"kaskad
+00000560: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00000570: 612e 7075 6c73 6172 5f70 6232 2902 da0a  a.pulsar_pb2)...
+00000580: 4445 5343 5249 5054 4f52 da0a 5f5f 6d6f  DESCRIPTOR..__mo
+00000590: 6475 6c65 5f5f 464e 73fb 0000 000a 1b63  dule__FNs......c
+000005a0: 6f6d 2e6b 6173 6b61 6461 2e6b 6173 6b61  om.kaskada.kaska
+000005b0: 6461 2e76 3161 6c70 6861 420b 5075 6c73  da.v1alphaB.Puls
+000005c0: 6172 5072 6f74 6f50 015a 5167 6974 6875  arProtoP.ZQgithu
+000005d0: 622e 636f 6d2f 6b61 736b 6164 612d 6169  b.com/kaskada-ai
+000005e0: 2f6b 6173 6b61 6461 2f67 656e 2f70 726f  /kaskada/gen/pro
+000005f0: 746f 2f67 6f2f 6b61 736b 6164 612f 6b61  to/go/kaskada/ka
+00000600: 736b 6164 612f 7631 616c 7068 613b 6b61  skada/v1alpha;ka
+00000610: 736b 6164 6176 3161 6c70 6861 a202 034b  skadav1alpha...K
+00000620: 4b58 aa02 174b 6173 6b61 6461 2e4b 6173  KX...Kaskada.Kas
+00000630: 6b61 6461 2e56 3161 6c70 6861 ca02 174b  kada.V1alpha...K
+00000640: 6173 6b61 6461 5c4b 6173 6b61 6461 5c56  askada\Kaskada\V
+00000650: 3161 6c70 6861 e202 234b 6173 6b61 6461  1alpha..#Kaskada
+00000660: 5c4b 6173 6b61 6461 5c56 3161 6c70 6861  \Kaskada\V1alpha
+00000670: 5c47 5042 4d65 7461 6461 7461 ea02 194b  \GPBMetadata...K
+00000680: 6173 6b61 6461 3a3a 4b61 736b 6164 613a  askada::Kaskada:
+00000690: 3a56 3161 6c70 6861 5a0b 6175 7468 5f70  :V1alphaZ.auth_p
+000006a0: 6172 616d 7373 0400 0000 80b5 1801 e98a  aramss..........
+000006b0: 0000 0069 8f01 0000 6992 0100 0069 5602  ...i....i....iV.
+000006c0: 0000 2923 da07 5f5f 646f 635f 5fda 0f67  ..)#..__doc__..g
+000006d0: 6f6f 676c 652e 7072 6f74 6f62 7566 7202  oogle.protobufr.
+000006e0: 0000 00da 0b5f 6465 7363 7269 7074 6f72  ....._descriptor
+000006f0: 7203 0000 00da 105f 6465 7363 7269 7074  r......_descript
+00000700: 6f72 5f70 6f6f 6c72 0400 0000 da08 5f6d  or_poolr......_m
+00000710: 6573 7361 6765 7205 0000 00da 0b5f 7265  essager......_re
+00000720: 666c 6563 7469 6f6e 7206 0000 00da 105f  flectionr......_
+00000730: 7379 6d62 6f6c 5f64 6174 6162 6173 65da  symbol_database.
+00000740: 0744 6566 6175 6c74 da07 5f73 796d 5f64  .Default.._sym_d
+00000750: 6272 0700 0000 5a26 676f 6f67 6c65 5f64  br....Z&google_d
+00000760: 6f74 5f70 726f 746f 6275 665f 646f 745f  ot_protobuf_dot_
+00000770: 7469 6d65 7374 616d 705f 5f70 6232 da17  timestamp__pb2..
+00000780: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000790: 7631 616c 7068 6172 0800 0000 da30 6b61  v1alphar.....0ka
+000007a0: 736b 6164 615f 646f 745f 6b61 736b 6164  skada_dot_kaskad
+000007b0: 615f 646f 745f 7631 616c 7068 615f 646f  a_dot_v1alpha_do
+000007c0: 745f 6f70 7469 6f6e 735f 5f70 6232 da11  t_options__pb2..
+000007d0: 4164 6453 6572 6961 6c69 7a65 6446 696c  AddSerializedFil
+000007e0: 6572 0b00 0000 da15 6d65 7373 6167 655f  er......message_
+000007f0: 7479 7065 735f 6279 5f6e 616d 655a 0d5f  types_by_nameZ._
+00000800: 5055 4c53 4152 434f 4e46 4947 5a13 5f50  PULSARCONFIGZ._P
+00000810: 554c 5341 5253 5542 5343 5249 5054 494f  ULSARSUBSCRIPTIO
+00000820: 4eda 1c47 656e 6572 6174 6564 5072 6f74  N..GeneratedProt
+00000830: 6f63 6f6c 4d65 7373 6167 6554 7970 65da  ocolMessageType.
+00000840: 074d 6573 7361 6765 7209 0000 00da 0f52  .Messager......R
+00000850: 6567 6973 7465 724d 6573 7361 6765 720a  egisterMessager.
+00000860: 0000 00da 125f 5553 455f 435f 4445 5343  ....._USE_C_DESC
+00000870: 5249 5054 4f52 53da 085f 6f70 7469 6f6e  RIPTORS.._option
+00000880: 73da 135f 7365 7269 616c 697a 6564 5f6f  s.._serialized_o
+00000890: 7074 696f 6e73 da0e 6669 656c 6473 5f62  ptions..fields_b
+000008a0: 795f 6e61 6d65 da11 5f73 6572 6961 6c69  y_name.._seriali
+000008b0: 7a65 645f 7374 6172 74da 0f5f 7365 7269  zed_start.._seri
+000008c0: 616c 697a 6564 5f65 6e64 a900 7224 0000  alized_end..r$..
+000008d0: 0072 2400 0000 fa2e 2f73 7263 2f73 7263  .r$...../src/src
+000008e0: 2f6b 6173 6b61 6461 2f6b 6173 6b61 6461  /kaskada/kaskada
+000008f0: 2f76 3161 6c70 6861 2f70 756c 7361 725f  /v1alpha/pulsar_
+00000900: 7062 322e 7079 da08 3c6d 6f64 756c 653e  pb2.py..<module>
+00000910: 0400 0000 733c 0000 0004 010c 010c 010c  ....s<..........
+00000920: 010c 010c 0308 030c 010c 030e 040a 010a  ................
+00000930: 010c 0102 0102 fe08 050a 020c 0102 0102  ................
+00000940: fe08 050a 020c 0206 0106 010c 010c 0106  ................
+00000950: 0106 0106 01                             .....
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/query_service_pb2.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/query_service_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 16795 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 9b41 0000  o.........5d.A..
+00000000: 610d 0d0a 0000 0000 2038 4164 9b41 0000  a....... 8Ad.A..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000d 0000 0040 0000 0073 0405 0000 6400  .....@...s....d.
+00000020: 000d 0000 0040 0000 0073 0005 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
 00000070: a00c a100 5a0d 6401 6407 6c0e 6d0f 5a10  ....Z.d.d.l.m.Z.
 00000080: 0100 6401 6408 6c0e 6d11 5a12 0100 6401  ..d.d.l.m.Z...d.
 00000090: 6409 6c01 6d13 5a14 0100 6401 640a 6c01  d.l.m.Z...d.d.l.
@@ -48,15 +48,15 @@
 000002f0: 0100 6509 a03b 641d 6507 6a3c 6601 6535  ..e..;d.e.j<f.e5
 00000300: 6422 6423 9c02 a103 5a48 650d a03e 6548  d"d#....ZHe..>eH
 00000310: a101 0100 6509 a03b 641e 6507 6a3c 6601  ....e..;d.e.j<f.
 00000320: 6536 6422 6423 9c02 a103 5a49 650d a03e  e6d"d#....ZIe..>
 00000330: 6549 a101 0100 6509 a03b 641f 6507 6a3c  eI....e..;d.e.j<
 00000340: 6601 6537 6422 6423 9c02 a103 5a4a 650d  f.e7d"d#....ZJe.
 00000350: a03e 654a a101 0100 6528 6a4b 6426 1900  .>eJ....e(jKd&..
-00000360: 5a4c 6503 6a4d 6427 6b02 9002 7280 6428  ZLe.jMd'k...r.d(
+00000360: 5a4c 6503 6a4d 6427 6b02 9004 72fc 6428  ZLe.jMd'k...r.d(
 00000370: 6528 5f4e 6429 6528 5f4f 6428 652a 6a50  e(_Nd)e(_Od(e*jP
 00000380: 642a 1900 5f4e 642b 652a 6a50 642a 1900  d*.._Nd+e*jPd*..
 00000390: 5f4f 6428 652a 6a50 642c 1900 5f4e 642d  _Od(e*jPd,.._Nd-
 000003a0: 652a 6a50 642c 1900 5f4f 6428 652a 6a50  e*jPd,.._Od(e*jP
 000003b0: 642e 1900 5f4e 642b 652a 6a50 642e 1900  d..._Nd+e*jPd...
 000003c0: 5f4f 6428 652a 6a50 642f 1900 5f4e 642b  _Od(e*jPd/.._Nd+
 000003d0: 652a 6a50 642f 1900 5f4f 6428 6534 6a50  e*jPd/.._Od(e4jP
@@ -76,474 +76,469 @@
 000004b0: 5f53 6445 6530 5f52 6446 6530 5f53 6447  _SdEe0_RdFe0_SdG
 000004c0: 6531 5f52 6448 6531 5f53 6449 6532 5f52  e1_RdHe1_SdIe2_R
 000004d0: 644a 6532 5f53 644b 6533 5f52 644c 6533  dJe2_SdKe3_RdLe3
 000004e0: 5f53 644d 653a 5f52 644e 653a 5f53 644f  _SdMe:_RdNe:_SdO
 000004f0: 6534 5f52 6450 6534 5f53 6451 6535 5f52  e4_RdPe4_SdQe5_R
 00000500: 6452 6535 5f53 6453 6536 5f52 6454 6536  dRe5_SdSe6_RdTe6
 00000510: 5f53 6455 6537 5f52 6456 6537 5f53 6457  _SdUe7_RdVe7_SdW
-00000520: 654c 5f52 6458 654c 5f53 6428 5300 6428  eL_RdXeL_Sd(S.d(
-00000530: 5300 2959 7a1f 4765 6e65 7261 7465 6420  S.)Yz.Generated 
-00000540: 7072 6f74 6f63 6f6c 2062 7566 6665 7220  protocol buffer 
-00000550: 636f 6465 2ee9 0000 0000 2901 da0a 6465  code......)...de
-00000560: 7363 7269 7074 6f72 2901 da0f 6465 7363  scriptor)...desc
-00000570: 7269 7074 6f72 5f70 6f6f 6c29 01da 076d  riptor_pool)...m
-00000580: 6573 7361 6765 2901 da0a 7265 666c 6563  essage)...reflec
-00000590: 7469 6f6e 2901 da0f 7379 6d62 6f6c 5f64  tion)...symbol_d
-000005a0: 6174 6162 6173 6529 01da 0f61 6e6e 6f74  atabase)...annot
-000005b0: 6174 696f 6e73 5f70 6232 2901 da12 6669  ations_pb2)...fi
-000005c0: 656c 645f 6265 6861 7669 6f72 5f70 6232  eld_behavior_pb2
-000005d0: 2901 da0c 6475 7261 7469 6f6e 5f70 6232  )...duration_pb2
-000005e0: 2901 da0d 7469 6d65 7374 616d 705f 7062  )...timestamp_pb
-000005f0: 3229 01da 0c77 7261 7070 6572 735f 7062  2)...wrappers_pb
-00000600: 3229 01da 0a63 6f6d 6d6f 6e5f 7062 3229  2)...common_pb2)
-00000610: 01da 1064 6573 7469 6e61 7469 6f6e 735f  ...destinations_
-00000620: 7062 3229 01da 1466 656e 6c5f 6469 6167  pb2)...fenl_diag
-00000630: 6e6f 7374 6963 735f 7062 3229 01da 0a73  nostics_pb2)...s
-00000640: 6368 656d 615f 7062 3229 01da 1076 6965  chema_pb2)...vie
-00000650: 775f 7365 7276 6963 655f 7062 3229 01da  w_service_pb2)..
-00000660: 0c76 616c 6964 6174 655f 7062 3273 7c10  .validate_pb2s|.
-00000670: 0000 0a2b 6b61 736b 6164 612f 6b61 736b  ...+kaskada/kask
-00000680: 6164 612f 7631 616c 7068 612f 7175 6572  ada/v1alpha/quer
-00000690: 795f 7365 7276 6963 652e 7072 6f74 6f12  y_service.proto.
-000006a0: 176b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
-000006b0: 2e76 3161 6c70 6861 1a1c 676f 6f67 6c65  .v1alpha..google
-000006c0: 2f61 7069 2f61 6e6e 6f74 6174 696f 6e73  /api/annotations
-000006d0: 2e70 726f 746f 1a1f 676f 6f67 6c65 2f61  .proto..google/a
-000006e0: 7069 2f66 6965 6c64 5f62 6568 6176 696f  pi/field_behavio
-000006f0: 722e 7072 6f74 6f1a 1e67 6f6f 676c 652f  r.proto..google/
-00000700: 7072 6f74 6f62 7566 2f64 7572 6174 696f  protobuf/duratio
-00000710: 6e2e 7072 6f74 6f1a 1f67 6f6f 676c 652f  n.proto..google/
-00000720: 7072 6f74 6f62 7566 2f74 696d 6573 7461  protobuf/timesta
-00000730: 6d70 2e70 726f 746f 1a1e 676f 6f67 6c65  mp.proto..google
-00000740: 2f70 726f 746f 6275 662f 7772 6170 7065  /protobuf/wrappe
-00000750: 7273 2e70 726f 746f 1a24 6b61 736b 6164  rs.proto.$kaskad
-00000760: 612f 6b61 736b 6164 612f 7631 616c 7068  a/kaskada/v1alph
-00000770: 612f 636f 6d6d 6f6e 2e70 726f 746f 1a2a  a/common.proto.*
-00000780: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
-00000790: 7631 616c 7068 612f 6465 7374 696e 6174  v1alpha/destinat
-000007a0: 696f 6e73 2e70 726f 746f 1a2e 6b61 736b  ions.proto..kask
-000007b0: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
-000007c0: 7068 612f 6665 6e6c 5f64 6961 676e 6f73  pha/fenl_diagnos
-000007d0: 7469 6373 2e70 726f 746f 1a24 6b61 736b  tics.proto.$kask
-000007e0: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
-000007f0: 7068 612f 7363 6865 6d61 2e70 726f 746f  pha/schema.proto
-00000800: 1a2a 6b61 736b 6164 612f 6b61 736b 6164  .*kaskada/kaskad
-00000810: 612f 7631 616c 7068 612f 7669 6577 5f73  a/v1alpha/view_s
-00000820: 6572 7669 6365 2e70 726f 746f 1a17 7661  ervice.proto..va
-00000830: 6c69 6461 7465 2f76 616c 6964 6174 652e  lidate/validate.
-00000840: 7072 6f74 6f22 c907 0a05 5175 6572 7912  proto"....Query.
-00000850: 1e0a 0871 7565 7279 5f69 6418 0120 0128  ...query_id.. .(
-00000860: 0942 03e0 4103 5207 7175 6572 7949 6412  .B..A.R.queryId.
-00000870: 270a 0a65 7870 7265 7373 696f 6e18 0220  '..expression.. 
-00000880: 0128 0942 07fa 4204 7202 1001 520a 6578  .(.B..B.r...R.ex
-00000890: 7072 6573 7369 6f6e 1246 0a0b 6465 7374  pression.F..dest
-000008a0: 696e 6174 696f 6e18 6820 0128 0b32 242e  ination.h .(.2$.
-000008b0: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
-000008c0: 7631 616c 7068 612e 4465 7374 696e 6174  v1alpha.Destinat
-000008d0: 696f 6e52 0b64 6573 7469 6e61 7469 6f6e  ionR.destination
-000008e0: 1240 0a0d 6461 7461 5f74 6f6b 656e 5f69  .@..data_token_i
-000008f0: 6418 0320 0128 0b32 1c2e 676f 6f67 6c65  d.. .(.2..google
-00000900: 2e70 726f 746f 6275 662e 5374 7269 6e67  .protobuf.String
-00000910: 5661 6c75 6552 0b64 6174 6154 6f6b 656e  ValueR.dataToken
-00000920: 4964 1238 0a05 7669 6577 7318 0420 0328  Id.8..views.. .(
-00000930: 0b32 1d2e 6b61 736b 6164 612e 6b61 736b  .2..kaskada.kask
-00000940: 6164 612e 7631 616c 7068 612e 5669 6577  ada.v1alpha.View
-00000950: 4203 e041 0352 0576 6965 7773 1256 0a0f  B..A.R.views.V..
-00000960: 7265 7375 6c74 5f62 6568 6176 696f 7218  result_behavior.
-00000970: 0520 0128 0e32 2d2e 6b61 736b 6164 612e  . .(.2-.kaskada.
-00000980: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
-00000990: 5175 6572 792e 5265 7375 6c74 4265 6861  Query.ResultBeha
-000009a0: 7669 6f72 520e 7265 7375 6c74 4265 6861  viorR.resultBeha
-000009b0: 7669 6f72 123d 0a06 6c69 6d69 7473 1806  vior.=..limits..
-000009c0: 2001 280b 3225 2e6b 6173 6b61 6461 2e6b   .(.2%.kaskada.k
-000009d0: 6173 6b61 6461 2e76 3161 6c70 6861 2e51  askada.v1alpha.Q
-000009e0: 7565 7279 2e4c 696d 6974 7352 066c 696d  uery.LimitsR.lim
-000009f0: 6974 7312 3b0a 0573 6c69 6365 1807 2001  its.;..slice.. .
-00000a00: 280b 3225 2e6b 6173 6b61 6461 2e6b 6173  (.2%.kaskada.kas
-00000a10: 6b61 6461 2e76 3161 6c70 6861 2e53 6c69  kada.v1alpha.Sli
-00000a20: 6365 5265 7175 6573 7452 0573 6c69 6365  ceRequestR.slice
-00000a30: 1248 0a12 6368 616e 6765 645f 7369 6e63  .H..changed_sinc
-00000a40: 655f 7469 6d65 1808 2001 280b 321a 2e67  e_time.. .(.2..g
-00000a50: 6f6f 676c 652e 7072 6f74 6f62 7566 2e54  oogle.protobuf.T
-00000a60: 696d 6573 7461 6d70 5210 6368 616e 6765  imestampR.change
-00000a70: 6453 696e 6365 5469 6d65 1246 0a11 6669  dSinceTime.F..fi
-00000a80: 6e61 6c5f 7265 7375 6c74 5f74 696d 6518  nal_result_time.
-00000a90: 0920 0128 0b32 1a2e 676f 6f67 6c65 2e70  . .(.2..google.p
-00000aa0: 726f 746f 6275 662e 5469 6d65 7374 616d  rotobuf.Timestam
-00000ab0: 7052 0f66 696e 616c 5265 7375 6c74 5469  pR.finalResultTi
-00000ac0: 6d65 1240 0a0b 6372 6561 7465 5f74 696d  me.@..create_tim
-00000ad0: 6518 0a20 0128 0b32 1a2e 676f 6f67 6c65  e.. .(.2..google
-00000ae0: 2e70 726f 746f 6275 662e 5469 6d65 7374  .protobuf.Timest
-00000af0: 616d 7042 03e0 4103 520a 6372 6561 7465  ampB..A.R.create
-00000b00: 5469 6d65 1a2b 0a06 4c69 6d69 7473 1221  Time.+..Limits.!
-00000b10: 0a0c 7072 6576 6965 775f 726f 7773 1801  ..preview_rows..
-00000b20: 2001 2803 520b 7072 6576 6965 7752 6f77   .(.R.previewRow
-00000b30: 731a 290a 1152 6564 6973 4275 6c6b 5265  s.)..RedisBulkRe
-00000b40: 7370 6f6e 7365 1214 0a05 7368 6170 6518  sponse....shape.
-00000b50: 0120 0328 0552 0573 6861 7065 22a0 010a  . .(.R.shape"...
-00000b60: 0e52 6573 756c 7442 6568 6176 696f 7212  .ResultBehavior.
-00000b70: 1f0a 1b52 4553 554c 545f 4245 4841 5649  ...RESULT_BEHAVI
-00000b80: 4f52 5f55 4e53 5045 4349 4649 4544 1000  OR_UNSPECIFIED..
-00000b90: 121f 0a1b 5245 5355 4c54 5f42 4548 4156  ....RESULT_BEHAV
-00000ba0: 494f 525f 414c 4c5f 5245 5355 4c54 5310  IOR_ALL_RESULTS.
-00000bb0: 0112 210a 1d52 4553 554c 545f 4245 4841  ..!..RESULT_BEHA
-00000bc0: 5649 4f52 5f46 494e 414c 5f52 4553 554c  VIOR_FINAL_RESUL
-00000bd0: 5453 1002 1229 0a25 5245 5355 4c54 5f42  TS...).%RESULT_B
-00000be0: 4548 4156 494f 525f 4649 4e41 4c5f 5245  EHAVIOR_FINAL_RE
-00000bf0: 5355 4c54 535f 4154 5f54 494d 4510 034a  SULTS_AT_TIME..J
-00000c00: 0408 6510 664a 0408 6610 674a 0408 6710  ..e.fJ..f.gJ..g.
-00000c10: 6822 ac01 0a0c 5175 6572 794f 7074 696f  h"....QueryOptio
-00000c20: 6e73 1217 0a07 6472 795f 7275 6e18 0120  ns....dry_run.. 
-00000c30: 0128 0852 0664 7279 5275 6e12 330a 1565  .(.R.dryRun.3..e
-00000c40: 7870 6572 696d 656e 7461 6c5f 6665 6174  xperimental_feat
-00000c50: 7572 6573 1802 2001 2808 5214 6578 7065  ures.. .(.R.expe
-00000c60: 7269 6d65 6e74 616c 4665 6174 7572 6573  rimentalFeatures
-00000c70: 1225 0a0e 7374 7265 616d 5f6d 6574 7269  .%..stream_metri
-00000c80: 6373 1803 2001 2808 520d 7374 7265 616d  cs.. .(.R.stream
-00000c90: 4d65 7472 6963 7312 270a 0f70 7265 7369  Metrics.'..presi
-00000ca0: 676e 5f72 6573 756c 7473 1804 2001 2808  gn_results.. .(.
-00000cb0: 520e 7072 6573 6967 6e52 6573 756c 7473  R.presignResults
-00000cc0: 2296 010a 1243 7265 6174 6551 7565 7279  "....CreateQuery
-00000cd0: 5265 7175 6573 7412 340a 0571 7565 7279  Request.4..query
-00000ce0: 1801 2001 280b 321e 2e6b 6173 6b61 6461  .. .(.2..kaskada
-00000cf0: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
-00000d00: 2e51 7565 7279 5205 7175 6572 7912 4a0a  .QueryR.query.J.
-00000d10: 0d71 7565 7279 5f6f 7074 696f 6e73 1802  .query_options..
-00000d20: 2001 280b 3225 2e6b 6173 6b61 6461 2e6b   .(.2%.kaskada.k
-00000d30: 6173 6b61 6461 2e76 3161 6c70 6861 2e51  askada.v1alpha.Q
-00000d40: 7565 7279 4f70 7469 6f6e 7352 0c71 7565  ueryOptionsR.que
-00000d50: 7279 4f70 7469 6f6e 7322 910a 0a13 4372  ryOptions"....Cr
-00000d60: 6561 7465 5175 6572 7952 6573 706f 6e73  eateQueryRespons
-00000d70: 6512 480a 0573 7461 7465 1801 2001 280e  e.H..state.. .(.
-00000d80: 3232 2e6b 6173 6b61 6461 2e6b 6173 6b61  22.kaskada.kaska
-00000d90: 6461 2e76 3161 6c70 6861 2e43 7265 6174  da.v1alpha.Creat
-00000da0: 6551 7565 7279 5265 7370 6f6e 7365 2e53  eQueryResponse.S
-00000db0: 7461 7465 5205 7374 6174 6512 4b0a 0663  tateR.state.K..c
-00000dc0: 6f6e 6669 6718 0220 0128 0b32 332e 6b61  onfig.. .(.23.ka
-00000dd0: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
-00000de0: 616c 7068 612e 4372 6561 7465 5175 6572  alpha.CreateQuer
-00000df0: 7952 6573 706f 6e73 652e 436f 6e66 6967  yResponse.Config
-00000e00: 5206 636f 6e66 6967 1251 0a08 616e 616c  R.config.Q..anal
-00000e10: 7973 6973 1803 2001 280b 3235 2e6b 6173  ysis.. .(.25.kas
-00000e20: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-00000e30: 6c70 6861 2e43 7265 6174 6551 7565 7279  lpha.CreateQuery
-00000e40: 5265 7370 6f6e 7365 2e41 6e61 6c79 7369  Response.Analysi
-00000e50: 7352 0861 6e61 6c79 7369 7312 530a 1066  sR.analysis.S..f
-00000e60: 656e 6c5f 6469 6167 6e6f 7374 6963 7318  enl_diagnostics.
-00000e70: 0420 0128 0b32 282e 6b61 736b 6164 612e  . .(.2(.kaskada.
-00000e80: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
-00000e90: 4665 6e6c 4469 6167 6e6f 7374 6963 7352  FenlDiagnosticsR
-00000ea0: 0f66 656e 6c44 6961 676e 6f73 7469 6373  .fenlDiagnostics
-00000eb0: 124e 0a07 6d65 7472 6963 7318 0520 0128  .N..metrics.. .(
-00000ec0: 0b32 342e 6b61 736b 6164 612e 6b61 736b  .24.kaskada.kask
-00000ed0: 6164 612e 7631 616c 7068 612e 4372 6561  ada.v1alpha.Crea
-00000ee0: 7465 5175 6572 7952 6573 706f 6e73 652e  teQueryResponse.
-00000ef0: 4d65 7472 6963 7352 076d 6574 7269 6373  MetricsR.metrics
-00000f00: 1250 0a0f 7265 7175 6573 745f 6465 7461  .P..request_deta
-00000f10: 696c 7318 0620 0128 0b32 272e 6b61 736b  ils.. .(.2'.kask
-00000f20: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-00000f30: 7068 612e 5265 7175 6573 7444 6574 6169  pha.RequestDetai
-00000f40: 6c73 520e 7265 7175 6573 7444 6574 6169  lsR.requestDetai
-00000f50: 6c73 1219 0a08 7175 6572 795f 6964 1807  ls....query_id..
-00000f60: 2001 2809 5207 7175 6572 7949 6412 460a   .(.R.queryId.F.
-00000f70: 0b64 6573 7469 6e61 7469 6f6e 1868 2001  .destination.h .
-00000f80: 280b 3224 2e6b 6173 6b61 6461 2e6b 6173  (.2$.kaskada.kas
-00000f90: 6b61 6461 2e76 3161 6c70 6861 2e44 6573  kada.v1alpha.Des
-00000fa0: 7469 6e61 7469 6f6e 520b 6465 7374 696e  tinationR.destin
-00000fb0: 6174 696f 6e1a 640a 0841 6e61 6c79 7369  ation.d..Analysi
-00000fc0: 7312 1f0a 0b63 616e 5f65 7865 6375 7465  s....can_execute
-00000fd0: 1801 2001 2808 520a 6361 6e45 7865 6375  .. .(.R.canExecu
-00000fe0: 7465 1237 0a06 7363 6865 6d61 1802 2001  te.7..schema.. .
-00000ff0: 280b 321f 2e6b 6173 6b61 6461 2e6b 6173  (.2..kaskada.kas
-00001000: 6b61 6461 2e76 3161 6c70 6861 2e53 6368  kada.v1alpha.Sch
-00001010: 656d 6152 0673 6368 656d 611a 780a 0643  emaR.schema.x..C
-00001020: 6f6e 6669 6712 220a 0d64 6174 615f 746f  onfig."..data_to
-00001030: 6b65 6e5f 6964 1801 2001 2809 520b 6461  ken_id.. .(.R.da
-00001040: 7461 546f 6b65 6e49 6412 4a0a 0d73 6c69  taTokenId.J..sli
-00001050: 6365 5f72 6571 7565 7374 1802 2001 280b  ce_request.. .(.
-00001060: 3225 2e6b 6173 6b61 6461 2e6b 6173 6b61  2%.kaskada.kaska
-00001070: 6461 2e76 3161 6c70 6861 2e53 6c69 6365  da.v1alpha.Slice
-00001080: 5265 7175 6573 7452 0c73 6c69 6365 5265  RequestR.sliceRe
-00001090: 7175 6573 741a be02 0a07 4d65 7472 6963  quest.....Metric
-000010a0: 7312 400a 0e74 696d 655f 7072 6570 6172  s.@..time_prepar
-000010b0: 696e 6718 0120 0128 0b32 192e 676f 6f67  ing.. .(.2..goog
-000010c0: 6c65 2e70 726f 746f 6275 662e 4475 7261  le.protobuf.Dura
-000010d0: 7469 6f6e 520d 7469 6d65 5072 6570 6172  tionR.timePrepar
-000010e0: 696e 6712 400a 0e74 696d 655f 636f 6d70  ing.@..time_comp
-000010f0: 7574 696e 6718 0220 0128 0b32 192e 676f  uting.. .(.2..go
-00001100: 6f67 6c65 2e70 726f 746f 6275 662e 4475  ogle.protobuf.Du
-00001110: 7261 7469 6f6e 520d 7469 6d65 436f 6d70  rationR.timeComp
-00001120: 7574 696e 6712 210a 0c6f 7574 7075 745f  uting.!..output_
-00001130: 6669 6c65 7318 0320 0128 0352 0b6f 7574  files.. .(.R.out
-00001140: 7075 7446 696c 6573 1228 0a10 746f 7461  putFiles.(..tota
-00001150: 6c5f 696e 7075 745f 726f 7773 1804 2001  l_input_rows.. .
-00001160: 2803 520e 746f 7461 6c49 6e70 7574 526f  (.R.totalInputRo
-00001170: 7773 1230 0a14 7072 6f63 6573 7365 645f  ws.0..processed_
-00001180: 696e 7075 745f 726f 7773 1805 2001 2803  input_rows.. .(.
-00001190: 5212 7072 6f63 6573 7365 6449 6e70 7574  R.processedInput
-000011a0: 526f 7773 1230 0a14 7072 6f64 7563 6564  Rows.0..produced
-000011b0: 5f6f 7574 7075 745f 726f 7773 1806 2001  _output_rows.. .
-000011c0: 2803 5212 7072 6f64 7563 6564 4f75 7470  (.R.producedOutp
-000011d0: 7574 526f 7773 2282 010a 0553 7461 7465  utRows"....State
-000011e0: 1215 0a11 5354 4154 455f 554e 5350 4543  ....STATE_UNSPEC
-000011f0: 4946 4945 4410 0012 120a 0e53 5441 5445  IFIED......STATE
-00001200: 5f41 4e41 4c59 5349 5310 0112 130a 0f53  _ANALYSIS......S
-00001210: 5441 5445 5f50 5245 5041 5249 4e47 1002  TATE_PREPARING..
-00001220: 1213 0a0f 5354 4154 455f 434f 4d50 5554  ....STATE_COMPUT
-00001230: 494e 4710 0312 110a 0d53 5441 5445 5f53  ING......STATE_S
-00001240: 5543 4345 5353 1004 1211 0a0d 5354 4154  UCCESS......STAT
-00001250: 455f 4641 494c 5552 4510 054a 0408 6510  E_FAILURE..J..e.
-00001260: 664a 0408 6610 674a 0408 6710 6822 350a  fJ..f.gJ..g.h"5.
-00001270: 0f47 6574 5175 6572 7952 6571 7565 7374  .GetQueryRequest
-00001280: 1222 0a08 7175 6572 795f 6964 1801 2001  ."..query_id.. .
-00001290: 2809 4207 fa42 0472 0210 0152 0771 7565  (.B..B.r...R.que
-000012a0: 7279 4964 224d 0a10 4765 7451 7565 7279  ryId"M..GetQuery
-000012b0: 5265 7370 6f6e 7365 1239 0a05 7175 6572  Response.9..quer
-000012c0: 7918 0120 0128 0b32 1e2e 6b61 736b 6164  y.. .(.2..kaskad
-000012d0: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
-000012e0: 612e 5175 6572 7942 03e0 4103 5205 7175  a.QueryB..A.R.qu
-000012f0: 6572 7922 740a 124c 6973 7451 7565 7269  ery"t..ListQueri
-00001300: 6573 5265 7175 6573 7412 160a 0673 6561  esRequest....sea
-00001310: 7263 6818 0120 0128 0952 0673 6561 7263  rch.. .(.R.searc
-00001320: 6812 270a 0970 6167 655f 7369 7a65 1802  h.'..page_size..
-00001330: 2001 2805 420a fa42 071a 0518 e807 2800   .(.B..B......(.
-00001340: 5208 7061 6765 5369 7a65 121d 0a0a 7061  R.pageSize....pa
-00001350: 6765 5f74 6f6b 656e 1803 2001 2809 5209  ge_token.. .(.R.
-00001360: 7061 6765 546f 6b65 6e22 c901 0a13 4c69  pageToken"....Li
-00001370: 7374 5175 6572 6965 7352 6573 706f 6e73  stQueriesRespons
-00001380: 6512 380a 0771 7565 7269 6573 1801 2003  e.8..queries.. .
-00001390: 280b 321e 2e6b 6173 6b61 6461 2e6b 6173  (.2..kaskada.kas
-000013a0: 6b61 6461 2e76 3161 6c70 6861 2e51 7565  kada.v1alpha.Que
-000013b0: 7279 5207 7175 6572 6965 7312 260a 0f6e  ryR.queries.&..n
-000013c0: 6578 745f 7061 6765 5f74 6f6b 656e 1802  ext_page_token..
-000013d0: 2001 2809 520d 6e65 7874 5061 6765 546f   .(.R.nextPageTo
-000013e0: 6b65 6e12 500a 0f72 6571 7565 7374 5f64  ken.P..request_d
-000013f0: 6574 6169 6c73 1803 2001 280b 3227 2e6b  etails.. .(.2'.k
-00001400: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
-00001410: 3161 6c70 6861 2e52 6571 7565 7374 4465  1alpha.RequestDe
-00001420: 7461 696c 7352 0e72 6571 7565 7374 4465  tailsR.requestDe
-00001430: 7461 696c 7332 aa03 0a0c 5175 6572 7953  tails2....QueryS
-00001440: 6572 7669 6365 128b 010a 0b43 7265 6174  ervice.....Creat
-00001450: 6551 7565 7279 122b 2e6b 6173 6b61 6461  eQuery.+.kaskada
-00001460: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
-00001470: 2e43 7265 6174 6551 7565 7279 5265 7175  .CreateQueryRequ
-00001480: 6573 741a 2c2e 6b61 736b 6164 612e 6b61  est.,.kaskada.ka
-00001490: 736b 6164 612e 7631 616c 7068 612e 4372  skada.v1alpha.Cr
-000014a0: 6561 7465 5175 6572 7952 6573 706f 6e73  eateQueryRespons
-000014b0: 6522 1f82 d3e4 9302 193a 0571 7565 7279  e".......:.query
-000014c0: 2210 2f76 3161 6c70 6861 2f71 7565 7269  "./v1alpha/queri
-000014d0: 6573 3001 1286 010a 0847 6574 5175 6572  es0......GetQuer
-000014e0: 7912 282e 6b61 736b 6164 612e 6b61 736b  y.(.kaskada.kask
-000014f0: 6164 612e 7631 616c 7068 612e 4765 7451  ada.v1alpha.GetQ
-00001500: 7565 7279 5265 7175 6573 741a 292e 6b61  ueryRequest.).ka
-00001510: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
-00001520: 616c 7068 612e 4765 7451 7565 7279 5265  alpha.GetQueryRe
-00001530: 7370 6f6e 7365 2225 82d3 e493 021f 121d  sponse"%........
-00001540: 2f76 3161 6c70 6861 2f71 7565 7269 6573  /v1alpha/queries
-00001550: 2f7b 7175 6572 795f 6964 3d2a 7d12 8201  /{query_id=*}...
-00001560: 0a0b 4c69 7374 5175 6572 6965 7312 2b2e  ..ListQueries.+.
-00001570: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
-00001580: 7631 616c 7068 612e 4c69 7374 5175 6572  v1alpha.ListQuer
-00001590: 6965 7352 6571 7565 7374 1a2c 2e6b 6173  iesRequest.,.kas
-000015a0: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-000015b0: 6c70 6861 2e4c 6973 7451 7565 7269 6573  lpha.ListQueries
-000015c0: 5265 7370 6f6e 7365 2218 82d3 e493 0212  Response".......
-000015d0: 1210 2f76 3161 6c70 6861 2f71 7565 7269  ../v1alpha/queri
-000015e0: 6573 4281 020a 1b63 6f6d 2e6b 6173 6b61  esB....com.kaska
-000015f0: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-00001600: 6861 4211 5175 6572 7953 6572 7669 6365  haB.QueryService
-00001610: 5072 6f74 6f50 015a 5167 6974 6875 622e  ProtoP.ZQgithub.
-00001620: 636f 6d2f 6b61 736b 6164 612d 6169 2f6b  com/kaskada-ai/k
-00001630: 6173 6b61 6461 2f67 656e 2f70 726f 746f  askada/gen/proto
-00001640: 2f67 6f2f 6b61 736b 6164 612f 6b61 736b  /go/kaskada/kask
-00001650: 6164 612f 7631 616c 7068 613b 6b61 736b  ada/v1alpha;kask
-00001660: 6164 6176 3161 6c70 6861 a202 034b 4b58  adav1alpha...KKX
-00001670: aa02 174b 6173 6b61 6461 2e4b 6173 6b61  ...Kaskada.Kaska
-00001680: 6461 2e56 3161 6c70 6861 ca02 174b 6173  da.V1alpha...Kas
-00001690: 6b61 6461 5c4b 6173 6b61 6461 5c56 3161  kada\Kaskada\V1a
-000016a0: 6c70 6861 e202 234b 6173 6b61 6461 5c4b  lpha..#Kaskada\K
-000016b0: 6173 6b61 6461 5c56 3161 6c70 6861 5c47  askada\V1alpha\G
-000016c0: 5042 4d65 7461 6461 7461 ea02 194b 6173  PBMetadata...Kas
-000016d0: 6b61 6461 3a3a 4b61 736b 6164 613a 3a56  kada::Kaskada::V
-000016e0: 3161 6c70 6861 6206 7072 6f74 6f33 da05  1alphab.proto3..
-000016f0: 5175 6572 79da 064c 696d 6974 73da 1152  Query..Limits..R
-00001700: 6564 6973 4275 6c6b 5265 7370 6f6e 7365  edisBulkResponse
-00001710: da0c 5175 6572 794f 7074 696f 6e73 da12  ..QueryOptions..
-00001720: 4372 6561 7465 5175 6572 7952 6571 7565  CreateQueryReque
-00001730: 7374 da13 4372 6561 7465 5175 6572 7952  st..CreateQueryR
-00001740: 6573 706f 6e73 65da 0841 6e61 6c79 7369  esponse..Analysi
-00001750: 73da 0643 6f6e 6669 67da 074d 6574 7269  s..Config..Metri
-00001760: 6373 da0f 4765 7451 7565 7279 5265 7175  cs..GetQueryRequ
-00001770: 6573 74da 1047 6574 5175 6572 7952 6573  est..GetQueryRes
-00001780: 706f 6e73 65da 124c 6973 7451 7565 7269  ponse..ListQueri
-00001790: 6573 5265 7175 6573 74da 134c 6973 7451  esRequest..ListQ
-000017a0: 7565 7269 6573 5265 7370 6f6e 7365 da0e  ueriesResponse..
-000017b0: 5265 7375 6c74 4265 6861 7669 6f72 da05  ResultBehavior..
-000017c0: 5374 6174 657a 296b 6173 6b61 6461 2e6b  Statez)kaskada.k
-000017d0: 6173 6b61 6461 2e76 3161 6c70 6861 2e71  askada.v1alpha.q
-000017e0: 7565 7279 5f73 6572 7669 6365 5f70 6232  uery_service_pb2
-000017f0: 2902 da0a 4445 5343 5249 5054 4f52 da0a  )...DESCRIPTOR..
-00001800: 5f5f 6d6f 6475 6c65 5f5f 2904 7213 0000  __module__).r...
-00001810: 0072 1400 0000 7221 0000 0072 2200 0000  .r....r!...r"...
-00001820: 2905 7218 0000 0072 1900 0000 721a 0000  ).r....r....r...
-00001830: 0072 2100 0000 7222 0000 00da 0c51 7565  .r!...r".....Que
-00001840: 7279 5365 7276 6963 6546 4e73 0101 0000  ryServiceFNs....
-00001850: 0a1b 636f 6d2e 6b61 736b 6164 612e 6b61  ..com.kaskada.ka
-00001860: 736b 6164 612e 7631 616c 7068 6142 1151  skada.v1alphaB.Q
-00001870: 7565 7279 5365 7276 6963 6550 726f 746f  ueryServiceProto
-00001880: 5001 5a51 6769 7468 7562 2e63 6f6d 2f6b  P.ZQgithub.com/k
-00001890: 6173 6b61 6461 2d61 692f 6b61 736b 6164  askada-ai/kaskad
-000018a0: 612f 6765 6e2f 7072 6f74 6f2f 676f 2f6b  a/gen/proto/go/k
-000018b0: 6173 6b61 6461 2f6b 6173 6b61 6461 2f76  askada/kaskada/v
-000018c0: 3161 6c70 6861 3b6b 6173 6b61 6461 7631  1alpha;kaskadav1
-000018d0: 616c 7068 61a2 0203 4b4b 58aa 0217 4b61  alpha...KKX...Ka
-000018e0: 736b 6164 612e 4b61 736b 6164 612e 5631  skada.Kaskada.V1
-000018f0: 616c 7068 61ca 0217 4b61 736b 6164 615c  alpha...Kaskada\
-00001900: 4b61 736b 6164 615c 5631 616c 7068 61e2  Kaskada\V1alpha.
-00001910: 0223 4b61 736b 6164 615c 4b61 736b 6164  .#Kaskada\Kaskad
-00001920: 615c 5631 616c 7068 615c 4750 424d 6574  a\V1alpha\GPBMet
-00001930: 6164 6174 61ea 0219 4b61 736b 6164 613a  adata...Kaskada:
-00001940: 3a4b 6173 6b61 6461 3a3a 5631 616c 7068  :Kaskada::V1alph
-00001950: 61da 0871 7565 7279 5f69 6473 0300 0000  a..query_ids....
-00001960: e041 03da 0a65 7870 7265 7373 696f 6e73  .A...expressions
-00001970: 0700 0000 fa42 0472 0210 01da 0576 6965  .....B.r.....vie
-00001980: 7773 da0b 6372 6561 7465 5f74 696d 65da  ws..create_time.
-00001990: 0571 7565 7279 da09 7061 6765 5f73 697a  .query..page_siz
-000019a0: 6573 0a00 0000 fa42 071a 0518 e807 2800  es.....B......(.
-000019b0: da0b 4372 6561 7465 5175 6572 7973 1f00  ..CreateQuerys..
-000019c0: 0000 82d3 e493 0219 3a05 7175 6572 7922  ........:.query"
-000019d0: 102f 7631 616c 7068 612f 7175 6572 6965  ./v1alpha/querie
-000019e0: 73da 0847 6574 5175 6572 7973 2500 0000  s..GetQuerys%...
-000019f0: 82d3 e493 021f 121d 2f76 3161 6c70 6861  ......../v1alpha
-00001a00: 2f71 7565 7269 6573 2f7b 7175 6572 795f  /queries/{query_
-00001a10: 6964 3d2a 7dda 0b4c 6973 7451 7565 7269  id=*}..ListQueri
-00001a20: 6573 7318 0000 0082 d3e4 9302 1212 102f  ess............/
-00001a30: 7631 616c 7068 612f 7175 6572 6965 7369  v1alpha/queriesi
-00001a40: d601 0000 699f 0500 0069 9404 0000 69bf  ....i....i....i.
-00001a50: 0400 0069 c104 0000 69ea 0400 0069 ed04  ...i....i....i..
-00001a60: 0000 698d 0500 0069 a205 0000 694e 0600  ..i....i....iN..
-00001a70: 0069 5106 0000 69e7 0600 0069 ea06 0000  .iQ...i....i....
-00001a80: 69fb 0b00 0069 4509 0000 69a9 0900 0069  i....iE...i....i
-00001a90: ab09 0000 6923 0a00 0069 260a 0000 6964  ....i#...i&...id
-00001aa0: 0b00 0069 670b 0000 69e9 0b00 0069 fd0b  ...ig...i....i..
-00001ab0: 0000 6932 0c00 0069 340c 0000 6981 0c00  ..i2...i4...i...
-00001ac0: 0069 830c 0000 69f7 0c00 0069 fa0c 0000  .i....i....i....
-00001ad0: 69c3 0d00 0069 c60d 0000 6970 0f00 0029  i....i....ip...)
-00001ae0: 54da 075f 5f64 6f63 5f5f da0f 676f 6f67  T..__doc__..goog
-00001af0: 6c65 2e70 726f 746f 6275 6672 0200 0000  le.protobufr....
-00001b00: da0b 5f64 6573 6372 6970 746f 7272 0300  .._descriptorr..
-00001b10: 0000 da10 5f64 6573 6372 6970 746f 725f  ...._descriptor_
-00001b20: 706f 6f6c 7204 0000 00da 085f 6d65 7373  poolr......_mess
-00001b30: 6167 6572 0500 0000 da0b 5f72 6566 6c65  ager......_refle
-00001b40: 6374 696f 6e72 0600 0000 da10 5f73 796d  ctionr......_sym
-00001b50: 626f 6c5f 6461 7461 6261 7365 da07 4465  bol_database..De
-00001b60: 6661 756c 74da 075f 7379 6d5f 6462 da0a  fault.._sym_db..
-00001b70: 676f 6f67 6c65 2e61 7069 7207 0000 00da  google.apir.....
-00001b80: 2367 6f6f 676c 655f 646f 745f 6170 695f  #google_dot_api_
-00001b90: 646f 745f 616e 6e6f 7461 7469 6f6e 735f  dot_annotations_
-00001ba0: 5f70 6232 7208 0000 00da 2767 6f6f 676c  _pb2r.....'googl
-00001bb0: 655f 646f 745f 6170 695f 646f 745f 6669  e_dot_api_dot_fi
-00001bc0: 656c 645f 5f62 6568 6176 696f 725f 5f70  eld__behavior__p
-00001bd0: 6232 7209 0000 00da 2567 6f6f 676c 655f  b2r.....%google_
-00001be0: 646f 745f 7072 6f74 6f62 7566 5f64 6f74  dot_protobuf_dot
-00001bf0: 5f64 7572 6174 696f 6e5f 5f70 6232 720a  _duration__pb2r.
-00001c00: 0000 00da 2667 6f6f 676c 655f 646f 745f  ....&google_dot_
-00001c10: 7072 6f74 6f62 7566 5f64 6f74 5f74 696d  protobuf_dot_tim
-00001c20: 6573 7461 6d70 5f5f 7062 3272 0b00 0000  estamp__pb2r....
-00001c30: da25 676f 6f67 6c65 5f64 6f74 5f70 726f  .%google_dot_pro
-00001c40: 746f 6275 665f 646f 745f 7772 6170 7065  tobuf_dot_wrappe
-00001c50: 7273 5f5f 7062 32da 176b 6173 6b61 6461  rs__pb2..kaskada
-00001c60: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
-00001c70: 720c 0000 00da 2f6b 6173 6b61 6461 5f64  r...../kaskada_d
-00001c80: 6f74 5f6b 6173 6b61 6461 5f64 6f74 5f76  ot_kaskada_dot_v
-00001c90: 3161 6c70 6861 5f64 6f74 5f63 6f6d 6d6f  1alpha_dot_commo
-00001ca0: 6e5f 5f70 6232 720d 0000 00da 356b 6173  n__pb2r.....5kas
-00001cb0: 6b61 6461 5f64 6f74 5f6b 6173 6b61 6461  kada_dot_kaskada
-00001cc0: 5f64 6f74 5f76 3161 6c70 6861 5f64 6f74  _dot_v1alpha_dot
-00001cd0: 5f64 6573 7469 6e61 7469 6f6e 735f 5f70  _destinations__p
-00001ce0: 6232 720e 0000 00da 3a6b 6173 6b61 6461  b2r.....:kaskada
-00001cf0: 5f64 6f74 5f6b 6173 6b61 6461 5f64 6f74  _dot_kaskada_dot
-00001d00: 5f76 3161 6c70 6861 5f64 6f74 5f66 656e  _v1alpha_dot_fen
-00001d10: 6c5f 5f64 6961 676e 6f73 7469 6373 5f5f  l__diagnostics__
-00001d20: 7062 3272 0f00 0000 da2f 6b61 736b 6164  pb2r...../kaskad
-00001d30: 615f 646f 745f 6b61 736b 6164 615f 646f  a_dot_kaskada_do
-00001d40: 745f 7631 616c 7068 615f 646f 745f 7363  t_v1alpha_dot_sc
-00001d50: 6865 6d61 5f5f 7062 3272 1000 0000 da36  hema__pb2r.....6
-00001d60: 6b61 736b 6164 615f 646f 745f 6b61 736b  kaskada_dot_kask
-00001d70: 6164 615f 646f 745f 7631 616c 7068 615f  ada_dot_v1alpha_
-00001d80: 646f 745f 7669 6577 5f5f 7365 7276 6963  dot_view__servic
-00001d90: 655f 5f70 6232 da08 7661 6c69 6461 7465  e__pb2..validate
-00001da0: 7211 0000 00da 1a76 616c 6964 6174 655f  r......validate_
-00001db0: 646f 745f 7661 6c69 6461 7465 5f5f 7062  dot_validate__pb
-00001dc0: 32da 1141 6464 5365 7269 616c 697a 6564  2..AddSerialized
-00001dd0: 4669 6c65 7221 0000 00da 156d 6573 7361  Filer!.....messa
-00001de0: 6765 5f74 7970 6573 5f62 795f 6e61 6d65  ge_types_by_name
-00001df0: da06 5f51 5545 5259 da14 6e65 7374 6564  .._QUERY..nested
-00001e00: 5f74 7970 6573 5f62 795f 6e61 6d65 da0d  _types_by_name..
-00001e10: 5f51 5545 5259 5f4c 494d 4954 53da 185f  _QUERY_LIMITS.._
-00001e20: 5155 4552 595f 5245 4449 5342 554c 4b52  QUERY_REDISBULKR
-00001e30: 4553 504f 4e53 45da 0d5f 5155 4552 594f  ESPONSE.._QUERYO
-00001e40: 5054 494f 4e53 da13 5f43 5245 4154 4551  PTIONS.._CREATEQ
-00001e50: 5545 5259 5245 5155 4553 54da 145f 4352  UERYREQUEST.._CR
-00001e60: 4541 5445 5155 4552 5952 4553 504f 4e53  EATEQUERYRESPONS
-00001e70: 45da 1d5f 4352 4541 5445 5155 4552 5952  E.._CREATEQUERYR
-00001e80: 4553 504f 4e53 455f 414e 414c 5953 4953  ESPONSE_ANALYSIS
-00001e90: da1b 5f43 5245 4154 4551 5545 5259 5245  .._CREATEQUERYRE
-00001ea0: 5350 4f4e 5345 5f43 4f4e 4649 47da 1c5f  SPONSE_CONFIG.._
-00001eb0: 4352 4541 5445 5155 4552 5952 4553 504f  CREATEQUERYRESPO
-00001ec0: 4e53 455f 4d45 5452 4943 53da 105f 4745  NSE_METRICS.._GE
-00001ed0: 5451 5545 5259 5245 5155 4553 54da 115f  TQUERYREQUEST.._
-00001ee0: 4745 5451 5545 5259 5245 5350 4f4e 5345  GETQUERYRESPONSE
-00001ef0: da13 5f4c 4953 5451 5545 5249 4553 5245  .._LISTQUERIESRE
-00001f00: 5155 4553 54da 145f 4c49 5354 5155 4552  QUEST.._LISTQUER
-00001f10: 4945 5352 4553 504f 4e53 45da 1265 6e75  IESRESPONSE..enu
-00001f20: 6d5f 7479 7065 735f 6279 5f6e 616d 65da  m_types_by_name.
-00001f30: 155f 5155 4552 595f 5245 5355 4c54 4245  ._QUERY_RESULTBE
-00001f40: 4841 5649 4f52 da1a 5f43 5245 4154 4551  HAVIOR.._CREATEQ
-00001f50: 5545 5259 5245 5350 4f4e 5345 5f53 5441  UERYRESPONSE_STA
-00001f60: 5445 da1c 4765 6e65 7261 7465 6450 726f  TE..GeneratedPro
-00001f70: 746f 636f 6c4d 6573 7361 6765 5479 7065  tocolMessageType
-00001f80: da07 4d65 7373 6167 6572 1200 0000 da0f  ..Messager......
-00001f90: 5265 6769 7374 6572 4d65 7373 6167 6572  RegisterMessager
-00001fa0: 1300 0000 7214 0000 0072 1500 0000 7216  ....r....r....r.
-00001fb0: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
-00001fc0: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00001fd0: 0072 1d00 0000 721e 0000 00da 1073 6572  .r....r......ser
-00001fe0: 7669 6365 735f 6279 5f6e 616d 65da 0d5f  vices_by_name.._
-00001ff0: 5155 4552 5953 4552 5649 4345 da12 5f55  QUERYSERVICE.._U
-00002000: 5345 5f43 5f44 4553 4352 4950 544f 5253  SE_C_DESCRIPTORS
-00002010: da08 5f6f 7074 696f 6e73 da13 5f73 6572  .._options.._ser
-00002020: 6961 6c69 7a65 645f 6f70 7469 6f6e 73da  ialized_options.
-00002030: 0e66 6965 6c64 735f 6279 5f6e 616d 65da  .fields_by_name.
-00002040: 0f6d 6574 686f 6473 5f62 795f 6e61 6d65  .methods_by_name
-00002050: da11 5f73 6572 6961 6c69 7a65 645f 7374  .._serialized_st
-00002060: 6172 74da 0f5f 7365 7269 616c 697a 6564  art.._serialized
-00002070: 5f65 6e64 a900 7263 0000 0072 6300 0000  _end..rc...rc...
-00002080: fa77 2f68 6f6d 652f 7468 6572 6170 6f6e  .w/home/therapon
-00002090: 2f52 6570 6f73 2f47 6974 4875 622f 4b61  /Repos/GitHub/Ka
-000020a0: 736b 6164 6141 492f 6b61 736b 6164 612f  skadaAI/kaskada/
-000020b0: 7265 6c65 6173 696e 672f 636c 6965 6e74  releasing/client
-000020c0: 732f 7079 7468 6f6e 2f73 7263 2f6b 6173  s/python/src/kas
-000020d0: 6b61 6461 2f6b 6173 6b61 6461 2f76 3161  kada/kaskada/v1a
-000020e0: 6c70 6861 2f71 7565 7279 5f73 6572 7669  lpha/query_servi
-000020f0: 6365 5f70 6232 2e70 79da 083c 6d6f 6475  ce_pb2.py..<modu
-00002100: 6c65 3e01 0000 0073 3801 0000 0403 0c01  le>....s8.......
-00002110: 0c01 0c01 0c01 0c01 0803 0c03 0c01 0c01  ................
-00002120: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00002130: 0e03 0a04 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00002140: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00002150: 0c01 0c02 0201 0201 06fe 0c07 0201 0201  ................
-00002160: 06fe 0206 0201 08f0 0a13 0c01 0c01 0c02  ................
-00002170: 0201 0201 08fe 0a05 0c02 0201 0201 08fe  ................
-00002180: 0a05 0c02 0c02 0201 0201 06fe 0c07 0201  ................
-00002190: 0201 06fe 0c07 0201 0201 06fe 0206 0201  ................
-000021a0: 08e9 0a1a 0c01 0c01 0c01 0c02 0201 0201  ................
-000021b0: 08fe 0a05 0c02 0201 0201 08fe 0a05 0c02  ................
-000021c0: 0201 0201 08fe 0a05 0c02 0201 0201 08fe  ................
-000021d0: 0a05 0a02 0c01 0602 0601 0c01 0c01 0c01  ................
-000021e0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000021f0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00002200: 0c01 0601 0601 0601 0601 0601 0601 0601  ................
-00002210: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00002220: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00002230: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00002240: 0a01 04c9                                ....
+00000520: 654c 5f52 6458 654c 5f53 6428 5300 2959  eL_RdXeL_Sd(S.)Y
+00000530: 7a1f 4765 6e65 7261 7465 6420 7072 6f74  z.Generated prot
+00000540: 6f63 6f6c 2062 7566 6665 7220 636f 6465  ocol buffer code
+00000550: 2ee9 0000 0000 2901 da0a 6465 7363 7269  ......)...descri
+00000560: 7074 6f72 2901 da0f 6465 7363 7269 7074  ptor)...descript
+00000570: 6f72 5f70 6f6f 6c29 01da 076d 6573 7361  or_pool)...messa
+00000580: 6765 2901 da0a 7265 666c 6563 7469 6f6e  ge)...reflection
+00000590: 2901 da0f 7379 6d62 6f6c 5f64 6174 6162  )...symbol_datab
+000005a0: 6173 6529 01da 0f61 6e6e 6f74 6174 696f  ase)...annotatio
+000005b0: 6e73 5f70 6232 2901 da12 6669 656c 645f  ns_pb2)...field_
+000005c0: 6265 6861 7669 6f72 5f70 6232 2901 da0c  behavior_pb2)...
+000005d0: 6475 7261 7469 6f6e 5f70 6232 2901 da0d  duration_pb2)...
+000005e0: 7469 6d65 7374 616d 705f 7062 3229 01da  timestamp_pb2)..
+000005f0: 0c77 7261 7070 6572 735f 7062 3229 01da  .wrappers_pb2)..
+00000600: 0a63 6f6d 6d6f 6e5f 7062 3229 01da 1064  .common_pb2)...d
+00000610: 6573 7469 6e61 7469 6f6e 735f 7062 3229  estinations_pb2)
+00000620: 01da 1466 656e 6c5f 6469 6167 6e6f 7374  ...fenl_diagnost
+00000630: 6963 735f 7062 3229 01da 0a73 6368 656d  ics_pb2)...schem
+00000640: 615f 7062 3229 01da 1076 6965 775f 7365  a_pb2)...view_se
+00000650: 7276 6963 655f 7062 3229 01da 0c76 616c  rvice_pb2)...val
+00000660: 6964 6174 655f 7062 3273 7c10 0000 0a2b  idate_pb2s|....+
+00000670: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
+00000680: 7631 616c 7068 612f 7175 6572 795f 7365  v1alpha/query_se
+00000690: 7276 6963 652e 7072 6f74 6f12 176b 6173  rvice.proto..kas
+000006a0: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
+000006b0: 6c70 6861 1a1c 676f 6f67 6c65 2f61 7069  lpha..google/api
+000006c0: 2f61 6e6e 6f74 6174 696f 6e73 2e70 726f  /annotations.pro
+000006d0: 746f 1a1f 676f 6f67 6c65 2f61 7069 2f66  to..google/api/f
+000006e0: 6965 6c64 5f62 6568 6176 696f 722e 7072  ield_behavior.pr
+000006f0: 6f74 6f1a 1e67 6f6f 676c 652f 7072 6f74  oto..google/prot
+00000700: 6f62 7566 2f64 7572 6174 696f 6e2e 7072  obuf/duration.pr
+00000710: 6f74 6f1a 1f67 6f6f 676c 652f 7072 6f74  oto..google/prot
+00000720: 6f62 7566 2f74 696d 6573 7461 6d70 2e70  obuf/timestamp.p
+00000730: 726f 746f 1a1e 676f 6f67 6c65 2f70 726f  roto..google/pro
+00000740: 746f 6275 662f 7772 6170 7065 7273 2e70  tobuf/wrappers.p
+00000750: 726f 746f 1a24 6b61 736b 6164 612f 6b61  roto.$kaskada/ka
+00000760: 736b 6164 612f 7631 616c 7068 612f 636f  skada/v1alpha/co
+00000770: 6d6d 6f6e 2e70 726f 746f 1a2a 6b61 736b  mmon.proto.*kask
+00000780: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
+00000790: 7068 612f 6465 7374 696e 6174 696f 6e73  pha/destinations
+000007a0: 2e70 726f 746f 1a2e 6b61 736b 6164 612f  .proto..kaskada/
+000007b0: 6b61 736b 6164 612f 7631 616c 7068 612f  kaskada/v1alpha/
+000007c0: 6665 6e6c 5f64 6961 676e 6f73 7469 6373  fenl_diagnostics
+000007d0: 2e70 726f 746f 1a24 6b61 736b 6164 612f  .proto.$kaskada/
+000007e0: 6b61 736b 6164 612f 7631 616c 7068 612f  kaskada/v1alpha/
+000007f0: 7363 6865 6d61 2e70 726f 746f 1a2a 6b61  schema.proto.*ka
+00000800: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
+00000810: 616c 7068 612f 7669 6577 5f73 6572 7669  alpha/view_servi
+00000820: 6365 2e70 726f 746f 1a17 7661 6c69 6461  ce.proto..valida
+00000830: 7465 2f76 616c 6964 6174 652e 7072 6f74  te/validate.prot
+00000840: 6f22 c907 0a05 5175 6572 7912 1e0a 0871  o"....Query....q
+00000850: 7565 7279 5f69 6418 0120 0128 0942 03e0  uery_id.. .(.B..
+00000860: 4103 5207 7175 6572 7949 6412 270a 0a65  A.R.queryId.'..e
+00000870: 7870 7265 7373 696f 6e18 0220 0128 0942  xpression.. .(.B
+00000880: 07fa 4204 7202 1001 520a 6578 7072 6573  ..B.r...R.expres
+00000890: 7369 6f6e 1246 0a0b 6465 7374 696e 6174  sion.F..destinat
+000008a0: 696f 6e18 6820 0128 0b32 242e 6b61 736b  ion.h .(.2$.kask
+000008b0: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
+000008c0: 7068 612e 4465 7374 696e 6174 696f 6e52  pha.DestinationR
+000008d0: 0b64 6573 7469 6e61 7469 6f6e 1240 0a0d  .destination.@..
+000008e0: 6461 7461 5f74 6f6b 656e 5f69 6418 0320  data_token_id.. 
+000008f0: 0128 0b32 1c2e 676f 6f67 6c65 2e70 726f  .(.2..google.pro
+00000900: 746f 6275 662e 5374 7269 6e67 5661 6c75  tobuf.StringValu
+00000910: 6552 0b64 6174 6154 6f6b 656e 4964 1238  eR.dataTokenId.8
+00000920: 0a05 7669 6577 7318 0420 0328 0b32 1d2e  ..views.. .(.2..
+00000930: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000940: 7631 616c 7068 612e 5669 6577 4203 e041  v1alpha.ViewB..A
+00000950: 0352 0576 6965 7773 1256 0a0f 7265 7375  .R.views.V..resu
+00000960: 6c74 5f62 6568 6176 696f 7218 0520 0128  lt_behavior.. .(
+00000970: 0e32 2d2e 6b61 736b 6164 612e 6b61 736b  .2-.kaskada.kask
+00000980: 6164 612e 7631 616c 7068 612e 5175 6572  ada.v1alpha.Quer
+00000990: 792e 5265 7375 6c74 4265 6861 7669 6f72  y.ResultBehavior
+000009a0: 520e 7265 7375 6c74 4265 6861 7669 6f72  R.resultBehavior
+000009b0: 123d 0a06 6c69 6d69 7473 1806 2001 280b  .=..limits.. .(.
+000009c0: 3225 2e6b 6173 6b61 6461 2e6b 6173 6b61  2%.kaskada.kaska
+000009d0: 6461 2e76 3161 6c70 6861 2e51 7565 7279  da.v1alpha.Query
+000009e0: 2e4c 696d 6974 7352 066c 696d 6974 7312  .LimitsR.limits.
+000009f0: 3b0a 0573 6c69 6365 1807 2001 280b 3225  ;..slice.. .(.2%
+00000a00: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00000a10: 2e76 3161 6c70 6861 2e53 6c69 6365 5265  .v1alpha.SliceRe
+00000a20: 7175 6573 7452 0573 6c69 6365 1248 0a12  questR.slice.H..
+00000a30: 6368 616e 6765 645f 7369 6e63 655f 7469  changed_since_ti
+00000a40: 6d65 1808 2001 280b 321a 2e67 6f6f 676c  me.. .(.2..googl
+00000a50: 652e 7072 6f74 6f62 7566 2e54 696d 6573  e.protobuf.Times
+00000a60: 7461 6d70 5210 6368 616e 6765 6453 696e  tampR.changedSin
+00000a70: 6365 5469 6d65 1246 0a11 6669 6e61 6c5f  ceTime.F..final_
+00000a80: 7265 7375 6c74 5f74 696d 6518 0920 0128  result_time.. .(
+00000a90: 0b32 1a2e 676f 6f67 6c65 2e70 726f 746f  .2..google.proto
+00000aa0: 6275 662e 5469 6d65 7374 616d 7052 0f66  buf.TimestampR.f
+00000ab0: 696e 616c 5265 7375 6c74 5469 6d65 1240  inalResultTime.@
+00000ac0: 0a0b 6372 6561 7465 5f74 696d 6518 0a20  ..create_time.. 
+00000ad0: 0128 0b32 1a2e 676f 6f67 6c65 2e70 726f  .(.2..google.pro
+00000ae0: 746f 6275 662e 5469 6d65 7374 616d 7042  tobuf.TimestampB
+00000af0: 03e0 4103 520a 6372 6561 7465 5469 6d65  ..A.R.createTime
+00000b00: 1a2b 0a06 4c69 6d69 7473 1221 0a0c 7072  .+..Limits.!..pr
+00000b10: 6576 6965 775f 726f 7773 1801 2001 2803  eview_rows.. .(.
+00000b20: 520b 7072 6576 6965 7752 6f77 731a 290a  R.previewRows.).
+00000b30: 1152 6564 6973 4275 6c6b 5265 7370 6f6e  .RedisBulkRespon
+00000b40: 7365 1214 0a05 7368 6170 6518 0120 0328  se....shape.. .(
+00000b50: 0552 0573 6861 7065 22a0 010a 0e52 6573  .R.shape"....Res
+00000b60: 756c 7442 6568 6176 696f 7212 1f0a 1b52  ultBehavior....R
+00000b70: 4553 554c 545f 4245 4841 5649 4f52 5f55  ESULT_BEHAVIOR_U
+00000b80: 4e53 5045 4349 4649 4544 1000 121f 0a1b  NSPECIFIED......
+00000b90: 5245 5355 4c54 5f42 4548 4156 494f 525f  RESULT_BEHAVIOR_
+00000ba0: 414c 4c5f 5245 5355 4c54 5310 0112 210a  ALL_RESULTS...!.
+00000bb0: 1d52 4553 554c 545f 4245 4841 5649 4f52  .RESULT_BEHAVIOR
+00000bc0: 5f46 494e 414c 5f52 4553 554c 5453 1002  _FINAL_RESULTS..
+00000bd0: 1229 0a25 5245 5355 4c54 5f42 4548 4156  .).%RESULT_BEHAV
+00000be0: 494f 525f 4649 4e41 4c5f 5245 5355 4c54  IOR_FINAL_RESULT
+00000bf0: 535f 4154 5f54 494d 4510 034a 0408 6510  S_AT_TIME..J..e.
+00000c00: 664a 0408 6610 674a 0408 6710 6822 ac01  fJ..f.gJ..g.h"..
+00000c10: 0a0c 5175 6572 794f 7074 696f 6e73 1217  ..QueryOptions..
+00000c20: 0a07 6472 795f 7275 6e18 0120 0128 0852  ..dry_run.. .(.R
+00000c30: 0664 7279 5275 6e12 330a 1565 7870 6572  .dryRun.3..exper
+00000c40: 696d 656e 7461 6c5f 6665 6174 7572 6573  imental_features
+00000c50: 1802 2001 2808 5214 6578 7065 7269 6d65  .. .(.R.experime
+00000c60: 6e74 616c 4665 6174 7572 6573 1225 0a0e  ntalFeatures.%..
+00000c70: 7374 7265 616d 5f6d 6574 7269 6373 1803  stream_metrics..
+00000c80: 2001 2808 520d 7374 7265 616d 4d65 7472   .(.R.streamMetr
+00000c90: 6963 7312 270a 0f70 7265 7369 676e 5f72  ics.'..presign_r
+00000ca0: 6573 756c 7473 1804 2001 2808 520e 7072  esults.. .(.R.pr
+00000cb0: 6573 6967 6e52 6573 756c 7473 2296 010a  esignResults"...
+00000cc0: 1243 7265 6174 6551 7565 7279 5265 7175  .CreateQueryRequ
+00000cd0: 6573 7412 340a 0571 7565 7279 1801 2001  est.4..query.. .
+00000ce0: 280b 321e 2e6b 6173 6b61 6461 2e6b 6173  (.2..kaskada.kas
+00000cf0: 6b61 6461 2e76 3161 6c70 6861 2e51 7565  kada.v1alpha.Que
+00000d00: 7279 5205 7175 6572 7912 4a0a 0d71 7565  ryR.query.J..que
+00000d10: 7279 5f6f 7074 696f 6e73 1802 2001 280b  ry_options.. .(.
+00000d20: 3225 2e6b 6173 6b61 6461 2e6b 6173 6b61  2%.kaskada.kaska
+00000d30: 6461 2e76 3161 6c70 6861 2e51 7565 7279  da.v1alpha.Query
+00000d40: 4f70 7469 6f6e 7352 0c71 7565 7279 4f70  OptionsR.queryOp
+00000d50: 7469 6f6e 7322 910a 0a13 4372 6561 7465  tions"....Create
+00000d60: 5175 6572 7952 6573 706f 6e73 6512 480a  QueryResponse.H.
+00000d70: 0573 7461 7465 1801 2001 280e 3232 2e6b  .state.. .(.22.k
+00000d80: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
+00000d90: 3161 6c70 6861 2e43 7265 6174 6551 7565  1alpha.CreateQue
+00000da0: 7279 5265 7370 6f6e 7365 2e53 7461 7465  ryResponse.State
+00000db0: 5205 7374 6174 6512 4b0a 0663 6f6e 6669  R.state.K..confi
+00000dc0: 6718 0220 0128 0b32 332e 6b61 736b 6164  g.. .(.23.kaskad
+00000dd0: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00000de0: 612e 4372 6561 7465 5175 6572 7952 6573  a.CreateQueryRes
+00000df0: 706f 6e73 652e 436f 6e66 6967 5206 636f  ponse.ConfigR.co
+00000e00: 6e66 6967 1251 0a08 616e 616c 7973 6973  nfig.Q..analysis
+00000e10: 1803 2001 280b 3235 2e6b 6173 6b61 6461  .. .(.25.kaskada
+00000e20: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00000e30: 2e43 7265 6174 6551 7565 7279 5265 7370  .CreateQueryResp
+00000e40: 6f6e 7365 2e41 6e61 6c79 7369 7352 0861  onse.AnalysisR.a
+00000e50: 6e61 6c79 7369 7312 530a 1066 656e 6c5f  nalysis.S..fenl_
+00000e60: 6469 6167 6e6f 7374 6963 7318 0420 0128  diagnostics.. .(
+00000e70: 0b32 282e 6b61 736b 6164 612e 6b61 736b  .2(.kaskada.kask
+00000e80: 6164 612e 7631 616c 7068 612e 4665 6e6c  ada.v1alpha.Fenl
+00000e90: 4469 6167 6e6f 7374 6963 7352 0f66 656e  DiagnosticsR.fen
+00000ea0: 6c44 6961 676e 6f73 7469 6373 124e 0a07  lDiagnostics.N..
+00000eb0: 6d65 7472 6963 7318 0520 0128 0b32 342e  metrics.. .(.24.
+00000ec0: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000ed0: 7631 616c 7068 612e 4372 6561 7465 5175  v1alpha.CreateQu
+00000ee0: 6572 7952 6573 706f 6e73 652e 4d65 7472  eryResponse.Metr
+00000ef0: 6963 7352 076d 6574 7269 6373 1250 0a0f  icsR.metrics.P..
+00000f00: 7265 7175 6573 745f 6465 7461 696c 7318  request_details.
+00000f10: 0620 0128 0b32 272e 6b61 736b 6164 612e  . .(.2'.kaskada.
+00000f20: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
+00000f30: 5265 7175 6573 7444 6574 6169 6c73 520e  RequestDetailsR.
+00000f40: 7265 7175 6573 7444 6574 6169 6c73 1219  requestDetails..
+00000f50: 0a08 7175 6572 795f 6964 1807 2001 2809  ..query_id.. .(.
+00000f60: 5207 7175 6572 7949 6412 460a 0b64 6573  R.queryId.F..des
+00000f70: 7469 6e61 7469 6f6e 1868 2001 280b 3224  tination.h .(.2$
+00000f80: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00000f90: 2e76 3161 6c70 6861 2e44 6573 7469 6e61  .v1alpha.Destina
+00000fa0: 7469 6f6e 520b 6465 7374 696e 6174 696f  tionR.destinatio
+00000fb0: 6e1a 640a 0841 6e61 6c79 7369 7312 1f0a  n.d..Analysis...
+00000fc0: 0b63 616e 5f65 7865 6375 7465 1801 2001  .can_execute.. .
+00000fd0: 2808 520a 6361 6e45 7865 6375 7465 1237  (.R.canExecute.7
+00000fe0: 0a06 7363 6865 6d61 1802 2001 280b 321f  ..schema.. .(.2.
+00000ff0: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00001000: 2e76 3161 6c70 6861 2e53 6368 656d 6152  .v1alpha.SchemaR
+00001010: 0673 6368 656d 611a 780a 0643 6f6e 6669  .schema.x..Confi
+00001020: 6712 220a 0d64 6174 615f 746f 6b65 6e5f  g."..data_token_
+00001030: 6964 1801 2001 2809 520b 6461 7461 546f  id.. .(.R.dataTo
+00001040: 6b65 6e49 6412 4a0a 0d73 6c69 6365 5f72  kenId.J..slice_r
+00001050: 6571 7565 7374 1802 2001 280b 3225 2e6b  equest.. .(.2%.k
+00001060: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
+00001070: 3161 6c70 6861 2e53 6c69 6365 5265 7175  1alpha.SliceRequ
+00001080: 6573 7452 0c73 6c69 6365 5265 7175 6573  estR.sliceReques
+00001090: 741a be02 0a07 4d65 7472 6963 7312 400a  t.....Metrics.@.
+000010a0: 0e74 696d 655f 7072 6570 6172 696e 6718  .time_preparing.
+000010b0: 0120 0128 0b32 192e 676f 6f67 6c65 2e70  . .(.2..google.p
+000010c0: 726f 746f 6275 662e 4475 7261 7469 6f6e  rotobuf.Duration
+000010d0: 520d 7469 6d65 5072 6570 6172 696e 6712  R.timePreparing.
+000010e0: 400a 0e74 696d 655f 636f 6d70 7574 696e  @..time_computin
+000010f0: 6718 0220 0128 0b32 192e 676f 6f67 6c65  g.. .(.2..google
+00001100: 2e70 726f 746f 6275 662e 4475 7261 7469  .protobuf.Durati
+00001110: 6f6e 520d 7469 6d65 436f 6d70 7574 696e  onR.timeComputin
+00001120: 6712 210a 0c6f 7574 7075 745f 6669 6c65  g.!..output_file
+00001130: 7318 0320 0128 0352 0b6f 7574 7075 7446  s.. .(.R.outputF
+00001140: 696c 6573 1228 0a10 746f 7461 6c5f 696e  iles.(..total_in
+00001150: 7075 745f 726f 7773 1804 2001 2803 520e  put_rows.. .(.R.
+00001160: 746f 7461 6c49 6e70 7574 526f 7773 1230  totalInputRows.0
+00001170: 0a14 7072 6f63 6573 7365 645f 696e 7075  ..processed_inpu
+00001180: 745f 726f 7773 1805 2001 2803 5212 7072  t_rows.. .(.R.pr
+00001190: 6f63 6573 7365 6449 6e70 7574 526f 7773  ocessedInputRows
+000011a0: 1230 0a14 7072 6f64 7563 6564 5f6f 7574  .0..produced_out
+000011b0: 7075 745f 726f 7773 1806 2001 2803 5212  put_rows.. .(.R.
+000011c0: 7072 6f64 7563 6564 4f75 7470 7574 526f  producedOutputRo
+000011d0: 7773 2282 010a 0553 7461 7465 1215 0a11  ws"....State....
+000011e0: 5354 4154 455f 554e 5350 4543 4946 4945  STATE_UNSPECIFIE
+000011f0: 4410 0012 120a 0e53 5441 5445 5f41 4e41  D......STATE_ANA
+00001200: 4c59 5349 5310 0112 130a 0f53 5441 5445  LYSIS......STATE
+00001210: 5f50 5245 5041 5249 4e47 1002 1213 0a0f  _PREPARING......
+00001220: 5354 4154 455f 434f 4d50 5554 494e 4710  STATE_COMPUTING.
+00001230: 0312 110a 0d53 5441 5445 5f53 5543 4345  .....STATE_SUCCE
+00001240: 5353 1004 1211 0a0d 5354 4154 455f 4641  SS......STATE_FA
+00001250: 494c 5552 4510 054a 0408 6510 664a 0408  ILURE..J..e.fJ..
+00001260: 6610 674a 0408 6710 6822 350a 0f47 6574  f.gJ..g.h"5..Get
+00001270: 5175 6572 7952 6571 7565 7374 1222 0a08  QueryRequest."..
+00001280: 7175 6572 795f 6964 1801 2001 2809 4207  query_id.. .(.B.
+00001290: fa42 0472 0210 0152 0771 7565 7279 4964  .B.r...R.queryId
+000012a0: 224d 0a10 4765 7451 7565 7279 5265 7370  "M..GetQueryResp
+000012b0: 6f6e 7365 1239 0a05 7175 6572 7918 0120  onse.9..query.. 
+000012c0: 0128 0b32 1e2e 6b61 736b 6164 612e 6b61  .(.2..kaskada.ka
+000012d0: 736b 6164 612e 7631 616c 7068 612e 5175  skada.v1alpha.Qu
+000012e0: 6572 7942 03e0 4103 5205 7175 6572 7922  eryB..A.R.query"
+000012f0: 740a 124c 6973 7451 7565 7269 6573 5265  t..ListQueriesRe
+00001300: 7175 6573 7412 160a 0673 6561 7263 6818  quest....search.
+00001310: 0120 0128 0952 0673 6561 7263 6812 270a  . .(.R.search.'.
+00001320: 0970 6167 655f 7369 7a65 1802 2001 2805  .page_size.. .(.
+00001330: 420a fa42 071a 0518 e807 2800 5208 7061  B..B......(.R.pa
+00001340: 6765 5369 7a65 121d 0a0a 7061 6765 5f74  geSize....page_t
+00001350: 6f6b 656e 1803 2001 2809 5209 7061 6765  oken.. .(.R.page
+00001360: 546f 6b65 6e22 c901 0a13 4c69 7374 5175  Token"....ListQu
+00001370: 6572 6965 7352 6573 706f 6e73 6512 380a  eriesResponse.8.
+00001380: 0771 7565 7269 6573 1801 2003 280b 321e  .queries.. .(.2.
+00001390: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+000013a0: 2e76 3161 6c70 6861 2e51 7565 7279 5207  .v1alpha.QueryR.
+000013b0: 7175 6572 6965 7312 260a 0f6e 6578 745f  queries.&..next_
+000013c0: 7061 6765 5f74 6f6b 656e 1802 2001 2809  page_token.. .(.
+000013d0: 520d 6e65 7874 5061 6765 546f 6b65 6e12  R.nextPageToken.
+000013e0: 500a 0f72 6571 7565 7374 5f64 6574 6169  P..request_detai
+000013f0: 6c73 1803 2001 280b 3227 2e6b 6173 6b61  ls.. .(.2'.kaska
+00001400: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
+00001410: 6861 2e52 6571 7565 7374 4465 7461 696c  ha.RequestDetail
+00001420: 7352 0e72 6571 7565 7374 4465 7461 696c  sR.requestDetail
+00001430: 7332 aa03 0a0c 5175 6572 7953 6572 7669  s2....QueryServi
+00001440: 6365 128b 010a 0b43 7265 6174 6551 7565  ce.....CreateQue
+00001450: 7279 122b 2e6b 6173 6b61 6461 2e6b 6173  ry.+.kaskada.kas
+00001460: 6b61 6461 2e76 3161 6c70 6861 2e43 7265  kada.v1alpha.Cre
+00001470: 6174 6551 7565 7279 5265 7175 6573 741a  ateQueryRequest.
+00001480: 2c2e 6b61 736b 6164 612e 6b61 736b 6164  ,.kaskada.kaskad
+00001490: 612e 7631 616c 7068 612e 4372 6561 7465  a.v1alpha.Create
+000014a0: 5175 6572 7952 6573 706f 6e73 6522 1f82  QueryResponse"..
+000014b0: d3e4 9302 193a 0571 7565 7279 2210 2f76  .....:.query"./v
+000014c0: 3161 6c70 6861 2f71 7565 7269 6573 3001  1alpha/queries0.
+000014d0: 1286 010a 0847 6574 5175 6572 7912 282e  .....GetQuery.(.
+000014e0: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+000014f0: 7631 616c 7068 612e 4765 7451 7565 7279  v1alpha.GetQuery
+00001500: 5265 7175 6573 741a 292e 6b61 736b 6164  Request.).kaskad
+00001510: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00001520: 612e 4765 7451 7565 7279 5265 7370 6f6e  a.GetQueryRespon
+00001530: 7365 2225 82d3 e493 021f 121d 2f76 3161  se"%......../v1a
+00001540: 6c70 6861 2f71 7565 7269 6573 2f7b 7175  lpha/queries/{qu
+00001550: 6572 795f 6964 3d2a 7d12 8201 0a0b 4c69  ery_id=*}.....Li
+00001560: 7374 5175 6572 6965 7312 2b2e 6b61 736b  stQueries.+.kask
+00001570: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
+00001580: 7068 612e 4c69 7374 5175 6572 6965 7352  pha.ListQueriesR
+00001590: 6571 7565 7374 1a2c 2e6b 6173 6b61 6461  equest.,.kaskada
+000015a0: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+000015b0: 2e4c 6973 7451 7565 7269 6573 5265 7370  .ListQueriesResp
+000015c0: 6f6e 7365 2218 82d3 e493 0212 1210 2f76  onse"........./v
+000015d0: 3161 6c70 6861 2f71 7565 7269 6573 4281  1alpha/queriesB.
+000015e0: 020a 1b63 6f6d 2e6b 6173 6b61 6461 2e6b  ...com.kaskada.k
+000015f0: 6173 6b61 6461 2e76 3161 6c70 6861 4211  askada.v1alphaB.
+00001600: 5175 6572 7953 6572 7669 6365 5072 6f74  QueryServiceProt
+00001610: 6f50 015a 5167 6974 6875 622e 636f 6d2f  oP.ZQgithub.com/
+00001620: 6b61 736b 6164 612d 6169 2f6b 6173 6b61  kaskada-ai/kaska
+00001630: 6461 2f67 656e 2f70 726f 746f 2f67 6f2f  da/gen/proto/go/
+00001640: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
+00001650: 7631 616c 7068 613b 6b61 736b 6164 6176  v1alpha;kaskadav
+00001660: 3161 6c70 6861 a202 034b 4b58 aa02 174b  1alpha...KKX...K
+00001670: 6173 6b61 6461 2e4b 6173 6b61 6461 2e56  askada.Kaskada.V
+00001680: 3161 6c70 6861 ca02 174b 6173 6b61 6461  1alpha...Kaskada
+00001690: 5c4b 6173 6b61 6461 5c56 3161 6c70 6861  \Kaskada\V1alpha
+000016a0: e202 234b 6173 6b61 6461 5c4b 6173 6b61  ..#Kaskada\Kaska
+000016b0: 6461 5c56 3161 6c70 6861 5c47 5042 4d65  da\V1alpha\GPBMe
+000016c0: 7461 6461 7461 ea02 194b 6173 6b61 6461  tadata...Kaskada
+000016d0: 3a3a 4b61 736b 6164 613a 3a56 3161 6c70  ::Kaskada::V1alp
+000016e0: 6861 6206 7072 6f74 6f33 da05 5175 6572  hab.proto3..Quer
+000016f0: 79da 064c 696d 6974 73da 1152 6564 6973  y..Limits..Redis
+00001700: 4275 6c6b 5265 7370 6f6e 7365 da0c 5175  BulkResponse..Qu
+00001710: 6572 794f 7074 696f 6e73 da12 4372 6561  eryOptions..Crea
+00001720: 7465 5175 6572 7952 6571 7565 7374 da13  teQueryRequest..
+00001730: 4372 6561 7465 5175 6572 7952 6573 706f  CreateQueryRespo
+00001740: 6e73 65da 0841 6e61 6c79 7369 73da 0643  nse..Analysis..C
+00001750: 6f6e 6669 67da 074d 6574 7269 6373 da0f  onfig..Metrics..
+00001760: 4765 7451 7565 7279 5265 7175 6573 74da  GetQueryRequest.
+00001770: 1047 6574 5175 6572 7952 6573 706f 6e73  .GetQueryRespons
+00001780: 65da 124c 6973 7451 7565 7269 6573 5265  e..ListQueriesRe
+00001790: 7175 6573 74da 134c 6973 7451 7565 7269  quest..ListQueri
+000017a0: 6573 5265 7370 6f6e 7365 5a0e 5265 7375  esResponseZ.Resu
+000017b0: 6c74 4265 6861 7669 6f72 da05 5374 6174  ltBehavior..Stat
+000017c0: 657a 296b 6173 6b61 6461 2e6b 6173 6b61  ez)kaskada.kaska
+000017d0: 6461 2e76 3161 6c70 6861 2e71 7565 7279  da.v1alpha.query
+000017e0: 5f73 6572 7669 6365 5f70 6232 2902 da0a  _service_pb2)...
+000017f0: 4445 5343 5249 5054 4f52 da0a 5f5f 6d6f  DESCRIPTOR..__mo
+00001800: 6475 6c65 5f5f 2904 7213 0000 0072 1400  dule__).r....r..
+00001810: 0000 7220 0000 0072 2100 0000 2905 7218  ..r ...r!...).r.
+00001820: 0000 0072 1900 0000 721a 0000 0072 2000  ...r....r....r .
+00001830: 0000 7221 0000 00da 0c51 7565 7279 5365  ..r!.....QuerySe
+00001840: 7276 6963 6546 4e73 0101 0000 0a1b 636f  rviceFNs......co
+00001850: 6d2e 6b61 736b 6164 612e 6b61 736b 6164  m.kaskada.kaskad
+00001860: 612e 7631 616c 7068 6142 1151 7565 7279  a.v1alphaB.Query
+00001870: 5365 7276 6963 6550 726f 746f 5001 5a51  ServiceProtoP.ZQ
+00001880: 6769 7468 7562 2e63 6f6d 2f6b 6173 6b61  github.com/kaska
+00001890: 6461 2d61 692f 6b61 736b 6164 612f 6765  da-ai/kaskada/ge
+000018a0: 6e2f 7072 6f74 6f2f 676f 2f6b 6173 6b61  n/proto/go/kaska
+000018b0: 6461 2f6b 6173 6b61 6461 2f76 3161 6c70  da/kaskada/v1alp
+000018c0: 6861 3b6b 6173 6b61 6461 7631 616c 7068  ha;kaskadav1alph
+000018d0: 61a2 0203 4b4b 58aa 0217 4b61 736b 6164  a...KKX...Kaskad
+000018e0: 612e 4b61 736b 6164 612e 5631 616c 7068  a.Kaskada.V1alph
+000018f0: 61ca 0217 4b61 736b 6164 615c 4b61 736b  a...Kaskada\Kask
+00001900: 6164 615c 5631 616c 7068 61e2 0223 4b61  ada\V1alpha..#Ka
+00001910: 736b 6164 615c 4b61 736b 6164 615c 5631  skada\Kaskada\V1
+00001920: 616c 7068 615c 4750 424d 6574 6164 6174  alpha\GPBMetadat
+00001930: 61ea 0219 4b61 736b 6164 613a 3a4b 6173  a...Kaskada::Kas
+00001940: 6b61 6461 3a3a 5631 616c 7068 61da 0871  kada::V1alpha..q
+00001950: 7565 7279 5f69 6473 0300 0000 e041 03da  uery_ids.....A..
+00001960: 0a65 7870 7265 7373 696f 6e73 0700 0000  .expressions....
+00001970: fa42 0472 0210 01da 0576 6965 7773 da0b  .B.r.....views..
+00001980: 6372 6561 7465 5f74 696d 65da 0571 7565  create_time..que
+00001990: 7279 da09 7061 6765 5f73 697a 6573 0a00  ry..page_sizes..
+000019a0: 0000 fa42 071a 0518 e807 2800 da0b 4372  ...B......(...Cr
+000019b0: 6561 7465 5175 6572 7973 1f00 0000 82d3  eateQuerys......
+000019c0: e493 0219 3a05 7175 6572 7922 102f 7631  ....:.query"./v1
+000019d0: 616c 7068 612f 7175 6572 6965 73da 0847  alpha/queries..G
+000019e0: 6574 5175 6572 7973 2500 0000 82d3 e493  etQuerys%.......
+000019f0: 021f 121d 2f76 3161 6c70 6861 2f71 7565  ..../v1alpha/que
+00001a00: 7269 6573 2f7b 7175 6572 795f 6964 3d2a  ries/{query_id=*
+00001a10: 7dda 0b4c 6973 7451 7565 7269 6573 7318  }..ListQueriess.
+00001a20: 0000 0082 d3e4 9302 1212 102f 7631 616c  .........../v1al
+00001a30: 7068 612f 7175 6572 6965 7369 d601 0000  pha/queriesi....
+00001a40: 699f 0500 0069 9404 0000 69bf 0400 0069  i....i....i....i
+00001a50: c104 0000 69ea 0400 0069 ed04 0000 698d  ....i....i....i.
+00001a60: 0500 0069 a205 0000 694e 0600 0069 5106  ...i....iN...iQ.
+00001a70: 0000 69e7 0600 0069 ea06 0000 69fb 0b00  ..i....i....i...
+00001a80: 0069 4509 0000 69a9 0900 0069 ab09 0000  .iE...i....i....
+00001a90: 6923 0a00 0069 260a 0000 6964 0b00 0069  i#...i&...id...i
+00001aa0: 670b 0000 69e9 0b00 0069 fd0b 0000 6932  g...i....i....i2
+00001ab0: 0c00 0069 340c 0000 6981 0c00 0069 830c  ...i4...i....i..
+00001ac0: 0000 69f7 0c00 0069 fa0c 0000 69c3 0d00  ..i....i....i...
+00001ad0: 0069 c60d 0000 6970 0f00 0029 54da 075f  .i....ip...)T.._
+00001ae0: 5f64 6f63 5f5f da0f 676f 6f67 6c65 2e70  _doc__..google.p
+00001af0: 726f 746f 6275 6672 0200 0000 da0b 5f64  rotobufr......_d
+00001b00: 6573 6372 6970 746f 7272 0300 0000 da10  escriptorr......
+00001b10: 5f64 6573 6372 6970 746f 725f 706f 6f6c  _descriptor_pool
+00001b20: 7204 0000 00da 085f 6d65 7373 6167 6572  r......_messager
+00001b30: 0500 0000 da0b 5f72 6566 6c65 6374 696f  ......_reflectio
+00001b40: 6e72 0600 0000 da10 5f73 796d 626f 6c5f  nr......_symbol_
+00001b50: 6461 7461 6261 7365 da07 4465 6661 756c  database..Defaul
+00001b60: 74da 075f 7379 6d5f 6462 da0a 676f 6f67  t.._sym_db..goog
+00001b70: 6c65 2e61 7069 7207 0000 00da 2367 6f6f  le.apir.....#goo
+00001b80: 676c 655f 646f 745f 6170 695f 646f 745f  gle_dot_api_dot_
+00001b90: 616e 6e6f 7461 7469 6f6e 735f 5f70 6232  annotations__pb2
+00001ba0: 7208 0000 00da 2767 6f6f 676c 655f 646f  r.....'google_do
+00001bb0: 745f 6170 695f 646f 745f 6669 656c 645f  t_api_dot_field_
+00001bc0: 5f62 6568 6176 696f 725f 5f70 6232 7209  _behavior__pb2r.
+00001bd0: 0000 00da 2567 6f6f 676c 655f 646f 745f  ....%google_dot_
+00001be0: 7072 6f74 6f62 7566 5f64 6f74 5f64 7572  protobuf_dot_dur
+00001bf0: 6174 696f 6e5f 5f70 6232 720a 0000 00da  ation__pb2r.....
+00001c00: 2667 6f6f 676c 655f 646f 745f 7072 6f74  &google_dot_prot
+00001c10: 6f62 7566 5f64 6f74 5f74 696d 6573 7461  obuf_dot_timesta
+00001c20: 6d70 5f5f 7062 3272 0b00 0000 da25 676f  mp__pb2r.....%go
+00001c30: 6f67 6c65 5f64 6f74 5f70 726f 746f 6275  ogle_dot_protobu
+00001c40: 665f 646f 745f 7772 6170 7065 7273 5f5f  f_dot_wrappers__
+00001c50: 7062 32da 176b 6173 6b61 6461 2e6b 6173  pb2..kaskada.kas
+00001c60: 6b61 6461 2e76 3161 6c70 6861 720c 0000  kada.v1alphar...
+00001c70: 00da 2f6b 6173 6b61 6461 5f64 6f74 5f6b  ../kaskada_dot_k
+00001c80: 6173 6b61 6461 5f64 6f74 5f76 3161 6c70  askada_dot_v1alp
+00001c90: 6861 5f64 6f74 5f63 6f6d 6d6f 6e5f 5f70  ha_dot_common__p
+00001ca0: 6232 720d 0000 00da 356b 6173 6b61 6461  b2r.....5kaskada
+00001cb0: 5f64 6f74 5f6b 6173 6b61 6461 5f64 6f74  _dot_kaskada_dot
+00001cc0: 5f76 3161 6c70 6861 5f64 6f74 5f64 6573  _v1alpha_dot_des
+00001cd0: 7469 6e61 7469 6f6e 735f 5f70 6232 720e  tinations__pb2r.
+00001ce0: 0000 00da 3a6b 6173 6b61 6461 5f64 6f74  ....:kaskada_dot
+00001cf0: 5f6b 6173 6b61 6461 5f64 6f74 5f76 3161  _kaskada_dot_v1a
+00001d00: 6c70 6861 5f64 6f74 5f66 656e 6c5f 5f64  lpha_dot_fenl__d
+00001d10: 6961 676e 6f73 7469 6373 5f5f 7062 3272  iagnostics__pb2r
+00001d20: 0f00 0000 da2f 6b61 736b 6164 615f 646f  ...../kaskada_do
+00001d30: 745f 6b61 736b 6164 615f 646f 745f 7631  t_kaskada_dot_v1
+00001d40: 616c 7068 615f 646f 745f 7363 6865 6d61  alpha_dot_schema
+00001d50: 5f5f 7062 3272 1000 0000 5a36 6b61 736b  __pb2r....Z6kask
+00001d60: 6164 615f 646f 745f 6b61 736b 6164 615f  ada_dot_kaskada_
+00001d70: 646f 745f 7631 616c 7068 615f 646f 745f  dot_v1alpha_dot_
+00001d80: 7669 6577 5f5f 7365 7276 6963 655f 5f70  view__service__p
+00001d90: 6232 da08 7661 6c69 6461 7465 7211 0000  b2..validater...
+00001da0: 00da 1a76 616c 6964 6174 655f 646f 745f  ...validate_dot_
+00001db0: 7661 6c69 6461 7465 5f5f 7062 32da 1141  validate__pb2..A
+00001dc0: 6464 5365 7269 616c 697a 6564 4669 6c65  ddSerializedFile
+00001dd0: 7220 0000 00da 156d 6573 7361 6765 5f74  r .....message_t
+00001de0: 7970 6573 5f62 795f 6e61 6d65 5a06 5f51  ypes_by_nameZ._Q
+00001df0: 5545 5259 da14 6e65 7374 6564 5f74 7970  UERY..nested_typ
+00001e00: 6573 5f62 795f 6e61 6d65 5a0d 5f51 5545  es_by_nameZ._QUE
+00001e10: 5259 5f4c 494d 4954 535a 185f 5155 4552  RY_LIMITSZ._QUER
+00001e20: 595f 5245 4449 5342 554c 4b52 4553 504f  Y_REDISBULKRESPO
+00001e30: 4e53 455a 0d5f 5155 4552 594f 5054 494f  NSEZ._QUERYOPTIO
+00001e40: 4e53 5a13 5f43 5245 4154 4551 5545 5259  NSZ._CREATEQUERY
+00001e50: 5245 5155 4553 545a 145f 4352 4541 5445  REQUESTZ._CREATE
+00001e60: 5155 4552 5952 4553 504f 4e53 455a 1d5f  QUERYRESPONSEZ._
+00001e70: 4352 4541 5445 5155 4552 5952 4553 504f  CREATEQUERYRESPO
+00001e80: 4e53 455f 414e 414c 5953 4953 5a1b 5f43  NSE_ANALYSISZ._C
+00001e90: 5245 4154 4551 5545 5259 5245 5350 4f4e  REATEQUERYRESPON
+00001ea0: 5345 5f43 4f4e 4649 475a 1c5f 4352 4541  SE_CONFIGZ._CREA
+00001eb0: 5445 5155 4552 5952 4553 504f 4e53 455f  TEQUERYRESPONSE_
+00001ec0: 4d45 5452 4943 535a 105f 4745 5451 5545  METRICSZ._GETQUE
+00001ed0: 5259 5245 5155 4553 545a 115f 4745 5451  RYREQUESTZ._GETQ
+00001ee0: 5545 5259 5245 5350 4f4e 5345 5a13 5f4c  UERYRESPONSEZ._L
+00001ef0: 4953 5451 5545 5249 4553 5245 5155 4553  ISTQUERIESREQUES
+00001f00: 545a 145f 4c49 5354 5155 4552 4945 5352  TZ._LISTQUERIESR
+00001f10: 4553 504f 4e53 45da 1265 6e75 6d5f 7479  ESPONSE..enum_ty
+00001f20: 7065 735f 6279 5f6e 616d 655a 155f 5155  pes_by_nameZ._QU
+00001f30: 4552 595f 5245 5355 4c54 4245 4841 5649  ERY_RESULTBEHAVI
+00001f40: 4f52 5a1a 5f43 5245 4154 4551 5545 5259  ORZ._CREATEQUERY
+00001f50: 5245 5350 4f4e 5345 5f53 5441 5445 da1c  RESPONSE_STATE..
+00001f60: 4765 6e65 7261 7465 6450 726f 746f 636f  GeneratedProtoco
+00001f70: 6c4d 6573 7361 6765 5479 7065 da07 4d65  lMessageType..Me
+00001f80: 7373 6167 6572 1200 0000 da0f 5265 6769  ssager......Regi
+00001f90: 7374 6572 4d65 7373 6167 6572 1300 0000  sterMessager....
+00001fa0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00001fb0: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
+00001fc0: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
+00001fd0: 0000 721e 0000 00da 1073 6572 7669 6365  ..r......service
+00001fe0: 735f 6279 5f6e 616d 655a 0d5f 5155 4552  s_by_nameZ._QUER
+00001ff0: 5953 4552 5649 4345 da12 5f55 5345 5f43  YSERVICE.._USE_C
+00002000: 5f44 4553 4352 4950 544f 5253 da08 5f6f  _DESCRIPTORS.._o
+00002010: 7074 696f 6e73 da13 5f73 6572 6961 6c69  ptions.._seriali
+00002020: 7a65 645f 6f70 7469 6f6e 73da 0e66 6965  zed_options..fie
+00002030: 6c64 735f 6279 5f6e 616d 65da 0f6d 6574  lds_by_name..met
+00002040: 686f 6473 5f62 795f 6e61 6d65 da11 5f73  hods_by_name.._s
+00002050: 6572 6961 6c69 7a65 645f 7374 6172 74da  erialized_start.
+00002060: 0f5f 7365 7269 616c 697a 6564 5f65 6e64  ._serialized_end
+00002070: a900 7251 0000 0072 5100 0000 fa35 2f73  ..rQ...rQ....5/s
+00002080: 7263 2f73 7263 2f6b 6173 6b61 6461 2f6b  rc/src/kaskada/k
+00002090: 6173 6b61 6461 2f76 3161 6c70 6861 2f71  askada/v1alpha/q
+000020a0: 7565 7279 5f73 6572 7669 6365 5f70 6232  uery_service_pb2
+000020b0: 2e70 79da 083c 6d6f 6475 6c65 3e04 0000  .py..<module>...
+000020c0: 0073 3401 0000 0401 0c01 0c01 0c01 0c01  .s4.............
+000020d0: 0c03 0803 0c01 0c01 0c01 0c01 0c01 0c01  ................
+000020e0: 0c01 0c01 0c01 0c01 0c03 0e04 0a01 0a01  ................
+000020f0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00002100: 0a01 0a01 0a01 0a01 0a01 0c02 0c01 0201  ................
+00002110: 02fe 0607 0c01 0201 02fe 0606 0201 02f0  ................
+00002120: 0813 0a01 0c01 0c02 0c01 0201 02fe 0805  ................
+00002130: 0a02 0c01 0201 02fe 0805 0a02 0c02 0c01  ................
+00002140: 0201 02fe 0607 0c01 0201 02fe 0607 0c01  ................
+00002150: 0201 02fe 0606 0201 02e9 081a 0a01 0c01  ................
+00002160: 0c01 0c02 0c01 0201 02fe 0805 0a02 0c01  ................
+00002170: 0201 02fe 0805 0a02 0c01 0201 02fe 0805  ................
+00002180: 0a02 0c01 0201 02fe 0805 0a02 0a01 0c02  ................
+00002190: 0601 0601 0c01 0c01 0c01 0c01 0c01 0c01  ................
+000021a0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+000021b0: 0c01 0c01 0c01 0c01 0c01 0c01 0601 0601  ................
+000021c0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+000021d0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+000021e0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+000021f0: 0601 0601 0601 0601 0601                 ..........
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/query_service_pb2_grpc.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/query_service_pb2_grpc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 6542 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 8e19 0000  o.........5d....
+00000000: 610d 0d0a 0000 0000 2038 4164 8e19 0000  a....... 8Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a04 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000050: 6505 8303 5a06 4700 6406 6407 8400 6407  e...Z.G.d.d...d.
 00000060: 6505 8303 5a07 6408 6409 8400 5a08 4700  e...Z.d.d...Z.G.
 00000070: 640a 640b 8400 640b 6505 8303 5a09 6402  d.d...d.e...Z.d.
@@ -59,187 +59,194 @@
 000003a0: 5265 7175 6573 74da 1047 6574 5175 6572  Request..GetQuer
 000003b0: 7952 6573 706f 6e73 65da 0847 6574 5175  yResponse..GetQu
 000003c0: 6572 79da 124c 6973 7451 7565 7269 6573  ery..ListQueries
 000003d0: 5265 7175 6573 74da 134c 6973 7451 7565  Request..ListQue
 000003e0: 7269 6573 5265 7370 6f6e 7365 da0b 4c69  riesResponse..Li
 000003f0: 7374 5175 6572 6965 7329 02da 0473 656c  stQueries)...sel
 00000400: 66da 0763 6861 6e6e 656c a900 721a 0000  f..channel..r...
-00000410: 00fa 7c2f 686f 6d65 2f74 6865 7261 706f  ..|/home/therapo
-00000420: 6e2f 5265 706f 732f 4769 7448 7562 2f4b  n/Repos/GitHub/K
-00000430: 6173 6b61 6461 4149 2f6b 6173 6b61 6461  askadaAI/kaskada
-00000440: 2f72 656c 6561 7369 6e67 2f63 6c69 656e  /releasing/clien
-00000450: 7473 2f70 7974 686f 6e2f 7372 632f 6b61  ts/python/src/ka
-00000460: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
-00000470: 616c 7068 612f 7175 6572 795f 7365 7276  alpha/query_serv
-00000480: 6963 655f 7062 325f 6772 7063 2e70 79da  ice_pb2_grpc.py.
-00000490: 085f 5f69 6e69 745f 5f0b 0000 0073 1e00  .__init__....s..
-000004a0: 0000 0406 0201 0601 0601 08fd 0405 0201  ................
-000004b0: 0601 0601 08fd 0405 0201 0601 0601 0cfd  ................
-000004c0: 7a19 5175 6572 7953 6572 7669 6365 5374  z.QueryServiceSt
-000004d0: 7562 2e5f 5f69 6e69 745f 5f4e 2905 da08  ub.__init__N)...
-000004e0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000004f0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000500: 5f5f da07 5f5f 646f 635f 5f72 1c00 0000  __..__doc__r....
-00000510: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
-00000520: 1b00 0000 7203 0000 0008 0000 0073 0600  ....r........s..
-00000530: 0000 0800 0401 0c02 7203 0000 0063 0000  ........r....c..
-00000540: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00000550: 0000 4000 0000 7328 0000 0065 005a 0164  ..@...s(...e.Z.d
-00000560: 005a 0264 015a 0364 0264 0384 005a 0464  .Z.d.Z.d.d...Z.d
-00000570: 0464 0584 005a 0564 0664 0784 005a 0664  .d...Z.d.d...Z.d
-00000580: 0853 0029 09da 1451 7565 7279 5365 7276  .S.)...QueryServ
-00000590: 6963 6553 6572 7669 6365 7272 0400 0000  iceServicerr....
-000005a0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-000005b0: 0003 0000 0043 0000 00f3 2000 0000 7c02  .....C.... ...|.
-000005c0: a000 7401 6a02 6a03 a101 0100 7c02 a004  ..t.j.j.....|...
-000005d0: 6401 a101 0100 7405 6401 8301 8201 2902  d.....t.d.....).
-000005e0: 7a19 4372 6561 7465 7320 6120 5175 6572  z.Creates a Quer
-000005f0: 792e 0a20 2020 2020 2020 20fa 174d 6574  y..        ..Met
-00000600: 686f 6420 6e6f 7420 696d 706c 656d 656e  hod not implemen
-00000610: 7465 6421 a906 da08 7365 745f 636f 6465  ted!....set_code
-00000620: da04 6772 7063 da0a 5374 6174 7573 436f  ..grpc..StatusCo
-00000630: 6465 da0d 554e 494d 504c 454d 454e 5445  de..UNIMPLEMENTE
-00000640: 44da 0b73 6574 5f64 6574 6169 6c73 da13  D..set_details..
-00000650: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-00000660: 726f 72a9 0372 1800 0000 da07 7265 7175  ror..r......requ
-00000670: 6573 74da 0763 6f6e 7465 7874 721a 0000  est..contextr...
-00000680: 0072 1a00 0000 721b 0000 0072 1000 0000  .r....r....r....
-00000690: 2500 0000 f306 0000 000e 030a 0108 017a  %..............z
-000006a0: 2051 7565 7279 5365 7276 6963 6553 6572   QueryServiceSer
-000006b0: 7669 6365 722e 4372 6561 7465 5175 6572  vicer.CreateQuer
-000006c0: 7963 0300 0000 0000 0000 0000 0000 0300  yc..............
-000006d0: 0000 0300 0000 4300 0000 7222 0000 0029  ......C...r"...)
-000006e0: 027a 1647 6574 7320 6120 5175 6572 792e  .z.Gets a Query.
-000006f0: 0a20 2020 2020 2020 2072 2300 0000 7224  .        r#...r$
-00000700: 0000 0072 2b00 0000 721a 0000 0072 1a00  ...r+...r....r..
-00000710: 0000 721b 0000 0072 1400 0000 2c00 0000  ..r....r....,...
-00000720: 722e 0000 007a 1d51 7565 7279 5365 7276  r....z.QueryServ
-00000730: 6963 6553 6572 7669 6365 722e 4765 7451  iceServicer.GetQ
-00000740: 7565 7279 6303 0000 0000 0000 0000 0000  ueryc...........
-00000750: 0003 0000 0003 0000 0043 0000 0072 2200  .........C...r".
-00000760: 0000 2902 7ac9 4c69 7374 7320 7175 6572  ..).z.Lists quer
-00000770: 6965 732e 0a0a 2020 2020 2020 2020 5468  ies...        Th
-00000780: 6520 7265 7370 6f6e 7365 2069 6e63 6c75  e response inclu
-00000790: 6465 7320 616c 6c20 5175 6572 6965 7320  des all Queries 
-000007a0: 6465 6669 6e65 6420 666f 7220 7468 6520  defined for the 
-000007b0: 4b61 736b 6164 6120 6163 636f 756e 742e  Kaskada account.
-000007c0: 0a20 2020 2020 2020 2049 6620 6120 7365  .        If a se
-000007d0: 6172 6368 2073 7472 696e 6720 6973 2070  arch string is p
-000007e0: 726f 7669 6465 642c 206f 6e6c 7920 5175  rovided, only Qu
-000007f0: 6572 6965 7320 6d61 7463 6869 6e67 2074  eries matching t
-00000800: 6865 2073 6561 7263 6820 7374 7269 6e67  he search string
-00000810: 0a20 2020 2020 2020 2061 7265 2072 6574  .        are ret
-00000820: 7572 6e65 642e 0a20 2020 2020 2020 2072  urned..        r
-00000830: 2300 0000 7224 0000 0072 2b00 0000 721a  #...r$...r+...r.
-00000840: 0000 0072 1a00 0000 721b 0000 0072 1700  ...r....r....r..
-00000850: 0000 3300 0000 7306 0000 000e 070a 0108  ..3...s.........
-00000860: 017a 2051 7565 7279 5365 7276 6963 6553  .z QueryServiceS
-00000870: 6572 7669 6365 722e 4c69 7374 5175 6572  ervicer.ListQuer
-00000880: 6965 734e 2907 721d 0000 0072 1e00 0000  iesN).r....r....
-00000890: 721f 0000 0072 2000 0000 7210 0000 0072  r....r ...r....r
-000008a0: 1400 0000 7217 0000 0072 1a00 0000 721a  ....r....r....r.
-000008b0: 0000 0072 1a00 0000 721b 0000 0072 2100  ...r....r....r!.
-000008c0: 0000 2200 0000 730a 0000 0008 0004 0108  .."...s.........
-000008d0: 0208 070c 0772 2100 0000 6302 0000 0000  .....r!...c.....
-000008e0: 0000 0000 0000 0004 0000 0007 0000 0043  ...............C
-000008f0: 0000 0073 6a00 0000 7400 6a01 7c00 6a02  ...sj...t.j.|.j.
-00000900: 7403 6a04 6a05 7403 6a06 6a07 6401 8d03  t.j.j.t.j.j.d...
-00000910: 7400 6a08 7c00 6a09 7403 6a0a 6a05 7403  t.j.|.j.t.j.j.t.
-00000920: 6a0b 6a07 6401 8d03 7400 6a08 7c00 6a0c  j.j.d...t.j.|.j.
-00000930: 7403 6a0d 6a05 7403 6a0e 6a07 6401 8d03  t.j.j.t.j.j.d...
-00000940: 6402 9c03 7d02 7400 a00f 6403 7c02 a102  d...}.t...d.|...
-00000950: 7d03 7c01 a010 7c03 6601 a101 0100 6400  }.|...|.f.....d.
-00000960: 5300 2904 4e29 02da 1472 6571 7565 7374  S.).N)...request
-00000970: 5f64 6573 6572 6961 6c69 7a65 72da 1372  _deserializer..r
-00000980: 6573 706f 6e73 655f 7365 7269 616c 697a  esponse_serializ
-00000990: 6572 2903 7210 0000 0072 1400 0000 7217  er).r....r....r.
-000009a0: 0000 007a 246b 6173 6b61 6461 2e6b 6173  ...z$kaskada.kas
-000009b0: 6b61 6461 2e76 3161 6c70 6861 2e51 7565  kada.v1alpha.Que
-000009c0: 7279 5365 7276 6963 6529 1172 2600 0000  ryService).r&...
-000009d0: da1f 756e 6172 795f 7374 7265 616d 5f72  ..unary_stream_r
-000009e0: 7063 5f6d 6574 686f 645f 6861 6e64 6c65  pc_method_handle
-000009f0: 7272 1000 0000 720b 0000 0072 0c00 0000  rr....r....r....
-00000a00: 720f 0000 0072 0e00 0000 720d 0000 00da  r....r....r.....
-00000a10: 1e75 6e61 7279 5f75 6e61 7279 5f72 7063  .unary_unary_rpc
-00000a20: 5f6d 6574 686f 645f 6861 6e64 6c65 7272  _method_handlerr
-00000a30: 1400 0000 7212 0000 0072 1300 0000 7217  ....r....r....r.
-00000a40: 0000 0072 1500 0000 7216 0000 00da 1f6d  ...r....r......m
-00000a50: 6574 686f 645f 6861 6e64 6c65 7273 5f67  ethod_handlers_g
-00000a60: 656e 6572 6963 5f68 616e 646c 6572 da18  eneric_handler..
-00000a70: 6164 645f 6765 6e65 7269 635f 7270 635f  add_generic_rpc_
-00000a80: 6861 6e64 6c65 7273 2904 da08 7365 7276  handlers)...serv
-00000a90: 6963 6572 da06 7365 7276 6572 da13 7270  icer..server..rp
-00000aa0: 635f 6d65 7468 6f64 5f68 616e 646c 6572  c_method_handler
-00000ab0: 73da 0f67 656e 6572 6963 5f68 616e 646c  s..generic_handl
-00000ac0: 6572 721a 0000 0072 1a00 0000 721b 0000  err....r....r...
-00000ad0: 00da 2261 6464 5f51 7565 7279 5365 7276  .."add_QueryServ
-00000ae0: 6963 6553 6572 7669 6365 725f 746f 5f73  iceServicer_to_s
-00000af0: 6572 7665 723f 0000 0073 2800 0000 0402  erver?...s(.....
-00000b00: 0401 0601 0601 04fd 0405 0401 0601 0601  ................
-00000b10: 04fd 0405 0401 0601 0601 04fd 06f5 0411  ................
-00000b20: 0401 04ff 1002 7239 0000 0063 0000 0000  ......r9...c....
-00000b30: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000b40: 4000 0000 736a 0000 0065 005a 0164 005a  @...sj...e.Z.d.Z
-00000b50: 0264 015a 0365 0409 0209 0309 0309 0409  .d.Z.e..........
-00000b60: 0309 0309 0309 0364 0b64 0564 0684 0183  .......d.d.d....
-00000b70: 015a 0565 0409 0209 0309 0309 0409 0309  .Z.e............
-00000b80: 0309 0309 0364 0b64 0764 0884 0183 015a  .....d.d.d.....Z
-00000b90: 0665 0409 0209 0309 0309 0409 0309 0309  .e..............
-00000ba0: 0309 0364 0b64 0964 0a84 0183 015a 0764  ...d.d.d.....Z.d
-00000bb0: 0353 0029 0cda 0c51 7565 7279 5365 7276  .S.)...QueryServ
-00000bc0: 6963 6572 0400 0000 721a 0000 004e 4663  icer....r....NFc
-00000bd0: 0a00 0000 0000 0000 0000 0000 0a00 0000  ................
-00000be0: 0f00 0000 4300 0000 f32c 0000 0074 006a  ....C....,...t.j
-00000bf0: 01a0 027c 007c 0164 0174 036a 046a 0574  ...|.|.d.t.j.j.t
-00000c00: 036a 066a 077c 027c 037c 057c 047c 067c  .j.j.|.|.|.|.|.|
-00000c10: 077c 087c 09a1 0d53 0029 024e 7205 0000  .|.|...S.).Nr...
-00000c20: 0029 0872 2600 0000 da0c 6578 7065 7269  .).r&.....experi
-00000c30: 6d65 6e74 616c 720a 0000 0072 0b00 0000  mentalr....r....
-00000c40: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00000c50: 0f00 0000 a90a 722c 0000 00da 0674 6172  ......r,.....tar
-00000c60: 6765 74da 076f 7074 696f 6e73 da13 6368  get..options..ch
-00000c70: 616e 6e65 6c5f 6372 6564 656e 7469 616c  annel_credential
-00000c80: 73da 1063 616c 6c5f 6372 6564 656e 7469  s..call_credenti
-00000c90: 616c 73da 0869 6e73 6563 7572 65da 0b63  als..insecure..c
-00000ca0: 6f6d 7072 6573 7369 6f6e da0e 7761 6974  ompression..wait
-00000cb0: 5f66 6f72 5f72 6561 6479 da07 7469 6d65  _for_ready..time
-00000cc0: 6f75 74da 086d 6574 6164 6174 6172 1a00  out..metadatar..
-00000cd0: 0000 721a 0000 0072 1b00 0000 7210 0000  ..r....r....r...
-00000ce0: 005a 0000 00f3 0c00 0000 0c0b 0601 0601  .Z..............
-00000cf0: 0401 0c01 04fc 7a18 5175 6572 7953 6572  ......z.QuerySer
-00000d00: 7669 6365 2e43 7265 6174 6551 7565 7279  vice.CreateQuery
-00000d10: 630a 0000 0000 0000 0000 0000 000a 0000  c...............
-00000d20: 000f 0000 0043 0000 0072 3b00 0000 2902  .....C...r;...).
-00000d30: 4e72 0800 0000 2908 7226 0000 0072 3c00  Nr....).r&...r<.
-00000d40: 0000 7211 0000 0072 0b00 0000 7212 0000  ..r....r....r...
-00000d50: 0072 0d00 0000 7213 0000 0072 0f00 0000  .r....r....r....
-00000d60: 723d 0000 0072 1a00 0000 721a 0000 0072  r=...r....r....r
-00000d70: 1b00 0000 7214 0000 006b 0000 0072 4700  ....r....k...rG.
-00000d80: 0000 7a15 5175 6572 7953 6572 7669 6365  ..z.QueryService
-00000d90: 2e47 6574 5175 6572 7963 0a00 0000 0000  .GetQueryc......
-00000da0: 0000 0000 0000 0a00 0000 0f00 0000 4300  ..............C.
-00000db0: 0000 723b 0000 0029 024e 7209 0000 0029  ..r;...).Nr....)
-00000dc0: 0872 2600 0000 723c 0000 0072 1100 0000  .r&...r<...r....
-00000dd0: 720b 0000 0072 1500 0000 720d 0000 0072  r....r....r....r
-00000de0: 1600 0000 720f 0000 0072 3d00 0000 721a  ....r....r=...r.
-00000df0: 0000 0072 1a00 0000 721b 0000 0072 1700  ...r....r....r..
-00000e00: 0000 7c00 0000 7247 0000 007a 1851 7565  ..|...rG...z.Que
-00000e10: 7279 5365 7276 6963 652e 4c69 7374 5175  ryService.ListQu
-00000e20: 6572 6965 7329 0872 1a00 0000 4e4e 464e  eries).r....NNFN
-00000e30: 4e4e 4e29 0872 1d00 0000 721e 0000 0072  NNN).r....r....r
-00000e40: 1f00 0000 7220 0000 00da 0c73 7461 7469  ....r .....stati
-00000e50: 636d 6574 686f 6472 1000 0000 7214 0000  cmethodr....r...
-00000e60: 0072 1700 0000 721a 0000 0072 1a00 0000  .r....r....r....
-00000e70: 721a 0000 0072 1b00 0000 723a 0000 0057  r....r....r:...W
-00000e80: 0000 0073 4000 0000 0800 0401 0202 0203  ...s@...........
-00000e90: 0201 0201 0201 0201 0201 0201 0201 0cf7  ................
-00000ea0: 0210 0203 0201 0201 0201 0201 0201 0201  ................
-00000eb0: 0201 0cf7 0210 0203 0201 0201 0201 0201  ................
-00000ec0: 0201 0201 0201 10f7 723a 0000 0029 0a72  ........r:...).r
-00000ed0: 2000 0000 7226 0000 00da 176b 6173 6b61   ...r&.....kaska
-00000ee0: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-00000ef0: 6861 7202 0000 0072 0b00 0000 da06 6f62  har....r......ob
-00000f00: 6a65 6374 7203 0000 0072 2100 0000 7239  jectr....r!...r9
-00000f10: 0000 0072 3a00 0000 721a 0000 0072 1a00  ...r:...r....r..
-00000f20: 0000 721a 0000 0072 1b00 0000 da08 3c6d  ..r....r......<m
-00000f30: 6f64 756c 653e 0100 0000 730e 0000 0004  odule>....s.....
-00000f40: 0108 010c 0210 0310 1a08 1d14 18         .............
+00000410: 00fa 3a2f 7372 632f 7372 632f 6b61 736b  ..:/src/src/kask
+00000420: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
+00000430: 7068 612f 7175 6572 795f 7365 7276 6963  pha/query_servic
+00000440: 655f 7062 325f 6772 7063 2e70 79da 085f  e_pb2_grpc.py.._
+00000450: 5f69 6e69 745f 5f0b 0000 0073 1e00 0000  _init__....s....
+00000460: 0006 0401 0201 0601 06fd 0805 0401 0201  ................
+00000470: 0601 06fd 0805 0401 0201 0601 06fd 7a19  ..............z.
+00000480: 5175 6572 7953 6572 7669 6365 5374 7562  QueryServiceStub
+00000490: 2e5f 5f69 6e69 745f 5f4e 2905 da08 5f5f  .__init__N)...__
+000004a0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+000004b0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+000004c0: da07 5f5f 646f 635f 5f72 1c00 0000 721a  ..__doc__r....r.
+000004d0: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
+000004e0: 0000 7203 0000 0008 0000 0073 0400 0000  ..r........s....
+000004f0: 0801 0402 7203 0000 0063 0000 0000 0000  ....r....c......
+00000500: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00000510: 0000 7328 0000 0065 005a 0164 005a 0264  ..s(...e.Z.d.Z.d
+00000520: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
+00000530: 005a 0564 0664 0784 005a 0664 0853 0029  .Z.d.d...Z.d.S.)
+00000540: 09da 1451 7565 7279 5365 7276 6963 6553  ...QueryServiceS
+00000550: 6572 7669 6365 7272 0400 0000 6303 0000  ervicerr....c...
+00000560: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00000570: 0043 0000 0073 2400 0000 7c02 a000 7401  .C...s$...|...t.
+00000580: 6a02 6a03 a101 0100 7c02 a004 6401 a101  j.j.....|...d...
+00000590: 0100 7405 6401 8301 8201 6402 5300 2903  ..t.d.....d.S.).
+000005a0: 7a19 4372 6561 7465 7320 6120 5175 6572  z.Creates a Quer
+000005b0: 792e 0a20 2020 2020 2020 20fa 174d 6574  y..        ..Met
+000005c0: 686f 6420 6e6f 7420 696d 706c 656d 656e  hod not implemen
+000005d0: 7465 6421 4ea9 06da 0873 6574 5f63 6f64  ted!N....set_cod
+000005e0: 65da 0467 7270 63da 0a53 7461 7475 7343  e..grpc..StatusC
+000005f0: 6f64 65da 0d55 4e49 4d50 4c45 4d45 4e54  ode..UNIMPLEMENT
+00000600: 4544 da0b 7365 745f 6465 7461 696c 73da  ED..set_details.
+00000610: 134e 6f74 496d 706c 656d 656e 7465 6445  .NotImplementedE
+00000620: 7272 6f72 a903 7218 0000 00da 0772 6571  rror..r......req
+00000630: 7565 7374 da07 636f 6e74 6578 7472 1a00  uest..contextr..
+00000640: 0000 721a 0000 0072 1b00 0000 7210 0000  ..r....r....r...
+00000650: 0025 0000 0073 0600 0000 0003 0e01 0a01  .%...s..........
+00000660: 7a20 5175 6572 7953 6572 7669 6365 5365  z QueryServiceSe
+00000670: 7276 6963 6572 2e43 7265 6174 6551 7565  rvicer.CreateQue
+00000680: 7279 6303 0000 0000 0000 0000 0000 0003  ryc.............
+00000690: 0000 0003 0000 0043 0000 0073 2400 0000  .......C...s$...
+000006a0: 7c02 a000 7401 6a02 6a03 a101 0100 7c02  |...t.j.j.....|.
+000006b0: a004 6401 a101 0100 7405 6401 8301 8201  ..d.....t.d.....
+000006c0: 6402 5300 2903 7a16 4765 7473 2061 2051  d.S.).z.Gets a Q
+000006d0: 7565 7279 2e0a 2020 2020 2020 2020 7222  uery..        r"
+000006e0: 0000 004e 7223 0000 0072 2a00 0000 721a  ...Nr#...r*...r.
+000006f0: 0000 0072 1a00 0000 721b 0000 0072 1400  ...r....r....r..
+00000700: 0000 2c00 0000 7306 0000 0000 030e 010a  ..,...s.........
+00000710: 017a 1d51 7565 7279 5365 7276 6963 6553  .z.QueryServiceS
+00000720: 6572 7669 6365 722e 4765 7451 7565 7279  ervicer.GetQuery
+00000730: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00000740: 0003 0000 0043 0000 0073 2400 0000 7c02  .....C...s$...|.
+00000750: a000 7401 6a02 6a03 a101 0100 7c02 a004  ..t.j.j.....|...
+00000760: 6401 a101 0100 7405 6401 8301 8201 6402  d.....t.d.....d.
+00000770: 5300 2903 7ac9 4c69 7374 7320 7175 6572  S.).z.Lists quer
+00000780: 6965 732e 0a0a 2020 2020 2020 2020 5468  ies...        Th
+00000790: 6520 7265 7370 6f6e 7365 2069 6e63 6c75  e response inclu
+000007a0: 6465 7320 616c 6c20 5175 6572 6965 7320  des all Queries 
+000007b0: 6465 6669 6e65 6420 666f 7220 7468 6520  defined for the 
+000007c0: 4b61 736b 6164 6120 6163 636f 756e 742e  Kaskada account.
+000007d0: 0a20 2020 2020 2020 2049 6620 6120 7365  .        If a se
+000007e0: 6172 6368 2073 7472 696e 6720 6973 2070  arch string is p
+000007f0: 726f 7669 6465 642c 206f 6e6c 7920 5175  rovided, only Qu
+00000800: 6572 6965 7320 6d61 7463 6869 6e67 2074  eries matching t
+00000810: 6865 2073 6561 7263 6820 7374 7269 6e67  he search string
+00000820: 0a20 2020 2020 2020 2061 7265 2072 6574  .        are ret
+00000830: 7572 6e65 642e 0a20 2020 2020 2020 2072  urned..        r
+00000840: 2200 0000 4e72 2300 0000 722a 0000 0072  "...Nr#...r*...r
+00000850: 1a00 0000 721a 0000 0072 1b00 0000 7217  ....r....r....r.
+00000860: 0000 0033 0000 0073 0600 0000 0007 0e01  ...3...s........
+00000870: 0a01 7a20 5175 6572 7953 6572 7669 6365  ..z QueryService
+00000880: 5365 7276 6963 6572 2e4c 6973 7451 7565  Servicer.ListQue
+00000890: 7269 6573 4e29 0772 1d00 0000 721e 0000  riesN).r....r...
+000008a0: 0072 1f00 0000 7220 0000 0072 1000 0000  .r....r ...r....
+000008b0: 7214 0000 0072 1700 0000 721a 0000 0072  r....r....r....r
+000008c0: 1a00 0000 721a 0000 0072 1b00 0000 7221  ....r....r....r!
+000008d0: 0000 0022 0000 0073 0800 0000 0801 0402  ..."...s........
+000008e0: 0807 0807 7221 0000 0063 0200 0000 0000  ....r!...c......
+000008f0: 0000 0000 0000 0400 0000 0700 0000 4300  ..............C.
+00000900: 0000 736a 0000 0074 006a 017c 006a 0274  ..sj...t.j.|.j.t
+00000910: 036a 046a 0574 036a 066a 0764 018d 0374  .j.j.t.j.j.d...t
+00000920: 006a 087c 006a 0974 036a 0a6a 0574 036a  .j.|.j.t.j.j.t.j
+00000930: 0b6a 0764 018d 0374 006a 087c 006a 0c74  .j.d...t.j.|.j.t
+00000940: 036a 0d6a 0574 036a 0e6a 0764 018d 0364  .j.j.t.j.j.d...d
+00000950: 029c 037d 0274 00a0 0f64 037c 02a1 027d  ...}.t...d.|...}
+00000960: 037c 01a0 107c 0366 01a1 0101 0064 0053  .|...|.f.....d.S
+00000970: 0029 044e 2902 da14 7265 7175 6573 745f  .).N)...request_
+00000980: 6465 7365 7269 616c 697a 6572 da13 7265  deserializer..re
+00000990: 7370 6f6e 7365 5f73 6572 6961 6c69 7a65  sponse_serialize
+000009a0: 7229 0372 1000 0000 7214 0000 0072 1700  r).r....r....r..
+000009b0: 0000 7a24 6b61 736b 6164 612e 6b61 736b  ..z$kaskada.kask
+000009c0: 6164 612e 7631 616c 7068 612e 5175 6572  ada.v1alpha.Quer
+000009d0: 7953 6572 7669 6365 2911 7225 0000 00da  yService).r%....
+000009e0: 1f75 6e61 7279 5f73 7472 6561 6d5f 7270  .unary_stream_rp
+000009f0: 635f 6d65 7468 6f64 5f68 616e 646c 6572  c_method_handler
+00000a00: 7210 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00000a10: 0f00 0000 720e 0000 0072 0d00 0000 da1e  ....r....r......
+00000a20: 756e 6172 795f 756e 6172 795f 7270 635f  unary_unary_rpc_
+00000a30: 6d65 7468 6f64 5f68 616e 646c 6572 7214  method_handlerr.
+00000a40: 0000 0072 1200 0000 7213 0000 0072 1700  ...r....r....r..
+00000a50: 0000 7215 0000 0072 1600 0000 da1f 6d65  ..r....r......me
+00000a60: 7468 6f64 5f68 616e 646c 6572 735f 6765  thod_handlers_ge
+00000a70: 6e65 7269 635f 6861 6e64 6c65 72da 1861  neric_handler..a
+00000a80: 6464 5f67 656e 6572 6963 5f72 7063 5f68  dd_generic_rpc_h
+00000a90: 616e 646c 6572 7329 04da 0873 6572 7669  andlers)...servi
+00000aa0: 6365 72da 0673 6572 7665 72da 1372 7063  cer..server..rpc
+00000ab0: 5f6d 6574 686f 645f 6861 6e64 6c65 7273  _method_handlers
+00000ac0: da0f 6765 6e65 7269 635f 6861 6e64 6c65  ..generic_handle
+00000ad0: 7272 1a00 0000 721a 0000 0072 1b00 0000  rr....r....r....
+00000ae0: da22 6164 645f 5175 6572 7953 6572 7669  ."add_QueryServi
+00000af0: 6365 5365 7276 6963 6572 5f74 6f5f 7365  ceServicer_to_se
+00000b00: 7276 6572 3f00 0000 7328 0000 0000 0204  rver?...s(......
+00000b10: 0104 0106 0106 fd04 0504 0104 0106 0106  ................
+00000b20: fd04 0504 0104 0106 0106 fd04 f506 1104  ................
+00000b30: 0104 ff04 0272 3700 0000 6300 0000 0000  .....r7...c.....
+00000b40: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
+00000b50: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
+00000b60: 6401 5a03 6504 640b 6405 6406 8401 8301  d.Z.e.d.d.d.....
+00000b70: 5a05 6504 640c 6407 6408 8401 8301 5a06  Z.e.d.d.d.....Z.
+00000b80: 6504 640d 6409 640a 8401 8301 5a07 6403  e.d.d.d.....Z.d.
+00000b90: 5300 290e da0c 5175 6572 7953 6572 7669  S.)...QueryServi
+00000ba0: 6365 7204 0000 0072 1a00 0000 4e46 630a  cer....r....NFc.
+00000bb0: 0000 0000 0000 0000 0000 000a 0000 000f  ................
+00000bc0: 0000 0043 0000 0073 2c00 0000 7400 6a01  ...C...s,...t.j.
+00000bd0: a002 7c00 7c01 6401 7403 6a04 6a05 7403  ..|.|.d.t.j.j.t.
+00000be0: 6a06 6a07 7c02 7c03 7c05 7c04 7c06 7c07  j.j.|.|.|.|.|.|.
+00000bf0: 7c08 7c09 a10d 5300 2902 4e72 0500 0000  |.|...S.).Nr....
+00000c00: 2908 7225 0000 00da 0c65 7870 6572 696d  ).r%.....experim
+00000c10: 656e 7461 6c72 0a00 0000 720b 0000 0072  entalr....r....r
+00000c20: 0c00 0000 720d 0000 0072 0e00 0000 720f  ....r....r....r.
+00000c30: 0000 00a9 0a72 2b00 0000 da06 7461 7267  .....r+.....targ
+00000c40: 6574 da07 6f70 7469 6f6e 73da 1363 6861  et..options..cha
+00000c50: 6e6e 656c 5f63 7265 6465 6e74 6961 6c73  nnel_credentials
+00000c60: da10 6361 6c6c 5f63 7265 6465 6e74 6961  ..call_credentia
+00000c70: 6c73 da08 696e 7365 6375 7265 da0b 636f  ls..insecure..co
+00000c80: 6d70 7265 7373 696f 6eda 0e77 6169 745f  mpression..wait_
+00000c90: 666f 725f 7265 6164 79da 0774 696d 656f  for_ready..timeo
+00000ca0: 7574 da08 6d65 7461 6461 7461 721a 0000  ut..metadatar...
+00000cb0: 0072 1a00 0000 721b 0000 0072 1000 0000  .r....r....r....
+00000cc0: 5a00 0000 730c 0000 0000 0b0c 0106 0106  Z...s...........
+00000cd0: 0104 010c fc7a 1851 7565 7279 5365 7276  .....z.QueryServ
+00000ce0: 6963 652e 4372 6561 7465 5175 6572 7963  ice.CreateQueryc
+00000cf0: 0a00 0000 0000 0000 0000 0000 0a00 0000  ................
+00000d00: 0f00 0000 4300 0000 732c 0000 0074 006a  ....C...s,...t.j
+00000d10: 01a0 027c 007c 0164 0174 036a 046a 0574  ...|.|.d.t.j.j.t
+00000d20: 036a 066a 077c 027c 037c 057c 047c 067c  .j.j.|.|.|.|.|.|
+00000d30: 077c 087c 09a1 0d53 0029 024e 7208 0000  .|.|...S.).Nr...
+00000d40: 0029 0872 2500 0000 7239 0000 0072 1100  .).r%...r9...r..
+00000d50: 0000 720b 0000 0072 1200 0000 720d 0000  ..r....r....r...
+00000d60: 0072 1300 0000 720f 0000 0072 3a00 0000  .r....r....r:...
+00000d70: 721a 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00000d80: 1400 0000 6b00 0000 730c 0000 0000 0b0c  ....k...s.......
+00000d90: 0106 0106 0104 010c fc7a 1551 7565 7279  .........z.Query
+00000da0: 5365 7276 6963 652e 4765 7451 7565 7279  Service.GetQuery
+00000db0: 630a 0000 0000 0000 0000 0000 000a 0000  c...............
+00000dc0: 000f 0000 0043 0000 0073 2c00 0000 7400  .....C...s,...t.
+00000dd0: 6a01 a002 7c00 7c01 6401 7403 6a04 6a05  j...|.|.d.t.j.j.
+00000de0: 7403 6a06 6a07 7c02 7c03 7c05 7c04 7c06  t.j.j.|.|.|.|.|.
+00000df0: 7c07 7c08 7c09 a10d 5300 2902 4e72 0900  |.|.|...S.).Nr..
+00000e00: 0000 2908 7225 0000 0072 3900 0000 7211  ..).r%...r9...r.
+00000e10: 0000 0072 0b00 0000 7215 0000 0072 0d00  ...r....r....r..
+00000e20: 0000 7216 0000 0072 0f00 0000 723a 0000  ..r....r....r:..
+00000e30: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00000e40: 7217 0000 007c 0000 0073 0c00 0000 000b  r....|...s......
+00000e50: 0c01 0601 0601 0401 0cfc 7a18 5175 6572  ..........z.Quer
+00000e60: 7953 6572 7669 6365 2e4c 6973 7451 7565  yService.ListQue
+00000e70: 7269 6573 2908 721a 0000 004e 4e46 4e4e  ries).r....NNFNN
+00000e80: 4e4e 2908 721a 0000 004e 4e46 4e4e 4e4e  NN).r....NNFNNNN
+00000e90: 2908 721a 0000 004e 4e46 4e4e 4e4e 2908  ).r....NNFNNNN).
+00000ea0: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000eb0: 2000 0000 da0c 7374 6174 6963 6d65 7468   .....staticmeth
+00000ec0: 6f64 7210 0000 0072 1400 0000 7217 0000  odr....r....r...
+00000ed0: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+00000ee0: 721b 0000 0072 3800 0000 5700 0000 733e  r....r8...W...s>
+00000ef0: 0000 0008 0104 0202 0300 0100 0100 0100  ................
+00000f00: 0100 0100 0100 0100 f70c 1002 0300 0100  ................
+00000f10: 0100 0100 0100 0100 0100 0100 f70c 1002  ................
+00000f20: 0300 0100 0100 0100 0100 0100 0100 0100  ................
+00000f30: f772 3800 0000 290a 7220 0000 0072 2500  .r8...).r ...r%.
+00000f40: 0000 da17 6b61 736b 6164 612e 6b61 736b  ....kaskada.kask
+00000f50: 6164 612e 7631 616c 7068 6172 0200 0000  ada.v1alphar....
+00000f60: 720b 0000 00da 066f 626a 6563 7472 0300  r......objectr..
+00000f70: 0000 7221 0000 0072 3700 0000 7238 0000  ..r!...r7...r8..
+00000f80: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+00000f90: 721b 0000 00da 083c 6d6f 6475 6c65 3e02  r......<module>.
+00000fa0: 0000 0073 0c00 0000 0401 0802 0c03 101a  ...s............
+00000fb0: 101d 0818                                ....
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/schema_pb2.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/schema_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 4886 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 1613 0000  o.........5d....
+00000000: 610d 0d0a 0000 0000 2038 4164 1613 0000  a....... 8Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000b 0000 0040 0000 0073 3e01 0000 6400  .....@...s>...d.
+00000020: 000b 0000 0040 0000 0073 3c01 0000 6400  .....@...s<...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
 00000070: a00c a100 5a0d 6401 6407 6c01 6d0e 5a0f  ....Z.d.d.l.m.Z.
 00000080: 0100 6505 a00c a100 a010 6408 a101 5a11  ..e.......d...Z.
 00000090: 6511 6a12 6409 1900 5a13 6511 6a12 640a  e.j.d...Z.e.j.d.
@@ -12,193 +12,188 @@
 000000b0: 6a17 640c 1900 5a18 6509 a019 6409 6507  j.d...Z.e...d.e.
 000000c0: 6a1a 6601 6513 640d 640e 9c02 a103 5a1b  j.f.e.d.d.....Z.
 000000d0: 650d a01c 651b a101 0100 6509 a019 640a  e...e.....e...d.
 000000e0: 6507 6a1a 6601 6509 a019 640b 6507 6a1a  e.j.f.e...d.e.j.
 000000f0: 6601 6516 640d 640e 9c02 a103 6514 640d  f.e.d.d.....e.d.
 00000100: 640f 9c03 a103 5a1d 650d a01c 651d a101  d.....Z.e...e...
 00000110: 0100 650d a01c 651d 6a1e a101 0100 6503  ..e...e.j.....e.
-00000120: 6a1f 6410 6b02 729d 6411 6511 5f20 6412  j.d.k.r.d.e._ d.
-00000130: 6511 5f21 6413 6513 5f22 6414 6513 5f23  e._!d.e._"d.e._#
-00000140: 6415 6518 5f22 6416 6518 5f23 6417 6514  d.e._"d.e._#d.e.
-00000150: 5f22 6418 6514 5f23 6419 6516 5f22 6418  _"d.e._#d.e._"d.
-00000160: 6516 5f23 6411 5300 6411 5300 291a 7a1f  e._#d.S.d.S.).z.
-00000170: 4765 6e65 7261 7465 6420 7072 6f74 6f63  Generated protoc
-00000180: 6f6c 2062 7566 6665 7220 636f 6465 2ee9  ol buffer code..
-00000190: 0000 0000 2901 da0a 6465 7363 7269 7074  ....)...descript
-000001a0: 6f72 2901 da0f 6465 7363 7269 7074 6f72  or)...descriptor
-000001b0: 5f70 6f6f 6c29 01da 076d 6573 7361 6765  _pool)...message
-000001c0: 2901 da0a 7265 666c 6563 7469 6f6e 2901  )...reflection).
-000001d0: da0f 7379 6d62 6f6c 5f64 6174 6162 6173  ..symbol_databas
-000001e0: 6529 01da 0965 6d70 7479 5f70 6232 735c  e)...empty_pb2s\
-000001f0: 0600 000a 246b 6173 6b61 6461 2f6b 6173  ....$kaskada/kas
-00000200: 6b61 6461 2f76 3161 6c70 6861 2f73 6368  kada/v1alpha/sch
-00000210: 656d 612e 7072 6f74 6f12 176b 6173 6b61  ema.proto..kaska
-00000220: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-00000230: 6861 1a1b 676f 6f67 6c65 2f70 726f 746f  ha..google/proto
-00000240: 6275 662f 656d 7074 792e 7072 6f74 6f22  buf/empty.proto"
-00000250: d008 0a08 4461 7461 5479 7065 124f 0a09  ....DataType.O..
-00000260: 7072 696d 6974 6976 6518 0120 0128 0e32  primitive.. .(.2
-00000270: 2f2e 6b61 736b 6164 612e 6b61 736b 6164  /.kaskada.kaskad
-00000280: 612e 7631 616c 7068 612e 4461 7461 5479  a.v1alpha.DataTy
-00000290: 7065 2e50 7269 6d69 7469 7665 5479 7065  pe.PrimitiveType
-000002a0: 4800 5209 7072 696d 6974 6976 6512 390a  H.R.primitive.9.
-000002b0: 0673 7472 7563 7418 0220 0128 0b32 1f2e  .struct.. .(.2..
-000002c0: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
-000002d0: 7631 616c 7068 612e 5363 6865 6d61 4800  v1alpha.SchemaH.
-000002e0: 5206 7374 7275 6374 1230 0a06 7769 6e64  R.struct.0..wind
-000002f0: 6f77 1803 2001 280b 3216 2e67 6f6f 676c  ow.. .(.2..googl
-00000300: 652e 7072 6f74 6f62 7566 2e45 6d70 7479  e.protobuf.Empty
-00000310: 4800 5206 7769 6e64 6f77 1237 0a04 6c69  H.R.window.7..li
-00000320: 7374 1804 2001 280b 3221 2e6b 6173 6b61  st.. .(.2!.kaska
-00000330: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-00000340: 6861 2e44 6174 6154 7970 6548 0052 046c  ha.DataTypeH.R.l
-00000350: 6973 7422 c406 0a0d 5072 696d 6974 6976  ist"....Primitiv
-00000360: 6554 7970 6512 1e0a 1a50 5249 4d49 5449  eType....PRIMITI
-00000370: 5645 5f54 5950 455f 554e 5350 4543 4946  VE_TYPE_UNSPECIF
-00000380: 4945 4410 0012 170a 1350 5249 4d49 5449  IED......PRIMITI
-00000390: 5645 5f54 5950 455f 4e55 4c4c 1001 1217  VE_TYPE_NULL....
-000003a0: 0a13 5052 494d 4954 4956 455f 5459 5045  ..PRIMITIVE_TYPE
-000003b0: 5f42 4f4f 4c10 0212 150a 1150 5249 4d49  _BOOL......PRIMI
-000003c0: 5449 5645 5f54 5950 455f 4938 1003 1216  TIVE_TYPE_I8....
-000003d0: 0a12 5052 494d 4954 4956 455f 5459 5045  ..PRIMITIVE_TYPE
-000003e0: 5f49 3136 1004 1216 0a12 5052 494d 4954  _I16......PRIMIT
-000003f0: 4956 455f 5459 5045 5f49 3332 1005 1216  IVE_TYPE_I32....
-00000400: 0a12 5052 494d 4954 4956 455f 5459 5045  ..PRIMITIVE_TYPE
-00000410: 5f49 3634 1006 1215 0a11 5052 494d 4954  _I64......PRIMIT
-00000420: 4956 455f 5459 5045 5f55 3810 0712 160a  IVE_TYPE_U8.....
-00000430: 1250 5249 4d49 5449 5645 5f54 5950 455f  .PRIMITIVE_TYPE_
-00000440: 5531 3610 0812 160a 1250 5249 4d49 5449  U16......PRIMITI
-00000450: 5645 5f54 5950 455f 5533 3210 0912 160a  VE_TYPE_U32.....
-00000460: 1250 5249 4d49 5449 5645 5f54 5950 455f  .PRIMITIVE_TYPE_
-00000470: 5536 3410 0a12 160a 1250 5249 4d49 5449  U64......PRIMITI
-00000480: 5645 5f54 5950 455f 4631 3610 0b12 160a  VE_TYPE_F16.....
-00000490: 1250 5249 4d49 5449 5645 5f54 5950 455f  .PRIMITIVE_TYPE_
-000004a0: 4633 3210 0c12 160a 1250 5249 4d49 5449  F32......PRIMITI
-000004b0: 5645 5f54 5950 455f 4636 3410 0d12 190a  VE_TYPE_F64.....
-000004c0: 1550 5249 4d49 5449 5645 5f54 5950 455f  .PRIMITIVE_TYPE_
-000004d0: 5354 5249 4e47 100e 1224 0a20 5052 494d  STRING...$. PRIM
-000004e0: 4954 4956 455f 5459 5045 5f49 4e54 4552  ITIVE_TYPE_INTER
-000004f0: 5641 4c5f 4441 595f 5449 4d45 100f 1226  VAL_DAY_TIME...&
-00000500: 0a22 5052 494d 4954 4956 455f 5459 5045  ."PRIMITIVE_TYPE
-00000510: 5f49 4e54 4552 5641 4c5f 5945 4152 5f4d  _INTERVAL_YEAR_M
-00000520: 4f4e 5448 1010 1222 0a1e 5052 494d 4954  ONTH..."..PRIMIT
-00000530: 4956 455f 5459 5045 5f44 5552 4154 494f  IVE_TYPE_DURATIO
-00000540: 4e5f 5345 434f 4e44 1011 1227 0a23 5052  N_SECOND...'.#PR
-00000550: 494d 4954 4956 455f 5459 5045 5f44 5552  IMITIVE_TYPE_DUR
-00000560: 4154 494f 4e5f 4d49 4c4c 4953 4543 4f4e  ATION_MILLISECON
-00000570: 4410 1212 270a 2350 5249 4d49 5449 5645  D...'.#PRIMITIVE
-00000580: 5f54 5950 455f 4455 5241 5449 4f4e 5f4d  _TYPE_DURATION_M
-00000590: 4943 524f 5345 434f 4e44 1013 1226 0a22  ICROSECOND...&."
-000005a0: 5052 494d 4954 4956 455f 5459 5045 5f44  PRIMITIVE_TYPE_D
-000005b0: 5552 4154 494f 4e5f 4e41 4e4f 5345 434f  URATION_NANOSECO
-000005c0: 4e44 1014 1223 0a1f 5052 494d 4954 4956  ND...#..PRIMITIV
-000005d0: 455f 5459 5045 5f54 494d 4553 5441 4d50  E_TYPE_TIMESTAMP
-000005e0: 5f53 4543 4f4e 4410 1512 280a 2450 5249  _SECOND...(.$PRI
-000005f0: 4d49 5449 5645 5f54 5950 455f 5449 4d45  MITIVE_TYPE_TIME
-00000600: 5354 414d 505f 4d49 4c4c 4953 4543 4f4e  STAMP_MILLISECON
-00000610: 4410 1612 280a 2450 5249 4d49 5449 5645  D...(.$PRIMITIVE
-00000620: 5f54 5950 455f 5449 4d45 5354 414d 505f  _TYPE_TIMESTAMP_
-00000630: 4d49 4352 4f53 4543 4f4e 4410 1712 270a  MICROSECOND...'.
-00000640: 2350 5249 4d49 5449 5645 5f54 5950 455f  #PRIMITIVE_TYPE_
-00000650: 5449 4d45 5354 414d 505f 4e41 4e4f 5345  TIMESTAMP_NANOSE
-00000660: 434f 4e44 1018 1217 0a13 5052 494d 4954  COND......PRIMIT
-00000670: 4956 455f 5459 5045 5f4a 534f 4e10 1912  IVE_TYPE_JSON...
-00000680: 190a 1550 5249 4d49 5449 5645 5f54 5950  ...PRIMITIVE_TYP
-00000690: 455f 4441 5445 3332 101a 4206 0a04 6b69  E_DATE32..B...ki
-000006a0: 6e64 22a4 010a 0653 6368 656d 6112 3d0a  nd"....Schema.=.
-000006b0: 0666 6965 6c64 7318 0120 0328 0b32 252e  .fields.. .(.2%.
-000006c0: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
-000006d0: 7631 616c 7068 612e 5363 6865 6d61 2e46  v1alpha.Schema.F
-000006e0: 6965 6c64 5206 6669 656c 6473 1a5b 0a05  ieldR.fields.[..
-000006f0: 4669 656c 6412 120a 046e 616d 6518 0120  Field....name.. 
-00000700: 0128 0952 046e 616d 6512 3e0a 0964 6174  .(.R.name.>..dat
-00000710: 615f 7479 7065 1802 2001 280b 3221 2e6b  a_type.. .(.2!.k
-00000720: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
-00000730: 3161 6c70 6861 2e44 6174 6154 7970 6552  1alpha.DataTypeR
-00000740: 0864 6174 6154 7970 6542 fb01 0a1b 636f  .dataTypeB....co
-00000750: 6d2e 6b61 736b 6164 612e 6b61 736b 6164  m.kaskada.kaskad
-00000760: 612e 7631 616c 7068 6142 0b53 6368 656d  a.v1alphaB.Schem
-00000770: 6150 726f 746f 5001 5a51 6769 7468 7562  aProtoP.ZQgithub
-00000780: 2e63 6f6d 2f6b 6173 6b61 6461 2d61 692f  .com/kaskada-ai/
-00000790: 6b61 736b 6164 612f 6765 6e2f 7072 6f74  kaskada/gen/prot
-000007a0: 6f2f 676f 2f6b 6173 6b61 6461 2f6b 6173  o/go/kaskada/kas
-000007b0: 6b61 6461 2f76 3161 6c70 6861 3b6b 6173  kada/v1alpha;kas
-000007c0: 6b61 6461 7631 616c 7068 61a2 0203 4b4b  kadav1alpha...KK
-000007d0: 58aa 0217 4b61 736b 6164 612e 4b61 736b  X...Kaskada.Kask
-000007e0: 6164 612e 5631 616c 7068 61ca 0217 4b61  ada.V1alpha...Ka
-000007f0: 736b 6164 615c 4b61 736b 6164 615c 5631  skada\Kaskada\V1
-00000800: 616c 7068 61e2 0223 4b61 736b 6164 615c  alpha..#Kaskada\
-00000810: 4b61 736b 6164 615c 5631 616c 7068 615c  Kaskada\V1alpha\
-00000820: 4750 424d 6574 6164 6174 61ea 0219 4b61  GPBMetadata...Ka
-00000830: 736b 6164 613a 3a4b 6173 6b61 6461 3a3a  skada::Kaskada::
-00000840: 5631 616c 7068 6162 0670 726f 746f 33da  V1alphab.proto3.
-00000850: 0844 6174 6154 7970 65da 0653 6368 656d  .DataType..Schem
-00000860: 61da 0546 6965 6c64 da0d 5072 696d 6974  a..Field..Primit
-00000870: 6976 6554 7970 657a 226b 6173 6b61 6461  iveTypez"kaskada
-00000880: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
-00000890: 2e73 6368 656d 615f 7062 3229 02da 0a44  .schema_pb2)...D
-000008a0: 4553 4352 4950 544f 52da 0a5f 5f6d 6f64  ESCRIPTOR..__mod
-000008b0: 756c 655f 5f29 0372 0a00 0000 720c 0000  ule__).r....r...
-000008c0: 0072 0d00 0000 464e 73fb 0000 000a 1b63  .r....FNs......c
-000008d0: 6f6d 2e6b 6173 6b61 6461 2e6b 6173 6b61  om.kaskada.kaska
-000008e0: 6461 2e76 3161 6c70 6861 420b 5363 6865  da.v1alphaB.Sche
-000008f0: 6d61 5072 6f74 6f50 015a 5167 6974 6875  maProtoP.ZQgithu
-00000900: 622e 636f 6d2f 6b61 736b 6164 612d 6169  b.com/kaskada-ai
-00000910: 2f6b 6173 6b61 6461 2f67 656e 2f70 726f  /kaskada/gen/pro
-00000920: 746f 2f67 6f2f 6b61 736b 6164 612f 6b61  to/go/kaskada/ka
-00000930: 736b 6164 612f 7631 616c 7068 613b 6b61  skada/v1alpha;ka
-00000940: 736b 6164 6176 3161 6c70 6861 a202 034b  skadav1alpha...K
-00000950: 4b58 aa02 174b 6173 6b61 6461 2e4b 6173  KX...Kaskada.Kas
-00000960: 6b61 6461 2e56 3161 6c70 6861 ca02 174b  kada.V1alpha...K
-00000970: 6173 6b61 6461 5c4b 6173 6b61 6461 5c56  askada\Kaskada\V
-00000980: 3161 6c70 6861 e202 234b 6173 6b61 6461  1alpha..#Kaskada
-00000990: 5c4b 6173 6b61 6461 5c56 3161 6c70 6861  \Kaskada\V1alpha
-000009a0: 5c47 5042 4d65 7461 6461 7461 ea02 194b  \GPBMetadata...K
-000009b0: 6173 6b61 6461 3a3a 4b61 736b 6164 613a  askada::Kaskada:
-000009c0: 3a56 3161 6c70 6861 e95f 0000 0069 af04  :V1alpha._...i..
-000009d0: 0000 6963 0100 0069 a704 0000 69b2 0400  ..ic...i....i...
-000009e0: 0069 5605 0000 69fb 0400 0029 24da 075f  .iV...i....)$.._
-000009f0: 5f64 6f63 5f5f da0f 676f 6f67 6c65 2e70  _doc__..google.p
-00000a00: 726f 746f 6275 6672 0200 0000 da0b 5f64  rotobufr......_d
-00000a10: 6573 6372 6970 746f 7272 0300 0000 da10  escriptorr......
-00000a20: 5f64 6573 6372 6970 746f 725f 706f 6f6c  _descriptor_pool
-00000a30: 7204 0000 00da 085f 6d65 7373 6167 6572  r......_messager
-00000a40: 0500 0000 da0b 5f72 6566 6c65 6374 696f  ......_reflectio
-00000a50: 6e72 0600 0000 da10 5f73 796d 626f 6c5f  nr......_symbol_
-00000a60: 6461 7461 6261 7365 da07 4465 6661 756c  database..Defaul
-00000a70: 74da 075f 7379 6d5f 6462 7207 0000 00da  t.._sym_dbr.....
-00000a80: 2267 6f6f 676c 655f 646f 745f 7072 6f74  "google_dot_prot
-00000a90: 6f62 7566 5f64 6f74 5f65 6d70 7479 5f5f  obuf_dot_empty__
-00000aa0: 7062 32da 1141 6464 5365 7269 616c 697a  pb2..AddSerializ
-00000ab0: 6564 4669 6c65 720c 0000 00da 156d 6573  edFiler......mes
-00000ac0: 7361 6765 5f74 7970 6573 5f62 795f 6e61  sage_types_by_na
-00000ad0: 6d65 da09 5f44 4154 4154 5950 45da 075f  me.._DATATYPE.._
-00000ae0: 5343 4845 4d41 da14 6e65 7374 6564 5f74  SCHEMA..nested_t
-00000af0: 7970 6573 5f62 795f 6e61 6d65 da0d 5f53  ypes_by_name.._S
-00000b00: 4348 454d 415f 4649 454c 44da 1265 6e75  CHEMA_FIELD..enu
-00000b10: 6d5f 7479 7065 735f 6279 5f6e 616d 65da  m_types_by_name.
-00000b20: 175f 4441 5441 5459 5045 5f50 5249 4d49  ._DATATYPE_PRIMI
-00000b30: 5449 5645 5459 5045 da1c 4765 6e65 7261  TIVETYPE..Genera
-00000b40: 7465 6450 726f 746f 636f 6c4d 6573 7361  tedProtocolMessa
-00000b50: 6765 5479 7065 da07 4d65 7373 6167 6572  geType..Messager
-00000b60: 0800 0000 da0f 5265 6769 7374 6572 4d65  ......RegisterMe
-00000b70: 7373 6167 6572 0900 0000 720a 0000 00da  ssager....r.....
-00000b80: 125f 5553 455f 435f 4445 5343 5249 5054  ._USE_C_DESCRIPT
-00000b90: 4f52 53da 085f 6f70 7469 6f6e 73da 135f  ORS.._options.._
-00000ba0: 7365 7269 616c 697a 6564 5f6f 7074 696f  serialized_optio
-00000bb0: 6e73 da11 5f73 6572 6961 6c69 7a65 645f  ns.._serialized_
-00000bc0: 7374 6172 74da 0f5f 7365 7269 616c 697a  start.._serializ
-00000bd0: 6564 5f65 6e64 a900 7229 0000 0072 2900  ed_end..r)...r).
-00000be0: 0000 fa70 2f68 6f6d 652f 7468 6572 6170  ...p/home/therap
-00000bf0: 6f6e 2f52 6570 6f73 2f47 6974 4875 622f  on/Repos/GitHub/
-00000c00: 4b61 736b 6164 6141 492f 6b61 736b 6164  KaskadaAI/kaskad
-00000c10: 612f 7265 6c65 6173 696e 672f 636c 6965  a/releasing/clie
-00000c20: 6e74 732f 7079 7468 6f6e 2f73 7263 2f6b  nts/python/src/k
-00000c30: 6173 6b61 6461 2f6b 6173 6b61 6461 2f76  askada/kaskada/v
-00000c40: 3161 6c70 6861 2f73 6368 656d 615f 7062  1alpha/schema_pb
-00000c50: 322e 7079 da08 3c6d 6f64 756c 653e 0100  2.py..<module>..
-00000c60: 0000 7350 0000 0004 030c 010c 010c 010c  ..sP............
-00000c70: 010c 0108 030c 030e 030a 040a 010a 010a  ................
-00000c80: 010c 0102 0102 0108 fe0a 050c 020c 0202  ................
-00000c90: 0102 0106 fe02 0602 0108 f70a 0c0c 010a  ................
-00000ca0: 0206 0206 0106 0106 0106 0106 0106 0106  ................
-00000cb0: 0106 010a 0104 f5                        .......
+00000120: 6a1f 6410 6b02 9001 7238 6411 6511 5f20  j.d.k...r8d.e._ 
+00000130: 6412 6511 5f21 6413 6513 5f22 6414 6513  d.e._!d.e._"d.e.
+00000140: 5f23 6415 6518 5f22 6416 6518 5f23 6417  _#d.e._"d.e._#d.
+00000150: 6514 5f22 6418 6514 5f23 6419 6516 5f22  e._"d.e._#d.e._"
+00000160: 6418 6516 5f23 6411 5300 291a 7a1f 4765  d.e._#d.S.).z.Ge
+00000170: 6e65 7261 7465 6420 7072 6f74 6f63 6f6c  nerated protocol
+00000180: 2062 7566 6665 7220 636f 6465 2ee9 0000   buffer code....
+00000190: 0000 2901 da0a 6465 7363 7269 7074 6f72  ..)...descriptor
+000001a0: 2901 da0f 6465 7363 7269 7074 6f72 5f70  )...descriptor_p
+000001b0: 6f6f 6c29 01da 076d 6573 7361 6765 2901  ool)...message).
+000001c0: da0a 7265 666c 6563 7469 6f6e 2901 da0f  ..reflection)...
+000001d0: 7379 6d62 6f6c 5f64 6174 6162 6173 6529  symbol_database)
+000001e0: 01da 0965 6d70 7479 5f70 6232 735c 0600  ...empty_pb2s\..
+000001f0: 000a 246b 6173 6b61 6461 2f6b 6173 6b61  ..$kaskada/kaska
+00000200: 6461 2f76 3161 6c70 6861 2f73 6368 656d  da/v1alpha/schem
+00000210: 612e 7072 6f74 6f12 176b 6173 6b61 6461  a.proto..kaskada
+00000220: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00000230: 1a1b 676f 6f67 6c65 2f70 726f 746f 6275  ..google/protobu
+00000240: 662f 656d 7074 792e 7072 6f74 6f22 d008  f/empty.proto"..
+00000250: 0a08 4461 7461 5479 7065 124f 0a09 7072  ..DataType.O..pr
+00000260: 696d 6974 6976 6518 0120 0128 0e32 2f2e  imitive.. .(.2/.
+00000270: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000280: 7631 616c 7068 612e 4461 7461 5479 7065  v1alpha.DataType
+00000290: 2e50 7269 6d69 7469 7665 5479 7065 4800  .PrimitiveTypeH.
+000002a0: 5209 7072 696d 6974 6976 6512 390a 0673  R.primitive.9..s
+000002b0: 7472 7563 7418 0220 0128 0b32 1f2e 6b61  truct.. .(.2..ka
+000002c0: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
+000002d0: 616c 7068 612e 5363 6865 6d61 4800 5206  alpha.SchemaH.R.
+000002e0: 7374 7275 6374 1230 0a06 7769 6e64 6f77  struct.0..window
+000002f0: 1803 2001 280b 3216 2e67 6f6f 676c 652e  .. .(.2..google.
+00000300: 7072 6f74 6f62 7566 2e45 6d70 7479 4800  protobuf.EmptyH.
+00000310: 5206 7769 6e64 6f77 1237 0a04 6c69 7374  R.window.7..list
+00000320: 1804 2001 280b 3221 2e6b 6173 6b61 6461  .. .(.2!.kaskada
+00000330: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00000340: 2e44 6174 6154 7970 6548 0052 046c 6973  .DataTypeH.R.lis
+00000350: 7422 c406 0a0d 5072 696d 6974 6976 6554  t"....PrimitiveT
+00000360: 7970 6512 1e0a 1a50 5249 4d49 5449 5645  ype....PRIMITIVE
+00000370: 5f54 5950 455f 554e 5350 4543 4946 4945  _TYPE_UNSPECIFIE
+00000380: 4410 0012 170a 1350 5249 4d49 5449 5645  D......PRIMITIVE
+00000390: 5f54 5950 455f 4e55 4c4c 1001 1217 0a13  _TYPE_NULL......
+000003a0: 5052 494d 4954 4956 455f 5459 5045 5f42  PRIMITIVE_TYPE_B
+000003b0: 4f4f 4c10 0212 150a 1150 5249 4d49 5449  OOL......PRIMITI
+000003c0: 5645 5f54 5950 455f 4938 1003 1216 0a12  VE_TYPE_I8......
+000003d0: 5052 494d 4954 4956 455f 5459 5045 5f49  PRIMITIVE_TYPE_I
+000003e0: 3136 1004 1216 0a12 5052 494d 4954 4956  16......PRIMITIV
+000003f0: 455f 5459 5045 5f49 3332 1005 1216 0a12  E_TYPE_I32......
+00000400: 5052 494d 4954 4956 455f 5459 5045 5f49  PRIMITIVE_TYPE_I
+00000410: 3634 1006 1215 0a11 5052 494d 4954 4956  64......PRIMITIV
+00000420: 455f 5459 5045 5f55 3810 0712 160a 1250  E_TYPE_U8......P
+00000430: 5249 4d49 5449 5645 5f54 5950 455f 5531  RIMITIVE_TYPE_U1
+00000440: 3610 0812 160a 1250 5249 4d49 5449 5645  6......PRIMITIVE
+00000450: 5f54 5950 455f 5533 3210 0912 160a 1250  _TYPE_U32......P
+00000460: 5249 4d49 5449 5645 5f54 5950 455f 5536  RIMITIVE_TYPE_U6
+00000470: 3410 0a12 160a 1250 5249 4d49 5449 5645  4......PRIMITIVE
+00000480: 5f54 5950 455f 4631 3610 0b12 160a 1250  _TYPE_F16......P
+00000490: 5249 4d49 5449 5645 5f54 5950 455f 4633  RIMITIVE_TYPE_F3
+000004a0: 3210 0c12 160a 1250 5249 4d49 5449 5645  2......PRIMITIVE
+000004b0: 5f54 5950 455f 4636 3410 0d12 190a 1550  _TYPE_F64......P
+000004c0: 5249 4d49 5449 5645 5f54 5950 455f 5354  RIMITIVE_TYPE_ST
+000004d0: 5249 4e47 100e 1224 0a20 5052 494d 4954  RING...$. PRIMIT
+000004e0: 4956 455f 5459 5045 5f49 4e54 4552 5641  IVE_TYPE_INTERVA
+000004f0: 4c5f 4441 595f 5449 4d45 100f 1226 0a22  L_DAY_TIME...&."
+00000500: 5052 494d 4954 4956 455f 5459 5045 5f49  PRIMITIVE_TYPE_I
+00000510: 4e54 4552 5641 4c5f 5945 4152 5f4d 4f4e  NTERVAL_YEAR_MON
+00000520: 5448 1010 1222 0a1e 5052 494d 4954 4956  TH..."..PRIMITIV
+00000530: 455f 5459 5045 5f44 5552 4154 494f 4e5f  E_TYPE_DURATION_
+00000540: 5345 434f 4e44 1011 1227 0a23 5052 494d  SECOND...'.#PRIM
+00000550: 4954 4956 455f 5459 5045 5f44 5552 4154  ITIVE_TYPE_DURAT
+00000560: 494f 4e5f 4d49 4c4c 4953 4543 4f4e 4410  ION_MILLISECOND.
+00000570: 1212 270a 2350 5249 4d49 5449 5645 5f54  ..'.#PRIMITIVE_T
+00000580: 5950 455f 4455 5241 5449 4f4e 5f4d 4943  YPE_DURATION_MIC
+00000590: 524f 5345 434f 4e44 1013 1226 0a22 5052  ROSECOND...&."PR
+000005a0: 494d 4954 4956 455f 5459 5045 5f44 5552  IMITIVE_TYPE_DUR
+000005b0: 4154 494f 4e5f 4e41 4e4f 5345 434f 4e44  ATION_NANOSECOND
+000005c0: 1014 1223 0a1f 5052 494d 4954 4956 455f  ...#..PRIMITIVE_
+000005d0: 5459 5045 5f54 494d 4553 5441 4d50 5f53  TYPE_TIMESTAMP_S
+000005e0: 4543 4f4e 4410 1512 280a 2450 5249 4d49  ECOND...(.$PRIMI
+000005f0: 5449 5645 5f54 5950 455f 5449 4d45 5354  TIVE_TYPE_TIMEST
+00000600: 414d 505f 4d49 4c4c 4953 4543 4f4e 4410  AMP_MILLISECOND.
+00000610: 1612 280a 2450 5249 4d49 5449 5645 5f54  ..(.$PRIMITIVE_T
+00000620: 5950 455f 5449 4d45 5354 414d 505f 4d49  YPE_TIMESTAMP_MI
+00000630: 4352 4f53 4543 4f4e 4410 1712 270a 2350  CROSECOND...'.#P
+00000640: 5249 4d49 5449 5645 5f54 5950 455f 5449  RIMITIVE_TYPE_TI
+00000650: 4d45 5354 414d 505f 4e41 4e4f 5345 434f  MESTAMP_NANOSECO
+00000660: 4e44 1018 1217 0a13 5052 494d 4954 4956  ND......PRIMITIV
+00000670: 455f 5459 5045 5f4a 534f 4e10 1912 190a  E_TYPE_JSON.....
+00000680: 1550 5249 4d49 5449 5645 5f54 5950 455f  .PRIMITIVE_TYPE_
+00000690: 4441 5445 3332 101a 4206 0a04 6b69 6e64  DATE32..B...kind
+000006a0: 22a4 010a 0653 6368 656d 6112 3d0a 0666  "....Schema.=..f
+000006b0: 6965 6c64 7318 0120 0328 0b32 252e 6b61  ields.. .(.2%.ka
+000006c0: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
+000006d0: 616c 7068 612e 5363 6865 6d61 2e46 6965  alpha.Schema.Fie
+000006e0: 6c64 5206 6669 656c 6473 1a5b 0a05 4669  ldR.fields.[..Fi
+000006f0: 656c 6412 120a 046e 616d 6518 0120 0128  eld....name.. .(
+00000700: 0952 046e 616d 6512 3e0a 0964 6174 615f  .R.name.>..data_
+00000710: 7479 7065 1802 2001 280b 3221 2e6b 6173  type.. .(.2!.kas
+00000720: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
+00000730: 6c70 6861 2e44 6174 6154 7970 6552 0864  lpha.DataTypeR.d
+00000740: 6174 6154 7970 6542 fb01 0a1b 636f 6d2e  ataTypeB....com.
+00000750: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000760: 7631 616c 7068 6142 0b53 6368 656d 6150  v1alphaB.SchemaP
+00000770: 726f 746f 5001 5a51 6769 7468 7562 2e63  rotoP.ZQgithub.c
+00000780: 6f6d 2f6b 6173 6b61 6461 2d61 692f 6b61  om/kaskada-ai/ka
+00000790: 736b 6164 612f 6765 6e2f 7072 6f74 6f2f  skada/gen/proto/
+000007a0: 676f 2f6b 6173 6b61 6461 2f6b 6173 6b61  go/kaskada/kaska
+000007b0: 6461 2f76 3161 6c70 6861 3b6b 6173 6b61  da/v1alpha;kaska
+000007c0: 6461 7631 616c 7068 61a2 0203 4b4b 58aa  dav1alpha...KKX.
+000007d0: 0217 4b61 736b 6164 612e 4b61 736b 6164  ..Kaskada.Kaskad
+000007e0: 612e 5631 616c 7068 61ca 0217 4b61 736b  a.V1alpha...Kask
+000007f0: 6164 615c 4b61 736b 6164 615c 5631 616c  ada\Kaskada\V1al
+00000800: 7068 61e2 0223 4b61 736b 6164 615c 4b61  pha..#Kaskada\Ka
+00000810: 736b 6164 615c 5631 616c 7068 615c 4750  skada\V1alpha\GP
+00000820: 424d 6574 6164 6174 61ea 0219 4b61 736b  BMetadata...Kask
+00000830: 6164 613a 3a4b 6173 6b61 6461 3a3a 5631  ada::Kaskada::V1
+00000840: 616c 7068 6162 0670 726f 746f 33da 0844  alphab.proto3..D
+00000850: 6174 6154 7970 65da 0653 6368 656d 61da  ataType..Schema.
+00000860: 0546 6965 6c64 5a0d 5072 696d 6974 6976  .FieldZ.Primitiv
+00000870: 6554 7970 657a 226b 6173 6b61 6461 2e6b  eTypez"kaskada.k
+00000880: 6173 6b61 6461 2e76 3161 6c70 6861 2e73  askada.v1alpha.s
+00000890: 6368 656d 615f 7062 3229 02da 0a44 4553  chema_pb2)...DES
+000008a0: 4352 4950 544f 52da 0a5f 5f6d 6f64 756c  CRIPTOR..__modul
+000008b0: 655f 5f29 0372 0a00 0000 720b 0000 0072  e__).r....r....r
+000008c0: 0c00 0000 464e 73fb 0000 000a 1b63 6f6d  ....FNs......com
+000008d0: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+000008e0: 2e76 3161 6c70 6861 420b 5363 6865 6d61  .v1alphaB.Schema
+000008f0: 5072 6f74 6f50 015a 5167 6974 6875 622e  ProtoP.ZQgithub.
+00000900: 636f 6d2f 6b61 736b 6164 612d 6169 2f6b  com/kaskada-ai/k
+00000910: 6173 6b61 6461 2f67 656e 2f70 726f 746f  askada/gen/proto
+00000920: 2f67 6f2f 6b61 736b 6164 612f 6b61 736b  /go/kaskada/kask
+00000930: 6164 612f 7631 616c 7068 613b 6b61 736b  ada/v1alpha;kask
+00000940: 6164 6176 3161 6c70 6861 a202 034b 4b58  adav1alpha...KKX
+00000950: aa02 174b 6173 6b61 6461 2e4b 6173 6b61  ...Kaskada.Kaska
+00000960: 6461 2e56 3161 6c70 6861 ca02 174b 6173  da.V1alpha...Kas
+00000970: 6b61 6461 5c4b 6173 6b61 6461 5c56 3161  kada\Kaskada\V1a
+00000980: 6c70 6861 e202 234b 6173 6b61 6461 5c4b  lpha..#Kaskada\K
+00000990: 6173 6b61 6461 5c56 3161 6c70 6861 5c47  askada\V1alpha\G
+000009a0: 5042 4d65 7461 6461 7461 ea02 194b 6173  PBMetadata...Kas
+000009b0: 6b61 6461 3a3a 4b61 736b 6164 613a 3a56  kada::Kaskada::V
+000009c0: 3161 6c70 6861 e95f 0000 0069 af04 0000  1alpha._...i....
+000009d0: 6963 0100 0069 a704 0000 69b2 0400 0069  ic...i....i....i
+000009e0: 5605 0000 69fb 0400 0029 24da 075f 5f64  V...i....)$..__d
+000009f0: 6f63 5f5f da0f 676f 6f67 6c65 2e70 726f  oc__..google.pro
+00000a00: 746f 6275 6672 0200 0000 da0b 5f64 6573  tobufr......_des
+00000a10: 6372 6970 746f 7272 0300 0000 da10 5f64  criptorr......_d
+00000a20: 6573 6372 6970 746f 725f 706f 6f6c 7204  escriptor_poolr.
+00000a30: 0000 00da 085f 6d65 7373 6167 6572 0500  ....._messager..
+00000a40: 0000 da0b 5f72 6566 6c65 6374 696f 6e72  ...._reflectionr
+00000a50: 0600 0000 da10 5f73 796d 626f 6c5f 6461  ......_symbol_da
+00000a60: 7461 6261 7365 da07 4465 6661 756c 74da  tabase..Default.
+00000a70: 075f 7379 6d5f 6462 7207 0000 005a 2267  ._sym_dbr....Z"g
+00000a80: 6f6f 676c 655f 646f 745f 7072 6f74 6f62  oogle_dot_protob
+00000a90: 7566 5f64 6f74 5f65 6d70 7479 5f5f 7062  uf_dot_empty__pb
+00000aa0: 32da 1141 6464 5365 7269 616c 697a 6564  2..AddSerialized
+00000ab0: 4669 6c65 720b 0000 00da 156d 6573 7361  Filer......messa
+00000ac0: 6765 5f74 7970 6573 5f62 795f 6e61 6d65  ge_types_by_name
+00000ad0: 5a09 5f44 4154 4154 5950 455a 075f 5343  Z._DATATYPEZ._SC
+00000ae0: 4845 4d41 da14 6e65 7374 6564 5f74 7970  HEMA..nested_typ
+00000af0: 6573 5f62 795f 6e61 6d65 5a0d 5f53 4348  es_by_nameZ._SCH
+00000b00: 454d 415f 4649 454c 44da 1265 6e75 6d5f  EMA_FIELD..enum_
+00000b10: 7479 7065 735f 6279 5f6e 616d 655a 175f  types_by_nameZ._
+00000b20: 4441 5441 5459 5045 5f50 5249 4d49 5449  DATATYPE_PRIMITI
+00000b30: 5645 5459 5045 da1c 4765 6e65 7261 7465  VETYPE..Generate
+00000b40: 6450 726f 746f 636f 6c4d 6573 7361 6765  dProtocolMessage
+00000b50: 5479 7065 da07 4d65 7373 6167 6572 0800  Type..Messager..
+00000b60: 0000 da0f 5265 6769 7374 6572 4d65 7373  ....RegisterMess
+00000b70: 6167 6572 0900 0000 720a 0000 00da 125f  ager....r......_
+00000b80: 5553 455f 435f 4445 5343 5249 5054 4f52  USE_C_DESCRIPTOR
+00000b90: 53da 085f 6f70 7469 6f6e 73da 135f 7365  S.._options.._se
+00000ba0: 7269 616c 697a 6564 5f6f 7074 696f 6e73  rialized_options
+00000bb0: da11 5f73 6572 6961 6c69 7a65 645f 7374  .._serialized_st
+00000bc0: 6172 74da 0f5f 7365 7269 616c 697a 6564  art.._serialized
+00000bd0: 5f65 6e64 a900 7223 0000 0072 2300 0000  _end..r#...r#...
+00000be0: fa2e 2f73 7263 2f73 7263 2f6b 6173 6b61  ../src/src/kaska
+00000bf0: 6461 2f6b 6173 6b61 6461 2f76 3161 6c70  da/kaskada/v1alp
+00000c00: 6861 2f73 6368 656d 615f 7062 322e 7079  ha/schema_pb2.py
+00000c10: da08 3c6d 6f64 756c 653e 0400 0000 734c  ..<module>....sL
+00000c20: 0000 0004 010c 010c 010c 010c 010c 0308  ................
+00000c30: 030c 030e 040a 010a 010a 010a 010c 0102  ................
+00000c40: 0102 fe08 050a 020c 020c 0102 0102 fe06  ................
+00000c50: 0602 0102 f708 0c0a 010c 020c 0206 0106  ................
+00000c60: 0106 0106 0106 0106 0106 0106 0106 01    ...............
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/sources_pb2.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/sources_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 3258 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,136 +1,132 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 ba0c 0000  o.........5d....
+00000000: 610d 0d0a 0000 0000 2038 4164 ba0c 0000  a....... 8Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
+00000020: 0007 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
 00000070: a00c a100 5a0d 6401 6407 6c0e 6d0f 5a10  ....Z.d.d.l.m.Z.
 00000080: 0100 6505 a00c a100 a011 6408 a101 5a12  ..e.......d...Z.
 00000090: 6512 6a13 6409 1900 5a14 6512 6a13 640a  e.j.d...Z.e.j.d.
 000000a0: 1900 5a15 6512 6a13 640b 1900 5a16 6509  ..Z.e.j.d...Z.e.
 000000b0: a017 6409 6507 6a18 6601 6514 640c 640d  ..d.e.j.f.e.d.d.
 000000c0: 9c02 a103 5a19 650d a01a 6519 a101 0100  ....Z.e...e.....
 000000d0: 6509 a017 640a 6507 6a18 6601 6515 640c  e...d.e.j.f.e.d.
 000000e0: 640d 9c02 a103 5a1b 650d a01a 651b a101  d.....Z.e...e...
 000000f0: 0100 6509 a017 640b 6507 6a18 6601 6516  ..e...d.e.j.f.e.
 00000100: 640c 640d 9c02 a103 5a1c 650d a01a 651c  d.d.....Z.e...e.
-00000110: a101 0100 6503 6a1d 640e 6b02 7292 640f  ....e.j.d.k.r.d.
-00000120: 6512 5f1e 6410 6512 5f1f 6411 6514 5f20  e._.d.e._.d.e._ 
-00000130: 6412 6514 5f21 6413 6515 5f20 6414 6515  d.e._!d.e._ d.e.
-00000140: 5f21 6415 6516 5f20 6416 6516 5f21 640f  _!d.e._ d.e._!d.
-00000150: 5300 640f 5300 2917 7a1f 4765 6e65 7261  S.d.S.).z.Genera
-00000160: 7465 6420 7072 6f74 6f63 6f6c 2062 7566  ted protocol buf
-00000170: 6665 7220 636f 6465 2ee9 0000 0000 2901  fer code......).
-00000180: da0a 6465 7363 7269 7074 6f72 2901 da0f  ..descriptor)...
-00000190: 6465 7363 7269 7074 6f72 5f70 6f6f 6c29  descriptor_pool)
-000001a0: 01da 076d 6573 7361 6765 2901 da0a 7265  ...message)...re
-000001b0: 666c 6563 7469 6f6e 2901 da0f 7379 6d62  flection)...symb
-000001c0: 6f6c 5f64 6174 6162 6173 6529 01da 0a70  ol_database)...p
-000001d0: 756c 7361 725f 7062 3273 6702 0000 0a25  ulsar_pb2sg....%
-000001e0: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
-000001f0: 7631 616c 7068 612f 736f 7572 6365 732e  v1alpha/sources.
-00000200: 7072 6f74 6f12 176b 6173 6b61 6461 2e6b  proto..kaskada.k
-00000210: 6173 6b61 6461 2e76 3161 6c70 6861 1a24  askada.v1alpha.$
-00000220: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
-00000230: 7631 616c 7068 612f 7075 6c73 6172 2e70  v1alpha/pulsar.p
-00000240: 726f 746f 2297 010a 0653 6f75 7263 6512  roto"....Source.
-00000250: 420a 076b 6173 6b61 6461 1801 2001 280b  B..kaskada.. .(.
-00000260: 3226 2e6b 6173 6b61 6461 2e6b 6173 6b61  2&.kaskada.kaska
-00000270: 6461 2e76 3161 6c70 6861 2e4b 6173 6b61  da.v1alpha.Kaska
-00000280: 6461 536f 7572 6365 4800 5207 6b61 736b  daSourceH.R.kask
-00000290: 6164 6112 3f0a 0670 756c 7361 7218 0220  ada.?..pulsar.. 
-000002a0: 0128 0b32 252e 6b61 736b 6164 612e 6b61  .(.2%.kaskada.ka
-000002b0: 736b 6164 612e 7631 616c 7068 612e 5075  skada.v1alpha.Pu
-000002c0: 6c73 6172 536f 7572 6365 4800 5206 7075  lsarSourceH.R.pu
-000002d0: 6c73 6172 4208 0a06 736f 7572 6365 220f  lsarB...source".
-000002e0: 0a0d 4b61 736b 6164 6153 6f75 7263 6522  ..KaskadaSource"
-000002f0: 4d0a 0c50 756c 7361 7253 6f75 7263 6512  M..PulsarSource.
-00000300: 3d0a 0663 6f6e 6669 6718 0120 0128 0b32  =..config.. .(.2
-00000310: 252e 6b61 736b 6164 612e 6b61 736b 6164  %.kaskada.kaskad
-00000320: 612e 7631 616c 7068 612e 5075 6c73 6172  a.v1alpha.Pulsar
-00000330: 436f 6e66 6967 5206 636f 6e66 6967 42fc  ConfigR.configB.
-00000340: 010a 1b63 6f6d 2e6b 6173 6b61 6461 2e6b  ...com.kaskada.k
-00000350: 6173 6b61 6461 2e76 3161 6c70 6861 420c  askada.v1alphaB.
-00000360: 536f 7572 6365 7350 726f 746f 5001 5a51  SourcesProtoP.ZQ
-00000370: 6769 7468 7562 2e63 6f6d 2f6b 6173 6b61  github.com/kaska
-00000380: 6461 2d61 692f 6b61 736b 6164 612f 6765  da-ai/kaskada/ge
-00000390: 6e2f 7072 6f74 6f2f 676f 2f6b 6173 6b61  n/proto/go/kaska
-000003a0: 6461 2f6b 6173 6b61 6461 2f76 3161 6c70  da/kaskada/v1alp
-000003b0: 6861 3b6b 6173 6b61 6461 7631 616c 7068  ha;kaskadav1alph
-000003c0: 61a2 0203 4b4b 58aa 0217 4b61 736b 6164  a...KKX...Kaskad
-000003d0: 612e 4b61 736b 6164 612e 5631 616c 7068  a.Kaskada.V1alph
-000003e0: 61ca 0217 4b61 736b 6164 615c 4b61 736b  a...Kaskada\Kask
-000003f0: 6164 615c 5631 616c 7068 61e2 0223 4b61  ada\V1alpha..#Ka
-00000400: 736b 6164 615c 4b61 736b 6164 615c 5631  skada\Kaskada\V1
-00000410: 616c 7068 615c 4750 424d 6574 6164 6174  alpha\GPBMetadat
-00000420: 61ea 0219 4b61 736b 6164 613a 3a4b 6173  a...Kaskada::Kas
-00000430: 6b61 6461 3a3a 5631 616c 7068 6162 0670  kada::V1alphab.p
-00000440: 726f 746f 33da 0653 6f75 7263 65da 0d4b  roto3..Source..K
-00000450: 6173 6b61 6461 536f 7572 6365 da0c 5075  askadaSource..Pu
-00000460: 6c73 6172 536f 7572 6365 7a23 6b61 736b  lsarSourcez#kask
-00000470: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-00000480: 7068 612e 736f 7572 6365 735f 7062 3229  pha.sources_pb2)
-00000490: 02da 0a44 4553 4352 4950 544f 52da 0a5f  ...DESCRIPTOR.._
-000004a0: 5f6d 6f64 756c 655f 5f46 4e73 fc00 0000  _module__FNs....
-000004b0: 0a1b 636f 6d2e 6b61 736b 6164 612e 6b61  ..com.kaskada.ka
-000004c0: 736b 6164 612e 7631 616c 7068 6142 0c53  skada.v1alphaB.S
-000004d0: 6f75 7263 6573 5072 6f74 6f50 015a 5167  ourcesProtoP.ZQg
-000004e0: 6974 6875 622e 636f 6d2f 6b61 736b 6164  ithub.com/kaskad
-000004f0: 612d 6169 2f6b 6173 6b61 6461 2f67 656e  a-ai/kaskada/gen
-00000500: 2f70 726f 746f 2f67 6f2f 6b61 736b 6164  /proto/go/kaskad
-00000510: 612f 6b61 736b 6164 612f 7631 616c 7068  a/kaskada/v1alph
-00000520: 613b 6b61 736b 6164 6176 3161 6c70 6861  a;kaskadav1alpha
-00000530: a202 034b 4b58 aa02 174b 6173 6b61 6461  ...KKX...Kaskada
-00000540: 2e4b 6173 6b61 6461 2e56 3161 6c70 6861  .Kaskada.V1alpha
-00000550: ca02 174b 6173 6b61 6461 5c4b 6173 6b61  ...Kaskada\Kaska
-00000560: 6461 5c56 3161 6c70 6861 e202 234b 6173  da\V1alpha..#Kas
-00000570: 6b61 6461 5c4b 6173 6b61 6461 5c56 3161  kada\Kaskada\V1a
-00000580: 6c70 6861 5c47 5042 4d65 7461 6461 7461  lpha\GPBMetadata
-00000590: ea02 194b 6173 6b61 6461 3a3a 4b61 736b  ...Kaskada::Kask
-000005a0: 6164 613a 3a56 3161 6c70 6861 e969 0000  ada::V1alpha.i..
-000005b0: 00e9 0001 0000 6902 0100 0069 1101 0000  ......i....i....
-000005c0: 6913 0100 0069 6001 0000 2922 da07 5f5f  i....i`...)"..__
-000005d0: 646f 635f 5fda 0f67 6f6f 676c 652e 7072  doc__..google.pr
-000005e0: 6f74 6f62 7566 7202 0000 00da 0b5f 6465  otobufr......_de
-000005f0: 7363 7269 7074 6f72 7203 0000 00da 105f  scriptorr......_
-00000600: 6465 7363 7269 7074 6f72 5f70 6f6f 6c72  descriptor_poolr
-00000610: 0400 0000 da08 5f6d 6573 7361 6765 7205  ......_messager.
-00000620: 0000 00da 0b5f 7265 666c 6563 7469 6f6e  ....._reflection
-00000630: 7206 0000 00da 105f 7379 6d62 6f6c 5f64  r......_symbol_d
-00000640: 6174 6162 6173 65da 0744 6566 6175 6c74  atabase..Default
-00000650: da07 5f73 796d 5f64 62da 176b 6173 6b61  .._sym_db..kaska
-00000660: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-00000670: 6861 7207 0000 00da 2f6b 6173 6b61 6461  har...../kaskada
-00000680: 5f64 6f74 5f6b 6173 6b61 6461 5f64 6f74  _dot_kaskada_dot
-00000690: 5f76 3161 6c70 6861 5f64 6f74 5f70 756c  _v1alpha_dot_pul
-000006a0: 7361 725f 5f70 6232 da11 4164 6453 6572  sar__pb2..AddSer
-000006b0: 6961 6c69 7a65 6446 696c 6572 0b00 0000  ializedFiler....
-000006c0: da15 6d65 7373 6167 655f 7479 7065 735f  ..message_types_
-000006d0: 6279 5f6e 616d 65da 075f 534f 5552 4345  by_name.._SOURCE
-000006e0: da0e 5f4b 4153 4b41 4441 534f 5552 4345  .._KASKADASOURCE
-000006f0: da0d 5f50 554c 5341 5253 4f55 5243 45da  .._PULSARSOURCE.
-00000700: 1c47 656e 6572 6174 6564 5072 6f74 6f63  .GeneratedProtoc
-00000710: 6f6c 4d65 7373 6167 6554 7970 65da 074d  olMessageType..M
-00000720: 6573 7361 6765 7208 0000 00da 0f52 6567  essager......Reg
-00000730: 6973 7465 724d 6573 7361 6765 7209 0000  isterMessager...
-00000740: 0072 0a00 0000 da12 5f55 5345 5f43 5f44  .r......_USE_C_D
-00000750: 4553 4352 4950 544f 5253 da08 5f6f 7074  ESCRIPTORS.._opt
-00000760: 696f 6e73 da13 5f73 6572 6961 6c69 7a65  ions.._serialize
-00000770: 645f 6f70 7469 6f6e 73da 115f 7365 7269  d_options.._seri
-00000780: 616c 697a 6564 5f73 7461 7274 da0f 5f73  alized_start.._s
-00000790: 6572 6961 6c69 7a65 645f 656e 64a9 0072  erialized_end..r
-000007a0: 2700 0000 7227 0000 00fa 712f 686f 6d65  '...r'....q/home
-000007b0: 2f74 6865 7261 706f 6e2f 5265 706f 732f  /therapon/Repos/
-000007c0: 4769 7448 7562 2f4b 6173 6b61 6461 4149  GitHub/KaskadaAI
-000007d0: 2f6b 6173 6b61 6461 2f72 656c 6561 7369  /kaskada/releasi
-000007e0: 6e67 2f63 6c69 656e 7473 2f70 7974 686f  ng/clients/pytho
-000007f0: 6e2f 7372 632f 6b61 736b 6164 612f 6b61  n/src/kaskada/ka
-00000800: 736b 6164 612f 7631 616c 7068 612f 736f  skada/v1alpha/so
-00000810: 7572 6365 735f 7062 322e 7079 da08 3c6d  urces_pb2.py..<m
-00000820: 6f64 756c 653e 0100 0000 734a 0000 0004  odule>....sJ....
-00000830: 030c 010c 010c 010c 010c 0108 030c 030e  ................
-00000840: 030a 040a 010a 010c 0102 0102 0108 fe0a  ................
-00000850: 050c 0202 0102 0108 fe0a 050c 0202 0102  ................
-00000860: 0108 fe0a 050a 0206 0206 0106 0106 0106  ................
-00000870: 0106 0106 010a 0104 f7                   .........
+00000110: a101 0100 6503 6a1d 640e 6b02 9001 7222  ....e.j.d.k...r"
+00000120: 640f 6512 5f1e 6410 6512 5f1f 6411 6514  d.e._.d.e._.d.e.
+00000130: 5f20 6412 6514 5f21 6413 6515 5f20 6414  _ d.e._!d.e._ d.
+00000140: 6515 5f21 6415 6516 5f20 6416 6516 5f21  e._!d.e._ d.e._!
+00000150: 640f 5300 2917 7a1f 4765 6e65 7261 7465  d.S.).z.Generate
+00000160: 6420 7072 6f74 6f63 6f6c 2062 7566 6665  d protocol buffe
+00000170: 7220 636f 6465 2ee9 0000 0000 2901 da0a  r code......)...
+00000180: 6465 7363 7269 7074 6f72 2901 da0f 6465  descriptor)...de
+00000190: 7363 7269 7074 6f72 5f70 6f6f 6c29 01da  scriptor_pool)..
+000001a0: 076d 6573 7361 6765 2901 da0a 7265 666c  .message)...refl
+000001b0: 6563 7469 6f6e 2901 da0f 7379 6d62 6f6c  ection)...symbol
+000001c0: 5f64 6174 6162 6173 6529 01da 0a70 756c  _database)...pul
+000001d0: 7361 725f 7062 3273 6702 0000 0a25 6b61  sar_pb2sg....%ka
+000001e0: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
+000001f0: 616c 7068 612f 736f 7572 6365 732e 7072  alpha/sources.pr
+00000200: 6f74 6f12 176b 6173 6b61 6461 2e6b 6173  oto..kaskada.kas
+00000210: 6b61 6461 2e76 3161 6c70 6861 1a24 6b61  kada.v1alpha.$ka
+00000220: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
+00000230: 616c 7068 612f 7075 6c73 6172 2e70 726f  alpha/pulsar.pro
+00000240: 746f 2297 010a 0653 6f75 7263 6512 420a  to"....Source.B.
+00000250: 076b 6173 6b61 6461 1801 2001 280b 3226  .kaskada.. .(.2&
+00000260: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00000270: 2e76 3161 6c70 6861 2e4b 6173 6b61 6461  .v1alpha.Kaskada
+00000280: 536f 7572 6365 4800 5207 6b61 736b 6164  SourceH.R.kaskad
+00000290: 6112 3f0a 0670 756c 7361 7218 0220 0128  a.?..pulsar.. .(
+000002a0: 0b32 252e 6b61 736b 6164 612e 6b61 736b  .2%.kaskada.kask
+000002b0: 6164 612e 7631 616c 7068 612e 5075 6c73  ada.v1alpha.Puls
+000002c0: 6172 536f 7572 6365 4800 5206 7075 6c73  arSourceH.R.puls
+000002d0: 6172 4208 0a06 736f 7572 6365 220f 0a0d  arB...source"...
+000002e0: 4b61 736b 6164 6153 6f75 7263 6522 4d0a  KaskadaSource"M.
+000002f0: 0c50 756c 7361 7253 6f75 7263 6512 3d0a  .PulsarSource.=.
+00000300: 0663 6f6e 6669 6718 0120 0128 0b32 252e  .config.. .(.2%.
+00000310: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000320: 7631 616c 7068 612e 5075 6c73 6172 436f  v1alpha.PulsarCo
+00000330: 6e66 6967 5206 636f 6e66 6967 42fc 010a  nfigR.configB...
+00000340: 1b63 6f6d 2e6b 6173 6b61 6461 2e6b 6173  .com.kaskada.kas
+00000350: 6b61 6461 2e76 3161 6c70 6861 420c 536f  kada.v1alphaB.So
+00000360: 7572 6365 7350 726f 746f 5001 5a51 6769  urcesProtoP.ZQgi
+00000370: 7468 7562 2e63 6f6d 2f6b 6173 6b61 6461  thub.com/kaskada
+00000380: 2d61 692f 6b61 736b 6164 612f 6765 6e2f  -ai/kaskada/gen/
+00000390: 7072 6f74 6f2f 676f 2f6b 6173 6b61 6461  proto/go/kaskada
+000003a0: 2f6b 6173 6b61 6461 2f76 3161 6c70 6861  /kaskada/v1alpha
+000003b0: 3b6b 6173 6b61 6461 7631 616c 7068 61a2  ;kaskadav1alpha.
+000003c0: 0203 4b4b 58aa 0217 4b61 736b 6164 612e  ..KKX...Kaskada.
+000003d0: 4b61 736b 6164 612e 5631 616c 7068 61ca  Kaskada.V1alpha.
+000003e0: 0217 4b61 736b 6164 615c 4b61 736b 6164  ..Kaskada\Kaskad
+000003f0: 615c 5631 616c 7068 61e2 0223 4b61 736b  a\V1alpha..#Kask
+00000400: 6164 615c 4b61 736b 6164 615c 5631 616c  ada\Kaskada\V1al
+00000410: 7068 615c 4750 424d 6574 6164 6174 61ea  pha\GPBMetadata.
+00000420: 0219 4b61 736b 6164 613a 3a4b 6173 6b61  ..Kaskada::Kaska
+00000430: 6461 3a3a 5631 616c 7068 6162 0670 726f  da::V1alphab.pro
+00000440: 746f 33da 0653 6f75 7263 65da 0d4b 6173  to3..Source..Kas
+00000450: 6b61 6461 536f 7572 6365 da0c 5075 6c73  kadaSource..Puls
+00000460: 6172 536f 7572 6365 7a23 6b61 736b 6164  arSourcez#kaskad
+00000470: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00000480: 612e 736f 7572 6365 735f 7062 3229 02da  a.sources_pb2)..
+00000490: 0a44 4553 4352 4950 544f 52da 0a5f 5f6d  .DESCRIPTOR..__m
+000004a0: 6f64 756c 655f 5f46 4e73 fc00 0000 0a1b  odule__FNs......
+000004b0: 636f 6d2e 6b61 736b 6164 612e 6b61 736b  com.kaskada.kask
+000004c0: 6164 612e 7631 616c 7068 6142 0c53 6f75  ada.v1alphaB.Sou
+000004d0: 7263 6573 5072 6f74 6f50 015a 5167 6974  rcesProtoP.ZQgit
+000004e0: 6875 622e 636f 6d2f 6b61 736b 6164 612d  hub.com/kaskada-
+000004f0: 6169 2f6b 6173 6b61 6461 2f67 656e 2f70  ai/kaskada/gen/p
+00000500: 726f 746f 2f67 6f2f 6b61 736b 6164 612f  roto/go/kaskada/
+00000510: 6b61 736b 6164 612f 7631 616c 7068 613b  kaskada/v1alpha;
+00000520: 6b61 736b 6164 6176 3161 6c70 6861 a202  kaskadav1alpha..
+00000530: 034b 4b58 aa02 174b 6173 6b61 6461 2e4b  .KKX...Kaskada.K
+00000540: 6173 6b61 6461 2e56 3161 6c70 6861 ca02  askada.V1alpha..
+00000550: 174b 6173 6b61 6461 5c4b 6173 6b61 6461  .Kaskada\Kaskada
+00000560: 5c56 3161 6c70 6861 e202 234b 6173 6b61  \V1alpha..#Kaska
+00000570: 6461 5c4b 6173 6b61 6461 5c56 3161 6c70  da\Kaskada\V1alp
+00000580: 6861 5c47 5042 4d65 7461 6461 7461 ea02  ha\GPBMetadata..
+00000590: 194b 6173 6b61 6461 3a3a 4b61 736b 6164  .Kaskada::Kaskad
+000005a0: 613a 3a56 3161 6c70 6861 e969 0000 00e9  a::V1alpha.i....
+000005b0: 0001 0000 6902 0100 0069 1101 0000 6913  ....i....i....i.
+000005c0: 0100 0069 6001 0000 2922 da07 5f5f 646f  ...i`...)"..__do
+000005d0: 635f 5fda 0f67 6f6f 676c 652e 7072 6f74  c__..google.prot
+000005e0: 6f62 7566 7202 0000 00da 0b5f 6465 7363  obufr......_desc
+000005f0: 7269 7074 6f72 7203 0000 00da 105f 6465  riptorr......_de
+00000600: 7363 7269 7074 6f72 5f70 6f6f 6c72 0400  scriptor_poolr..
+00000610: 0000 da08 5f6d 6573 7361 6765 7205 0000  ...._messager...
+00000620: 00da 0b5f 7265 666c 6563 7469 6f6e 7206  ..._reflectionr.
+00000630: 0000 00da 105f 7379 6d62 6f6c 5f64 6174  ....._symbol_dat
+00000640: 6162 6173 65da 0744 6566 6175 6c74 da07  abase..Default..
+00000650: 5f73 796d 5f64 62da 176b 6173 6b61 6461  _sym_db..kaskada
+00000660: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00000670: 7207 0000 00da 2f6b 6173 6b61 6461 5f64  r...../kaskada_d
+00000680: 6f74 5f6b 6173 6b61 6461 5f64 6f74 5f76  ot_kaskada_dot_v
+00000690: 3161 6c70 6861 5f64 6f74 5f70 756c 7361  1alpha_dot_pulsa
+000006a0: 725f 5f70 6232 da11 4164 6453 6572 6961  r__pb2..AddSeria
+000006b0: 6c69 7a65 6446 696c 6572 0b00 0000 da15  lizedFiler......
+000006c0: 6d65 7373 6167 655f 7479 7065 735f 6279  message_types_by
+000006d0: 5f6e 616d 655a 075f 534f 5552 4345 5a0e  _nameZ._SOURCEZ.
+000006e0: 5f4b 4153 4b41 4441 534f 5552 4345 5a0d  _KASKADASOURCEZ.
+000006f0: 5f50 554c 5341 5253 4f55 5243 45da 1c47  _PULSARSOURCE..G
+00000700: 656e 6572 6174 6564 5072 6f74 6f63 6f6c  eneratedProtocol
+00000710: 4d65 7373 6167 6554 7970 65da 074d 6573  MessageType..Mes
+00000720: 7361 6765 7208 0000 00da 0f52 6567 6973  sager......Regis
+00000730: 7465 724d 6573 7361 6765 7209 0000 0072  terMessager....r
+00000740: 0a00 0000 da12 5f55 5345 5f43 5f44 4553  ......_USE_C_DES
+00000750: 4352 4950 544f 5253 da08 5f6f 7074 696f  CRIPTORS.._optio
+00000760: 6e73 da13 5f73 6572 6961 6c69 7a65 645f  ns.._serialized_
+00000770: 6f70 7469 6f6e 73da 115f 7365 7269 616c  options.._serial
+00000780: 697a 6564 5f73 7461 7274 da0f 5f73 6572  ized_start.._ser
+00000790: 6961 6c69 7a65 645f 656e 64a9 0072 2400  ialized_end..r$.
+000007a0: 0000 7224 0000 00fa 2f2f 7372 632f 7372  ..r$....//src/sr
+000007b0: 632f 6b61 736b 6164 612f 6b61 736b 6164  c/kaskada/kaskad
+000007c0: 612f 7631 616c 7068 612f 736f 7572 6365  a/v1alpha/source
+000007d0: 735f 7062 322e 7079 da08 3c6d 6f64 756c  s_pb2.py..<modul
+000007e0: 653e 0400 0000 7346 0000 0004 010c 010c  e>....sF........
+000007f0: 010c 010c 010c 0308 030c 030e 040a 010a  ................
+00000800: 010a 010c 0102 0102 fe08 050a 020c 0102  ................
+00000810: 0102 fe08 050a 020c 0102 0102 fe08 050a  ................
+00000820: 020c 0206 0106 0106 0106 0106 0106 0106  ................
+00000830: 01                                       .
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/table_service_pb2.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/table_service_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 15322 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 da3b 0000  o.........5d.;..
+00000000: 610d 0d0a 0000 0000 2038 4164 da3b 0000  a....... 8Ad.;..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 4c05 0000 6400  .....@...sL...d.
+00000020: 0007 0000 0040 0000 0073 4805 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
 00000070: a00c a100 5a0d 6401 6407 6c0e 6d0f 5a10  ....Z.d.d.l.m.Z.
 00000080: 0100 6401 6408 6c0e 6d11 5a12 0100 6401  ..d.d.l.m.Z...d.
 00000090: 6409 6c01 6d13 5a14 0100 6401 640a 6c01  d.l.m.Z...d.d.l.
@@ -39,15 +39,15 @@
 00000260: 0100 6509 a02f 6418 6507 6a30 6601 652c  ..e../d.e.j0f.e,
 00000270: 641b 641c 9c02 a103 5a3a 650d a032 653a  d.d.....Z:e..2e:
 00000280: a101 0100 6509 a02f 6419 6507 6a30 6601  ....e../d.e.j0f.
 00000290: 652d 641b 641c 9c02 a103 5a3b 650d a032  e-d.d.....Z;e..2
 000002a0: 653b a101 0100 6509 a02f 641a 6507 6a30  e;....e../d.e.j0
 000002b0: 6601 652e 641b 641c 9c02 a103 5a3c 650d  f.e.d.d.....Z<e.
 000002c0: a032 653c a101 0100 6522 6a3d 641d 1900  .2e<....e"j=d...
-000002d0: 5a3e 6503 6a3f 641e 6b02 9002 72a4 641f  Z>e.j?d.k...r.d.
+000002d0: 5a3e 6503 6a3f 641e 6b02 9005 7244 641f  Z>e.j?d.k...rDd.
 000002e0: 6522 5f40 6420 6522 5f41 641f 6524 6a42  e"_@d e"_Ad.e$jB
 000002f0: 6421 1900 5f40 6422 6524 6a42 6421 1900  d!.._@d"e$jBd!..
 00000300: 5f41 641f 6524 6a42 6423 1900 5f40 6424  _Ad.e$jBd#.._@d$
 00000310: 6524 6a42 6423 1900 5f41 641f 6524 6a42  e$jBd#.._Ad.e$jB
 00000320: 6425 1900 5f40 6424 6524 6a42 6425 1900  d%.._@d$e$jBd%..
 00000330: 5f41 641f 6524 6a42 6426 1900 5f40 6424  _Ad.e$jBd&.._@d$
 00000340: 6524 6a42 6426 1900 5f41 641f 6524 6a42  e$jBd&.._Ad.e$jB
@@ -81,395 +81,390 @@
 00000500: 6442 6526 5f46 6443 6527 5f45 6444 6527  dBe&_FdCe'_EdDe'
 00000510: 5f46 6445 6528 5f45 6446 6528 5f46 6447  _FdEe(_EdFe(_FdG
 00000520: 6529 5f45 6448 6529 5f46 6449 652a 5f45  e)_EdHe)_FdIe*_E
 00000530: 644a 652a 5f46 644b 652b 5f45 644c 652b  dJe*_FdKe+_EdLe+
 00000540: 5f46 644d 652c 5f45 644e 652c 5f46 644f  _FdMe,_EdNe,_FdO
 00000550: 652d 5f45 6450 652d 5f46 6451 652e 5f45  e-_EdPe-_FdQe._E
 00000560: 6452 652e 5f46 6453 653e 5f45 6454 653e  dRe._FdSe>_EdTe>
-00000570: 5f46 641f 5300 641f 5300 2955 7a1f 4765  _Fd.S.d.S.)Uz.Ge
-00000580: 6e65 7261 7465 6420 7072 6f74 6f63 6f6c  nerated protocol
-00000590: 2062 7566 6665 7220 636f 6465 2ee9 0000   buffer code....
-000005a0: 0000 2901 da0a 6465 7363 7269 7074 6f72  ..)...descriptor
-000005b0: 2901 da0f 6465 7363 7269 7074 6f72 5f70  )...descriptor_p
-000005c0: 6f6f 6c29 01da 076d 6573 7361 6765 2901  ool)...message).
-000005d0: da0a 7265 666c 6563 7469 6f6e 2901 da0f  ..reflection)...
-000005e0: 7379 6d62 6f6c 5f64 6174 6162 6173 6529  symbol_database)
-000005f0: 01da 0f61 6e6e 6f74 6174 696f 6e73 5f70  ...annotations_p
-00000600: 6232 2901 da12 6669 656c 645f 6265 6861  b2)...field_beha
-00000610: 7669 6f72 5f70 6232 2901 da0d 7469 6d65  vior_pb2)...time
-00000620: 7374 616d 705f 7062 3229 01da 0c77 7261  stamp_pb2)...wra
-00000630: 7070 6572 735f 7062 3229 01da 0a63 6f6d  ppers_pb2)...com
-00000640: 6d6f 6e5f 7062 3229 01da 0a73 6368 656d  mon_pb2)...schem
-00000650: 615f 7062 3229 01da 0b73 6f75 7263 6573  a_pb2)...sources
-00000660: 5f70 6232 2901 da0c 7661 6c69 6461 7465  _pb2)...validate
-00000670: 5f70 6232 73a6 0c00 000a 2b6b 6173 6b61  _pb2s.....+kaska
-00000680: 6461 2f6b 6173 6b61 6461 2f76 3161 6c70  da/kaskada/v1alp
-00000690: 6861 2f74 6162 6c65 5f73 6572 7669 6365  ha/table_service
-000006a0: 2e70 726f 746f 1217 6b61 736b 6164 612e  .proto..kaskada.
-000006b0: 6b61 736b 6164 612e 7631 616c 7068 611a  kaskada.v1alpha.
-000006c0: 1c67 6f6f 676c 652f 6170 692f 616e 6e6f  .google/api/anno
-000006d0: 7461 7469 6f6e 732e 7072 6f74 6f1a 1f67  tations.proto..g
-000006e0: 6f6f 676c 652f 6170 692f 6669 656c 645f  oogle/api/field_
-000006f0: 6265 6861 7669 6f72 2e70 726f 746f 1a1f  behavior.proto..
-00000700: 676f 6f67 6c65 2f70 726f 746f 6275 662f  google/protobuf/
-00000710: 7469 6d65 7374 616d 702e 7072 6f74 6f1a  timestamp.proto.
-00000720: 1e67 6f6f 676c 652f 7072 6f74 6f62 7566  .google/protobuf
-00000730: 2f77 7261 7070 6572 732e 7072 6f74 6f1a  /wrappers.proto.
-00000740: 246b 6173 6b61 6461 2f6b 6173 6b61 6461  $kaskada/kaskada
-00000750: 2f76 3161 6c70 6861 2f63 6f6d 6d6f 6e2e  /v1alpha/common.
-00000760: 7072 6f74 6f1a 246b 6173 6b61 6461 2f6b  proto.$kaskada/k
-00000770: 6173 6b61 6461 2f76 3161 6c70 6861 2f73  askada/v1alpha/s
-00000780: 6368 656d 612e 7072 6f74 6f1a 256b 6173  chema.proto.%kas
-00000790: 6b61 6461 2f6b 6173 6b61 6461 2f76 3161  kada/kaskada/v1a
-000007a0: 6c70 6861 2f73 6f75 7263 6573 2e70 726f  lpha/sources.pro
-000007b0: 746f 1a17 7661 6c69 6461 7465 2f76 616c  to..validate/val
-000007c0: 6964 6174 652e 7072 6f74 6f22 f604 0a05  idate.proto"....
-000007d0: 5461 626c 6512 1e0a 0874 6162 6c65 5f69  Table....table_i
-000007e0: 6418 0120 0128 0942 03e0 4103 5207 7461  d.. .(.B..A.R.ta
-000007f0: 626c 6549 6412 260a 0a74 6162 6c65 5f6e  bleId.&..table_n
-00000800: 616d 6518 0220 0128 0942 07fa 4204 7202  ame.. .(.B..B.r.
-00000810: 1001 5209 7461 626c 654e 616d 6512 310a  ..R.tableName.1.
-00000820: 1074 696d 655f 636f 6c75 6d6e 5f6e 616d  .time_column_nam
-00000830: 6518 0320 0128 0942 07fa 4204 7202 1001  e.. .(.B..B.r...
-00000840: 520e 7469 6d65 436f 6c75 6d6e 4e61 6d65  R.timeColumnName
-00000850: 123c 0a16 656e 7469 7479 5f6b 6579 5f63  .<..entity_key_c
-00000860: 6f6c 756d 6e5f 6e61 6d65 1804 2001 2809  olumn_name.. .(.
-00000870: 4207 fa42 0472 0210 0152 1365 6e74 6974  B..B.r...R.entit
-00000880: 794b 6579 436f 6c75 6d6e 4e61 6d65 1255  yKeyColumnName.U
-00000890: 0a13 7375 6273 6f72 745f 636f 6c75 6d6e  ..subsort_column
-000008a0: 5f6e 616d 6518 0520 0128 0b32 1c2e 676f  _name.. .(.2..go
-000008b0: 6f67 6c65 2e70 726f 746f 6275 662e 5374  ogle.protobuf.St
-000008c0: 7269 6e67 5661 6c75 6542 07fa 4204 7202  ringValueB..B.r.
-000008d0: 1001 5211 7375 6273 6f72 7443 6f6c 756d  ..R.subsortColum
-000008e0: 6e4e 616d 6512 1f0a 0b67 726f 7570 696e  nName....groupin
-000008f0: 675f 6964 1806 2001 2809 520a 6772 6f75  g_id.. .(.R.grou
-00000900: 7069 6e67 4964 1240 0a0b 6372 6561 7465  pingId.@..create
-00000910: 5f74 696d 6518 0720 0128 0b32 1a2e 676f  _time.. .(.2..go
-00000920: 6f67 6c65 2e70 726f 746f 6275 662e 5469  ogle.protobuf.Ti
-00000930: 6d65 7374 616d 7042 03e0 4103 520a 6372  mestampB..A.R.cr
-00000940: 6561 7465 5469 6d65 1240 0a0b 7570 6461  eateTime.@..upda
-00000950: 7465 5f74 696d 6518 0820 0128 0b32 1a2e  te_time.. .(.2..
-00000960: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-00000970: 5469 6d65 7374 616d 7042 03e0 4103 520a  TimestampB..A.R.
-00000980: 7570 6461 7465 5469 6d65 121d 0a07 7665  updateTime....ve
-00000990: 7273 696f 6e18 0920 0128 0342 03e0 4103  rsion.. .(.B..A.
-000009a0: 5207 7665 7273 696f 6e12 3c0a 0673 6368  R.version.<..sch
-000009b0: 656d 6118 0a20 0128 0b32 1f2e 6b61 736b  ema.. .(.2..kask
-000009c0: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-000009d0: 7068 612e 5363 6865 6d61 4203 e041 0352  pha.SchemaB..A.R
-000009e0: 0673 6368 656d 6112 220a 0a66 696c 655f  .schema."..file_
-000009f0: 636f 756e 7418 0b20 0128 0342 03e0 4103  count.. .(.B..A.
-00000a00: 5209 6669 6c65 436f 756e 7412 370a 0673  R.fileCount.7..s
-00000a10: 6f75 7263 6518 0c20 0128 0b32 1f2e 6b61  ource.. .(.2..ka
-00000a20: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
-00000a30: 616c 7068 612e 536f 7572 6365 5206 736f  alpha.SourceR.so
-00000a40: 7572 6365 2273 0a11 4c69 7374 5461 626c  urce"s..ListTabl
-00000a50: 6573 5265 7175 6573 7412 160a 0673 6561  esRequest....sea
-00000a60: 7263 6818 0120 0128 0952 0673 6561 7263  rch.. .(.R.searc
-00000a70: 6812 270a 0970 6167 655f 7369 7a65 1802  h.'..page_size..
-00000a80: 2001 2805 420a fa42 071a 0518 e807 2800   .(.B..B......(.
-00000a90: 5208 7061 6765 5369 7a65 121d 0a0a 7061  R.pageSize....pa
-00000aa0: 6765 5f74 6f6b 656e 1803 2001 2809 5209  ge_token.. .(.R.
-00000ab0: 7061 6765 546f 6b65 6e22 c601 0a12 4c69  pageToken"....Li
-00000ac0: 7374 5461 626c 6573 5265 7370 6f6e 7365  stTablesResponse
-00000ad0: 1236 0a06 7461 626c 6573 1801 2003 280b  .6..tables.. .(.
-00000ae0: 321e 2e6b 6173 6b61 6461 2e6b 6173 6b61  2..kaskada.kaska
-00000af0: 6461 2e76 3161 6c70 6861 2e54 6162 6c65  da.v1alpha.Table
-00000b00: 5206 7461 626c 6573 1226 0a0f 6e65 7874  R.tables.&..next
-00000b10: 5f70 6167 655f 746f 6b65 6e18 0220 0128  _page_token.. .(
-00000b20: 0952 0d6e 6578 7450 6167 6554 6f6b 656e  .R.nextPageToken
-00000b30: 1250 0a0f 7265 7175 6573 745f 6465 7461  .P..request_deta
-00000b40: 696c 7318 0320 0128 0b32 272e 6b61 736b  ils.. .(.2'.kask
-00000b50: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-00000b60: 7068 612e 5265 7175 6573 7444 6574 6169  pha.RequestDetai
-00000b70: 6c73 520e 7265 7175 6573 7444 6574 6169  lsR.requestDetai
-00000b80: 6c73 2239 0a0f 4765 7454 6162 6c65 5265  ls"9..GetTableRe
-00000b90: 7175 6573 7412 260a 0a74 6162 6c65 5f6e  quest.&..table_n
-00000ba0: 616d 6518 0120 0128 0942 07fa 4204 7202  ame.. .(.B..B.r.
-00000bb0: 1001 5209 7461 626c 654e 616d 6522 9a01  ..R.tableName"..
-00000bc0: 0a10 4765 7454 6162 6c65 5265 7370 6f6e  ..GetTableRespon
-00000bd0: 7365 1234 0a05 7461 626c 6518 0120 0128  se.4..table.. .(
-00000be0: 0b32 1e2e 6b61 736b 6164 612e 6b61 736b  .2..kaskada.kask
-00000bf0: 6164 612e 7631 616c 7068 612e 5461 626c  ada.v1alpha.Tabl
-00000c00: 6552 0574 6162 6c65 1250 0a0f 7265 7175  eR.table.P..requ
-00000c10: 6573 745f 6465 7461 696c 7318 0220 0128  est_details.. .(
-00000c20: 0b32 272e 6b61 736b 6164 612e 6b61 736b  .2'.kaskada.kask
-00000c30: 6164 612e 7631 616c 7068 612e 5265 7175  ada.v1alpha.Requ
-00000c40: 6573 7444 6574 6169 6c73 520e 7265 7175  estDetailsR.requ
-00000c50: 6573 7444 6574 6169 6c73 2254 0a12 4372  estDetails"T..Cr
-00000c60: 6561 7465 5461 626c 6552 6571 7565 7374  eateTableRequest
-00000c70: 123e 0a05 7461 626c 6518 0120 0128 0b32  .>..table.. .(.2
-00000c80: 1e2e 6b61 736b 6164 612e 6b61 736b 6164  ..kaskada.kaskad
-00000c90: 612e 7631 616c 7068 612e 5461 626c 6542  a.v1alpha.TableB
-00000ca0: 08fa 4205 8a01 0210 0152 0574 6162 6c65  ..B......R.table
-00000cb0: 229d 010a 1343 7265 6174 6554 6162 6c65  "....CreateTable
-00000cc0: 5265 7370 6f6e 7365 1234 0a05 7461 626c  Response.4..tabl
-00000cd0: 6518 0120 0128 0b32 1e2e 6b61 736b 6164  e.. .(.2..kaskad
-00000ce0: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
-00000cf0: 612e 5461 626c 6552 0574 6162 6c65 1250  a.TableR.table.P
-00000d00: 0a0f 7265 7175 6573 745f 6465 7461 696c  ..request_detail
-00000d10: 7318 0220 0128 0b32 272e 6b61 736b 6164  s.. .(.2'.kaskad
-00000d20: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
-00000d30: 612e 5265 7175 6573 7444 6574 6169 6c73  a.RequestDetails
-00000d40: 520e 7265 7175 6573 7444 6574 6169 6c73  R.requestDetails
-00000d50: 2252 0a12 4465 6c65 7465 5461 626c 6552  "R..DeleteTableR
-00000d60: 6571 7565 7374 1226 0a0a 7461 626c 655f  equest.&..table_
-00000d70: 6e61 6d65 1801 2001 2809 4207 fa42 0472  name.. .(.B..B.r
-00000d80: 0210 0152 0974 6162 6c65 4e61 6d65 1214  ...R.tableName..
-00000d90: 0a05 666f 7263 6518 0220 0128 0852 0566  ..force.. .(.R.f
-00000da0: 6f72 6365 228b 010a 1344 656c 6574 6554  orce"....DeleteT
-00000db0: 6162 6c65 5265 7370 6f6e 7365 1222 0a0d  ableResponse."..
-00000dc0: 6461 7461 5f74 6f6b 656e 5f69 6418 0120  data_token_id.. 
-00000dd0: 0128 0952 0b64 6174 6154 6f6b 656e 4964  .(.R.dataTokenId
-00000de0: 1250 0a0f 7265 7175 6573 745f 6465 7461  .P..request_deta
-00000df0: 696c 7318 0220 0128 0b32 272e 6b61 736b  ils.. .(.2'.kask
-00000e00: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-00000e10: 7068 612e 5265 7175 6573 7444 6574 6169  pha.RequestDetai
-00000e20: 6c73 520e 7265 7175 6573 7444 6574 6169  lsR.requestDetai
-00000e30: 6c73 2292 010a 0f4c 6f61 6444 6174 6152  ls"....LoadDataR
-00000e40: 6571 7565 7374 1226 0a0a 7461 626c 655f  equest.&..table_
-00000e50: 6e61 6d65 1801 2001 2809 4207 fa42 0472  name.. .(.B..B.r
-00000e60: 0210 0152 0974 6162 6c65 4e61 6d65 1243  ...R.tableName.C
-00000e70: 0a0a 6669 6c65 5f69 6e70 7574 1802 2001  ..file_input.. .
-00000e80: 280b 3222 2e6b 6173 6b61 6461 2e6b 6173  (.2".kaskada.kas
-00000e90: 6b61 6461 2e76 3161 6c70 6861 2e46 696c  kada.v1alpha.Fil
-00000ea0: 6549 6e70 7574 4800 5209 6669 6c65 496e  eInputH.R.fileIn
-00000eb0: 7075 7442 120a 0b73 6f75 7263 655f 6461  putB...source_da
-00000ec0: 7461 1203 f842 0122 8801 0a10 4c6f 6164  ta...B."....Load
-00000ed0: 4461 7461 5265 7370 6f6e 7365 1222 0a0d  DataResponse."..
-00000ee0: 6461 7461 5f74 6f6b 656e 5f69 6418 0120  data_token_id.. 
-00000ef0: 0128 0952 0b64 6174 6154 6f6b 656e 4964  .(.R.dataTokenId
-00000f00: 1250 0a0f 7265 7175 6573 745f 6465 7461  .P..request_deta
-00000f10: 696c 7318 0220 0128 0b32 272e 6b61 736b  ils.. .(.2'.kask
-00000f20: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-00000f30: 7068 612e 5265 7175 6573 7444 6574 6169  pha.RequestDetai
-00000f40: 6c73 520e 7265 7175 6573 7444 6574 6169  lsR.requestDetai
-00000f50: 6c73 32be 050a 0c54 6162 6c65 5365 7276  ls2....TableServ
-00000f60: 6963 6512 7e0a 0a4c 6973 7454 6162 6c65  ice.~..ListTable
-00000f70: 7312 2a2e 6b61 736b 6164 612e 6b61 736b  s.*.kaskada.kask
-00000f80: 6164 612e 7631 616c 7068 612e 4c69 7374  ada.v1alpha.List
-00000f90: 5461 626c 6573 5265 7175 6573 741a 2b2e  TablesRequest.+.
-00000fa0: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
-00000fb0: 7631 616c 7068 612e 4c69 7374 5461 626c  v1alpha.ListTabl
-00000fc0: 6573 5265 7370 6f6e 7365 2217 82d3 e493  esResponse".....
-00000fd0: 0211 120f 2f76 3161 6c70 6861 2f74 6162  ..../v1alpha/tab
-00000fe0: 6c65 7312 8701 0a08 4765 7454 6162 6c65  les.....GetTable
-00000ff0: 1228 2e6b 6173 6b61 6461 2e6b 6173 6b61  .(.kaskada.kaska
-00001000: 6461 2e76 3161 6c70 6861 2e47 6574 5461  da.v1alpha.GetTa
-00001010: 626c 6552 6571 7565 7374 1a29 2e6b 6173  bleRequest.).kas
-00001020: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-00001030: 6c70 6861 2e47 6574 5461 626c 6552 6573  lpha.GetTableRes
-00001040: 706f 6e73 6522 2682 d3e4 9302 2012 1e2f  ponse"&..... ../
-00001050: 7631 616c 7068 612f 7461 626c 6573 2f7b  v1alpha/tables/{
-00001060: 7461 626c 655f 6e61 6d65 3d2a 7d12 8801  table_name=*}...
-00001070: 0a0b 4372 6561 7465 5461 626c 6512 2b2e  ..CreateTable.+.
-00001080: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
-00001090: 7631 616c 7068 612e 4372 6561 7465 5461  v1alpha.CreateTa
-000010a0: 626c 6552 6571 7565 7374 1a2c 2e6b 6173  bleRequest.,.kas
-000010b0: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-000010c0: 6c70 6861 2e43 7265 6174 6554 6162 6c65  lpha.CreateTable
-000010d0: 5265 7370 6f6e 7365 221e 82d3 e493 0218  Response".......
-000010e0: 3a05 7461 626c 6522 0f2f 7631 616c 7068  :.table"./v1alph
-000010f0: 612f 7461 626c 6573 1290 010a 0b44 656c  a/tables.....Del
-00001100: 6574 6554 6162 6c65 122b 2e6b 6173 6b61  eteTable.+.kaska
-00001110: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-00001120: 6861 2e44 656c 6574 6554 6162 6c65 5265  ha.DeleteTableRe
-00001130: 7175 6573 741a 2c2e 6b61 736b 6164 612e  quest.,.kaskada.
-00001140: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
-00001150: 4465 6c65 7465 5461 626c 6552 6573 706f  DeleteTableRespo
-00001160: 6e73 6522 2682 d3e4 9302 202a 1e2f 7631  nse"&..... *./v1
-00001170: 616c 7068 612f 7461 626c 6573 2f7b 7461  alpha/tables/{ta
-00001180: 626c 655f 6e61 6d65 3d2a 7d12 8501 0a08  ble_name=*}.....
-00001190: 4c6f 6164 4461 7461 1228 2e6b 6173 6b61  LoadData.(.kaska
-000011a0: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-000011b0: 6861 2e4c 6f61 6444 6174 6152 6571 7565  ha.LoadDataReque
-000011c0: 7374 1a29 2e6b 6173 6b61 6461 2e6b 6173  st.).kaskada.kas
-000011d0: 6b61 6461 2e76 3161 6c70 6861 2e4c 6f61  kada.v1alpha.Loa
-000011e0: 6444 6174 6152 6573 706f 6e73 6522 2482  dDataResponse"$.
-000011f0: d3e4 9302 1e3a 012a 2219 2f76 3161 6c70  .....:.*"./v1alp
-00001200: 6861 2f74 6162 6c65 732f 6c6f 6164 5f64  ha/tables/load_d
-00001210: 6174 6142 8102 0a1b 636f 6d2e 6b61 736b  ataB....com.kask
-00001220: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-00001230: 7068 6142 1154 6162 6c65 5365 7276 6963  phaB.TableServic
-00001240: 6550 726f 746f 5001 5a51 6769 7468 7562  eProtoP.ZQgithub
-00001250: 2e63 6f6d 2f6b 6173 6b61 6461 2d61 692f  .com/kaskada-ai/
-00001260: 6b61 736b 6164 612f 6765 6e2f 7072 6f74  kaskada/gen/prot
-00001270: 6f2f 676f 2f6b 6173 6b61 6461 2f6b 6173  o/go/kaskada/kas
-00001280: 6b61 6461 2f76 3161 6c70 6861 3b6b 6173  kada/v1alpha;kas
-00001290: 6b61 6461 7631 616c 7068 61a2 0203 4b4b  kadav1alpha...KK
-000012a0: 58aa 0217 4b61 736b 6164 612e 4b61 736b  X...Kaskada.Kask
-000012b0: 6164 612e 5631 616c 7068 61ca 0217 4b61  ada.V1alpha...Ka
-000012c0: 736b 6164 615c 4b61 736b 6164 615c 5631  skada\Kaskada\V1
-000012d0: 616c 7068 61e2 0223 4b61 736b 6164 615c  alpha..#Kaskada\
-000012e0: 4b61 736b 6164 615c 5631 616c 7068 615c  Kaskada\V1alpha\
-000012f0: 4750 424d 6574 6164 6174 61ea 0219 4b61  GPBMetadata...Ka
-00001300: 736b 6164 613a 3a4b 6173 6b61 6461 3a3a  skada::Kaskada::
-00001310: 5631 616c 7068 6162 0670 726f 746f 33da  V1alphab.proto3.
-00001320: 0554 6162 6c65 da11 4c69 7374 5461 626c  .Table..ListTabl
-00001330: 6573 5265 7175 6573 74da 124c 6973 7454  esRequest..ListT
-00001340: 6162 6c65 7352 6573 706f 6e73 65da 0f47  ablesResponse..G
-00001350: 6574 5461 626c 6552 6571 7565 7374 da10  etTableRequest..
-00001360: 4765 7454 6162 6c65 5265 7370 6f6e 7365  GetTableResponse
-00001370: da12 4372 6561 7465 5461 626c 6552 6571  ..CreateTableReq
-00001380: 7565 7374 da13 4372 6561 7465 5461 626c  uest..CreateTabl
-00001390: 6552 6573 706f 6e73 65da 1244 656c 6574  eResponse..Delet
-000013a0: 6554 6162 6c65 5265 7175 6573 74da 1344  eTableRequest..D
-000013b0: 656c 6574 6554 6162 6c65 5265 7370 6f6e  eleteTableRespon
-000013c0: 7365 da0f 4c6f 6164 4461 7461 5265 7175  se..LoadDataRequ
-000013d0: 6573 74da 104c 6f61 6444 6174 6152 6573  est..LoadDataRes
-000013e0: 706f 6e73 657a 296b 6173 6b61 6461 2e6b  ponsez)kaskada.k
-000013f0: 6173 6b61 6461 2e76 3161 6c70 6861 2e74  askada.v1alpha.t
-00001400: 6162 6c65 5f73 6572 7669 6365 5f70 6232  able_service_pb2
-00001410: 2902 da0a 4445 5343 5249 5054 4f52 da0a  )...DESCRIPTOR..
-00001420: 5f5f 6d6f 6475 6c65 5f5f da0c 5461 626c  __module__..Tabl
-00001430: 6553 6572 7669 6365 464e 7301 0100 000a  eServiceFNs.....
-00001440: 1b63 6f6d 2e6b 6173 6b61 6461 2e6b 6173  .com.kaskada.kas
-00001450: 6b61 6461 2e76 3161 6c70 6861 4211 5461  kada.v1alphaB.Ta
-00001460: 626c 6553 6572 7669 6365 5072 6f74 6f50  bleServiceProtoP
-00001470: 015a 5167 6974 6875 622e 636f 6d2f 6b61  .ZQgithub.com/ka
-00001480: 736b 6164 612d 6169 2f6b 6173 6b61 6461  skada-ai/kaskada
-00001490: 2f67 656e 2f70 726f 746f 2f67 6f2f 6b61  /gen/proto/go/ka
-000014a0: 736b 6164 612f 6b61 736b 6164 612f 7631  skada/kaskada/v1
-000014b0: 616c 7068 613b 6b61 736b 6164 6176 3161  alpha;kaskadav1a
-000014c0: 6c70 6861 a202 034b 4b58 aa02 174b 6173  lpha...KKX...Kas
-000014d0: 6b61 6461 2e4b 6173 6b61 6461 2e56 3161  kada.Kaskada.V1a
-000014e0: 6c70 6861 ca02 174b 6173 6b61 6461 5c4b  lpha...Kaskada\K
-000014f0: 6173 6b61 6461 5c56 3161 6c70 6861 e202  askada\V1alpha..
-00001500: 234b 6173 6b61 6461 5c4b 6173 6b61 6461  #Kaskada\Kaskada
-00001510: 5c56 3161 6c70 6861 5c47 5042 4d65 7461  \V1alpha\GPBMeta
-00001520: 6461 7461 ea02 194b 6173 6b61 6461 3a3a  data...Kaskada::
-00001530: 4b61 736b 6164 613a 3a56 3161 6c70 6861  Kaskada::V1alpha
-00001540: da08 7461 626c 655f 6964 7303 0000 00e0  ..table_ids.....
-00001550: 4103 da0a 7461 626c 655f 6e61 6d65 7307  A...table_names.
-00001560: 0000 00fa 4204 7202 1001 da10 7469 6d65  ....B.r.....time
-00001570: 5f63 6f6c 756d 6e5f 6e61 6d65 da16 656e  _column_name..en
-00001580: 7469 7479 5f6b 6579 5f63 6f6c 756d 6e5f  tity_key_column_
-00001590: 6e61 6d65 da13 7375 6273 6f72 745f 636f  name..subsort_co
-000015a0: 6c75 6d6e 5f6e 616d 65da 0b63 7265 6174  lumn_name..creat
-000015b0: 655f 7469 6d65 da0b 7570 6461 7465 5f74  e_time..update_t
-000015c0: 696d 65da 0776 6572 7369 6f6e da06 7363  ime..version..sc
-000015d0: 6865 6d61 da0a 6669 6c65 5f63 6f75 6e74  hema..file_count
-000015e0: da09 7061 6765 5f73 697a 6573 0a00 0000  ..page_sizes....
-000015f0: fa42 071a 0518 e807 2800 da05 7461 626c  .B......(...tabl
-00001600: 6573 0800 0000 fa42 058a 0102 1001 da0b  es.....B........
-00001610: 736f 7572 6365 5f64 6174 6173 0300 0000  source_datas....
-00001620: f842 01da 0a4c 6973 7454 6162 6c65 7373  .B...ListTabless
-00001630: 1700 0000 82d3 e493 0211 120f 2f76 3161  ............/v1a
-00001640: 6c70 6861 2f74 6162 6c65 73da 0847 6574  lpha/tables..Get
-00001650: 5461 626c 6573 2600 0000 82d3 e493 0220  Tables&........ 
-00001660: 121e 2f76 3161 6c70 6861 2f74 6162 6c65  ../v1alpha/table
-00001670: 732f 7b74 6162 6c65 5f6e 616d 653d 2a7d  s/{table_name=*}
-00001680: da0b 4372 6561 7465 5461 626c 6573 1e00  ..CreateTables..
-00001690: 0000 82d3 e493 0218 3a05 7461 626c 6522  ........:.table"
-000016a0: 0f2f 7631 616c 7068 612f 7461 626c 6573  ./v1alpha/tables
-000016b0: da0b 4465 6c65 7465 5461 626c 6573 2600  ..DeleteTables&.
-000016c0: 0000 82d3 e493 0220 2a1e 2f76 3161 6c70  ....... *./v1alp
-000016d0: 6861 2f74 6162 6c65 732f 7b74 6162 6c65  ha/tables/{table
-000016e0: 5f6e 616d 653d 2a7d da08 4c6f 6164 4461  _name=*}..LoadDa
-000016f0: 7461 7324 0000 0082 d3e4 9302 1e3a 012a  tas$.........:.*
-00001700: 2219 2f76 3161 6c70 6861 2f74 6162 6c65  "./v1alpha/table
-00001710: 732f 6c6f 6164 5f64 6174 6169 5501 0000  s/load_dataiU...
-00001720: 69cb 0300 0069 cd03 0000 6940 0400 0069  i....i....i@...i
-00001730: 4304 0000 6909 0500 0069 0b05 0000 6944  C...i....i....iD
-00001740: 0500 0069 4705 0000 69e1 0500 0069 e305  ...iG...i....i..
-00001750: 0000 6937 0600 0069 3a06 0000 69d7 0600  ..i7...i:...i...
-00001760: 0069 d906 0000 692b 0700 0069 2e07 0000  .i....i+...i....
-00001770: 69b9 0700 0069 bc07 0000 694e 0800 0069  i....i....iN...i
-00001780: 5108 0000 69d9 0800 0069 dc08 0000 699a  Q...i....i....i.
-00001790: 0b00 0029 47da 075f 5f64 6f63 5f5f da0f  ...)G..__doc__..
-000017a0: 676f 6f67 6c65 2e70 726f 746f 6275 6672  google.protobufr
-000017b0: 0200 0000 da0b 5f64 6573 6372 6970 746f  ......_descripto
-000017c0: 7272 0300 0000 da10 5f64 6573 6372 6970  rr......_descrip
-000017d0: 746f 725f 706f 6f6c 7204 0000 00da 085f  tor_poolr......_
-000017e0: 6d65 7373 6167 6572 0500 0000 da0b 5f72  messager......_r
-000017f0: 6566 6c65 6374 696f 6e72 0600 0000 da10  eflectionr......
-00001800: 5f73 796d 626f 6c5f 6461 7461 6261 7365  _symbol_database
-00001810: da07 4465 6661 756c 74da 075f 7379 6d5f  ..Default.._sym_
-00001820: 6462 da0a 676f 6f67 6c65 2e61 7069 7207  db..google.apir.
-00001830: 0000 00da 2367 6f6f 676c 655f 646f 745f  ....#google_dot_
-00001840: 6170 695f 646f 745f 616e 6e6f 7461 7469  api_dot_annotati
-00001850: 6f6e 735f 5f70 6232 7208 0000 00da 2767  ons__pb2r.....'g
-00001860: 6f6f 676c 655f 646f 745f 6170 695f 646f  oogle_dot_api_do
-00001870: 745f 6669 656c 645f 5f62 6568 6176 696f  t_field__behavio
-00001880: 725f 5f70 6232 7209 0000 00da 2667 6f6f  r__pb2r.....&goo
-00001890: 676c 655f 646f 745f 7072 6f74 6f62 7566  gle_dot_protobuf
-000018a0: 5f64 6f74 5f74 696d 6573 7461 6d70 5f5f  _dot_timestamp__
-000018b0: 7062 3272 0a00 0000 da25 676f 6f67 6c65  pb2r.....%google
-000018c0: 5f64 6f74 5f70 726f 746f 6275 665f 646f  _dot_protobuf_do
-000018d0: 745f 7772 6170 7065 7273 5f5f 7062 32da  t_wrappers__pb2.
-000018e0: 176b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
-000018f0: 2e76 3161 6c70 6861 720b 0000 00da 2f6b  .v1alphar...../k
-00001900: 6173 6b61 6461 5f64 6f74 5f6b 6173 6b61  askada_dot_kaska
-00001910: 6461 5f64 6f74 5f76 3161 6c70 6861 5f64  da_dot_v1alpha_d
-00001920: 6f74 5f63 6f6d 6d6f 6e5f 5f70 6232 720c  ot_common__pb2r.
-00001930: 0000 00da 2f6b 6173 6b61 6461 5f64 6f74  ..../kaskada_dot
-00001940: 5f6b 6173 6b61 6461 5f64 6f74 5f76 3161  _kaskada_dot_v1a
-00001950: 6c70 6861 5f64 6f74 5f73 6368 656d 615f  lpha_dot_schema_
-00001960: 5f70 6232 720d 0000 00da 306b 6173 6b61  _pb2r.....0kaska
-00001970: 6461 5f64 6f74 5f6b 6173 6b61 6461 5f64  da_dot_kaskada_d
-00001980: 6f74 5f76 3161 6c70 6861 5f64 6f74 5f73  ot_v1alpha_dot_s
-00001990: 6f75 7263 6573 5f5f 7062 32da 0876 616c  ources__pb2..val
-000019a0: 6964 6174 6572 0e00 0000 da1a 7661 6c69  idater......vali
-000019b0: 6461 7465 5f64 6f74 5f76 616c 6964 6174  date_dot_validat
-000019c0: 655f 5f70 6232 da11 4164 6453 6572 6961  e__pb2..AddSeria
-000019d0: 6c69 7a65 6446 696c 6572 1a00 0000 da15  lizedFiler......
-000019e0: 6d65 7373 6167 655f 7479 7065 735f 6279  message_types_by
-000019f0: 5f6e 616d 65da 065f 5441 424c 45da 125f  _name.._TABLE.._
-00001a00: 4c49 5354 5441 424c 4553 5245 5155 4553  LISTTABLESREQUES
-00001a10: 54da 135f 4c49 5354 5441 424c 4553 5245  T.._LISTTABLESRE
-00001a20: 5350 4f4e 5345 da10 5f47 4554 5441 424c  SPONSE.._GETTABL
-00001a30: 4552 4551 5545 5354 da11 5f47 4554 5441  EREQUEST.._GETTA
-00001a40: 424c 4552 4553 504f 4e53 45da 135f 4352  BLERESPONSE.._CR
-00001a50: 4541 5445 5441 424c 4552 4551 5545 5354  EATETABLEREQUEST
-00001a60: da14 5f43 5245 4154 4554 4142 4c45 5245  .._CREATETABLERE
-00001a70: 5350 4f4e 5345 da13 5f44 454c 4554 4554  SPONSE.._DELETET
-00001a80: 4142 4c45 5245 5155 4553 54da 145f 4445  ABLEREQUEST.._DE
-00001a90: 4c45 5445 5441 424c 4552 4553 504f 4e53  LETETABLERESPONS
-00001aa0: 45da 105f 4c4f 4144 4441 5441 5245 5155  E.._LOADDATAREQU
-00001ab0: 4553 54da 115f 4c4f 4144 4441 5441 5245  EST.._LOADDATARE
-00001ac0: 5350 4f4e 5345 da1c 4765 6e65 7261 7465  SPONSE..Generate
-00001ad0: 6450 726f 746f 636f 6c4d 6573 7361 6765  dProtocolMessage
-00001ae0: 5479 7065 da07 4d65 7373 6167 6572 0f00  Type..Messager..
-00001af0: 0000 da0f 5265 6769 7374 6572 4d65 7373  ....RegisterMess
-00001b00: 6167 6572 1000 0000 7211 0000 0072 1200  ager....r....r..
-00001b10: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00001b20: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-00001b30: 7219 0000 00da 1073 6572 7669 6365 735f  r......services_
-00001b40: 6279 5f6e 616d 65da 0d5f 5441 424c 4553  by_name.._TABLES
-00001b50: 4552 5649 4345 da12 5f55 5345 5f43 5f44  ERVICE.._USE_C_D
-00001b60: 4553 4352 4950 544f 5253 da08 5f6f 7074  ESCRIPTORS.._opt
-00001b70: 696f 6e73 da13 5f73 6572 6961 6c69 7a65  ions.._serialize
-00001b80: 645f 6f70 7469 6f6e 73da 0e66 6965 6c64  d_options..field
-00001b90: 735f 6279 5f6e 616d 65da 0e6f 6e65 6f66  s_by_name..oneof
-00001ba0: 735f 6279 5f6e 616d 65da 0f6d 6574 686f  s_by_name..metho
-00001bb0: 6473 5f62 795f 6e61 6d65 da11 5f73 6572  ds_by_name.._ser
-00001bc0: 6961 6c69 7a65 645f 7374 6172 74da 0f5f  ialized_start.._
-00001bd0: 7365 7269 616c 697a 6564 5f65 6e64 a900  serialized_end..
-00001be0: 725d 0000 0072 5d00 0000 fa77 2f68 6f6d  r]...r]....w/hom
-00001bf0: 652f 7468 6572 6170 6f6e 2f52 6570 6f73  e/therapon/Repos
-00001c00: 2f47 6974 4875 622f 4b61 736b 6164 6141  /GitHub/KaskadaA
-00001c10: 492f 6b61 736b 6164 612f 7265 6c65 6173  I/kaskada/releas
-00001c20: 696e 672f 636c 6965 6e74 732f 7079 7468  ing/clients/pyth
-00001c30: 6f6e 2f73 7263 2f6b 6173 6b61 6461 2f6b  on/src/kaskada/k
-00001c40: 6173 6b61 6461 2f76 3161 6c70 6861 2f74  askada/v1alpha/t
-00001c50: 6162 6c65 5f73 6572 7669 6365 5f70 6232  able_service_pb2
-00001c60: 2e70 79da 083c 6d6f 6475 6c65 3e01 0000  .py..<module>...
-00001c70: 0073 3201 0000 0403 0c01 0c01 0c01 0c01  .s2.............
-00001c80: 0c01 0803 0c03 0c01 0c01 0c01 0c01 0c01  ................
-00001c90: 0c01 0c01 0e03 0a04 0a01 0a01 0a01 0a01  ................
-00001ca0: 0a01 0a01 0a01 0a01 0a01 0a01 0c01 0201  ................
-00001cb0: 0201 08fe 0a05 0c02 0201 0201 08fe 0a05  ................
-00001cc0: 0c02 0201 0201 08fe 0a05 0c02 0201 0201  ................
-00001cd0: 08fe 0a05 0c02 0201 0201 08fe 0a05 0c02  ................
-00001ce0: 0201 0201 08fe 0a05 0c02 0201 0201 08fe  ................
-00001cf0: 0a05 0c02 0201 0201 08fe 0a05 0c02 0201  ................
-00001d00: 0201 08fe 0a05 0c02 0201 0201 08fe 0a05  ................
-00001d10: 0c02 0201 0201 08fe 0a05 0a02 0c01 0602  ................
-00001d20: 0601 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00001d30: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00001d40: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00001d50: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00001d60: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00001d70: 0c01 0c01 0c01 0601 0601 0601 0601 0601  ................
-00001d80: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00001d90: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00001da0: 0601 0601 0a01 04bb                      ........
+00000570: 5f46 641f 5300 2955 7a1f 4765 6e65 7261  _Fd.S.)Uz.Genera
+00000580: 7465 6420 7072 6f74 6f63 6f6c 2062 7566  ted protocol buf
+00000590: 6665 7220 636f 6465 2ee9 0000 0000 2901  fer code......).
+000005a0: da0a 6465 7363 7269 7074 6f72 2901 da0f  ..descriptor)...
+000005b0: 6465 7363 7269 7074 6f72 5f70 6f6f 6c29  descriptor_pool)
+000005c0: 01da 076d 6573 7361 6765 2901 da0a 7265  ...message)...re
+000005d0: 666c 6563 7469 6f6e 2901 da0f 7379 6d62  flection)...symb
+000005e0: 6f6c 5f64 6174 6162 6173 6529 01da 0f61  ol_database)...a
+000005f0: 6e6e 6f74 6174 696f 6e73 5f70 6232 2901  nnotations_pb2).
+00000600: da12 6669 656c 645f 6265 6861 7669 6f72  ..field_behavior
+00000610: 5f70 6232 2901 da0d 7469 6d65 7374 616d  _pb2)...timestam
+00000620: 705f 7062 3229 01da 0c77 7261 7070 6572  p_pb2)...wrapper
+00000630: 735f 7062 3229 01da 0a63 6f6d 6d6f 6e5f  s_pb2)...common_
+00000640: 7062 3229 01da 0a73 6368 656d 615f 7062  pb2)...schema_pb
+00000650: 3229 01da 0b73 6f75 7263 6573 5f70 6232  2)...sources_pb2
+00000660: 2901 da0c 7661 6c69 6461 7465 5f70 6232  )...validate_pb2
+00000670: 73a6 0c00 000a 2b6b 6173 6b61 6461 2f6b  s.....+kaskada/k
+00000680: 6173 6b61 6461 2f76 3161 6c70 6861 2f74  askada/v1alpha/t
+00000690: 6162 6c65 5f73 6572 7669 6365 2e70 726f  able_service.pro
+000006a0: 746f 1217 6b61 736b 6164 612e 6b61 736b  to..kaskada.kask
+000006b0: 6164 612e 7631 616c 7068 611a 1c67 6f6f  ada.v1alpha..goo
+000006c0: 676c 652f 6170 692f 616e 6e6f 7461 7469  gle/api/annotati
+000006d0: 6f6e 732e 7072 6f74 6f1a 1f67 6f6f 676c  ons.proto..googl
+000006e0: 652f 6170 692f 6669 656c 645f 6265 6861  e/api/field_beha
+000006f0: 7669 6f72 2e70 726f 746f 1a1f 676f 6f67  vior.proto..goog
+00000700: 6c65 2f70 726f 746f 6275 662f 7469 6d65  le/protobuf/time
+00000710: 7374 616d 702e 7072 6f74 6f1a 1e67 6f6f  stamp.proto..goo
+00000720: 676c 652f 7072 6f74 6f62 7566 2f77 7261  gle/protobuf/wra
+00000730: 7070 6572 732e 7072 6f74 6f1a 246b 6173  ppers.proto.$kas
+00000740: 6b61 6461 2f6b 6173 6b61 6461 2f76 3161  kada/kaskada/v1a
+00000750: 6c70 6861 2f63 6f6d 6d6f 6e2e 7072 6f74  lpha/common.prot
+00000760: 6f1a 246b 6173 6b61 6461 2f6b 6173 6b61  o.$kaskada/kaska
+00000770: 6461 2f76 3161 6c70 6861 2f73 6368 656d  da/v1alpha/schem
+00000780: 612e 7072 6f74 6f1a 256b 6173 6b61 6461  a.proto.%kaskada
+00000790: 2f6b 6173 6b61 6461 2f76 3161 6c70 6861  /kaskada/v1alpha
+000007a0: 2f73 6f75 7263 6573 2e70 726f 746f 1a17  /sources.proto..
+000007b0: 7661 6c69 6461 7465 2f76 616c 6964 6174  validate/validat
+000007c0: 652e 7072 6f74 6f22 f604 0a05 5461 626c  e.proto"....Tabl
+000007d0: 6512 1e0a 0874 6162 6c65 5f69 6418 0120  e....table_id.. 
+000007e0: 0128 0942 03e0 4103 5207 7461 626c 6549  .(.B..A.R.tableI
+000007f0: 6412 260a 0a74 6162 6c65 5f6e 616d 6518  d.&..table_name.
+00000800: 0220 0128 0942 07fa 4204 7202 1001 5209  . .(.B..B.r...R.
+00000810: 7461 626c 654e 616d 6512 310a 1074 696d  tableName.1..tim
+00000820: 655f 636f 6c75 6d6e 5f6e 616d 6518 0320  e_column_name.. 
+00000830: 0128 0942 07fa 4204 7202 1001 520e 7469  .(.B..B.r...R.ti
+00000840: 6d65 436f 6c75 6d6e 4e61 6d65 123c 0a16  meColumnName.<..
+00000850: 656e 7469 7479 5f6b 6579 5f63 6f6c 756d  entity_key_colum
+00000860: 6e5f 6e61 6d65 1804 2001 2809 4207 fa42  n_name.. .(.B..B
+00000870: 0472 0210 0152 1365 6e74 6974 794b 6579  .r...R.entityKey
+00000880: 436f 6c75 6d6e 4e61 6d65 1255 0a13 7375  ColumnName.U..su
+00000890: 6273 6f72 745f 636f 6c75 6d6e 5f6e 616d  bsort_column_nam
+000008a0: 6518 0520 0128 0b32 1c2e 676f 6f67 6c65  e.. .(.2..google
+000008b0: 2e70 726f 746f 6275 662e 5374 7269 6e67  .protobuf.String
+000008c0: 5661 6c75 6542 07fa 4204 7202 1001 5211  ValueB..B.r...R.
+000008d0: 7375 6273 6f72 7443 6f6c 756d 6e4e 616d  subsortColumnNam
+000008e0: 6512 1f0a 0b67 726f 7570 696e 675f 6964  e....grouping_id
+000008f0: 1806 2001 2809 520a 6772 6f75 7069 6e67  .. .(.R.grouping
+00000900: 4964 1240 0a0b 6372 6561 7465 5f74 696d  Id.@..create_tim
+00000910: 6518 0720 0128 0b32 1a2e 676f 6f67 6c65  e.. .(.2..google
+00000920: 2e70 726f 746f 6275 662e 5469 6d65 7374  .protobuf.Timest
+00000930: 616d 7042 03e0 4103 520a 6372 6561 7465  ampB..A.R.create
+00000940: 5469 6d65 1240 0a0b 7570 6461 7465 5f74  Time.@..update_t
+00000950: 696d 6518 0820 0128 0b32 1a2e 676f 6f67  ime.. .(.2..goog
+00000960: 6c65 2e70 726f 746f 6275 662e 5469 6d65  le.protobuf.Time
+00000970: 7374 616d 7042 03e0 4103 520a 7570 6461  stampB..A.R.upda
+00000980: 7465 5469 6d65 121d 0a07 7665 7273 696f  teTime....versio
+00000990: 6e18 0920 0128 0342 03e0 4103 5207 7665  n.. .(.B..A.R.ve
+000009a0: 7273 696f 6e12 3c0a 0673 6368 656d 6118  rsion.<..schema.
+000009b0: 0a20 0128 0b32 1f2e 6b61 736b 6164 612e  . .(.2..kaskada.
+000009c0: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
+000009d0: 5363 6865 6d61 4203 e041 0352 0673 6368  SchemaB..A.R.sch
+000009e0: 656d 6112 220a 0a66 696c 655f 636f 756e  ema."..file_coun
+000009f0: 7418 0b20 0128 0342 03e0 4103 5209 6669  t.. .(.B..A.R.fi
+00000a00: 6c65 436f 756e 7412 370a 0673 6f75 7263  leCount.7..sourc
+00000a10: 6518 0c20 0128 0b32 1f2e 6b61 736b 6164  e.. .(.2..kaskad
+00000a20: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00000a30: 612e 536f 7572 6365 5206 736f 7572 6365  a.SourceR.source
+00000a40: 2273 0a11 4c69 7374 5461 626c 6573 5265  "s..ListTablesRe
+00000a50: 7175 6573 7412 160a 0673 6561 7263 6818  quest....search.
+00000a60: 0120 0128 0952 0673 6561 7263 6812 270a  . .(.R.search.'.
+00000a70: 0970 6167 655f 7369 7a65 1802 2001 2805  .page_size.. .(.
+00000a80: 420a fa42 071a 0518 e807 2800 5208 7061  B..B......(.R.pa
+00000a90: 6765 5369 7a65 121d 0a0a 7061 6765 5f74  geSize....page_t
+00000aa0: 6f6b 656e 1803 2001 2809 5209 7061 6765  oken.. .(.R.page
+00000ab0: 546f 6b65 6e22 c601 0a12 4c69 7374 5461  Token"....ListTa
+00000ac0: 626c 6573 5265 7370 6f6e 7365 1236 0a06  blesResponse.6..
+00000ad0: 7461 626c 6573 1801 2003 280b 321e 2e6b  tables.. .(.2..k
+00000ae0: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
+00000af0: 3161 6c70 6861 2e54 6162 6c65 5206 7461  1alpha.TableR.ta
+00000b00: 626c 6573 1226 0a0f 6e65 7874 5f70 6167  bles.&..next_pag
+00000b10: 655f 746f 6b65 6e18 0220 0128 0952 0d6e  e_token.. .(.R.n
+00000b20: 6578 7450 6167 6554 6f6b 656e 1250 0a0f  extPageToken.P..
+00000b30: 7265 7175 6573 745f 6465 7461 696c 7318  request_details.
+00000b40: 0320 0128 0b32 272e 6b61 736b 6164 612e  . .(.2'.kaskada.
+00000b50: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
+00000b60: 5265 7175 6573 7444 6574 6169 6c73 520e  RequestDetailsR.
+00000b70: 7265 7175 6573 7444 6574 6169 6c73 2239  requestDetails"9
+00000b80: 0a0f 4765 7454 6162 6c65 5265 7175 6573  ..GetTableReques
+00000b90: 7412 260a 0a74 6162 6c65 5f6e 616d 6518  t.&..table_name.
+00000ba0: 0120 0128 0942 07fa 4204 7202 1001 5209  . .(.B..B.r...R.
+00000bb0: 7461 626c 654e 616d 6522 9a01 0a10 4765  tableName"....Ge
+00000bc0: 7454 6162 6c65 5265 7370 6f6e 7365 1234  tTableResponse.4
+00000bd0: 0a05 7461 626c 6518 0120 0128 0b32 1e2e  ..table.. .(.2..
+00000be0: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000bf0: 7631 616c 7068 612e 5461 626c 6552 0574  v1alpha.TableR.t
+00000c00: 6162 6c65 1250 0a0f 7265 7175 6573 745f  able.P..request_
+00000c10: 6465 7461 696c 7318 0220 0128 0b32 272e  details.. .(.2'.
+00000c20: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000c30: 7631 616c 7068 612e 5265 7175 6573 7444  v1alpha.RequestD
+00000c40: 6574 6169 6c73 520e 7265 7175 6573 7444  etailsR.requestD
+00000c50: 6574 6169 6c73 2254 0a12 4372 6561 7465  etails"T..Create
+00000c60: 5461 626c 6552 6571 7565 7374 123e 0a05  TableRequest.>..
+00000c70: 7461 626c 6518 0120 0128 0b32 1e2e 6b61  table.. .(.2..ka
+00000c80: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
+00000c90: 616c 7068 612e 5461 626c 6542 08fa 4205  alpha.TableB..B.
+00000ca0: 8a01 0210 0152 0574 6162 6c65 229d 010a  .....R.table"...
+00000cb0: 1343 7265 6174 6554 6162 6c65 5265 7370  .CreateTableResp
+00000cc0: 6f6e 7365 1234 0a05 7461 626c 6518 0120  onse.4..table.. 
+00000cd0: 0128 0b32 1e2e 6b61 736b 6164 612e 6b61  .(.2..kaskada.ka
+00000ce0: 736b 6164 612e 7631 616c 7068 612e 5461  skada.v1alpha.Ta
+00000cf0: 626c 6552 0574 6162 6c65 1250 0a0f 7265  bleR.table.P..re
+00000d00: 7175 6573 745f 6465 7461 696c 7318 0220  quest_details.. 
+00000d10: 0128 0b32 272e 6b61 736b 6164 612e 6b61  .(.2'.kaskada.ka
+00000d20: 736b 6164 612e 7631 616c 7068 612e 5265  skada.v1alpha.Re
+00000d30: 7175 6573 7444 6574 6169 6c73 520e 7265  questDetailsR.re
+00000d40: 7175 6573 7444 6574 6169 6c73 2252 0a12  questDetails"R..
+00000d50: 4465 6c65 7465 5461 626c 6552 6571 7565  DeleteTableReque
+00000d60: 7374 1226 0a0a 7461 626c 655f 6e61 6d65  st.&..table_name
+00000d70: 1801 2001 2809 4207 fa42 0472 0210 0152  .. .(.B..B.r...R
+00000d80: 0974 6162 6c65 4e61 6d65 1214 0a05 666f  .tableName....fo
+00000d90: 7263 6518 0220 0128 0852 0566 6f72 6365  rce.. .(.R.force
+00000da0: 228b 010a 1344 656c 6574 6554 6162 6c65  "....DeleteTable
+00000db0: 5265 7370 6f6e 7365 1222 0a0d 6461 7461  Response."..data
+00000dc0: 5f74 6f6b 656e 5f69 6418 0120 0128 0952  _token_id.. .(.R
+00000dd0: 0b64 6174 6154 6f6b 656e 4964 1250 0a0f  .dataTokenId.P..
+00000de0: 7265 7175 6573 745f 6465 7461 696c 7318  request_details.
+00000df0: 0220 0128 0b32 272e 6b61 736b 6164 612e  . .(.2'.kaskada.
+00000e00: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
+00000e10: 5265 7175 6573 7444 6574 6169 6c73 520e  RequestDetailsR.
+00000e20: 7265 7175 6573 7444 6574 6169 6c73 2292  requestDetails".
+00000e30: 010a 0f4c 6f61 6444 6174 6152 6571 7565  ...LoadDataReque
+00000e40: 7374 1226 0a0a 7461 626c 655f 6e61 6d65  st.&..table_name
+00000e50: 1801 2001 2809 4207 fa42 0472 0210 0152  .. .(.B..B.r...R
+00000e60: 0974 6162 6c65 4e61 6d65 1243 0a0a 6669  .tableName.C..fi
+00000e70: 6c65 5f69 6e70 7574 1802 2001 280b 3222  le_input.. .(.2"
+00000e80: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00000e90: 2e76 3161 6c70 6861 2e46 696c 6549 6e70  .v1alpha.FileInp
+00000ea0: 7574 4800 5209 6669 6c65 496e 7075 7442  utH.R.fileInputB
+00000eb0: 120a 0b73 6f75 7263 655f 6461 7461 1203  ...source_data..
+00000ec0: f842 0122 8801 0a10 4c6f 6164 4461 7461  .B."....LoadData
+00000ed0: 5265 7370 6f6e 7365 1222 0a0d 6461 7461  Response."..data
+00000ee0: 5f74 6f6b 656e 5f69 6418 0120 0128 0952  _token_id.. .(.R
+00000ef0: 0b64 6174 6154 6f6b 656e 4964 1250 0a0f  .dataTokenId.P..
+00000f00: 7265 7175 6573 745f 6465 7461 696c 7318  request_details.
+00000f10: 0220 0128 0b32 272e 6b61 736b 6164 612e  . .(.2'.kaskada.
+00000f20: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
+00000f30: 5265 7175 6573 7444 6574 6169 6c73 520e  RequestDetailsR.
+00000f40: 7265 7175 6573 7444 6574 6169 6c73 32be  requestDetails2.
+00000f50: 050a 0c54 6162 6c65 5365 7276 6963 6512  ...TableService.
+00000f60: 7e0a 0a4c 6973 7454 6162 6c65 7312 2a2e  ~..ListTables.*.
+00000f70: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000f80: 7631 616c 7068 612e 4c69 7374 5461 626c  v1alpha.ListTabl
+00000f90: 6573 5265 7175 6573 741a 2b2e 6b61 736b  esRequest.+.kask
+00000fa0: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
+00000fb0: 7068 612e 4c69 7374 5461 626c 6573 5265  pha.ListTablesRe
+00000fc0: 7370 6f6e 7365 2217 82d3 e493 0211 120f  sponse".........
+00000fd0: 2f76 3161 6c70 6861 2f74 6162 6c65 7312  /v1alpha/tables.
+00000fe0: 8701 0a08 4765 7454 6162 6c65 1228 2e6b  ....GetTable.(.k
+00000ff0: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
+00001000: 3161 6c70 6861 2e47 6574 5461 626c 6552  1alpha.GetTableR
+00001010: 6571 7565 7374 1a29 2e6b 6173 6b61 6461  equest.).kaskada
+00001020: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00001030: 2e47 6574 5461 626c 6552 6573 706f 6e73  .GetTableRespons
+00001040: 6522 2682 d3e4 9302 2012 1e2f 7631 616c  e"&..... ../v1al
+00001050: 7068 612f 7461 626c 6573 2f7b 7461 626c  pha/tables/{tabl
+00001060: 655f 6e61 6d65 3d2a 7d12 8801 0a0b 4372  e_name=*}.....Cr
+00001070: 6561 7465 5461 626c 6512 2b2e 6b61 736b  eateTable.+.kask
+00001080: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
+00001090: 7068 612e 4372 6561 7465 5461 626c 6552  pha.CreateTableR
+000010a0: 6571 7565 7374 1a2c 2e6b 6173 6b61 6461  equest.,.kaskada
+000010b0: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+000010c0: 2e43 7265 6174 6554 6162 6c65 5265 7370  .CreateTableResp
+000010d0: 6f6e 7365 221e 82d3 e493 0218 3a05 7461  onse".......:.ta
+000010e0: 626c 6522 0f2f 7631 616c 7068 612f 7461  ble"./v1alpha/ta
+000010f0: 626c 6573 1290 010a 0b44 656c 6574 6554  bles.....DeleteT
+00001100: 6162 6c65 122b 2e6b 6173 6b61 6461 2e6b  able.+.kaskada.k
+00001110: 6173 6b61 6461 2e76 3161 6c70 6861 2e44  askada.v1alpha.D
+00001120: 656c 6574 6554 6162 6c65 5265 7175 6573  eleteTableReques
+00001130: 741a 2c2e 6b61 736b 6164 612e 6b61 736b  t.,.kaskada.kask
+00001140: 6164 612e 7631 616c 7068 612e 4465 6c65  ada.v1alpha.Dele
+00001150: 7465 5461 626c 6552 6573 706f 6e73 6522  teTableResponse"
+00001160: 2682 d3e4 9302 202a 1e2f 7631 616c 7068  &..... *./v1alph
+00001170: 612f 7461 626c 6573 2f7b 7461 626c 655f  a/tables/{table_
+00001180: 6e61 6d65 3d2a 7d12 8501 0a08 4c6f 6164  name=*}.....Load
+00001190: 4461 7461 1228 2e6b 6173 6b61 6461 2e6b  Data.(.kaskada.k
+000011a0: 6173 6b61 6461 2e76 3161 6c70 6861 2e4c  askada.v1alpha.L
+000011b0: 6f61 6444 6174 6152 6571 7565 7374 1a29  oadDataRequest.)
+000011c0: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+000011d0: 2e76 3161 6c70 6861 2e4c 6f61 6444 6174  .v1alpha.LoadDat
+000011e0: 6152 6573 706f 6e73 6522 2482 d3e4 9302  aResponse"$.....
+000011f0: 1e3a 012a 2219 2f76 3161 6c70 6861 2f74  .:.*"./v1alpha/t
+00001200: 6162 6c65 732f 6c6f 6164 5f64 6174 6142  ables/load_dataB
+00001210: 8102 0a1b 636f 6d2e 6b61 736b 6164 612e  ....com.kaskada.
+00001220: 6b61 736b 6164 612e 7631 616c 7068 6142  kaskada.v1alphaB
+00001230: 1154 6162 6c65 5365 7276 6963 6550 726f  .TableServicePro
+00001240: 746f 5001 5a51 6769 7468 7562 2e63 6f6d  toP.ZQgithub.com
+00001250: 2f6b 6173 6b61 6461 2d61 692f 6b61 736b  /kaskada-ai/kask
+00001260: 6164 612f 6765 6e2f 7072 6f74 6f2f 676f  ada/gen/proto/go
+00001270: 2f6b 6173 6b61 6461 2f6b 6173 6b61 6461  /kaskada/kaskada
+00001280: 2f76 3161 6c70 6861 3b6b 6173 6b61 6461  /v1alpha;kaskada
+00001290: 7631 616c 7068 61a2 0203 4b4b 58aa 0217  v1alpha...KKX...
+000012a0: 4b61 736b 6164 612e 4b61 736b 6164 612e  Kaskada.Kaskada.
+000012b0: 5631 616c 7068 61ca 0217 4b61 736b 6164  V1alpha...Kaskad
+000012c0: 615c 4b61 736b 6164 615c 5631 616c 7068  a\Kaskada\V1alph
+000012d0: 61e2 0223 4b61 736b 6164 615c 4b61 736b  a..#Kaskada\Kask
+000012e0: 6164 615c 5631 616c 7068 615c 4750 424d  ada\V1alpha\GPBM
+000012f0: 6574 6164 6174 61ea 0219 4b61 736b 6164  etadata...Kaskad
+00001300: 613a 3a4b 6173 6b61 6461 3a3a 5631 616c  a::Kaskada::V1al
+00001310: 7068 6162 0670 726f 746f 33da 0554 6162  phab.proto3..Tab
+00001320: 6c65 da11 4c69 7374 5461 626c 6573 5265  le..ListTablesRe
+00001330: 7175 6573 74da 124c 6973 7454 6162 6c65  quest..ListTable
+00001340: 7352 6573 706f 6e73 65da 0f47 6574 5461  sResponse..GetTa
+00001350: 626c 6552 6571 7565 7374 da10 4765 7454  bleRequest..GetT
+00001360: 6162 6c65 5265 7370 6f6e 7365 da12 4372  ableResponse..Cr
+00001370: 6561 7465 5461 626c 6552 6571 7565 7374  eateTableRequest
+00001380: da13 4372 6561 7465 5461 626c 6552 6573  ..CreateTableRes
+00001390: 706f 6e73 65da 1244 656c 6574 6554 6162  ponse..DeleteTab
+000013a0: 6c65 5265 7175 6573 74da 1344 656c 6574  leRequest..Delet
+000013b0: 6554 6162 6c65 5265 7370 6f6e 7365 da0f  eTableResponse..
+000013c0: 4c6f 6164 4461 7461 5265 7175 6573 74da  LoadDataRequest.
+000013d0: 104c 6f61 6444 6174 6152 6573 706f 6e73  .LoadDataRespons
+000013e0: 657a 296b 6173 6b61 6461 2e6b 6173 6b61  ez)kaskada.kaska
+000013f0: 6461 2e76 3161 6c70 6861 2e74 6162 6c65  da.v1alpha.table
+00001400: 5f73 6572 7669 6365 5f70 6232 2902 da0a  _service_pb2)...
+00001410: 4445 5343 5249 5054 4f52 da0a 5f5f 6d6f  DESCRIPTOR..__mo
+00001420: 6475 6c65 5f5f 5a0c 5461 626c 6553 6572  dule__Z.TableSer
+00001430: 7669 6365 464e 7301 0100 000a 1b63 6f6d  viceFNs......com
+00001440: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00001450: 2e76 3161 6c70 6861 4211 5461 626c 6553  .v1alphaB.TableS
+00001460: 6572 7669 6365 5072 6f74 6f50 015a 5167  erviceProtoP.ZQg
+00001470: 6974 6875 622e 636f 6d2f 6b61 736b 6164  ithub.com/kaskad
+00001480: 612d 6169 2f6b 6173 6b61 6461 2f67 656e  a-ai/kaskada/gen
+00001490: 2f70 726f 746f 2f67 6f2f 6b61 736b 6164  /proto/go/kaskad
+000014a0: 612f 6b61 736b 6164 612f 7631 616c 7068  a/kaskada/v1alph
+000014b0: 613b 6b61 736b 6164 6176 3161 6c70 6861  a;kaskadav1alpha
+000014c0: a202 034b 4b58 aa02 174b 6173 6b61 6461  ...KKX...Kaskada
+000014d0: 2e4b 6173 6b61 6461 2e56 3161 6c70 6861  .Kaskada.V1alpha
+000014e0: ca02 174b 6173 6b61 6461 5c4b 6173 6b61  ...Kaskada\Kaska
+000014f0: 6461 5c56 3161 6c70 6861 e202 234b 6173  da\V1alpha..#Kas
+00001500: 6b61 6461 5c4b 6173 6b61 6461 5c56 3161  kada\Kaskada\V1a
+00001510: 6c70 6861 5c47 5042 4d65 7461 6461 7461  lpha\GPBMetadata
+00001520: ea02 194b 6173 6b61 6461 3a3a 4b61 736b  ...Kaskada::Kask
+00001530: 6164 613a 3a56 3161 6c70 6861 da08 7461  ada::V1alpha..ta
+00001540: 626c 655f 6964 7303 0000 00e0 4103 da0a  ble_ids.....A...
+00001550: 7461 626c 655f 6e61 6d65 7307 0000 00fa  table_names.....
+00001560: 4204 7202 1001 da10 7469 6d65 5f63 6f6c  B.r.....time_col
+00001570: 756d 6e5f 6e61 6d65 da16 656e 7469 7479  umn_name..entity
+00001580: 5f6b 6579 5f63 6f6c 756d 6e5f 6e61 6d65  _key_column_name
+00001590: da13 7375 6273 6f72 745f 636f 6c75 6d6e  ..subsort_column
+000015a0: 5f6e 616d 65da 0b63 7265 6174 655f 7469  _name..create_ti
+000015b0: 6d65 da0b 7570 6461 7465 5f74 696d 65da  me..update_time.
+000015c0: 0776 6572 7369 6f6e da06 7363 6865 6d61  .version..schema
+000015d0: 5a0a 6669 6c65 5f63 6f75 6e74 5a09 7061  Z.file_countZ.pa
+000015e0: 6765 5f73 697a 6573 0a00 0000 fa42 071a  ge_sizes.....B..
+000015f0: 0518 e807 2800 da05 7461 626c 6573 0800  ....(...tables..
+00001600: 0000 fa42 058a 0102 1001 5a0b 736f 7572  ...B......Z.sour
+00001610: 6365 5f64 6174 6173 0300 0000 f842 015a  ce_datas.....B.Z
+00001620: 0a4c 6973 7454 6162 6c65 7373 1700 0000  .ListTabless....
+00001630: 82d3 e493 0211 120f 2f76 3161 6c70 6861  ......../v1alpha
+00001640: 2f74 6162 6c65 735a 0847 6574 5461 626c  /tablesZ.GetTabl
+00001650: 6573 2600 0000 82d3 e493 0220 121e 2f76  es&........ ../v
+00001660: 3161 6c70 6861 2f74 6162 6c65 732f 7b74  1alpha/tables/{t
+00001670: 6162 6c65 5f6e 616d 653d 2a7d da0b 4372  able_name=*}..Cr
+00001680: 6561 7465 5461 626c 6573 1e00 0000 82d3  eateTables......
+00001690: e493 0218 3a05 7461 626c 6522 0f2f 7631  ....:.table"./v1
+000016a0: 616c 7068 612f 7461 626c 6573 5a0b 4465  alpha/tablesZ.De
+000016b0: 6c65 7465 5461 626c 6573 2600 0000 82d3  leteTables&.....
+000016c0: e493 0220 2a1e 2f76 3161 6c70 6861 2f74  ... *./v1alpha/t
+000016d0: 6162 6c65 732f 7b74 6162 6c65 5f6e 616d  ables/{table_nam
+000016e0: 653d 2a7d 5a08 4c6f 6164 4461 7461 7324  e=*}Z.LoadDatas$
+000016f0: 0000 0082 d3e4 9302 1e3a 012a 2219 2f76  .........:.*"./v
+00001700: 3161 6c70 6861 2f74 6162 6c65 732f 6c6f  1alpha/tables/lo
+00001710: 6164 5f64 6174 6169 5501 0000 69cb 0300  ad_dataiU...i...
+00001720: 0069 cd03 0000 6940 0400 0069 4304 0000  .i....i@...iC...
+00001730: 6909 0500 0069 0b05 0000 6944 0500 0069  i....i....iD...i
+00001740: 4705 0000 69e1 0500 0069 e305 0000 6937  G...i....i....i7
+00001750: 0600 0069 3a06 0000 69d7 0600 0069 d906  ...i:...i....i..
+00001760: 0000 692b 0700 0069 2e07 0000 69b9 0700  ..i+...i....i...
+00001770: 0069 bc07 0000 694e 0800 0069 5108 0000  .i....iN...iQ...
+00001780: 69d9 0800 0069 dc08 0000 699a 0b00 0029  i....i....i....)
+00001790: 47da 075f 5f64 6f63 5f5f da0f 676f 6f67  G..__doc__..goog
+000017a0: 6c65 2e70 726f 746f 6275 6672 0200 0000  le.protobufr....
+000017b0: da0b 5f64 6573 6372 6970 746f 7272 0300  .._descriptorr..
+000017c0: 0000 da10 5f64 6573 6372 6970 746f 725f  ...._descriptor_
+000017d0: 706f 6f6c 7204 0000 00da 085f 6d65 7373  poolr......_mess
+000017e0: 6167 6572 0500 0000 da0b 5f72 6566 6c65  ager......_refle
+000017f0: 6374 696f 6e72 0600 0000 da10 5f73 796d  ctionr......_sym
+00001800: 626f 6c5f 6461 7461 6261 7365 da07 4465  bol_database..De
+00001810: 6661 756c 74da 075f 7379 6d5f 6462 5a0a  fault.._sym_dbZ.
+00001820: 676f 6f67 6c65 2e61 7069 7207 0000 005a  google.apir....Z
+00001830: 2367 6f6f 676c 655f 646f 745f 6170 695f  #google_dot_api_
+00001840: 646f 745f 616e 6e6f 7461 7469 6f6e 735f  dot_annotations_
+00001850: 5f70 6232 7208 0000 005a 2767 6f6f 676c  _pb2r....Z'googl
+00001860: 655f 646f 745f 6170 695f 646f 745f 6669  e_dot_api_dot_fi
+00001870: 656c 645f 5f62 6568 6176 696f 725f 5f70  eld__behavior__p
+00001880: 6232 7209 0000 00da 2667 6f6f 676c 655f  b2r.....&google_
+00001890: 646f 745f 7072 6f74 6f62 7566 5f64 6f74  dot_protobuf_dot
+000018a0: 5f74 696d 6573 7461 6d70 5f5f 7062 3272  _timestamp__pb2r
+000018b0: 0a00 0000 5a25 676f 6f67 6c65 5f64 6f74  ....Z%google_dot
+000018c0: 5f70 726f 746f 6275 665f 646f 745f 7772  _protobuf_dot_wr
+000018d0: 6170 7065 7273 5f5f 7062 32da 176b 6173  appers__pb2..kas
+000018e0: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
+000018f0: 6c70 6861 720b 0000 005a 2f6b 6173 6b61  lphar....Z/kaska
+00001900: 6461 5f64 6f74 5f6b 6173 6b61 6461 5f64  da_dot_kaskada_d
+00001910: 6f74 5f76 3161 6c70 6861 5f64 6f74 5f63  ot_v1alpha_dot_c
+00001920: 6f6d 6d6f 6e5f 5f70 6232 720c 0000 005a  ommon__pb2r....Z
+00001930: 2f6b 6173 6b61 6461 5f64 6f74 5f6b 6173  /kaskada_dot_kas
+00001940: 6b61 6461 5f64 6f74 5f76 3161 6c70 6861  kada_dot_v1alpha
+00001950: 5f64 6f74 5f73 6368 656d 615f 5f70 6232  _dot_schema__pb2
+00001960: 720d 0000 005a 306b 6173 6b61 6461 5f64  r....Z0kaskada_d
+00001970: 6f74 5f6b 6173 6b61 6461 5f64 6f74 5f76  ot_kaskada_dot_v
+00001980: 3161 6c70 6861 5f64 6f74 5f73 6f75 7263  1alpha_dot_sourc
+00001990: 6573 5f5f 7062 32da 0876 616c 6964 6174  es__pb2..validat
+000019a0: 6572 0e00 0000 5a1a 7661 6c69 6461 7465  er....Z.validate
+000019b0: 5f64 6f74 5f76 616c 6964 6174 655f 5f70  _dot_validate__p
+000019c0: 6232 da11 4164 6453 6572 6961 6c69 7a65  b2..AddSerialize
+000019d0: 6446 696c 6572 1a00 0000 da15 6d65 7373  dFiler......mess
+000019e0: 6167 655f 7479 7065 735f 6279 5f6e 616d  age_types_by_nam
+000019f0: 655a 065f 5441 424c 455a 125f 4c49 5354  eZ._TABLEZ._LIST
+00001a00: 5441 424c 4553 5245 5155 4553 545a 135f  TABLESREQUESTZ._
+00001a10: 4c49 5354 5441 424c 4553 5245 5350 4f4e  LISTTABLESRESPON
+00001a20: 5345 5a10 5f47 4554 5441 424c 4552 4551  SEZ._GETTABLEREQ
+00001a30: 5545 5354 5a11 5f47 4554 5441 424c 4552  UESTZ._GETTABLER
+00001a40: 4553 504f 4e53 455a 135f 4352 4541 5445  ESPONSEZ._CREATE
+00001a50: 5441 424c 4552 4551 5545 5354 5a14 5f43  TABLEREQUESTZ._C
+00001a60: 5245 4154 4554 4142 4c45 5245 5350 4f4e  REATETABLERESPON
+00001a70: 5345 5a13 5f44 454c 4554 4554 4142 4c45  SEZ._DELETETABLE
+00001a80: 5245 5155 4553 545a 145f 4445 4c45 5445  REQUESTZ._DELETE
+00001a90: 5441 424c 4552 4553 504f 4e53 455a 105f  TABLERESPONSEZ._
+00001aa0: 4c4f 4144 4441 5441 5245 5155 4553 545a  LOADDATAREQUESTZ
+00001ab0: 115f 4c4f 4144 4441 5441 5245 5350 4f4e  ._LOADDATARESPON
+00001ac0: 5345 da1c 4765 6e65 7261 7465 6450 726f  SE..GeneratedPro
+00001ad0: 746f 636f 6c4d 6573 7361 6765 5479 7065  tocolMessageType
+00001ae0: da07 4d65 7373 6167 6572 0f00 0000 da0f  ..Messager......
+00001af0: 5265 6769 7374 6572 4d65 7373 6167 6572  RegisterMessager
+00001b00: 1000 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
+00001b10: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
+00001b20: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00001b30: 00da 1073 6572 7669 6365 735f 6279 5f6e  ...services_by_n
+00001b40: 616d 655a 0d5f 5441 424c 4553 4552 5649  ameZ._TABLESERVI
+00001b50: 4345 da12 5f55 5345 5f43 5f44 4553 4352  CE.._USE_C_DESCR
+00001b60: 4950 544f 5253 da08 5f6f 7074 696f 6e73  IPTORS.._options
+00001b70: da13 5f73 6572 6961 6c69 7a65 645f 6f70  .._serialized_op
+00001b80: 7469 6f6e 73da 0e66 6965 6c64 735f 6279  tions..fields_by
+00001b90: 5f6e 616d 65da 0e6f 6e65 6f66 735f 6279  _name..oneofs_by
+00001ba0: 5f6e 616d 65da 0f6d 6574 686f 6473 5f62  _name..methods_b
+00001bb0: 795f 6e61 6d65 da11 5f73 6572 6961 6c69  y_name.._seriali
+00001bc0: 7a65 645f 7374 6172 74da 0f5f 7365 7269  zed_start.._seri
+00001bd0: 616c 697a 6564 5f65 6e64 a900 7241 0000  alized_end..rA..
+00001be0: 0072 4100 0000 fa35 2f73 7263 2f73 7263  .rA....5/src/src
+00001bf0: 2f6b 6173 6b61 6461 2f6b 6173 6b61 6461  /kaskada/kaskada
+00001c00: 2f76 3161 6c70 6861 2f74 6162 6c65 5f73  /v1alpha/table_s
+00001c10: 6572 7669 6365 5f70 6232 2e70 79da 083c  ervice_pb2.py..<
+00001c20: 6d6f 6475 6c65 3e04 0000 0073 2e01 0000  module>....s....
+00001c30: 0401 0c01 0c01 0c01 0c01 0c03 0803 0c01  ................
+00001c40: 0c01 0c01 0c01 0c01 0c01 0c01 0c03 0e04  ................
+00001c50: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00001c60: 0a01 0a01 0a01 0c01 0201 02fe 0805 0a02  ................
+00001c70: 0c01 0201 02fe 0805 0a02 0c01 0201 02fe  ................
+00001c80: 0805 0a02 0c01 0201 02fe 0805 0a02 0c01  ................
+00001c90: 0201 02fe 0805 0a02 0c01 0201 02fe 0805  ................
+00001ca0: 0a02 0c01 0201 02fe 0805 0a02 0c01 0201  ................
+00001cb0: 02fe 0805 0a02 0c01 0201 02fe 0805 0a02  ................
+00001cc0: 0c01 0201 02fe 0805 0a02 0c01 0201 02fe  ................
+00001cd0: 0805 0a02 0a01 0c02 0601 0601 0c01 0c01  ................
+00001ce0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00001cf0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00001d00: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00001d10: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00001d20: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00001d30: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+00001d40: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+00001d50: 0601 0601 0601 0601 0601 0601 0601       ..............
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/table_service_pb2_grpc.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/table_service_pb2_grpc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 10053 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 4527 0000  o.........5dE'..
+00000000: 610d 0d0a 0000 0000 2038 4164 4527 0000  a....... 8AdE'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a04 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000050: 6505 8303 5a06 4700 6406 6407 8400 6407  e...Z.G.d.d...d.
 00000060: 6505 8303 5a07 6408 6409 8400 5a08 4700  e...Z.d.d...Z.G.
 00000070: 640a 640b 8400 640b 6505 8303 5a09 6402  d.d...d.e...Z.d.
@@ -72,239 +72,258 @@
 00000470: 6554 6162 6c65 5265 7175 6573 74da 1344  eTableRequest..D
 00000480: 656c 6574 6554 6162 6c65 5265 7370 6f6e  eleteTableRespon
 00000490: 7365 da0b 4465 6c65 7465 5461 626c 65da  se..DeleteTable.
 000004a0: 0f4c 6f61 6444 6174 6152 6571 7565 7374  .LoadDataRequest
 000004b0: da10 4c6f 6164 4461 7461 5265 7370 6f6e  ..LoadDataRespon
 000004c0: 7365 da08 4c6f 6164 4461 7461 2902 da04  se..LoadData)...
 000004d0: 7365 6c66 da07 6368 616e 6e65 6ca9 0072  self..channel..r
-000004e0: 2100 0000 fa7c 2f68 6f6d 652f 7468 6572  !....|/home/ther
-000004f0: 6170 6f6e 2f52 6570 6f73 2f47 6974 4875  apon/Repos/GitHu
-00000500: 622f 4b61 736b 6164 6141 492f 6b61 736b  b/KaskadaAI/kask
-00000510: 6164 612f 7265 6c65 6173 696e 672f 636c  ada/releasing/cl
-00000520: 6965 6e74 732f 7079 7468 6f6e 2f73 7263  ients/python/src
-00000530: 2f6b 6173 6b61 6461 2f6b 6173 6b61 6461  /kaskada/kaskada
-00000540: 2f76 3161 6c70 6861 2f74 6162 6c65 5f73  /v1alpha/table_s
-00000550: 6572 7669 6365 5f70 6232 5f67 7270 632e  ervice_pb2_grpc.
-00000560: 7079 da08 5f5f 696e 6974 5f5f 0c00 0000  py..__init__....
-00000570: 7332 0000 0004 0602 0106 0106 0108 fd04  s2..............
-00000580: 0502 0106 0106 0108 fd04 0502 0106 0106  ................
-00000590: 0108 fd04 0502 0106 0106 0108 fd04 0502  ................
-000005a0: 0106 0106 010c fd7a 1954 6162 6c65 5365  .......z.TableSe
-000005b0: 7276 6963 6553 7475 622e 5f5f 696e 6974  rviceStub.__init
-000005c0: 5f5f 4e29 05da 085f 5f6e 616d 655f 5fda  __N)...__name__.
-000005d0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000005e0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
-000005f0: 5f5f 7223 0000 0072 2100 0000 7221 0000  __r#...r!...r!..
-00000600: 0072 2100 0000 7222 0000 0072 0300 0000  .r!...r"...r....
-00000610: 0800 0000 7306 0000 0008 0004 010c 0372  ....s..........r
-00000620: 0300 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000630: 0000 0000 0002 0000 0040 0000 0073 3800  .........@...s8.
-00000640: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00000650: 6403 8400 5a04 6404 6405 8400 5a05 6406  d...Z.d.d...Z.d.
-00000660: 6407 8400 5a06 6408 6409 8400 5a07 640a  d...Z.d.d...Z.d.
-00000670: 640b 8400 5a08 640c 5300 290d da14 5461  d...Z.d.S.)...Ta
-00000680: 626c 6553 6572 7669 6365 5365 7276 6963  bleServiceServic
-00000690: 6572 7204 0000 0063 0300 0000 0000 0000  err....c........
-000006a0: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
-000006b0: f320 0000 007c 02a0 0074 016a 026a 03a1  . ...|...t.j.j..
-000006c0: 0101 007c 02a0 0464 01a1 0101 0074 0564  ...|...d.....t.d
-000006d0: 0183 0182 0129 027a c64c 6973 7473 2074  .....).z.Lists t
-000006e0: 6162 6c65 732e 0a0a 2020 2020 2020 2020  ables...        
-000006f0: 5468 6520 7265 7370 6f6e 7365 2069 6e63  The response inc
-00000700: 6c75 6465 7320 616c 6c20 5461 626c 6573  ludes all Tables
-00000710: 2064 6566 696e 6564 2066 6f72 2074 6865   defined for the
-00000720: 204b 6173 6b61 6461 2061 6363 6f75 6e74   Kaskada account
-00000730: 2e0a 2020 2020 2020 2020 4966 2061 2073  ..        If a s
-00000740: 6561 7263 6820 7374 7269 6e67 2069 7320  earch string is 
-00000750: 7072 6f76 6964 6564 2c20 6f6e 6c79 2054  provided, only T
-00000760: 6162 6c65 7320 6d61 7463 6869 6e67 2074  ables matching t
-00000770: 6865 2073 6561 7263 680a 2020 2020 2020  he search.      
-00000780: 2020 7374 7269 6e67 2061 7265 2072 6574    string are ret
-00000790: 7572 6e65 642e 0a20 2020 2020 2020 20fa  urned..        .
-000007a0: 174d 6574 686f 6420 6e6f 7420 696d 706c  .Method not impl
-000007b0: 656d 656e 7465 6421 a906 da08 7365 745f  emented!....set_
-000007c0: 636f 6465 da04 6772 7063 da0a 5374 6174  code..grpc..Stat
-000007d0: 7573 436f 6465 da0d 554e 494d 504c 454d  usCode..UNIMPLEM
-000007e0: 454e 5445 44da 0b73 6574 5f64 6574 6169  ENTED..set_detai
-000007f0: 6c73 da13 4e6f 7449 6d70 6c65 6d65 6e74  ls..NotImplement
-00000800: 6564 4572 726f 72a9 0372 1f00 0000 da07  edError..r......
-00000810: 7265 7175 6573 74da 0763 6f6e 7465 7874  request..context
-00000820: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00000830: 1200 0000 3100 0000 7306 0000 000e 070a  ....1...s.......
-00000840: 0108 017a 1f54 6162 6c65 5365 7276 6963  ...z.TableServic
-00000850: 6553 6572 7669 6365 722e 4c69 7374 5461  eServicer.ListTa
-00000860: 626c 6573 6303 0000 0000 0000 0000 0000  blesc...........
-00000870: 0003 0000 0003 0000 0043 0000 0072 2900  .........C...r).
-00000880: 0000 2902 7a16 4765 7473 2061 2074 6162  ..).z.Gets a tab
-00000890: 6c65 2e0a 2020 2020 2020 2020 722a 0000  le..        r*..
-000008a0: 0072 2b00 0000 7232 0000 0072 2100 0000  .r+...r2...r!...
-000008b0: 7221 0000 0072 2200 0000 7215 0000 003c  r!...r"...r....<
-000008c0: 0000 00f3 0600 0000 0e03 0a01 0801 7a1d  ..............z.
-000008d0: 5461 626c 6553 6572 7669 6365 5365 7276  TableServiceServ
-000008e0: 6963 6572 2e47 6574 5461 626c 6563 0300  icer.GetTablec..
-000008f0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00000900: 0000 4300 0000 7229 0000 0029 027a 1943  ..C...r)...).z.C
-00000910: 7265 6174 6573 2061 2074 6162 6c65 2e0a  reates a table..
-00000920: 2020 2020 2020 2020 722a 0000 0072 2b00          r*...r+.
-00000930: 0000 7232 0000 0072 2100 0000 7221 0000  ..r2...r!...r!..
-00000940: 0072 2200 0000 7218 0000 0043 0000 0072  .r"...r....C...r
-00000950: 3500 0000 7a20 5461 626c 6553 6572 7669  5...z TableServi
-00000960: 6365 5365 7276 6963 6572 2e43 7265 6174  ceServicer.Creat
-00000970: 6554 6162 6c65 6303 0000 0000 0000 0000  eTablec.........
-00000980: 0000 0003 0000 0003 0000 0043 0000 0072  ...........C...r
-00000990: 2900 0000 2902 7a37 4465 6c65 7465 7320  )...).z7Deletes 
-000009a0: 6120 7461 626c 6520 616e 6420 616e 7920  a table and any 
-000009b0: 6576 656e 7473 206c 6f61 6465 6420 696e  events loaded in
-000009c0: 746f 2069 742e 0a20 2020 2020 2020 2072  to it..        r
-000009d0: 2a00 0000 722b 0000 0072 3200 0000 7221  *...r+...r2...r!
-000009e0: 0000 0072 2100 0000 7222 0000 0072 1b00  ...r!...r"...r..
-000009f0: 0000 4a00 0000 7235 0000 007a 2054 6162  ..J...r5...z Tab
-00000a00: 6c65 5365 7276 6963 6553 6572 7669 6365  leServiceService
-00000a10: 722e 4465 6c65 7465 5461 626c 6563 0300  r.DeleteTablec..
-00000a20: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00000a30: 0000 4300 0000 7229 0000 0029 027a 294c  ..C...r)...).z)L
-00000a40: 6f61 6473 2061 2073 7461 6765 6420 6669  oads a staged fi
-00000a50: 6c65 2069 6e74 6f20 6120 7461 626c 650a  le into a table.
-00000a60: 2020 2020 2020 2020 722a 0000 0072 2b00          r*...r+.
-00000a70: 0000 7232 0000 0072 2100 0000 7221 0000  ..r2...r!...r!..
-00000a80: 0072 2200 0000 721e 0000 0051 0000 0072  .r"...r....Q...r
-00000a90: 3500 0000 7a1d 5461 626c 6553 6572 7669  5...z.TableServi
-00000aa0: 6365 5365 7276 6963 6572 2e4c 6f61 6444  ceServicer.LoadD
-00000ab0: 6174 614e 2909 7224 0000 0072 2500 0000  ataN).r$...r%...
-00000ac0: 7226 0000 0072 2700 0000 7212 0000 0072  r&...r'...r....r
-00000ad0: 1500 0000 7218 0000 0072 1b00 0000 721e  ....r....r....r.
-00000ae0: 0000 0072 2100 0000 7221 0000 0072 2100  ...r!...r!...r!.
-00000af0: 0000 7222 0000 0072 2800 0000 2d00 0000  ..r"...r(...-...
-00000b00: 730e 0000 0008 0004 0108 0308 0b08 0708  s...............
-00000b10: 070c 0772 2800 0000 6302 0000 0000 0000  ...r(...c.......
-00000b20: 0000 0000 0004 0000 0009 0000 0043 0000  .............C..
-00000b30: 0073 9a00 0000 7400 6a01 7c00 6a02 7403  .s....t.j.|.j.t.
-00000b40: 6a04 6a05 7403 6a06 6a07 6401 8d03 7400  j.j.t.j.j.d...t.
-00000b50: 6a01 7c00 6a08 7403 6a09 6a05 7403 6a0a  j.|.j.t.j.j.t.j.
-00000b60: 6a07 6401 8d03 7400 6a01 7c00 6a0b 7403  j.d...t.j.|.j.t.
-00000b70: 6a0c 6a05 7403 6a0d 6a07 6401 8d03 7400  j.j.t.j.j.d...t.
-00000b80: 6a01 7c00 6a0e 7403 6a0f 6a05 7403 6a10  j.|.j.t.j.j.t.j.
-00000b90: 6a07 6401 8d03 7400 6a01 7c00 6a11 7403  j.d...t.j.|.j.t.
-00000ba0: 6a12 6a05 7403 6a13 6a07 6401 8d03 6402  j.j.t.j.j.d...d.
-00000bb0: 9c05 7d02 7400 a014 6403 7c02 a102 7d03  ..}.t...d.|...}.
-00000bc0: 7c01 a015 7c03 6601 a101 0100 6400 5300  |...|.f.....d.S.
-00000bd0: 2904 4e29 02da 1472 6571 7565 7374 5f64  ).N)...request_d
-00000be0: 6573 6572 6961 6c69 7a65 72da 1372 6573  eserializer..res
-00000bf0: 706f 6e73 655f 7365 7269 616c 697a 6572  ponse_serializer
-00000c00: 2905 7212 0000 0072 1500 0000 7218 0000  ).r....r....r...
-00000c10: 0072 1b00 0000 721e 0000 007a 246b 6173  .r....r....z$kas
-00000c20: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-00000c30: 6c70 6861 2e54 6162 6c65 5365 7276 6963  lpha.TableServic
-00000c40: 6529 1672 2d00 0000 da1e 756e 6172 795f  e).r-.....unary_
-00000c50: 756e 6172 795f 7270 635f 6d65 7468 6f64  unary_rpc_method
-00000c60: 5f68 616e 646c 6572 7212 0000 0072 0d00  _handlerr....r..
-00000c70: 0000 720e 0000 0072 1100 0000 7210 0000  ..r....r....r...
-00000c80: 0072 0f00 0000 7215 0000 0072 1300 0000  .r....r....r....
-00000c90: 7214 0000 0072 1800 0000 7216 0000 0072  r....r....r....r
-00000ca0: 1700 0000 721b 0000 0072 1900 0000 721a  ....r....r....r.
-00000cb0: 0000 0072 1e00 0000 721c 0000 0072 1d00  ...r....r....r..
-00000cc0: 0000 da1f 6d65 7468 6f64 5f68 616e 646c  ....method_handl
-00000cd0: 6572 735f 6765 6e65 7269 635f 6861 6e64  ers_generic_hand
-00000ce0: 6c65 72da 1861 6464 5f67 656e 6572 6963  ler..add_generic
-00000cf0: 5f72 7063 5f68 616e 646c 6572 7329 04da  _rpc_handlers)..
-00000d00: 0873 6572 7669 6365 72da 0673 6572 7665  .servicer..serve
-00000d10: 72da 1372 7063 5f6d 6574 686f 645f 6861  r..rpc_method_ha
-00000d20: 6e64 6c65 7273 da0f 6765 6e65 7269 635f  ndlers..generic_
-00000d30: 6861 6e64 6c65 7272 2100 0000 7221 0000  handlerr!...r!..
-00000d40: 0072 2200 0000 da22 6164 645f 5461 626c  .r"...."add_Tabl
-00000d50: 6553 6572 7669 6365 5365 7276 6963 6572  eServiceServicer
-00000d60: 5f74 6f5f 7365 7276 6572 5900 0000 733c  _to_serverY...s<
-00000d70: 0000 0004 0204 0106 0106 0104 fd04 0504  ................
-00000d80: 0106 0106 0104 fd04 0504 0106 0106 0104  ................
-00000d90: fd04 0504 0106 0106 0104 fd04 0504 0106  ................
-00000da0: 0106 0104 fd06 eb04 1b04 0104 ff10 0272  ...............r
-00000db0: 3f00 0000 6300 0000 0000 0000 0000 0000  ?...c...........
-00000dc0: 0000 0000 0004 0000 0040 0000 0073 a600  .........@...s..
-00000dd0: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
-00000de0: 0902 0903 0903 0904 0903 0903 0903 0903  ................
-00000df0: 640f 6405 6406 8401 8301 5a05 6504 0902  d.d.d.....Z.e...
-00000e00: 0903 0903 0904 0903 0903 0903 0903 640f  ..............d.
-00000e10: 6407 6408 8401 8301 5a06 6504 0902 0903  d.d.....Z.e.....
-00000e20: 0903 0904 0903 0903 0903 0903 640f 6409  ............d.d.
-00000e30: 640a 8401 8301 5a07 6504 0902 0903 0903  d.....Z.e.......
-00000e40: 0904 0903 0903 0903 0903 640f 640b 640c  ..........d.d.d.
-00000e50: 8401 8301 5a08 6504 0902 0903 0903 0904  ....Z.e.........
-00000e60: 0903 0903 0903 0903 640f 640d 640e 8401  ........d.d.d...
-00000e70: 8301 5a09 6403 5300 2910 da0c 5461 626c  ..Z.d.S.)...Tabl
-00000e80: 6553 6572 7669 6365 7204 0000 0072 2100  eServicer....r!.
-00000e90: 0000 4e46 630a 0000 0000 0000 0000 0000  ..NFc...........
-00000ea0: 000a 0000 000f 0000 0043 0000 00f3 2c00  .........C....,.
-00000eb0: 0000 7400 6a01 a002 7c00 7c01 6401 7403  ..t.j...|.|.d.t.
-00000ec0: 6a04 6a05 7403 6a06 6a07 7c02 7c03 7c05  j.j.t.j.j.|.|.|.
-00000ed0: 7c04 7c06 7c07 7c08 7c09 a10d 5300 2902  |.|.|.|.|...S.).
-00000ee0: 4e72 0500 0000 2908 722d 0000 00da 0c65  Nr....).r-.....e
-00000ef0: 7870 6572 696d 656e 7461 6c72 0c00 0000  xperimentalr....
-00000f00: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-00000f10: 1000 0000 7211 0000 00a9 0a72 3300 0000  ....r......r3...
-00000f20: da06 7461 7267 6574 da07 6f70 7469 6f6e  ..target..option
-00000f30: 73da 1363 6861 6e6e 656c 5f63 7265 6465  s..channel_crede
-00000f40: 6e74 6961 6c73 da10 6361 6c6c 5f63 7265  ntials..call_cre
-00000f50: 6465 6e74 6961 6c73 da08 696e 7365 6375  dentials..insecu
-00000f60: 7265 da0b 636f 6d70 7265 7373 696f 6eda  re..compression.
-00000f70: 0e77 6169 745f 666f 725f 7265 6164 79da  .wait_for_ready.
-00000f80: 0774 696d 656f 7574 da08 6d65 7461 6461  .timeout..metada
-00000f90: 7461 7221 0000 0072 2100 0000 7222 0000  tar!...r!...r"..
-00000fa0: 0072 1200 0000 7f00 0000 f30c 0000 000c  .r..............
-00000fb0: 0b06 0106 0104 010c 0104 fc7a 1754 6162  ...........z.Tab
-00000fc0: 6c65 5365 7276 6963 652e 4c69 7374 5461  leService.ListTa
-00000fd0: 626c 6573 630a 0000 0000 0000 0000 0000  blesc...........
-00000fe0: 000a 0000 000f 0000 0043 0000 0072 4100  .........C...rA.
-00000ff0: 0000 2902 4e72 0800 0000 2908 722d 0000  ..).Nr....).r-..
-00001000: 0072 4200 0000 720c 0000 0072 0d00 0000  .rB...r....r....
-00001010: 7213 0000 0072 0f00 0000 7214 0000 0072  r....r....r....r
-00001020: 1100 0000 7243 0000 0072 2100 0000 7221  ....rC...r!...r!
-00001030: 0000 0072 2200 0000 7215 0000 0090 0000  ...r"...r.......
-00001040: 0072 4d00 0000 7a15 5461 626c 6553 6572  .rM...z.TableSer
-00001050: 7669 6365 2e47 6574 5461 626c 6563 0a00  vice.GetTablec..
-00001060: 0000 0000 0000 0000 0000 0a00 0000 0f00  ................
-00001070: 0000 4300 0000 7241 0000 0029 024e 7209  ..C...rA...).Nr.
-00001080: 0000 0029 0872 2d00 0000 7242 0000 0072  ...).r-...rB...r
-00001090: 0c00 0000 720d 0000 0072 1600 0000 720f  ....r....r....r.
-000010a0: 0000 0072 1700 0000 7211 0000 0072 4300  ...r....r....rC.
-000010b0: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-000010c0: 0072 1800 0000 a100 0000 724d 0000 007a  .r........rM...z
-000010d0: 1854 6162 6c65 5365 7276 6963 652e 4372  .TableService.Cr
-000010e0: 6561 7465 5461 626c 6563 0a00 0000 0000  eateTablec......
-000010f0: 0000 0000 0000 0a00 0000 0f00 0000 4300  ..............C.
-00001100: 0000 7241 0000 0029 024e 720a 0000 0029  ..rA...).Nr....)
-00001110: 0872 2d00 0000 7242 0000 0072 0c00 0000  .r-...rB...r....
-00001120: 720d 0000 0072 1900 0000 720f 0000 0072  r....r....r....r
-00001130: 1a00 0000 7211 0000 0072 4300 0000 7221  ....r....rC...r!
-00001140: 0000 0072 2100 0000 7222 0000 0072 1b00  ...r!...r"...r..
-00001150: 0000 b200 0000 724d 0000 007a 1854 6162  ......rM...z.Tab
-00001160: 6c65 5365 7276 6963 652e 4465 6c65 7465  leService.Delete
-00001170: 5461 626c 6563 0a00 0000 0000 0000 0000  Tablec..........
-00001180: 0000 0a00 0000 0f00 0000 4300 0000 7241  ..........C...rA
-00001190: 0000 0029 024e 720b 0000 0029 0872 2d00  ...).Nr....).r-.
-000011a0: 0000 7242 0000 0072 0c00 0000 720d 0000  ..rB...r....r...
-000011b0: 0072 1c00 0000 720f 0000 0072 1d00 0000  .r....r....r....
-000011c0: 7211 0000 0072 4300 0000 7221 0000 0072  r....rC...r!...r
-000011d0: 2100 0000 7222 0000 0072 1e00 0000 c300  !...r"...r......
-000011e0: 0000 724d 0000 007a 1554 6162 6c65 5365  ..rM...z.TableSe
-000011f0: 7276 6963 652e 4c6f 6164 4461 7461 2908  rvice.LoadData).
-00001200: 7221 0000 004e 4e46 4e4e 4e4e 290a 7224  r!...NNFNNNN).r$
-00001210: 0000 0072 2500 0000 7226 0000 0072 2700  ...r%...r&...r'.
-00001220: 0000 da0c 7374 6174 6963 6d65 7468 6f64  ....staticmethod
-00001230: 7212 0000 0072 1500 0000 7218 0000 0072  r....r....r....r
-00001240: 1b00 0000 721e 0000 0072 2100 0000 7221  ....r....r!...r!
-00001250: 0000 0072 2100 0000 7222 0000 0072 4000  ...r!...r"...r@.
-00001260: 0000 7b00 0000 7368 0000 0008 0004 0102  ..{...sh........
-00001270: 0302 0302 0102 0102 0102 0102 0102 0102  ................
-00001280: 010c f702 1002 0302 0102 0102 0102 0102  ................
-00001290: 0102 0102 010c f702 1002 0302 0102 0102  ................
-000012a0: 0102 0102 0102 0102 010c f702 1002 0302  ................
-000012b0: 0102 0102 0102 0102 0102 0102 010c f702  ................
-000012c0: 1002 0302 0102 0102 0102 0102 0102 0102  ................
-000012d0: 0110 f772 4000 0000 290a 7227 0000 0072  ...r@...).r'...r
-000012e0: 2d00 0000 da17 6b61 736b 6164 612e 6b61  -.....kaskada.ka
-000012f0: 736b 6164 612e 7631 616c 7068 6172 0200  skada.v1alphar..
-00001300: 0000 720d 0000 00da 066f 626a 6563 7472  ..r......objectr
-00001310: 0300 0000 7228 0000 0072 3f00 0000 7240  ....r(...r?...r@
-00001320: 0000 0072 2100 0000 7221 0000 0072 2100  ...r!...r!...r!.
-00001330: 0000 7222 0000 00da 083c 6d6f 6475 6c65  ..r".....<module
-00001340: 3e01 0000 0073 0e00 0000 0401 0801 0c02  >....s..........
-00001350: 1003 1025 082c 1422                      ...%.,."
+000004e0: 2100 0000 fa3a 2f73 7263 2f73 7263 2f6b  !....:/src/src/k
+000004f0: 6173 6b61 6461 2f6b 6173 6b61 6461 2f76  askada/kaskada/v
+00000500: 3161 6c70 6861 2f74 6162 6c65 5f73 6572  1alpha/table_ser
+00000510: 7669 6365 5f70 6232 5f67 7270 632e 7079  vice_pb2_grpc.py
+00000520: da08 5f5f 696e 6974 5f5f 0c00 0000 7332  ..__init__....s2
+00000530: 0000 0000 0604 0102 0106 0106 fd08 0504  ................
+00000540: 0102 0106 0106 fd08 0504 0102 0106 0106  ................
+00000550: fd08 0504 0102 0106 0106 fd08 0504 0102  ................
+00000560: 0106 0106 fd7a 1954 6162 6c65 5365 7276  .....z.TableServ
+00000570: 6963 6553 7475 622e 5f5f 696e 6974 5f5f  iceStub.__init__
+00000580: 4e29 05da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000590: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000005a0: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+000005b0: 7223 0000 0072 2100 0000 7221 0000 0072  r#...r!...r!...r
+000005c0: 2100 0000 7222 0000 0072 0300 0000 0800  !...r"...r......
+000005d0: 0000 7304 0000 0008 0104 0372 0300 0000  ..s........r....
+000005e0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000005f0: 0002 0000 0040 0000 0073 3800 0000 6500  .....@...s8...e.
+00000600: 5a01 6400 5a02 6401 5a03 6402 6403 8400  Z.d.Z.d.Z.d.d...
+00000610: 5a04 6404 6405 8400 5a05 6406 6407 8400  Z.d.d...Z.d.d...
+00000620: 5a06 6408 6409 8400 5a07 640a 640b 8400  Z.d.d...Z.d.d...
+00000630: 5a08 640c 5300 290d da14 5461 626c 6553  Z.d.S.)...TableS
+00000640: 6572 7669 6365 5365 7276 6963 6572 7204  erviceServicerr.
+00000650: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+00000660: 0300 0000 0300 0000 4300 0000 7324 0000  ........C...s$..
+00000670: 007c 02a0 0074 016a 026a 03a1 0101 007c  .|...t.j.j.....|
+00000680: 02a0 0464 01a1 0101 0074 0564 0183 0182  ...d.....t.d....
+00000690: 0164 0253 0029 037a c64c 6973 7473 2074  .d.S.).z.Lists t
+000006a0: 6162 6c65 732e 0a0a 2020 2020 2020 2020  ables...        
+000006b0: 5468 6520 7265 7370 6f6e 7365 2069 6e63  The response inc
+000006c0: 6c75 6465 7320 616c 6c20 5461 626c 6573  ludes all Tables
+000006d0: 2064 6566 696e 6564 2066 6f72 2074 6865   defined for the
+000006e0: 204b 6173 6b61 6461 2061 6363 6f75 6e74   Kaskada account
+000006f0: 2e0a 2020 2020 2020 2020 4966 2061 2073  ..        If a s
+00000700: 6561 7263 6820 7374 7269 6e67 2069 7320  earch string is 
+00000710: 7072 6f76 6964 6564 2c20 6f6e 6c79 2054  provided, only T
+00000720: 6162 6c65 7320 6d61 7463 6869 6e67 2074  ables matching t
+00000730: 6865 2073 6561 7263 680a 2020 2020 2020  he search.      
+00000740: 2020 7374 7269 6e67 2061 7265 2072 6574    string are ret
+00000750: 7572 6e65 642e 0a20 2020 2020 2020 20fa  urned..        .
+00000760: 174d 6574 686f 6420 6e6f 7420 696d 706c  .Method not impl
+00000770: 656d 656e 7465 6421 4ea9 06da 0873 6574  emented!N....set
+00000780: 5f63 6f64 65da 0467 7270 63da 0a53 7461  _code..grpc..Sta
+00000790: 7475 7343 6f64 65da 0d55 4e49 4d50 4c45  tusCode..UNIMPLE
+000007a0: 4d45 4e54 4544 da0b 7365 745f 6465 7461  MENTED..set_deta
+000007b0: 696c 73da 134e 6f74 496d 706c 656d 656e  ils..NotImplemen
+000007c0: 7465 6445 7272 6f72 a903 721f 0000 00da  tedError..r.....
+000007d0: 0772 6571 7565 7374 da07 636f 6e74 6578  .request..contex
+000007e0: 7472 2100 0000 7221 0000 0072 2200 0000  tr!...r!...r"...
+000007f0: 7212 0000 0031 0000 0073 0600 0000 0007  r....1...s......
+00000800: 0e01 0a01 7a1f 5461 626c 6553 6572 7669  ....z.TableServi
+00000810: 6365 5365 7276 6963 6572 2e4c 6973 7454  ceServicer.ListT
+00000820: 6162 6c65 7363 0300 0000 0000 0000 0000  ablesc..........
+00000830: 0000 0300 0000 0300 0000 4300 0000 7324  ..........C...s$
+00000840: 0000 007c 02a0 0074 016a 026a 03a1 0101  ...|...t.j.j....
+00000850: 007c 02a0 0464 01a1 0101 0074 0564 0183  .|...d.....t.d..
+00000860: 0182 0164 0253 0029 037a 1647 6574 7320  ...d.S.).z.Gets 
+00000870: 6120 7461 626c 652e 0a20 2020 2020 2020  a table..       
+00000880: 2072 2900 0000 4e72 2a00 0000 7231 0000   r)...Nr*...r1..
+00000890: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+000008a0: 7215 0000 003c 0000 0073 0600 0000 0003  r....<...s......
+000008b0: 0e01 0a01 7a1d 5461 626c 6553 6572 7669  ....z.TableServi
+000008c0: 6365 5365 7276 6963 6572 2e47 6574 5461  ceServicer.GetTa
+000008d0: 626c 6563 0300 0000 0000 0000 0000 0000  blec............
+000008e0: 0300 0000 0300 0000 4300 0000 7324 0000  ........C...s$..
+000008f0: 007c 02a0 0074 016a 026a 03a1 0101 007c  .|...t.j.j.....|
+00000900: 02a0 0464 01a1 0101 0074 0564 0183 0182  ...d.....t.d....
+00000910: 0164 0253 0029 037a 1943 7265 6174 6573  .d.S.).z.Creates
+00000920: 2061 2074 6162 6c65 2e0a 2020 2020 2020   a table..      
+00000930: 2020 7229 0000 004e 722a 0000 0072 3100    r)...Nr*...r1.
+00000940: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+00000950: 0072 1800 0000 4300 0000 7306 0000 0000  .r....C...s.....
+00000960: 030e 010a 017a 2054 6162 6c65 5365 7276  .....z TableServ
+00000970: 6963 6553 6572 7669 6365 722e 4372 6561  iceServicer.Crea
+00000980: 7465 5461 626c 6563 0300 0000 0000 0000  teTablec........
+00000990: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
+000009a0: 7324 0000 007c 02a0 0074 016a 026a 03a1  s$...|...t.j.j..
+000009b0: 0101 007c 02a0 0464 01a1 0101 0074 0564  ...|...d.....t.d
+000009c0: 0183 0182 0164 0253 0029 037a 3744 656c  .....d.S.).z7Del
+000009d0: 6574 6573 2061 2074 6162 6c65 2061 6e64  etes a table and
+000009e0: 2061 6e79 2065 7665 6e74 7320 6c6f 6164   any events load
+000009f0: 6564 2069 6e74 6f20 6974 2e0a 2020 2020  ed into it..    
+00000a00: 2020 2020 7229 0000 004e 722a 0000 0072      r)...Nr*...r
+00000a10: 3100 0000 7221 0000 0072 2100 0000 7222  1...r!...r!...r"
+00000a20: 0000 0072 1b00 0000 4a00 0000 7306 0000  ...r....J...s...
+00000a30: 0000 030e 010a 017a 2054 6162 6c65 5365  .......z TableSe
+00000a40: 7276 6963 6553 6572 7669 6365 722e 4465  rviceServicer.De
+00000a50: 6c65 7465 5461 626c 6563 0300 0000 0000  leteTablec......
+00000a60: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
+00000a70: 0000 7324 0000 007c 02a0 0074 016a 026a  ..s$...|...t.j.j
+00000a80: 03a1 0101 007c 02a0 0464 01a1 0101 0074  .....|...d.....t
+00000a90: 0564 0183 0182 0164 0253 0029 037a 294c  .d.....d.S.).z)L
+00000aa0: 6f61 6473 2061 2073 7461 6765 6420 6669  oads a staged fi
+00000ab0: 6c65 2069 6e74 6f20 6120 7461 626c 650a  le into a table.
+00000ac0: 2020 2020 2020 2020 7229 0000 004e 722a          r)...Nr*
+00000ad0: 0000 0072 3100 0000 7221 0000 0072 2100  ...r1...r!...r!.
+00000ae0: 0000 7222 0000 0072 1e00 0000 5100 0000  ..r"...r....Q...
+00000af0: 7306 0000 0000 030e 010a 017a 1d54 6162  s..........z.Tab
+00000b00: 6c65 5365 7276 6963 6553 6572 7669 6365  leServiceService
+00000b10: 722e 4c6f 6164 4461 7461 4e29 0972 2400  r.LoadDataN).r$.
+00000b20: 0000 7225 0000 0072 2600 0000 7227 0000  ..r%...r&...r'..
+00000b30: 0072 1200 0000 7215 0000 0072 1800 0000  .r....r....r....
+00000b40: 721b 0000 0072 1e00 0000 7221 0000 0072  r....r....r!...r
+00000b50: 2100 0000 7221 0000 0072 2200 0000 7228  !...r!...r"...r(
+00000b60: 0000 002d 0000 0073 0c00 0000 0801 0403  ...-...s........
+00000b70: 080b 0807 0807 0807 7228 0000 0063 0200  ........r(...c..
+00000b80: 0000 0000 0000 0000 0000 0400 0000 0900  ................
+00000b90: 0000 4300 0000 739a 0000 0074 006a 017c  ..C...s....t.j.|
+00000ba0: 006a 0274 036a 046a 0574 036a 066a 0764  .j.t.j.j.t.j.j.d
+00000bb0: 018d 0374 006a 017c 006a 0874 036a 096a  ...t.j.|.j.t.j.j
+00000bc0: 0574 036a 0a6a 0764 018d 0374 006a 017c  .t.j.j.d...t.j.|
+00000bd0: 006a 0b74 036a 0c6a 0574 036a 0d6a 0764  .j.t.j.j.t.j.j.d
+00000be0: 018d 0374 006a 017c 006a 0e74 036a 0f6a  ...t.j.|.j.t.j.j
+00000bf0: 0574 036a 106a 0764 018d 0374 006a 017c  .t.j.j.d...t.j.|
+00000c00: 006a 1174 036a 126a 0574 036a 136a 0764  .j.t.j.j.t.j.j.d
+00000c10: 018d 0364 029c 057d 0274 00a0 1464 037c  ...d...}.t...d.|
+00000c20: 02a1 027d 037c 01a0 157c 0366 01a1 0101  ...}.|...|.f....
+00000c30: 0064 0053 0029 044e 2902 da14 7265 7175  .d.S.).N)...requ
+00000c40: 6573 745f 6465 7365 7269 616c 697a 6572  est_deserializer
+00000c50: da13 7265 7370 6f6e 7365 5f73 6572 6961  ..response_seria
+00000c60: 6c69 7a65 7229 0572 1200 0000 7215 0000  lizer).r....r...
+00000c70: 0072 1800 0000 721b 0000 0072 1e00 0000  .r....r....r....
+00000c80: 7a24 6b61 736b 6164 612e 6b61 736b 6164  z$kaskada.kaskad
+00000c90: 612e 7631 616c 7068 612e 5461 626c 6553  a.v1alpha.TableS
+00000ca0: 6572 7669 6365 2916 722c 0000 00da 1e75  ervice).r,.....u
+00000cb0: 6e61 7279 5f75 6e61 7279 5f72 7063 5f6d  nary_unary_rpc_m
+00000cc0: 6574 686f 645f 6861 6e64 6c65 7272 1200  ethod_handlerr..
+00000cd0: 0000 720d 0000 0072 0e00 0000 7211 0000  ..r....r....r...
+00000ce0: 0072 1000 0000 720f 0000 0072 1500 0000  .r....r....r....
+00000cf0: 7213 0000 0072 1400 0000 7218 0000 0072  r....r....r....r
+00000d00: 1600 0000 7217 0000 0072 1b00 0000 7219  ....r....r....r.
+00000d10: 0000 0072 1a00 0000 721e 0000 0072 1c00  ...r....r....r..
+00000d20: 0000 721d 0000 00da 1f6d 6574 686f 645f  ..r......method_
+00000d30: 6861 6e64 6c65 7273 5f67 656e 6572 6963  handlers_generic
+00000d40: 5f68 616e 646c 6572 da18 6164 645f 6765  _handler..add_ge
+00000d50: 6e65 7269 635f 7270 635f 6861 6e64 6c65  neric_rpc_handle
+00000d60: 7273 2904 da08 7365 7276 6963 6572 da06  rs)...servicer..
+00000d70: 7365 7276 6572 da13 7270 635f 6d65 7468  server..rpc_meth
+00000d80: 6f64 5f68 616e 646c 6572 73da 0f67 656e  od_handlers..gen
+00000d90: 6572 6963 5f68 616e 646c 6572 7221 0000  eric_handlerr!..
+00000da0: 0072 2100 0000 7222 0000 00da 2261 6464  .r!...r"...."add
+00000db0: 5f54 6162 6c65 5365 7276 6963 6553 6572  _TableServiceSer
+00000dc0: 7669 6365 725f 746f 5f73 6572 7665 7259  vicer_to_serverY
+00000dd0: 0000 0073 3c00 0000 0002 0401 0401 0601  ...s<...........
+00000de0: 06fd 0405 0401 0401 0601 06fd 0405 0401  ................
+00000df0: 0401 0601 06fd 0405 0401 0401 0601 06fd  ................
+00000e00: 0405 0401 0401 0601 06fd 04eb 061b 0401  ................
+00000e10: 04ff 0402 723d 0000 0063 0000 0000 0000  ....r=...c......
+00000e20: 0000 0000 0000 0000 0000 0900 0000 4000  ..............@.
+00000e30: 0000 7356 0000 0065 005a 0164 005a 0264  ..sV...e.Z.d.Z.d
+00000e40: 015a 0365 0464 0f64 0564 0684 0183 015a  .Z.e.d.d.d.....Z
+00000e50: 0565 0464 1064 0764 0884 0183 015a 0665  .e.d.d.d.....Z.e
+00000e60: 0464 1164 0964 0a84 0183 015a 0765 0464  .d.d.d.....Z.e.d
+00000e70: 1264 0b64 0c84 0183 015a 0865 0464 1364  .d.d.....Z.e.d.d
+00000e80: 0d64 0e84 0183 015a 0964 0353 0029 14da  .d.....Z.d.S.)..
+00000e90: 0c54 6162 6c65 5365 7276 6963 6572 0400  .TableServicer..
+00000ea0: 0000 7221 0000 004e 4663 0a00 0000 0000  ..r!...NFc......
+00000eb0: 0000 0000 0000 0a00 0000 0f00 0000 4300  ..............C.
+00000ec0: 0000 732c 0000 0074 006a 01a0 027c 007c  ..s,...t.j...|.|
+00000ed0: 0164 0174 036a 046a 0574 036a 066a 077c  .d.t.j.j.t.j.j.|
+00000ee0: 027c 037c 057c 047c 067c 077c 087c 09a1  .|.|.|.|.|.|.|..
+00000ef0: 0d53 0029 024e 7205 0000 0029 0872 2c00  .S.).Nr....).r,.
+00000f00: 0000 da0c 6578 7065 7269 6d65 6e74 616c  ....experimental
+00000f10: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00000f20: 0f00 0000 7210 0000 0072 1100 0000 a90a  ....r....r......
+00000f30: 7232 0000 00da 0674 6172 6765 74da 076f  r2.....target..o
+00000f40: 7074 696f 6e73 da13 6368 616e 6e65 6c5f  ptions..channel_
+00000f50: 6372 6564 656e 7469 616c 73da 1063 616c  credentials..cal
+00000f60: 6c5f 6372 6564 656e 7469 616c 73da 0869  l_credentials..i
+00000f70: 6e73 6563 7572 65da 0b63 6f6d 7072 6573  nsecure..compres
+00000f80: 7369 6f6e da0e 7761 6974 5f66 6f72 5f72  sion..wait_for_r
+00000f90: 6561 6479 da07 7469 6d65 6f75 74da 086d  eady..timeout..m
+00000fa0: 6574 6164 6174 6172 2100 0000 7221 0000  etadatar!...r!..
+00000fb0: 0072 2200 0000 7212 0000 007f 0000 0073  .r"...r........s
+00000fc0: 0c00 0000 000b 0c01 0601 0601 0401 0cfc  ................
+00000fd0: 7a17 5461 626c 6553 6572 7669 6365 2e4c  z.TableService.L
+00000fe0: 6973 7454 6162 6c65 7363 0a00 0000 0000  istTablesc......
+00000ff0: 0000 0000 0000 0a00 0000 0f00 0000 4300  ..............C.
+00001000: 0000 732c 0000 0074 006a 01a0 027c 007c  ..s,...t.j...|.|
+00001010: 0164 0174 036a 046a 0574 036a 066a 077c  .d.t.j.j.t.j.j.|
+00001020: 027c 037c 057c 047c 067c 077c 087c 09a1  .|.|.|.|.|.|.|..
+00001030: 0d53 0029 024e 7208 0000 0029 0872 2c00  .S.).Nr....).r,.
+00001040: 0000 723f 0000 0072 0c00 0000 720d 0000  ..r?...r....r...
+00001050: 0072 1300 0000 720f 0000 0072 1400 0000  .r....r....r....
+00001060: 7211 0000 0072 4000 0000 7221 0000 0072  r....r@...r!...r
+00001070: 2100 0000 7222 0000 0072 1500 0000 9000  !...r"...r......
+00001080: 0000 730c 0000 0000 0b0c 0106 0106 0104  ..s.............
+00001090: 010c fc7a 1554 6162 6c65 5365 7276 6963  ...z.TableServic
+000010a0: 652e 4765 7454 6162 6c65 630a 0000 0000  e.GetTablec.....
+000010b0: 0000 0000 0000 000a 0000 000f 0000 0043  ...............C
+000010c0: 0000 0073 2c00 0000 7400 6a01 a002 7c00  ...s,...t.j...|.
+000010d0: 7c01 6401 7403 6a04 6a05 7403 6a06 6a07  |.d.t.j.j.t.j.j.
+000010e0: 7c02 7c03 7c05 7c04 7c06 7c07 7c08 7c09  |.|.|.|.|.|.|.|.
+000010f0: a10d 5300 2902 4e72 0900 0000 2908 722c  ..S.).Nr....).r,
+00001100: 0000 0072 3f00 0000 720c 0000 0072 0d00  ...r?...r....r..
+00001110: 0000 7216 0000 0072 0f00 0000 7217 0000  ..r....r....r...
+00001120: 0072 1100 0000 7240 0000 0072 2100 0000  .r....r@...r!...
+00001130: 7221 0000 0072 2200 0000 7218 0000 00a1  r!...r"...r.....
+00001140: 0000 0073 0c00 0000 000b 0c01 0601 0601  ...s............
+00001150: 0401 0cfc 7a18 5461 626c 6553 6572 7669  ....z.TableServi
+00001160: 6365 2e43 7265 6174 6554 6162 6c65 630a  ce.CreateTablec.
+00001170: 0000 0000 0000 0000 0000 000a 0000 000f  ................
+00001180: 0000 0043 0000 0073 2c00 0000 7400 6a01  ...C...s,...t.j.
+00001190: a002 7c00 7c01 6401 7403 6a04 6a05 7403  ..|.|.d.t.j.j.t.
+000011a0: 6a06 6a07 7c02 7c03 7c05 7c04 7c06 7c07  j.j.|.|.|.|.|.|.
+000011b0: 7c08 7c09 a10d 5300 2902 4e72 0a00 0000  |.|...S.).Nr....
+000011c0: 2908 722c 0000 0072 3f00 0000 720c 0000  ).r,...r?...r...
+000011d0: 0072 0d00 0000 7219 0000 0072 0f00 0000  .r....r....r....
+000011e0: 721a 0000 0072 1100 0000 7240 0000 0072  r....r....r@...r
+000011f0: 2100 0000 7221 0000 0072 2200 0000 721b  !...r!...r"...r.
+00001200: 0000 00b2 0000 0073 0c00 0000 000b 0c01  .......s........
+00001210: 0601 0601 0401 0cfc 7a18 5461 626c 6553  ........z.TableS
+00001220: 6572 7669 6365 2e44 656c 6574 6554 6162  ervice.DeleteTab
+00001230: 6c65 630a 0000 0000 0000 0000 0000 000a  lec.............
+00001240: 0000 000f 0000 0043 0000 0073 2c00 0000  .......C...s,...
+00001250: 7400 6a01 a002 7c00 7c01 6401 7403 6a04  t.j...|.|.d.t.j.
+00001260: 6a05 7403 6a06 6a07 7c02 7c03 7c05 7c04  j.t.j.j.|.|.|.|.
+00001270: 7c06 7c07 7c08 7c09 a10d 5300 2902 4e72  |.|.|.|...S.).Nr
+00001280: 0b00 0000 2908 722c 0000 0072 3f00 0000  ....).r,...r?...
+00001290: 720c 0000 0072 0d00 0000 721c 0000 0072  r....r....r....r
+000012a0: 0f00 0000 721d 0000 0072 1100 0000 7240  ....r....r....r@
+000012b0: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+000012c0: 0000 721e 0000 00c3 0000 0073 0c00 0000  ..r........s....
+000012d0: 000b 0c01 0601 0601 0401 0cfc 7a15 5461  ............z.Ta
+000012e0: 626c 6553 6572 7669 6365 2e4c 6f61 6444  bleService.LoadD
+000012f0: 6174 6129 0872 2100 0000 4e4e 464e 4e4e  ata).r!...NNFNNN
+00001300: 4e29 0872 2100 0000 4e4e 464e 4e4e 4e29  N).r!...NNFNNNN)
+00001310: 0872 2100 0000 4e4e 464e 4e4e 4e29 0872  .r!...NNFNNNN).r
+00001320: 2100 0000 4e4e 464e 4e4e 4e29 0872 2100  !...NNFNNNN).r!.
+00001330: 0000 4e4e 464e 4e4e 4e29 0a72 2400 0000  ..NNFNNNN).r$...
+00001340: 7225 0000 0072 2600 0000 7227 0000 00da  r%...r&...r'....
+00001350: 0c73 7461 7469 636d 6574 686f 6472 1200  .staticmethodr..
+00001360: 0000 7215 0000 0072 1800 0000 721b 0000  ..r....r....r...
+00001370: 0072 1e00 0000 7221 0000 0072 2100 0000  .r....r!...r!...
+00001380: 7221 0000 0072 2200 0000 723e 0000 007b  r!...r"...r>...{
+00001390: 0000 0073 6600 0000 0801 0403 0203 0001  ...sf...........
+000013a0: 0001 0001 0001 0001 0001 0001 00f7 0c10  ................
+000013b0: 0203 0001 0001 0001 0001 0001 0001 0001  ................
+000013c0: 00f7 0c10 0203 0001 0001 0001 0001 0001  ................
+000013d0: 0001 0001 00f7 0c10 0203 0001 0001 0001  ................
+000013e0: 0001 0001 0001 0001 00f7 0c10 0203 0001  ................
+000013f0: 0001 0001 0001 0001 0001 0001 00f7 723e  ..............r>
+00001400: 0000 0029 0a72 2700 0000 722c 0000 00da  ...).r'...r,....
+00001410: 176b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00001420: 2e76 3161 6c70 6861 7202 0000 0072 0d00  .v1alphar....r..
+00001430: 0000 da06 6f62 6a65 6374 7203 0000 0072  ....objectr....r
+00001440: 2800 0000 723d 0000 0072 3e00 0000 7221  (...r=...r>...r!
+00001450: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00001460: 0000 da08 3c6d 6f64 756c 653e 0200 0000  ....<module>....
+00001470: 730c 0000 0004 0108 020c 0310 2510 2c08  s...........%.,.
+00001480: 22                                       "
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2.cpython-310-pytest-7.2.1.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2.cpython-39-pytest-7.2.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 6835 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 b31a 0000  o.........5d....
+00000000: 610d 0d0a 0000 0000 0449 2364 b31a 0000  a........I#d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000d 0000 0040 0000 0073 0c02 0000 6400  .....@...s....d.
+00000020: 000d 0000 0040 0000 0073 0802 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 0200 0100 6d05 5a06 0100 6401 6403  m.....m.Z...d.d.
 00000050: 6c07 6d08 5a09 0100 6401 6404 6c07 6d0a  l.m.Z...d.d.l.m.
 00000060: 5a0b 0100 6401 6405 6c07 6d0c 5a0d 0100  Z...d.d.l.m.Z...
 00000070: 6401 6406 6c07 6d0e 5a0f 0100 6401 6407  d.d.l.m.Z...d.d.
 00000080: 6c07 6d10 5a11 0100 6511 a012 a100 5a13  l.m.Z...e.....Z.
 00000090: 6401 6408 6c14 6d15 5a16 0100 650b a012  d.d.l.m.Z...e...
@@ -16,223 +16,219 @@
 000000f0: 9c02 a103 650f a01f 640c 650d 6a20 6601  ....e...d.e.j f.
 00000100: 651d 640e 640f 9c02 a103 650f a01f 640d  e.d.d.....e...d.
 00000110: 650d 6a20 6601 651e 640e 640f 9c02 a103  e.j f.e.d.d.....
 00000120: 651a 640e 6410 9c05 a103 5a21 6513 a022  e.d.d.....Z!e.."
 00000130: 6521 a101 0100 6513 a022 6521 6a23 a101  e!....e.."e!j#..
 00000140: 0100 6513 a022 6521 6a24 a101 0100 6513  ..e.."e!j$....e.
 00000150: a022 6521 6a25 a101 0100 6509 6a26 6411  ."e!j%....e.j&d.
-00000160: 6b02 9001 7204 6402 6518 5f27 6412 6518  k...r.d.e._'d.e.
+00000160: 6b02 9002 7204 6402 6518 5f27 6412 6518  k...r.d.e._'d.e.
 00000170: 5f28 6402 651c 5f27 6413 651c 5f28 6402  _(d.e._'d.e._(d.
 00000180: 651d 5f27 6413 651d 5f28 6402 651e 6a29  e._'d.e._(d.e.j)
 00000190: 6414 1900 5f27 6415 651e 6a29 6414 1900  d..._'d.e.j)d...
 000001a0: 5f28 6402 651a 6a29 6416 1900 5f27 6415  _(d.e.j)d..._'d.
 000001b0: 651a 6a29 6416 1900 5f28 6402 651a 6a29  e.j)d..._(d.e.j)
 000001c0: 6417 1900 5f27 6415 651a 6a29 6417 1900  d..._'d.e.j)d...
 000001d0: 5f28 6402 651a 6a29 6418 1900 5f27 6415  _(d.e.j)d..._'d.
 000001e0: 651a 6a29 6418 1900 5f28 6402 651a 6a29  e.j)d..._(d.e.j)
 000001f0: 6419 1900 5f27 6415 651a 6a29 6419 1900  d..._'d.e.j)d...
 00000200: 5f28 641a 651a 5f2a 641b 651a 5f2b 641c  _(d.e._*d.e._+d.
 00000210: 651c 5f2a 641d 651c 5f2b 641e 651d 5f2a  e._*d.e._+d.e._*
 00000220: 641f 651d 5f2b 6420 651e 5f2a 6421 651e  d.e._+d e._*d!e.
-00000230: 5f2b 6402 5300 6402 5300 2922 7a1f 4765  _+d.S.d.S.)"z.Ge
-00000240: 6e65 7261 7465 6420 7072 6f74 6f63 6f6c  nerated protocol
-00000250: 2062 7566 6665 7220 636f 6465 2ee9 0000   buffer code....
-00000260: 0000 4e29 01da 0a64 6573 6372 6970 746f  ..N)...descripto
-00000270: 7229 01da 0f64 6573 6372 6970 746f 725f  r)...descriptor_
-00000280: 706f 6f6c 2901 da07 6d65 7373 6167 6529  pool)...message)
-00000290: 01da 0a72 6566 6c65 6374 696f 6e29 01da  ...reflection)..
-000002a0: 0f73 796d 626f 6c5f 6461 7461 6261 7365  .symbol_database
-000002b0: 2901 da0b 6f70 7469 6f6e 735f 7062 3273  )...options_pb2s
-000002c0: 0606 0000 0a28 6b61 736b 6164 612f 6b61  .....(kaskada/ka
-000002d0: 736b 6164 612f 7631 616c 7068 612f 7465  skada/v1alpha/te
-000002e0: 7374 5f63 6173 6573 2e70 726f 746f 1217  st_cases.proto..
-000002f0: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
-00000300: 7631 616c 7068 611a 256b 6173 6b61 6461  v1alpha.%kaskada
-00000310: 2f6b 6173 6b61 6461 2f76 3161 6c70 6861  /kaskada/v1alpha
-00000320: 2f6f 7074 696f 6e73 2e70 726f 746f 2290  /options.proto".
-00000330: 090a 0e52 6564 6163 7454 6573 7443 6173  ...RedactTestCas
-00000340: 6512 260a 0f72 6f6f 745f 7361 6665 5f76  e.&..root_safe_v
-00000350: 616c 7565 1801 2001 2809 520d 726f 6f74  alue.. .(.R.root
-00000360: 5361 6665 5661 6c75 6512 360a 1472 6f6f  SafeValue.6..roo
-00000370: 745f 7365 6e73 6974 6976 655f 7661 6c75  t_sensitive_valu
-00000380: 6518 0220 0128 0942 0480 b518 0152 1272  e.. .(.B.....R.r
-00000390: 6f6f 7453 656e 7369 7469 7665 5661 6c75  ootSensitiveValu
-000003a0: 6512 400a 1972 6570 6561 7465 645f 7365  e.@..repeated_se
-000003b0: 6e73 6974 6976 655f 7661 6c75 6573 1803  nsitive_values..
-000003c0: 2003 2809 4204 80b5 1801 5217 7265 7065   .(.B.....R.repe
-000003d0: 6174 6564 5365 6e73 6974 6976 6556 616c  atedSensitiveVal
-000003e0: 7565 7312 680a 1472 6f6f 745f 656d 6265  ues.h..root_embe
-000003f0: 6464 6564 5f6f 626a 6563 7418 0420 0128  dded_object.. .(
-00000400: 0b32 362e 6b61 736b 6164 612e 6b61 736b  .26.kaskada.kask
-00000410: 6164 612e 7631 616c 7068 612e 5265 6461  ada.v1alpha.Reda
-00000420: 6374 5465 7374 4361 7365 2e45 6d62 6564  ctTestCase.Embed
-00000430: 6465 644f 626a 6563 7452 1272 6f6f 7445  dedObjectR.rootE
-00000440: 6d62 6564 6465 644f 626a 6563 7412 700a  mbeddedObject.p.
-00000450: 1872 6570 6561 7465 645f 656d 6265 6464  .repeated_embedd
-00000460: 6564 5f6f 626a 6563 7418 0520 0328 0b32  ed_object.. .(.2
-00000470: 362e 6b61 736b 6164 612e 6b61 736b 6164  6.kaskada.kaskad
-00000480: 612e 7631 616c 7068 612e 5265 6461 6374  a.v1alpha.Redact
-00000490: 5465 7374 4361 7365 2e45 6d62 6564 6465  TestCase.Embedde
-000004a0: 644f 626a 6563 7452 1672 6570 6561 7465  dObjectR.repeate
-000004b0: 6445 6d62 6564 6465 644f 626a 6563 7412  dEmbeddedObject.
-000004c0: 2b0a 116f 6e65 5f6f 665f 7361 6665 5f76  +..one_of_safe_v
-000004d0: 616c 7565 1807 2001 2809 4800 520e 6f6e  alue.. .(.H.R.on
-000004e0: 654f 6653 6166 6556 616c 7565 123b 0a16  eOfSafeValue.;..
-000004f0: 6f6e 655f 6f66 5f73 656e 7369 7469 7665  one_of_sensitive
-00000500: 5f76 616c 7565 1808 2001 2809 4204 80b5  _value.. .(.B...
-00000510: 1801 4800 5213 6f6e 654f 6653 656e 7369  ..H.R.oneOfSensi
-00000520: 7469 7665 5661 6c75 6512 6b0a 156f 6e65  tiveValue.k..one
-00000530: 5f6f 665f 656d 6265 6464 6564 5f76 616c  _of_embedded_val
-00000540: 7565 1809 2001 280b 3236 2e6b 6173 6b61  ue.. .(.26.kaska
-00000550: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
-00000560: 6861 2e52 6564 6163 7454 6573 7443 6173  ha.RedactTestCas
-00000570: 652e 456d 6265 6464 6564 4f62 6a65 6374  e.EmbeddedObject
-00000580: 4800 5212 6f6e 654f 6645 6d62 6564 6465  H.R.oneOfEmbedde
-00000590: 6456 616c 7565 1277 0a14 6d61 705f 7365  dValue.w..map_se
-000005a0: 6e73 6974 6976 655f 7661 6c75 6573 180a  nsitive_values..
-000005b0: 2003 280b 323f 2e6b 6173 6b61 6461 2e6b   .(.2?.kaskada.k
-000005c0: 6173 6b61 6461 2e76 3161 6c70 6861 2e52  askada.v1alpha.R
-000005d0: 6564 6163 7454 6573 7443 6173 652e 4d61  edactTestCase.Ma
-000005e0: 7053 656e 7369 7469 7665 5661 6c75 6573  pSensitiveValues
-000005f0: 456e 7472 7942 0480 b518 0152 126d 6170  EntryB.....R.map
-00000600: 5365 6e73 6974 6976 6556 616c 7565 7312  SensitiveValues.
-00000610: 710a 146d 6170 5f65 6d62 6564 6465 645f  q..map_embedded_
-00000620: 6f62 6a65 6374 7318 0b20 0328 0b32 3f2e  objects.. .(.2?.
-00000630: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
-00000640: 7631 616c 7068 612e 5265 6461 6374 5465  v1alpha.RedactTe
-00000650: 7374 4361 7365 2e4d 6170 456d 6265 6464  stCase.MapEmbedd
-00000660: 6564 4f62 6a65 6374 7345 6e74 7279 5212  edObjectsEntryR.
-00000670: 6d61 7045 6d62 6564 6465 644f 626a 6563  mapEmbeddedObjec
-00000680: 7473 1a45 0a17 4d61 7053 656e 7369 7469  ts.E..MapSensiti
-00000690: 7665 5661 6c75 6573 456e 7472 7912 100a  veValuesEntry...
-000006a0: 036b 6579 1801 2001 2809 5203 6b65 7912  .key.. .(.R.key.
-000006b0: 140a 0576 616c 7565 1802 2001 2809 5205  ...value.. .(.R.
-000006c0: 7661 6c75 653a 0238 011a 7d0a 174d 6170  value:.8..}..Map
-000006d0: 456d 6265 6464 6564 4f62 6a65 6374 7345  EmbeddedObjectsE
-000006e0: 6e74 7279 1210 0a03 6b65 7918 0120 0128  ntry....key.. .(
-000006f0: 0952 036b 6579 124c 0a05 7661 6c75 6518  .R.key.L..value.
-00000700: 0220 0128 0b32 362e 6b61 736b 6164 612e  . .(.26.kaskada.
-00000710: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
-00000720: 5265 6461 6374 5465 7374 4361 7365 2e45  RedactTestCase.E
-00000730: 6d62 6564 6465 644f 626a 6563 7452 0576  mbeddedObjectR.v
-00000740: 616c 7565 3a02 3801 1a62 0a0e 456d 6265  alue:.8..b..Embe
-00000750: 6464 6564 4f62 6a65 6374 121f 0a0b 7361  ddedObject....sa
-00000760: 6665 5f73 7472 696e 6718 0120 0128 0952  fe_string.. .(.R
-00000770: 0a73 6166 6553 7472 696e 6712 2f0a 1073  .safeString./..s
-00000780: 656e 7369 7469 7665 5f73 7472 696e 6718  ensitive_string.
-00000790: 0220 0128 0942 0480 b518 0152 0f73 656e  . .(.B.....R.sen
-000007a0: 7369 7469 7665 5374 7269 6e67 420d 0a0b  sitiveStringB...
-000007b0: 6f6e 655f 6f66 5f74 6573 744a 0408 0610  one_of_testJ....
-000007c0: 0742 fe01 0a1b 636f 6d2e 6b61 736b 6164  .B....com.kaskad
-000007d0: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
-000007e0: 6142 0e54 6573 7443 6173 6573 5072 6f74  aB.TestCasesProt
-000007f0: 6f50 015a 5167 6974 6875 622e 636f 6d2f  oP.ZQgithub.com/
-00000800: 6b61 736b 6164 612d 6169 2f6b 6173 6b61  kaskada-ai/kaska
-00000810: 6461 2f67 656e 2f70 726f 746f 2f67 6f2f  da/gen/proto/go/
-00000820: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
-00000830: 7631 616c 7068 613b 6b61 736b 6164 6176  v1alpha;kaskadav
-00000840: 3161 6c70 6861 a202 034b 4b58 aa02 174b  1alpha...KKX...K
-00000850: 6173 6b61 6461 2e4b 6173 6b61 6461 2e56  askada.Kaskada.V
-00000860: 3161 6c70 6861 ca02 174b 6173 6b61 6461  1alpha...Kaskada
-00000870: 5c4b 6173 6b61 6461 5c56 3161 6c70 6861  \Kaskada\V1alpha
-00000880: e202 234b 6173 6b61 6461 5c4b 6173 6b61  ..#Kaskada\Kaska
-00000890: 6461 5c56 3161 6c70 6861 5c47 5042 4d65  da\V1alpha\GPBMe
-000008a0: 7461 6461 7461 ea02 194b 6173 6b61 6461  tadata...Kaskada
-000008b0: 3a3a 4b61 736b 6164 613a 3a56 3161 6c70  ::Kaskada::V1alp
-000008c0: 6861 6206 7072 6f74 6f33 da0e 5265 6461  hab.proto3..Reda
-000008d0: 6374 5465 7374 4361 7365 da17 4d61 7053  ctTestCase..MapS
-000008e0: 656e 7369 7469 7665 5661 6c75 6573 456e  ensitiveValuesEn
-000008f0: 7472 79da 174d 6170 456d 6265 6464 6564  try..MapEmbedded
-00000900: 4f62 6a65 6374 7345 6e74 7279 da0e 456d  ObjectsEntry..Em
-00000910: 6265 6464 6564 4f62 6a65 6374 7a26 6b61  beddedObjectz&ka
-00000920: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
-00000930: 616c 7068 612e 7465 7374 5f63 6173 6573  alpha.test_cases
-00000940: 5f70 6232 2902 da0a 4445 5343 5249 5054  _pb2)...DESCRIPT
-00000950: 4f52 da0a 5f5f 6d6f 6475 6c65 5f5f 2905  OR..__module__).
-00000960: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00000970: 0c00 0000 720d 0000 0046 73fe 0000 000a  ....r....Fs.....
-00000980: 1b63 6f6d 2e6b 6173 6b61 6461 2e6b 6173  .com.kaskada.kas
-00000990: 6b61 6461 2e76 3161 6c70 6861 420e 5465  kada.v1alphaB.Te
-000009a0: 7374 4361 7365 7350 726f 746f 5001 5a51  stCasesProtoP.ZQ
-000009b0: 6769 7468 7562 2e63 6f6d 2f6b 6173 6b61  github.com/kaska
-000009c0: 6461 2d61 692f 6b61 736b 6164 612f 6765  da-ai/kaskada/ge
-000009d0: 6e2f 7072 6f74 6f2f 676f 2f6b 6173 6b61  n/proto/go/kaska
-000009e0: 6461 2f6b 6173 6b61 6461 2f76 3161 6c70  da/kaskada/v1alp
-000009f0: 6861 3b6b 6173 6b61 6461 7631 616c 7068  ha;kaskadav1alph
-00000a00: 61a2 0203 4b4b 58aa 0217 4b61 736b 6164  a...KKX...Kaskad
-00000a10: 612e 4b61 736b 6164 612e 5631 616c 7068  a.Kaskada.V1alph
-00000a20: 61ca 0217 4b61 736b 6164 615c 4b61 736b  a...Kaskada\Kask
-00000a30: 6164 615c 5631 616c 7068 61e2 0223 4b61  ada\V1alpha..#Ka
-00000a40: 736b 6164 615c 4b61 736b 6164 615c 5631  skada\Kaskada\V1
-00000a50: 616c 7068 615c 4750 424d 6574 6164 6174  alpha\GPBMetadat
-00000a60: 61ea 0219 4b61 736b 6164 613a 3a4b 6173  a...Kaskada::Kas
-00000a70: 6b61 6461 3a3a 5631 616c 7068 6173 0200  kada::V1alphas..
-00000a80: 0000 3801 da10 7365 6e73 6974 6976 655f  ..8...sensitive_
-00000a90: 7374 7269 6e67 7304 0000 0080 b518 01da  strings.........
-00000aa0: 1472 6f6f 745f 7365 6e73 6974 6976 655f  .root_sensitive_
-00000ab0: 7661 6c75 65da 1972 6570 6561 7465 645f  value..repeated_
-00000ac0: 7365 6e73 6974 6976 655f 7661 6c75 6573  sensitive_values
-00000ad0: da16 6f6e 655f 6f66 5f73 656e 7369 7469  ..one_of_sensiti
-00000ae0: 7665 5f76 616c 7565 da14 6d61 705f 7365  ve_value..map_se
-00000af0: 6e73 6974 6976 655f 7661 6c75 6573 e96d  nsitive_values.m
-00000b00: 0000 0069 fd04 0000 69c0 0300 0069 0504  ...i....i....i..
-00000b10: 0000 6907 0400 0069 8404 0000 6986 0400  ..i....i....i...
-00000b20: 0069 e804 0000 292c da07 5f5f 646f 635f  .i....),..__doc_
-00000b30: 5fda 0862 7569 6c74 696e 73da 0c40 7079  _..builtins..@py
-00000b40: 5f62 7569 6c74 696e 73da 195f 7079 7465  _builtins.._pyte
-00000b50: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
-00000b60: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
-00000b70: 0772 6577 7269 7465 da0a 4070 7974 6573  .rewrite..@pytes
-00000b80: 745f 6172 da0f 676f 6f67 6c65 2e70 726f  t_ar..google.pro
-00000b90: 746f 6275 6672 0200 0000 da0b 5f64 6573  tobufr......_des
-00000ba0: 6372 6970 746f 7272 0300 0000 da10 5f64  criptorr......_d
-00000bb0: 6573 6372 6970 746f 725f 706f 6f6c 7204  escriptor_poolr.
-00000bc0: 0000 00da 085f 6d65 7373 6167 6572 0500  ....._messager..
-00000bd0: 0000 da0b 5f72 6566 6c65 6374 696f 6e72  ...._reflectionr
-00000be0: 0600 0000 da10 5f73 796d 626f 6c5f 6461  ......_symbol_da
-00000bf0: 7461 6261 7365 da07 4465 6661 756c 74da  tabase..Default.
-00000c00: 075f 7379 6d5f 6462 da17 6b61 736b 6164  ._sym_db..kaskad
-00000c10: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
-00000c20: 6172 0700 0000 da30 6b61 736b 6164 615f  ar.....0kaskada_
-00000c30: 646f 745f 6b61 736b 6164 615f 646f 745f  dot_kaskada_dot_
-00000c40: 7631 616c 7068 615f 646f 745f 6f70 7469  v1alpha_dot_opti
-00000c50: 6f6e 735f 5f70 6232 da11 4164 6453 6572  ons__pb2..AddSer
-00000c60: 6961 6c69 7a65 6446 696c 6572 0c00 0000  ializedFiler....
-00000c70: da15 6d65 7373 6167 655f 7479 7065 735f  ..message_types_
-00000c80: 6279 5f6e 616d 65da 0f5f 5245 4441 4354  by_name.._REDACT
-00000c90: 5445 5354 4341 5345 da14 6e65 7374 6564  TESTCASE..nested
-00000ca0: 5f74 7970 6573 5f62 795f 6e61 6d65 da27  _types_by_name.'
-00000cb0: 5f52 4544 4143 5454 4553 5443 4153 455f  _REDACTTESTCASE_
-00000cc0: 4d41 5053 454e 5349 5449 5645 5641 4c55  MAPSENSITIVEVALU
-00000cd0: 4553 454e 5452 59da 275f 5245 4441 4354  ESENTRY.'_REDACT
-00000ce0: 5445 5354 4341 5345 5f4d 4150 454d 4245  TESTCASE_MAPEMBE
-00000cf0: 4444 4544 4f42 4a45 4354 5345 4e54 5259  DDEDOBJECTSENTRY
-00000d00: da1e 5f52 4544 4143 5454 4553 5443 4153  .._REDACTTESTCAS
-00000d10: 455f 454d 4245 4444 4544 4f42 4a45 4354  E_EMBEDDEDOBJECT
-00000d20: da1c 4765 6e65 7261 7465 6450 726f 746f  ..GeneratedProto
-00000d30: 636f 6c4d 6573 7361 6765 5479 7065 da07  colMessageType..
-00000d40: 4d65 7373 6167 6572 0800 0000 da0f 5265  Messager......Re
-00000d50: 6769 7374 6572 4d65 7373 6167 6572 0900  gisterMessager..
-00000d60: 0000 720a 0000 0072 0b00 0000 da12 5f55  ..r....r......_U
-00000d70: 5345 5f43 5f44 4553 4352 4950 544f 5253  SE_C_DESCRIPTORS
-00000d80: da08 5f6f 7074 696f 6e73 da13 5f73 6572  .._options.._ser
-00000d90: 6961 6c69 7a65 645f 6f70 7469 6f6e 73da  ialized_options.
-00000da0: 0e66 6965 6c64 735f 6279 5f6e 616d 65da  .fields_by_name.
-00000db0: 115f 7365 7269 616c 697a 6564 5f73 7461  ._serialized_sta
-00000dc0: 7274 da0f 5f73 6572 6961 6c69 7a65 645f  rt.._serialized_
-00000dd0: 656e 64a9 0072 3500 0000 7235 0000 00fa  end..r5...r5....
-00000de0: 742f 686f 6d65 2f74 6865 7261 706f 6e2f  t/home/therapon/
-00000df0: 5265 706f 732f 4769 7448 7562 2f4b 6173  Repos/GitHub/Kas
-00000e00: 6b61 6461 4149 2f6b 6173 6b61 6461 2f72  kadaAI/kaskada/r
-00000e10: 656c 6561 7369 6e67 2f63 6c69 656e 7473  eleasing/clients
-00000e20: 2f70 7974 686f 6e2f 7372 632f 6b61 736b  /python/src/kask
-00000e30: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
-00000e40: 7068 612f 7465 7374 5f63 6173 6573 5f70  pha/test_cases_p
-00000e50: 6232 2e70 79da 083c 6d6f 6475 6c65 3e01  b2.py..<module>.
-00000e60: 0000 0073 7600 0000 0403 2601 0c01 0c01  ...sv.....&.....
-00000e70: 0c01 0c01 0803 0c03 0e03 0a04 0a01 0a01  ................
-00000e80: 0a01 0c01 0c02 0201 0201 06fe 0c07 0201  ................
-00000e90: 0201 06fe 0c07 0201 0201 06fe 0206 0201  ................
-00000ea0: 08e9 0a1a 0c01 0c01 0c01 0c02 0602 0601  ................
-00000eb0: 0601 0601 0601 0601 0c01 0c01 0c01 0c01  ................
-00000ec0: 0c01 0c01 0c01 0c01 0c01 0c01 0601 0601  ................
-00000ed0: 0601 0601 0601 0601 0601 0a01 04e7       ..............
+00000230: 5f2b 6402 5300 2922 7a1f 4765 6e65 7261  _+d.S.)"z.Genera
+00000240: 7465 6420 7072 6f74 6f63 6f6c 2062 7566  ted protocol buf
+00000250: 6665 7220 636f 6465 2ee9 0000 0000 4e29  fer code......N)
+00000260: 01da 0a64 6573 6372 6970 746f 7229 01da  ...descriptor)..
+00000270: 0f64 6573 6372 6970 746f 725f 706f 6f6c  .descriptor_pool
+00000280: 2901 da07 6d65 7373 6167 6529 01da 0a72  )...message)...r
+00000290: 6566 6c65 6374 696f 6e29 01da 0f73 796d  eflection)...sym
+000002a0: 626f 6c5f 6461 7461 6261 7365 2901 da0b  bol_database)...
+000002b0: 6f70 7469 6f6e 735f 7062 3273 0606 0000  options_pb2s....
+000002c0: 0a28 6b61 736b 6164 612f 6b61 736b 6164  .(kaskada/kaskad
+000002d0: 612f 7631 616c 7068 612f 7465 7374 5f63  a/v1alpha/test_c
+000002e0: 6173 6573 2e70 726f 746f 1217 6b61 736b  ases.proto..kask
+000002f0: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
+00000300: 7068 611a 256b 6173 6b61 6461 2f6b 6173  pha.%kaskada/kas
+00000310: 6b61 6461 2f76 3161 6c70 6861 2f6f 7074  kada/v1alpha/opt
+00000320: 696f 6e73 2e70 726f 746f 2290 090a 0e52  ions.proto"....R
+00000330: 6564 6163 7454 6573 7443 6173 6512 260a  edactTestCase.&.
+00000340: 0f72 6f6f 745f 7361 6665 5f76 616c 7565  .root_safe_value
+00000350: 1801 2001 2809 520d 726f 6f74 5361 6665  .. .(.R.rootSafe
+00000360: 5661 6c75 6512 360a 1472 6f6f 745f 7365  Value.6..root_se
+00000370: 6e73 6974 6976 655f 7661 6c75 6518 0220  nsitive_value.. 
+00000380: 0128 0942 0480 b518 0152 1272 6f6f 7453  .(.B.....R.rootS
+00000390: 656e 7369 7469 7665 5661 6c75 6512 400a  ensitiveValue.@.
+000003a0: 1972 6570 6561 7465 645f 7365 6e73 6974  .repeated_sensit
+000003b0: 6976 655f 7661 6c75 6573 1803 2003 2809  ive_values.. .(.
+000003c0: 4204 80b5 1801 5217 7265 7065 6174 6564  B.....R.repeated
+000003d0: 5365 6e73 6974 6976 6556 616c 7565 7312  SensitiveValues.
+000003e0: 680a 1472 6f6f 745f 656d 6265 6464 6564  h..root_embedded
+000003f0: 5f6f 626a 6563 7418 0420 0128 0b32 362e  _object.. .(.26.
+00000400: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000410: 7631 616c 7068 612e 5265 6461 6374 5465  v1alpha.RedactTe
+00000420: 7374 4361 7365 2e45 6d62 6564 6465 644f  stCase.EmbeddedO
+00000430: 626a 6563 7452 1272 6f6f 7445 6d62 6564  bjectR.rootEmbed
+00000440: 6465 644f 626a 6563 7412 700a 1872 6570  dedObject.p..rep
+00000450: 6561 7465 645f 656d 6265 6464 6564 5f6f  eated_embedded_o
+00000460: 626a 6563 7418 0520 0328 0b32 362e 6b61  bject.. .(.26.ka
+00000470: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
+00000480: 616c 7068 612e 5265 6461 6374 5465 7374  alpha.RedactTest
+00000490: 4361 7365 2e45 6d62 6564 6465 644f 626a  Case.EmbeddedObj
+000004a0: 6563 7452 1672 6570 6561 7465 6445 6d62  ectR.repeatedEmb
+000004b0: 6564 6465 644f 626a 6563 7412 2b0a 116f  eddedObject.+..o
+000004c0: 6e65 5f6f 665f 7361 6665 5f76 616c 7565  ne_of_safe_value
+000004d0: 1807 2001 2809 4800 520e 6f6e 654f 6653  .. .(.H.R.oneOfS
+000004e0: 6166 6556 616c 7565 123b 0a16 6f6e 655f  afeValue.;..one_
+000004f0: 6f66 5f73 656e 7369 7469 7665 5f76 616c  of_sensitive_val
+00000500: 7565 1808 2001 2809 4204 80b5 1801 4800  ue.. .(.B.....H.
+00000510: 5213 6f6e 654f 6653 656e 7369 7469 7665  R.oneOfSensitive
+00000520: 5661 6c75 6512 6b0a 156f 6e65 5f6f 665f  Value.k..one_of_
+00000530: 656d 6265 6464 6564 5f76 616c 7565 1809  embedded_value..
+00000540: 2001 280b 3236 2e6b 6173 6b61 6461 2e6b   .(.26.kaskada.k
+00000550: 6173 6b61 6461 2e76 3161 6c70 6861 2e52  askada.v1alpha.R
+00000560: 6564 6163 7454 6573 7443 6173 652e 456d  edactTestCase.Em
+00000570: 6265 6464 6564 4f62 6a65 6374 4800 5212  beddedObjectH.R.
+00000580: 6f6e 654f 6645 6d62 6564 6465 6456 616c  oneOfEmbeddedVal
+00000590: 7565 1277 0a14 6d61 705f 7365 6e73 6974  ue.w..map_sensit
+000005a0: 6976 655f 7661 6c75 6573 180a 2003 280b  ive_values.. .(.
+000005b0: 323f 2e6b 6173 6b61 6461 2e6b 6173 6b61  2?.kaskada.kaska
+000005c0: 6461 2e76 3161 6c70 6861 2e52 6564 6163  da.v1alpha.Redac
+000005d0: 7454 6573 7443 6173 652e 4d61 7053 656e  tTestCase.MapSen
+000005e0: 7369 7469 7665 5661 6c75 6573 456e 7472  sitiveValuesEntr
+000005f0: 7942 0480 b518 0152 126d 6170 5365 6e73  yB.....R.mapSens
+00000600: 6974 6976 6556 616c 7565 7312 710a 146d  itiveValues.q..m
+00000610: 6170 5f65 6d62 6564 6465 645f 6f62 6a65  ap_embedded_obje
+00000620: 6374 7318 0b20 0328 0b32 3f2e 6b61 736b  cts.. .(.2?.kask
+00000630: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
+00000640: 7068 612e 5265 6461 6374 5465 7374 4361  pha.RedactTestCa
+00000650: 7365 2e4d 6170 456d 6265 6464 6564 4f62  se.MapEmbeddedOb
+00000660: 6a65 6374 7345 6e74 7279 5212 6d61 7045  jectsEntryR.mapE
+00000670: 6d62 6564 6465 644f 626a 6563 7473 1a45  mbeddedObjects.E
+00000680: 0a17 4d61 7053 656e 7369 7469 7665 5661  ..MapSensitiveVa
+00000690: 6c75 6573 456e 7472 7912 100a 036b 6579  luesEntry....key
+000006a0: 1801 2001 2809 5203 6b65 7912 140a 0576  .. .(.R.key....v
+000006b0: 616c 7565 1802 2001 2809 5205 7661 6c75  alue.. .(.R.valu
+000006c0: 653a 0238 011a 7d0a 174d 6170 456d 6265  e:.8..}..MapEmbe
+000006d0: 6464 6564 4f62 6a65 6374 7345 6e74 7279  ddedObjectsEntry
+000006e0: 1210 0a03 6b65 7918 0120 0128 0952 036b  ....key.. .(.R.k
+000006f0: 6579 124c 0a05 7661 6c75 6518 0220 0128  ey.L..value.. .(
+00000700: 0b32 362e 6b61 736b 6164 612e 6b61 736b  .26.kaskada.kask
+00000710: 6164 612e 7631 616c 7068 612e 5265 6461  ada.v1alpha.Reda
+00000720: 6374 5465 7374 4361 7365 2e45 6d62 6564  ctTestCase.Embed
+00000730: 6465 644f 626a 6563 7452 0576 616c 7565  dedObjectR.value
+00000740: 3a02 3801 1a62 0a0e 456d 6265 6464 6564  :.8..b..Embedded
+00000750: 4f62 6a65 6374 121f 0a0b 7361 6665 5f73  Object....safe_s
+00000760: 7472 696e 6718 0120 0128 0952 0a73 6166  tring.. .(.R.saf
+00000770: 6553 7472 696e 6712 2f0a 1073 656e 7369  eString./..sensi
+00000780: 7469 7665 5f73 7472 696e 6718 0220 0128  tive_string.. .(
+00000790: 0942 0480 b518 0152 0f73 656e 7369 7469  .B.....R.sensiti
+000007a0: 7665 5374 7269 6e67 420d 0a0b 6f6e 655f  veStringB...one_
+000007b0: 6f66 5f74 6573 744a 0408 0610 0742 fe01  of_testJ.....B..
+000007c0: 0a1b 636f 6d2e 6b61 736b 6164 612e 6b61  ..com.kaskada.ka
+000007d0: 736b 6164 612e 7631 616c 7068 6142 0e54  skada.v1alphaB.T
+000007e0: 6573 7443 6173 6573 5072 6f74 6f50 015a  estCasesProtoP.Z
+000007f0: 5167 6974 6875 622e 636f 6d2f 6b61 736b  Qgithub.com/kask
+00000800: 6164 612d 6169 2f6b 6173 6b61 6461 2f67  ada-ai/kaskada/g
+00000810: 656e 2f70 726f 746f 2f67 6f2f 6b61 736b  en/proto/go/kask
+00000820: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
+00000830: 7068 613b 6b61 736b 6164 6176 3161 6c70  pha;kaskadav1alp
+00000840: 6861 a202 034b 4b58 aa02 174b 6173 6b61  ha...KKX...Kaska
+00000850: 6461 2e4b 6173 6b61 6461 2e56 3161 6c70  da.Kaskada.V1alp
+00000860: 6861 ca02 174b 6173 6b61 6461 5c4b 6173  ha...Kaskada\Kas
+00000870: 6b61 6461 5c56 3161 6c70 6861 e202 234b  kada\V1alpha..#K
+00000880: 6173 6b61 6461 5c4b 6173 6b61 6461 5c56  askada\Kaskada\V
+00000890: 3161 6c70 6861 5c47 5042 4d65 7461 6461  1alpha\GPBMetada
+000008a0: 7461 ea02 194b 6173 6b61 6461 3a3a 4b61  ta...Kaskada::Ka
+000008b0: 736b 6164 613a 3a56 3161 6c70 6861 6206  skada::V1alphab.
+000008c0: 7072 6f74 6f33 da0e 5265 6461 6374 5465  proto3..RedactTe
+000008d0: 7374 4361 7365 da17 4d61 7053 656e 7369  stCase..MapSensi
+000008e0: 7469 7665 5661 6c75 6573 456e 7472 79da  tiveValuesEntry.
+000008f0: 174d 6170 456d 6265 6464 6564 4f62 6a65  .MapEmbeddedObje
+00000900: 6374 7345 6e74 7279 da0e 456d 6265 6464  ctsEntry..Embedd
+00000910: 6564 4f62 6a65 6374 7a26 6b61 736b 6164  edObjectz&kaskad
+00000920: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00000930: 612e 7465 7374 5f63 6173 6573 5f70 6232  a.test_cases_pb2
+00000940: 2902 da0a 4445 5343 5249 5054 4f52 da0a  )...DESCRIPTOR..
+00000950: 5f5f 6d6f 6475 6c65 5f5f 2905 7209 0000  __module__).r...
+00000960: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00000970: 720d 0000 0046 73fe 0000 000a 1b63 6f6d  r....Fs......com
+00000980: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00000990: 2e76 3161 6c70 6861 420e 5465 7374 4361  .v1alphaB.TestCa
+000009a0: 7365 7350 726f 746f 5001 5a51 6769 7468  sesProtoP.ZQgith
+000009b0: 7562 2e63 6f6d 2f6b 6173 6b61 6461 2d61  ub.com/kaskada-a
+000009c0: 692f 6b61 736b 6164 612f 6765 6e2f 7072  i/kaskada/gen/pr
+000009d0: 6f74 6f2f 676f 2f6b 6173 6b61 6461 2f6b  oto/go/kaskada/k
+000009e0: 6173 6b61 6461 2f76 3161 6c70 6861 3b6b  askada/v1alpha;k
+000009f0: 6173 6b61 6461 7631 616c 7068 61a2 0203  askadav1alpha...
+00000a00: 4b4b 58aa 0217 4b61 736b 6164 612e 4b61  KKX...Kaskada.Ka
+00000a10: 736b 6164 612e 5631 616c 7068 61ca 0217  skada.V1alpha...
+00000a20: 4b61 736b 6164 615c 4b61 736b 6164 615c  Kaskada\Kaskada\
+00000a30: 5631 616c 7068 61e2 0223 4b61 736b 6164  V1alpha..#Kaskad
+00000a40: 615c 4b61 736b 6164 615c 5631 616c 7068  a\Kaskada\V1alph
+00000a50: 615c 4750 424d 6574 6164 6174 61ea 0219  a\GPBMetadata...
+00000a60: 4b61 736b 6164 613a 3a4b 6173 6b61 6461  Kaskada::Kaskada
+00000a70: 3a3a 5631 616c 7068 6173 0200 0000 3801  ::V1alphas....8.
+00000a80: 5a10 7365 6e73 6974 6976 655f 7374 7269  Z.sensitive_stri
+00000a90: 6e67 7304 0000 0080 b518 015a 1472 6f6f  ngs........Z.roo
+00000aa0: 745f 7365 6e73 6974 6976 655f 7661 6c75  t_sensitive_valu
+00000ab0: 655a 1972 6570 6561 7465 645f 7365 6e73  eZ.repeated_sens
+00000ac0: 6974 6976 655f 7661 6c75 6573 5a16 6f6e  itive_valuesZ.on
+00000ad0: 655f 6f66 5f73 656e 7369 7469 7665 5f76  e_of_sensitive_v
+00000ae0: 616c 7565 5a14 6d61 705f 7365 6e73 6974  alueZ.map_sensit
+00000af0: 6976 655f 7661 6c75 6573 e96d 0000 0069  ive_values.m...i
+00000b00: fd04 0000 69c0 0300 0069 0504 0000 6907  ....i....i....i.
+00000b10: 0400 0069 8404 0000 6986 0400 0069 e804  ...i....i....i..
+00000b20: 0000 292c da07 5f5f 646f 635f 5fda 0862  ..),..__doc__..b
+00000b30: 7569 6c74 696e 73da 0c40 7079 5f62 7569  uiltins..@py_bui
+00000b40: 6c74 696e 73da 195f 7079 7465 7374 2e61  ltins.._pytest.a
+00000b50: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
+00000b60: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
+00000b70: 7269 7465 da0a 4070 7974 6573 745f 6172  rite..@pytest_ar
+00000b80: 5a0f 676f 6f67 6c65 2e70 726f 746f 6275  Z.google.protobu
+00000b90: 6672 0200 0000 5a0b 5f64 6573 6372 6970  fr....Z._descrip
+00000ba0: 746f 7272 0300 0000 5a10 5f64 6573 6372  torr....Z._descr
+00000bb0: 6970 746f 725f 706f 6f6c 7204 0000 00da  iptor_poolr.....
+00000bc0: 085f 6d65 7373 6167 6572 0500 0000 5a0b  ._messager....Z.
+00000bd0: 5f72 6566 6c65 6374 696f 6e72 0600 0000  _reflectionr....
+00000be0: 5a10 5f73 796d 626f 6c5f 6461 7461 6261  Z._symbol_databa
+00000bf0: 7365 5a07 4465 6661 756c 745a 075f 7379  seZ.DefaultZ._sy
+00000c00: 6d5f 6462 5a17 6b61 736b 6164 612e 6b61  m_dbZ.kaskada.ka
+00000c10: 736b 6164 612e 7631 616c 7068 6172 0700  skada.v1alphar..
+00000c20: 0000 5a30 6b61 736b 6164 615f 646f 745f  ..Z0kaskada_dot_
+00000c30: 6b61 736b 6164 615f 646f 745f 7631 616c  kaskada_dot_v1al
+00000c40: 7068 615f 646f 745f 6f70 7469 6f6e 735f  pha_dot_options_
+00000c50: 5f70 6232 5a11 4164 6453 6572 6961 6c69  _pb2Z.AddSeriali
+00000c60: 7a65 6446 696c 6572 0c00 0000 5a15 6d65  zedFiler....Z.me
+00000c70: 7373 6167 655f 7479 7065 735f 6279 5f6e  ssage_types_by_n
+00000c80: 616d 655a 0f5f 5245 4441 4354 5445 5354  ameZ._REDACTTEST
+00000c90: 4341 5345 5a14 6e65 7374 6564 5f74 7970  CASEZ.nested_typ
+00000ca0: 6573 5f62 795f 6e61 6d65 5a27 5f52 4544  es_by_nameZ'_RED
+00000cb0: 4143 5454 4553 5443 4153 455f 4d41 5053  ACTTESTCASE_MAPS
+00000cc0: 454e 5349 5449 5645 5641 4c55 4553 454e  ENSITIVEVALUESEN
+00000cd0: 5452 595a 275f 5245 4441 4354 5445 5354  TRYZ'_REDACTTEST
+00000ce0: 4341 5345 5f4d 4150 454d 4245 4444 4544  CASE_MAPEMBEDDED
+00000cf0: 4f42 4a45 4354 5345 4e54 5259 5a1e 5f52  OBJECTSENTRYZ._R
+00000d00: 4544 4143 5454 4553 5443 4153 455f 454d  EDACTTESTCASE_EM
+00000d10: 4245 4444 4544 4f42 4a45 4354 5a1c 4765  BEDDEDOBJECTZ.Ge
+00000d20: 6e65 7261 7465 6450 726f 746f 636f 6c4d  neratedProtocolM
+00000d30: 6573 7361 6765 5479 7065 da07 4d65 7373  essageType..Mess
+00000d40: 6167 6572 0800 0000 5a0f 5265 6769 7374  ager....Z.Regist
+00000d50: 6572 4d65 7373 6167 6572 0900 0000 720a  erMessager....r.
+00000d60: 0000 0072 0b00 0000 5a12 5f55 5345 5f43  ...r....Z._USE_C
+00000d70: 5f44 4553 4352 4950 544f 5253 da08 5f6f  _DESCRIPTORS.._o
+00000d80: 7074 696f 6e73 5a13 5f73 6572 6961 6c69  ptionsZ._seriali
+00000d90: 7a65 645f 6f70 7469 6f6e 735a 0e66 6965  zed_optionsZ.fie
+00000da0: 6c64 735f 6279 5f6e 616d 655a 115f 7365  lds_by_nameZ._se
+00000db0: 7269 616c 697a 6564 5f73 7461 7274 5a0f  rialized_startZ.
+00000dc0: 5f73 6572 6961 6c69 7a65 645f 656e 64a9  _serialized_end.
+00000dd0: 0072 1900 0000 7219 0000 00fa 322f 7372  .r....r.....2/sr
+00000de0: 632f 7372 632f 6b61 736b 6164 612f 6b61  c/src/kaskada/ka
+00000df0: 736b 6164 612f 7631 616c 7068 612f 7465  skada/v1alpha/te
+00000e00: 7374 5f63 6173 6573 5f70 6232 2e70 79da  st_cases_pb2.py.
+00000e10: 083c 6d6f 6475 6c65 3e04 0000 0073 7200  .<module>....sr.
+00000e20: 0000 0401 2601 0c01 0c01 0c01 0c03 0803  ....&...........
+00000e30: 0c03 0e04 0a01 0a01 0a01 0a01 0c02 0c01  ................
+00000e40: 0201 02fe 0607 0c01 0201 02fe 0607 0c01  ................
+00000e50: 0201 02fe 0606 0201 02e9 081a 0a01 0c01  ................
+00000e60: 0c01 0c02 0c02 0601 0601 0601 0601 0601  ................
+00000e70: 0601 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000e80: 0c01 0c01 0c01 0601 0601 0601 0601 0601  ................
+00000e90: 0601 0601                                ....
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/view_service_pb2.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/view_service_pb2.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 11387 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 7b2c 0000  o.........5d{,..
+00000000: 610d 0d0a 0000 0000 2038 4164 7b2c 0000  a....... 8Ad{,..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 f803 0000 6400  .....@...s....d.
+00000020: 0007 0000 0040 0000 0073 f403 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c01 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c01 6d0a 5a0b 0100 650b  ..d.d.l.m.Z...e.
 00000070: a00c a100 5a0d 6401 6407 6c0e 6d0f 5a10  ....Z.d.d.l.m.Z.
 00000080: 0100 6401 6408 6c0e 6d11 5a12 0100 6401  ..d.d.l.m.Z...d.
 00000090: 6409 6c13 6d14 5a15 0100 6401 640a 6c13  d.l.m.Z...d.d.l.
@@ -31,16 +31,16 @@
 000001e0: 652f a101 0100 6509 a027 6413 6507 6a28  e/....e..'d.e.j(
 000001f0: 6601 6524 6416 6417 9c02 a103 5a30 650d  f.e$d.d.....Z0e.
 00000200: a02a 6530 a101 0100 6509 a027 6414 6507  .*e0....e..'d.e.
 00000210: 6a28 6601 6525 6416 6417 9c02 a103 5a31  j(f.e%d.d.....Z1
 00000220: 650d a02a 6531 a101 0100 6509 a027 6415  e..*e1....e..'d.
 00000230: 6507 6a28 6601 6526 6416 6417 9c02 a103  e.j(f.e&d.d.....
 00000240: 5a32 650d a02a 6532 a101 0100 651c 6a33  Z2e..*e2....e.j3
-00000250: 6418 1900 5a34 6503 6a35 6419 6b02 9001  d...Z4e.j5d.k...
-00000260: 72fa 641a 651c 5f36 641b 651c 5f37 641a  r.d.e._6d.e._7d.
+00000250: 6418 1900 5a34 6503 6a35 6419 6b02 9003  d...Z4e.j5d.k...
+00000260: 72f0 641a 651c 5f36 641b 651c 5f37 641a  r.d.e._6d.e._7d.
 00000270: 651e 6a38 641c 1900 5f36 641d 651e 6a38  e.j8d..._6d.e.j8
 00000280: 641c 1900 5f37 641a 651e 6a38 641e 1900  d..._7d.e.j8d...
 00000290: 5f36 641f 651e 6a38 641e 1900 5f37 641a  _6d.e.j8d..._7d.
 000002a0: 651e 6a38 6420 1900 5f36 641f 651e 6a38  e.j8d .._6d.e.j8
 000002b0: 6420 1900 5f37 641a 651e 6a38 6421 1900  d .._7d.e.j8d!..
 000002c0: 5f36 641d 651e 6a38 6421 1900 5f37 641a  _6d.e.j8d!.._7d.
 000002d0: 651e 6a38 6422 1900 5f36 641d 651e 6a38  e.j8d".._6d.e.j8
@@ -60,303 +60,298 @@
 000003b0: 5f3b 6431 651f 5f3a 6432 651f 5f3b 6433  _;d1e._:d2e._;d3
 000003c0: 6520 5f3a 6434 6520 5f3b 6435 6521 5f3a  e _:d4e _;d5e!_:
 000003d0: 6436 6521 5f3b 6437 6522 5f3a 6438 6522  d6e!_;d7e"_:d8e"
 000003e0: 5f3b 6439 6523 5f3a 643a 6523 5f3b 643b  _;d9e#_:d:e#_;d;
 000003f0: 6524 5f3a 643c 6524 5f3b 643d 6525 5f3a  e$_:d<e$_;d=e%_:
 00000400: 643e 6525 5f3b 643f 6526 5f3a 6440 6526  d>e%_;d?e&_:d@e&
 00000410: 5f3b 6441 6534 5f3a 6442 6534 5f3b 641a  _;dAe4_:dBe4_;d.
-00000420: 5300 641a 5300 2943 7a1f 4765 6e65 7261  S.d.S.)Cz.Genera
-00000430: 7465 6420 7072 6f74 6f63 6f6c 2062 7566  ted protocol buf
-00000440: 6665 7220 636f 6465 2ee9 0000 0000 2901  fer code......).
-00000450: da0a 6465 7363 7269 7074 6f72 2901 da0f  ..descriptor)...
-00000460: 6465 7363 7269 7074 6f72 5f70 6f6f 6c29  descriptor_pool)
-00000470: 01da 076d 6573 7361 6765 2901 da0a 7265  ...message)...re
-00000480: 666c 6563 7469 6f6e 2901 da0f 7379 6d62  flection)...symb
-00000490: 6f6c 5f64 6174 6162 6173 6529 01da 0f61  ol_database)...a
-000004a0: 6e6e 6f74 6174 696f 6e73 5f70 6232 2901  nnotations_pb2).
-000004b0: da12 6669 656c 645f 6265 6861 7669 6f72  ..field_behavior
-000004c0: 5f70 6232 2901 da0a 636f 6d6d 6f6e 5f70  _pb2)...common_p
-000004d0: 6232 2901 da0a 7363 6865 6d61 5f70 6232  b2)...schema_pb2
-000004e0: 2901 da0c 7661 6c69 6461 7465 5f70 6232  )...validate_pb2
-000004f0: 7325 0900 000a 2a6b 6173 6b61 6461 2f6b  s%....*kaskada/k
-00000500: 6173 6b61 6461 2f76 3161 6c70 6861 2f76  askada/v1alpha/v
-00000510: 6965 775f 7365 7276 6963 652e 7072 6f74  iew_service.prot
-00000520: 6f12 176b 6173 6b61 6461 2e6b 6173 6b61  o..kaskada.kaska
-00000530: 6461 2e76 3161 6c70 6861 1a1c 676f 6f67  da.v1alpha..goog
-00000540: 6c65 2f61 7069 2f61 6e6e 6f74 6174 696f  le/api/annotatio
-00000550: 6e73 2e70 726f 746f 1a1f 676f 6f67 6c65  ns.proto..google
-00000560: 2f61 7069 2f66 6965 6c64 5f62 6568 6176  /api/field_behav
-00000570: 696f 722e 7072 6f74 6f1a 246b 6173 6b61  ior.proto.$kaska
-00000580: 6461 2f6b 6173 6b61 6461 2f76 3161 6c70  da/kaskada/v1alp
-00000590: 6861 2f63 6f6d 6d6f 6e2e 7072 6f74 6f1a  ha/common.proto.
-000005a0: 246b 6173 6b61 6461 2f6b 6173 6b61 6461  $kaskada/kaskada
-000005b0: 2f76 3161 6c70 6861 2f73 6368 656d 612e  /v1alpha/schema.
-000005c0: 7072 6f74 6f1a 1776 616c 6964 6174 652f  proto..validate/
-000005d0: 7661 6c69 6461 7465 2e70 726f 746f 2280  validate.proto".
-000005e0: 020a 0456 6965 7712 1c0a 0776 6965 775f  ...View....view_
-000005f0: 6964 1801 2001 2809 4203 e041 0352 0676  id.. .(.B..A.R.v
-00000600: 6965 7749 6412 240a 0976 6965 775f 6e61  iewId.$..view_na
-00000610: 6d65 1802 2001 2809 4207 fa42 0472 0210  me.. .(.B..B.r..
-00000620: 0152 0876 6965 774e 616d 6512 270a 0a65  .R.viewName.'..e
-00000630: 7870 7265 7373 696f 6e18 0320 0128 0942  xpression.. .(.B
-00000640: 07fa 4204 7202 1001 520a 6578 7072 6573  ..B.r...R.expres
-00000650: 7369 6f6e 1247 0a0b 7265 7375 6c74 5f74  sion.G..result_t
-00000660: 7970 6518 0720 0128 0b32 212e 6b61 736b  ype.. .(.2!.kask
-00000670: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-00000680: 7068 612e 4461 7461 5479 7065 4203 e041  pha.DataTypeB..A
-00000690: 0352 0a72 6573 756c 7454 7970 6512 420a  .R.resultType.B.
-000006a0: 0861 6e61 6c79 7369 7318 0820 0128 0b32  .analysis.. .(.2
-000006b0: 212e 6b61 736b 6164 612e 6b61 736b 6164  !.kaskada.kaskad
-000006c0: 612e 7631 616c 7068 612e 416e 616c 7973  a.v1alpha.Analys
-000006d0: 6973 4203 e041 0352 0861 6e61 6c79 7369  isB..A.R.analysi
-000006e0: 7322 720a 104c 6973 7456 6965 7773 5265  s"r..ListViewsRe
-000006f0: 7175 6573 7412 160a 0673 6561 7263 6818  quest....search.
-00000700: 0120 0128 0952 0673 6561 7263 6812 270a  . .(.R.search.'.
-00000710: 0970 6167 655f 7369 7a65 1802 2001 2805  .page_size.. .(.
-00000720: 420a fa42 071a 0518 e807 2800 5208 7061  B..B......(.R.pa
-00000730: 6765 5369 7a65 121d 0a0a 7061 6765 5f74  geSize....page_t
-00000740: 6f6b 656e 1803 2001 2809 5209 7061 6765  oken.. .(.R.page
-00000750: 546f 6b65 6e22 c201 0a11 4c69 7374 5669  Token"....ListVi
-00000760: 6577 7352 6573 706f 6e73 6512 330a 0576  ewsResponse.3..v
-00000770: 6965 7773 1801 2003 280b 321d 2e6b 6173  iews.. .(.2..kas
-00000780: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-00000790: 6c70 6861 2e56 6965 7752 0576 6965 7773  lpha.ViewR.views
-000007a0: 1250 0a0f 7265 7175 6573 745f 6465 7461  .P..request_deta
-000007b0: 696c 7318 0220 0128 0b32 272e 6b61 736b  ils.. .(.2'.kask
-000007c0: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-000007d0: 7068 612e 5265 7175 6573 7444 6574 6169  pha.RequestDetai
-000007e0: 6c73 520e 7265 7175 6573 7444 6574 6169  lsR.requestDetai
-000007f0: 6c73 1226 0a0f 6e65 7874 5f70 6167 655f  ls.&..next_page_
-00000800: 746f 6b65 6e18 0320 0128 0952 0d6e 6578  token.. .(.R.nex
-00000810: 7450 6167 6554 6f6b 656e 2236 0a0e 4765  tPageToken"6..Ge
-00000820: 7456 6965 7752 6571 7565 7374 1224 0a09  tViewRequest.$..
-00000830: 7669 6577 5f6e 616d 6518 0120 0128 0942  view_name.. .(.B
-00000840: 07fa 4204 7202 1001 5208 7669 6577 4e61  ..B.r...R.viewNa
-00000850: 6d65 2296 010a 0f47 6574 5669 6577 5265  me"....GetViewRe
-00000860: 7370 6f6e 7365 1231 0a04 7669 6577 1801  sponse.1..view..
-00000870: 2001 280b 321d 2e6b 6173 6b61 6461 2e6b   .(.2..kaskada.k
-00000880: 6173 6b61 6461 2e76 3161 6c70 6861 2e56  askada.v1alpha.V
-00000890: 6965 7752 0476 6965 7712 500a 0f72 6571  iewR.view.P..req
-000008a0: 7565 7374 5f64 6574 6169 6c73 1802 2001  uest_details.. .
-000008b0: 280b 3227 2e6b 6173 6b61 6461 2e6b 6173  (.2'.kaskada.kas
-000008c0: 6b61 6461 2e76 3161 6c70 6861 2e52 6571  kada.v1alpha.Req
-000008d0: 7565 7374 4465 7461 696c 7352 0e72 6571  uestDetailsR.req
-000008e0: 7565 7374 4465 7461 696c 7322 690a 1143  uestDetails"i..C
-000008f0: 7265 6174 6556 6965 7752 6571 7565 7374  reateViewRequest
-00000900: 123b 0a04 7669 6577 1801 2001 280b 321d  .;..view.. .(.2.
-00000910: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
-00000920: 2e76 3161 6c70 6861 2e56 6965 7742 08fa  .v1alpha.ViewB..
-00000930: 4205 8a01 0210 0152 0476 6965 7712 170a  B......R.view...
-00000940: 0764 7279 5f72 756e 1802 2001 2808 5206  .dry_run.. .(.R.
-00000950: 6472 7952 756e 22d8 010a 1243 7265 6174  dryRun"....Creat
-00000960: 6556 6965 7752 6573 706f 6e73 6512 310a  eViewResponse.1.
-00000970: 0476 6965 7718 0120 0128 0b32 1d2e 6b61  .view.. .(.2..ka
-00000980: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
-00000990: 616c 7068 612e 5669 6577 5204 7669 6577  alpha.ViewR.view
-000009a0: 1250 0a0f 7265 7175 6573 745f 6465 7461  .P..request_deta
-000009b0: 696c 7318 0220 0128 0b32 272e 6b61 736b  ils.. .(.2'.kask
-000009c0: 6164 612e 6b61 736b 6164 612e 7631 616c  ada.kaskada.v1al
-000009d0: 7068 612e 5265 7175 6573 7444 6574 6169  pha.RequestDetai
-000009e0: 6c73 520e 7265 7175 6573 7444 6574 6169  lsR.requestDetai
-000009f0: 6c73 123d 0a08 616e 616c 7973 6973 1803  ls.=..analysis..
-00000a00: 2001 280b 3221 2e6b 6173 6b61 6461 2e6b   .(.2!.kaskada.k
-00000a10: 6173 6b61 6461 2e76 3161 6c70 6861 2e41  askada.v1alpha.A
-00000a20: 6e61 6c79 7369 7352 0861 6e61 6c79 7369  nalysisR.analysi
-00000a30: 7322 4f0a 1144 656c 6574 6556 6965 7752  s"O..DeleteViewR
-00000a40: 6571 7565 7374 1224 0a09 7669 6577 5f6e  equest.$..view_n
-00000a50: 616d 6518 0120 0128 0942 07fa 4204 7202  ame.. .(.B..B.r.
-00000a60: 1001 5208 7669 6577 4e61 6d65 1214 0a05  ..R.viewName....
-00000a70: 666f 7263 6518 0220 0128 0852 0566 6f72  force.. .(.R.for
-00000a80: 6365 2266 0a12 4465 6c65 7465 5669 6577  ce"f..DeleteView
-00000a90: 5265 7370 6f6e 7365 1250 0a0f 7265 7175  Response.P..requ
-00000aa0: 6573 745f 6465 7461 696c 7318 0120 0128  est_details.. .(
-00000ab0: 0b32 272e 6b61 736b 6164 612e 6b61 736b  .2'.kaskada.kask
-00000ac0: 6164 612e 7631 616c 7068 612e 5265 7175  ada.v1alpha.Requ
-00000ad0: 6573 7444 6574 6169 6c73 520e 7265 7175  estDetailsR.requ
-00000ae0: 6573 7444 6574 6169 6c73 32a2 040a 0b56  estDetails2....V
-00000af0: 6965 7753 6572 7669 6365 127a 0a09 4c69  iewService.z..Li
-00000b00: 7374 5669 6577 7312 292e 6b61 736b 6164  stViews.).kaskad
-00000b10: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
-00000b20: 612e 4c69 7374 5669 6577 7352 6571 7565  a.ListViewsReque
-00000b30: 7374 1a2a 2e6b 6173 6b61 6461 2e6b 6173  st.*.kaskada.kas
-00000b40: 6b61 6461 2e76 3161 6c70 6861 2e4c 6973  kada.v1alpha.Lis
-00000b50: 7456 6965 7773 5265 7370 6f6e 7365 2216  tViewsResponse".
-00000b60: 82d3 e493 0210 120e 2f76 3161 6c70 6861  ......../v1alpha
-00000b70: 2f76 6965 7773 1282 010a 0747 6574 5669  /views.....GetVi
-00000b80: 6577 1227 2e6b 6173 6b61 6461 2e6b 6173  ew.'.kaskada.kas
-00000b90: 6b61 6461 2e76 3161 6c70 6861 2e47 6574  kada.v1alpha.Get
-00000ba0: 5669 6577 5265 7175 6573 741a 282e 6b61  ViewRequest.(.ka
-00000bb0: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
-00000bc0: 616c 7068 612e 4765 7456 6965 7752 6573  alpha.GetViewRes
-00000bd0: 706f 6e73 6522 2482 d3e4 9302 1e12 1c2f  ponse"$......../
-00000be0: 7631 616c 7068 612f 7669 6577 732f 7b76  v1alpha/views/{v
-00000bf0: 6965 775f 6e61 6d65 3d2a 7d12 8301 0a0a  iew_name=*}.....
-00000c00: 4372 6561 7465 5669 6577 122a 2e6b 6173  CreateView.*.kas
-00000c10: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
-00000c20: 6c70 6861 2e43 7265 6174 6556 6965 7752  lpha.CreateViewR
-00000c30: 6571 7565 7374 1a2b 2e6b 6173 6b61 6461  equest.+.kaskada
-00000c40: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
-00000c50: 2e43 7265 6174 6556 6965 7752 6573 706f  .CreateViewRespo
-00000c60: 6e73 6522 1c82 d3e4 9302 163a 0476 6965  nse".......:.vie
-00000c70: 7722 0e2f 7631 616c 7068 612f 7669 6577  w"./v1alpha/view
-00000c80: 7312 8b01 0a0a 4465 6c65 7465 5669 6577  s.....DeleteView
-00000c90: 122a 2e6b 6173 6b61 6461 2e6b 6173 6b61  .*.kaskada.kaska
-00000ca0: 6461 2e76 3161 6c70 6861 2e44 656c 6574  da.v1alpha.Delet
-00000cb0: 6556 6965 7752 6571 7565 7374 1a2b 2e6b  eViewRequest.+.k
-00000cc0: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
-00000cd0: 3161 6c70 6861 2e44 656c 6574 6556 6965  1alpha.DeleteVie
-00000ce0: 7752 6573 706f 6e73 6522 2482 d3e4 9302  wResponse"$.....
-00000cf0: 1e2a 1c2f 7631 616c 7068 612f 7669 6577  .*./v1alpha/view
-00000d00: 732f 7b76 6965 775f 6e61 6d65 3d2a 7d42  s/{view_name=*}B
-00000d10: 8002 0a1b 636f 6d2e 6b61 736b 6164 612e  ....com.kaskada.
-00000d20: 6b61 736b 6164 612e 7631 616c 7068 6142  kaskada.v1alphaB
-00000d30: 1056 6965 7753 6572 7669 6365 5072 6f74  .ViewServiceProt
-00000d40: 6f50 015a 5167 6974 6875 622e 636f 6d2f  oP.ZQgithub.com/
-00000d50: 6b61 736b 6164 612d 6169 2f6b 6173 6b61  kaskada-ai/kaska
-00000d60: 6461 2f67 656e 2f70 726f 746f 2f67 6f2f  da/gen/proto/go/
-00000d70: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
-00000d80: 7631 616c 7068 613b 6b61 736b 6164 6176  v1alpha;kaskadav
-00000d90: 3161 6c70 6861 a202 034b 4b58 aa02 174b  1alpha...KKX...K
-00000da0: 6173 6b61 6461 2e4b 6173 6b61 6461 2e56  askada.Kaskada.V
-00000db0: 3161 6c70 6861 ca02 174b 6173 6b61 6461  1alpha...Kaskada
-00000dc0: 5c4b 6173 6b61 6461 5c56 3161 6c70 6861  \Kaskada\V1alpha
-00000dd0: e202 234b 6173 6b61 6461 5c4b 6173 6b61  ..#Kaskada\Kaska
-00000de0: 6461 5c56 3161 6c70 6861 5c47 5042 4d65  da\V1alpha\GPBMe
-00000df0: 7461 6461 7461 ea02 194b 6173 6b61 6461  tadata...Kaskada
-00000e00: 3a3a 4b61 736b 6164 613a 3a56 3161 6c70  ::Kaskada::V1alp
-00000e10: 6861 6206 7072 6f74 6f33 da04 5669 6577  hab.proto3..View
-00000e20: da10 4c69 7374 5669 6577 7352 6571 7565  ..ListViewsReque
-00000e30: 7374 da11 4c69 7374 5669 6577 7352 6573  st..ListViewsRes
-00000e40: 706f 6e73 65da 0e47 6574 5669 6577 5265  ponse..GetViewRe
-00000e50: 7175 6573 74da 0f47 6574 5669 6577 5265  quest..GetViewRe
-00000e60: 7370 6f6e 7365 da11 4372 6561 7465 5669  sponse..CreateVi
-00000e70: 6577 5265 7175 6573 74da 1243 7265 6174  ewRequest..Creat
-00000e80: 6556 6965 7752 6573 706f 6e73 65da 1144  eViewResponse..D
-00000e90: 656c 6574 6556 6965 7752 6571 7565 7374  eleteViewRequest
-00000ea0: da12 4465 6c65 7465 5669 6577 5265 7370  ..DeleteViewResp
-00000eb0: 6f6e 7365 7a28 6b61 736b 6164 612e 6b61  onsez(kaskada.ka
-00000ec0: 736b 6164 612e 7631 616c 7068 612e 7669  skada.v1alpha.vi
-00000ed0: 6577 5f73 6572 7669 6365 5f70 6232 2902  ew_service_pb2).
-00000ee0: da0a 4445 5343 5249 5054 4f52 da0a 5f5f  ..DESCRIPTOR..__
-00000ef0: 6d6f 6475 6c65 5f5f da0b 5669 6577 5365  module__..ViewSe
-00000f00: 7276 6963 6546 4e73 0001 0000 0a1b 636f  rviceFNs......co
-00000f10: 6d2e 6b61 736b 6164 612e 6b61 736b 6164  m.kaskada.kaskad
-00000f20: 612e 7631 616c 7068 6142 1056 6965 7753  a.v1alphaB.ViewS
-00000f30: 6572 7669 6365 5072 6f74 6f50 015a 5167  erviceProtoP.ZQg
-00000f40: 6974 6875 622e 636f 6d2f 6b61 736b 6164  ithub.com/kaskad
-00000f50: 612d 6169 2f6b 6173 6b61 6461 2f67 656e  a-ai/kaskada/gen
-00000f60: 2f70 726f 746f 2f67 6f2f 6b61 736b 6164  /proto/go/kaskad
-00000f70: 612f 6b61 736b 6164 612f 7631 616c 7068  a/kaskada/v1alph
-00000f80: 613b 6b61 736b 6164 6176 3161 6c70 6861  a;kaskadav1alpha
-00000f90: a202 034b 4b58 aa02 174b 6173 6b61 6461  ...KKX...Kaskada
-00000fa0: 2e4b 6173 6b61 6461 2e56 3161 6c70 6861  .Kaskada.V1alpha
-00000fb0: ca02 174b 6173 6b61 6461 5c4b 6173 6b61  ...Kaskada\Kaska
-00000fc0: 6461 5c56 3161 6c70 6861 e202 234b 6173  da\V1alpha..#Kas
-00000fd0: 6b61 6461 5c4b 6173 6b61 6461 5c56 3161  kada\Kaskada\V1a
-00000fe0: 6c70 6861 5c47 5042 4d65 7461 6461 7461  lpha\GPBMetadata
-00000ff0: ea02 194b 6173 6b61 6461 3a3a 4b61 736b  ...Kaskada::Kask
-00001000: 6164 613a 3a56 3161 6c70 6861 da07 7669  ada::V1alpha..vi
-00001010: 6577 5f69 6473 0300 0000 e041 03da 0976  ew_ids.....A...v
-00001020: 6965 775f 6e61 6d65 7307 0000 00fa 4204  iew_names.....B.
-00001030: 7202 1001 da0a 6578 7072 6573 7369 6f6e  r.....expression
-00001040: da0b 7265 7375 6c74 5f74 7970 65da 0861  ..result_type..a
-00001050: 6e61 6c79 7369 73da 0970 6167 655f 7369  nalysis..page_si
-00001060: 7a65 730a 0000 00fa 4207 1a05 18e8 0728  zes.....B......(
-00001070: 00da 0476 6965 7773 0800 0000 fa42 058a  ...views.....B..
-00001080: 0102 1001 da09 4c69 7374 5669 6577 7373  ......ListViewss
-00001090: 1600 0000 82d3 e493 0210 120e 2f76 3161  ............/v1a
-000010a0: 6c70 6861 2f76 6965 7773 da07 4765 7456  lpha/views..GetV
-000010b0: 6965 7773 2400 0000 82d3 e493 021e 121c  iews$...........
-000010c0: 2f76 3161 6c70 6861 2f76 6965 7773 2f7b  /v1alpha/views/{
-000010d0: 7669 6577 5f6e 616d 653d 2a7d da0a 4372  view_name=*}..Cr
-000010e0: 6561 7465 5669 6577 731c 0000 0082 d3e4  eateViews.......
-000010f0: 9302 163a 0476 6965 7722 0e2f 7631 616c  ...:.view"./v1al
-00001100: 7068 612f 7669 6577 73da 0a44 656c 6574  pha/views..Delet
-00001110: 6556 6965 7773 2400 0000 82d3 e493 021e  eViews$.........
-00001120: 2a1c 2f76 3161 6c70 6861 2f76 6965 7773  *./v1alpha/views
-00001130: 2f7b 7669 6577 5f6e 616d 653d 2a7d e9ec  /{view_name=*}..
-00001140: 0000 0069 ec01 0000 69ee 0100 0069 6002  ...i....i....i`.
-00001150: 0000 6963 0200 0069 2503 0000 6927 0300  ..ic...i%...i'..
-00001160: 0069 5d03 0000 6960 0300 0069 f603 0000  .i]...i`...i....
-00001170: 69f8 0300 0069 6104 0000 6964 0400 0069  i....ia...id...i
-00001180: 3c05 0000 693e 0500 0069 8d05 0000 698f  <...i>...i....i.
-00001190: 0500 0069 f505 0000 69f8 0500 0069 1a08  ...i....i....i..
-000011a0: 0000 293c da07 5f5f 646f 635f 5fda 0f67  ..)<..__doc__..g
-000011b0: 6f6f 676c 652e 7072 6f74 6f62 7566 7202  oogle.protobufr.
-000011c0: 0000 00da 0b5f 6465 7363 7269 7074 6f72  ....._descriptor
-000011d0: 7203 0000 00da 105f 6465 7363 7269 7074  r......_descript
-000011e0: 6f72 5f70 6f6f 6c72 0400 0000 da08 5f6d  or_poolr......_m
-000011f0: 6573 7361 6765 7205 0000 00da 0b5f 7265  essager......_re
-00001200: 666c 6563 7469 6f6e 7206 0000 00da 105f  flectionr......_
-00001210: 7379 6d62 6f6c 5f64 6174 6162 6173 65da  symbol_database.
-00001220: 0744 6566 6175 6c74 da07 5f73 796d 5f64  .Default.._sym_d
-00001230: 62da 0a67 6f6f 676c 652e 6170 6972 0700  b..google.apir..
-00001240: 0000 da23 676f 6f67 6c65 5f64 6f74 5f61  ...#google_dot_a
-00001250: 7069 5f64 6f74 5f61 6e6e 6f74 6174 696f  pi_dot_annotatio
-00001260: 6e73 5f5f 7062 3272 0800 0000 da27 676f  ns__pb2r.....'go
-00001270: 6f67 6c65 5f64 6f74 5f61 7069 5f64 6f74  ogle_dot_api_dot
-00001280: 5f66 6965 6c64 5f5f 6265 6861 7669 6f72  _field__behavior
-00001290: 5f5f 7062 32da 176b 6173 6b61 6461 2e6b  __pb2..kaskada.k
-000012a0: 6173 6b61 6461 2e76 3161 6c70 6861 7209  askada.v1alphar.
-000012b0: 0000 00da 2f6b 6173 6b61 6461 5f64 6f74  ..../kaskada_dot
-000012c0: 5f6b 6173 6b61 6461 5f64 6f74 5f76 3161  _kaskada_dot_v1a
-000012d0: 6c70 6861 5f64 6f74 5f63 6f6d 6d6f 6e5f  lpha_dot_common_
-000012e0: 5f70 6232 720a 0000 00da 2f6b 6173 6b61  _pb2r...../kaska
-000012f0: 6461 5f64 6f74 5f6b 6173 6b61 6461 5f64  da_dot_kaskada_d
-00001300: 6f74 5f76 3161 6c70 6861 5f64 6f74 5f73  ot_v1alpha_dot_s
-00001310: 6368 656d 615f 5f70 6232 da08 7661 6c69  chema__pb2..vali
-00001320: 6461 7465 720b 0000 00da 1a76 616c 6964  dater......valid
-00001330: 6174 655f 646f 745f 7661 6c69 6461 7465  ate_dot_validate
-00001340: 5f5f 7062 32da 1141 6464 5365 7269 616c  __pb2..AddSerial
-00001350: 697a 6564 4669 6c65 7215 0000 00da 156d  izedFiler......m
-00001360: 6573 7361 6765 5f74 7970 6573 5f62 795f  essage_types_by_
-00001370: 6e61 6d65 da05 5f56 4945 57da 115f 4c49  name.._VIEW.._LI
-00001380: 5354 5649 4557 5352 4551 5545 5354 da12  STVIEWSREQUEST..
-00001390: 5f4c 4953 5456 4945 5753 5245 5350 4f4e  _LISTVIEWSRESPON
-000013a0: 5345 da0f 5f47 4554 5649 4557 5245 5155  SE.._GETVIEWREQU
-000013b0: 4553 54da 105f 4745 5456 4945 5752 4553  EST.._GETVIEWRES
-000013c0: 504f 4e53 45da 125f 4352 4541 5445 5649  PONSE.._CREATEVI
-000013d0: 4557 5245 5155 4553 54da 135f 4352 4541  EWREQUEST.._CREA
-000013e0: 5445 5649 4557 5245 5350 4f4e 5345 da12  TEVIEWRESPONSE..
-000013f0: 5f44 454c 4554 4556 4945 5752 4551 5545  _DELETEVIEWREQUE
-00001400: 5354 da13 5f44 454c 4554 4556 4945 5752  ST.._DELETEVIEWR
-00001410: 4553 504f 4e53 45da 1c47 656e 6572 6174  ESPONSE..Generat
-00001420: 6564 5072 6f74 6f63 6f6c 4d65 7373 6167  edProtocolMessag
-00001430: 6554 7970 65da 074d 6573 7361 6765 720c  eType..Messager.
-00001440: 0000 00da 0f52 6567 6973 7465 724d 6573  .....RegisterMes
-00001450: 7361 6765 720d 0000 0072 0e00 0000 720f  sager....r....r.
-00001460: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
-00001470: 0000 7213 0000 0072 1400 0000 da10 7365  ..r....r......se
-00001480: 7276 6963 6573 5f62 795f 6e61 6d65 da0c  rvices_by_name..
-00001490: 5f56 4945 5753 4552 5649 4345 da12 5f55  _VIEWSERVICE.._U
-000014a0: 5345 5f43 5f44 4553 4352 4950 544f 5253  SE_C_DESCRIPTORS
-000014b0: da08 5f6f 7074 696f 6e73 da13 5f73 6572  .._options.._ser
-000014c0: 6961 6c69 7a65 645f 6f70 7469 6f6e 73da  ialized_options.
-000014d0: 0e66 6965 6c64 735f 6279 5f6e 616d 65da  .fields_by_name.
-000014e0: 0f6d 6574 686f 6473 5f62 795f 6e61 6d65  .methods_by_name
-000014f0: da11 5f73 6572 6961 6c69 7a65 645f 7374  .._serialized_st
-00001500: 6172 74da 0f5f 7365 7269 616c 697a 6564  art.._serialized
-00001510: 5f65 6e64 a900 724c 0000 0072 4c00 0000  _end..rL...rL...
-00001520: fa76 2f68 6f6d 652f 7468 6572 6170 6f6e  .v/home/therapon
-00001530: 2f52 6570 6f73 2f47 6974 4875 622f 4b61  /Repos/GitHub/Ka
-00001540: 736b 6164 6141 492f 6b61 736b 6164 612f  skadaAI/kaskada/
-00001550: 7265 6c65 6173 696e 672f 636c 6965 6e74  releasing/client
-00001560: 732f 7079 7468 6f6e 2f73 7263 2f6b 6173  s/python/src/kas
-00001570: 6b61 6461 2f6b 6173 6b61 6461 2f76 3161  kada/kaskada/v1a
-00001580: 6c70 6861 2f76 6965 775f 7365 7276 6963  lpha/view_servic
-00001590: 655f 7062 322e 7079 da08 3c6d 6f64 756c  e_pb2.py..<modul
-000015a0: 653e 0100 0000 73ec 0000 0004 030c 010c  e>....s.........
-000015b0: 010c 010c 010c 0108 030c 030c 010c 010c  ................
-000015c0: 010c 010e 030a 040a 010a 010a 010a 010a  ................
-000015d0: 010a 010a 010a 010c 0102 0102 0108 fe0a  ................
-000015e0: 050c 0202 0102 0108 fe0a 050c 0202 0102  ................
-000015f0: 0108 fe0a 050c 0202 0102 0108 fe0a 050c  ................
-00001600: 0202 0102 0108 fe0a 050c 0202 0102 0108  ................
-00001610: fe0a 050c 0202 0102 0108 fe0a 050c 0202  ................
-00001620: 0102 0108 fe0a 050c 0202 0102 0108 fe0a  ................
-00001630: 050a 020c 0106 0206 010c 010c 010c 010c  ................
-00001640: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00001650: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00001660: 010c 010c 010c 010c 010c 010c 0106 0106  ................
-00001670: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00001680: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00001690: 0106 010a 0104 cf                        .......
+00000420: 5300 2943 7a1f 4765 6e65 7261 7465 6420  S.)Cz.Generated 
+00000430: 7072 6f74 6f63 6f6c 2062 7566 6665 7220  protocol buffer 
+00000440: 636f 6465 2ee9 0000 0000 2901 da0a 6465  code......)...de
+00000450: 7363 7269 7074 6f72 2901 da0f 6465 7363  scriptor)...desc
+00000460: 7269 7074 6f72 5f70 6f6f 6c29 01da 076d  riptor_pool)...m
+00000470: 6573 7361 6765 2901 da0a 7265 666c 6563  essage)...reflec
+00000480: 7469 6f6e 2901 da0f 7379 6d62 6f6c 5f64  tion)...symbol_d
+00000490: 6174 6162 6173 6529 01da 0f61 6e6e 6f74  atabase)...annot
+000004a0: 6174 696f 6e73 5f70 6232 2901 da12 6669  ations_pb2)...fi
+000004b0: 656c 645f 6265 6861 7669 6f72 5f70 6232  eld_behavior_pb2
+000004c0: 2901 da0a 636f 6d6d 6f6e 5f70 6232 2901  )...common_pb2).
+000004d0: da0a 7363 6865 6d61 5f70 6232 2901 da0c  ..schema_pb2)...
+000004e0: 7661 6c69 6461 7465 5f70 6232 7325 0900  validate_pb2s%..
+000004f0: 000a 2a6b 6173 6b61 6461 2f6b 6173 6b61  ..*kaskada/kaska
+00000500: 6461 2f76 3161 6c70 6861 2f76 6965 775f  da/v1alpha/view_
+00000510: 7365 7276 6963 652e 7072 6f74 6f12 176b  service.proto..k
+00000520: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
+00000530: 3161 6c70 6861 1a1c 676f 6f67 6c65 2f61  1alpha..google/a
+00000540: 7069 2f61 6e6e 6f74 6174 696f 6e73 2e70  pi/annotations.p
+00000550: 726f 746f 1a1f 676f 6f67 6c65 2f61 7069  roto..google/api
+00000560: 2f66 6965 6c64 5f62 6568 6176 696f 722e  /field_behavior.
+00000570: 7072 6f74 6f1a 246b 6173 6b61 6461 2f6b  proto.$kaskada/k
+00000580: 6173 6b61 6461 2f76 3161 6c70 6861 2f63  askada/v1alpha/c
+00000590: 6f6d 6d6f 6e2e 7072 6f74 6f1a 246b 6173  ommon.proto.$kas
+000005a0: 6b61 6461 2f6b 6173 6b61 6461 2f76 3161  kada/kaskada/v1a
+000005b0: 6c70 6861 2f73 6368 656d 612e 7072 6f74  lpha/schema.prot
+000005c0: 6f1a 1776 616c 6964 6174 652f 7661 6c69  o..validate/vali
+000005d0: 6461 7465 2e70 726f 746f 2280 020a 0456  date.proto"....V
+000005e0: 6965 7712 1c0a 0776 6965 775f 6964 1801  iew....view_id..
+000005f0: 2001 2809 4203 e041 0352 0676 6965 7749   .(.B..A.R.viewI
+00000600: 6412 240a 0976 6965 775f 6e61 6d65 1802  d.$..view_name..
+00000610: 2001 2809 4207 fa42 0472 0210 0152 0876   .(.B..B.r...R.v
+00000620: 6965 774e 616d 6512 270a 0a65 7870 7265  iewName.'..expre
+00000630: 7373 696f 6e18 0320 0128 0942 07fa 4204  ssion.. .(.B..B.
+00000640: 7202 1001 520a 6578 7072 6573 7369 6f6e  r...R.expression
+00000650: 1247 0a0b 7265 7375 6c74 5f74 7970 6518  .G..result_type.
+00000660: 0720 0128 0b32 212e 6b61 736b 6164 612e  . .(.2!.kaskada.
+00000670: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
+00000680: 4461 7461 5479 7065 4203 e041 0352 0a72  DataTypeB..A.R.r
+00000690: 6573 756c 7454 7970 6512 420a 0861 6e61  esultType.B..ana
+000006a0: 6c79 7369 7318 0820 0128 0b32 212e 6b61  lysis.. .(.2!.ka
+000006b0: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
+000006c0: 616c 7068 612e 416e 616c 7973 6973 4203  alpha.AnalysisB.
+000006d0: e041 0352 0861 6e61 6c79 7369 7322 720a  .A.R.analysis"r.
+000006e0: 104c 6973 7456 6965 7773 5265 7175 6573  .ListViewsReques
+000006f0: 7412 160a 0673 6561 7263 6818 0120 0128  t....search.. .(
+00000700: 0952 0673 6561 7263 6812 270a 0970 6167  .R.search.'..pag
+00000710: 655f 7369 7a65 1802 2001 2805 420a fa42  e_size.. .(.B..B
+00000720: 071a 0518 e807 2800 5208 7061 6765 5369  ......(.R.pageSi
+00000730: 7a65 121d 0a0a 7061 6765 5f74 6f6b 656e  ze....page_token
+00000740: 1803 2001 2809 5209 7061 6765 546f 6b65  .. .(.R.pageToke
+00000750: 6e22 c201 0a11 4c69 7374 5669 6577 7352  n"....ListViewsR
+00000760: 6573 706f 6e73 6512 330a 0576 6965 7773  esponse.3..views
+00000770: 1801 2003 280b 321d 2e6b 6173 6b61 6461  .. .(.2..kaskada
+00000780: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00000790: 2e56 6965 7752 0576 6965 7773 1250 0a0f  .ViewR.views.P..
+000007a0: 7265 7175 6573 745f 6465 7461 696c 7318  request_details.
+000007b0: 0220 0128 0b32 272e 6b61 736b 6164 612e  . .(.2'.kaskada.
+000007c0: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
+000007d0: 5265 7175 6573 7444 6574 6169 6c73 520e  RequestDetailsR.
+000007e0: 7265 7175 6573 7444 6574 6169 6c73 1226  requestDetails.&
+000007f0: 0a0f 6e65 7874 5f70 6167 655f 746f 6b65  ..next_page_toke
+00000800: 6e18 0320 0128 0952 0d6e 6578 7450 6167  n.. .(.R.nextPag
+00000810: 6554 6f6b 656e 2236 0a0e 4765 7456 6965  eToken"6..GetVie
+00000820: 7752 6571 7565 7374 1224 0a09 7669 6577  wRequest.$..view
+00000830: 5f6e 616d 6518 0120 0128 0942 07fa 4204  _name.. .(.B..B.
+00000840: 7202 1001 5208 7669 6577 4e61 6d65 2296  r...R.viewName".
+00000850: 010a 0f47 6574 5669 6577 5265 7370 6f6e  ...GetViewRespon
+00000860: 7365 1231 0a04 7669 6577 1801 2001 280b  se.1..view.. .(.
+00000870: 321d 2e6b 6173 6b61 6461 2e6b 6173 6b61  2..kaskada.kaska
+00000880: 6461 2e76 3161 6c70 6861 2e56 6965 7752  da.v1alpha.ViewR
+00000890: 0476 6965 7712 500a 0f72 6571 7565 7374  .view.P..request
+000008a0: 5f64 6574 6169 6c73 1802 2001 280b 3227  _details.. .(.2'
+000008b0: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+000008c0: 2e76 3161 6c70 6861 2e52 6571 7565 7374  .v1alpha.Request
+000008d0: 4465 7461 696c 7352 0e72 6571 7565 7374  DetailsR.request
+000008e0: 4465 7461 696c 7322 690a 1143 7265 6174  Details"i..Creat
+000008f0: 6556 6965 7752 6571 7565 7374 123b 0a04  eViewRequest.;..
+00000900: 7669 6577 1801 2001 280b 321d 2e6b 6173  view.. .(.2..kas
+00000910: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
+00000920: 6c70 6861 2e56 6965 7742 08fa 4205 8a01  lpha.ViewB..B...
+00000930: 0210 0152 0476 6965 7712 170a 0764 7279  ...R.view....dry
+00000940: 5f72 756e 1802 2001 2808 5206 6472 7952  _run.. .(.R.dryR
+00000950: 756e 22d8 010a 1243 7265 6174 6556 6965  un"....CreateVie
+00000960: 7752 6573 706f 6e73 6512 310a 0476 6965  wResponse.1..vie
+00000970: 7718 0120 0128 0b32 1d2e 6b61 736b 6164  w.. .(.2..kaskad
+00000980: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00000990: 612e 5669 6577 5204 7669 6577 1250 0a0f  a.ViewR.view.P..
+000009a0: 7265 7175 6573 745f 6465 7461 696c 7318  request_details.
+000009b0: 0220 0128 0b32 272e 6b61 736b 6164 612e  . .(.2'.kaskada.
+000009c0: 6b61 736b 6164 612e 7631 616c 7068 612e  kaskada.v1alpha.
+000009d0: 5265 7175 6573 7444 6574 6169 6c73 520e  RequestDetailsR.
+000009e0: 7265 7175 6573 7444 6574 6169 6c73 123d  requestDetails.=
+000009f0: 0a08 616e 616c 7973 6973 1803 2001 280b  ..analysis.. .(.
+00000a00: 3221 2e6b 6173 6b61 6461 2e6b 6173 6b61  2!.kaskada.kaska
+00000a10: 6461 2e76 3161 6c70 6861 2e41 6e61 6c79  da.v1alpha.Analy
+00000a20: 7369 7352 0861 6e61 6c79 7369 7322 4f0a  sisR.analysis"O.
+00000a30: 1144 656c 6574 6556 6965 7752 6571 7565  .DeleteViewReque
+00000a40: 7374 1224 0a09 7669 6577 5f6e 616d 6518  st.$..view_name.
+00000a50: 0120 0128 0942 07fa 4204 7202 1001 5208  . .(.B..B.r...R.
+00000a60: 7669 6577 4e61 6d65 1214 0a05 666f 7263  viewName....forc
+00000a70: 6518 0220 0128 0852 0566 6f72 6365 2266  e.. .(.R.force"f
+00000a80: 0a12 4465 6c65 7465 5669 6577 5265 7370  ..DeleteViewResp
+00000a90: 6f6e 7365 1250 0a0f 7265 7175 6573 745f  onse.P..request_
+00000aa0: 6465 7461 696c 7318 0120 0128 0b32 272e  details.. .(.2'.
+00000ab0: 6b61 736b 6164 612e 6b61 736b 6164 612e  kaskada.kaskada.
+00000ac0: 7631 616c 7068 612e 5265 7175 6573 7444  v1alpha.RequestD
+00000ad0: 6574 6169 6c73 520e 7265 7175 6573 7444  etailsR.requestD
+00000ae0: 6574 6169 6c73 32a2 040a 0b56 6965 7753  etails2....ViewS
+00000af0: 6572 7669 6365 127a 0a09 4c69 7374 5669  ervice.z..ListVi
+00000b00: 6577 7312 292e 6b61 736b 6164 612e 6b61  ews.).kaskada.ka
+00000b10: 736b 6164 612e 7631 616c 7068 612e 4c69  skada.v1alpha.Li
+00000b20: 7374 5669 6577 7352 6571 7565 7374 1a2a  stViewsRequest.*
+00000b30: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00000b40: 2e76 3161 6c70 6861 2e4c 6973 7456 6965  .v1alpha.ListVie
+00000b50: 7773 5265 7370 6f6e 7365 2216 82d3 e493  wsResponse".....
+00000b60: 0210 120e 2f76 3161 6c70 6861 2f76 6965  ..../v1alpha/vie
+00000b70: 7773 1282 010a 0747 6574 5669 6577 1227  ws.....GetView.'
+00000b80: 2e6b 6173 6b61 6461 2e6b 6173 6b61 6461  .kaskada.kaskada
+00000b90: 2e76 3161 6c70 6861 2e47 6574 5669 6577  .v1alpha.GetView
+00000ba0: 5265 7175 6573 741a 282e 6b61 736b 6164  Request.(.kaskad
+00000bb0: 612e 6b61 736b 6164 612e 7631 616c 7068  a.kaskada.v1alph
+00000bc0: 612e 4765 7456 6965 7752 6573 706f 6e73  a.GetViewRespons
+00000bd0: 6522 2482 d3e4 9302 1e12 1c2f 7631 616c  e"$......../v1al
+00000be0: 7068 612f 7669 6577 732f 7b76 6965 775f  pha/views/{view_
+00000bf0: 6e61 6d65 3d2a 7d12 8301 0a0a 4372 6561  name=*}.....Crea
+00000c00: 7465 5669 6577 122a 2e6b 6173 6b61 6461  teView.*.kaskada
+00000c10: 2e6b 6173 6b61 6461 2e76 3161 6c70 6861  .kaskada.v1alpha
+00000c20: 2e43 7265 6174 6556 6965 7752 6571 7565  .CreateViewReque
+00000c30: 7374 1a2b 2e6b 6173 6b61 6461 2e6b 6173  st.+.kaskada.kas
+00000c40: 6b61 6461 2e76 3161 6c70 6861 2e43 7265  kada.v1alpha.Cre
+00000c50: 6174 6556 6965 7752 6573 706f 6e73 6522  ateViewResponse"
+00000c60: 1c82 d3e4 9302 163a 0476 6965 7722 0e2f  .......:.view"./
+00000c70: 7631 616c 7068 612f 7669 6577 7312 8b01  v1alpha/views...
+00000c80: 0a0a 4465 6c65 7465 5669 6577 122a 2e6b  ..DeleteView.*.k
+00000c90: 6173 6b61 6461 2e6b 6173 6b61 6461 2e76  askada.kaskada.v
+00000ca0: 3161 6c70 6861 2e44 656c 6574 6556 6965  1alpha.DeleteVie
+00000cb0: 7752 6571 7565 7374 1a2b 2e6b 6173 6b61  wRequest.+.kaska
+00000cc0: 6461 2e6b 6173 6b61 6461 2e76 3161 6c70  da.kaskada.v1alp
+00000cd0: 6861 2e44 656c 6574 6556 6965 7752 6573  ha.DeleteViewRes
+00000ce0: 706f 6e73 6522 2482 d3e4 9302 1e2a 1c2f  ponse"$......*./
+00000cf0: 7631 616c 7068 612f 7669 6577 732f 7b76  v1alpha/views/{v
+00000d00: 6965 775f 6e61 6d65 3d2a 7d42 8002 0a1b  iew_name=*}B....
+00000d10: 636f 6d2e 6b61 736b 6164 612e 6b61 736b  com.kaskada.kask
+00000d20: 6164 612e 7631 616c 7068 6142 1056 6965  ada.v1alphaB.Vie
+00000d30: 7753 6572 7669 6365 5072 6f74 6f50 015a  wServiceProtoP.Z
+00000d40: 5167 6974 6875 622e 636f 6d2f 6b61 736b  Qgithub.com/kask
+00000d50: 6164 612d 6169 2f6b 6173 6b61 6461 2f67  ada-ai/kaskada/g
+00000d60: 656e 2f70 726f 746f 2f67 6f2f 6b61 736b  en/proto/go/kask
+00000d70: 6164 612f 6b61 736b 6164 612f 7631 616c  ada/kaskada/v1al
+00000d80: 7068 613b 6b61 736b 6164 6176 3161 6c70  pha;kaskadav1alp
+00000d90: 6861 a202 034b 4b58 aa02 174b 6173 6b61  ha...KKX...Kaska
+00000da0: 6461 2e4b 6173 6b61 6461 2e56 3161 6c70  da.Kaskada.V1alp
+00000db0: 6861 ca02 174b 6173 6b61 6461 5c4b 6173  ha...Kaskada\Kas
+00000dc0: 6b61 6461 5c56 3161 6c70 6861 e202 234b  kada\V1alpha..#K
+00000dd0: 6173 6b61 6461 5c4b 6173 6b61 6461 5c56  askada\Kaskada\V
+00000de0: 3161 6c70 6861 5c47 5042 4d65 7461 6461  1alpha\GPBMetada
+00000df0: 7461 ea02 194b 6173 6b61 6461 3a3a 4b61  ta...Kaskada::Ka
+00000e00: 736b 6164 613a 3a56 3161 6c70 6861 6206  skada::V1alphab.
+00000e10: 7072 6f74 6f33 da04 5669 6577 da10 4c69  proto3..View..Li
+00000e20: 7374 5669 6577 7352 6571 7565 7374 da11  stViewsRequest..
+00000e30: 4c69 7374 5669 6577 7352 6573 706f 6e73  ListViewsRespons
+00000e40: 65da 0e47 6574 5669 6577 5265 7175 6573  e..GetViewReques
+00000e50: 74da 0f47 6574 5669 6577 5265 7370 6f6e  t..GetViewRespon
+00000e60: 7365 da11 4372 6561 7465 5669 6577 5265  se..CreateViewRe
+00000e70: 7175 6573 74da 1243 7265 6174 6556 6965  quest..CreateVie
+00000e80: 7752 6573 706f 6e73 65da 1144 656c 6574  wResponse..Delet
+00000e90: 6556 6965 7752 6571 7565 7374 da12 4465  eViewRequest..De
+00000ea0: 6c65 7465 5669 6577 5265 7370 6f6e 7365  leteViewResponse
+00000eb0: 7a28 6b61 736b 6164 612e 6b61 736b 6164  z(kaskada.kaskad
+00000ec0: 612e 7631 616c 7068 612e 7669 6577 5f73  a.v1alpha.view_s
+00000ed0: 6572 7669 6365 5f70 6232 2902 da0a 4445  ervice_pb2)...DE
+00000ee0: 5343 5249 5054 4f52 da0a 5f5f 6d6f 6475  SCRIPTOR..__modu
+00000ef0: 6c65 5f5f 5a0b 5669 6577 5365 7276 6963  le__Z.ViewServic
+00000f00: 6546 4e73 0001 0000 0a1b 636f 6d2e 6b61  eFNs......com.ka
+00000f10: 736b 6164 612e 6b61 736b 6164 612e 7631  skada.kaskada.v1
+00000f20: 616c 7068 6142 1056 6965 7753 6572 7669  alphaB.ViewServi
+00000f30: 6365 5072 6f74 6f50 015a 5167 6974 6875  ceProtoP.ZQgithu
+00000f40: 622e 636f 6d2f 6b61 736b 6164 612d 6169  b.com/kaskada-ai
+00000f50: 2f6b 6173 6b61 6461 2f67 656e 2f70 726f  /kaskada/gen/pro
+00000f60: 746f 2f67 6f2f 6b61 736b 6164 612f 6b61  to/go/kaskada/ka
+00000f70: 736b 6164 612f 7631 616c 7068 613b 6b61  skada/v1alpha;ka
+00000f80: 736b 6164 6176 3161 6c70 6861 a202 034b  skadav1alpha...K
+00000f90: 4b58 aa02 174b 6173 6b61 6461 2e4b 6173  KX...Kaskada.Kas
+00000fa0: 6b61 6461 2e56 3161 6c70 6861 ca02 174b  kada.V1alpha...K
+00000fb0: 6173 6b61 6461 5c4b 6173 6b61 6461 5c56  askada\Kaskada\V
+00000fc0: 3161 6c70 6861 e202 234b 6173 6b61 6461  1alpha..#Kaskada
+00000fd0: 5c4b 6173 6b61 6461 5c56 3161 6c70 6861  \Kaskada\V1alpha
+00000fe0: 5c47 5042 4d65 7461 6461 7461 ea02 194b  \GPBMetadata...K
+00000ff0: 6173 6b61 6461 3a3a 4b61 736b 6164 613a  askada::Kaskada:
+00001000: 3a56 3161 6c70 6861 5a07 7669 6577 5f69  :V1alphaZ.view_i
+00001010: 6473 0300 0000 e041 03da 0976 6965 775f  ds.....A...view_
+00001020: 6e61 6d65 7307 0000 00fa 4204 7202 1001  names.....B.r...
+00001030: da0a 6578 7072 6573 7369 6f6e da0b 7265  ..expression..re
+00001040: 7375 6c74 5f74 7970 65da 0861 6e61 6c79  sult_type..analy
+00001050: 7369 73da 0970 6167 655f 7369 7a65 730a  sis..page_sizes.
+00001060: 0000 00fa 4207 1a05 18e8 0728 00da 0476  ....B......(...v
+00001070: 6965 7773 0800 0000 fa42 058a 0102 1001  iews.....B......
+00001080: 5a09 4c69 7374 5669 6577 7373 1600 0000  Z.ListViewss....
+00001090: 82d3 e493 0210 120e 2f76 3161 6c70 6861  ......../v1alpha
+000010a0: 2f76 6965 7773 5a07 4765 7456 6965 7773  /viewsZ.GetViews
+000010b0: 2400 0000 82d3 e493 021e 121c 2f76 3161  $.........../v1a
+000010c0: 6c70 6861 2f76 6965 7773 2f7b 7669 6577  lpha/views/{view
+000010d0: 5f6e 616d 653d 2a7d 5a0a 4372 6561 7465  _name=*}Z.Create
+000010e0: 5669 6577 731c 0000 0082 d3e4 9302 163a  Views..........:
+000010f0: 0476 6965 7722 0e2f 7631 616c 7068 612f  .view"./v1alpha/
+00001100: 7669 6577 735a 0a44 656c 6574 6556 6965  viewsZ.DeleteVie
+00001110: 7773 2400 0000 82d3 e493 021e 2a1c 2f76  ws$.........*./v
+00001120: 3161 6c70 6861 2f76 6965 7773 2f7b 7669  1alpha/views/{vi
+00001130: 6577 5f6e 616d 653d 2a7d e9ec 0000 0069  ew_name=*}.....i
+00001140: ec01 0000 69ee 0100 0069 6002 0000 6963  ....i....i`...ic
+00001150: 0200 0069 2503 0000 6927 0300 0069 5d03  ...i%...i'...i].
+00001160: 0000 6960 0300 0069 f603 0000 69f8 0300  ..i`...i....i...
+00001170: 0069 6104 0000 6964 0400 0069 3c05 0000  .ia...id...i<...
+00001180: 693e 0500 0069 8d05 0000 698f 0500 0069  i>...i....i....i
+00001190: f505 0000 69f8 0500 0069 1a08 0000 293c  ....i....i....)<
+000011a0: da07 5f5f 646f 635f 5fda 0f67 6f6f 676c  ..__doc__..googl
+000011b0: 652e 7072 6f74 6f62 7566 7202 0000 00da  e.protobufr.....
+000011c0: 0b5f 6465 7363 7269 7074 6f72 7203 0000  ._descriptorr...
+000011d0: 00da 105f 6465 7363 7269 7074 6f72 5f70  ..._descriptor_p
+000011e0: 6f6f 6c72 0400 0000 da08 5f6d 6573 7361  oolr......_messa
+000011f0: 6765 7205 0000 00da 0b5f 7265 666c 6563  ger......_reflec
+00001200: 7469 6f6e 7206 0000 00da 105f 7379 6d62  tionr......_symb
+00001210: 6f6c 5f64 6174 6162 6173 65da 0744 6566  ol_database..Def
+00001220: 6175 6c74 da07 5f73 796d 5f64 62da 0a67  ault.._sym_db..g
+00001230: 6f6f 676c 652e 6170 6972 0700 0000 da23  oogle.apir.....#
+00001240: 676f 6f67 6c65 5f64 6f74 5f61 7069 5f64  google_dot_api_d
+00001250: 6f74 5f61 6e6e 6f74 6174 696f 6e73 5f5f  ot_annotations__
+00001260: 7062 3272 0800 0000 da27 676f 6f67 6c65  pb2r.....'google
+00001270: 5f64 6f74 5f61 7069 5f64 6f74 5f66 6965  _dot_api_dot_fie
+00001280: 6c64 5f5f 6265 6861 7669 6f72 5f5f 7062  ld__behavior__pb
+00001290: 32da 176b 6173 6b61 6461 2e6b 6173 6b61  2..kaskada.kaska
+000012a0: 6461 2e76 3161 6c70 6861 7209 0000 00da  da.v1alphar.....
+000012b0: 2f6b 6173 6b61 6461 5f64 6f74 5f6b 6173  /kaskada_dot_kas
+000012c0: 6b61 6461 5f64 6f74 5f76 3161 6c70 6861  kada_dot_v1alpha
+000012d0: 5f64 6f74 5f63 6f6d 6d6f 6e5f 5f70 6232  _dot_common__pb2
+000012e0: 720a 0000 00da 2f6b 6173 6b61 6461 5f64  r...../kaskada_d
+000012f0: 6f74 5f6b 6173 6b61 6461 5f64 6f74 5f76  ot_kaskada_dot_v
+00001300: 3161 6c70 6861 5f64 6f74 5f73 6368 656d  1alpha_dot_schem
+00001310: 615f 5f70 6232 da08 7661 6c69 6461 7465  a__pb2..validate
+00001320: 720b 0000 00da 1a76 616c 6964 6174 655f  r......validate_
+00001330: 646f 745f 7661 6c69 6461 7465 5f5f 7062  dot_validate__pb
+00001340: 32da 1141 6464 5365 7269 616c 697a 6564  2..AddSerialized
+00001350: 4669 6c65 7215 0000 00da 156d 6573 7361  Filer......messa
+00001360: 6765 5f74 7970 6573 5f62 795f 6e61 6d65  ge_types_by_name
+00001370: 5a05 5f56 4945 575a 115f 4c49 5354 5649  Z._VIEWZ._LISTVI
+00001380: 4557 5352 4551 5545 5354 5a12 5f4c 4953  EWSREQUESTZ._LIS
+00001390: 5456 4945 5753 5245 5350 4f4e 5345 5a0f  TVIEWSRESPONSEZ.
+000013a0: 5f47 4554 5649 4557 5245 5155 4553 545a  _GETVIEWREQUESTZ
+000013b0: 105f 4745 5456 4945 5752 4553 504f 4e53  ._GETVIEWRESPONS
+000013c0: 455a 125f 4352 4541 5445 5649 4557 5245  EZ._CREATEVIEWRE
+000013d0: 5155 4553 545a 135f 4352 4541 5445 5649  QUESTZ._CREATEVI
+000013e0: 4557 5245 5350 4f4e 5345 5a12 5f44 454c  EWRESPONSEZ._DEL
+000013f0: 4554 4556 4945 5752 4551 5545 5354 5a13  ETEVIEWREQUESTZ.
+00001400: 5f44 454c 4554 4556 4945 5752 4553 504f  _DELETEVIEWRESPO
+00001410: 4e53 45da 1c47 656e 6572 6174 6564 5072  NSE..GeneratedPr
+00001420: 6f74 6f63 6f6c 4d65 7373 6167 6554 7970  otocolMessageTyp
+00001430: 65da 074d 6573 7361 6765 720c 0000 00da  e..Messager.....
+00001440: 0f52 6567 6973 7465 724d 6573 7361 6765  .RegisterMessage
+00001450: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+00001460: 1000 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
+00001470: 0000 0072 1400 0000 da10 7365 7276 6963  ...r......servic
+00001480: 6573 5f62 795f 6e61 6d65 5a0c 5f56 4945  es_by_nameZ._VIE
+00001490: 5753 4552 5649 4345 da12 5f55 5345 5f43  WSERVICE.._USE_C
+000014a0: 5f44 4553 4352 4950 544f 5253 da08 5f6f  _DESCRIPTORS.._o
+000014b0: 7074 696f 6e73 da13 5f73 6572 6961 6c69  ptions.._seriali
+000014c0: 7a65 645f 6f70 7469 6f6e 73da 0e66 6965  zed_options..fie
+000014d0: 6c64 735f 6279 5f6e 616d 65da 0f6d 6574  lds_by_name..met
+000014e0: 686f 6473 5f62 795f 6e61 6d65 da11 5f73  hods_by_name.._s
+000014f0: 6572 6961 6c69 7a65 645f 7374 6172 74da  erialized_start.
+00001500: 0f5f 7365 7269 616c 697a 6564 5f65 6e64  ._serialized_end
+00001510: a900 723c 0000 0072 3c00 0000 fa34 2f73  ..r<...r<....4/s
+00001520: 7263 2f73 7263 2f6b 6173 6b61 6461 2f6b  rc/src/kaskada/k
+00001530: 6173 6b61 6461 2f76 3161 6c70 6861 2f76  askada/v1alpha/v
+00001540: 6965 775f 7365 7276 6963 655f 7062 322e  iew_service_pb2.
+00001550: 7079 da08 3c6d 6f64 756c 653e 0400 0000  py..<module>....
+00001560: 73e8 0000 0004 010c 010c 010c 010c 010c  s...............
+00001570: 0308 030c 010c 010c 010c 010c 030e 040a  ................
+00001580: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00001590: 010c 0102 0102 fe08 050a 020c 0102 0102  ................
+000015a0: fe08 050a 020c 0102 0102 fe08 050a 020c  ................
+000015b0: 0102 0102 fe08 050a 020c 0102 0102 fe08  ................
+000015c0: 050a 020c 0102 0102 fe08 050a 020c 0102  ................
+000015d0: 0102 fe08 050a 020c 0102 0102 fe08 050a  ................
+000015e0: 020c 0102 0102 fe08 050a 020a 010c 0206  ................
+000015f0: 0106 010c 010c 010c 010c 010c 010c 010c  ................
+00001600: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00001610: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00001620: 010c 010c 010c 0106 0106 0106 0106 0106  ................
+00001630: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00001640: 0106 0106 0106 0106 0106 0106 01         .............
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/view_service_pb2_grpc.cpython-310.pyc` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/__pycache__/view_service_pb2_grpc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 23:44:52 2023 UTC, .py size: 8153 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 f4f0 3564 d91f 0000  o.........5d....
+00000000: 610d 0d0a 0000 0000 2038 4164 d91f 0000  a....... 8Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a04 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000050: 6505 8303 5a06 4700 6406 6407 8400 6407  e...Z.G.d.d...d.
 00000060: 6505 8303 5a07 6408 6409 8400 5a08 4700  e...Z.d.d...Z.G.
 00000070: 640a 640b 8400 640b 6505 8303 5a09 6402  d.d...d.e...Z.d.
@@ -63,209 +63,222 @@
 000003e0: 6965 7752 6571 7565 7374 da12 4372 6561  iewRequest..Crea
 000003f0: 7465 5669 6577 5265 7370 6f6e 7365 da0a  teViewResponse..
 00000400: 4372 6561 7465 5669 6577 da11 4465 6c65  CreateView..Dele
 00000410: 7465 5669 6577 5265 7175 6573 74da 1244  teViewRequest..D
 00000420: 656c 6574 6556 6965 7752 6573 706f 6e73  eleteViewRespons
 00000430: 65da 0a44 656c 6574 6556 6965 7729 02da  e..DeleteView)..
 00000440: 0473 656c 66da 0763 6861 6e6e 656c a900  .self..channel..
-00000450: 721d 0000 00fa 7b2f 686f 6d65 2f74 6865  r.....{/home/the
-00000460: 7261 706f 6e2f 5265 706f 732f 4769 7448  rapon/Repos/GitH
-00000470: 7562 2f4b 6173 6b61 6461 4149 2f6b 6173  ub/KaskadaAI/kas
-00000480: 6b61 6461 2f72 656c 6561 7369 6e67 2f63  kada/releasing/c
-00000490: 6c69 656e 7473 2f70 7974 686f 6e2f 7372  lients/python/sr
-000004a0: 632f 6b61 736b 6164 612f 6b61 736b 6164  c/kaskada/kaskad
-000004b0: 612f 7631 616c 7068 612f 7669 6577 5f73  a/v1alpha/view_s
-000004c0: 6572 7669 6365 5f70 6232 5f67 7270 632e  ervice_pb2_grpc.
-000004d0: 7079 da08 5f5f 696e 6974 5f5f 0c00 0000  py..__init__....
-000004e0: 7328 0000 0004 0602 0106 0106 0108 fd04  s(..............
-000004f0: 0502 0106 0106 0108 fd04 0502 0106 0106  ................
-00000500: 0108 fd04 0502 0106 0106 010c fd7a 1856  .............z.V
-00000510: 6965 7753 6572 7669 6365 5374 7562 2e5f  iewServiceStub._
-00000520: 5f69 6e69 745f 5f4e 2905 da08 5f5f 6e61  _init__N)...__na
-00000530: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000540: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00000550: 5f5f 646f 635f 5f72 1f00 0000 721d 0000  __doc__r....r...
-00000560: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00000570: 7203 0000 0008 0000 0073 0600 0000 0800  r........s......
-00000580: 0401 0c03 7203 0000 0063 0000 0000 0000  ....r....c......
-00000590: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-000005a0: 0000 7330 0000 0065 005a 0164 005a 0264  ..s0...e.Z.d.Z.d
-000005b0: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
-000005c0: 005a 0564 0664 0784 005a 0664 0864 0984  .Z.d.d...Z.d.d..
-000005d0: 005a 0764 0a53 0029 0bda 1356 6965 7753  .Z.d.S.)...ViewS
-000005e0: 6572 7669 6365 5365 7276 6963 6572 7204  erviceServicerr.
-000005f0: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00000600: 0300 0000 0300 0000 4300 0000 f320 0000  ........C.... ..
-00000610: 007c 02a0 0074 016a 026a 03a1 0101 007c  .|...t.j.j.....|
-00000620: 02a0 0464 01a1 0101 0074 0564 0183 0182  ...d.....t.d....
-00000630: 0129 027a c34c 6973 7473 2076 6965 7773  .).z.Lists views
-00000640: 2e0a 0a20 2020 2020 2020 2054 6865 2072  ...        The r
-00000650: 6573 706f 6e73 6520 696e 636c 7564 6573  esponse includes
-00000660: 2061 6c6c 2056 6965 7773 2064 6566 696e   all Views defin
-00000670: 6564 2066 6f72 2074 6865 204b 6173 6b61  ed for the Kaska
-00000680: 6461 2061 6363 6f75 6e74 2e0a 2020 2020  da account..    
-00000690: 2020 2020 4966 2061 2073 6561 7263 6820      If a search 
-000006a0: 7374 7269 6e67 2069 7320 7072 6f76 6964  string is provid
-000006b0: 6564 2c20 6f6e 6c79 2056 6965 7773 206d  ed, only Views m
-000006c0: 6174 6368 696e 6720 7468 6520 7365 6172  atching the sear
-000006d0: 6368 2073 7472 696e 670a 2020 2020 2020  ch string.      
-000006e0: 2020 6172 6520 7265 7475 726e 6564 2e0a    are returned..
-000006f0: 2020 2020 2020 2020 fa17 4d65 7468 6f64          ..Method
-00000700: 206e 6f74 2069 6d70 6c65 6d65 6e74 6564   not implemented
-00000710: 21a9 06da 0873 6574 5f63 6f64 65da 0467  !....set_code..g
-00000720: 7270 63da 0a53 7461 7475 7343 6f64 65da  rpc..StatusCode.
-00000730: 0d55 4e49 4d50 4c45 4d45 4e54 4544 da0b  .UNIMPLEMENTED..
-00000740: 7365 745f 6465 7461 696c 73da 134e 6f74  set_details..Not
-00000750: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-00000760: a903 721b 0000 00da 0772 6571 7565 7374  ..r......request
-00000770: da07 636f 6e74 6578 7472 1d00 0000 721d  ..contextr....r.
-00000780: 0000 0072 1e00 0000 7211 0000 002c 0000  ...r....r....,..
-00000790: 0073 0600 0000 0e07 0a01 0801 7a1d 5669  .s..........z.Vi
-000007a0: 6577 5365 7276 6963 6553 6572 7669 6365  ewServiceService
-000007b0: 722e 4c69 7374 5669 6577 7363 0300 0000  r.ListViewsc....
-000007c0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-000007d0: 4300 0000 7225 0000 0029 027a 1547 6574  C...r%...).z.Get
-000007e0: 7320 6120 7669 6577 2e0a 2020 2020 2020  s a view..      
-000007f0: 2020 7226 0000 0072 2700 0000 722e 0000    r&...r'...r...
-00000800: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00000810: 7214 0000 0037 0000 00f3 0600 0000 0e03  r....7..........
-00000820: 0a01 0801 7a1b 5669 6577 5365 7276 6963  ....z.ViewServic
-00000830: 6553 6572 7669 6365 722e 4765 7456 6965  eServicer.GetVie
-00000840: 7763 0300 0000 0000 0000 0000 0000 0300  wc..............
-00000850: 0000 0300 0000 4300 0000 7225 0000 0029  ......C...r%...)
-00000860: 027a 1843 7265 6174 6573 2061 2076 6965  .z.Creates a vie
-00000870: 772e 0a20 2020 2020 2020 2072 2600 0000  w..        r&...
-00000880: 7227 0000 0072 2e00 0000 721d 0000 0072  r'...r....r....r
-00000890: 1d00 0000 721e 0000 0072 1700 0000 3e00  ....r....r....>.
-000008a0: 0000 7231 0000 007a 1e56 6965 7753 6572  ..r1...z.ViewSer
-000008b0: 7669 6365 5365 7276 6963 6572 2e43 7265  viceServicer.Cre
-000008c0: 6174 6556 6965 7763 0300 0000 0000 0000  ateViewc........
-000008d0: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
-000008e0: 7225 0000 0029 027a 1844 656c 6574 6573  r%...).z.Deletes
-000008f0: 2061 2076 6965 772e 0a20 2020 2020 2020   a view..       
-00000900: 2072 2600 0000 7227 0000 0072 2e00 0000   r&...r'...r....
-00000910: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000920: 1a00 0000 4500 0000 7231 0000 007a 1e56  ....E...r1...z.V
-00000930: 6965 7753 6572 7669 6365 5365 7276 6963  iewServiceServic
-00000940: 6572 2e44 656c 6574 6556 6965 774e 2908  er.DeleteViewN).
-00000950: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
-00000960: 2300 0000 7211 0000 0072 1400 0000 7217  #...r....r....r.
-00000970: 0000 0072 1a00 0000 721d 0000 0072 1d00  ...r....r....r..
-00000980: 0000 721d 0000 0072 1e00 0000 7224 0000  ..r....r....r$..
-00000990: 0028 0000 0073 0c00 0000 0800 0401 0803  .(...s..........
-000009a0: 080b 0807 0c07 7224 0000 0063 0200 0000  ......r$...c....
-000009b0: 0000 0000 0000 0000 0400 0000 0800 0000  ................
-000009c0: 4300 0000 7382 0000 0074 006a 017c 006a  C...s....t.j.|.j
-000009d0: 0274 036a 046a 0574 036a 066a 0764 018d  .t.j.j.t.j.j.d..
-000009e0: 0374 006a 017c 006a 0874 036a 096a 0574  .t.j.|.j.t.j.j.t
-000009f0: 036a 0a6a 0764 018d 0374 006a 017c 006a  .j.j.d...t.j.|.j
-00000a00: 0b74 036a 0c6a 0574 036a 0d6a 0764 018d  .t.j.j.t.j.j.d..
-00000a10: 0374 006a 017c 006a 0e74 036a 0f6a 0574  .t.j.|.j.t.j.j.t
-00000a20: 036a 106a 0764 018d 0364 029c 047d 0274  .j.j.d...d...}.t
-00000a30: 00a0 1164 037c 02a1 027d 037c 01a0 127c  ...d.|...}.|...|
-00000a40: 0366 01a1 0101 0064 0053 0029 044e 2902  .f.....d.S.).N).
-00000a50: da14 7265 7175 6573 745f 6465 7365 7269  ..request_deseri
-00000a60: 616c 697a 6572 da13 7265 7370 6f6e 7365  alizer..response
-00000a70: 5f73 6572 6961 6c69 7a65 7229 0472 1100  _serializer).r..
-00000a80: 0000 7214 0000 0072 1700 0000 721a 0000  ..r....r....r...
-00000a90: 007a 236b 6173 6b61 6461 2e6b 6173 6b61  .z#kaskada.kaska
-00000aa0: 6461 2e76 3161 6c70 6861 2e56 6965 7753  da.v1alpha.ViewS
-00000ab0: 6572 7669 6365 2913 7229 0000 00da 1e75  ervice).r).....u
-00000ac0: 6e61 7279 5f75 6e61 7279 5f72 7063 5f6d  nary_unary_rpc_m
-00000ad0: 6574 686f 645f 6861 6e64 6c65 7272 1100  ethod_handlerr..
-00000ae0: 0000 720c 0000 0072 0d00 0000 7210 0000  ..r....r....r...
-00000af0: 0072 0f00 0000 720e 0000 0072 1400 0000  .r....r....r....
-00000b00: 7212 0000 0072 1300 0000 7217 0000 0072  r....r....r....r
-00000b10: 1500 0000 7216 0000 0072 1a00 0000 7218  ....r....r....r.
-00000b20: 0000 0072 1900 0000 da1f 6d65 7468 6f64  ...r......method
-00000b30: 5f68 616e 646c 6572 735f 6765 6e65 7269  _handlers_generi
-00000b40: 635f 6861 6e64 6c65 72da 1861 6464 5f67  c_handler..add_g
-00000b50: 656e 6572 6963 5f72 7063 5f68 616e 646c  eneric_rpc_handl
-00000b60: 6572 7329 04da 0873 6572 7669 6365 72da  ers)...servicer.
-00000b70: 0673 6572 7665 72da 1372 7063 5f6d 6574  .server..rpc_met
-00000b80: 686f 645f 6861 6e64 6c65 7273 da0f 6765  hod_handlers..ge
-00000b90: 6e65 7269 635f 6861 6e64 6c65 7272 1d00  neric_handlerr..
-00000ba0: 0000 721d 0000 0072 1e00 0000 da21 6164  ..r....r.....!ad
-00000bb0: 645f 5669 6577 5365 7276 6963 6553 6572  d_ViewServiceSer
-00000bc0: 7669 6365 725f 746f 5f73 6572 7665 724d  vicer_to_serverM
-00000bd0: 0000 0073 3200 0000 0402 0401 0601 0601  ...s2...........
-00000be0: 04fd 0405 0401 0601 0601 04fd 0405 0401  ................
-00000bf0: 0601 0601 04fd 0405 0401 0601 0601 04fd  ................
-00000c00: 06f0 0416 0401 04ff 1002 723b 0000 0063  ..........r;...c
-00000c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c20: 0400 0000 4000 0000 7388 0000 0065 005a  ....@...s....e.Z
-00000c30: 0164 005a 0264 015a 0365 0409 0209 0309  .d.Z.d.Z.e......
-00000c40: 0309 0409 0309 0309 0309 0364 0d64 0564  ...........d.d.d
-00000c50: 0684 0183 015a 0565 0409 0209 0309 0309  .....Z.e........
-00000c60: 0409 0309 0309 0309 0364 0d64 0764 0884  .........d.d.d..
-00000c70: 0183 015a 0665 0409 0209 0309 0309 0409  ...Z.e..........
-00000c80: 0309 0309 0309 0364 0d64 0964 0a84 0183  .......d.d.d....
-00000c90: 015a 0765 0409 0209 0309 0309 0409 0309  .Z.e............
-00000ca0: 0309 0309 0364 0d64 0b64 0c84 0183 015a  .....d.d.d.....Z
-00000cb0: 0864 0353 0029 0eda 0b56 6965 7753 6572  .d.S.)...ViewSer
-00000cc0: 7669 6365 7204 0000 0072 1d00 0000 4e46  vicer....r....NF
-00000cd0: 630a 0000 0000 0000 0000 0000 000a 0000  c...............
-00000ce0: 000f 0000 0043 0000 00f3 2c00 0000 7400  .....C....,...t.
-00000cf0: 6a01 a002 7c00 7c01 6401 7403 6a04 6a05  j...|.|.d.t.j.j.
-00000d00: 7403 6a06 6a07 7c02 7c03 7c05 7c04 7c06  t.j.j.|.|.|.|.|.
-00000d10: 7c07 7c08 7c09 a10d 5300 2902 4e72 0500  |.|.|...S.).Nr..
-00000d20: 0000 2908 7229 0000 00da 0c65 7870 6572  ..).r).....exper
-00000d30: 696d 656e 7461 6c72 0b00 0000 720c 0000  imentalr....r...
-00000d40: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00000d50: 7210 0000 00a9 0a72 2f00 0000 da06 7461  r......r/.....ta
-00000d60: 7267 6574 da07 6f70 7469 6f6e 73da 1363  rget..options..c
-00000d70: 6861 6e6e 656c 5f63 7265 6465 6e74 6961  hannel_credentia
-00000d80: 6c73 da10 6361 6c6c 5f63 7265 6465 6e74  ls..call_credent
-00000d90: 6961 6c73 da08 696e 7365 6375 7265 da0b  ials..insecure..
-00000da0: 636f 6d70 7265 7373 696f 6eda 0e77 6169  compression..wai
-00000db0: 745f 666f 725f 7265 6164 79da 0774 696d  t_for_ready..tim
-00000dc0: 656f 7574 da08 6d65 7461 6461 7461 721d  eout..metadatar.
-00000dd0: 0000 0072 1d00 0000 721e 0000 0072 1100  ...r....r....r..
-00000de0: 0000 6e00 0000 f30c 0000 000c 0b06 0106  ..n.............
-00000df0: 0104 010c 0104 fc7a 1556 6965 7753 6572  .......z.ViewSer
-00000e00: 7669 6365 2e4c 6973 7456 6965 7773 630a  vice.ListViewsc.
-00000e10: 0000 0000 0000 0000 0000 000a 0000 000f  ................
-00000e20: 0000 0043 0000 0072 3d00 0000 2902 4e72  ...C...r=...).Nr
-00000e30: 0800 0000 2908 7229 0000 0072 3e00 0000  ....).r)...r>...
-00000e40: 720b 0000 0072 0c00 0000 7212 0000 0072  r....r....r....r
-00000e50: 0e00 0000 7213 0000 0072 1000 0000 723f  ....r....r....r?
-00000e60: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
-00000e70: 0000 7214 0000 007f 0000 0072 4900 0000  ..r........rI...
-00000e80: 7a13 5669 6577 5365 7276 6963 652e 4765  z.ViewService.Ge
-00000e90: 7456 6965 7763 0a00 0000 0000 0000 0000  tViewc..........
-00000ea0: 0000 0a00 0000 0f00 0000 4300 0000 723d  ..........C...r=
-00000eb0: 0000 0029 024e 7209 0000 0029 0872 2900  ...).Nr....).r).
-00000ec0: 0000 723e 0000 0072 0b00 0000 720c 0000  ..r>...r....r...
-00000ed0: 0072 1500 0000 720e 0000 0072 1600 0000  .r....r....r....
-00000ee0: 7210 0000 0072 3f00 0000 721d 0000 0072  r....r?...r....r
-00000ef0: 1d00 0000 721e 0000 0072 1700 0000 9000  ....r....r......
-00000f00: 0000 7249 0000 007a 1656 6965 7753 6572  ..rI...z.ViewSer
-00000f10: 7669 6365 2e43 7265 6174 6556 6965 7763  vice.CreateViewc
-00000f20: 0a00 0000 0000 0000 0000 0000 0a00 0000  ................
-00000f30: 0f00 0000 4300 0000 723d 0000 0029 024e  ....C...r=...).N
-00000f40: 720a 0000 0029 0872 2900 0000 723e 0000  r....).r)...r>..
-00000f50: 0072 0b00 0000 720c 0000 0072 1800 0000  .r....r....r....
-00000f60: 720e 0000 0072 1900 0000 7210 0000 0072  r....r....r....r
-00000f70: 3f00 0000 721d 0000 0072 1d00 0000 721e  ?...r....r....r.
-00000f80: 0000 0072 1a00 0000 a100 0000 7249 0000  ...r........rI..
-00000f90: 007a 1656 6965 7753 6572 7669 6365 2e44  .z.ViewService.D
-00000fa0: 656c 6574 6556 6965 7729 0872 1d00 0000  eleteView).r....
-00000fb0: 4e4e 464e 4e4e 4e29 0972 2000 0000 7221  NNFNNNN).r ...r!
-00000fc0: 0000 0072 2200 0000 7223 0000 00da 0c73  ...r"...r#.....s
-00000fd0: 7461 7469 636d 6574 686f 6472 1100 0000  taticmethodr....
-00000fe0: 7214 0000 0072 1700 0000 721a 0000 0072  r....r....r....r
-00000ff0: 1d00 0000 721d 0000 0072 1d00 0000 721e  ....r....r....r.
-00001000: 0000 0072 3c00 0000 6a00 0000 7354 0000  ...r<...j...sT..
-00001010: 0008 0004 0102 0302 0302 0102 0102 0102  ................
-00001020: 0102 0102 0102 010c f702 1002 0302 0102  ................
-00001030: 0102 0102 0102 0102 0102 010c f702 1002  ................
-00001040: 0302 0102 0102 0102 0102 0102 0102 010c  ................
-00001050: f702 1002 0302 0102 0102 0102 0102 0102  ................
-00001060: 0102 0110 f772 3c00 0000 290a 7223 0000  .....r<...).r#..
-00001070: 0072 2900 0000 da17 6b61 736b 6164 612e  .r).....kaskada.
-00001080: 6b61 736b 6164 612e 7631 616c 7068 6172  kaskada.v1alphar
-00001090: 0200 0000 720c 0000 00da 066f 626a 6563  ....r......objec
-000010a0: 7472 0300 0000 7224 0000 0072 3b00 0000  tr....r$...r;...
-000010b0: 723c 0000 0072 1d00 0000 721d 0000 0072  r<...r....r....r
-000010c0: 1d00 0000 721e 0000 00da 083c 6d6f 6475  ....r......<modu
-000010d0: 6c65 3e01 0000 0073 0e00 0000 0401 0801  le>....s........
-000010e0: 0c02 1003 1020 0825 141d                 ..... .%..
+00000450: 721d 0000 00fa 392f 7372 632f 7372 632f  r.....9/src/src/
+00000460: 6b61 736b 6164 612f 6b61 736b 6164 612f  kaskada/kaskada/
+00000470: 7631 616c 7068 612f 7669 6577 5f73 6572  v1alpha/view_ser
+00000480: 7669 6365 5f70 6232 5f67 7270 632e 7079  vice_pb2_grpc.py
+00000490: da08 5f5f 696e 6974 5f5f 0c00 0000 7328  ..__init__....s(
+000004a0: 0000 0000 0604 0102 0106 0106 fd08 0504  ................
+000004b0: 0102 0106 0106 fd08 0504 0102 0106 0106  ................
+000004c0: fd08 0504 0102 0106 0106 fd7a 1856 6965  ...........z.Vie
+000004d0: 7753 6572 7669 6365 5374 7562 2e5f 5f69  wServiceStub.__i
+000004e0: 6e69 745f 5f4e 2905 da08 5f5f 6e61 6d65  nit__N)...__name
+000004f0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000500: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+00000510: 646f 635f 5f72 1f00 0000 721d 0000 0072  doc__r....r....r
+00000520: 1d00 0000 721d 0000 0072 1e00 0000 7203  ....r....r....r.
+00000530: 0000 0008 0000 0073 0400 0000 0801 0403  .......s........
+00000540: 7203 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000550: 0000 0000 0000 0200 0000 4000 0000 7330  ..........@...s0
+00000560: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00000570: 0264 0384 005a 0464 0464 0584 005a 0564  .d...Z.d.d...Z.d
+00000580: 0664 0784 005a 0664 0864 0984 005a 0764  .d...Z.d.d...Z.d
+00000590: 0a53 0029 0bda 1356 6965 7753 6572 7669  .S.)...ViewServi
+000005a0: 6365 5365 7276 6963 6572 7204 0000 0063  ceServicerr....c
+000005b0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+000005c0: 0300 0000 4300 0000 7324 0000 007c 02a0  ....C...s$...|..
+000005d0: 0074 016a 026a 03a1 0101 007c 02a0 0464  .t.j.j.....|...d
+000005e0: 01a1 0101 0074 0564 0183 0182 0164 0253  .....t.d.....d.S
+000005f0: 0029 037a c34c 6973 7473 2076 6965 7773  .).z.Lists views
+00000600: 2e0a 0a20 2020 2020 2020 2054 6865 2072  ...        The r
+00000610: 6573 706f 6e73 6520 696e 636c 7564 6573  esponse includes
+00000620: 2061 6c6c 2056 6965 7773 2064 6566 696e   all Views defin
+00000630: 6564 2066 6f72 2074 6865 204b 6173 6b61  ed for the Kaska
+00000640: 6461 2061 6363 6f75 6e74 2e0a 2020 2020  da account..    
+00000650: 2020 2020 4966 2061 2073 6561 7263 6820      If a search 
+00000660: 7374 7269 6e67 2069 7320 7072 6f76 6964  string is provid
+00000670: 6564 2c20 6f6e 6c79 2056 6965 7773 206d  ed, only Views m
+00000680: 6174 6368 696e 6720 7468 6520 7365 6172  atching the sear
+00000690: 6368 2073 7472 696e 670a 2020 2020 2020  ch string.      
+000006a0: 2020 6172 6520 7265 7475 726e 6564 2e0a    are returned..
+000006b0: 2020 2020 2020 2020 fa17 4d65 7468 6f64          ..Method
+000006c0: 206e 6f74 2069 6d70 6c65 6d65 6e74 6564   not implemented
+000006d0: 214e a906 da08 7365 745f 636f 6465 da04  !N....set_code..
+000006e0: 6772 7063 da0a 5374 6174 7573 436f 6465  grpc..StatusCode
+000006f0: da0d 554e 494d 504c 454d 454e 5445 44da  ..UNIMPLEMENTED.
+00000700: 0b73 6574 5f64 6574 6169 6c73 da13 4e6f  .set_details..No
+00000710: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
+00000720: 72a9 0372 1b00 0000 da07 7265 7175 6573  r..r......reques
+00000730: 74da 0763 6f6e 7465 7874 721d 0000 0072  t..contextr....r
+00000740: 1d00 0000 721e 0000 0072 1100 0000 2c00  ....r....r....,.
+00000750: 0000 7306 0000 0000 070e 010a 017a 1d56  ..s..........z.V
+00000760: 6965 7753 6572 7669 6365 5365 7276 6963  iewServiceServic
+00000770: 6572 2e4c 6973 7456 6965 7773 6303 0000  er.ListViewsc...
+00000780: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00000790: 0043 0000 0073 2400 0000 7c02 a000 7401  .C...s$...|...t.
+000007a0: 6a02 6a03 a101 0100 7c02 a004 6401 a101  j.j.....|...d...
+000007b0: 0100 7405 6401 8301 8201 6402 5300 2903  ..t.d.....d.S.).
+000007c0: 7a15 4765 7473 2061 2076 6965 772e 0a20  z.Gets a view.. 
+000007d0: 2020 2020 2020 2072 2500 0000 4e72 2600         r%...Nr&.
+000007e0: 0000 722d 0000 0072 1d00 0000 721d 0000  ..r-...r....r...
+000007f0: 0072 1e00 0000 7214 0000 0037 0000 0073  .r....r....7...s
+00000800: 0600 0000 0003 0e01 0a01 7a1b 5669 6577  ..........z.View
+00000810: 5365 7276 6963 6553 6572 7669 6365 722e  ServiceServicer.
+00000820: 4765 7456 6965 7763 0300 0000 0000 0000  GetViewc........
+00000830: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
+00000840: 7324 0000 007c 02a0 0074 016a 026a 03a1  s$...|...t.j.j..
+00000850: 0101 007c 02a0 0464 01a1 0101 0074 0564  ...|...d.....t.d
+00000860: 0183 0182 0164 0253 0029 037a 1843 7265  .....d.S.).z.Cre
+00000870: 6174 6573 2061 2076 6965 772e 0a20 2020  ates a view..   
+00000880: 2020 2020 2072 2500 0000 4e72 2600 0000       r%...Nr&...
+00000890: 722d 0000 0072 1d00 0000 721d 0000 0072  r-...r....r....r
+000008a0: 1e00 0000 7217 0000 003e 0000 0073 0600  ....r....>...s..
+000008b0: 0000 0003 0e01 0a01 7a1e 5669 6577 5365  ........z.ViewSe
+000008c0: 7276 6963 6553 6572 7669 6365 722e 4372  rviceServicer.Cr
+000008d0: 6561 7465 5669 6577 6303 0000 0000 0000  eateViewc.......
+000008e0: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
+000008f0: 0073 2400 0000 7c02 a000 7401 6a02 6a03  .s$...|...t.j.j.
+00000900: a101 0100 7c02 a004 6401 a101 0100 7405  ....|...d.....t.
+00000910: 6401 8301 8201 6402 5300 2903 7a18 4465  d.....d.S.).z.De
+00000920: 6c65 7465 7320 6120 7669 6577 2e0a 2020  letes a view..  
+00000930: 2020 2020 2020 7225 0000 004e 7226 0000        r%...Nr&..
+00000940: 0072 2d00 0000 721d 0000 0072 1d00 0000  .r-...r....r....
+00000950: 721e 0000 0072 1a00 0000 4500 0000 7306  r....r....E...s.
+00000960: 0000 0000 030e 010a 017a 1e56 6965 7753  .........z.ViewS
+00000970: 6572 7669 6365 5365 7276 6963 6572 2e44  erviceServicer.D
+00000980: 656c 6574 6556 6965 774e 2908 7220 0000  eleteViewN).r ..
+00000990: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
+000009a0: 7211 0000 0072 1400 0000 7217 0000 0072  r....r....r....r
+000009b0: 1a00 0000 721d 0000 0072 1d00 0000 721d  ....r....r....r.
+000009c0: 0000 0072 1e00 0000 7224 0000 0028 0000  ...r....r$...(..
+000009d0: 0073 0a00 0000 0801 0403 080b 0807 0807  .s..............
+000009e0: 7224 0000 0063 0200 0000 0000 0000 0000  r$...c..........
+000009f0: 0000 0400 0000 0800 0000 4300 0000 7382  ..........C...s.
+00000a00: 0000 0074 006a 017c 006a 0274 036a 046a  ...t.j.|.j.t.j.j
+00000a10: 0574 036a 066a 0764 018d 0374 006a 017c  .t.j.j.d...t.j.|
+00000a20: 006a 0874 036a 096a 0574 036a 0a6a 0764  .j.t.j.j.t.j.j.d
+00000a30: 018d 0374 006a 017c 006a 0b74 036a 0c6a  ...t.j.|.j.t.j.j
+00000a40: 0574 036a 0d6a 0764 018d 0374 006a 017c  .t.j.j.d...t.j.|
+00000a50: 006a 0e74 036a 0f6a 0574 036a 106a 0764  .j.t.j.j.t.j.j.d
+00000a60: 018d 0364 029c 047d 0274 00a0 1164 037c  ...d...}.t...d.|
+00000a70: 02a1 027d 037c 01a0 127c 0366 01a1 0101  ...}.|...|.f....
+00000a80: 0064 0053 0029 044e 2902 da14 7265 7175  .d.S.).N)...requ
+00000a90: 6573 745f 6465 7365 7269 616c 697a 6572  est_deserializer
+00000aa0: da13 7265 7370 6f6e 7365 5f73 6572 6961  ..response_seria
+00000ab0: 6c69 7a65 7229 0472 1100 0000 7214 0000  lizer).r....r...
+00000ac0: 0072 1700 0000 721a 0000 007a 236b 6173  .r....r....z#kas
+00000ad0: 6b61 6461 2e6b 6173 6b61 6461 2e76 3161  kada.kaskada.v1a
+00000ae0: 6c70 6861 2e56 6965 7753 6572 7669 6365  lpha.ViewService
+00000af0: 2913 7228 0000 00da 1e75 6e61 7279 5f75  ).r(.....unary_u
+00000b00: 6e61 7279 5f72 7063 5f6d 6574 686f 645f  nary_rpc_method_
+00000b10: 6861 6e64 6c65 7272 1100 0000 720c 0000  handlerr....r...
+00000b20: 0072 0d00 0000 7210 0000 0072 0f00 0000  .r....r....r....
+00000b30: 720e 0000 0072 1400 0000 7212 0000 0072  r....r....r....r
+00000b40: 1300 0000 7217 0000 0072 1500 0000 7216  ....r....r....r.
+00000b50: 0000 0072 1a00 0000 7218 0000 0072 1900  ...r....r....r..
+00000b60: 0000 da1f 6d65 7468 6f64 5f68 616e 646c  ....method_handl
+00000b70: 6572 735f 6765 6e65 7269 635f 6861 6e64  ers_generic_hand
+00000b80: 6c65 72da 1861 6464 5f67 656e 6572 6963  ler..add_generic
+00000b90: 5f72 7063 5f68 616e 646c 6572 7329 04da  _rpc_handlers)..
+00000ba0: 0873 6572 7669 6365 72da 0673 6572 7665  .servicer..serve
+00000bb0: 72da 1372 7063 5f6d 6574 686f 645f 6861  r..rpc_method_ha
+00000bc0: 6e64 6c65 7273 da0f 6765 6e65 7269 635f  ndlers..generic_
+00000bd0: 6861 6e64 6c65 7272 1d00 0000 721d 0000  handlerr....r...
+00000be0: 0072 1e00 0000 da21 6164 645f 5669 6577  .r.....!add_View
+00000bf0: 5365 7276 6963 6553 6572 7669 6365 725f  ServiceServicer_
+00000c00: 746f 5f73 6572 7665 724d 0000 0073 3200  to_serverM...s2.
+00000c10: 0000 0002 0401 0401 0601 06fd 0405 0401  ................
+00000c20: 0401 0601 06fd 0405 0401 0401 0601 06fd  ................
+00000c30: 0405 0401 0401 0601 06fd 04f0 0616 0401  ................
+00000c40: 04ff 0402 7239 0000 0063 0000 0000 0000  ....r9...c......
+00000c50: 0000 0000 0000 0000 0000 0900 0000 4000  ..............@.
+00000c60: 0000 7348 0000 0065 005a 0164 005a 0264  ..sH...e.Z.d.Z.d
+00000c70: 015a 0365 0464 0d64 0564 0684 0183 015a  .Z.e.d.d.d.....Z
+00000c80: 0565 0464 0e64 0764 0884 0183 015a 0665  .e.d.d.d.....Z.e
+00000c90: 0464 0f64 0964 0a84 0183 015a 0765 0464  .d.d.d.....Z.e.d
+00000ca0: 1064 0b64 0c84 0183 015a 0864 0353 0029  .d.d.....Z.d.S.)
+00000cb0: 11da 0b56 6965 7753 6572 7669 6365 7204  ...ViewServicer.
+00000cc0: 0000 0072 1d00 0000 4e46 630a 0000 0000  ...r....NFc.....
+00000cd0: 0000 0000 0000 000a 0000 000f 0000 0043  ...............C
+00000ce0: 0000 0073 2c00 0000 7400 6a01 a002 7c00  ...s,...t.j...|.
+00000cf0: 7c01 6401 7403 6a04 6a05 7403 6a06 6a07  |.d.t.j.j.t.j.j.
+00000d00: 7c02 7c03 7c05 7c04 7c06 7c07 7c08 7c09  |.|.|.|.|.|.|.|.
+00000d10: a10d 5300 2902 4e72 0500 0000 2908 7228  ..S.).Nr....).r(
+00000d20: 0000 00da 0c65 7870 6572 696d 656e 7461  .....experimenta
+00000d30: 6c72 0b00 0000 720c 0000 0072 0d00 0000  lr....r....r....
+00000d40: 720e 0000 0072 0f00 0000 7210 0000 00a9  r....r....r.....
+00000d50: 0a72 2e00 0000 da06 7461 7267 6574 da07  .r......target..
+00000d60: 6f70 7469 6f6e 73da 1363 6861 6e6e 656c  options..channel
+00000d70: 5f63 7265 6465 6e74 6961 6c73 da10 6361  _credentials..ca
+00000d80: 6c6c 5f63 7265 6465 6e74 6961 6c73 da08  ll_credentials..
+00000d90: 696e 7365 6375 7265 da0b 636f 6d70 7265  insecure..compre
+00000da0: 7373 696f 6eda 0e77 6169 745f 666f 725f  ssion..wait_for_
+00000db0: 7265 6164 79da 0774 696d 656f 7574 da08  ready..timeout..
+00000dc0: 6d65 7461 6461 7461 721d 0000 0072 1d00  metadatar....r..
+00000dd0: 0000 721e 0000 0072 1100 0000 6e00 0000  ..r....r....n...
+00000de0: 730c 0000 0000 0b0c 0106 0106 0104 010c  s...............
+00000df0: fc7a 1556 6965 7753 6572 7669 6365 2e4c  .z.ViewService.L
+00000e00: 6973 7456 6965 7773 630a 0000 0000 0000  istViewsc.......
+00000e10: 0000 0000 000a 0000 000f 0000 0043 0000  .............C..
+00000e20: 0073 2c00 0000 7400 6a01 a002 7c00 7c01  .s,...t.j...|.|.
+00000e30: 6401 7403 6a04 6a05 7403 6a06 6a07 7c02  d.t.j.j.t.j.j.|.
+00000e40: 7c03 7c05 7c04 7c06 7c07 7c08 7c09 a10d  |.|.|.|.|.|.|...
+00000e50: 5300 2902 4e72 0800 0000 2908 7228 0000  S.).Nr....).r(..
+00000e60: 0072 3b00 0000 720b 0000 0072 0c00 0000  .r;...r....r....
+00000e70: 7212 0000 0072 0e00 0000 7213 0000 0072  r....r....r....r
+00000e80: 1000 0000 723c 0000 0072 1d00 0000 721d  ....r<...r....r.
+00000e90: 0000 0072 1e00 0000 7214 0000 007f 0000  ...r....r.......
+00000ea0: 0073 0c00 0000 000b 0c01 0601 0601 0401  .s..............
+00000eb0: 0cfc 7a13 5669 6577 5365 7276 6963 652e  ..z.ViewService.
+00000ec0: 4765 7456 6965 7763 0a00 0000 0000 0000  GetViewc........
+00000ed0: 0000 0000 0a00 0000 0f00 0000 4300 0000  ............C...
+00000ee0: 732c 0000 0074 006a 01a0 027c 007c 0164  s,...t.j...|.|.d
+00000ef0: 0174 036a 046a 0574 036a 066a 077c 027c  .t.j.j.t.j.j.|.|
+00000f00: 037c 057c 047c 067c 077c 087c 09a1 0d53  .|.|.|.|.|.|...S
+00000f10: 0029 024e 7209 0000 0029 0872 2800 0000  .).Nr....).r(...
+00000f20: 723b 0000 0072 0b00 0000 720c 0000 0072  r;...r....r....r
+00000f30: 1500 0000 720e 0000 0072 1600 0000 7210  ....r....r....r.
+00000f40: 0000 0072 3c00 0000 721d 0000 0072 1d00  ...r<...r....r..
+00000f50: 0000 721e 0000 0072 1700 0000 9000 0000  ..r....r........
+00000f60: 730c 0000 0000 0b0c 0106 0106 0104 010c  s...............
+00000f70: fc7a 1656 6965 7753 6572 7669 6365 2e43  .z.ViewService.C
+00000f80: 7265 6174 6556 6965 7763 0a00 0000 0000  reateViewc......
+00000f90: 0000 0000 0000 0a00 0000 0f00 0000 4300  ..............C.
+00000fa0: 0000 732c 0000 0074 006a 01a0 027c 007c  ..s,...t.j...|.|
+00000fb0: 0164 0174 036a 046a 0574 036a 066a 077c  .d.t.j.j.t.j.j.|
+00000fc0: 027c 037c 057c 047c 067c 077c 087c 09a1  .|.|.|.|.|.|.|..
+00000fd0: 0d53 0029 024e 720a 0000 0029 0872 2800  .S.).Nr....).r(.
+00000fe0: 0000 723b 0000 0072 0b00 0000 720c 0000  ..r;...r....r...
+00000ff0: 0072 1800 0000 720e 0000 0072 1900 0000  .r....r....r....
+00001000: 7210 0000 0072 3c00 0000 721d 0000 0072  r....r<...r....r
+00001010: 1d00 0000 721e 0000 0072 1a00 0000 a100  ....r....r......
+00001020: 0000 730c 0000 0000 0b0c 0106 0106 0104  ..s.............
+00001030: 010c fc7a 1656 6965 7753 6572 7669 6365  ...z.ViewService
+00001040: 2e44 656c 6574 6556 6965 7729 0872 1d00  .DeleteView).r..
+00001050: 0000 4e4e 464e 4e4e 4e29 0872 1d00 0000  ..NNFNNNN).r....
+00001060: 4e4e 464e 4e4e 4e29 0872 1d00 0000 4e4e  NNFNNNN).r....NN
+00001070: 464e 4e4e 4e29 0872 1d00 0000 4e4e 464e  FNNNN).r....NNFN
+00001080: 4e4e 4e29 0972 2000 0000 7221 0000 0072  NNN).r ...r!...r
+00001090: 2200 0000 7223 0000 00da 0c73 7461 7469  "...r#.....stati
+000010a0: 636d 6574 686f 6472 1100 0000 7214 0000  cmethodr....r...
+000010b0: 0072 1700 0000 721a 0000 0072 1d00 0000  .r....r....r....
+000010c0: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+000010d0: 3a00 0000 6a00 0000 7352 0000 0008 0104  :...j...sR......
+000010e0: 0302 0300 0100 0100 0100 0100 0100 0100  ................
+000010f0: 0100 f70c 1002 0300 0100 0100 0100 0100  ................
+00001100: 0100 0100 0100 f70c 1002 0300 0100 0100  ................
+00001110: 0100 0100 0100 0100 0100 f70c 1002 0300  ................
+00001120: 0100 0100 0100 0100 0100 0100 0100 f772  ...............r
+00001130: 3a00 0000 290a 7223 0000 0072 2800 0000  :...).r#...r(...
+00001140: da17 6b61 736b 6164 612e 6b61 736b 6164  ..kaskada.kaskad
+00001150: 612e 7631 616c 7068 6172 0200 0000 720c  a.v1alphar....r.
+00001160: 0000 00da 066f 626a 6563 7472 0300 0000  .....objectr....
+00001170: 7224 0000 0072 3900 0000 723a 0000 0072  r$...r9...r:...r
+00001180: 1d00 0000 721d 0000 0072 1d00 0000 721e  ....r....r....r.
+00001190: 0000 00da 083c 6d6f 6475 6c65 3e02 0000  .....<module>...
+000011a0: 0073 0c00 0000 0401 0802 0c03 1020 1025  .s........... .%
+000011b0: 081d                                     ..
```

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/common_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/common_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/compute_service_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/compute_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/destinations_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/destinations_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/file_service_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/file_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/options_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/options_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/plan_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/plan_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/pulsar_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/pulsar_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/query_service_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/schema_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/sources_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/sources_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/spec_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/table_service_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/table_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/test_cases_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/test_cases_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/view_service_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/view_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py` & `kaskada-0.1.5/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v2alpha/query_service_pb2.py` & `kaskada-0.1.5/src/kaskada/kaskada/v2alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py` & `kaskada-0.1.5/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/materialization.py` & `kaskada-0.1.5/src/kaskada/materialization.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/query.py` & `kaskada-0.1.5/src/kaskada/query.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/slice_filters.py` & `kaskada-0.1.5/src/kaskada/slice_filters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/table.py` & `kaskada-0.1.5/src/kaskada/table.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/src/kaskada/utils.py` & `kaskada-0.1.5/src/kaskada/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,17 +111,19 @@
     return f"file://{path}"
 
 
 def unpack_details(grpc_detail):
     """Unpack a grpc status detail field (which is a 'google.protobuf.Any' type).
     `Unpack()` checks the descriptor of the passed-in message object against the stored one
     and returns False if they don't match and does not attempt any unpacking; True otherwise.
-        Source:
-            https://github.com/protocolbuffers/protobuf/blob/master/python/google/protobuf/internal/well_known_types.py#L81
-            https://github.com/protocolbuffers/protobuf/blob/master/python/google/protobuf/internal/python_message.py#L1135
+
+    Sources
+
+    * `well_known_types.py  <https://github.com/protocolbuffers/protobuf/blob/master/python/google/protobuf/internal/well_known_types.py#L81>`_
+    * `python_message.py <https://github.com/protocolbuffers/protobuf/blob/master/python/google/protobuf/internal/python_message.py#L1135>`_
 
         Raises:
             google.protobuf.message.DecodeError: If it can't deserialize the message object
 
     `Is()` checks if the `Any` message represents the given protocol buffer type.
     """
     if grpc_detail.Is(error_details_pb2.BadRequest.DESCRIPTOR):
```

### Comparing `kaskada-0.1.4/src/kaskada/view.py` & `kaskada-0.1.5/src/kaskada/view.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/vendor/validate/validate.proto` & `kaskada-0.1.5/vendor/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/vendor/validate/validate_pb2.py` & `kaskada-0.1.5/vendor/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/vendor/validate/validate_pb2.pyi` & `kaskada-0.1.5/vendor/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.4/PKG-INFO` & `kaskada-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaskada
-Version: 0.1.4
+Version: 0.1.5
 Summary: A client library for the Kaskada time travel machine learning service
 License: Apache-2.0
 Author: Kaskada
 Author-email: maintainers@kaskada.io
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -50,14 +50,24 @@
 
 #### Check Static Type Task
 To perform static type analysis (mypy): `$ poetry run poe types`
 
 #### Lint Task
 To run the linter (pylint): `$ poetry run poe lint`
 
+#### Generate documentation 
+We use Sphinx and rely on autogeneration extensions within Sphinx to read docstrings and 
+generate an HTML formatted version of the codes documentation. 
+
+* `poetry run poe docs` : generates and builds the docs 
+* `poetry run poe docs-generate` : generates the docs (.rst files)
+* `poetry run poe docs-build` : builds the HTML rendered version of the generated docs (from .rst to .html)
+
+The generated HTML is located inside `docs/build`. Load `docs/build/index.html` in your browser to see the HTML rendered output. 
+
 ## Using the Client from Jupyter
 
 #### Install Jupyter
 To install Jupyter: `$ pip install notebook`
 
 #### Build the Client
 To build the client: `$ poetry build`
```

