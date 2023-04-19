# Comparing `tmp/ord-schema-0.3.46.tar.gz` & `tmp/ord-schema-0.3.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord-schema-0.3.46.tar", last modified: Wed Apr 19 23:15:19 2023, max compression
+gzip compressed data, was "ord-schema-0.3.47.tar", last modified: Wed Apr 19 23:24:39 2023, max compression
```

## Comparing `ord-schema-0.3.46.tar` & `ord-schema-0.3.47.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:19.397425 ord-schema-0.3.46/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-19 23:14:57.000000 ord-schema-0.3.46/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 23:14:57.000000 ord-schema-0.3.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 23:15:19.397425 ord-schema-0.3.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-19 23:14:57.000000 ord-schema-0.3.46/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:19.389425 ord-schema-0.3.46/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:19.389425 ord-schema-0.3.46/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (123)    35625 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:19.393425 ord-schema-0.3.46/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/orm/add_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/orm/add_datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:19.393425 ord-schema-0.3.46/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    76886 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:19.397425 ord-schema-0.3.46/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45244 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-19 23:14:57.000000 ord-schema-0.3.46/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:15:19.389425 ord-schema-0.3.46/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 23:15:19.000000 ord-schema-0.3.46/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-19 23:15:19.000000 ord-schema-0.3.46/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:15:19.000000 ord-schema-0.3.46/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-19 23:15:19.000000 ord-schema-0.3.46/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 23:15:19.000000 ord-schema-0.3.46/ord_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-19 23:14:57.000000 ord-schema-0.3.46/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:15:19.397425 ord-schema-0.3.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-19 23:15:00.000000 ord-schema-0.3.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.420493 ord-schema-0.3.47/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-19 23:24:19.000000 ord-schema-0.3.47/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 23:24:19.000000 ord-schema-0.3.47/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 23:24:39.420493 ord-schema-0.3.47/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-19 23:24:19.000000 ord-schema-0.3.47/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.408493 ord-schema-0.3.47/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.412493 ord-schema-0.3.47/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35625 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.416493 ord-schema-0.3.47/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/add_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/add_datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13438 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.416493 ord-schema-0.3.47/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76886 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.420493 ord-schema-0.3.47/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45244 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.408493 ord-schema-0.3.47/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 23:24:39.000000 ord-schema-0.3.47/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-19 23:24:39.000000 ord-schema-0.3.47/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:24:39.000000 ord-schema-0.3.47/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-19 23:24:39.000000 ord-schema-0.3.47/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 23:24:39.000000 ord-schema-0.3.47/ord_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-19 23:24:19.000000 ord-schema-0.3.47/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:24:39.420493 ord-schema-0.3.47/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-19 23:24:21.000000 ord-schema-0.3.47/setup.py
```

### Comparing `ord-schema-0.3.46/LICENSE` & `ord-schema-0.3.47/LICENSE`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/PKG-INFO` & `ord-schema-0.3.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.46
+Version: 0.3.47
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.46/README.md` & `ord-schema-0.3.47/README.md`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/__init__.py` & `ord-schema-0.3.47/ord_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/frozen_message.py` & `ord-schema-0.3.47/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/frozen_message_test.py` & `ord-schema-0.3.47/ord_schema/frozen_message_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/logging.py` & `ord-schema-0.3.47/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/macros/__init__.py` & `ord-schema-0.3.47/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/macros/solutions.py` & `ord-schema-0.3.47/ord_schema/macros/solutions.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/macros/solutions_test.py` & `ord-schema-0.3.47/ord_schema/macros/solutions_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/macros/workups.py` & `ord-schema-0.3.47/ord_schema/macros/workups.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/message_helpers.py` & `ord-schema-0.3.47/ord_schema/message_helpers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/message_helpers_test.py` & `ord-schema-0.3.47/ord_schema/message_helpers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/orm/__init__.py` & `ord-schema-0.3.47/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/orm/add_datasets.py` & `ord-schema-0.3.47/ord_schema/orm/add_datasets.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/orm/add_datasets_test.py` & `ord-schema-0.3.47/ord_schema/orm/add_datasets_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/orm/conftest.py` & `ord-schema-0.3.47/ord_schema/orm/conftest.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/orm/database.py` & `ord-schema-0.3.47/ord_schema/orm/database.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/orm/database_test.py` & `ord-schema-0.3.47/ord_schema/orm/database_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/orm/mappers.py` & `ord-schema-0.3.47/ord_schema/orm/mappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,23 +124,22 @@
     Args:
         message_type: Protocol buffer message type.
         parents: Dict mapping message types to lists of (parent message type, field name, unique) tuples.
 
     Returns:
         Generated mapper class.
     """
-    table_name = underscore(message_type.DESCRIPTOR.name)
     attrs = {
-        "__tablename__": table_name,
+        "__tablename__": underscore(message_type.DESCRIPTOR.name),
         "id": Column(Integer, primary_key=True),
-        "_polymorphic_type": Column(Text, nullable=False),
+        "ord_schema_context": Column(Text, nullable=False),
     }
     attrs["__mapper_args__"] = {
-        "polymorphic_on": attrs["_polymorphic_type"],
-        "polymorphic_identity": table_name,
+        "polymorphic_on": attrs["ord_schema_context"],
+        "polymorphic_identity": message_type.DESCRIPTOR.name,
         "with_polymorphic": "*",
     }
     add_key = False
     for parent_type, field_name, _ in parents[message_type]:
         if isinstance(getattr(parent_type(), field_name), Mapping):
             add_key = True
     if add_key:
@@ -180,18 +179,16 @@
         attrs["reaction_id"] = Column(Text, ForeignKey("reaction.reaction_id", ondelete="CASCADE"), **kwargs)
     logger.debug(f"Creating mapper {message_type.DESCRIPTOR.name}: {attrs}")
     mapper_class = type(message_type.DESCRIPTOR.name, (Base,), attrs)
     # Create polymorphic child classes.
     for parent_type, field_name, _ in parents[message_type]:
         foreign_table_name = underscore(parent_type.DESCRIPTOR.name)
         foreign_key = f"{foreign_table_name}.id"
-        if foreign_table_name in ["structure"]:
-            foreign_key = f"rdkit.{foreign_key}"
         child_attrs = {
-            "__mapper_args__": {"polymorphic_identity": f"{foreign_table_name}__{field_name}"},
+            "__mapper_args__": {"polymorphic_identity": f"{parent_type.DESCRIPTOR.name}.{field_name}"},
             # Use get() to avoid column conflicts; see
             # https://docs.sqlalchemy.org/en/14/orm/inheritance.html#resolving-column-conflicts.
             #
             # NOTE(skearnes): We are not enforcing unique constraints on this column; see the module docstring.
             f"{foreign_table_name}_id": mapper_class.__table__.c.get(
                 f"{foreign_table_name}_id",
                 Column(Integer, ForeignKey(foreign_key, ondelete="CASCADE")),
```

### Comparing `ord-schema-0.3.46/ord_schema/orm/mappers_test.py` & `ord-schema-0.3.47/ord_schema/orm/mappers_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for ord_schema.orm."""
+"""Tests for ord_schema.orm.mappers."""
 import os
 import pytest
 
 from ord_schema.message_helpers import load_message
 from ord_schema.orm.mappers import from_proto, to_proto
 from ord_schema.proto.dataset_pb2 import Dataset
```

### Comparing `ord-schema-0.3.46/ord_schema/orm/rdkit_mappers.py` & `ord-schema-0.3.47/ord_schema/orm/rdkit_mappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""RDKit PostgreSQL cartridge functionality."""
+"""RDKit PostgreSQL cartridge functionality.
+
+Notes:
+  * These tables live in a separate "rdkit" schema to avoid name conflicts between tables and extension types.
+  * The RDKit-specific columns are populated by ord_schema.orm.database.add_rdkit; this allows the ORM to function
+    normally even if if the RDKit PostgreSQL cartridge is not installed (the `smiles` column will be populated and
+    the other columns will be empty).
+  * Objects with this type are added to the ORM in from_proto() using the `rdkit` field.
+"""
 from __future__ import annotations
 
 import os
 from distutils.util import strtobool  # pylint: disable=deprecated-module
 from enum import Enum
 
 from sqlalchemy import Column, Index, Integer, ForeignKey, Text, func
@@ -145,60 +153,52 @@
             else:
                 raise ValueError(f"unable to determine dtype for {name}")
             table_args.extend([Column(name, dtype), Index(f"{name}_index", name, postgresql_using="gist")])
         return table_args
 
 
 class RDKitMol(Base):
-    """Table for storing compound structures and associated RDKit cartridge data.
-
-    Notes:
-      * This table lives in a separate "rdkit" schema to avoid name conflicts between tables and extension types.
-      * The RDKit-specific columns are populated by ord_schema.orm.database.add_rdkit; this allows the ORM to function
-        normally even if if the RDKit PostgreSQL cartridge is not installed (the `smiles` column will be populated and
-        the other columns will be empty).
-      * Objects with this type are added to the ORM in from_proto() using the `structure` field.
-    """
+    """Table for storing compound structures and associated RDKit cartridge data."""
 
     __tablename__ = "mols"
     id = Column(Integer, primary_key=True)
     smiles = Column(Text)
     mol = Column(_RDKitMol)
 
     __table_args__ = (
         Index("mol_index", "mol", postgresql_using="gist"),
         *FingerprintType.get_table_args(),
         {"schema": "rdkit"},
     )
 
-    _polymorphic_type = Column(Text, nullable=False)
+    ord_schema_context = Column(Text, nullable=False)
     __mapper_args__ = {
-        "polymorphic_on": _polymorphic_type,
+        "polymorphic_on": ord_schema_context,
         "polymorphic_identity": "mols",
         "with_polymorphic": "*",
     }
 
     @classmethod
     def tanimoto(cls, other: str, fp_type: FingerprintType = FingerprintType.MORGAN_BFP):
         return func.rdkit.tanimoto_sml(getattr(cls, fp_type.name.lower()), fp_type(other))
 
 
 class _CompoundRDKit(RDKitMol):
     compound_id = Column(Integer, ForeignKey("compound.id", ondelete="CASCADE"))
 
     __mapper_args__ = {
-        "polymorphic_identity": "compound__rdkit",
+        "polymorphic_identity": "Compound.rdkit",
     }
 
 
 class _ProductCompoundRDKit(RDKitMol):
     product_compound_id = Column(Integer, ForeignKey("product_compound.id", ondelete="CASCADE"))
 
     __mapper_args__ = {
-        "polymorphic_identity": "product_compound__rdkit",
+        "polymorphic_identity": "ProductCompound.rdkit",
     }
 
 
 class RDKitReaction(Base):
     """Table for storing reaction objects and associated RDKit cartridge data."""
 
     __tablename__ = "reactions"
@@ -207,21 +207,21 @@
     reaction = Column(_RDKitReaction)
 
     __table_args__ = (
         Index("reaction_index", "reaction", postgresql_using="gist"),
         {"schema": "rdkit"},
     )
 
-    _polymorphic_type = Column(Text, nullable=False)
+    ord_schema_context = Column(Text, nullable=False)
     __mapper_args__ = {
-        "polymorphic_on": _polymorphic_type,
+        "polymorphic_on": ord_schema_context,
         "polymorphic_identity": "reactions",
         "with_polymorphic": "*",
     }
 
 
 class _ReactionRDKit(RDKitReaction):
     reaction_id = Column(Integer, ForeignKey("reaction.id", ondelete="CASCADE"))
 
     __mapper_args__ = {
-        "polymorphic_identity": "reaction__rdkit",
+        "polymorphic_identity": "Reaction.rdkit",
     }
```

### Comparing `ord-schema-0.3.46/ord_schema/orm/rdkit_mappers_test.py` & `ord-schema-0.3.47/ord_schema/orm/rdkit_mappers_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for ord_schema.orm.structure."""
+"""Tests for ord_schema.orm.rdkit_mappers."""
 import pytest
 from sqlalchemy import select
 from ord_schema.orm.mappers import Mappers
 from ord_schema.orm.rdkit_mappers import FingerprintType, RDKitMol
 
 
 def test_tanimoto_operator(test_session):
```

### Comparing `ord-schema-0.3.46/ord_schema/proto/__init__.py` & `ord-schema-0.3.47/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/proto/dataset_pb2.py` & `ord-schema-0.3.47/ord_schema/proto/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/proto/dataset_pb2_test.py` & `ord-schema-0.3.47/ord_schema/proto/dataset_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/proto/reaction_pb2.py` & `ord-schema-0.3.47/ord_schema/proto/reaction_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/proto/reaction_pb2_test.py` & `ord-schema-0.3.47/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/proto/test_pb2.py` & `ord-schema-0.3.47/ord_schema/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/resolvers.py` & `ord-schema-0.3.47/ord_schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/resolvers_test.py` & `ord-schema-0.3.47/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/scripts/__init__.py` & `ord-schema-0.3.47/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/scripts/build_dataset.py` & `ord-schema-0.3.47/ord_schema/scripts/build_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/scripts/build_dataset_test.py` & `ord-schema-0.3.47/ord_schema/scripts/build_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/scripts/check_pb.py` & `ord-schema-0.3.47/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/scripts/check_pb_test.py` & `ord-schema-0.3.47/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/scripts/enumerate_dataset.py` & `ord-schema-0.3.47/ord_schema/scripts/enumerate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/scripts/enumerate_dataset_test.py` & `ord-schema-0.3.47/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/scripts/parse_uspto.py` & `ord-schema-0.3.47/ord_schema/scripts/parse_uspto.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/scripts/process_dataset.py` & `ord-schema-0.3.47/ord_schema/scripts/process_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/scripts/process_dataset_test.py` & `ord-schema-0.3.47/ord_schema/scripts/process_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/scripts/validate_dataset.py` & `ord-schema-0.3.47/ord_schema/scripts/validate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/scripts/validate_dataset_test.py` & `ord-schema-0.3.47/ord_schema/scripts/validate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/templating.py` & `ord-schema-0.3.47/ord_schema/templating.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/templating_test.py` & `ord-schema-0.3.47/ord_schema/templating_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/units.py` & `ord-schema-0.3.47/ord_schema/units.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/units_test.py` & `ord-schema-0.3.47/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/updates.py` & `ord-schema-0.3.47/ord_schema/updates.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/updates_test.py` & `ord-schema-0.3.47/ord_schema/updates_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/validations.py` & `ord-schema-0.3.47/ord_schema/validations.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema/validations_test.py` & `ord-schema-0.3.47/ord_schema/validations_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema.egg-info/PKG-INFO` & `ord-schema-0.3.47/ord_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.46
+Version: 0.3.47
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.46/ord_schema.egg-info/SOURCES.txt` & `ord-schema-0.3.47/ord_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/ord_schema.egg-info/requires.txt` & `ord-schema-0.3.47/ord_schema.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.46/setup.py` & `ord-schema-0.3.47/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.46",
+    version="0.3.47",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

