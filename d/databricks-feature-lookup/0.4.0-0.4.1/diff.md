# Comparing `tmp/databricks-feature-lookup-0.4.0.tar.gz` & `tmp/databricks-feature-lookup-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-feature-lookup-0.4.0.tar", last modified: Thu Apr  6 20:47:14 2023, max compression
+gzip compressed data, was "databricks-feature-lookup-0.4.1.tar", last modified: Thu Apr 20 18:14:44 2023, max compression
```

## Comparing `databricks-feature-lookup-0.4.0.tar` & `databricks-feature-lookup-0.4.1.tar`

### file list

```diff
@@ -1,72 +1,76 @@
-drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-04-06 20:47:14.623471 databricks-feature-lookup-0.4.0/
--rw-r--r--   0 victor.sun   (502) staff       (20)     2414 2022-04-15 06:23:53.000000 databricks-feature-lookup-0.4.0/LICENSE.md
--rw-r--r--   0 victor.sun   (502) staff       (20)      426 2022-04-15 06:23:53.000000 databricks-feature-lookup-0.4.0/NOTICE.md
--rw-r--r--   0 victor.sun   (502) staff       (20)     4219 2023-04-06 20:47:14.623304 databricks-feature-lookup-0.4.0/PKG-INFO
--rw-r--r--   0 victor.sun   (502) staff       (20)     3488 2023-04-06 20:47:14.000000 databricks-feature-lookup-0.4.0/README.md
-drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-04-06 20:47:14.597884 databricks-feature-lookup-0.4.0/databricks/
-drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-04-06 20:47:14.599890 databricks-feature-lookup-0.4.0/databricks/_feature_store_pkg_metadata/
--rw-r--r--   0 victor.sun   (502) staff       (20)      166 2022-09-26 23:04:45.000000 databricks-feature-lookup-0.4.0/databricks/_feature_store_pkg_metadata/__init__.py
-drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-04-06 20:47:14.600250 databricks-feature-lookup-0.4.0/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/
--rw-r--r--   0 victor.sun   (502) staff       (20)        0 2022-09-26 23:04:45.000000 databricks-feature-lookup-0.4.0/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/__init__.py
-drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-04-06 20:47:14.601666 databricks-feature-lookup-0.4.0/databricks/feature_store/
--rw-r--r--   0 victor.sun   (502) staff       (20)     1980 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/__init__.py
-drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-04-06 20:47:14.613784 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/
--rw-r--r--   0 victor.sun   (502) staff       (20)        0 2022-09-28 20:02:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/__init__.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     1309 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/_feature_store_object.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     1489 2022-09-28 20:02:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/_proto_enum_entity.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      444 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/cloud.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     3039 2023-04-04 22:12:23.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/column_info.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      913 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/data_type.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     2553 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/feature_column_info.py
--rw-r--r--   0 victor.sun   (502) staff       (20)    19284 2023-04-04 22:12:23.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/feature_spec.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      715 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/feature_spec_constants.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     1055 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/feature_table_info.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     3635 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/feature_tables_for_serving.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      891 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/function_info.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     1978 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/on_demand_column_info.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     6817 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/online_feature_table.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     5484 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/online_store_for_serving.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      489 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/query_mode.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      855 2023-04-04 22:12:23.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/source_data_column_info.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      607 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/entities/store_type.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      139 2023-04-06 20:39:11.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/feature_lookup_version.py
-drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-04-06 20:47:14.615838 databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/
--rw-r--r--   0 victor.sun   (502) staff       (20)      753 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/__init__.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     7740 2023-04-04 23:58:41.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py
--rw-r--r--   0 victor.sun   (502) staff       (20)    21707 2023-04-04 23:58:41.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      923 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/lookup_engine.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     2832 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/lookup_mysql_engine.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     7533 2023-04-04 23:58:41.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/lookup_sql_engine.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     2130 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py
--rw-r--r--   0 victor.sun   (502) staff       (20)    27030 2023-04-04 23:33:14.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/mlflow_model.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     1638 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/mlflow_model_constants.py
--rw-r--r--   0 victor.sun   (502) staff       (20)    10759 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/online_lookup_client.py
-drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-04-06 20:47:14.616924 databricks-feature-lookup-0.4.0/databricks/feature_store/protos/
--rw-r--r--   0 victor.sun   (502) staff       (20)        0 2022-04-15 06:23:53.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/protos/__init__.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     6382 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/protos/feature_spec_pb2.py
--rw-r--r--   0 victor.sun   (502) staff       (20)    20655 2023-04-04 23:58:41.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/protos/feature_store_serving_pb2.py
-drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-04-06 20:47:14.621869 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/
--rw-r--r--   0 victor.sun   (502) staff       (20)        0 2022-09-28 20:02:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/__init__.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     3877 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/converter_utils.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     1736 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/cosmosdb_type_utils.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      949 2022-12-14 01:59:08.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/cosmosdb_utils.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      765 2022-12-14 01:59:08.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/data_type_details_utils.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     1739 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/dynamodb_type_utils.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     4955 2023-03-28 23:36:17.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/dynamodb_utils.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      347 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/feature_serving_patch.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     2302 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/feature_spec_test_utils.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     2631 2023-04-04 23:58:41.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/metrics_utils.py
--rw-r--r--   0 victor.sun   (502) staff       (20)    11749 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/pandas_type_utils.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     8049 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/serving_test_utils.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     1278 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/sql_type_utils.py
--rw-r--r--   0 victor.sun   (502) staff       (20)      318 2022-09-28 20:02:48.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/test_utils_common.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     8595 2022-12-14 01:59:08.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/uc_utils.py
--rw-r--r--   0 victor.sun   (502) staff       (20)     1539 2023-04-04 22:12:23.000000 databricks-feature-lookup-0.4.0/databricks/feature_store/utils/utils_common.py
-drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-04-06 20:47:14.623037 databricks-feature-lookup-0.4.0/databricks_feature_lookup.egg-info/
--rw-r--r--   0 victor.sun   (502) staff       (20)     4219 2023-04-06 20:47:14.000000 databricks-feature-lookup-0.4.0/databricks_feature_lookup.egg-info/PKG-INFO
--rw-r--r--   0 victor.sun   (502) staff       (20)     3014 2023-04-06 20:47:14.000000 databricks-feature-lookup-0.4.0/databricks_feature_lookup.egg-info/SOURCES.txt
--rw-r--r--   0 victor.sun   (502) staff       (20)        1 2023-04-06 20:47:14.000000 databricks-feature-lookup-0.4.0/databricks_feature_lookup.egg-info/dependency_links.txt
--rw-r--r--   0 victor.sun   (502) staff       (20)       94 2023-04-06 20:47:14.000000 databricks-feature-lookup-0.4.0/databricks_feature_lookup.egg-info/requires.txt
--rw-r--r--   0 victor.sun   (502) staff       (20)       11 2023-04-06 20:47:14.000000 databricks-feature-lookup-0.4.0/databricks_feature_lookup.egg-info/top_level.txt
--rw-r--r--   0 victor.sun   (502) staff       (20)       38 2023-04-06 20:47:14.623526 databricks-feature-lookup-0.4.0/setup.cfg
--rw-r--r--   0 victor.sun   (502) staff       (20)     2724 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.4.0/setup.py
+drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:44.009162 databricks-feature-lookup-0.4.1/
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     2414 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/LICENSE.md
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      426 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/NOTICE.md
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     4219 2023-04-20 18:14:44.008973 databricks-feature-lookup-0.4.1/PKG-INFO
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     3488 2023-04-20 18:14:43.000000 databricks-feature-lookup-0.4.1/README.md
+drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:43.981344 databricks-feature-lookup-0.4.1/databricks/
+drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:43.984541 databricks-feature-lookup-0.4.1/databricks/_feature_store_pkg_metadata/
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      166 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/_feature_store_pkg_metadata/__init__.py
+drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:43.984928 databricks-feature-lookup-0.4.1/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)        0 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/__init__.py
+drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:43.987155 databricks-feature-lookup-0.4.1/databricks/feature_store/
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     1980 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/__init__.py
+drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:43.996674 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)        0 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/__init__.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     1309 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/_feature_store_object.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     1489 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/_proto_enum_entity.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      444 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/cloud.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     3039 2023-04-12 14:15:52.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/column_info.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      913 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/data_type.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     2553 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_column_info.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)    19284 2023-04-20 18:13:39.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_spec.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      715 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_spec_constants.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     1055 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_table_info.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     3635 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_tables_for_serving.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      891 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/function_info.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     1978 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/on_demand_column_info.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     6817 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/online_feature_table.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     5484 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/online_store_for_serving.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      489 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/query_mode.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      855 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/source_data_column_info.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      607 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/store_type.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      139 2023-04-20 18:08:03.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/feature_lookup_version.py
+drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:43.999448 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      753 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/__init__.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     7740 2023-04-14 03:58:25.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)    21707 2023-04-14 03:58:25.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      923 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_engine.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     2832 2023-04-20 18:13:39.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_mysql_engine.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     7533 2023-04-14 03:58:25.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_sql_engine.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     2130 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)    27030 2023-04-20 18:13:39.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/mlflow_model.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     1638 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/mlflow_model_constants.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)    10759 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/online_lookup_client.py
+drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:44.000581 databricks-feature-lookup-0.4.1/databricks/feature_store/protos/
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)        0 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/protos/__init__.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     6382 2023-04-20 18:14:29.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/protos/feature_spec_pb2.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)    20655 2023-04-20 18:14:29.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/protos/feature_store_serving_pb2.py
+drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:44.006364 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)        0 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/__init__.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     3871 2023-04-20 18:08:03.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/converter_utils.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     1736 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/cosmosdb_type_utils.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      949 2023-04-20 01:23:16.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/cosmosdb_utils.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      765 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/data_type_details_utils.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     1739 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/dynamodb_type_utils.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     4955 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/dynamodb_utils.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      347 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/feature_serving_patch.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     2302 2023-04-20 18:08:03.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/feature_spec_test_utils.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     2631 2023-04-14 03:58:25.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/metrics_utils.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)    11749 2023-04-20 18:13:39.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/pandas_type_utils.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     8049 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/serving_test_utils.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     1278 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/sql_type_utils.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      318 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/test_utils_common.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     8595 2023-04-20 18:08:03.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/uc_utils.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     1539 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/utils_common.py
+drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:44.007946 databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     4219 2023-04-20 18:14:43.000000 databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/PKG-INFO
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     3113 2023-04-20 18:14:43.000000 databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/SOURCES.txt
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)        1 2023-04-20 18:14:43.000000 databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/dependency_links.txt
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)       94 2023-04-20 18:14:43.000000 databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/requires.txt
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)       11 2023-04-20 18:14:43.000000 databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/top_level.txt
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)       38 2023-04-20 18:14:44.009214 databricks-feature-lookup-0.4.1/setup.cfg
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     2724 2023-04-20 18:13:39.000000 databricks-feature-lookup-0.4.1/setup.py
+drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:44.008686 databricks-feature-lookup-0.4.1/tests/
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)    65035 2023-04-20 18:13:39.000000 databricks-feature-lookup-0.4.1/tests/test_mlflow_model.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)      369 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/tests/test_mlflow_model_constants.py
+-rw-r--r--   0 aakrati.talati   (502) staff       (20)     8686 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/tests/test_online_lookup_client.py
```

### Comparing `databricks-feature-lookup-0.4.0/LICENSE.md` & `databricks-feature-lookup-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/PKG-INFO` & `databricks-feature-lookup-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-feature-lookup
-Version: 0.4.0
+Version: 0.4.1
 Summary: Databricks Feature Store Feature Lookup Client
 Author: Databricks
 Author-email: feedback@databricks.com
 License: Databricks Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `databricks-feature-lookup-0.4.0/README.md` & `databricks-feature-lookup-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/__init__.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/_feature_store_object.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/_feature_store_object.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/_proto_enum_entity.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/_proto_enum_entity.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/column_info.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/data_type.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/data_type.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/feature_column_info.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/feature_spec.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_spec.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/feature_spec_constants.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_spec_constants.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/feature_table_info.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_table_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/feature_tables_for_serving.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_tables_for_serving.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/function_info.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/function_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/on_demand_column_info.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/on_demand_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/online_feature_table.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/online_feature_table.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/online_store_for_serving.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/online_store_for_serving.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/source_data_column_info.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/source_data_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/entities/store_type.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/store_type.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/__init__.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/lookup_engine.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/lookup_mysql_engine.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_mysql_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/lookup_sql_engine.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_sql_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/mlflow_model.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/mlflow_model.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/mlflow_model_constants.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/mlflow_model_constants.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/online_lookup_client.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/online_lookup_client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/protos/feature_spec_pb2.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/protos/feature_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/protos/feature_store_serving_pb2.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/protos/feature_store_serving_pb2.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/converter_utils.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/converter_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 
     TODO (ML-20967): Determine what represents a empty value in online lookup and update this decorator.
     """
 
     def inner(value):
         """
         We currently use np.nan to represent missing values from the online store.
-        np.nan is a np.float type and can't be coerced to a np.int16/32/64.
+        np.nan is a float type and can't be coerced to a np.int16/32/64.
         """
-        if isinstance(value, np.float) and np.isnan(value):
+        if isinstance(value, float) and np.isnan(value):
             return np.nan
         return converter(value)
 
     return inner
 
 
 class ConverterFactory:
```

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/cosmosdb_type_utils.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/cosmosdb_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/cosmosdb_utils.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/cosmosdb_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/data_type_details_utils.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/data_type_details_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/dynamodb_type_utils.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/dynamodb_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/dynamodb_utils.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/dynamodb_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/feature_spec_test_utils.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/feature_spec_test_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/metrics_utils.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/pandas_type_utils.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/pandas_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/serving_test_utils.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/serving_test_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/sql_type_utils.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/sql_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/uc_utils.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/uc_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks/feature_store/utils/utils_common.py` & `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/utils_common.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.0/databricks_feature_lookup.egg-info/PKG-INFO` & `databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-feature-lookup
-Version: 0.4.0
+Version: 0.4.1
 Summary: Databricks Feature Store Feature Lookup Client
 Author: Databricks
 Author-email: feedback@databricks.com
 License: Databricks Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `databricks-feature-lookup-0.4.0/databricks_feature_lookup.egg-info/SOURCES.txt` & `databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -53,8 +53,11 @@
 databricks/feature_store/utils/test_utils_common.py
 databricks/feature_store/utils/uc_utils.py
 databricks/feature_store/utils/utils_common.py
 databricks_feature_lookup.egg-info/PKG-INFO
 databricks_feature_lookup.egg-info/SOURCES.txt
 databricks_feature_lookup.egg-info/dependency_links.txt
 databricks_feature_lookup.egg-info/requires.txt
-databricks_feature_lookup.egg-info/top_level.txt
+databricks_feature_lookup.egg-info/top_level.txt
+tests/test_mlflow_model.py
+tests/test_mlflow_model_constants.py
+tests/test_online_lookup_client.py
```

### Comparing `databricks-feature-lookup-0.4.0/setup.py` & `databricks-feature-lookup-0.4.1/setup.py`

 * *Files identical despite different names*

