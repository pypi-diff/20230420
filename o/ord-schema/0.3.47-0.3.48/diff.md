# Comparing `tmp/ord-schema-0.3.47.tar.gz` & `tmp/ord-schema-0.3.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord-schema-0.3.47.tar", last modified: Wed Apr 19 23:24:39 2023, max compression
+gzip compressed data, was "ord-schema-0.3.48.tar", last modified: Thu Apr 20 08:27:56 2023, max compression
```

## Comparing `ord-schema-0.3.47.tar` & `ord-schema-0.3.48.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.420493 ord-schema-0.3.47/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-19 23:24:19.000000 ord-schema-0.3.47/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 23:24:19.000000 ord-schema-0.3.47/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 23:24:39.420493 ord-schema-0.3.47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-19 23:24:19.000000 ord-schema-0.3.47/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.408493 ord-schema-0.3.47/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.412493 ord-schema-0.3.47/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (123)    35625 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.416493 ord-schema-0.3.47/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/add_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/add_datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13438 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.416493 ord-schema-0.3.47/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    76886 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.420493 ord-schema-0.3.47/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45244 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-19 23:24:19.000000 ord-schema-0.3.47/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:24:39.408493 ord-schema-0.3.47/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 23:24:39.000000 ord-schema-0.3.47/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-19 23:24:39.000000 ord-schema-0.3.47/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:24:39.000000 ord-schema-0.3.47/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-19 23:24:39.000000 ord-schema-0.3.47/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 23:24:39.000000 ord-schema-0.3.47/ord_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-19 23:24:19.000000 ord-schema-0.3.47/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:24:39.420493 ord-schema-0.3.47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-19 23:24:21.000000 ord-schema-0.3.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.341699 ord-schema-0.3.48/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-20 08:27:33.000000 ord-schema-0.3.48/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 08:27:33.000000 ord-schema-0.3.48/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-20 08:27:56.341699 ord-schema-0.3.48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-20 08:27:33.000000 ord-schema-0.3.48/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.333698 ord-schema-0.3.48/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.333698 ord-schema-0.3.48/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35625 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.337698 ord-schema-0.3.48/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/add_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/add_datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.337698 ord-schema-0.3.48/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77919 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.341699 ord-schema-0.3.48/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45244 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.333698 ord-schema-0.3.48/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-20 08:27:56.000000 ord-schema-0.3.48/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-20 08:27:56.000000 ord-schema-0.3.48/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:27:56.000000 ord-schema-0.3.48/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-20 08:27:56.000000 ord-schema-0.3.48/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 08:27:56.000000 ord-schema-0.3.48/ord_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-20 08:27:34.000000 ord-schema-0.3.48/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 08:27:56.341699 ord-schema-0.3.48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-20 08:27:37.000000 ord-schema-0.3.48/setup.py
```

### Comparing `ord-schema-0.3.47/LICENSE` & `ord-schema-0.3.48/LICENSE`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/PKG-INFO` & `ord-schema-0.3.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.47
+Version: 0.3.48
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.47/README.md` & `ord-schema-0.3.48/README.md`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/__init__.py` & `ord-schema-0.3.48/ord_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/frozen_message.py` & `ord-schema-0.3.48/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/frozen_message_test.py` & `ord-schema-0.3.48/ord_schema/frozen_message_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/logging.py` & `ord-schema-0.3.48/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/macros/__init__.py` & `ord-schema-0.3.48/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/macros/solutions.py` & `ord-schema-0.3.48/ord_schema/macros/solutions.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/macros/solutions_test.py` & `ord-schema-0.3.48/ord_schema/macros/solutions_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/macros/workups.py` & `ord-schema-0.3.48/ord_schema/macros/workups.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/message_helpers.py` & `ord-schema-0.3.48/ord_schema/message_helpers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/message_helpers_test.py` & `ord-schema-0.3.48/ord_schema/message_helpers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/orm/__init__.py` & `ord-schema-0.3.48/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/orm/add_datasets.py` & `ord-schema-0.3.48/ord_schema/orm/add_datasets.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/orm/add_datasets_test.py` & `ord-schema-0.3.48/ord_schema/orm/add_datasets_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/orm/conftest.py` & `ord-schema-0.3.48/ord_schema/orm/conftest.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/orm/database.py` & `ord-schema-0.3.48/ord_schema/orm/database.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/orm/database_test.py` & `ord-schema-0.3.48/ord_schema/orm/database_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/orm/mappers.py` & `ord-schema-0.3.48/ord_schema/orm/mappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,19 +70,22 @@
     return parents
 
 
 def _get_message_contexts(
     descriptor: Descriptor, parent: str | None, field_name: str | None, unique: bool | None
 ) -> set[tuple[str, str | None, str | None, bool | None]]:
     """Returns the set of contexts for each message type."""
+    if descriptor is None:
+        raise ValueError((descriptor, parent, field_name, unique))
     counts = {(descriptor.full_name, parent, field_name, unique)}
     for field in descriptor.fields:
         if field.type == FieldDescriptor.TYPE_MESSAGE:
             if set(field.message_type.fields_by_name.keys()) == {"key", "value"}:
                 # Check for maps.
+                logger.info(f"Found map: ({descriptor.full_name}, {field.name})")
                 field_message_type = field.message_type.fields_by_name["value"].message_type
             else:
                 field_message_type = field.message_type
             counts |= _get_message_contexts(
                 field_message_type,
                 parent=descriptor.full_name,
                 field_name=field.name,
```

### Comparing `ord-schema-0.3.47/ord_schema/orm/mappers_test.py` & `ord-schema-0.3.48/ord_schema/orm/mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/orm/rdkit_mappers.py` & `ord-schema-0.3.48/ord_schema/orm/rdkit_mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/orm/rdkit_mappers_test.py` & `ord-schema-0.3.48/ord_schema/orm/rdkit_mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/proto/__init__.py` & `ord-schema-0.3.48/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/proto/dataset_pb2.py` & `ord-schema-0.3.48/ord_schema/proto/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/proto/dataset_pb2_test.py` & `ord-schema-0.3.48/ord_schema/proto/dataset_pb2_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,19 @@
     dataset.name = "test"
     dataset.description = "test dataset"
     # Add a reaction directly to the dataset.
     reaction1 = dataset.reactions.add()
     reaction1.identifiers.add(value="C(C)Cl.Br>>C(C)Br.Cl", type="REACTION_SMILES")
     # Copy a reaction created elsewhere.
     reaction2 = reaction_pb2.Reaction()
-    reaction2.identifiers.add(value="amide coupling", type="NAME")
+    reaction2.identifiers.add(value="amide coupling", type="REACTION_TYPE")
     dataset.reactions.add().CopyFrom(reaction2)
     yield dataset.SerializeToString()
 
 
 def test_dataset(serialized_dataset):
     dataset = dataset_pb2.Dataset.FromString(serialized_dataset)
     assert dataset.name == "test"
     assert dataset.description == "test dataset"
     assert len(dataset.reactions) == 2
     assert dataset.reactions[0].identifiers[0].type == reaction_pb2.ReactionIdentifier.REACTION_SMILES
-    assert dataset.reactions[1].identifiers[0].type == reaction_pb2.ReactionIdentifier.NAME
+    assert dataset.reactions[1].identifiers[0].type == reaction_pb2.ReactionIdentifier.REACTION_TYPE
```

### Comparing `ord-schema-0.3.47/ord_schema/proto/reaction_pb2.py` & `ord-schema-0.3.48/ord_schema/proto/reaction_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ford-schema/proto/reaction.proto\x12\x03ord\"\xd9\x03\n\x08Reaction\x12,\n\x0bidentifiers\x18\x01 \x03(\x0b\x32\x17.ord.ReactionIdentifier\x12)\n\x06inputs\x18\x02 \x03(\x0b\x32\x19.ord.Reaction.InputsEntry\x12!\n\x05setup\x18\x03 \x01(\x0b\x32\x12.ord.ReactionSetup\x12+\n\nconditions\x18\x04 \x01(\x0b\x32\x17.ord.ReactionConditions\x12!\n\x05notes\x18\x05 \x01(\x0b\x32\x12.ord.ReactionNotes\x12.\n\x0cobservations\x18\x06 \x03(\x0b\x32\x18.ord.ReactionObservation\x12$\n\x07workups\x18\x07 \x03(\x0b\x32\x13.ord.ReactionWorkup\x12&\n\x08outcomes\x18\x08 \x03(\x0b\x32\x14.ord.ReactionOutcome\x12+\n\nprovenance\x18\t \x01(\x0b\x32\x17.ord.ReactionProvenance\x12\x13\n\x0breaction_id\x18\n \x01(\t\x1a\x41\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.ord.ReactionInput:\x02\x38\x01\"\x9e\x02\n\x12ReactionIdentifier\x12<\n\x04type\x18\x01 \x01(\x0e\x32..ord.ReactionIdentifier.ReactionIdentifierType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x16\n\tis_mapped\x18\x04 \x01(\x08H\x00\x88\x01\x01\"\x83\x01\n\x16ReactionIdentifierType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x13\n\x0fREACTION_SMILES\x10\x02\x12\x15\n\x11REACTION_CXSMILES\x10\x06\x12\n\n\x06RDFILE\x10\x03\x12\n\n\x06RINCHI\x10\x04\x12\x08\n\x04NAME\x10\x05\x42\x0c\n\n_is_mapped\"\xbc\x06\n\rReactionInput\x12!\n\ncomponents\x18\x01 \x03(\x0b\x32\r.ord.Compound\x12-\n\x10\x63rude_components\x18\x02 \x03(\x0b\x32\x13.ord.CrudeComponent\x12\x16\n\x0e\x61\x64\x64ition_order\x18\x03 \x01(\x05\x12 \n\raddition_time\x18\x04 \x01(\x0b\x32\t.ord.Time\x12\x38\n\x0e\x61\x64\x64ition_speed\x18\x05 \x01(\x0b\x32 .ord.ReactionInput.AdditionSpeed\x12$\n\x11\x61\x64\x64ition_duration\x18\x06 \x01(\x0b\x32\t.ord.Time\x12 \n\tflow_rate\x18\x07 \x01(\x0b\x32\r.ord.FlowRate\x12:\n\x0f\x61\x64\x64ition_device\x18\x08 \x01(\x0b\x32!.ord.ReactionInput.AdditionDevice\x12.\n\x14\x61\x64\x64ition_temperature\x18\t \x01(\x0b\x32\x10.ord.Temperature\x1a\xdc\x01\n\rAdditionSpeed\x12@\n\x04type\x18\x01 \x01(\x0e\x32\x32.ord.ReactionInput.AdditionSpeed.AdditionSpeedType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"x\n\x11\x41\x64\x64itionSpeedType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0f\n\x0b\x41LL_AT_ONCE\x10\x01\x12\x08\n\x04\x46\x41ST\x10\x02\x12\x08\n\x04SLOW\x10\x03\x12\x0c\n\x08\x44ROPWISE\x10\x04\x12\x0e\n\nCONTINUOUS\x10\x05\x12\x0f\n\x0bPORTIONWISE\x10\x06\x1a\xd1\x01\n\x0e\x41\x64\x64itionDevice\x12\x42\n\x04type\x18\x01 \x01(\x0e\x32\x34.ord.ReactionInput.AdditionDevice.AdditionDeviceType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"j\n\x12\x41\x64\x64itionDeviceType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0b\n\x07SYRINGE\x10\x03\x12\x0b\n\x07\x43\x41NNULA\x10\x04\x12\x13\n\x0f\x41\x44\x44ITION_FUNNEL\x10\x05\"\xd6\x01\n\x06\x41mount\x12\x19\n\x04mass\x18\x01 \x01(\x0b\x32\t.ord.MassH\x00\x12\x1b\n\x05moles\x18\x02 \x01(\x0b\x32\n.ord.MolesH\x00\x12\x1d\n\x06volume\x18\x03 \x01(\x0b\x32\x0b.ord.VolumeH\x00\x12+\n\nunmeasured\x18\x05 \x01(\x0b\x32\x15.ord.UnmeasuredAmountH\x00\x12$\n\x17volume_includes_solutes\x18\x04 \x01(\x08H\x01\x88\x01\x01\x42\x06\n\x04kindB\x1a\n\x18_volume_includes_solutes\"\xbe\x01\n\x10UnmeasuredAmount\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.ord.UnmeasuredAmount.UnmeasuredAmountType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"_\n\x14UnmeasuredAmountType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\r\n\tSATURATED\x10\x02\x12\r\n\tCATALYTIC\x10\x03\x12\x0c\n\x08TITRATED\x10\x04\"\xac\x01\n\x0e\x43rudeComponent\x12\x13\n\x0breaction_id\x18\x01 \x01(\t\x12\x1c\n\x0fincludes_workup\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1f\n\x12has_derived_amount\x18\x03 \x01(\x08H\x01\x88\x01\x01\x12\x1b\n\x06\x61mount\x18\x04 \x01(\x0b\x32\x0b.ord.AmountB\x12\n\x10_includes_workupB\x15\n\x13_has_derived_amount\"\xa5\x04\n\x08\x43ompound\x12,\n\x0bidentifiers\x18\x01 \x03(\x0b\x32\x17.ord.CompoundIdentifier\x12\x1b\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x0b.ord.Amount\x12\x39\n\rreaction_role\x18\x03 \x01(\x0e\x32\".ord.ReactionRole.ReactionRoleType\x12\x18\n\x0bis_limiting\x18\x04 \x01(\x08H\x00\x88\x01\x01\x12.\n\x0cpreparations\x18\x05 \x03(\x0b\x32\x18.ord.CompoundPreparation\x12$\n\x06source\x18\x06 \x01(\x0b\x32\x14.ord.Compound.Source\x12-\n\x08\x66\x65\x61tures\x18\x07 \x03(\x0b\x32\x1b.ord.Compound.FeaturesEntry\x12-\n\x08\x61nalyses\x18\x08 \x03(\x0b\x32\x1b.ord.Compound.AnalysesEntry\x1a\x39\n\x06Source\x12\x0e\n\x06vendor\x18\x01 \x01(\t\x12\x12\n\ncatalog_id\x18\x02 \x01(\t\x12\x0b\n\x03lot\x18\x03 \x01(\t\x1a:\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x1a>\n\rAnalysesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.ord.Analysis:\x02\x38\x01\x42\x0e\n\x0c_is_limiting\"\xb2\x01\n\x0cReactionRole\"\xa1\x01\n\x10ReactionRoleType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0c\n\x08REACTANT\x10\x01\x12\x0b\n\x07REAGENT\x10\x02\x12\x0b\n\x07SOLVENT\x10\x03\x12\x0c\n\x08\x43\x41TALYST\x10\x04\x12\n\n\x06WORKUP\x10\x05\x12\x15\n\x11INTERNAL_STANDARD\x10\x06\x12\x16\n\x12\x41UTHENTIC_STANDARD\x10\x07\x12\x0b\n\x07PRODUCT\x10\x08\"\xf6\x01\n\x13\x43ompoundPreparation\x12>\n\x04type\x18\x01 \x01(\x0e\x32\x30.ord.CompoundPreparation.CompoundPreparationType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x13\n\x0breaction_id\x18\x03 \x01(\t\"y\n\x17\x43ompoundPreparationType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0e\n\nREPURIFIED\x10\x03\x12\x0b\n\x07SPARGED\x10\x04\x12\t\n\x05\x44RIED\x10\x05\x12\x0f\n\x0bSYNTHESIZED\x10\x06\"\x82\x03\n\x12\x43ompoundIdentifier\x12<\n\x04type\x18\x01 \x01(\x0e\x32..ord.CompoundIdentifier.CompoundIdentifierType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\x8d\x02\n\x16\x43ompoundIdentifierType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\n\n\x06SMILES\x10\x02\x12\t\n\x05INCHI\x10\x03\x12\x0c\n\x08MOLBLOCK\x10\x04\x12\x0e\n\nIUPAC_NAME\x10\x05\x12\x08\n\x04NAME\x10\x06\x12\x0e\n\nCAS_NUMBER\x10\x07\x12\x0f\n\x0bPUBCHEM_CID\x10\x08\x12\x11\n\rCHEMSPIDER_ID\x10\t\x12\x0c\n\x08\x43XSMILES\x10\n\x12\r\n\tINCHI_KEY\x10\x0b\x12\x07\n\x03XYZ\x10\x0c\x12\x0e\n\nUNIPROT_ID\x10\r\x12\n\n\x06PDB_ID\x10\x0e\x12\x17\n\x13\x41MINO_ACID_SEQUENCE\x10\x0f\x12\x08\n\x04HELM\x10\x10\"\x92\x04\n\x06Vessel\x12$\n\x04type\x18\x01 \x01(\x0e\x32\x16.ord.Vessel.VesselType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12%\n\x08material\x18\x03 \x01(\x0b\x32\x13.ord.VesselMaterial\x12,\n\x0cpreparations\x18\x04 \x03(\x0b\x32\x16.ord.VesselPreparation\x12*\n\x0b\x61ttachments\x18\x05 \x03(\x0b\x32\x15.ord.VesselAttachment\x12\x1b\n\x06volume\x18\x06 \x01(\x0b\x32\x0b.ord.Volume\x12\x10\n\x08plate_id\x18\x07 \x01(\t\x12\x16\n\x0eplate_position\x18\x08 \x01(\t\"\x88\x02\n\nVesselType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x16\n\x12ROUND_BOTTOM_FLASK\x10\x02\x12\x08\n\x04VIAL\x10\x03\x12\x0e\n\nWELL_PLATE\x10\x04\x12\x12\n\x0eMICROWAVE_VIAL\x10\x05\x12\x08\n\x04TUBE\x10\x06\x12#\n\x1f\x43ONTINUOUS_STIRRED_TANK_REACTOR\x10\x07\x12\x16\n\x12PACKED_BED_REACTOR\x10\x08\x12\x0c\n\x08NMR_TUBE\x10\t\x12\x12\n\x0ePRESSURE_FLASK\x10\n\x12\x14\n\x10PRESSURE_REACTOR\x10\x0b\x12\x18\n\x14\x45LECTROCHEMICAL_CELL\x10\x0c\"\xcc\x01\n\x0eVesselMaterial\x12\x34\n\x04type\x18\x01 \x01(\x0e\x32&.ord.VesselMaterial.VesselMaterialType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"s\n\x12VesselMaterialType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\t\n\x05GLASS\x10\x02\x12\x11\n\rPOLYPROPYLENE\x10\x03\x12\x0b\n\x07PLASTIC\x10\x04\x12\t\n\x05METAL\x10\x05\x12\n\n\x06QUARTZ\x10\x06\"\x97\x03\n\x10VesselAttachment\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.ord.VesselAttachment.VesselAttachmentType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\xb7\x02\n\x14VesselAttachmentType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\n\n\x06SEPTUM\x10\x03\x12\x07\n\x03\x43\x41P\x10\x04\x12\x07\n\x03MAT\x10\x05\x12\x14\n\x10REFLUX_CONDENSER\x10\x06\x12\x0f\n\x0bVENT_NEEDLE\x10\x07\x12\x0e\n\nDEAN_STARK\x10\x08\x12\x0f\n\x0bVACUUM_TUBE\x10\t\x12\x13\n\x0f\x41\x44\x44ITION_FUNNEL\x10\n\x12\x0f\n\x0b\x44RYING_TUBE\x10\x0b\x12\x11\n\rALUMINUM_FOIL\x10\x0c\x12\x10\n\x0cTHERMOCOUPLE\x10\r\x12\x0b\n\x07\x42\x41LLOON\x10\x0e\x12\x0f\n\x0bGAS_ADAPTER\x10\x0f\x12\x16\n\x12PRESSURE_REGULATOR\x10\x10\x12\x11\n\rRELEASE_VALVE\x10\x11\"\xe8\x01\n\x11VesselPreparation\x12:\n\x04type\x18\x01 \x01(\x0e\x32,.ord.VesselPreparation.VesselPreparationType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\x85\x01\n\x15VesselPreparationType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0e\n\nOVEN_DRIED\x10\x03\x12\x0f\n\x0b\x46LAME_DRIED\x10\x04\x12\x18\n\x14\x45VACUATED_BACKFILLED\x10\x05\x12\n\n\x06PURGED\x10\x06\"\xa0\x04\n\rReactionSetup\x12\x1b\n\x06vessel\x18\x01 \x01(\x0b\x32\x0b.ord.Vessel\x12\x19\n\x0cis_automated\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1b\n\x13\x61utomation_platform\x18\x03 \x01(\t\x12?\n\x0f\x61utomation_code\x18\x04 \x03(\x0b\x32&.ord.ReactionSetup.AutomationCodeEntry\x12;\n\x0b\x65nvironment\x18\x05 \x01(\x0b\x32&.ord.ReactionSetup.ReactionEnvironment\x1a@\n\x13\x41utomationCodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x1a\xe8\x01\n\x13ReactionEnvironment\x12L\n\x04type\x18\x01 \x01(\x0e\x32>.ord.ReactionSetup.ReactionEnvironment.ReactionEnvironmentType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"r\n\x17ReactionEnvironmentType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\r\n\tFUME_HOOD\x10\x02\x12\r\n\tBENCH_TOP\x10\x03\x12\r\n\tGLOVE_BOX\x10\x04\x12\r\n\tGLOVE_BAG\x10\x05\x42\x0f\n\r_is_automated\"\xb5\x03\n\x12ReactionConditions\x12/\n\x0btemperature\x18\x01 \x01(\x0b\x32\x1a.ord.TemperatureConditions\x12)\n\x08pressure\x18\x02 \x01(\x0b\x32\x17.ord.PressureConditions\x12)\n\x08stirring\x18\x03 \x01(\x0b\x32\x17.ord.StirringConditions\x12\x31\n\x0cillumination\x18\x04 \x01(\x0b\x32\x1b.ord.IlluminationConditions\x12\x39\n\x10\x65lectrochemistry\x18\x05 \x01(\x0b\x32\x1f.ord.ElectrochemistryConditions\x12!\n\x04\x66low\x18\x06 \x01(\x0b\x32\x13.ord.FlowConditions\x12\x13\n\x06reflux\x18\x07 \x01(\x08H\x00\x88\x01\x01\x12\x0f\n\x02ph\x18\x08 \x01(\x02H\x01\x88\x01\x01\x12#\n\x16\x63onditions_are_dynamic\x18\t \x01(\x08H\x02\x88\x01\x01\x12\x0f\n\x07\x64\x65tails\x18\n \x01(\tB\t\n\x07_refluxB\x05\n\x03_phB\x19\n\x17_conditions_are_dynamic\"\xe2\x06\n\x15TemperatureConditions\x12>\n\x07\x63ontrol\x18\x01 \x01(\x0b\x32-.ord.TemperatureConditions.TemperatureControl\x12\"\n\x08setpoint\x18\x02 \x01(\x0b\x32\x10.ord.Temperature\x12G\n\x0cmeasurements\x18\x03 \x03(\x0b\x32\x31.ord.TemperatureConditions.TemperatureMeasurement\x1a\xd4\x02\n\x12TemperatureControl\x12R\n\x04type\x18\x01 \x01(\x0e\x32\x44.ord.TemperatureConditions.TemperatureControl.TemperatureControlType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\xd8\x01\n\x16TemperatureControlType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0b\n\x07\x41MBIENT\x10\x02\x12\x0c\n\x08OIL_BATH\x10\x03\x12\x0e\n\nWATER_BATH\x10\x04\x12\r\n\tSAND_BATH\x10\x05\x12\x0c\n\x08ICE_BATH\x10\x06\x12\x16\n\x12\x44RY_ALUMINUM_PLATE\x10\x07\x12\r\n\tMICROWAVE\x10\x08\x12\x10\n\x0c\x44RY_ICE_BATH\x10\t\x12\x0b\n\x07\x41IR_FAN\x10\n\x12\x13\n\x0fLIQUID_NITROGEN\x10\x0b\x1a\xc4\x02\n\x16TemperatureMeasurement\x12Z\n\x04type\x18\x01 \x01(\x0e\x32L.ord.TemperatureConditions.TemperatureMeasurement.TemperatureMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x17\n\x04time\x18\x03 \x01(\x0b\x32\t.ord.Time\x12%\n\x0btemperature\x18\x04 \x01(\x0b\x32\x10.ord.Temperature\"}\n\x1aTemperatureMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x19\n\x15THERMOCOUPLE_INTERNAL\x10\x02\x12\x19\n\x15THERMOCOUPLE_EXTERNAL\x10\x03\x12\x0c\n\x08INFRARED\x10\x04\"\x8c\x08\n\x12PressureConditions\x12\x38\n\x07\x63ontrol\x18\x01 \x01(\x0b\x32\'.ord.PressureConditions.PressureControl\x12\x1f\n\x08setpoint\x18\x02 \x01(\x0b\x32\r.ord.Pressure\x12\x36\n\natmosphere\x18\x03 \x01(\x0b\x32\".ord.PressureConditions.Atmosphere\x12\x41\n\x0cmeasurements\x18\x04 \x03(\x0b\x32+.ord.PressureConditions.PressureMeasurement\x1a\xe0\x01\n\x0fPressureControl\x12I\n\x04type\x18\x01 \x01(\x0e\x32;.ord.PressureConditions.PressureControl.PressureControlType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"q\n\x13PressureControlType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0b\n\x07\x41MBIENT\x10\x02\x12\x13\n\x0fSLIGHT_POSITIVE\x10\x03\x12\n\n\x06SEALED\x10\x04\x12\x0f\n\x0bPRESSURIZED\x10\x05\x1a\xb5\x02\n\nAtmosphere\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.ord.PressureConditions.Atmosphere.AtmosphereType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\xd4\x01\n\x0e\x41tmosphereType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x07\n\x03\x41IR\x10\x02\x12\x0c\n\x08NITROGEN\x10\x03\x12\t\n\x05\x41RGON\x10\x04\x12\n\n\x06OXYGEN\x10\x05\x12\x0c\n\x08HYDROGEN\x10\x06\x12\x13\n\x0f\x43\x41RBON_MONOXIDE\x10\x07\x12\x12\n\x0e\x43\x41RBON_DIOXIDE\x10\x08\x12\x0b\n\x07METHANE\x10\t\x12\x0b\n\x07\x41MMONIA\x10\n\x12\t\n\x05OZONE\x10\x0b\x12\x0c\n\x08\x45THYLENE\x10\x0c\x12\r\n\tACETYLENE\x10\r\x1a\x84\x02\n\x13PressureMeasurement\x12Q\n\x04type\x18\x01 \x01(\x0e\x32\x43.ord.PressureConditions.PressureMeasurement.PressureMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x17\n\x04time\x18\x03 \x01(\x0b\x32\t.ord.Time\x12\x1f\n\x08pressure\x18\x04 \x01(\x0b\x32\r.ord.Pressure\"O\n\x17PressureMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x17\n\x13PRESSURE_TRANSDUCER\x10\x02\"\xdc\x03\n\x12StirringConditions\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.ord.StirringConditions.StirringMethodType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x32\n\x04rate\x18\x03 \x01(\x0b\x32$.ord.StirringConditions.StirringRate\x1a\xb5\x01\n\x0cStirringRate\x12\x43\n\x04type\x18\x01 \x01(\x0e\x32\x35.ord.StirringConditions.StirringRate.StirringRateType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x0b\n\x03rpm\x18\x03 \x01(\x05\"B\n\x10StirringRateType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04HIGH\x10\x01\x12\n\n\x06MEDIUM\x10\x02\x12\x07\n\x03LOW\x10\x03\"\x8e\x01\n\x12StirringMethodType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0c\n\x08STIR_BAR\x10\x03\x12\x12\n\x0eOVERHEAD_MIXER\x10\x04\x12\r\n\tAGITATION\x10\x05\x12\x10\n\x0c\x42\x41LL_MILLING\x10\x06\x12\x0e\n\nSONICATION\x10\x07\"\xe8\x02\n\x16IlluminationConditions\x12:\n\x04type\x18\x01 \x01(\x0e\x32,.ord.IlluminationConditions.IlluminationType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12(\n\x0fpeak_wavelength\x18\x03 \x01(\x0b\x32\x0f.ord.Wavelength\x12\r\n\x05\x63olor\x18\x04 \x01(\t\x12\'\n\x12\x64istance_to_vessel\x18\x05 \x01(\x0b\x32\x0b.ord.Length\"\x9e\x01\n\x10IlluminationType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0b\n\x07\x41MBIENT\x10\x02\x12\x08\n\x04\x44\x41RK\x10\x03\x12\x07\n\x03LED\x10\x04\x12\x10\n\x0cHALOGEN_LAMP\x10\x05\x12\x12\n\x0e\x44\x45UTERIUM_LAMP\x10\x06\x12\x13\n\x0fSOLAR_SIMULATOR\x10\x07\x12\x12\n\x0e\x42ROAD_SPECTRUM\x10\x08\"\xed\x06\n\x1a\x45lectrochemistryConditions\x12\x42\n\x04type\x18\x01 \x01(\x0e\x32\x34.ord.ElectrochemistryConditions.ElectrochemistryType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1d\n\x07\x63urrent\x18\x03 \x01(\x0b\x32\x0c.ord.Current\x12\x1d\n\x07voltage\x18\x04 \x01(\x0b\x32\x0c.ord.Voltage\x12\x16\n\x0e\x61node_material\x18\x05 \x01(\t\x12\x18\n\x10\x63\x61thode_material\x18\x06 \x01(\t\x12)\n\x14\x65lectrode_separation\x18\x07 \x01(\x0b\x32\x0b.ord.Length\x12Q\n\x0cmeasurements\x18\x08 \x03(\x0b\x32;.ord.ElectrochemistryConditions.ElectrochemistryMeasurement\x12\x42\n\x04\x63\x65ll\x18\t \x01(\x0b\x32\x34.ord.ElectrochemistryConditions.ElectrochemistryCell\x1a\x80\x01\n\x1b\x45lectrochemistryMeasurement\x12\x17\n\x04time\x18\x01 \x01(\x0b\x32\t.ord.Time\x12\x1f\n\x07\x63urrent\x18\x02 \x01(\x0b\x32\x0c.ord.CurrentH\x00\x12\x1f\n\x07voltage\x18\x03 \x01(\x0b\x32\x0c.ord.VoltageH\x00\x42\x06\n\x04kind\x1a\xe3\x01\n\x14\x45lectrochemistryCell\x12[\n\x04type\x18\x01 \x01(\x0e\x32M.ord.ElectrochemistryConditions.ElectrochemistryCell.ElectrochemistryCellType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"]\n\x18\x45lectrochemistryCellType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x10\n\x0c\x44IVIDED_CELL\x10\x02\x12\x12\n\x0eUNDIVIDED_CELL\x10\x03\"_\n\x14\x45lectrochemistryType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x14\n\x10\x43ONSTANT_CURRENT\x10\x02\x12\x14\n\x10\x43ONSTANT_VOLTAGE\x10\x03\"\x94\x04\n\x0e\x46lowConditions\x12*\n\x04type\x18\x01 \x01(\x0e\x32\x1c.ord.FlowConditions.FlowType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x11\n\tpump_type\x18\x03 \x01(\t\x12*\n\x06tubing\x18\x04 \x01(\x0b\x32\x1a.ord.FlowConditions.Tubing\x1a\x88\x02\n\x06Tubing\x12\x33\n\x04type\x18\x01 \x01(\x0e\x32%.ord.FlowConditions.Tubing.TubingType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1d\n\x08\x64iameter\x18\x03 \x01(\x0b\x32\x0b.ord.Length\"\x98\x01\n\nTubingType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\t\n\x05STEEL\x10\x02\x12\n\n\x06\x43OPPER\x10\x03\x12\x07\n\x03PFA\x10\x04\x12\x07\n\x03\x46\x45P\x10\x05\x12\x0c\n\x08TEFLONAF\x10\x06\x12\x08\n\x04PTFE\x10\x07\x12\t\n\x05GLASS\x10\x08\x12\n\n\x06QUARTZ\x10\t\x12\x0b\n\x07SILICON\x10\n\x12\x08\n\x04PDMS\x10\x0b\"{\n\x08\x46lowType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x15\n\x11PLUG_FLOW_REACTOR\x10\x02\x12#\n\x1f\x43ONTINUOUS_STIRRED_TANK_REACTOR\x10\x03\x12\x16\n\x12PACKED_BED_REACTOR\x10\x04\"\xc0\x03\n\rReactionNotes\x12\x1d\n\x10is_heterogeneous\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x1e\n\x11\x66orms_precipitate\x18\x02 \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\ris_exothermic\x18\x03 \x01(\x08H\x02\x88\x01\x01\x12\x16\n\toffgasses\x18\x04 \x01(\x08H\x03\x88\x01\x01\x12%\n\x18is_sensitive_to_moisture\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12#\n\x16is_sensitive_to_oxygen\x18\x06 \x01(\x08H\x05\x88\x01\x01\x12\"\n\x15is_sensitive_to_light\x18\x07 \x01(\x08H\x06\x88\x01\x01\x12\x14\n\x0csafety_notes\x18\x08 \x01(\t\x12\x19\n\x11procedure_details\x18\t \x01(\tB\x13\n\x11_is_heterogeneousB\x14\n\x12_forms_precipitateB\x10\n\x0e_is_exothermicB\x0c\n\n_offgassesB\x1b\n\x19_is_sensitive_to_moistureB\x19\n\x17_is_sensitive_to_oxygenB\x18\n\x16_is_sensitive_to_light\"Y\n\x13ReactionObservation\x12\x17\n\x04time\x18\x01 \x01(\x0b\x32\t.ord.Time\x12\x0f\n\x07\x63omment\x18\x02 \x01(\t\x12\x18\n\x05image\x18\x03 \x01(\x0b\x32\t.ord.Data\"\xcb\x05\n\x0eReactionWorkup\x12\x34\n\x04type\x18\x01 \x01(\x0e\x32&.ord.ReactionWorkup.ReactionWorkupType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1b\n\x08\x64uration\x18\x03 \x01(\x0b\x32\t.ord.Time\x12!\n\x05input\x18\x04 \x01(\x0b\x32\x12.ord.ReactionInput\x12\x1b\n\x06\x61mount\x18\x05 \x01(\x0b\x32\x0b.ord.Amount\x12/\n\x0btemperature\x18\x06 \x01(\x0b\x32\x1a.ord.TemperatureConditions\x12\x12\n\nkeep_phase\x18\x07 \x01(\t\x12)\n\x08stirring\x18\x08 \x01(\x0b\x32\x17.ord.StirringConditions\x12\x16\n\ttarget_ph\x18\t \x01(\x02H\x00\x88\x01\x01\x12\x19\n\x0cis_automated\x18\n \x01(\x08H\x01\x88\x01\x01\"\xd2\x02\n\x12ReactionWorkupType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0c\n\x08\x41\x44\x44ITION\x10\x02\x12\x0b\n\x07\x41LIQUOT\x10\x03\x12\x0f\n\x0bTEMPERATURE\x10\x04\x12\x11\n\rCONCENTRATION\x10\x05\x12\x0e\n\nEXTRACTION\x10\x06\x12\x0e\n\nFILTRATION\x10\x07\x12\x08\n\x04WASH\x10\x08\x12\x11\n\rDRY_IN_VACUUM\x10\t\x12\x15\n\x11\x44RY_WITH_MATERIAL\x10\n\x12\x18\n\x14\x46LASH_CHROMATOGRAPHY\x10\x0b\x12\x18\n\x14OTHER_CHROMATOGRAPHY\x10\x0c\x12\x0e\n\nSCAVENGING\x10\r\x12\x08\n\x04WAIT\x10\x0e\x12\x0c\n\x08STIRRING\x10\x0f\x12\r\n\tPH_ADJUST\x10\x10\x12\x0f\n\x0b\x44ISSOLUTION\x10\x11\x12\x10\n\x0c\x44ISTILLATION\x10\x12\x42\x0c\n\n_target_phB\x0f\n\r_is_automated\"\xf6\x01\n\x0fReactionOutcome\x12 \n\rreaction_time\x18\x01 \x01(\x0b\x32\t.ord.Time\x12#\n\nconversion\x18\x02 \x01(\x0b\x32\x0f.ord.Percentage\x12&\n\x08products\x18\x03 \x03(\x0b\x32\x14.ord.ProductCompound\x12\x34\n\x08\x61nalyses\x18\x04 \x03(\x0b\x32\".ord.ReactionOutcome.AnalysesEntry\x1a>\n\rAnalysesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.ord.Analysis:\x02\x38\x01\"\x8d\x05\n\x0fProductCompound\x12,\n\x0bidentifiers\x18\x01 \x03(\x0b\x32\x17.ord.CompoundIdentifier\x12\x1f\n\x12is_desired_product\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12-\n\x0cmeasurements\x18\x03 \x03(\x0b\x32\x17.ord.ProductMeasurement\x12\x16\n\x0eisolated_color\x18\x04 \x01(\t\x12-\n\x07texture\x18\x05 \x01(\x0b\x32\x1c.ord.ProductCompound.Texture\x12\x34\n\x08\x66\x65\x61tures\x18\x06 \x03(\x0b\x32\".ord.ProductCompound.FeaturesEntry\x12\x39\n\rreaction_role\x18\x07 \x01(\x0e\x32\".ord.ReactionRole.ReactionRoleType\x1a\xf0\x01\n\x07Texture\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.ord.ProductCompound.Texture.TextureType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\x9b\x01\n\x0bTextureType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\n\n\x06POWDER\x10\x02\x12\x0b\n\x07\x43RYSTAL\x10\x03\x12\x07\n\x03OIL\x10\x04\x12\x13\n\x0f\x41MORPHOUS_SOLID\x10\x05\x12\x08\n\x04\x46OAM\x10\x06\x12\x07\n\x03WAX\x10\x07\x12\x0e\n\nSEMI_SOLID\x10\x08\x12\t\n\x05SOLID\x10\t\x12\n\n\x06LIQUID\x10\n\x1a:\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x42\x15\n\x13_is_desired_product\"\xfb\n\n\x12ProductMeasurement\x12\x14\n\x0c\x61nalysis_key\x18\x01 \x01(\t\x12<\n\x04type\x18\x02 \x01(\x0e\x32..ord.ProductMeasurement.ProductMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\t\x12#\n\x16uses_internal_standard\x18\x04 \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\ris_normalized\x18\x05 \x01(\x08H\x02\x88\x01\x01\x12$\n\x17uses_authentic_standard\x18\x06 \x01(\x08H\x03\x88\x01\x01\x12)\n\x12\x61uthentic_standard\x18\x07 \x01(\x0b\x32\r.ord.Compound\x12%\n\npercentage\x18\x08 \x01(\x0b\x32\x0f.ord.PercentageH\x00\x12&\n\x0b\x66loat_value\x18\t \x01(\x0b\x32\x0f.ord.FloatValueH\x00\x12\x16\n\x0cstring_value\x18\n \x01(\tH\x00\x12\x1d\n\x06\x61mount\x18\x0b \x01(\x0b\x32\x0b.ord.AmountH\x00\x12!\n\x0eretention_time\x18\x0c \x01(\x0b\x32\t.ord.Time\x12M\n\x11mass_spec_details\x18\r \x01(\x0b\x32\x32.ord.ProductMeasurement.MassSpecMeasurementDetails\x12\x38\n\x0bselectivity\x18\x0e \x01(\x0b\x32#.ord.ProductMeasurement.Selectivity\x12#\n\nwavelength\x18\x0f \x01(\x0b\x32\x0f.ord.Wavelength\x1a\xe9\x02\n\x1aMassSpecMeasurementDetails\x12X\n\x04type\x18\x01 \x01(\x0e\x32J.ord.ProductMeasurement.MassSpecMeasurementDetails.MassSpecMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1b\n\x0etic_minimum_mz\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12\x1b\n\x0etic_maximum_mz\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\neic_masses\x18\x05 \x03(\x02\"l\n\x17MassSpecMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x07\n\x03TIC\x10\x02\x12\x10\n\x0cTIC_POSITIVE\x10\x03\x12\x10\n\x0cTIC_NEGATIVE\x10\x04\x12\x07\n\x03\x45IC\x10\x05\x42\x11\n\x0f_tic_minimum_mzB\x11\n\x0f_tic_maximum_mz\x1a\xb9\x01\n\x0bSelectivity\x12\x41\n\x04type\x18\x01 \x01(\x0e\x32\x33.ord.ProductMeasurement.Selectivity.SelectivityType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"V\n\x0fSelectivityType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x06\n\x02\x45\x45\x10\x02\x12\x06\n\x02\x45R\x10\x03\x12\x06\n\x02\x44R\x10\x04\x12\x06\n\x02\x45Z\x10\x05\x12\x06\n\x02ZE\x10\x06\"\x9c\x01\n\x16ProductMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0c\n\x08IDENTITY\x10\x02\x12\t\n\x05YIELD\x10\x03\x12\x0f\n\x0bSELECTIVITY\x10\x04\x12\n\n\x06PURITY\x10\x05\x12\x08\n\x04\x41REA\x10\x06\x12\n\n\x06\x43OUNTS\x10\x07\x12\r\n\tINTENSITY\x10\x08\x12\n\n\x06\x41MOUNT\x10\tB\x07\n\x05valueB\x19\n\x17_uses_internal_standardB\x10\n\x0e_is_normalizedB\x1a\n\x18_uses_authentic_standard\"\x19\n\x08\x44\x61teTime\x12\r\n\x05value\x18\x01 \x01(\t\"\xcc\x04\n\x08\x41nalysis\x12(\n\x04type\x18\x01 \x01(\x0e\x32\x1a.ord.Analysis.AnalysisType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x0f\n\x07\x63hmo_id\x18\x03 \x01(\x05\x12#\n\x16is_of_isolated_species\x18\x04 \x01(\x08H\x00\x88\x01\x01\x12%\n\x04\x64\x61ta\x18\x05 \x03(\x0b\x32\x17.ord.Analysis.DataEntry\x12\x1f\n\x17instrument_manufacturer\x18\x06 \x01(\t\x12\x31\n\x1ainstrument_last_calibrated\x18\x07 \x01(\x0b\x32\r.ord.DateTime\x1a\x36\n\tDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\"\x80\x02\n\x0c\x41nalysisType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x06\n\x02LC\x10\x02\x12\x06\n\x02GC\x10\x03\x12\x06\n\x02IR\x10\x04\x12\n\n\x06NMR_1H\x10\x05\x12\x0b\n\x07NMR_13C\x10\x06\x12\r\n\tNMR_OTHER\x10\x07\x12\x06\n\x02MP\x10\x08\x12\x06\n\x02UV\x10\t\x12\x07\n\x03TLC\x10\n\x12\x06\n\x02MS\x10\x0b\x12\x08\n\x04HRMS\x10\x0c\x12\x08\n\x04MSMS\x10\r\x12\n\n\x06WEIGHT\x10\x0e\x12\x08\n\x04LCMS\x10\x0f\x12\x08\n\x04GCMS\x10\x10\x12\x08\n\x04\x45LSD\x10\x11\x12\x06\n\x02\x43\x44\x10\x12\x12\x07\n\x03SFC\x10\x13\x12\x07\n\x03\x45PR\x10\x14\x12\x07\n\x03XRD\x10\x15\x12\t\n\x05RAMAN\x10\x16\x12\x06\n\x02\x45\x44\x10\x17\x42\x19\n\x17_is_of_isolated_species\"\xf9\x01\n\x12ReactionProvenance\x12!\n\x0c\x65xperimenter\x18\x01 \x01(\x0b\x32\x0b.ord.Person\x12\x0c\n\x04\x63ity\x18\x02 \x01(\t\x12\'\n\x10\x65xperiment_start\x18\x03 \x01(\x0b\x32\r.ord.DateTime\x12\x0b\n\x03\x64oi\x18\x04 \x01(\t\x12\x0e\n\x06patent\x18\x05 \x01(\t\x12\x17\n\x0fpublication_url\x18\x06 \x01(\t\x12(\n\x0erecord_created\x18\x07 \x01(\x0b\x32\x10.ord.RecordEvent\x12)\n\x0frecord_modified\x18\x08 \x03(\x0b\x32\x10.ord.RecordEvent\"\\\n\x06Person\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05orcid\x18\x03 \x01(\t\x12\x14\n\x0corganization\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x01(\t\"X\n\x0bRecordEvent\x12\x1b\n\x04time\x18\x01 \x01(\x0b\x32\r.ord.DateTime\x12\x1b\n\x06person\x18\x02 \x01(\x0b\x32\x0b.ord.Person\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\t\"\xb5\x01\n\x04Time\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12!\n\x05units\x18\x03 \x01(\x0e\x32\x12.ord.Time.TimeUnit\"F\n\x08TimeUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x07\n\x03\x44\x41Y\x10\x04\x12\x08\n\x04HOUR\x10\x01\x12\n\n\x06MINUTE\x10\x02\x12\n\n\x06SECOND\x10\x03\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xc0\x01\n\x04Mass\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12!\n\x05units\x18\x03 \x01(\x0e\x32\x12.ord.Mass.MassUnit\"Q\n\x08MassUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0c\n\x08KILOGRAM\x10\x01\x12\x08\n\x04GRAM\x10\x02\x12\r\n\tMILLIGRAM\x10\x03\x12\r\n\tMICROGRAM\x10\x04\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xc4\x01\n\x05Moles\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12#\n\x05units\x18\x03 \x01(\x0e\x32\x14.ord.Moles.MolesUnit\"R\n\tMolesUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04MOLE\x10\x01\x12\r\n\tMILLIMOLE\x10\x02\x12\r\n\tMICROMOLE\x10\x03\x12\x0c\n\x08NANOMOLE\x10\x04\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xcc\x01\n\x06Volume\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12%\n\x05units\x18\x03 \x01(\x0e\x32\x16.ord.Volume.VolumeUnit\"W\n\nVolumeUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\t\n\x05LITER\x10\x01\x12\x0e\n\nMILLILITER\x10\x02\x12\x0e\n\nMICROLITER\x10\x03\x12\r\n\tNANOLITER\x10\x04\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xd9\x01\n\rConcentration\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x33\n\x05units\x18\x03 \x01(\x0e\x32$.ord.Concentration.ConcentrationUnit\"O\n\x11\x43oncentrationUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\t\n\x05MOLAR\x10\x01\x12\x0e\n\nMILLIMOLAR\x10\x02\x12\x0e\n\nMICROMOLAR\x10\x03\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xf7\x01\n\x08Pressure\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12)\n\x05units\x18\x03 \x01(\x0e\x32\x1a.ord.Pressure.PressureUnit\"|\n\x0cPressureUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x07\n\x03\x42\x41R\x10\x01\x12\x0e\n\nATMOSPHERE\x10\x02\x12\x07\n\x03PSI\x10\x03\x12\x08\n\x04KPSI\x10\x04\x12\n\n\x06PASCAL\x10\x05\x12\x0e\n\nKILOPASCAL\x10\x06\x12\x08\n\x04TORR\x10\x07\x12\t\n\x05MM_HG\x10\x08\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xcf\x01\n\x0bTemperature\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12/\n\x05units\x18\x03 \x01(\x0e\x32 .ord.Temperature.TemperatureUnit\"K\n\x0fTemperatureUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0b\n\x07\x43\x45LSIUS\x10\x01\x12\x0e\n\nFAHRENHEIT\x10\x02\x12\n\n\x06KELVIN\x10\x03\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xb3\x01\n\x07\x43urrent\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\'\n\x05units\x18\x03 \x01(\x0e\x32\x18.ord.Current.CurrentUnit\";\n\x0b\x43urrentUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x41MPERE\x10\x01\x12\x0f\n\x0bMILLIAMPERE\x10\x02\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xaf\x01\n\x07Voltage\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\'\n\x05units\x18\x03 \x01(\x0e\x32\x18.ord.Voltage.VoltageUnit\"7\n\x0bVoltageUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04VOLT\x10\x01\x12\r\n\tMILLIVOLT\x10\x02\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xd1\x01\n\x06Length\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12%\n\x05units\x18\x03 \x01(\x0e\x32\x16.ord.Length.LengthUnit\"\\\n\nLengthUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0e\n\nCENTIMETER\x10\x01\x12\x0e\n\nMILLIMETER\x10\x02\x12\t\n\x05METER\x10\x03\x12\x08\n\x04INCH\x10\x04\x12\x08\n\x04\x46OOT\x10\x05\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xc1\x01\n\nWavelength\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12-\n\x05units\x18\x03 \x01(\x0e\x32\x1e.ord.Wavelength.WavelengthUnit\"@\n\x0eWavelengthUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\r\n\tNANOMETER\x10\x01\x12\x0e\n\nWAVENUMBER\x10\x02\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xa0\x02\n\x08\x46lowRate\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12)\n\x05units\x18\x03 \x01(\x0e\x32\x1a.ord.FlowRate.FlowRateUnit\"\xa4\x01\n\x0c\x46lowRateUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x19\n\x15MICROLITER_PER_MINUTE\x10\x01\x12\x19\n\x15MICROLITER_PER_SECOND\x10\x02\x12\x19\n\x15MILLILITER_PER_MINUTE\x10\x03\x12\x19\n\x15MILLILITER_PER_SECOND\x10\x04\x12\x17\n\x13MICROLITER_PER_HOUR\x10\x05\x42\x08\n\x06_valueB\x0c\n\n_precision\"P\n\nPercentage\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x08\n\x06_valueB\x0c\n\n_precision\"P\n\nFloatValue\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xa1\x01\n\x04\x44\x61ta\x12\x15\n\x0b\x66loat_value\x18\x01 \x01(\x02H\x00\x12\x17\n\rinteger_value\x18\x02 \x01(\x05H\x00\x12\x15\n\x0b\x62ytes_value\x18\x03 \x01(\x0cH\x00\x12\x16\n\x0cstring_value\x18\x04 \x01(\tH\x00\x12\r\n\x03url\x18\x05 \x01(\tH\x00\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x07 \x01(\tB\x06\n\x04kindb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ford-schema/proto/reaction.proto\x12\x03ord\"\xd9\x03\n\x08Reaction\x12,\n\x0bidentifiers\x18\x01 \x03(\x0b\x32\x17.ord.ReactionIdentifier\x12)\n\x06inputs\x18\x02 \x03(\x0b\x32\x19.ord.Reaction.InputsEntry\x12!\n\x05setup\x18\x03 \x01(\x0b\x32\x12.ord.ReactionSetup\x12+\n\nconditions\x18\x04 \x01(\x0b\x32\x17.ord.ReactionConditions\x12!\n\x05notes\x18\x05 \x01(\x0b\x32\x12.ord.ReactionNotes\x12.\n\x0cobservations\x18\x06 \x03(\x0b\x32\x18.ord.ReactionObservation\x12$\n\x07workups\x18\x07 \x03(\x0b\x32\x13.ord.ReactionWorkup\x12&\n\x08outcomes\x18\x08 \x03(\x0b\x32\x14.ord.ReactionOutcome\x12+\n\nprovenance\x18\t \x01(\x0b\x32\x17.ord.ReactionProvenance\x12\x13\n\x0breaction_id\x18\n \x01(\t\x1a\x41\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.ord.ReactionInput:\x02\x38\x01\"\xa7\x02\n\x12ReactionIdentifier\x12<\n\x04type\x18\x01 \x01(\x0e\x32..ord.ReactionIdentifier.ReactionIdentifierType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x16\n\tis_mapped\x18\x04 \x01(\x08H\x00\x88\x01\x01\"\x8c\x01\n\x16ReactionIdentifierType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x13\n\x0fREACTION_SMILES\x10\x02\x12\x15\n\x11REACTION_CXSMILES\x10\x06\x12\n\n\x06RDFILE\x10\x03\x12\n\n\x06RINCHI\x10\x04\x12\x11\n\rREACTION_TYPE\x10\x05\x42\x0c\n\n_is_mapped\"\xbc\x06\n\rReactionInput\x12!\n\ncomponents\x18\x01 \x03(\x0b\x32\r.ord.Compound\x12-\n\x10\x63rude_components\x18\x02 \x03(\x0b\x32\x13.ord.CrudeComponent\x12\x16\n\x0e\x61\x64\x64ition_order\x18\x03 \x01(\x05\x12 \n\raddition_time\x18\x04 \x01(\x0b\x32\t.ord.Time\x12\x38\n\x0e\x61\x64\x64ition_speed\x18\x05 \x01(\x0b\x32 .ord.ReactionInput.AdditionSpeed\x12$\n\x11\x61\x64\x64ition_duration\x18\x06 \x01(\x0b\x32\t.ord.Time\x12 \n\tflow_rate\x18\x07 \x01(\x0b\x32\r.ord.FlowRate\x12:\n\x0f\x61\x64\x64ition_device\x18\x08 \x01(\x0b\x32!.ord.ReactionInput.AdditionDevice\x12.\n\x14\x61\x64\x64ition_temperature\x18\t \x01(\x0b\x32\x10.ord.Temperature\x1a\xdc\x01\n\rAdditionSpeed\x12@\n\x04type\x18\x01 \x01(\x0e\x32\x32.ord.ReactionInput.AdditionSpeed.AdditionSpeedType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"x\n\x11\x41\x64\x64itionSpeedType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0f\n\x0b\x41LL_AT_ONCE\x10\x01\x12\x08\n\x04\x46\x41ST\x10\x02\x12\x08\n\x04SLOW\x10\x03\x12\x0c\n\x08\x44ROPWISE\x10\x04\x12\x0e\n\nCONTINUOUS\x10\x05\x12\x0f\n\x0bPORTIONWISE\x10\x06\x1a\xd1\x01\n\x0e\x41\x64\x64itionDevice\x12\x42\n\x04type\x18\x01 \x01(\x0e\x32\x34.ord.ReactionInput.AdditionDevice.AdditionDeviceType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"j\n\x12\x41\x64\x64itionDeviceType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0b\n\x07SYRINGE\x10\x03\x12\x0b\n\x07\x43\x41NNULA\x10\x04\x12\x13\n\x0f\x41\x44\x44ITION_FUNNEL\x10\x05\"\xd6\x01\n\x06\x41mount\x12\x19\n\x04mass\x18\x01 \x01(\x0b\x32\t.ord.MassH\x00\x12\x1b\n\x05moles\x18\x02 \x01(\x0b\x32\n.ord.MolesH\x00\x12\x1d\n\x06volume\x18\x03 \x01(\x0b\x32\x0b.ord.VolumeH\x00\x12+\n\nunmeasured\x18\x05 \x01(\x0b\x32\x15.ord.UnmeasuredAmountH\x00\x12$\n\x17volume_includes_solutes\x18\x04 \x01(\x08H\x01\x88\x01\x01\x42\x06\n\x04kindB\x1a\n\x18_volume_includes_solutes\"\xbe\x01\n\x10UnmeasuredAmount\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.ord.UnmeasuredAmount.UnmeasuredAmountType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"_\n\x14UnmeasuredAmountType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\r\n\tSATURATED\x10\x02\x12\r\n\tCATALYTIC\x10\x03\x12\x0c\n\x08TITRATED\x10\x04\"\xac\x01\n\x0e\x43rudeComponent\x12\x13\n\x0breaction_id\x18\x01 \x01(\t\x12\x1c\n\x0fincludes_workup\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1f\n\x12has_derived_amount\x18\x03 \x01(\x08H\x01\x88\x01\x01\x12\x1b\n\x06\x61mount\x18\x04 \x01(\x0b\x32\x0b.ord.AmountB\x12\n\x10_includes_workupB\x15\n\x13_has_derived_amount\"\xa5\x04\n\x08\x43ompound\x12,\n\x0bidentifiers\x18\x01 \x03(\x0b\x32\x17.ord.CompoundIdentifier\x12\x1b\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x0b.ord.Amount\x12\x39\n\rreaction_role\x18\x03 \x01(\x0e\x32\".ord.ReactionRole.ReactionRoleType\x12\x18\n\x0bis_limiting\x18\x04 \x01(\x08H\x00\x88\x01\x01\x12.\n\x0cpreparations\x18\x05 \x03(\x0b\x32\x18.ord.CompoundPreparation\x12$\n\x06source\x18\x06 \x01(\x0b\x32\x14.ord.Compound.Source\x12-\n\x08\x66\x65\x61tures\x18\x07 \x03(\x0b\x32\x1b.ord.Compound.FeaturesEntry\x12-\n\x08\x61nalyses\x18\x08 \x03(\x0b\x32\x1b.ord.Compound.AnalysesEntry\x1a\x39\n\x06Source\x12\x0e\n\x06vendor\x18\x01 \x01(\t\x12\x12\n\ncatalog_id\x18\x02 \x01(\t\x12\x0b\n\x03lot\x18\x03 \x01(\t\x1a:\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x1a>\n\rAnalysesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.ord.Analysis:\x02\x38\x01\x42\x0e\n\x0c_is_limiting\"\xb2\x01\n\x0cReactionRole\"\xa1\x01\n\x10ReactionRoleType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0c\n\x08REACTANT\x10\x01\x12\x0b\n\x07REAGENT\x10\x02\x12\x0b\n\x07SOLVENT\x10\x03\x12\x0c\n\x08\x43\x41TALYST\x10\x04\x12\n\n\x06WORKUP\x10\x05\x12\x15\n\x11INTERNAL_STANDARD\x10\x06\x12\x16\n\x12\x41UTHENTIC_STANDARD\x10\x07\x12\x0b\n\x07PRODUCT\x10\x08\"\xf6\x01\n\x13\x43ompoundPreparation\x12>\n\x04type\x18\x01 \x01(\x0e\x32\x30.ord.CompoundPreparation.CompoundPreparationType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x13\n\x0breaction_id\x18\x03 \x01(\t\"y\n\x17\x43ompoundPreparationType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0e\n\nREPURIFIED\x10\x03\x12\x0b\n\x07SPARGED\x10\x04\x12\t\n\x05\x44RIED\x10\x05\x12\x0f\n\x0bSYNTHESIZED\x10\x06\"\x82\x03\n\x12\x43ompoundIdentifier\x12<\n\x04type\x18\x01 \x01(\x0e\x32..ord.CompoundIdentifier.CompoundIdentifierType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\x8d\x02\n\x16\x43ompoundIdentifierType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\n\n\x06SMILES\x10\x02\x12\t\n\x05INCHI\x10\x03\x12\x0c\n\x08MOLBLOCK\x10\x04\x12\x0e\n\nIUPAC_NAME\x10\x05\x12\x08\n\x04NAME\x10\x06\x12\x0e\n\nCAS_NUMBER\x10\x07\x12\x0f\n\x0bPUBCHEM_CID\x10\x08\x12\x11\n\rCHEMSPIDER_ID\x10\t\x12\x0c\n\x08\x43XSMILES\x10\n\x12\r\n\tINCHI_KEY\x10\x0b\x12\x07\n\x03XYZ\x10\x0c\x12\x0e\n\nUNIPROT_ID\x10\r\x12\n\n\x06PDB_ID\x10\x0e\x12\x17\n\x13\x41MINO_ACID_SEQUENCE\x10\x0f\x12\x08\n\x04HELM\x10\x10\"\xa7\x04\n\x06Vessel\x12$\n\x04type\x18\x01 \x01(\x0e\x32\x16.ord.Vessel.VesselType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12%\n\x08material\x18\x03 \x01(\x0b\x32\x13.ord.VesselMaterial\x12,\n\x0cpreparations\x18\x04 \x03(\x0b\x32\x16.ord.VesselPreparation\x12*\n\x0b\x61ttachments\x18\x05 \x03(\x0b\x32\x15.ord.VesselAttachment\x12\x1b\n\x06volume\x18\x06 \x01(\x0b\x32\x0b.ord.Volume\x12\x11\n\tvessel_id\x18\x07 \x01(\t\x12\x10\n\x08position\x18\x08 \x01(\t\x12\x0b\n\x03row\x18\t \x01(\t\x12\x0b\n\x03\x63ol\x18\n \x01(\t\"\x88\x02\n\nVesselType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x16\n\x12ROUND_BOTTOM_FLASK\x10\x02\x12\x08\n\x04VIAL\x10\x03\x12\x0e\n\nWELL_PLATE\x10\x04\x12\x12\n\x0eMICROWAVE_VIAL\x10\x05\x12\x08\n\x04TUBE\x10\x06\x12#\n\x1f\x43ONTINUOUS_STIRRED_TANK_REACTOR\x10\x07\x12\x16\n\x12PACKED_BED_REACTOR\x10\x08\x12\x0c\n\x08NMR_TUBE\x10\t\x12\x12\n\x0ePRESSURE_FLASK\x10\n\x12\x14\n\x10PRESSURE_REACTOR\x10\x0b\x12\x18\n\x14\x45LECTROCHEMICAL_CELL\x10\x0c\"\xcc\x01\n\x0eVesselMaterial\x12\x34\n\x04type\x18\x01 \x01(\x0e\x32&.ord.VesselMaterial.VesselMaterialType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"s\n\x12VesselMaterialType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\t\n\x05GLASS\x10\x02\x12\x11\n\rPOLYPROPYLENE\x10\x03\x12\x0b\n\x07PLASTIC\x10\x04\x12\t\n\x05METAL\x10\x05\x12\n\n\x06QUARTZ\x10\x06\"\x97\x03\n\x10VesselAttachment\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.ord.VesselAttachment.VesselAttachmentType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\xb7\x02\n\x14VesselAttachmentType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\n\n\x06SEPTUM\x10\x03\x12\x07\n\x03\x43\x41P\x10\x04\x12\x07\n\x03MAT\x10\x05\x12\x14\n\x10REFLUX_CONDENSER\x10\x06\x12\x0f\n\x0bVENT_NEEDLE\x10\x07\x12\x0e\n\nDEAN_STARK\x10\x08\x12\x0f\n\x0bVACUUM_TUBE\x10\t\x12\x13\n\x0f\x41\x44\x44ITION_FUNNEL\x10\n\x12\x0f\n\x0b\x44RYING_TUBE\x10\x0b\x12\x11\n\rALUMINUM_FOIL\x10\x0c\x12\x10\n\x0cTHERMOCOUPLE\x10\r\x12\x0b\n\x07\x42\x41LLOON\x10\x0e\x12\x0f\n\x0bGAS_ADAPTER\x10\x0f\x12\x16\n\x12PRESSURE_REGULATOR\x10\x10\x12\x11\n\rRELEASE_VALVE\x10\x11\"\xe8\x01\n\x11VesselPreparation\x12:\n\x04type\x18\x01 \x01(\x0e\x32,.ord.VesselPreparation.VesselPreparationType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\x85\x01\n\x15VesselPreparationType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0e\n\nOVEN_DRIED\x10\x03\x12\x0f\n\x0b\x46LAME_DRIED\x10\x04\x12\x18\n\x14\x45VACUATED_BACKFILLED\x10\x05\x12\n\n\x06PURGED\x10\x06\"\xa0\x04\n\rReactionSetup\x12\x1b\n\x06vessel\x18\x01 \x01(\x0b\x32\x0b.ord.Vessel\x12\x19\n\x0cis_automated\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1b\n\x13\x61utomation_platform\x18\x03 \x01(\t\x12?\n\x0f\x61utomation_code\x18\x04 \x03(\x0b\x32&.ord.ReactionSetup.AutomationCodeEntry\x12;\n\x0b\x65nvironment\x18\x05 \x01(\x0b\x32&.ord.ReactionSetup.ReactionEnvironment\x1a@\n\x13\x41utomationCodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x1a\xe8\x01\n\x13ReactionEnvironment\x12L\n\x04type\x18\x01 \x01(\x0e\x32>.ord.ReactionSetup.ReactionEnvironment.ReactionEnvironmentType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"r\n\x17ReactionEnvironmentType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\r\n\tFUME_HOOD\x10\x02\x12\r\n\tBENCH_TOP\x10\x03\x12\r\n\tGLOVE_BOX\x10\x04\x12\r\n\tGLOVE_BAG\x10\x05\x42\x0f\n\r_is_automated\"\xb5\x03\n\x12ReactionConditions\x12/\n\x0btemperature\x18\x01 \x01(\x0b\x32\x1a.ord.TemperatureConditions\x12)\n\x08pressure\x18\x02 \x01(\x0b\x32\x17.ord.PressureConditions\x12)\n\x08stirring\x18\x03 \x01(\x0b\x32\x17.ord.StirringConditions\x12\x31\n\x0cillumination\x18\x04 \x01(\x0b\x32\x1b.ord.IlluminationConditions\x12\x39\n\x10\x65lectrochemistry\x18\x05 \x01(\x0b\x32\x1f.ord.ElectrochemistryConditions\x12!\n\x04\x66low\x18\x06 \x01(\x0b\x32\x13.ord.FlowConditions\x12\x13\n\x06reflux\x18\x07 \x01(\x08H\x00\x88\x01\x01\x12\x0f\n\x02ph\x18\x08 \x01(\x02H\x01\x88\x01\x01\x12#\n\x16\x63onditions_are_dynamic\x18\t \x01(\x08H\x02\x88\x01\x01\x12\x0f\n\x07\x64\x65tails\x18\n \x01(\tB\t\n\x07_refluxB\x05\n\x03_phB\x19\n\x17_conditions_are_dynamic\"\xe2\x06\n\x15TemperatureConditions\x12>\n\x07\x63ontrol\x18\x01 \x01(\x0b\x32-.ord.TemperatureConditions.TemperatureControl\x12\"\n\x08setpoint\x18\x02 \x01(\x0b\x32\x10.ord.Temperature\x12G\n\x0cmeasurements\x18\x03 \x03(\x0b\x32\x31.ord.TemperatureConditions.TemperatureMeasurement\x1a\xd4\x02\n\x12TemperatureControl\x12R\n\x04type\x18\x01 \x01(\x0e\x32\x44.ord.TemperatureConditions.TemperatureControl.TemperatureControlType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\xd8\x01\n\x16TemperatureControlType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0b\n\x07\x41MBIENT\x10\x02\x12\x0c\n\x08OIL_BATH\x10\x03\x12\x0e\n\nWATER_BATH\x10\x04\x12\r\n\tSAND_BATH\x10\x05\x12\x0c\n\x08ICE_BATH\x10\x06\x12\x16\n\x12\x44RY_ALUMINUM_PLATE\x10\x07\x12\r\n\tMICROWAVE\x10\x08\x12\x10\n\x0c\x44RY_ICE_BATH\x10\t\x12\x0b\n\x07\x41IR_FAN\x10\n\x12\x13\n\x0fLIQUID_NITROGEN\x10\x0b\x1a\xc4\x02\n\x16TemperatureMeasurement\x12Z\n\x04type\x18\x01 \x01(\x0e\x32L.ord.TemperatureConditions.TemperatureMeasurement.TemperatureMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x17\n\x04time\x18\x03 \x01(\x0b\x32\t.ord.Time\x12%\n\x0btemperature\x18\x04 \x01(\x0b\x32\x10.ord.Temperature\"}\n\x1aTemperatureMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x19\n\x15THERMOCOUPLE_INTERNAL\x10\x02\x12\x19\n\x15THERMOCOUPLE_EXTERNAL\x10\x03\x12\x0c\n\x08INFRARED\x10\x04\"\x8c\x08\n\x12PressureConditions\x12\x38\n\x07\x63ontrol\x18\x01 \x01(\x0b\x32\'.ord.PressureConditions.PressureControl\x12\x1f\n\x08setpoint\x18\x02 \x01(\x0b\x32\r.ord.Pressure\x12\x36\n\natmosphere\x18\x03 \x01(\x0b\x32\".ord.PressureConditions.Atmosphere\x12\x41\n\x0cmeasurements\x18\x04 \x03(\x0b\x32+.ord.PressureConditions.PressureMeasurement\x1a\xe0\x01\n\x0fPressureControl\x12I\n\x04type\x18\x01 \x01(\x0e\x32;.ord.PressureConditions.PressureControl.PressureControlType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"q\n\x13PressureControlType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0b\n\x07\x41MBIENT\x10\x02\x12\x13\n\x0fSLIGHT_POSITIVE\x10\x03\x12\n\n\x06SEALED\x10\x04\x12\x0f\n\x0bPRESSURIZED\x10\x05\x1a\xb5\x02\n\nAtmosphere\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.ord.PressureConditions.Atmosphere.AtmosphereType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\xd4\x01\n\x0e\x41tmosphereType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x07\n\x03\x41IR\x10\x02\x12\x0c\n\x08NITROGEN\x10\x03\x12\t\n\x05\x41RGON\x10\x04\x12\n\n\x06OXYGEN\x10\x05\x12\x0c\n\x08HYDROGEN\x10\x06\x12\x13\n\x0f\x43\x41RBON_MONOXIDE\x10\x07\x12\x12\n\x0e\x43\x41RBON_DIOXIDE\x10\x08\x12\x0b\n\x07METHANE\x10\t\x12\x0b\n\x07\x41MMONIA\x10\n\x12\t\n\x05OZONE\x10\x0b\x12\x0c\n\x08\x45THYLENE\x10\x0c\x12\r\n\tACETYLENE\x10\r\x1a\x84\x02\n\x13PressureMeasurement\x12Q\n\x04type\x18\x01 \x01(\x0e\x32\x43.ord.PressureConditions.PressureMeasurement.PressureMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x17\n\x04time\x18\x03 \x01(\x0b\x32\t.ord.Time\x12\x1f\n\x08pressure\x18\x04 \x01(\x0b\x32\r.ord.Pressure\"O\n\x17PressureMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x17\n\x13PRESSURE_TRANSDUCER\x10\x02\"\xdc\x03\n\x12StirringConditions\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.ord.StirringConditions.StirringMethodType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x32\n\x04rate\x18\x03 \x01(\x0b\x32$.ord.StirringConditions.StirringRate\x1a\xb5\x01\n\x0cStirringRate\x12\x43\n\x04type\x18\x01 \x01(\x0e\x32\x35.ord.StirringConditions.StirringRate.StirringRateType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x0b\n\x03rpm\x18\x03 \x01(\x05\"B\n\x10StirringRateType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04HIGH\x10\x01\x12\n\n\x06MEDIUM\x10\x02\x12\x07\n\x03LOW\x10\x03\"\x8e\x01\n\x12StirringMethodType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0c\n\x08STIR_BAR\x10\x03\x12\x12\n\x0eOVERHEAD_MIXER\x10\x04\x12\r\n\tAGITATION\x10\x05\x12\x10\n\x0c\x42\x41LL_MILLING\x10\x06\x12\x0e\n\nSONICATION\x10\x07\"\xe8\x02\n\x16IlluminationConditions\x12:\n\x04type\x18\x01 \x01(\x0e\x32,.ord.IlluminationConditions.IlluminationType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12(\n\x0fpeak_wavelength\x18\x03 \x01(\x0b\x32\x0f.ord.Wavelength\x12\r\n\x05\x63olor\x18\x04 \x01(\t\x12\'\n\x12\x64istance_to_vessel\x18\x05 \x01(\x0b\x32\x0b.ord.Length\"\x9e\x01\n\x10IlluminationType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0b\n\x07\x41MBIENT\x10\x02\x12\x08\n\x04\x44\x41RK\x10\x03\x12\x07\n\x03LED\x10\x04\x12\x10\n\x0cHALOGEN_LAMP\x10\x05\x12\x12\n\x0e\x44\x45UTERIUM_LAMP\x10\x06\x12\x13\n\x0fSOLAR_SIMULATOR\x10\x07\x12\x12\n\x0e\x42ROAD_SPECTRUM\x10\x08\"\xe0\x06\n\x1a\x45lectrochemistryConditions\x12\x42\n\x04type\x18\x01 \x01(\x0e\x32\x34.ord.ElectrochemistryConditions.ElectrochemistryType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1d\n\x07\x63urrent\x18\x03 \x01(\x0b\x32\x0c.ord.Current\x12\x1d\n\x07voltage\x18\x04 \x01(\x0b\x32\x0c.ord.Voltage\x12\x16\n\x0e\x61node_material\x18\x05 \x01(\t\x12\x18\n\x10\x63\x61thode_material\x18\x06 \x01(\t\x12)\n\x14\x65lectrode_separation\x18\x07 \x01(\x0b\x32\x0b.ord.Length\x12Q\n\x0cmeasurements\x18\x08 \x03(\x0b\x32;.ord.ElectrochemistryConditions.ElectrochemistryMeasurement\x12\x42\n\x04\x63\x65ll\x18\t \x01(\x0b\x32\x34.ord.ElectrochemistryConditions.ElectrochemistryCell\x1at\n\x1b\x45lectrochemistryMeasurement\x12\x17\n\x04time\x18\x01 \x01(\x0b\x32\t.ord.Time\x12\x1d\n\x07\x63urrent\x18\x02 \x01(\x0b\x32\x0c.ord.Current\x12\x1d\n\x07voltage\x18\x03 \x01(\x0b\x32\x0c.ord.Voltage\x1a\xe3\x01\n\x14\x45lectrochemistryCell\x12[\n\x04type\x18\x01 \x01(\x0e\x32M.ord.ElectrochemistryConditions.ElectrochemistryCell.ElectrochemistryCellType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"]\n\x18\x45lectrochemistryCellType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x10\n\x0c\x44IVIDED_CELL\x10\x02\x12\x12\n\x0eUNDIVIDED_CELL\x10\x03\"_\n\x14\x45lectrochemistryType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x14\n\x10\x43ONSTANT_CURRENT\x10\x02\x12\x14\n\x10\x43ONSTANT_VOLTAGE\x10\x03\"\x94\x04\n\x0e\x46lowConditions\x12*\n\x04type\x18\x01 \x01(\x0e\x32\x1c.ord.FlowConditions.FlowType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x11\n\tpump_type\x18\x03 \x01(\t\x12*\n\x06tubing\x18\x04 \x01(\x0b\x32\x1a.ord.FlowConditions.Tubing\x1a\x88\x02\n\x06Tubing\x12\x33\n\x04type\x18\x01 \x01(\x0e\x32%.ord.FlowConditions.Tubing.TubingType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1d\n\x08\x64iameter\x18\x03 \x01(\x0b\x32\x0b.ord.Length\"\x98\x01\n\nTubingType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\t\n\x05STEEL\x10\x02\x12\n\n\x06\x43OPPER\x10\x03\x12\x07\n\x03PFA\x10\x04\x12\x07\n\x03\x46\x45P\x10\x05\x12\x0c\n\x08TEFLONAF\x10\x06\x12\x08\n\x04PTFE\x10\x07\x12\t\n\x05GLASS\x10\x08\x12\n\n\x06QUARTZ\x10\t\x12\x0b\n\x07SILICON\x10\n\x12\x08\n\x04PDMS\x10\x0b\"{\n\x08\x46lowType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x15\n\x11PLUG_FLOW_REACTOR\x10\x02\x12#\n\x1f\x43ONTINUOUS_STIRRED_TANK_REACTOR\x10\x03\x12\x16\n\x12PACKED_BED_REACTOR\x10\x04\"\xc0\x03\n\rReactionNotes\x12\x1d\n\x10is_heterogeneous\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x1e\n\x11\x66orms_precipitate\x18\x02 \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\ris_exothermic\x18\x03 \x01(\x08H\x02\x88\x01\x01\x12\x16\n\toffgasses\x18\x04 \x01(\x08H\x03\x88\x01\x01\x12%\n\x18is_sensitive_to_moisture\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12#\n\x16is_sensitive_to_oxygen\x18\x06 \x01(\x08H\x05\x88\x01\x01\x12\"\n\x15is_sensitive_to_light\x18\x07 \x01(\x08H\x06\x88\x01\x01\x12\x14\n\x0csafety_notes\x18\x08 \x01(\t\x12\x19\n\x11procedure_details\x18\t \x01(\tB\x13\n\x11_is_heterogeneousB\x14\n\x12_forms_precipitateB\x10\n\x0e_is_exothermicB\x0c\n\n_offgassesB\x1b\n\x19_is_sensitive_to_moistureB\x19\n\x17_is_sensitive_to_oxygenB\x18\n\x16_is_sensitive_to_light\"Y\n\x13ReactionObservation\x12\x17\n\x04time\x18\x01 \x01(\x0b\x32\t.ord.Time\x12\x0f\n\x07\x63omment\x18\x02 \x01(\t\x12\x18\n\x05image\x18\x03 \x01(\x0b\x32\t.ord.Data\"\xcb\x05\n\x0eReactionWorkup\x12\x34\n\x04type\x18\x01 \x01(\x0e\x32&.ord.ReactionWorkup.ReactionWorkupType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1b\n\x08\x64uration\x18\x03 \x01(\x0b\x32\t.ord.Time\x12!\n\x05input\x18\x04 \x01(\x0b\x32\x12.ord.ReactionInput\x12\x1b\n\x06\x61mount\x18\x05 \x01(\x0b\x32\x0b.ord.Amount\x12/\n\x0btemperature\x18\x06 \x01(\x0b\x32\x1a.ord.TemperatureConditions\x12\x12\n\nkeep_phase\x18\x07 \x01(\t\x12)\n\x08stirring\x18\x08 \x01(\x0b\x32\x17.ord.StirringConditions\x12\x16\n\ttarget_ph\x18\t \x01(\x02H\x00\x88\x01\x01\x12\x19\n\x0cis_automated\x18\n \x01(\x08H\x01\x88\x01\x01\"\xd2\x02\n\x12ReactionWorkupType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0c\n\x08\x41\x44\x44ITION\x10\x02\x12\x0b\n\x07\x41LIQUOT\x10\x03\x12\x0f\n\x0bTEMPERATURE\x10\x04\x12\x11\n\rCONCENTRATION\x10\x05\x12\x0e\n\nEXTRACTION\x10\x06\x12\x0e\n\nFILTRATION\x10\x07\x12\x08\n\x04WASH\x10\x08\x12\x11\n\rDRY_IN_VACUUM\x10\t\x12\x15\n\x11\x44RY_WITH_MATERIAL\x10\n\x12\x18\n\x14\x46LASH_CHROMATOGRAPHY\x10\x0b\x12\x18\n\x14OTHER_CHROMATOGRAPHY\x10\x0c\x12\x0e\n\nSCAVENGING\x10\r\x12\x08\n\x04WAIT\x10\x0e\x12\x0c\n\x08STIRRING\x10\x0f\x12\r\n\tPH_ADJUST\x10\x10\x12\x0f\n\x0b\x44ISSOLUTION\x10\x11\x12\x10\n\x0c\x44ISTILLATION\x10\x12\x42\x0c\n\n_target_phB\x0f\n\r_is_automated\"\xf6\x01\n\x0fReactionOutcome\x12 \n\rreaction_time\x18\x01 \x01(\x0b\x32\t.ord.Time\x12#\n\nconversion\x18\x02 \x01(\x0b\x32\x0f.ord.Percentage\x12&\n\x08products\x18\x03 \x03(\x0b\x32\x14.ord.ProductCompound\x12\x34\n\x08\x61nalyses\x18\x04 \x03(\x0b\x32\".ord.ReactionOutcome.AnalysesEntry\x1a>\n\rAnalysesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.ord.Analysis:\x02\x38\x01\"\x8d\x05\n\x0fProductCompound\x12,\n\x0bidentifiers\x18\x01 \x03(\x0b\x32\x17.ord.CompoundIdentifier\x12\x1f\n\x12is_desired_product\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12-\n\x0cmeasurements\x18\x03 \x03(\x0b\x32\x17.ord.ProductMeasurement\x12\x16\n\x0eisolated_color\x18\x04 \x01(\t\x12-\n\x07texture\x18\x05 \x01(\x0b\x32\x1c.ord.ProductCompound.Texture\x12\x34\n\x08\x66\x65\x61tures\x18\x06 \x03(\x0b\x32\".ord.ProductCompound.FeaturesEntry\x12\x39\n\rreaction_role\x18\x07 \x01(\x0e\x32\".ord.ReactionRole.ReactionRoleType\x1a\xf0\x01\n\x07Texture\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.ord.ProductCompound.Texture.TextureType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\x9b\x01\n\x0bTextureType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\n\n\x06POWDER\x10\x02\x12\x0b\n\x07\x43RYSTAL\x10\x03\x12\x07\n\x03OIL\x10\x04\x12\x13\n\x0f\x41MORPHOUS_SOLID\x10\x05\x12\x08\n\x04\x46OAM\x10\x06\x12\x07\n\x03WAX\x10\x07\x12\x0e\n\nSEMI_SOLID\x10\x08\x12\t\n\x05SOLID\x10\t\x12\n\n\x06LIQUID\x10\n\x1a:\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x42\x15\n\x13_is_desired_product\"\xfb\n\n\x12ProductMeasurement\x12\x14\n\x0c\x61nalysis_key\x18\x01 \x01(\t\x12<\n\x04type\x18\x02 \x01(\x0e\x32..ord.ProductMeasurement.ProductMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\t\x12#\n\x16uses_internal_standard\x18\x04 \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\ris_normalized\x18\x05 \x01(\x08H\x02\x88\x01\x01\x12$\n\x17uses_authentic_standard\x18\x06 \x01(\x08H\x03\x88\x01\x01\x12)\n\x12\x61uthentic_standard\x18\x07 \x01(\x0b\x32\r.ord.Compound\x12%\n\npercentage\x18\x08 \x01(\x0b\x32\x0f.ord.PercentageH\x00\x12&\n\x0b\x66loat_value\x18\t \x01(\x0b\x32\x0f.ord.FloatValueH\x00\x12\x16\n\x0cstring_value\x18\n \x01(\tH\x00\x12\x1d\n\x06\x61mount\x18\x0b \x01(\x0b\x32\x0b.ord.AmountH\x00\x12!\n\x0eretention_time\x18\x0c \x01(\x0b\x32\t.ord.Time\x12M\n\x11mass_spec_details\x18\r \x01(\x0b\x32\x32.ord.ProductMeasurement.MassSpecMeasurementDetails\x12\x38\n\x0bselectivity\x18\x0e \x01(\x0b\x32#.ord.ProductMeasurement.Selectivity\x12#\n\nwavelength\x18\x0f \x01(\x0b\x32\x0f.ord.Wavelength\x1a\xe9\x02\n\x1aMassSpecMeasurementDetails\x12X\n\x04type\x18\x01 \x01(\x0e\x32J.ord.ProductMeasurement.MassSpecMeasurementDetails.MassSpecMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1b\n\x0etic_minimum_mz\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12\x1b\n\x0etic_maximum_mz\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\neic_masses\x18\x05 \x03(\x02\"l\n\x17MassSpecMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x07\n\x03TIC\x10\x02\x12\x10\n\x0cTIC_POSITIVE\x10\x03\x12\x10\n\x0cTIC_NEGATIVE\x10\x04\x12\x07\n\x03\x45IC\x10\x05\x42\x11\n\x0f_tic_minimum_mzB\x11\n\x0f_tic_maximum_mz\x1a\xb9\x01\n\x0bSelectivity\x12\x41\n\x04type\x18\x01 \x01(\x0e\x32\x33.ord.ProductMeasurement.Selectivity.SelectivityType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"V\n\x0fSelectivityType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x06\n\x02\x45\x45\x10\x02\x12\x06\n\x02\x45R\x10\x03\x12\x06\n\x02\x44R\x10\x04\x12\x06\n\x02\x45Z\x10\x05\x12\x06\n\x02ZE\x10\x06\"\x9c\x01\n\x16ProductMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0c\n\x08IDENTITY\x10\x02\x12\t\n\x05YIELD\x10\x03\x12\x0f\n\x0bSELECTIVITY\x10\x04\x12\n\n\x06PURITY\x10\x05\x12\x08\n\x04\x41REA\x10\x06\x12\n\n\x06\x43OUNTS\x10\x07\x12\r\n\tINTENSITY\x10\x08\x12\n\n\x06\x41MOUNT\x10\tB\x07\n\x05valueB\x19\n\x17_uses_internal_standardB\x10\n\x0e_is_normalizedB\x1a\n\x18_uses_authentic_standard\"\x19\n\x08\x44\x61teTime\x12\r\n\x05value\x18\x01 \x01(\t\"\xcc\x04\n\x08\x41nalysis\x12(\n\x04type\x18\x01 \x01(\x0e\x32\x1a.ord.Analysis.AnalysisType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x0f\n\x07\x63hmo_id\x18\x03 \x01(\x05\x12#\n\x16is_of_isolated_species\x18\x04 \x01(\x08H\x00\x88\x01\x01\x12%\n\x04\x64\x61ta\x18\x05 \x03(\x0b\x32\x17.ord.Analysis.DataEntry\x12\x1f\n\x17instrument_manufacturer\x18\x06 \x01(\t\x12\x31\n\x1ainstrument_last_calibrated\x18\x07 \x01(\x0b\x32\r.ord.DateTime\x1a\x36\n\tDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\"\x80\x02\n\x0c\x41nalysisType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x06\n\x02LC\x10\x02\x12\x06\n\x02GC\x10\x03\x12\x06\n\x02IR\x10\x04\x12\n\n\x06NMR_1H\x10\x05\x12\x0b\n\x07NMR_13C\x10\x06\x12\r\n\tNMR_OTHER\x10\x07\x12\x06\n\x02MP\x10\x08\x12\x06\n\x02UV\x10\t\x12\x07\n\x03TLC\x10\n\x12\x06\n\x02MS\x10\x0b\x12\x08\n\x04HRMS\x10\x0c\x12\x08\n\x04MSMS\x10\r\x12\n\n\x06WEIGHT\x10\x0e\x12\x08\n\x04LCMS\x10\x0f\x12\x08\n\x04GCMS\x10\x10\x12\x08\n\x04\x45LSD\x10\x11\x12\x06\n\x02\x43\x44\x10\x12\x12\x07\n\x03SFC\x10\x13\x12\x07\n\x03\x45PR\x10\x14\x12\x07\n\x03XRD\x10\x15\x12\t\n\x05RAMAN\x10\x16\x12\x06\n\x02\x45\x44\x10\x17\x42\x19\n\x17_is_of_isolated_species\"\x87\x03\n\x12ReactionProvenance\x12!\n\x0c\x65xperimenter\x18\x01 \x01(\x0b\x32\x0b.ord.Person\x12\x0c\n\x04\x63ity\x18\x02 \x01(\t\x12\'\n\x10\x65xperiment_start\x18\x03 \x01(\x0b\x32\r.ord.DateTime\x12\x0b\n\x03\x64oi\x18\x04 \x01(\t\x12\x0e\n\x06patent\x18\x05 \x01(\t\x12\x17\n\x0fpublication_url\x18\x06 \x01(\t\x12(\n\x0erecord_created\x18\x07 \x01(\x0b\x32\x10.ord.RecordEvent\x12)\n\x0frecord_modified\x18\x08 \x03(\x0b\x32\x10.ord.RecordEvent\x12H\n\x11reaction_metadata\x18\t \x03(\x0b\x32-.ord.ReactionProvenance.ReactionMetadataEntry\x1a\x42\n\x15ReactionMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\"\\\n\x06Person\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05orcid\x18\x03 \x01(\t\x12\x14\n\x0corganization\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x01(\t\"X\n\x0bRecordEvent\x12\x1b\n\x04time\x18\x01 \x01(\x0b\x32\r.ord.DateTime\x12\x1b\n\x06person\x18\x02 \x01(\x0b\x32\x0b.ord.Person\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\t\"\xb5\x01\n\x04Time\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12!\n\x05units\x18\x03 \x01(\x0e\x32\x12.ord.Time.TimeUnit\"F\n\x08TimeUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x07\n\x03\x44\x41Y\x10\x04\x12\x08\n\x04HOUR\x10\x01\x12\n\n\x06MINUTE\x10\x02\x12\n\n\x06SECOND\x10\x03\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xc0\x01\n\x04Mass\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12!\n\x05units\x18\x03 \x01(\x0e\x32\x12.ord.Mass.MassUnit\"Q\n\x08MassUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0c\n\x08KILOGRAM\x10\x01\x12\x08\n\x04GRAM\x10\x02\x12\r\n\tMILLIGRAM\x10\x03\x12\r\n\tMICROGRAM\x10\x04\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xc4\x01\n\x05Moles\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12#\n\x05units\x18\x03 \x01(\x0e\x32\x14.ord.Moles.MolesUnit\"R\n\tMolesUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04MOLE\x10\x01\x12\r\n\tMILLIMOLE\x10\x02\x12\r\n\tMICROMOLE\x10\x03\x12\x0c\n\x08NANOMOLE\x10\x04\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xcc\x01\n\x06Volume\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12%\n\x05units\x18\x03 \x01(\x0e\x32\x16.ord.Volume.VolumeUnit\"W\n\nVolumeUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\t\n\x05LITER\x10\x01\x12\x0e\n\nMILLILITER\x10\x02\x12\x0e\n\nMICROLITER\x10\x03\x12\r\n\tNANOLITER\x10\x04\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xd9\x01\n\rConcentration\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x33\n\x05units\x18\x03 \x01(\x0e\x32$.ord.Concentration.ConcentrationUnit\"O\n\x11\x43oncentrationUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\t\n\x05MOLAR\x10\x01\x12\x0e\n\nMILLIMOLAR\x10\x02\x12\x0e\n\nMICROMOLAR\x10\x03\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xf7\x01\n\x08Pressure\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12)\n\x05units\x18\x03 \x01(\x0e\x32\x1a.ord.Pressure.PressureUnit\"|\n\x0cPressureUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x07\n\x03\x42\x41R\x10\x01\x12\x0e\n\nATMOSPHERE\x10\x02\x12\x07\n\x03PSI\x10\x03\x12\x08\n\x04KPSI\x10\x04\x12\n\n\x06PASCAL\x10\x05\x12\x0e\n\nKILOPASCAL\x10\x06\x12\x08\n\x04TORR\x10\x07\x12\t\n\x05MM_HG\x10\x08\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xcf\x01\n\x0bTemperature\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12/\n\x05units\x18\x03 \x01(\x0e\x32 .ord.Temperature.TemperatureUnit\"K\n\x0fTemperatureUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0b\n\x07\x43\x45LSIUS\x10\x01\x12\x0e\n\nFAHRENHEIT\x10\x02\x12\n\n\x06KELVIN\x10\x03\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xb3\x01\n\x07\x43urrent\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\'\n\x05units\x18\x03 \x01(\x0e\x32\x18.ord.Current.CurrentUnit\";\n\x0b\x43urrentUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x41MPERE\x10\x01\x12\x0f\n\x0bMILLIAMPERE\x10\x02\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xaf\x01\n\x07Voltage\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\'\n\x05units\x18\x03 \x01(\x0e\x32\x18.ord.Voltage.VoltageUnit\"7\n\x0bVoltageUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04VOLT\x10\x01\x12\r\n\tMILLIVOLT\x10\x02\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xd1\x01\n\x06Length\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12%\n\x05units\x18\x03 \x01(\x0e\x32\x16.ord.Length.LengthUnit\"\\\n\nLengthUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0e\n\nCENTIMETER\x10\x01\x12\x0e\n\nMILLIMETER\x10\x02\x12\t\n\x05METER\x10\x03\x12\x08\n\x04INCH\x10\x04\x12\x08\n\x04\x46OOT\x10\x05\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xc1\x01\n\nWavelength\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12-\n\x05units\x18\x03 \x01(\x0e\x32\x1e.ord.Wavelength.WavelengthUnit\"@\n\x0eWavelengthUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\r\n\tNANOMETER\x10\x01\x12\x0e\n\nWAVENUMBER\x10\x02\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xa0\x02\n\x08\x46lowRate\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12)\n\x05units\x18\x03 \x01(\x0e\x32\x1a.ord.FlowRate.FlowRateUnit\"\xa4\x01\n\x0c\x46lowRateUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x19\n\x15MICROLITER_PER_MINUTE\x10\x01\x12\x19\n\x15MICROLITER_PER_SECOND\x10\x02\x12\x19\n\x15MILLILITER_PER_MINUTE\x10\x03\x12\x19\n\x15MILLILITER_PER_SECOND\x10\x04\x12\x17\n\x13MICROLITER_PER_HOUR\x10\x05\x42\x08\n\x06_valueB\x0c\n\n_precision\"P\n\nPercentage\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x08\n\x06_valueB\x0c\n\n_precision\"P\n\nFloatValue\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xa1\x01\n\x04\x44\x61ta\x12\x15\n\x0b\x66loat_value\x18\x01 \x01(\x02H\x00\x12\x17\n\rinteger_value\x18\x02 \x01(\x05H\x00\x12\x15\n\x0b\x62ytes_value\x18\x03 \x01(\x0cH\x00\x12\x16\n\x0cstring_value\x18\x04 \x01(\tH\x00\x12\r\n\x03url\x18\x05 \x01(\tH\x00\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x07 \x01(\tB\x06\n\x04kindb\x06proto3')
 
 
 
 _REACTION = DESCRIPTOR.message_types_by_name['Reaction']
 _REACTION_INPUTSENTRY = _REACTION.nested_types_by_name['InputsEntry']
 _REACTIONIDENTIFIER = DESCRIPTOR.message_types_by_name['ReactionIdentifier']
 _REACTIONINPUT = DESCRIPTOR.message_types_by_name['ReactionInput']
@@ -82,14 +82,15 @@
 _PRODUCTMEASUREMENT = DESCRIPTOR.message_types_by_name['ProductMeasurement']
 _PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS = _PRODUCTMEASUREMENT.nested_types_by_name['MassSpecMeasurementDetails']
 _PRODUCTMEASUREMENT_SELECTIVITY = _PRODUCTMEASUREMENT.nested_types_by_name['Selectivity']
 _DATETIME = DESCRIPTOR.message_types_by_name['DateTime']
 _ANALYSIS = DESCRIPTOR.message_types_by_name['Analysis']
 _ANALYSIS_DATAENTRY = _ANALYSIS.nested_types_by_name['DataEntry']
 _REACTIONPROVENANCE = DESCRIPTOR.message_types_by_name['ReactionProvenance']
+_REACTIONPROVENANCE_REACTIONMETADATAENTRY = _REACTIONPROVENANCE.nested_types_by_name['ReactionMetadataEntry']
 _PERSON = DESCRIPTOR.message_types_by_name['Person']
 _RECORDEVENT = DESCRIPTOR.message_types_by_name['RecordEvent']
 _TIME = DESCRIPTOR.message_types_by_name['Time']
 _MASS = DESCRIPTOR.message_types_by_name['Mass']
 _MOLES = DESCRIPTOR.message_types_by_name['Moles']
 _VOLUME = DESCRIPTOR.message_types_by_name['Volume']
 _CONCENTRATION = DESCRIPTOR.message_types_by_name['Concentration']
@@ -536,19 +537,27 @@
   '__module__' : 'ord_schema.proto.reaction_pb2'
   # @@protoc_insertion_point(class_scope:ord.Analysis)
   })
 _sym_db.RegisterMessage(Analysis)
 _sym_db.RegisterMessage(Analysis.DataEntry)
 
 ReactionProvenance = _reflection.GeneratedProtocolMessageType('ReactionProvenance', (_message.Message,), {
+
+  'ReactionMetadataEntry' : _reflection.GeneratedProtocolMessageType('ReactionMetadataEntry', (_message.Message,), {
+    'DESCRIPTOR' : _REACTIONPROVENANCE_REACTIONMETADATAENTRY,
+    '__module__' : 'ord_schema.proto.reaction_pb2'
+    # @@protoc_insertion_point(class_scope:ord.ReactionProvenance.ReactionMetadataEntry)
+    })
+  ,
   'DESCRIPTOR' : _REACTIONPROVENANCE,
   '__module__' : 'ord_schema.proto.reaction_pb2'
   # @@protoc_insertion_point(class_scope:ord.ReactionProvenance)
   })
 _sym_db.RegisterMessage(ReactionProvenance)
+_sym_db.RegisterMessage(ReactionProvenance.ReactionMetadataEntry)
 
 Person = _reflection.GeneratedProtocolMessageType('Person', (_message.Message,), {
   'DESCRIPTOR' : _PERSON,
   '__module__' : 'ord_schema.proto.reaction_pb2'
   # @@protoc_insertion_point(class_scope:ord.Person)
   })
 _sym_db.RegisterMessage(Person)
@@ -678,234 +687,238 @@
   _REACTIONSETUP_AUTOMATIONCODEENTRY._serialized_options = b'8\001'
   _REACTIONOUTCOME_ANALYSESENTRY._options = None
   _REACTIONOUTCOME_ANALYSESENTRY._serialized_options = b'8\001'
   _PRODUCTCOMPOUND_FEATURESENTRY._options = None
   _PRODUCTCOMPOUND_FEATURESENTRY._serialized_options = b'8\001'
   _ANALYSIS_DATAENTRY._options = None
   _ANALYSIS_DATAENTRY._serialized_options = b'8\001'
+  _REACTIONPROVENANCE_REACTIONMETADATAENTRY._options = None
+  _REACTIONPROVENANCE_REACTIONMETADATAENTRY._serialized_options = b'8\001'
   _REACTION._serialized_start=41
   _REACTION._serialized_end=514
   _REACTION_INPUTSENTRY._serialized_start=449
   _REACTION_INPUTSENTRY._serialized_end=514
   _REACTIONIDENTIFIER._serialized_start=517
-  _REACTIONIDENTIFIER._serialized_end=803
+  _REACTIONIDENTIFIER._serialized_end=812
   _REACTIONIDENTIFIER_REACTIONIDENTIFIERTYPE._serialized_start=658
-  _REACTIONIDENTIFIER_REACTIONIDENTIFIERTYPE._serialized_end=789
-  _REACTIONINPUT._serialized_start=806
-  _REACTIONINPUT._serialized_end=1634
-  _REACTIONINPUT_ADDITIONSPEED._serialized_start=1202
-  _REACTIONINPUT_ADDITIONSPEED._serialized_end=1422
-  _REACTIONINPUT_ADDITIONSPEED_ADDITIONSPEEDTYPE._serialized_start=1302
-  _REACTIONINPUT_ADDITIONSPEED_ADDITIONSPEEDTYPE._serialized_end=1422
-  _REACTIONINPUT_ADDITIONDEVICE._serialized_start=1425
-  _REACTIONINPUT_ADDITIONDEVICE._serialized_end=1634
-  _REACTIONINPUT_ADDITIONDEVICE_ADDITIONDEVICETYPE._serialized_start=1528
-  _REACTIONINPUT_ADDITIONDEVICE_ADDITIONDEVICETYPE._serialized_end=1634
-  _AMOUNT._serialized_start=1637
-  _AMOUNT._serialized_end=1851
-  _UNMEASUREDAMOUNT._serialized_start=1854
-  _UNMEASUREDAMOUNT._serialized_end=2044
-  _UNMEASUREDAMOUNT_UNMEASUREDAMOUNTTYPE._serialized_start=1949
-  _UNMEASUREDAMOUNT_UNMEASUREDAMOUNTTYPE._serialized_end=2044
-  _CRUDECOMPONENT._serialized_start=2047
-  _CRUDECOMPONENT._serialized_end=2219
-  _COMPOUND._serialized_start=2222
-  _COMPOUND._serialized_end=2771
-  _COMPOUND_SOURCE._serialized_start=2574
-  _COMPOUND_SOURCE._serialized_end=2631
-  _COMPOUND_FEATURESENTRY._serialized_start=2633
-  _COMPOUND_FEATURESENTRY._serialized_end=2691
-  _COMPOUND_ANALYSESENTRY._serialized_start=2693
-  _COMPOUND_ANALYSESENTRY._serialized_end=2755
-  _REACTIONROLE._serialized_start=2774
-  _REACTIONROLE._serialized_end=2952
-  _REACTIONROLE_REACTIONROLETYPE._serialized_start=2791
-  _REACTIONROLE_REACTIONROLETYPE._serialized_end=2952
-  _COMPOUNDPREPARATION._serialized_start=2955
-  _COMPOUNDPREPARATION._serialized_end=3201
-  _COMPOUNDPREPARATION_COMPOUNDPREPARATIONTYPE._serialized_start=3080
-  _COMPOUNDPREPARATION_COMPOUNDPREPARATIONTYPE._serialized_end=3201
-  _COMPOUNDIDENTIFIER._serialized_start=3204
-  _COMPOUNDIDENTIFIER._serialized_end=3590
-  _COMPOUNDIDENTIFIER_COMPOUNDIDENTIFIERTYPE._serialized_start=3321
-  _COMPOUNDIDENTIFIER_COMPOUNDIDENTIFIERTYPE._serialized_end=3590
-  _VESSEL._serialized_start=3593
-  _VESSEL._serialized_end=4123
-  _VESSEL_VESSELTYPE._serialized_start=3859
-  _VESSEL_VESSELTYPE._serialized_end=4123
-  _VESSELMATERIAL._serialized_start=4126
-  _VESSELMATERIAL._serialized_end=4330
-  _VESSELMATERIAL_VESSELMATERIALTYPE._serialized_start=4215
-  _VESSELMATERIAL_VESSELMATERIALTYPE._serialized_end=4330
-  _VESSELATTACHMENT._serialized_start=4333
-  _VESSELATTACHMENT._serialized_end=4740
-  _VESSELATTACHMENT_VESSELATTACHMENTTYPE._serialized_start=4429
-  _VESSELATTACHMENT_VESSELATTACHMENTTYPE._serialized_end=4740
-  _VESSELPREPARATION._serialized_start=4743
-  _VESSELPREPARATION._serialized_end=4975
-  _VESSELPREPARATION_VESSELPREPARATIONTYPE._serialized_start=4842
-  _VESSELPREPARATION_VESSELPREPARATIONTYPE._serialized_end=4975
-  _REACTIONSETUP._serialized_start=4978
-  _REACTIONSETUP._serialized_end=5522
-  _REACTIONSETUP_AUTOMATIONCODEENTRY._serialized_start=5206
-  _REACTIONSETUP_AUTOMATIONCODEENTRY._serialized_end=5270
-  _REACTIONSETUP_REACTIONENVIRONMENT._serialized_start=5273
-  _REACTIONSETUP_REACTIONENVIRONMENT._serialized_end=5505
-  _REACTIONSETUP_REACTIONENVIRONMENT_REACTIONENVIRONMENTTYPE._serialized_start=5391
-  _REACTIONSETUP_REACTIONENVIRONMENT_REACTIONENVIRONMENTTYPE._serialized_end=5505
-  _REACTIONCONDITIONS._serialized_start=5525
-  _REACTIONCONDITIONS._serialized_end=5962
-  _TEMPERATURECONDITIONS._serialized_start=5965
-  _TEMPERATURECONDITIONS._serialized_end=6831
-  _TEMPERATURECONDITIONS_TEMPERATURECONTROL._serialized_start=6164
-  _TEMPERATURECONDITIONS_TEMPERATURECONTROL._serialized_end=6504
-  _TEMPERATURECONDITIONS_TEMPERATURECONTROL_TEMPERATURECONTROLTYPE._serialized_start=6288
-  _TEMPERATURECONDITIONS_TEMPERATURECONTROL_TEMPERATURECONTROLTYPE._serialized_end=6504
-  _TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT._serialized_start=6507
-  _TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT._serialized_end=6831
-  _TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT_TEMPERATUREMEASUREMENTTYPE._serialized_start=6706
-  _TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT_TEMPERATUREMEASUREMENTTYPE._serialized_end=6831
-  _PRESSURECONDITIONS._serialized_start=6834
-  _PRESSURECONDITIONS._serialized_end=7870
-  _PRESSURECONDITIONS_PRESSURECONTROL._serialized_start=7071
-  _PRESSURECONDITIONS_PRESSURECONTROL._serialized_end=7295
-  _PRESSURECONDITIONS_PRESSURECONTROL_PRESSURECONTROLTYPE._serialized_start=7182
-  _PRESSURECONDITIONS_PRESSURECONTROL_PRESSURECONTROLTYPE._serialized_end=7295
-  _PRESSURECONDITIONS_ATMOSPHERE._serialized_start=7298
-  _PRESSURECONDITIONS_ATMOSPHERE._serialized_end=7607
-  _PRESSURECONDITIONS_ATMOSPHERE_ATMOSPHERETYPE._serialized_start=7395
-  _PRESSURECONDITIONS_ATMOSPHERE_ATMOSPHERETYPE._serialized_end=7607
-  _PRESSURECONDITIONS_PRESSUREMEASUREMENT._serialized_start=7610
-  _PRESSURECONDITIONS_PRESSUREMEASUREMENT._serialized_end=7870
-  _PRESSURECONDITIONS_PRESSUREMEASUREMENT_PRESSUREMEASUREMENTTYPE._serialized_start=7791
-  _PRESSURECONDITIONS_PRESSUREMEASUREMENT_PRESSUREMEASUREMENTTYPE._serialized_end=7870
-  _STIRRINGCONDITIONS._serialized_start=7873
-  _STIRRINGCONDITIONS._serialized_end=8349
-  _STIRRINGCONDITIONS_STIRRINGRATE._serialized_start=8023
-  _STIRRINGCONDITIONS_STIRRINGRATE._serialized_end=8204
-  _STIRRINGCONDITIONS_STIRRINGRATE_STIRRINGRATETYPE._serialized_start=8138
-  _STIRRINGCONDITIONS_STIRRINGRATE_STIRRINGRATETYPE._serialized_end=8204
-  _STIRRINGCONDITIONS_STIRRINGMETHODTYPE._serialized_start=8207
-  _STIRRINGCONDITIONS_STIRRINGMETHODTYPE._serialized_end=8349
-  _ILLUMINATIONCONDITIONS._serialized_start=8352
-  _ILLUMINATIONCONDITIONS._serialized_end=8712
-  _ILLUMINATIONCONDITIONS_ILLUMINATIONTYPE._serialized_start=8554
-  _ILLUMINATIONCONDITIONS_ILLUMINATIONTYPE._serialized_end=8712
-  _ELECTROCHEMISTRYCONDITIONS._serialized_start=8715
-  _ELECTROCHEMISTRYCONDITIONS._serialized_end=9592
-  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYMEASUREMENT._serialized_start=9137
-  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYMEASUREMENT._serialized_end=9265
-  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL._serialized_start=9268
-  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL._serialized_end=9495
-  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL_ELECTROCHEMISTRYCELLTYPE._serialized_start=9402
-  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL_ELECTROCHEMISTRYCELLTYPE._serialized_end=9495
-  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYTYPE._serialized_start=9497
-  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYTYPE._serialized_end=9592
-  _FLOWCONDITIONS._serialized_start=9595
-  _FLOWCONDITIONS._serialized_end=10127
-  _FLOWCONDITIONS_TUBING._serialized_start=9738
-  _FLOWCONDITIONS_TUBING._serialized_end=10002
-  _FLOWCONDITIONS_TUBING_TUBINGTYPE._serialized_start=9850
-  _FLOWCONDITIONS_TUBING_TUBINGTYPE._serialized_end=10002
-  _FLOWCONDITIONS_FLOWTYPE._serialized_start=10004
-  _FLOWCONDITIONS_FLOWTYPE._serialized_end=10127
-  _REACTIONNOTES._serialized_start=10130
-  _REACTIONNOTES._serialized_end=10578
-  _REACTIONOBSERVATION._serialized_start=10580
-  _REACTIONOBSERVATION._serialized_end=10669
-  _REACTIONWORKUP._serialized_start=10672
-  _REACTIONWORKUP._serialized_end=11387
-  _REACTIONWORKUP_REACTIONWORKUPTYPE._serialized_start=11018
-  _REACTIONWORKUP_REACTIONWORKUPTYPE._serialized_end=11356
-  _REACTIONOUTCOME._serialized_start=11390
-  _REACTIONOUTCOME._serialized_end=11636
-  _REACTIONOUTCOME_ANALYSESENTRY._serialized_start=2693
-  _REACTIONOUTCOME_ANALYSESENTRY._serialized_end=2755
-  _PRODUCTCOMPOUND._serialized_start=11639
-  _PRODUCTCOMPOUND._serialized_end=12292
-  _PRODUCTCOMPOUND_TEXTURE._serialized_start=11969
-  _PRODUCTCOMPOUND_TEXTURE._serialized_end=12209
-  _PRODUCTCOMPOUND_TEXTURE_TEXTURETYPE._serialized_start=12054
-  _PRODUCTCOMPOUND_TEXTURE_TEXTURETYPE._serialized_end=12209
-  _PRODUCTCOMPOUND_FEATURESENTRY._serialized_start=2633
-  _PRODUCTCOMPOUND_FEATURESENTRY._serialized_end=2691
-  _PRODUCTMEASUREMENT._serialized_start=12295
-  _PRODUCTMEASUREMENT._serialized_end=13698
-  _PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS._serialized_start=12908
-  _PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS._serialized_end=13269
-  _PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS_MASSSPECMEASUREMENTTYPE._serialized_start=13123
-  _PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS_MASSSPECMEASUREMENTTYPE._serialized_end=13231
-  _PRODUCTMEASUREMENT_SELECTIVITY._serialized_start=13272
-  _PRODUCTMEASUREMENT_SELECTIVITY._serialized_end=13457
-  _PRODUCTMEASUREMENT_SELECTIVITY_SELECTIVITYTYPE._serialized_start=13371
-  _PRODUCTMEASUREMENT_SELECTIVITY_SELECTIVITYTYPE._serialized_end=13457
-  _PRODUCTMEASUREMENT_PRODUCTMEASUREMENTTYPE._serialized_start=13460
-  _PRODUCTMEASUREMENT_PRODUCTMEASUREMENTTYPE._serialized_end=13616
-  _DATETIME._serialized_start=13700
-  _DATETIME._serialized_end=13725
-  _ANALYSIS._serialized_start=13728
-  _ANALYSIS._serialized_end=14316
-  _ANALYSIS_DATAENTRY._serialized_start=13976
-  _ANALYSIS_DATAENTRY._serialized_end=14030
-  _ANALYSIS_ANALYSISTYPE._serialized_start=14033
-  _ANALYSIS_ANALYSISTYPE._serialized_end=14289
-  _REACTIONPROVENANCE._serialized_start=14319
-  _REACTIONPROVENANCE._serialized_end=14568
-  _PERSON._serialized_start=14570
-  _PERSON._serialized_end=14662
-  _RECORDEVENT._serialized_start=14664
-  _RECORDEVENT._serialized_end=14752
-  _TIME._serialized_start=14755
-  _TIME._serialized_end=14936
-  _TIME_TIMEUNIT._serialized_start=14842
-  _TIME_TIMEUNIT._serialized_end=14912
-  _MASS._serialized_start=14939
-  _MASS._serialized_end=15131
-  _MASS_MASSUNIT._serialized_start=15026
-  _MASS_MASSUNIT._serialized_end=15107
-  _MOLES._serialized_start=15134
-  _MOLES._serialized_end=15330
-  _MOLES_MOLESUNIT._serialized_start=15224
-  _MOLES_MOLESUNIT._serialized_end=15306
-  _VOLUME._serialized_start=15333
-  _VOLUME._serialized_end=15537
-  _VOLUME_VOLUMEUNIT._serialized_start=15426
-  _VOLUME_VOLUMEUNIT._serialized_end=15513
-  _CONCENTRATION._serialized_start=15540
-  _CONCENTRATION._serialized_end=15757
-  _CONCENTRATION_CONCENTRATIONUNIT._serialized_start=15654
-  _CONCENTRATION_CONCENTRATIONUNIT._serialized_end=15733
-  _PRESSURE._serialized_start=15760
-  _PRESSURE._serialized_end=16007
-  _PRESSURE_PRESSUREUNIT._serialized_start=15859
-  _PRESSURE_PRESSUREUNIT._serialized_end=15983
-  _TEMPERATURE._serialized_start=16010
-  _TEMPERATURE._serialized_end=16217
-  _TEMPERATURE_TEMPERATUREUNIT._serialized_start=16118
-  _TEMPERATURE_TEMPERATUREUNIT._serialized_end=16193
-  _CURRENT._serialized_start=16220
-  _CURRENT._serialized_end=16399
-  _CURRENT_CURRENTUNIT._serialized_start=16316
-  _CURRENT_CURRENTUNIT._serialized_end=16375
-  _VOLTAGE._serialized_start=16402
-  _VOLTAGE._serialized_end=16577
-  _VOLTAGE_VOLTAGEUNIT._serialized_start=16498
-  _VOLTAGE_VOLTAGEUNIT._serialized_end=16553
-  _LENGTH._serialized_start=16580
-  _LENGTH._serialized_end=16789
-  _LENGTH_LENGTHUNIT._serialized_start=16673
-  _LENGTH_LENGTHUNIT._serialized_end=16765
-  _WAVELENGTH._serialized_start=16792
-  _WAVELENGTH._serialized_end=16985
-  _WAVELENGTH_WAVELENGTHUNIT._serialized_start=16897
-  _WAVELENGTH_WAVELENGTHUNIT._serialized_end=16961
-  _FLOWRATE._serialized_start=16988
-  _FLOWRATE._serialized_end=17276
-  _FLOWRATE_FLOWRATEUNIT._serialized_start=17088
-  _FLOWRATE_FLOWRATEUNIT._serialized_end=17252
-  _PERCENTAGE._serialized_start=17278
-  _PERCENTAGE._serialized_end=17358
-  _FLOATVALUE._serialized_start=17360
-  _FLOATVALUE._serialized_end=17440
-  _DATA._serialized_start=17443
-  _DATA._serialized_end=17604
+  _REACTIONIDENTIFIER_REACTIONIDENTIFIERTYPE._serialized_end=798
+  _REACTIONINPUT._serialized_start=815
+  _REACTIONINPUT._serialized_end=1643
+  _REACTIONINPUT_ADDITIONSPEED._serialized_start=1211
+  _REACTIONINPUT_ADDITIONSPEED._serialized_end=1431
+  _REACTIONINPUT_ADDITIONSPEED_ADDITIONSPEEDTYPE._serialized_start=1311
+  _REACTIONINPUT_ADDITIONSPEED_ADDITIONSPEEDTYPE._serialized_end=1431
+  _REACTIONINPUT_ADDITIONDEVICE._serialized_start=1434
+  _REACTIONINPUT_ADDITIONDEVICE._serialized_end=1643
+  _REACTIONINPUT_ADDITIONDEVICE_ADDITIONDEVICETYPE._serialized_start=1537
+  _REACTIONINPUT_ADDITIONDEVICE_ADDITIONDEVICETYPE._serialized_end=1643
+  _AMOUNT._serialized_start=1646
+  _AMOUNT._serialized_end=1860
+  _UNMEASUREDAMOUNT._serialized_start=1863
+  _UNMEASUREDAMOUNT._serialized_end=2053
+  _UNMEASUREDAMOUNT_UNMEASUREDAMOUNTTYPE._serialized_start=1958
+  _UNMEASUREDAMOUNT_UNMEASUREDAMOUNTTYPE._serialized_end=2053
+  _CRUDECOMPONENT._serialized_start=2056
+  _CRUDECOMPONENT._serialized_end=2228
+  _COMPOUND._serialized_start=2231
+  _COMPOUND._serialized_end=2780
+  _COMPOUND_SOURCE._serialized_start=2583
+  _COMPOUND_SOURCE._serialized_end=2640
+  _COMPOUND_FEATURESENTRY._serialized_start=2642
+  _COMPOUND_FEATURESENTRY._serialized_end=2700
+  _COMPOUND_ANALYSESENTRY._serialized_start=2702
+  _COMPOUND_ANALYSESENTRY._serialized_end=2764
+  _REACTIONROLE._serialized_start=2783
+  _REACTIONROLE._serialized_end=2961
+  _REACTIONROLE_REACTIONROLETYPE._serialized_start=2800
+  _REACTIONROLE_REACTIONROLETYPE._serialized_end=2961
+  _COMPOUNDPREPARATION._serialized_start=2964
+  _COMPOUNDPREPARATION._serialized_end=3210
+  _COMPOUNDPREPARATION_COMPOUNDPREPARATIONTYPE._serialized_start=3089
+  _COMPOUNDPREPARATION_COMPOUNDPREPARATIONTYPE._serialized_end=3210
+  _COMPOUNDIDENTIFIER._serialized_start=3213
+  _COMPOUNDIDENTIFIER._serialized_end=3599
+  _COMPOUNDIDENTIFIER_COMPOUNDIDENTIFIERTYPE._serialized_start=3330
+  _COMPOUNDIDENTIFIER_COMPOUNDIDENTIFIERTYPE._serialized_end=3599
+  _VESSEL._serialized_start=3602
+  _VESSEL._serialized_end=4153
+  _VESSEL_VESSELTYPE._serialized_start=3889
+  _VESSEL_VESSELTYPE._serialized_end=4153
+  _VESSELMATERIAL._serialized_start=4156
+  _VESSELMATERIAL._serialized_end=4360
+  _VESSELMATERIAL_VESSELMATERIALTYPE._serialized_start=4245
+  _VESSELMATERIAL_VESSELMATERIALTYPE._serialized_end=4360
+  _VESSELATTACHMENT._serialized_start=4363
+  _VESSELATTACHMENT._serialized_end=4770
+  _VESSELATTACHMENT_VESSELATTACHMENTTYPE._serialized_start=4459
+  _VESSELATTACHMENT_VESSELATTACHMENTTYPE._serialized_end=4770
+  _VESSELPREPARATION._serialized_start=4773
+  _VESSELPREPARATION._serialized_end=5005
+  _VESSELPREPARATION_VESSELPREPARATIONTYPE._serialized_start=4872
+  _VESSELPREPARATION_VESSELPREPARATIONTYPE._serialized_end=5005
+  _REACTIONSETUP._serialized_start=5008
+  _REACTIONSETUP._serialized_end=5552
+  _REACTIONSETUP_AUTOMATIONCODEENTRY._serialized_start=5236
+  _REACTIONSETUP_AUTOMATIONCODEENTRY._serialized_end=5300
+  _REACTIONSETUP_REACTIONENVIRONMENT._serialized_start=5303
+  _REACTIONSETUP_REACTIONENVIRONMENT._serialized_end=5535
+  _REACTIONSETUP_REACTIONENVIRONMENT_REACTIONENVIRONMENTTYPE._serialized_start=5421
+  _REACTIONSETUP_REACTIONENVIRONMENT_REACTIONENVIRONMENTTYPE._serialized_end=5535
+  _REACTIONCONDITIONS._serialized_start=5555
+  _REACTIONCONDITIONS._serialized_end=5992
+  _TEMPERATURECONDITIONS._serialized_start=5995
+  _TEMPERATURECONDITIONS._serialized_end=6861
+  _TEMPERATURECONDITIONS_TEMPERATURECONTROL._serialized_start=6194
+  _TEMPERATURECONDITIONS_TEMPERATURECONTROL._serialized_end=6534
+  _TEMPERATURECONDITIONS_TEMPERATURECONTROL_TEMPERATURECONTROLTYPE._serialized_start=6318
+  _TEMPERATURECONDITIONS_TEMPERATURECONTROL_TEMPERATURECONTROLTYPE._serialized_end=6534
+  _TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT._serialized_start=6537
+  _TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT._serialized_end=6861
+  _TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT_TEMPERATUREMEASUREMENTTYPE._serialized_start=6736
+  _TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT_TEMPERATUREMEASUREMENTTYPE._serialized_end=6861
+  _PRESSURECONDITIONS._serialized_start=6864
+  _PRESSURECONDITIONS._serialized_end=7900
+  _PRESSURECONDITIONS_PRESSURECONTROL._serialized_start=7101
+  _PRESSURECONDITIONS_PRESSURECONTROL._serialized_end=7325
+  _PRESSURECONDITIONS_PRESSURECONTROL_PRESSURECONTROLTYPE._serialized_start=7212
+  _PRESSURECONDITIONS_PRESSURECONTROL_PRESSURECONTROLTYPE._serialized_end=7325
+  _PRESSURECONDITIONS_ATMOSPHERE._serialized_start=7328
+  _PRESSURECONDITIONS_ATMOSPHERE._serialized_end=7637
+  _PRESSURECONDITIONS_ATMOSPHERE_ATMOSPHERETYPE._serialized_start=7425
+  _PRESSURECONDITIONS_ATMOSPHERE_ATMOSPHERETYPE._serialized_end=7637
+  _PRESSURECONDITIONS_PRESSUREMEASUREMENT._serialized_start=7640
+  _PRESSURECONDITIONS_PRESSUREMEASUREMENT._serialized_end=7900
+  _PRESSURECONDITIONS_PRESSUREMEASUREMENT_PRESSUREMEASUREMENTTYPE._serialized_start=7821
+  _PRESSURECONDITIONS_PRESSUREMEASUREMENT_PRESSUREMEASUREMENTTYPE._serialized_end=7900
+  _STIRRINGCONDITIONS._serialized_start=7903
+  _STIRRINGCONDITIONS._serialized_end=8379
+  _STIRRINGCONDITIONS_STIRRINGRATE._serialized_start=8053
+  _STIRRINGCONDITIONS_STIRRINGRATE._serialized_end=8234
+  _STIRRINGCONDITIONS_STIRRINGRATE_STIRRINGRATETYPE._serialized_start=8168
+  _STIRRINGCONDITIONS_STIRRINGRATE_STIRRINGRATETYPE._serialized_end=8234
+  _STIRRINGCONDITIONS_STIRRINGMETHODTYPE._serialized_start=8237
+  _STIRRINGCONDITIONS_STIRRINGMETHODTYPE._serialized_end=8379
+  _ILLUMINATIONCONDITIONS._serialized_start=8382
+  _ILLUMINATIONCONDITIONS._serialized_end=8742
+  _ILLUMINATIONCONDITIONS_ILLUMINATIONTYPE._serialized_start=8584
+  _ILLUMINATIONCONDITIONS_ILLUMINATIONTYPE._serialized_end=8742
+  _ELECTROCHEMISTRYCONDITIONS._serialized_start=8745
+  _ELECTROCHEMISTRYCONDITIONS._serialized_end=9609
+  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYMEASUREMENT._serialized_start=9166
+  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYMEASUREMENT._serialized_end=9282
+  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL._serialized_start=9285
+  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL._serialized_end=9512
+  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL_ELECTROCHEMISTRYCELLTYPE._serialized_start=9419
+  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL_ELECTROCHEMISTRYCELLTYPE._serialized_end=9512
+  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYTYPE._serialized_start=9514
+  _ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYTYPE._serialized_end=9609
+  _FLOWCONDITIONS._serialized_start=9612
+  _FLOWCONDITIONS._serialized_end=10144
+  _FLOWCONDITIONS_TUBING._serialized_start=9755
+  _FLOWCONDITIONS_TUBING._serialized_end=10019
+  _FLOWCONDITIONS_TUBING_TUBINGTYPE._serialized_start=9867
+  _FLOWCONDITIONS_TUBING_TUBINGTYPE._serialized_end=10019
+  _FLOWCONDITIONS_FLOWTYPE._serialized_start=10021
+  _FLOWCONDITIONS_FLOWTYPE._serialized_end=10144
+  _REACTIONNOTES._serialized_start=10147
+  _REACTIONNOTES._serialized_end=10595
+  _REACTIONOBSERVATION._serialized_start=10597
+  _REACTIONOBSERVATION._serialized_end=10686
+  _REACTIONWORKUP._serialized_start=10689
+  _REACTIONWORKUP._serialized_end=11404
+  _REACTIONWORKUP_REACTIONWORKUPTYPE._serialized_start=11035
+  _REACTIONWORKUP_REACTIONWORKUPTYPE._serialized_end=11373
+  _REACTIONOUTCOME._serialized_start=11407
+  _REACTIONOUTCOME._serialized_end=11653
+  _REACTIONOUTCOME_ANALYSESENTRY._serialized_start=2702
+  _REACTIONOUTCOME_ANALYSESENTRY._serialized_end=2764
+  _PRODUCTCOMPOUND._serialized_start=11656
+  _PRODUCTCOMPOUND._serialized_end=12309
+  _PRODUCTCOMPOUND_TEXTURE._serialized_start=11986
+  _PRODUCTCOMPOUND_TEXTURE._serialized_end=12226
+  _PRODUCTCOMPOUND_TEXTURE_TEXTURETYPE._serialized_start=12071
+  _PRODUCTCOMPOUND_TEXTURE_TEXTURETYPE._serialized_end=12226
+  _PRODUCTCOMPOUND_FEATURESENTRY._serialized_start=2642
+  _PRODUCTCOMPOUND_FEATURESENTRY._serialized_end=2700
+  _PRODUCTMEASUREMENT._serialized_start=12312
+  _PRODUCTMEASUREMENT._serialized_end=13715
+  _PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS._serialized_start=12925
+  _PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS._serialized_end=13286
+  _PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS_MASSSPECMEASUREMENTTYPE._serialized_start=13140
+  _PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS_MASSSPECMEASUREMENTTYPE._serialized_end=13248
+  _PRODUCTMEASUREMENT_SELECTIVITY._serialized_start=13289
+  _PRODUCTMEASUREMENT_SELECTIVITY._serialized_end=13474
+  _PRODUCTMEASUREMENT_SELECTIVITY_SELECTIVITYTYPE._serialized_start=13388
+  _PRODUCTMEASUREMENT_SELECTIVITY_SELECTIVITYTYPE._serialized_end=13474
+  _PRODUCTMEASUREMENT_PRODUCTMEASUREMENTTYPE._serialized_start=13477
+  _PRODUCTMEASUREMENT_PRODUCTMEASUREMENTTYPE._serialized_end=13633
+  _DATETIME._serialized_start=13717
+  _DATETIME._serialized_end=13742
+  _ANALYSIS._serialized_start=13745
+  _ANALYSIS._serialized_end=14333
+  _ANALYSIS_DATAENTRY._serialized_start=13993
+  _ANALYSIS_DATAENTRY._serialized_end=14047
+  _ANALYSIS_ANALYSISTYPE._serialized_start=14050
+  _ANALYSIS_ANALYSISTYPE._serialized_end=14306
+  _REACTIONPROVENANCE._serialized_start=14336
+  _REACTIONPROVENANCE._serialized_end=14727
+  _REACTIONPROVENANCE_REACTIONMETADATAENTRY._serialized_start=14661
+  _REACTIONPROVENANCE_REACTIONMETADATAENTRY._serialized_end=14727
+  _PERSON._serialized_start=14729
+  _PERSON._serialized_end=14821
+  _RECORDEVENT._serialized_start=14823
+  _RECORDEVENT._serialized_end=14911
+  _TIME._serialized_start=14914
+  _TIME._serialized_end=15095
+  _TIME_TIMEUNIT._serialized_start=15001
+  _TIME_TIMEUNIT._serialized_end=15071
+  _MASS._serialized_start=15098
+  _MASS._serialized_end=15290
+  _MASS_MASSUNIT._serialized_start=15185
+  _MASS_MASSUNIT._serialized_end=15266
+  _MOLES._serialized_start=15293
+  _MOLES._serialized_end=15489
+  _MOLES_MOLESUNIT._serialized_start=15383
+  _MOLES_MOLESUNIT._serialized_end=15465
+  _VOLUME._serialized_start=15492
+  _VOLUME._serialized_end=15696
+  _VOLUME_VOLUMEUNIT._serialized_start=15585
+  _VOLUME_VOLUMEUNIT._serialized_end=15672
+  _CONCENTRATION._serialized_start=15699
+  _CONCENTRATION._serialized_end=15916
+  _CONCENTRATION_CONCENTRATIONUNIT._serialized_start=15813
+  _CONCENTRATION_CONCENTRATIONUNIT._serialized_end=15892
+  _PRESSURE._serialized_start=15919
+  _PRESSURE._serialized_end=16166
+  _PRESSURE_PRESSUREUNIT._serialized_start=16018
+  _PRESSURE_PRESSUREUNIT._serialized_end=16142
+  _TEMPERATURE._serialized_start=16169
+  _TEMPERATURE._serialized_end=16376
+  _TEMPERATURE_TEMPERATUREUNIT._serialized_start=16277
+  _TEMPERATURE_TEMPERATUREUNIT._serialized_end=16352
+  _CURRENT._serialized_start=16379
+  _CURRENT._serialized_end=16558
+  _CURRENT_CURRENTUNIT._serialized_start=16475
+  _CURRENT_CURRENTUNIT._serialized_end=16534
+  _VOLTAGE._serialized_start=16561
+  _VOLTAGE._serialized_end=16736
+  _VOLTAGE_VOLTAGEUNIT._serialized_start=16657
+  _VOLTAGE_VOLTAGEUNIT._serialized_end=16712
+  _LENGTH._serialized_start=16739
+  _LENGTH._serialized_end=16948
+  _LENGTH_LENGTHUNIT._serialized_start=16832
+  _LENGTH_LENGTHUNIT._serialized_end=16924
+  _WAVELENGTH._serialized_start=16951
+  _WAVELENGTH._serialized_end=17144
+  _WAVELENGTH_WAVELENGTHUNIT._serialized_start=17056
+  _WAVELENGTH_WAVELENGTHUNIT._serialized_end=17120
+  _FLOWRATE._serialized_start=17147
+  _FLOWRATE._serialized_end=17435
+  _FLOWRATE_FLOWRATEUNIT._serialized_start=17247
+  _FLOWRATE_FLOWRATEUNIT._serialized_end=17411
+  _PERCENTAGE._serialized_start=17437
+  _PERCENTAGE._serialized_end=17517
+  _FLOATVALUE._serialized_start=17519
+  _FLOATVALUE._serialized_end=17599
+  _DATA._serialized_start=17602
+  _DATA._serialized_end=17763
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ord-schema-0.3.47/ord_schema/proto/reaction_pb2_test.py` & `ord-schema-0.3.48/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/proto/test_pb2.py` & `ord-schema-0.3.48/ord_schema/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/resolvers.py` & `ord-schema-0.3.48/ord_schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/resolvers_test.py` & `ord-schema-0.3.48/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/scripts/__init__.py` & `ord-schema-0.3.48/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/scripts/build_dataset.py` & `ord-schema-0.3.48/ord_schema/scripts/build_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/scripts/build_dataset_test.py` & `ord-schema-0.3.48/ord_schema/scripts/build_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/scripts/check_pb.py` & `ord-schema-0.3.48/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/scripts/check_pb_test.py` & `ord-schema-0.3.48/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/scripts/enumerate_dataset.py` & `ord-schema-0.3.48/ord_schema/scripts/enumerate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/scripts/enumerate_dataset_test.py` & `ord-schema-0.3.48/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/scripts/parse_uspto.py` & `ord-schema-0.3.48/ord_schema/scripts/parse_uspto.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/scripts/process_dataset.py` & `ord-schema-0.3.48/ord_schema/scripts/process_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/scripts/process_dataset_test.py` & `ord-schema-0.3.48/ord_schema/scripts/process_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/scripts/validate_dataset.py` & `ord-schema-0.3.48/ord_schema/scripts/validate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/scripts/validate_dataset_test.py` & `ord-schema-0.3.48/ord_schema/scripts/validate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/templating.py` & `ord-schema-0.3.48/ord_schema/templating.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/templating_test.py` & `ord-schema-0.3.48/ord_schema/templating_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/units.py` & `ord-schema-0.3.48/ord_schema/units.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/units_test.py` & `ord-schema-0.3.48/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/updates.py` & `ord-schema-0.3.48/ord_schema/updates.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/updates_test.py` & `ord-schema-0.3.48/ord_schema/updates_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/validations.py` & `ord-schema-0.3.48/ord_schema/validations.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema/validations_test.py` & `ord-schema-0.3.48/ord_schema/validations_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema.egg-info/PKG-INFO` & `ord-schema-0.3.48/ord_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.47
+Version: 0.3.48
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.47/ord_schema.egg-info/SOURCES.txt` & `ord-schema-0.3.48/ord_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/ord_schema.egg-info/requires.txt` & `ord-schema-0.3.48/ord_schema.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.47/setup.py` & `ord-schema-0.3.48/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.47",
+    version="0.3.48",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

