# Comparing `tmp/hstestaq-0.1.9.tar.gz` & `tmp/hstestaq-0.2.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstestaq-0.1.9.tar", last modified: Sat Jan 21 06:15:51 2023, max compression
+gzip compressed data, was "hstestaq-0.2.11.tar", last modified: Thu Apr 20 19:16:59 2023, max compression
```

## Comparing `hstestaq-0.1.9.tar` & `hstestaq-0.2.11.tar`

### file list

```diff
@@ -1,120 +1,129 @@
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.106713 hstestaq-0.1.9/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       24 2022-08-04 23:41:01.000000 hstestaq-0.1.9/MANIFEST.in
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5980 2023-01-21 06:15:51.106409 hstestaq-0.1.9/PKG-INFO
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.061982 hstestaq-0.1.9/aqueduct_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.062240 hstestaq-0.1.9/aqueduct_executor/migrators/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/migrators/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.064037 hstestaq-0.1.9/aqueduct_executor/migrators/artifact_migration_000016/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     4538 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/migrators/artifact_migration_000016/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      441 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/migrators/artifact_migration_000016/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      455 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/migrators/artifact_migration_000016/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.066505 hstestaq-0.1.9/aqueduct_executor/migrators/backfill_python_type_000022/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      566 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      445 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/migrators/backfill_python_type_000022/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2698 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      437 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.068509 hstestaq-0.1.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1039 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      598 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     4168 2022-11-11 00:14:28.000000 hstestaq-0.1.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      398 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.068892 hstestaq-0.1.9/aqueduct_executor/operators/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.070355 hstestaq-0.1.9/aqueduct_executor/operators/airflow/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/airflow/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3010 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/operators/airflow/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      405 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/airflow/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1122 2022-09-23 18:28:31.000000 hstestaq-0.1.9/aqueduct_executor/operators/airflow/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.071236 hstestaq-0.1.9/aqueduct_executor/operators/connectors/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/__init__.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.084534 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2677 2022-11-11 00:14:28.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/athena.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      134 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/azure_sql.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3297 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/bigquery.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      694 2022-11-11 00:14:28.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/common.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2666 2023-01-21 04:27:50.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/config.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1829 2022-11-11 00:14:28.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/connector.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)    13199 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)    13241 2023-01-21 04:27:50.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/execute_spark.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     6205 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/extract.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1462 2022-11-11 00:14:28.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/gcs.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      650 2022-09-08 13:08:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/load.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      421 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      119 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/maria_db.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      825 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/models.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3821 2022-11-11 00:14:28.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/mongodb.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      798 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/mysql.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1099 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/postgres.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      129 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/redshift.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3010 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/relational.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)    10236 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/s3.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      876 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/snowflake.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5675 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/spec.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1722 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/sql_server.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2434 2022-11-11 00:14:28.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/sqlite.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2728 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.089753 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2349 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/conf.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      254 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/conftest.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1909 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_bigquery.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1169 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_mariadb.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1149 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_mysql.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_postgres.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_redshift.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1185 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_snowflake.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1173 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_sql_server.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1150 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_sqlite.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      925 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.093490 hstestaq-0.1.9/aqueduct_executor/operators/function_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/function_executor/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)    13692 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/operators/function_executor/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2630 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/operators/function_executor/extract_function.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      801 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/function_executor/get_extract_path.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3126 2022-11-18 21:59:12.000000 hstestaq-0.1.9/aqueduct_executor/operators/function_executor/install_requirements.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      425 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/function_executor/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1280 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/function_executor/set_conda_version.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1471 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/operators/function_executor/spec.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       14 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/function_executor/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.095235 hstestaq-0.1.9/aqueduct_executor/operators/param_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/param_executor/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     3211 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/operators/param_executor/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      419 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/param_executor/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      885 2022-09-21 17:33:03.000000 hstestaq-0.1.9/aqueduct_executor/operators/param_executor/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.096853 hstestaq-0.1.9/aqueduct_executor/operators/system_metric_executor/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/system_metric_executor/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2264 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/operators/system_metric_executor/execute.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      435 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/system_metric_executor/main.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      837 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/system_metric_executor/spec.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.100155 hstestaq-0.1.9/aqueduct_executor/operators/utils/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2019 2023-01-21 04:27:33.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/enums.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      345 2022-11-11 00:14:28.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/exceptions.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     7496 2022-11-11 00:14:28.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/execution.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      251 2022-08-23 23:45:17.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/saved_object_delete.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.103818 hstestaq-0.1.9/aqueduct_executor/operators/utils/storage/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/storage/__init__.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      787 2022-09-06 16:45:31.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/storage/config.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      771 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/storage/file.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     1136 2022-08-25 18:47:36.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/storage/gcs.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      720 2022-09-13 18:25:00.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/storage/parse.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     2425 2022-09-13 18:25:00.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/storage/s3.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      214 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/storage/storage.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      819 2022-08-04 23:41:01.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/timer.py
--rw-r--r--   0 harisubbaraj   (501) staff       (20)    11898 2023-01-21 04:27:50.000000 hstestaq-0.1.9/aqueduct_executor/operators/utils/utils.py
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.104173 hstestaq-0.1.9/bin/
--rwxr-xr-x   0 harisubbaraj   (501) staff       (20)    26230 2023-01-21 04:27:50.000000 hstestaq-0.1.9/bin/aqueduct
-drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-01-21 06:15:51.106090 hstestaq-0.1.9/hstestaq.egg-info/
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5980 2023-01-21 06:15:51.000000 hstestaq-0.1.9/hstestaq.egg-info/PKG-INFO
--rw-r--r--   0 harisubbaraj   (501) staff       (20)     5337 2023-01-21 06:15:51.000000 hstestaq-0.1.9/hstestaq.egg-info/SOURCES.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)        1 2023-01-21 06:15:51.000000 hstestaq-0.1.9/hstestaq.egg-info/dependency_links.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      156 2023-01-21 06:15:51.000000 hstestaq-0.1.9/hstestaq.egg-info/requires.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       18 2023-01-21 06:15:51.000000 hstestaq-0.1.9/hstestaq.egg-info/top_level.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      156 2023-01-21 04:27:50.000000 hstestaq-0.1.9/requirements.txt
--rw-r--r--   0 harisubbaraj   (501) staff       (20)       38 2023-01-21 06:15:51.106792 hstestaq-0.1.9/setup.cfg
--rw-r--r--   0 harisubbaraj   (501) staff       (20)      804 2023-01-21 06:15:42.000000 hstestaq-0.1.9/setup.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.236527 hstestaq-0.2.11/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       24 2023-01-27 20:50:40.000000 hstestaq-0.2.11/MANIFEST.in
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 19:16:59.236279 hstestaq-0.2.11/PKG-INFO
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.193970 hstestaq-0.2.11/aqueduct_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.194280 hstestaq-0.2.11/aqueduct_executor/migrators/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.196318 hstestaq-0.2.11/aqueduct_executor/migrators/artifact_migration_000016/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4538 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/migrators/artifact_migration_000016/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      441 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/artifact_migration_000016/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      455 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/artifact_migration_000016/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.198401 hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      566 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      445 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2698 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      437 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.200689 hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1039 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      598 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4168 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      398 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.201014 hstestaq-0.2.11/aqueduct_executor/operators/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.202078 hstestaq-0.2.11/aqueduct_executor/operators/airflow/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/airflow/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3010 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/airflow/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      405 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/airflow/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1122 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/airflow/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.202411 hstestaq-0.2.11/aqueduct_executor/operators/connectors/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/__init__.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.214595 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2680 2023-02-07 17:55:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/athena.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      134 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/azure_sql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3297 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/bigquery.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      694 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/common.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2892 2023-04-12 05:14:24.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1829 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/connector.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    12911 2023-04-18 17:47:10.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     6060 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/extract.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1462 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/gcs.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      650 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/load.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      576 2023-02-21 20:43:25.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      119 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/maria_db.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      825 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/models.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3821 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/mongodb.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      798 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/mysql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1099 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/postgres.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      129 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/redshift.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     4774 2023-03-20 22:51:19.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/relational.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     8690 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     6878 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/s3_serialization.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1808 2023-03-13 17:44:55.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/snowflake.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.215750 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spark/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spark/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5385 2023-02-07 17:55:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spark/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2833 2023-03-13 17:44:55.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spark/snowflake.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5473 2023-04-03 17:36:30.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spec.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1722 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/sql_server.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2434 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/sqlite.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2728 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.220148 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2349 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/conf.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      254 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/conftest.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1909 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_bigquery.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1169 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_mariadb.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1149 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_mysql.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_postgres.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1176 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_redshift.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1185 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_snowflake.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1173 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_sql_server.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1150 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_sqlite.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      925 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.223703 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)    15880 2023-04-20 19:11:46.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2770 2023-02-21 20:43:25.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/extract_function.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      801 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/get_extract_path.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3286 2023-02-21 20:43:25.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/install_requirements.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      594 2023-02-21 20:43:25.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1280 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/set_conda_version.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1471 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/spec.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       14 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/function_executor/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.225061 hstestaq-0.2.11/aqueduct_executor/operators/param_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/param_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3211 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/operators/param_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      419 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/param_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      885 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/param_executor/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.226429 hstestaq-0.2.11/aqueduct_executor/operators/spark/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-30 19:20:10.000000 hstestaq-0.2.11/aqueduct_executor/operators/spark/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     8793 2023-04-03 17:36:30.000000 hstestaq-0.2.11/aqueduct_executor/operators/spark/execute_data.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      979 2023-04-20 19:11:46.000000 hstestaq-0.2.11/aqueduct_executor/operators/spark/execute_function.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5401 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/operators/spark/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.227879 hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2264 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/execute.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      435 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/main.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      837 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/spec.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.230587 hstestaq-0.2.11/aqueduct_executor/operators/utils/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     2259 2023-02-21 20:43:25.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/enums.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      465 2023-01-30 19:20:10.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/exceptions.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7531 2023-04-12 05:14:24.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/execution.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      251 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/saved_object_delete.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.234263 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        0 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/__init__.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      914 2023-04-12 05:14:24.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/config.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      948 2023-02-10 20:54:54.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/file.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     1354 2023-02-10 20:54:54.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/gcs.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      720 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/parse.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     3780 2023-04-12 05:14:24.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/s3.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      288 2023-02-10 20:54:54.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/storage.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      819 2023-01-27 20:50:40.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/timer.py
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     9254 2023-04-20 19:10:16.000000 hstestaq-0.2.11/aqueduct_executor/operators/utils/utils.py
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.234615 hstestaq-0.2.11/bin/
+-rwxr-xr-x   0 harisubbaraj   (501) staff       (20)    29291 2023-04-20 19:11:46.000000 hstestaq-0.2.11/bin/aqueduct
+drwxr-xr-x   0 harisubbaraj   (501) staff       (20)        0 2023-04-20 19:16:59.235962 hstestaq-0.2.11/hstestaq.egg-info/
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     7514 2023-04-20 19:16:59.000000 hstestaq-0.2.11/hstestaq.egg-info/PKG-INFO
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)     5714 2023-04-20 19:16:59.000000 hstestaq-0.2.11/hstestaq.egg-info/SOURCES.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)        1 2023-04-20 19:16:59.000000 hstestaq-0.2.11/hstestaq.egg-info/dependency_links.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 19:16:59.000000 hstestaq-0.2.11/hstestaq.egg-info/requires.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       18 2023-04-20 19:16:59.000000 hstestaq-0.2.11/hstestaq.egg-info/top_level.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      249 2023-04-20 19:10:16.000000 hstestaq-0.2.11/requirements.txt
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)       38 2023-04-20 19:16:59.236605 hstestaq-0.2.11/setup.cfg
+-rw-r--r--   0 harisubbaraj   (501) staff       (20)      805 2023-04-20 19:16:47.000000 hstestaq-0.2.11/setup.py
```

### Comparing `hstestaq-0.1.9/PKG-INFO` & `hstestaq-0.2.11/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,94 @@
 Metadata-Version: 2.1
 Name: hstestaq
-Version: 0.1.9
+Version: 0.2.11
 Summary: Prediction Infrastructure for Data Scientists
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-[<img src="https://aqueduct-public-assets-bucket.s3.us-east-2.amazonaws.com/webapp/logos/aqueduct-logo-two-tone/1x/aqueduct-logo-two-tone-1x.png" width= "35%" />](https://www.aqueducthq.com)
 
-## Aqueduct: Orchestrate & manage production ML
 
+<div align="center">
+  <a href="https://aqueducthq.com">
+    <img src="https://aqueduct-public-assets-bucket.s3.us-east-2.amazonaws.com/webapp/logos/aqueduct-logo-two-tone/1x/aqueduct-logo-two-tone-1x.png" width= "40%" />
+  </a>
+  
+  <h2 style="border: none;">The control center for ML in the cloud</h2>
+
+### 📢 [Slack](https://slack.aqueducthq.com)&nbsp;&nbsp;|&nbsp;&nbsp;🗺️ [Roadmap](https://roadmap.aqueducthq.com)&nbsp;&nbsp;|&nbsp;&nbsp;🐞 [Report a bug](https://github.com/aqueducthq/aqueduct/issues/new?assignees=&labels=bug&template=bug_report.md&title=%5BBUG%5D)&nbsp;&nbsp;|&nbsp;&nbsp;✍️ [Blog](https://blog.aqueducthq.com)
+
+  
+  [![Start Sandbox](https://img.shields.io/static/v1?label=%20&logo=github&message=Start%20Sandbox&color=black)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=496844646)
 [![Downloads](https://pepy.tech/badge/aqueduct-ml/month)](https://pypi.org/project/aqueduct-ml/)
 [![Slack](https://img.shields.io/static/v1.svg?label=chat&message=on%20slack&color=27b1ff&style=flat)](https://join.slack.com/t/aqueductusers/shared_invite/zt-11hby91cx-cpmgfK0qfXqEYXv25hqD6A)
 [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/aqueducthq/aqueduct/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/aqueduct-ml.svg)](https://pypi.org/project/aqueduct-ml/)
 [![Tests](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml)
+</div>
+
+<h1></h1>
 
-**Aqueduct enables you to define, deploy and monitor robust ML pipelines on any cloud infrastructure.** Check out our [quickstart guide](https://docs.aqueducthq.com/quickstart-guide)!
+**Aqueduct enables you to easily define, run, and manage AI & ML tasks on any cloud infrastructure. [Check out our quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
-Aqueduct gives you a simple Python-native API to define machine learning pipelines, the ability to deploy those pipelines on your existing infrastructure (e.g., Spark, Kubernetes, Lambda), and visibility into the code, data, and metadata associated with your workflows. 
-Aqueduct is fully open-source and runs securely in your cloud.
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/867892/230214641-b0aec53b-4988-4581-84ed-134f97ed9276.png" width="80%" />
+</p>
+
+Aqueduct is an open-source MLOps framework that allows you to write code in vanilla Python, run that code on any cloud infrastructure you'd like to use, and gain visibility into the execution and performance of your models and predictions. **[See what infrastructure Aqueduct works with. →](https://aqueducthq.com/integrations/)**
+
+Here's how you can get started: 
 
-You can install Aqueduct via `pip`:
 ```bash
 pip3 install aqueduct-ml
 aqueduct start
 ```
 
-Now, we can create our first workflow:
-
-```python
-from aqueduct import Client, op, metric
-
-client = Client()
-
-@op
-def transform_data(reviews):
-    reviews['strlen'] = reviews['review'].str.len()
-    return reviews
+### How it works
 
+Aqueduct's Python native API allows you to define ML tasks in regular Python code. You can connect Aqueduct to your existing cloud infrastructure ([docs](https://docs.aqueducthq.com/integrations)), and Aqueduct will seamlessly move your code from your laptop to the cloud or between different cloud infrastructure layers. 
 
-demo_db = client.integration("aqueduct_demo")
-reviews_table = demo_db.sql("select * from hotel_reviews;")
+<!--- TODO(vikram): Modify this once we add support for switching into/out of Databricks in a single workflow. --->
+For example, we can define a pipeline that trains a model on Kubernetes using a GPU and validates that model in AWS Lambda in a few lines of Python: 
 
-strlen_table = transform_data(reviews_table)
-strlen_table.save(demo_db.config(table="strlen_table", update_mode="replace")) 
+```python
+@op(
+  engine='eks-us-east-2', 
+  resources={'gpu_resource_name': 'nvidia.com/gpu'}
+)
+def train(features):
+  return model.train(features)
+
+@metric(engine='lambda-us-east-2')
+def validate(model):
+    return validation_test(model)
 
-client.publish_flow(name="review_strlen", artifacts=[strlen_table])
+validate(train(features))
 ```
 
-Once we've created a workflow, we can view that workflow in the Aqueduct UI: 
+Once you publish this workflow to Aqueduct, you can see it on the UI: 
+
+![image](https://user-images.githubusercontent.com/867892/228295996-4ba3de23-3106-431d-93a9-afd8d77a707b.png)
 
-![image](https://user-images.githubusercontent.com/867892/196529730-3c9582d5-8692-495d-a7df-8eb62ddf305f.png)
+To see how to build your first workflow, check out our **[quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
 ## Why Aqueduct?
 
-The engineering required to get data science & machine learning projects in production slows down data teams. Aqueduct automates away that engineering and allows you to define robust data & ML pipelines in a few lines of code and run them anywhere.
+MLOps has become a [tangled mess of siloed infrastructure](https://aqueducthq.com/post/the-mlops-knot/). Most teams need to set up and operate many different cloud infrastructure tools to run ML effectively, but these tools have disparate APIs and interoperate poorly.
+
+Aqueduct provides a single interface to running machine learning tasks on your existing cloud infrastructure — Kubernetes, Spark, Lambda, etc. From the same Python API, you can run code across any or all of these systems seamlessly and gain visibility into how your code is performing.
 
 * **Python-native pipeline API**: Aqueduct’s API allows you define your workflows in vanilla Python, so you can get code into production quickly and effectively. No more DSLs or YAML configs to worry about.
 * **Integrated with your infrastructure**: Workflows defined in Aqueduct can run on any cloud infrastructure you use, like Kubernetes, Spark, Airflow, or AWS Lambda. You can get all the benefits of Aqueduct without having to rip-and-replace your existing tooling.
 * **Centralized visibility into code, data, & metadata**: Once your workflows are in production, you need to know what’s running, whether it’s working, and when it breaks. Aqueduct gives you visibility into what code, data, metrics, and metadata are generated by each workflow run, so you can have confidence that your pipelines work as expected — and know immediately when they don’t.
-* **Runs securely in your cloud**: Aqueduct is fully open-source and runs in any Unix environment. It runs entirely in your cloud and on your infrastructure, so you can be confident that nothing is ever leaving your cloud.
+* **Runs securely in your cloud**: Aqueduct is fully open-source and runs in any Unix environment. It runs entirely in your cloud and on your infrastructure, so you can be confident that your data and code are secure.
 
 ## Overview & Examples
 
 The core abstraction in Aqueduct is a [Workflow](https://docs.aqueducthq.com/workflows), which is a sequence of [Artifacts](https://docs.aqueducthq.com/artifacts) (data) that are transformed by [Operators](https://docs.aqueducthq.com/operators) (compute). 
 The input Artifact(s) for a Workflow is typically loaded from a database, and the output Artifact(s) are typically persisted back to a database. 
 Each Workflow can either be run on a fixed schedule or triggered on-demand.
 
@@ -87,8 +107,8 @@
 * and more details on [creating workflows](https://docs.aqueducthq.com/workflows)
 
 If you have questions or comments or would like to learn more about what we're
 building, please [reach out](mailto:hello@aqueducthq.com), [join our Slack
 channel](https://join.slack.com/t/aqueductusers/shared_invite/zt-11hby91cx-cpmgfK0qfXqEYXv25hqD6A), or [start a conversation on GitHub](https://github.com/aqueducthq/aqueduct/issues/new).
 We'd love to hear from you!
 
-If you're interested in contributing, please check out our [roadmap](https://github.com/aqueducthq/aqueduct/wiki/Aqueduct-Roadmap) and join the development channel in [our community Slack](https://slack.aqueducthq.com).
+If you're interested in contributing, please check out our [roadmap](https://roadmap.aqueducthq.com) and join the development channel in [our community Slack](https://slack.aqueducthq.com).
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/migrators/artifact_migration_000016/execute.py` & `hstestaq-0.2.11/aqueduct_executor/migrators/artifact_migration_000016/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/migrators/backfill_python_type_000022/execute.py` & `hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py` & `hstestaq-0.2.11/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py` & `hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py` & `hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py` & `hstestaq-0.2.11/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/airflow/execute.py` & `hstestaq-0.2.11/aqueduct_executor/operators/airflow/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/airflow/spec.py` & `hstestaq-0.2.11/aqueduct_executor/operators/airflow/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/athena.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/athena.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def discover(self) -> List[str]:
         return self._list_tables()
 
     def extract(self, params: extract.RelationalParams) -> pd.DataFrame:
         assert params.usable(), "Query is not usable. Did you forget to expand placeholders?"
         if params.query == LIST_TABLES_QUERY_ATHENA:
-            return pd.DataFrame(self._list_tables(), columns=["Tables"])
+            return pd.DataFrame(self._list_tables(), columns=["tablename"])
         else:
             return wr.athena.read_sql_query(
                 sql=params.query,
                 database=self.database,
                 boto3_session=self.session,
                 # Disabling ctas improves generality at the cost of performance.
                 # More details here: https://aws-sdk-pandas.readthedocs.io/en/stable/stubs/awswrangler.athena.read_sql_query.html
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/bigquery.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/common.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/common.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/config.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from enum import Enum
 from typing import Optional, Union
 
 from aqueduct_executor.operators.connectors.data import models
 from aqueduct_executor.operators.utils.enums import MetaEnum
 from pydantic import Field
 
+"""Duplicated at `aqueduct/integrations/connect_config.py` for now, please keep them in sync."""
+
 
 class BigQueryConfig(models.BaseConfig):
     project_id: str
     service_account_credentials: str
 
 
 class MySqlConfig(models.BaseConfig):
@@ -48,16 +50,19 @@
 
     # Config credentials
     config_file_path: str = ""
     config_file_content: str = ""
     config_file_profile: str = ""
 
     bucket: str = ""
-
     region: str = ""
+
+    # This is unused for data integrations. It is only used for storage.
+    root_dir: str = ""
+
     use_as_storage: str = ""
 
 
 class AthenaConfig(models.BaseConfig):
     # default type to ACCESS_KEY mainly for backward compatibility
     type: AWSCredentialType = AWSCredentialType.ACCESS_KEY
 
@@ -84,14 +89,15 @@
 class SnowflakeConfig(models.BaseConfig):
     username: str
     password: str
     account_identifier: str
     database: str
     warehouse: str
     db_schema: Optional[str] = Field("public", alias="schema")  # schema is a Pydantic keyword
+    role: Optional[str] = None
 
     class Config:
         # Ensures that Pydantic parses JSON keys named "schema" or "db_schema" to
         # the `db_schema` field
         allow_population_by_field_name = True
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/connector.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/connector.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/execute.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import platform
 import sys
 from typing import Any
 
 from aqueduct_executor.operators.connectors.data import common, config, connector, extract
 from aqueduct_executor.operators.connectors.data.spec import (
     AQUEDUCT_DEMO_NAME,
     AuthenticateSpec,
@@ -13,15 +14,14 @@
 )
 from aqueduct_executor.operators.utils import utils
 from aqueduct_executor.operators.utils.enums import (
     ArtifactType,
     ExecutionStatus,
     FailureType,
     JobType,
-    SerializationType,
 )
 from aqueduct_executor.operators.utils.exceptions import MissingConnectorDependencyException
 from aqueduct_executor.operators.utils.execution import (
     TIP_DEMO_CONNECTION,
     TIP_EXTRACT,
     TIP_INTEGRATION_CONNECTION,
     TIP_LOAD,
@@ -44,16 +44,14 @@
     - load-table
     - delete-saved-objects
     - discover
 
     Arguments:
     - spec: The spec provided for this operator.
     """
-    print("Started %s job: %s" % (spec.type, spec.name))
-
     storage = parse_storage(spec.storage_config)
     exec_state = ExecutionState(user_logs=Logs())
 
     try:
         _execute(spec, storage, exec_state)
         # Write operator execution metadata
         # Each decorator may set exec_state.status to FAILED, but if none of them did, then we are
@@ -127,31 +125,28 @@
 
 
 def run_extract(
     spec: ExtractSpec, op: connector.DataConnector, storage: Storage, exec_state: ExecutionState
 ) -> None:
     extract_params = spec.parameters
 
-    # Search for user-defined placeholder if this is a relational query, and replace them with
+    # Search for user-defined placeholders if this is a relational query, and replace them with
     # the appropriate values.
     if isinstance(extract_params, extract.RelationalParams) or isinstance(
         extract_params, extract.MongoDBParams
     ):
-        assert len(spec.input_param_names) == len(spec.input_content_paths)
         input_vals, _, _ = utils.read_artifacts(
             storage,
             spec.input_content_paths,
             spec.input_metadata_paths,
         )
         assert all(
             isinstance(param_val, str) for param_val in input_vals
         ), "Parameter value must be a string."
-
-        parameters = dict(zip(spec.input_param_names, input_vals))
-        extract_params.compile(parameters)
+        extract_params.compile(input_vals)
 
     @exec_state.user_fn_redirected(failure_tip=TIP_EXTRACT)
     def _extract() -> Any:
         return op.extract(spec.parameters)
 
     output = _extract()
 
@@ -255,50 +250,45 @@
         try:
             import psycopg2
         except:
             raise MissingConnectorDependencyException(
                 "Unable to initialize the Redshift connector. Have you run `aqueduct install redshift`?"
             )
 
-        from aqueduct_executor.operators.connectors.data.redshift import (  # type: ignore
+        from aqueduct_executor.operators.connectors.data.redshift import (
             RedshiftConnector as OpConnector,
         )
     elif connector_name == common.Name.SQL_SERVER:
         try:
             import pyodbc
         except:
             raise MissingConnectorDependencyException(
                 "Unable to initialize the SQL Server connector. Have you run `aqueduct install sqlserver`?"
             )
 
         from aqueduct_executor.operators.connectors.data.sql_server import (  # type: ignore
             SqlServerConnector as OpConnector,
         )
-    elif connector_name == common.Name.MYSQL:
+    elif connector_name == common.Name.MYSQL or connector_name == common.Name.MARIA_DB:
         try:
+            # Use pythonic mysql library to fix crossplatform compatibility issues.
+            # MySQLdb is a C-based library
+            import pymysql
+
+            # Implementation can be found here: https://github.com/PyMySQL/PyMySQL/blob/main/pymysql/__init__.py
+            pymysql.install_as_MySQLdb()
             import MySQLdb
         except:
             raise MissingConnectorDependencyException(
-                "Unable to initialize the MySQL connector. Have you run `aqueduct install mysql`?"
+                "Unable to initialize the MySQL\/MariaDB connector. Have you run `aqueduct install mysql`?"
             )
 
         from aqueduct_executor.operators.connectors.data.mysql import (  # type: ignore
             MySqlConnector as OpConnector,
         )
-    elif connector_name == common.Name.MARIA_DB:
-        try:
-            import MySQLdb
-        except:
-            raise MissingConnectorDependencyException(
-                "Unable to initialize the MariaDB connector. Have you run `aqueduct install mariadb`?"
-            )
-
-        from aqueduct_executor.operators.connectors.data.maria_db import (  # type: ignore
-            MariaDbConnector as OpConnector,
-        )
     elif connector_name == common.Name.AZURE_SQL:
         try:
             import pyodbc
         except:
             raise MissingConnectorDependencyException(
                 "Unable to initialize the Azure SQL connector. Have you run `aqueduct install azuresql`?"
             )
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/extract.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/extract.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 import json
 import re
 import uuid
-from datetime import date
 from typing import Any, Dict, List, Optional, Union
 
-from aqueduct.integrations.sql_integration import BUILT_IN_EXPANSIONS, PREV_TABLE_TAG, TAG_PATTERN
+from aqueduct.integrations.parameters import BUILT_IN_EXPANSIONS, TAG_PATTERN
 from aqueduct_executor.operators.connectors.data import common, models
 from aqueduct_executor.operators.utils.enums import ArtifactType
 from pydantic import parse_obj_as
 
+# The TAG for 'previous table' when the user specifies a chained query.
+PREV_TABLE_TAG = "$"
 
-def replace_today() -> str:
-    return "'" + date.today().strftime("%Y-%m-%d") + "'"
 
-
-def _expand_placeholders(query: str, parameters: Dict[str, str]) -> str:
-    """Expands any tags found in the raw query, eg. {{ today }}.
-
-    Relational queries can be arbitrarily parameterized the same way operators are. The only
-    requirement is that these parameters must be defined as strings.
-
-    User-defined parameters are prioritized over built-in ones. Eg. if the user defines a parameter
-    named "today" that they set with value "1234", the "{{today}}" will be expanded as "1234", even
-    though there already is a built-in expansion.
-    """
+def _replace_builtin_tags(query: str) -> str:
+    """Expands any builtin tags found in the raw query, eg. {{ today }}."""
     matches = re.findall(TAG_PATTERN, query)
     for match in matches:
         tag_name = match.strip(" {}")
-
-        if tag_name in parameters:
-            query = query.replace(match, parameters[tag_name])
-        elif tag_name in BUILT_IN_EXPANSIONS:
+        if tag_name in BUILT_IN_EXPANSIONS:
             expansion_func = BUILT_IN_EXPANSIONS[tag_name]
             query = query.replace(match, expansion_func())
-        else:
-            # If there's a tag in the query for which no expansion value is available, we error here.
-            raise Exception("Unable to expand tag `%s` for query `%s`." % (tag_name, query))
+    return query
+
+
+def _replace_param_placeholders(query: str, parameter_vals: List[str]) -> str:
+    """Replaces any user-defined placeholders in the query with the corresponding parameter value.
+
+    Assumes that we've already validated that every parameter value has a corresponding placeholder in the query.
+    """
+    for i in range(len(parameter_vals)):
+        query = query.replace("$" + str(i + 1), parameter_vals[i])
     return query
 
 
 class RelationalParams(models.BaseParams):
     # The query cannot be used until `apply_placeholders()` is called on it. This flushes out
     # any user-defined tags like `{{today}}`.
     query_is_usable: Optional[bool] = False
@@ -78,15 +72,15 @@
 
         if len(queries) == 1:
             return queries[0]
 
         with_clause = "WITH\n"
         prev_table_name = ""
         normalized_query = ""
-        for (idx, query) in enumerate(queries):
+        for idx, query in enumerate(queries):
             # Remove spaces and trailing semicolumns if any.
             normalized_query = query.strip().rstrip(";")
 
             # Replace tag except for the first query
             if idx == 0:
                 if PREV_TABLE_TAG in normalized_query:
                     raise Exception(
@@ -104,33 +98,37 @@
                 if idx < len(queries) - 2:
                     with_clause += ",\n"
                 prev_table_name = cur_table_name
 
         # Returns `WITH` clause with the normalized final query.
         return f"{with_clause}\n{normalized_query}"
 
-    def compile(self, parameters: Dict[str, str]) -> None:
+    def compile(self, parameter_vals: List[str]) -> None:
         """
         `compile` compiles this object to a single query that can be
         executed.
         """
         assert (
             int(bool(self.query)) + int(bool(self.queries)) == 1
         ), "Exactly one of .query and .queries fields should be set."
 
         queries = self.queries or []
         if self.query:
             queries = [self.query]
 
+        # Expand the placeholders first, before collapsing the query chain, since $ is broader than $1, $2, etc.
+        for i, q in enumerate(queries):
+            q = _replace_param_placeholders(q, parameter_vals)
+            queries[i] = _replace_builtin_tags(q)
+        print(f"Expanded queries are `{queries}`.")
+
         print(f"Compiling queries {queries} .")
         query = self._compile_chain(queries)
         print(f"Compiled query is {query} .")
 
-        query = _expand_placeholders(query, parameters)
-        print(f"Expanded query is `{query}`.")
         self.query = query
         self.query_is_usable = True
 
     def usable(self) -> bool:
         """Denotes whether all placeholders have already been expanded for this query.
 
         Callers should check that `usable()` -> True before actually executing this query.
@@ -153,16 +151,16 @@
 
 
 class MongoDBParams(models.BaseParams):
     collection: str
     query_serialized: str
     query: Optional[MongoDBFindParams] = None
 
-    def compile(self, parameters: Dict[str, str]) -> None:
-        expanded = _expand_placeholders(self.query_serialized, parameters)
+    def compile(self, parameters: List[str]) -> None:
+        expanded = _replace_param_placeholders(self.query_serialized, parameters)
         self.query = parse_obj_as(MongoDBFindParams, json.loads(expanded))
 
     def usable(self) -> bool:
         return bool(self.query) and bool(self.collection)
 
 
 Params = Union[RelationalParams, S3Params, MongoDBParams]
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/gcs.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/gcs.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/load.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/load.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/models.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/models.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/mongodb.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/mysql.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/mysql.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/postgres.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/postgres.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/relational.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/sqlite.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,29 @@
-from typing import Any, Callable, Dict, List, Optional
+import sqlite3
 
 import pandas as pd
-from aqueduct_executor.operators.connectors.data import connector, extract, load
+from aqueduct_executor.operators.connectors.data import config, load, relational
 from aqueduct_executor.operators.utils.enums import ArtifactType
-from aqueduct_executor.operators.utils.saved_object_delete import SavedObjectDelete
-from aqueduct_executor.operators.utils.utils import delete_object
-from sqlalchemy import MetaData, engine, inspect
-from sqlalchemy.exc import SQLAlchemyError
-from sqlalchemy.ext.declarative import declarative_base
-
-
-class RelationalConnector(connector.DataConnector):
-    def __init__(self, conn_engine: engine.Engine):
-        self.engine = conn_engine
-
-    def __del__(self) -> None:
-        self.engine.dispose()
-
-    def authenticate(self) -> None:
-        try:
-            self.engine.connect()
-        except SQLAlchemyError as e:
-            raise ConnectionError("Unable to connect.") from e
-
-    def discover(self) -> List[str]:
-        return inspect(self.engine).get_table_names()  # type: ignore
-
-    def extract(self, params: extract.RelationalParams) -> Any:
-        assert params.usable(), "Query is not usable. Did you forget to expand placeholders?"
-        return pd.read_sql(params.query, con=self.engine)
-
-    def _delete_object(self, name: str, context: Optional[Dict[str, Any]] = None) -> None:
-        if context:
-            metadata = context["metadata"]
-            base = context["base"]
+from packaging.version import parse as parse_version
+from sqlalchemy import create_engine, engine
+
+# https://www.sqlite.org/limits.html#max_variable_number
+SQLITE_MAX_VARIABLE_NUMBER = 32766
+SQLITE_MAX_VARIABLE_NUMBER_EARLIER_VERSION = 999
+
+
+class SqliteConnector(relational.RelationalConnector):
+    def __init__(self, config: config.SqliteConfig):
+        if parse_version(sqlite3.sqlite_version) >= parse_version("3.32.0"):
+            self.variable_number_limit = SQLITE_MAX_VARIABLE_NUMBER
         else:
-            raise Exception("Unexpectedly cannot find context for deletion.")
-        sql_table = metadata.tables[name]
-        base.metadata.drop_all(self.engine, [sql_table], checkfirst=True)
-
-    def delete(self, tables: List[str]) -> List[SavedObjectDelete]:
-        results = []
-        base = declarative_base()
-        metadata = MetaData()
-        metadata.reflect(bind=self.engine)
-        delete_helper: Callable[[str], None] = lambda name: self._delete_object(
-            name, context={"metadata": metadata, "base": base}
-        )
-        for table in tables:
-            results.append(
-                delete_object(
-                    table,
-                    delete_helper,
-                )
-            )
-        return results
+            self.variable_number_limit = SQLITE_MAX_VARIABLE_NUMBER_EARLIER_VERSION
+
+        conn_engine = _create_engine(config)
+        super().__init__(conn_engine)
 
     def load(
         self, params: load.RelationalParams, df: pd.DataFrame, artifact_type: ArtifactType
     ) -> None:
         if artifact_type != ArtifactType.TABLE:
             raise Exception("The data being loaded must be of type table, found %s" % artifact_type)
         # NOTE (saurav): df._to_sql has known performance issues. Using `method="multi"` helps incrementally,
@@ -67,8 +32,22 @@
         # See: https://pandas.pydata.org/docs/user_guide/io.html#io-sql-method
         df.to_sql(
             params.table,
             con=self.engine,
             if_exists=params.update_mode.value,
             index=False,
             method="multi",
+            # We need to specify chunksize due to sqlite3's variable number limit.
+            # chunksize corresponds to the max number of rows in each batch to be written at a time.
+            # Variable number is the multiplication of the row count and the column count, so we can
+            # calculate chunksize by dividing the max variable number with the number of columns.
+            chunksize=int(self.variable_number_limit / len(df.columns)),
         )
+
+
+def _create_engine(config: config.SqliteConfig) -> engine.Engine:
+    # SQLite Dialect:
+    # https://docs.sqlalchemy.org/en/14/dialects/sqlite.html#dialect-sqlite-pysqlite-connect
+    url = "sqlite:///{database}".format(
+        database=config.database,
+    )
+    return create_engine(url)
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/s3.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/s3.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,217 +1,187 @@
-import io
 import json
 from typing import Any, Dict, List, Optional
 
-import cloudpickle as pickle
 import numpy as np
 import pandas as pd
-from aqueduct_executor.operators.connectors.data import common, connector, extract, load
+from aqueduct.utils.serialization import deserialize
+from aqueduct_executor.operators.connectors.data import connector, extract, load
 from aqueduct_executor.operators.connectors.data.config import S3Config
+from aqueduct_executor.operators.connectors.data.s3_serialization import (
+    S3UnknownFileFormatException,
+    S3UnsupportedArtifactTypeException,
+    _s3_deserialization_function_mapping,
+    artifact_type_to_s3_serialization_type,
+    serialize_val_for_s3,
+)
 from aqueduct_executor.operators.connectors.data.utils import construct_boto_session
 from aqueduct_executor.operators.utils.enums import ArtifactType
 from aqueduct_executor.operators.utils.saved_object_delete import SavedObjectDelete
 from aqueduct_executor.operators.utils.utils import delete_object
-from PIL import Image
-
-_DEFAULT_JSON_ENCODING = "utf8"
-_DEFAULT_IMAGE_FORMAT = "jpeg"
+from botocore.client import ClientError
 
 
 class S3Connector(connector.DataConnector):
     def __init__(self, config: S3Config):
         session = construct_boto_session(config)
         self.s3 = session.resource("s3")
         self.bucket = config.bucket
+        self.root_dir = config.root_dir
 
     def authenticate(self) -> None:
-        bucket = self.s3.Bucket(self.bucket)
-        # Below is a low-overhead way of checking if the user has access to the bucket.
-        # Source: https://stackoverflow.com/a/49817544
-        if not bucket.creation_date:
+        try:
+            # Below is a low-overhead way of checking if the user has access to the bucket.
+            # Source: https://stackoverflow.com/a/49817544
+            self.s3.meta.client.head_bucket(Bucket=self.bucket)
+        except ClientError as e:
             raise Exception(
-                "Bucket does not exist or you do not have permission to access the bucket."
+                "Bucket does not exist or you do not have permission to access the bucket: %s."
+                % str(e)
             )
 
+        # Check that any user-supplied root directory exists.
+        if self.root_dir != "":
+            # If nothing is returned by this filter call, then the directory does not exist.
+            if len(list(self.s3.Bucket(self.bucket).objects.filter(Prefix=self.root_dir))) == 0:
+                raise Exception(
+                    "Supplied root directory `%s` does not exist in bucket %s."
+                    % (self.root_dir, self.bucket)
+                )
+
     def discover(self) -> List[str]:
         raise Exception("Discover is not supported for S3.")
 
-    def _fetch_object(self, key: str, params: extract.S3Params) -> Any:
+    def fetch_object(self, key: str, params: extract.S3Params) -> Any:
         response = self.s3.Object(self.bucket, key).get()
         data = response["Body"].read()
-        if params.artifact_type == ArtifactType.TABLE:
-            if params.format is None:
-                raise Exception("You must specify a file format for table data.")
-            buf = io.BytesIO(data)
-
-            try:
-                if params.format == common.S3TableFormat.CSV:
-                    return pd.read_csv(buf)
-                elif params.format == common.S3TableFormat.JSON:
-                    return pd.read_json(buf)
-                elif params.format == common.S3TableFormat.PARQUET:
-                    return pd.read_parquet(buf)
-            except Exception:
+
+        try:
+            s3_serialization_type = artifact_type_to_s3_serialization_type(
+                params.artifact_type, params.format
+            )
+
+        # Append the S3 filepath to the message for additional error context.
+        except S3UnsupportedArtifactTypeException:
+            raise S3UnsupportedArtifactTypeException(
+                "Unsupported data type %s when fetching file at %s." % (params.artifact_type, key)
+            )
+        except S3UnknownFileFormatException:
+            raise S3UnknownFileFormatException(
+                "Unknown S3 file format `%s` for file at path `%s`." % (params.format, key)
+            )
+
+        try:
+            deserialized_val = deserialize(
+                s3_serialization_type,
+                params.artifact_type,
+                data,
+                custom_deserialization_function_mapping=_s3_deserialization_function_mapping,
+            )
+        except Exception as e:
+            print(str(e))
+            err_msg = "The file at path `%s` is not a valid %s object." % (
+                key,
+                params.artifact_type,
+            )
+            if params.artifact_type == ArtifactType.TABLE and params.format is not None:
+                err_msg += " (with S3 file format `%s`)" % params.format.value
+
+            raise Exception(err_msg)
+
+        # Perform some additional type checking after deserialization.
+        if params.artifact_type == ArtifactType.STRING:
+            if not isinstance(deserialized_val, str):
                 raise Exception(
-                    "Unable to read in table at path `%s` with S3 file format `%s`."
-                    % (key, params.format)
+                    "The file at path `%s` is expected to be a string, got %s."
+                    % (key, type(deserialized_val))
                 )
-            else:
+        elif params.artifact_type == ArtifactType.BOOL:
+            if not (isinstance(deserialized_val, bool) or isinstance(deserialized_val, np.bool_)):
                 raise Exception(
-                    "Unknown S3 file format `%s` for file at path `%s`." % (params.format, key)
+                    "The file at path `%s` is expected to be a bool, got %s."
+                    % (key, type(deserialized_val))
+                )
+        elif params.artifact_type == ArtifactType.NUMERIC:
+            if not (
+                isinstance(deserialized_val, int)
+                or isinstance(deserialized_val, float)
+                or isinstance(deserialized_val, np.number)
+            ):
+                raise Exception(
+                    "The file at path `%s` is expected to be a numeric, got %s."
+                    % (key, type(deserialized_val))
+                )
+        elif params.artifact_type == ArtifactType.DICT:
+            if not isinstance(deserialized_val, dict):
+                raise Exception(
+                    "The file at path `%s` is expected to be a dictionary, got %s."
+                    % (key, type(deserialized_val))
+                )
+        elif params.artifact_type == ArtifactType.TUPLE:
+            if not isinstance(deserialized_val, tuple):
+                raise Exception(
+                    "The file at path `%s` is expected to be a tuple, got %s."
+                    % (key, type(deserialized_val))
+                )
+        elif params.artifact_type == ArtifactType.LIST:
+            if not isinstance(deserialized_val, list):
+                raise Exception(
+                    "The file at path `%s` is expected to be a list, got %s."
+                    % (key, type(deserialized_val))
                 )
 
-        elif params.artifact_type == ArtifactType.JSON:
-            # This assumes that the encoding is "utf-8". May worth considering letting the user
-            # specify custom encoding in the future.
-            json_data = data.decode(_DEFAULT_JSON_ENCODING)
-            # Make sure the data is a valid json object.
-            try:
-                json.loads(json_data)
-                return json_data
-            except:
-                raise Exception("The file at path `%s` is not a valid JSON object.", key)
-        elif params.artifact_type == ArtifactType.IMAGE:
-            try:
-                return Image.open(io.BytesIO(data))
-            except:
-                raise Exception("The file at path `%s` is not a valid image object.", key)
-
-        elif params.artifact_type == ArtifactType.BYTES:
-            return data
-        elif (
-            params.artifact_type == ArtifactType.STRING
-            or params.artifact_type == ArtifactType.BOOL
-            or params.artifact_type == ArtifactType.NUMERIC
-            or params.artifact_type == ArtifactType.DICT
-            or params.artifact_type == ArtifactType.LIST
-            or params.artifact_type == ArtifactType.TUPLE
-            or params.artifact_type == ArtifactType.PICKLABLE
-        ):
-            try:
-                unpickled_data = pickle.loads(data)
-            except Exception:
-                raise Exception(
-                    "The file at path `%s` is not a valid %s object." % (key, params.artifact_type),
-                )
-
-            if params.artifact_type == ArtifactType.STRING:
-                if not isinstance(unpickled_data, str):
-                    raise Exception(
-                        "The file at path `%s` is expected to be a string, got %s."
-                        % (key, type(unpickled_data))
-                    )
-            elif params.artifact_type == ArtifactType.BOOL:
-                if not (isinstance(unpickled_data, bool) or isinstance(unpickled_data, np.bool_)):
-                    raise Exception(
-                        "The file at path `%s` is expected to be a bool, got %s."
-                        % (key, type(unpickled_data))
-                    )
-            elif params.artifact_type == ArtifactType.NUMERIC:
-                if not (
-                    isinstance(unpickled_data, int)
-                    or isinstance(unpickled_data, float)
-                    or isinstance(unpickled_data, np.number)
-                ):
-                    raise Exception(
-                        "The file at path `%s` is expected to be a numeric, got %s."
-                        % (key, type(unpickled_data))
-                    )
-            elif params.artifact_type == ArtifactType.DICT:
-                if not isinstance(unpickled_data, dict):
-                    raise Exception(
-                        "The file at path `%s` is expected to be a dictionary, got %s."
-                        % (key, type(unpickled_data))
-                    )
-            elif params.artifact_type == ArtifactType.TUPLE:
-                if not isinstance(unpickled_data, tuple):
-                    raise Exception(
-                        "The file at path `%s` is expected to be a tuple, got %s."
-                        % (key, type(unpickled_data))
-                    )
-
-            return unpickled_data
-        else:
-            raise Exception(
-                "Unsupported data type %s when fetching file at %s." % (params.artifact_type, key)
-            )
+        return deserialized_val
 
     def extract(self, params: extract.S3Params) -> Any:
         path = json.loads(params.filepath)
         if not isinstance(path, List):
             if len(path) == 0:
                 raise Exception("S3 file path cannot be an empty string.")
             if path[-1] == "/":
-                # This means the path is a directory, and we will do a prefix search.
                 files = []
-                for obj in self.s3.Bucket(self.bucket).objects.filter(Prefix=path):
+                s3_file_collection = self.s3.Bucket(self.bucket).objects.filter(Prefix=path)
+                # If nothing is returned, that means the file directory does not exist.
+                if (len(list(s3_file_collection))) == 0:
+                    raise Exception("Given path to S3 directory '%s' does not exist." % (path))
+                for obj in s3_file_collection:
                     # The filter api also returns the directories, so we filter them out.
                     if (obj.key)[-1] != "/":
-                        files.append(self._fetch_object(obj.key, params))
+                        files.append(self.fetch_object(obj.key, params))
 
                 if params.artifact_type == ArtifactType.TABLE and params.merge:
                     # We ignore indexes anyways when serializing the data later, so it's ok to do it earlier here.
                     return pd.concat(files, ignore_index=True)
                 else:
                     return tuple(files)
             else:
                 # This means the path is a file name, and we do a regular file retrieval.
-                return self._fetch_object(path, params)
+                return self.fetch_object(path, params)
         else:
             # This means we have a list of file paths.
             files = []
             for key in path:
                 if len(key) == 0:
                     raise Exception("S3 file path cannot be an empty string.")
                 if key[-1] == "/":
                     raise Exception("Each key in the list must not be a directory, found %s." % key)
-                files.append(self._fetch_object(key, params))
+                files.append(self.fetch_object(key, params))
 
             if params.artifact_type == ArtifactType.TABLE and params.merge:
                 # We ignore indexes anyways when serializing the data later, so it's ok to do it earlier here.
                 return pd.concat(files, ignore_index=True)
             else:
                 return tuple(files)
 
     def load(self, params: load.S3Params, data: Any, artifact_type: ArtifactType) -> None:
-        if artifact_type == ArtifactType.TABLE:
-            if params.format is None:
-                raise Exception("You must specify a file format for table data.")
-            buf = io.BytesIO()
-            if params.format == common.S3TableFormat.CSV:
-                data.to_csv(buf, index=False)
-            elif params.format == common.S3TableFormat.JSON:
-                # Index cannot be False for `to.json` for default orient
-                # See: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_json.html
-                data.to_json(buf)
-            elif params.format == common.S3TableFormat.PARQUET:
-                data.to_parquet(buf, index=False)
-            else:
-                raise Exception("Unknown S3 file format %s." % params.format)
-            serialized_data = buf.getvalue()
-        elif artifact_type == ArtifactType.JSON:
-            serialized_data = data.encode(_DEFAULT_JSON_ENCODING)
-        elif artifact_type == ArtifactType.IMAGE:
-            img_bytes = io.BytesIO()
-            data.save(img_bytes, format=_DEFAULT_IMAGE_FORMAT)
-            serialized_data = img_bytes.getvalue()
-        elif artifact_type == ArtifactType.BYTES:
-            serialized_data = data
-        elif (
-            artifact_type == ArtifactType.STRING
-            or artifact_type == ArtifactType.BOOL
-            or artifact_type == ArtifactType.NUMERIC
-            or artifact_type == ArtifactType.DICT
-            or artifact_type == ArtifactType.LIST
-            or artifact_type == ArtifactType.TUPLE
-            or artifact_type == ArtifactType.PICKLABLE
-        ):
-            serialized_data = pickle.dumps(data)
-        else:
-            raise Exception("Unsupported data type `%s`." % artifact_type)
+        serialization_type = artifact_type_to_s3_serialization_type(artifact_type, params.format)
+        serialized_data = serialize_val_for_s3(
+            data,
+            serialization_type,
+            params.format,
+        )
 
         self.s3.Object(self.bucket, params.filepath).put(Body=serialized_data)
 
     def _delete_object(self, name: str, context: Optional[Dict[str, Any]] = None) -> None:
         """`name` is expected to be the S3 FilePath, found in S3Params."""
         self.s3.Object(self.bucket, name).delete()
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/spec.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/spec.py`

 * *Files 11% similar despite different names*

```diff
@@ -85,17 +85,14 @@
     type: Literal[enums.JobType.EXTRACT]
     storage_config: sconfig.StorageConfig
     metadata_path: str
     connector_name: common.Name
     connector_config: config.Config
     parameters: extract.Params
 
-    # The input fields are only used to record user-defined parameters for relational queries.
-    # The tags in the queries will be expanded into the parameter values.
-    input_param_names: List[str]
     input_content_paths: List[str]
     input_metadata_paths: List[str]  # This field is ignored and is only here for completeness.
     output_content_path: str
     output_metadata_path: str
 
     # validators
     _unwrap_connector_config = validator("connector_config", allow_reuse=True, pre=True)(
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/sql_server.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/sql_server.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/data/utils.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/data/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/conf.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/conf.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_bigquery.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_mariadb.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_mysql.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_postgres.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_redshift.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_snowflake.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_sql_server.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_sql_server.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/test_sqlite.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/connectors/tests/utils.py` & `hstestaq-0.2.11/aqueduct_executor/operators/connectors/tests/utils.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/function_executor/execute.py` & `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/execute.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import sys
 import tracemalloc
 import uuid
 from typing import Any, Callable, Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
+from aqueduct.utils.serialization import check_and_fetch_pickled_collection_format
 from aqueduct.utils.type_inference import infer_artifact_type
 from aqueduct_executor.operators.function_executor import extract_function, get_extract_path
 from aqueduct_executor.operators.function_executor.spec import FunctionSpec
 from aqueduct_executor.operators.function_executor.utils import OP_DIR
 from aqueduct_executor.operators.utils import utils
 from aqueduct_executor.operators.utils.enums import (
     ArtifactType,
@@ -30,18 +31,20 @@
     TIP_UNKNOWN_ERROR,
     ExecFailureException,
     ExecutionState,
     Logs,
     exception_traceback,
 )
 from aqueduct_executor.operators.utils.storage.parse import parse_storage
+from aqueduct_executor.operators.utils.storage.storage import Storage
 from aqueduct_executor.operators.utils.timer import Timer
+from aqueduct_executor.operators.utils.utils import time_it
 
 
-def _get_py_import_path(spec: FunctionSpec) -> str:
+def get_py_import_path(spec: FunctionSpec) -> str:
     """
     Generates the import path based on fixed function dir and
     FUNCTION_ENTRY_POINT_FILE env var.
 
     It removes .py (if any) from the entry point and replaces all
     '/' with '.'
 
@@ -53,17 +56,17 @@
         file_path = file_path[:-3]
 
     if file_path.startswith("/"):
         file_path = file_path[1:]
     return file_path.replace("/", ".")
 
 
-def _import_invoke_method(spec: FunctionSpec) -> Callable[..., Any]:
+def import_invoke_method(spec: FunctionSpec) -> Callable[..., Any]:
     """
-    `_import_invoke_method` imports the model object.
+    `import_invoke_method` imports the model object.
     it assumes the operator has been extracted to `<storage>/operators/<id>/op`
     and imports the route from the above path.
     """
 
     # fn_path should be `<storage>/operators/<id>`
     fn_path = spec.function_extract_path
 
@@ -73,15 +76,15 @@
     print(f"listdir(fn_path): {os.listdir(fn_path)}")
 
     # this ensures any file manipulation happens with respect to work_dir
     os.chdir(work_dir)
     # adds work_dir to sys.path to support relative imports from work_dir
     sys.path.append(work_dir)
 
-    import_path = _get_py_import_path(spec)
+    import_path = get_py_import_path(spec)
     print(f"import_path: {import_path}")
     class_name = spec.entry_point_class
     method_name = spec.entry_point_method
     custom_args_str = spec.custom_args
 
     # Invoke the function and parse out the result object.
 
@@ -100,57 +103,97 @@
     return getattr(function, method_name)  # type: ignore
 
 
 def _execute_function(
     spec: FunctionSpec,
     inputs: List[Any],
     exec_state: ExecutionState,
-) -> Tuple[List[Any], List[ArtifactType], Dict[str, str]]:
+) -> Tuple[List[Any], Dict[str, str]]:
     """
     Invokes the given function on the input data. Does not raise an exception on any
     user function errors, but instead annotates the given exec state with the error.
 
     :param inputs: the input data to feed into the user's function.
     """
 
-    invoke = _import_invoke_method(spec)
+    invoke = import_invoke_method(spec)
     timer = Timer()
-    print("Invoking the function...")
     timer.start()
     tracemalloc.start()
 
     @exec_state.user_fn_redirected(failure_tip=TIP_OP_EXECUTION)
     def _invoke() -> Any:
         return invoke(*inputs)
 
     results = _invoke()
-
-    # We only validate the number of results if multiple outputs are expected.
-    # Otherwise, we treat the results as a single object.
-    if len(spec.output_content_paths) > 1 and len(spec.output_content_paths) != len(results):
-        raise ExecFailureException(
-            failure_type=FailureType.USER_FATAL,
-            tip="Expected function to have %s outputs, but instead it had %s."
-            % (len(spec.output_content_paths), len(results)),
-        )
-
     if len(spec.output_content_paths) == 1:
         results = [results]
 
-    inferred_result_types = [infer_artifact_type(res) for res in results]
-
     elapsedTime = timer.stop()
     _, peak = tracemalloc.get_traced_memory()
     system_metadata = {
         utils._RUNTIME_SEC_METRIC_NAME: str(elapsedTime),
         utils._MAX_MEMORY_MB_METRIC_NAME: str(peak / 10**6),
     }
 
     sys.path.pop(0)
-    return results, inferred_result_types, system_metadata
+    return results, system_metadata
+
+
+def _validate_result_count_and_infer_type(
+    spec: FunctionSpec,
+    results: List[Any],
+    infer_type_func: Any,
+) -> List[ArtifactType]:
+    """
+    Validates that the expected number of results were returned by the Function
+    and infers the ArtifactType of each result.
+
+    Args:
+        spec: The FunctionSpec for the Function
+        results: The results returned by the Function
+
+    Returns:
+        The ArtifactType of each result
+
+    Raises:
+        ExecFailureException: If the expected number of results were not returned
+    """
+    if len(spec.output_content_paths) > 1 and len(spec.output_content_paths) != len(results):
+        raise ExecFailureException(
+            failure_type=FailureType.USER_FATAL,
+            tip="Expected function to have %s outputs, but instead it had %s."
+            % (len(spec.output_content_paths), len(results)),
+        )
+
+    return [infer_type_func(res) for res in results]
+
+
+def _write_artifacts(
+    write_func: Any,
+    results: Any,
+    result_types: List[ArtifactType],
+    derived_from_bson: bool,
+    output_content_paths: List[str],
+    output_metadata_paths: List[str],
+    system_metadata: Any,
+    storage: Storage,
+    **kwargs,
+) -> None:
+    for i, result in enumerate(results):
+        write_func(
+            storage,
+            result_types[i],
+            derived_from_bson,
+            output_content_paths[i],
+            output_metadata_paths[i],
+            result,
+            system_metadata=system_metadata,
+            **kwargs,
+        )
 
 
 def validate_spec(spec: FunctionSpec) -> None:
     if len(spec.input_content_paths) != len(spec.input_metadata_paths):
         raise Exception(
             "Found inconsistent number of input paths (%d) and input metadata paths (%d)"
             % (
@@ -182,50 +225,83 @@
     if (spec.operator_type == OperatorType.CHECK or spec.operator_type == OperatorType.METRIC) and (
         spec.expected_output_artifact_types is not None
         and len(spec.expected_output_artifact_types) != 1
     ):
         raise Exception("%s operators must only have a single output." % spec.operator_type)
 
 
-def _cleanup(spec: FunctionSpec) -> None:
+def cleanup(spec: FunctionSpec) -> None:
     """
     Cleans up any temporary files created during function execution.
     """
     # Delete the extracted fn file if it exists and the file path is not
     # something dangerous
     if spec.function_extract_path and spec.function_extract_path[-1] != "*":
         shutil.rmtree(spec.function_extract_path)
 
 
 def run(spec: FunctionSpec) -> None:
     """
     Executes a function operator.
     """
-    print("Started %s job: %s" % (spec.type, spec.name))
+    run_helper(
+        spec=spec,
+        read_func=utils.read_artifacts,
+        write_func=utils.write_artifact, 
+        infer_type_func=infer_artifact_type,
+    )
 
+
+def run_helper(spec: FunctionSpec, read_func: Any, write_func: Any, infer_type_func: Any, **kwargs) -> None:
+    """
+    Executes a function operator.
+    """
     exec_state = ExecutionState(user_logs=Logs())
     storage = parse_storage(spec.storage_config)
     try:
         validate_spec(spec)
 
         # Read the input data from intermediate storage.
-        inputs, _, serialization_types = utils.read_artifacts(
-            storage, spec.input_content_paths, spec.input_metadata_paths
+        inputs, _, serialization_types = time_it(
+            job_name=spec.name, job_type=spec.type.value, step="Reading Inputs"
+        )(read_func)(
+            storage=storage, 
+            input_paths=spec.input_content_paths, 
+            input_metadata_paths=spec.input_metadata_paths, 
+            **kwargs
         )
 
+        # We need to check for BSON_TABLE serialization type at both the top level
+        # and within any serialized pickled collection (if it exists).
         derived_from_bson = SerializationType.BSON_TABLE in serialization_types
-        print("Invoking the function...")
-        results, result_types, system_metadata = _execute_function(spec, inputs, exec_state)
+        if not derived_from_bson:
+            for i, serialization_type in enumerate(serialization_types):
+                collection_data = check_and_fetch_pickled_collection_format(
+                    serialization_type, inputs[i]
+                )
+                if (
+                    collection_data is not None
+                    and SerializationType.BSON_TABLE in collection_data.aqueduct_serialization_types
+                ):
+                    derived_from_bson = True
+                    break
+
+        results, system_metadata = time_it(
+            job_name=spec.name, job_type=spec.type.value, step="Running Function"
+        )(_execute_function)(spec, inputs, exec_state)
+
         if exec_state.status == ExecutionStatus.FAILED:
             # user failure
             utils.write_exec_state(storage, spec.metadata_path, exec_state)
             sys.exit(1)
 
         print("Function invoked successfully!")
 
+        result_types = _validate_result_count_and_infer_type(spec=spec, results=results, infer_type_func=infer_type_func)
+
         # Perform type checking on the function output.
         if spec.operator_type == OperatorType.METRIC:
             assert len(results) == 1, "Metric operator can only have a single output."
             result = results[0]
 
             if not (
                 isinstance(result, int)
@@ -257,23 +333,23 @@
                     tip=TIP_NOT_BOOL,
                 )
 
             # If the check returned a value we interpret to mean 'false', we exit here, but
             # not before recording the output artifact value (which will be False).
             if not check_passed:
                 print(f"Check Operator did not pass.")
-
-                utils.write_artifact(
-                    storage,
-                    ArtifactType.BOOL,
-                    derived_from_bson,  # derived_from_bson doesn't apply to bool artifact
-                    spec.output_content_paths[0],
-                    spec.output_metadata_paths[0],
-                    check_passed,
+                write_func(
+                    storage=storage,
+                    artifact_type=ArtifactType.BOOL,
+                    derived_from_bson=derived_from_bson,  # derived_from_bson doesn't apply to bool artifact
+                    output_path=spec.output_content_paths[0],
+                    output_metadata_path=spec.output_metadata_paths[0],
+                    content=check_passed,
                     system_metadata=system_metadata,
+                    **kwargs,
                 )
 
                 check_severity = spec.check_severity
                 if spec.check_severity is None:
                     print(
                         "Check operator has an unspecified severity on spec. Defaulting to ERROR."
                     )
@@ -286,43 +362,38 @@
                 raise ExecFailureException(failure_type, tip=TIP_CHECK_DID_NOT_PASS)
 
             # If we get here, we know that the check has passed. The artifact type might need
             # still be updated. Eg. if the output was a pandas series.
             result_types[0] = ArtifactType.BOOL
             results[0] = True
         else:
-            # Error if the number of expected outputs is not what was returned by the user's function.
-            if len(results) != len(spec.expected_output_artifact_types):
-                raise ExecFailureException(
-                    failure_type=FailureType.USER_FATAL,
-                    tip="Expected function to return %d outputs, but instead got %d."
-                    % (len(spec.expected_output_artifact_types), len(results)),
-                )
-
             for i, expected_output_type in enumerate(spec.expected_output_artifact_types):
                 if (
                     expected_output_type != ArtifactType.UNTYPED
                     and expected_output_type != result_types[i]
                 ):
                     raise ExecFailureException(
                         failure_type=FailureType.USER_FATAL,
                         tip="Expected type %s for the %d-th output of function, but it is of type %s."
                         % (expected_output_type, i, result_types[i]),
                     )
 
-        for i, result in enumerate(results):
-            utils.write_artifact(
-                storage,
-                result_types[i],
-                derived_from_bson,
-                spec.output_content_paths[i],
-                spec.output_metadata_paths[i],
-                result,
-                system_metadata=system_metadata,
-            )
+        time_it(job_name=spec.name, job_type=spec.type.value, step="Writing Outputs")(
+            _write_artifacts
+        )(
+            write_func=write_func,
+            results=results,
+            result_types=result_types,
+            derived_from_bson=derived_from_bson,
+            output_content_paths=spec.output_content_paths,
+            output_metadata_paths=spec.output_metadata_paths,
+            system_metadata=system_metadata,
+            storage=storage,
+            **kwargs,
+        )
 
         # If we made it here, then the operator has succeeded.
         exec_state.status = ExecutionStatus.SUCCEEDED
         print(f"Succeeded! Full logs: {exec_state.json()}")
         utils.write_exec_state(storage, spec.metadata_path, exec_state)
 
     except ExecFailureException as e:
@@ -337,15 +408,16 @@
             FailureType.SYSTEM, TIP_UNKNOWN_ERROR, context=exception_traceback(e)
         )
         print(f"Failed with system error. Full Logs:\n{exec_state.json()}")
         utils.write_exec_state(storage, spec.metadata_path, exec_state)
         sys.exit(1)
     finally:
         # Perform any cleanup
-        _cleanup(spec)
+        cleanup(spec)
+
 
 
 def run_with_setup(spec: FunctionSpec) -> None:
     """
     Performs the setup needed for a Function operator and then executes it.
     """
     # Generate a unique function extract path if one does not exist already
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/function_executor/extract_function.py` & `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/extract_function.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import traceback
 import zipfile
 
 from aqueduct_executor.operators.function_executor.spec import FunctionSpec, parse_spec
 from aqueduct_executor.operators.function_executor.utils import OP_DIR
 from aqueduct_executor.operators.utils.storage.parse import parse_storage
 from aqueduct_executor.operators.utils.storage.storage import Storage
+from aqueduct_executor.operators.utils.utils import time_it
 
 
 def _unzip_function_contents(function_in_bytes: bytes, extract_path: str) -> None:
     """
     Unzips raw function bytes into the current directory, assuming the bytes represent
     a zip file.
     """
@@ -77,8 +78,8 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("-s", "--spec", required=True)
     args = parser.parse_args()
 
     spec_json = base64.b64decode(args.spec)
     spec = parse_spec(spec_json)
 
-    run(spec)
+    time_it(job_name=spec.name, job_type=spec.type.value, step="Loading Function")(run)(spec)
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/function_executor/get_extract_path.py` & `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/get_extract_path.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/function_executor/install_requirements.py` & `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/install_requirements.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from typing import Optional
 
 from aqueduct_executor.operators.function_executor.spec import FunctionSpec, parse_spec
 from aqueduct_executor.operators.utils import utils
 from aqueduct_executor.operators.utils.enums import FailureType
 from aqueduct_executor.operators.utils.execution import ExecFailureException, ExecutionState, Logs
 from aqueduct_executor.operators.utils.storage.parse import parse_storage
+from aqueduct_executor.operators.utils.utils import time_it
 
 
 def install_missing_packages(
     missing_path: str, spec: FunctionSpec, conda_env: Optional[str]
 ) -> None:
-
     if conda_env:
         install_output = subprocess.run(
             [
                 "conda",
                 "run",
                 "-n",
                 conda_env,
@@ -89,8 +89,10 @@
     parser.add_argument("--spec", required=True)
     parser.add_argument("--conda_env")
     args = parser.parse_args()
 
     spec_json = base64.b64decode(args.spec)
     spec = parse_spec(spec_json)
 
-    run(args.local_path, args.requirements_path, args.missing_path, spec, args.conda_env)
+    time_it(job_name=spec.name, job_type=spec.type.value, step="Installing Dependencies")(run)(
+        args.local_path, args.requirements_path, args.missing_path, spec, args.conda_env
+    )
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/function_executor/set_conda_version.py` & `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/set_conda_version.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/function_executor/spec.py` & `hstestaq-0.2.11/aqueduct_executor/operators/function_executor/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/param_executor/execute.py` & `hstestaq-0.2.11/aqueduct_executor/operators/param_executor/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/param_executor/spec.py` & `hstestaq-0.2.11/aqueduct_executor/operators/param_executor/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/system_metric_executor/execute.py` & `hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/execute.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/system_metric_executor/spec.py` & `hstestaq-0.2.11/aqueduct_executor/operators/system_metric_executor/spec.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/utils/enums.py` & `hstestaq-0.2.11/aqueduct_executor/operators/utils/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,7 +77,14 @@
     BSON_TABLE = "bson_table"
     JSON = "json"
     PICKLE = "pickle"
     IMAGE = "image"
     STRING = "string"
     BYTES = "bytes"
     TF_KERAS = "tensorflow-keras-model"
+
+
+class PrintColorType(str, Enum, metaclass=MetaEnum):
+    # These are the ANSI color codes for Python.
+    # More color codes here (https://code-maven.com/ansi-command-line-colors-with-python).
+    GREEN = "\33[32m"
+    YELLOW = "\33[33m"
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/utils/execution.py` & `hstestaq-0.2.11/aqueduct_executor/operators/utils/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 _TIP_CREATE_BUG_REPORT = (
     f"Please create bug report in github: {_GITHUB_ISSUE_LINK} . "
     "We will get back to you as soon as we can."
 )
 TIP_UNKNOWN_ERROR = f"Sorry, we've run into an unexpected error! {_TIP_CREATE_BUG_REPORT}"
 TIP_INTEGRATION_CONNECTION = (
     "We were unable to connect to this integration. "
-    "Please check your credentials or contact your integration's provider."
+    "If the stack trace is not helpful, please check your credentials or contact your integration's provider."
 )
 TIP_DEMO_CONNECTION = f"We have trouble connecting to demo DB. {_TIP_CREATE_BUG_REPORT}"
 
 TIP_EXTRACT = "We couldn't execute the provided query. Please double check your query is correct."
 TIP_LOAD = "We couldn't load to the integration. Please make sure the target exists, or you have the right permission."
 TIP_DISCOVER = "We couldn't list items in the integration. Please make sure your credentials have the right permission."
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/utils/storage/config.py` & `hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 class FileStorageConfig(BaseModel):
     directory: str
 
 
 class S3StorageConfig(BaseModel):
     region: str
     bucket: str
+
+    # Expected to be in the format "path/to/dir/" (without a leading slash, but with a trailing one).
+    root_dir: str = ""
+
     credentials_path: str
     credentials_profile: str
     aws_access_key_id: str = ""
     aws_secret_access_key: str = ""
 
 
 class GCSStorageConfig(BaseModel):
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/utils/storage/file.py` & `hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 from aqueduct_executor.operators.utils.storage.config import FileStorageConfig
 from aqueduct_executor.operators.utils.storage.storage import Storage
 
 
 class FileStorage(Storage):
     _config: FileStorageConfig
 
@@ -16,9 +18,14 @@
 
     def get(self, key: str) -> bytes:
         path = self.get_full_path(key)
         print(f"reading from file: {path}")
         with open(path, "rb") as f:
             return f.read()
 
+    def exists(self, key: str) -> bool:
+        path = self.get_full_path(key)
+        print(f"checking if file exists: {path}")
+        return os.path.isfile(path)
+
     def get_full_path(self, key: str) -> str:
         return self._config.directory + "/" + key
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/utils/storage/gcs.py` & `hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/gcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,7 +28,14 @@
 
     def get(self, key: str) -> bytes:
         bucket = self._client.bucket(self._config.bucket)
         blob = bucket.blob(key)
 
         print(f"reading from gcs: {key}")
         return bytes(blob.download_as_bytes())
+
+    def exists(self, key: str) -> bool:
+        bucket = self._client.bucket(self._config.bucket)
+        blob = bucket.blob(key)
+
+        print(f"checking if exists in gcs: {key}")
+        return bool(blob.exists())
```

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/utils/storage/parse.py` & `hstestaq-0.2.11/aqueduct_executor/operators/utils/storage/parse.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/aqueduct_executor/operators/utils/timer.py` & `hstestaq-0.2.11/aqueduct_executor/operators/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hstestaq-0.1.9/bin/aqueduct` & `hstestaq-0.2.11/bin/aqueduct`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,32 @@
 
 import distro
 import requests
 import yaml
 from packaging.version import parse as parse_version
 from tqdm import tqdm
 
-SCHEMA_VERSION = "22"
+SCHEMA_VERSION = "25"
 CHUNK_SIZE = 4096
 
+# Connector Package Version Bounds
+PYMONGO_VERSION_BOUND = "<=4.3.3"
+PSYCOPG2_VERSION_BOUND = "<=2.9.5"
+BIGQUERY_VERSION_BOUND = "<=3.5.0"
+SNOWFLAKE_VERSION_BOUND = "<=1.4.4"
+PYARROW_VERSION_BOUND = "<=11.0.0"
+AWS_WRANGLER_VERSION_BOUND = "<=2.19.0"
+MYSQL_CLIENT_VERSION_BOUND = "<=2.1.1"
+PYODBC_VERSION_BOUND = "<=4.0.35"
+
 base_directory = os.path.join(os.environ["HOME"], ".aqueduct")
 server_directory = os.path.join(os.environ["HOME"], ".aqueduct", "server")
 ui_directory = os.path.join(os.environ["HOME"], ".aqueduct", "ui")
 
-package_version = "0.1.9"
+package_version = "0.2.11"
 aws_credentials_path = os.path.join(os.environ["HOME"], ".aws", "credentials")
 
 default_server_port = 8080
 
 s3_server_prefix = (
     "https://aqueduct-ai.s3.us-east-2.amazonaws.com/assets/%s/server" % package_version
 )
@@ -173,21 +183,17 @@
 
 
 def download_server_binaries(architecture):
     print("Downloading server binaries...")
     with open(os.path.join(server_directory, "bin/server"), "wb") as f:
         _download_file(os.path.join(s3_server_prefix, f"bin/{architecture}/server"), f, "Server")
     with open(os.path.join(server_directory, "bin/executor"), "wb") as f:
-        _download_file(
-            os.path.join(s3_server_prefix, f"bin/{architecture}/executor"), f, "Executor"
-        )
+        _download_file(os.path.join(s3_server_prefix, f"bin/{architecture}/executor"), f, "Executor")
     with open(os.path.join(server_directory, "bin/migrator"), "wb") as f:
-        _download_file(
-            os.path.join(s3_server_prefix, f"bin/{architecture}/migrator"), f, "Migrator"
-        )
+        _download_file(os.path.join(s3_server_prefix, f"bin/{architecture}/migrator"), f, "Migrator")
 
     print("Downloading integration set up scripts...")
     with open(os.path.join(server_directory, "bin/start-function-executor.sh"), "wb") as f:
         _download_file(os.path.join(s3_server_prefix, f"bin/start-function-executor.sh"), f)
     with open(os.path.join(server_directory, "bin/dag.template"), "wb") as f:
         _download_file(os.path.join(s3_server_prefix, f"bin/dag.template"), f)
     with open(os.path.join(server_directory, "bin/install_sqlserver_ubuntu.sh"), "wb") as f:
@@ -213,14 +219,24 @@
         download_server_binaries("darwin_arm64")
     else:
         raise Exception(
             "Unsupported operating system and architecture combination: %s, %s" % (system, arch)
         )
 
 
+def download_terraform_template():
+    terraform_folder = os.path.join(server_directory, "template", "aws", "eks")
+    terraform_zip_path = os.path.join(terraform_folder, "eks_terraform.zip")
+    with open(terraform_zip_path, "wb") as f:
+        _download_file(os.path.join(s3_server_prefix, "template", "aws", "eks", "eks_terraform.zip"), f)
+    with zipfile.ZipFile(terraform_zip_path, "r") as zip:
+        zip.extractall(terraform_folder)
+    os.remove(terraform_zip_path)
+
+
 def update_ui_version():
     print("Updating UI version to %s..." % package_version)
     try:
         shutil.rmtree(ui_directory, ignore_errors=True)
         os.mkdir(ui_directory)
         generate_version_file(os.path.join(ui_directory, "__version__"))
         ui_zip_path = os.path.join(ui_directory, "ui.zip")
@@ -247,28 +263,31 @@
         os.remove(version_file)
 
     generate_version_file(version_file)
 
     setup_server_binaries()
     update_executable_permissions()
 
+    download_terraform_template()
+
     execute_command(
         [
             os.path.join(server_directory, "bin", "migrator"),
             "--type",
             "sqlite",
             "goto",
             SCHEMA_VERSION,
         ]
     )
 
     if parse_version(current_version) < parse_version("0.1.0") and parse_version(package_version) >= parse_version("0.1.0"):
         # We add a couple new tables to the demo db for the v0.1.0 release.
         # If we want to add tables in other releases in the future, we should refactor each of them
         # into a helper function.
+        print("Adding new tables to the demo db...")
         data_script_path = os.path.join(server_directory, "db", "0.1.0", "create_tables.py")
         data_script_dir = os.path.dirname(data_script_path)
         if not os.path.isdir(data_script_dir):
             os.mkdir(data_script_dir)
         s3_path = ("https://aqueduct-ai.s3.us-east-2.amazonaws.com/assets/demo/0.1.0/create_tables.py")
         with open(data_script_path, "wb") as f:
             f.write(requests.get(s3_path).content)
@@ -317,14 +336,24 @@
     # Ensure that the preview outputs directory always exists, and always starts off empty.
     # Contents from previous server sessions will be cleared.
     preview_outputs_directory = os.path.join(server_directory, "storage", "preview")
     if os.path.isdir(preview_outputs_directory):
         shutil.rmtree(preview_outputs_directory)
     os.mkdir(preview_outputs_directory)
 
+    template_directories = [
+        os.path.join(server_directory, "template"),
+        os.path.join(server_directory, "template", "aws"),
+        os.path.join(server_directory, "template", "aws", "eks"),
+    ]
+
+    for directory in template_directories:
+        if not os.path.isdir(directory):
+            os.mkdir(directory)
+
     server_version_file = os.path.join(server_directory, "__version__")
     if require_update(server_version_file):
         try:
             update_server_version()
             if is_tool(conda_cmd_prefix):
                 update_base_conda_environments()
         except Exception as e:
@@ -341,44 +370,65 @@
             raise Exception("Error executing command: %s" % args)
 
 
 def execute_command_nonblocking(args, cwd=None):
     return subprocess.Popen(args, stdout=sys.stdout, stderr=sys.stderr, cwd=cwd)
 
 
-def generate_welcome_message(expose, port):
+def get_address(expose):
     if not expose:
         expose_ip = "localhost"
     else:
         try:
-            expose_ip = requests.get(
+            ec2_ip = requests.get(
                 "http://169.254.169.254/latest/meta-data/public-ipv4", timeout=0.25
-            ).content.decode("utf-8")
+            )
+            if ec2_ip.status_code != 404: # User is in EC2 instance.
+                expose_ip = ec2_ip.content.decode("utf-8")
+            else:
+                # Assume is Google Cloud
+                metadata_flavor = {'Metadata-Flavor': 'Google'}
+                gcp_ip = requests.get('http://169.254.169.254/computeMetadata/v1/instance/network-interfaces/0/access-configs/0/external-ip', headers=metadata_flavor, timeout=0.25)
+                if gcp_ip.status_code != 404:
+                    expose_ip = gcp_ip.text
+                else:
+                    # Assume is Azure
+                    azure_ip = requests.get('http://169.254.169.254/metadata/instance/network/interface/0/ipv4/ipAddress/0/publicIpAddress?api-version=2017-08-01&format=text', headers={'Metadata': 'true'}, timeout=0.25)
+                    if azure_ip.status_code != 404:
+                        expose_ip = azure_ip.text
+                    else:
+                        # Default
+                        expose_ip = "<IP_ADDRESS>"
         except:  # If you're not running on EC2, this will return an error.
             expose_ip = "<IP_ADDRESS>"
 
+    return expose_ip
+
+
+def generate_welcome_message(addr, port):
     apikey = get_apikey()
+
     return (
-        welcome_message % (apikey, package_version, expose_ip, port, apikey),
-        login_url % (expose_ip, port, apikey),
+        welcome_message % (apikey, package_version, addr, port, apikey),
+        login_url % (addr, port, apikey),
     )
 
 
 def is_port_in_use(port: int) -> bool:
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         return s.connect_ex(("localhost", port)) == 0
 
 
 def cache_env(env):
     if env:
         with open(env_file_path, "w") as f:
             f.write(env)
 
 
-def start(expose, port, verbose, env, disable_usage_stats):
+def start(addr, expose, port, verbose, env, disable_usage_stats):
     update()
 
     if port is None:
         server_port = default_server_port
         while is_port_in_use(server_port):
             server_port += 1
         if not server_port == default_server_port:
@@ -394,45 +444,54 @@
 
     command = [
         os.path.join(server_directory, "bin", "server"),
         "--config",
         os.path.join(server_directory, "config", "config.yml"),
         "--port",
         str(server_port),
+        "--external-ip",
+        addr,
     ]
 
     if expose:
         command.append("--expose")
-    
+
     if verbose:
         command.append("--verbose")
 
     if disable_usage_stats:
         command.append("--disable-usage-stats")
 
     popen_handle = execute_command_nonblocking(command)
     return popen_handle, server_port
 
+
 def install_mongodb():
-    execute_command([sys.executable, "-m", "pip", "install", "pymongo"])
+    execute_command([sys.executable, "-m", "pip", "install", "pymongo%s" % PYMONGO_VERSION_BOUND])
+
 
 def install_postgres():
-    execute_command([sys.executable, "-m", "pip", "install", "psycopg2-binary"])
+    execute_command([sys.executable, "-m", "pip", "install", "psycopg2-binary%s" % PSYCOPG2_VERSION_BOUND])
+
 
 def install_bigquery():
-    execute_command([sys.executable, "-m", "pip", "install", "google-cloud-bigquery"])
+    execute_command([sys.executable, "-m", "pip", "install", "google-cloud-bigquery%s" % BIGQUERY_VERSION_BOUND])
+
 
 def install_snowflake():
-    execute_command([sys.executable, "-m", "pip", "install", "snowflake-sqlalchemy"])
+    execute_command([sys.executable, "-m", "pip", "install", "snowflake-sqlalchemy%s" % SNOWFLAKE_VERSION_BOUND])
+
 
 def install_s3():
-    execute_command([sys.executable, "-m", "pip", "install", "pyarrow"])
+    execute_command([sys.executable, "-m", "pip", "install", "pyarrow%s" % PYARROW_VERSION_BOUND])
+
 
 def install_athena():
-    execute_command([sys.executable, "-m", "pip", "install", "awswrangler"])
+    execute_command([sys.executable, "-m", "pip", "install", "awswrangler%s" % AWS_WRANGLER_VERSION_BOUND])
+
 
 def install_mysql():
     system = platform.system()
     if system == "Linux":
         if distro.id() == "ubuntu" or distro.id() == "debian":
             execute_command(
                 [
@@ -446,27 +505,35 @@
                 ]
             )
         elif distro.id() == "centos" or distro.id() == "rhel":
             execute_command(["sudo", "yum", "install", "-y", "python3-devel", "mysql-devel"])
         else:
             print("Unsupported distribution:", distro.id())
     elif system == "Darwin":
-        execute_command(["brew", "install", "mysql"])
+        cmd = ["brew", "install", "mysql"]
+        architecture = subprocess.Popen(
+            ["which", "-a", "brew"], stdout=subprocess.PIPE).communicate()[0]
+        # Using arm verison of brew
+        if architecture.startswith(b"/opt/homebrew"):
+            cmd = ["arch", "-arm64", *cmd]
+        execute_command(cmd)
     else:
         print("Unsupported operating system:", system)
 
-    execute_command([sys.executable, "-m", "pip", "install", "mysqlclient"])
-
+    execute_command(["pip", "install", "PyMySQL"])
+    execute_command([sys.executable, "-m", "pip", "install",
+                    "mysqlclient%s" % MYSQL_CLIENT_VERSION_BOUND])
 
 def install_sqlserver():
     system = platform.system()
     if system == "Linux":
         if distro.id() == "ubuntu":
             execute_command(
-                ["bash", os.path.join(server_directory, "bin", "install_sqlserver_ubuntu.sh")]
+                ["bash", os.path.join(
+                    server_directory, "bin", "install_sqlserver_ubuntu.sh")]
             )
         else:
             print("Unsupported distribution:", distro.id())
     elif system == "Darwin":
         execute_command(
             [
                 "brew",
@@ -485,15 +552,16 @@
                 "msodbcsql17",
                 "mssql-tools",
             ]
         )
     else:
         print("Unsupported operating system:", system)
 
-    execute_command([sys.executable, "-m", "pip", "install", "pyodbc"])
+    execute_command([sys.executable, "-m", "pip", "install",
+                    "pyodbc%s" % PYODBC_VERSION_BOUND])
 
 
 def install(system):
     if system == "postgres" or system == "redshift":
         install_postgres()
     elif system == "bigquery":
         install_bigquery()
@@ -632,17 +700,20 @@
     )
     install_args.add_argument(
         "system",
         nargs=1,
         help="Supported integrations: postgres, redshift, mysql, mariadb, sqlserver, azuresql, s3, athena, snowflake, bigquery.",
     )
 
-    apikey_args = subparsers.add_parser("apikey", help="Display your Aqueduct API key.")
-    clear_args = subparsers.add_parser("clear", help="Erase your Aqueduct installation.")
-    version_args = subparsers.add_parser("version", help="Retrieve the package version number.")
+    apikey_args = subparsers.add_parser(
+        "apikey", help="Display your Aqueduct API key.")
+    clear_args = subparsers.add_parser(
+        "clear", help="Erase your Aqueduct installation.")
+    version_args = subparsers.add_parser(
+        "version", help="Retrieve the package version number.")
 
     storage_args = subparsers.add_parser(
         "storage",
         help="""This changes the storage location for any new workflows created.
                                The change will take affect once you restart the Aqueduct server.
                                We are currently working on adding support for modifying the storage
                                location of existing workflows.
@@ -684,21 +755,30 @@
     )
 
     args = parser.parse_args()
     sysargs = sys.argv
 
     if args.command == "start":
         try:
-            popen_handle, server_port = start(args.expose, args.port, args.verbose, args.env, args.disable_usage_stats)
+            addr = get_address(args.expose)
+            popen_handle, server_port = start(
+                addr,
+                args.expose,
+                args.port,
+                args.verbose,
+                args.env,
+                args.disable_usage_stats,
+            )
             time.sleep(1)
             terminated = popen_handle.poll()
             if terminated:
                 print("Server terminated due to an error.")
             else:
-                welcome_message, url = generate_welcome_message(args.expose, server_port)
+                welcome_message, url = generate_welcome_message(
+                    addr, server_port)
                 print(welcome_message)
 
                 if not args.expose:
                     webbrowser.open(url)
                 popen_handle.wait()
         except (Exception, KeyboardInterrupt) as e:
             print(e)
@@ -706,15 +786,16 @@
             popen_handle.kill()
             print("Aqueduct service successfully terminated.")
     elif args.command == "server":
         print(
             "aqueduct ui and aqueduct server have been deprecated; please use aqueduct start to run both the UI and backend servers"
         )
     elif args.command == "install":
-        install(args.system[0])  # argparse makes this an array so only pass in value [0].
+        # argparse makes this an array so only pass in value [0].
+        install(args.system[0])
     elif args.command == "ui":
         print(
             "aqueduct ui and aqueduct server have been deprecated; please use aqueduct start to run both the UI and backend servers"
         )
     elif args.command == "apikey":
         apikey()
     elif args.command == "clear":
```

### Comparing `hstestaq-0.1.9/hstestaq.egg-info/PKG-INFO` & `hstestaq-0.2.11/hstestaq.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,94 @@
 Metadata-Version: 2.1
 Name: hstestaq
-Version: 0.1.9
+Version: 0.2.11
 Summary: Prediction Infrastructure for Data Scientists
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-[<img src="https://aqueduct-public-assets-bucket.s3.us-east-2.amazonaws.com/webapp/logos/aqueduct-logo-two-tone/1x/aqueduct-logo-two-tone-1x.png" width= "35%" />](https://www.aqueducthq.com)
 
-## Aqueduct: Orchestrate & manage production ML
 
+<div align="center">
+  <a href="https://aqueducthq.com">
+    <img src="https://aqueduct-public-assets-bucket.s3.us-east-2.amazonaws.com/webapp/logos/aqueduct-logo-two-tone/1x/aqueduct-logo-two-tone-1x.png" width= "40%" />
+  </a>
+  
+  <h2 style="border: none;">The control center for ML in the cloud</h2>
+
+### 📢 [Slack](https://slack.aqueducthq.com)&nbsp;&nbsp;|&nbsp;&nbsp;🗺️ [Roadmap](https://roadmap.aqueducthq.com)&nbsp;&nbsp;|&nbsp;&nbsp;🐞 [Report a bug](https://github.com/aqueducthq/aqueduct/issues/new?assignees=&labels=bug&template=bug_report.md&title=%5BBUG%5D)&nbsp;&nbsp;|&nbsp;&nbsp;✍️ [Blog](https://blog.aqueducthq.com)
+
+  
+  [![Start Sandbox](https://img.shields.io/static/v1?label=%20&logo=github&message=Start%20Sandbox&color=black)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=496844646)
 [![Downloads](https://pepy.tech/badge/aqueduct-ml/month)](https://pypi.org/project/aqueduct-ml/)
 [![Slack](https://img.shields.io/static/v1.svg?label=chat&message=on%20slack&color=27b1ff&style=flat)](https://join.slack.com/t/aqueductusers/shared_invite/zt-11hby91cx-cpmgfK0qfXqEYXv25hqD6A)
 [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/aqueducthq/aqueduct/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/aqueduct-ml.svg)](https://pypi.org/project/aqueduct-ml/)
 [![Tests](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml)
+</div>
+
+<h1></h1>
 
-**Aqueduct enables you to define, deploy and monitor robust ML pipelines on any cloud infrastructure.** Check out our [quickstart guide](https://docs.aqueducthq.com/quickstart-guide)!
+**Aqueduct enables you to easily define, run, and manage AI & ML tasks on any cloud infrastructure. [Check out our quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
-Aqueduct gives you a simple Python-native API to define machine learning pipelines, the ability to deploy those pipelines on your existing infrastructure (e.g., Spark, Kubernetes, Lambda), and visibility into the code, data, and metadata associated with your workflows. 
-Aqueduct is fully open-source and runs securely in your cloud.
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/867892/230214641-b0aec53b-4988-4581-84ed-134f97ed9276.png" width="80%" />
+</p>
+
+Aqueduct is an open-source MLOps framework that allows you to write code in vanilla Python, run that code on any cloud infrastructure you'd like to use, and gain visibility into the execution and performance of your models and predictions. **[See what infrastructure Aqueduct works with. →](https://aqueducthq.com/integrations/)**
+
+Here's how you can get started: 
 
-You can install Aqueduct via `pip`:
 ```bash
 pip3 install aqueduct-ml
 aqueduct start
 ```
 
-Now, we can create our first workflow:
-
-```python
-from aqueduct import Client, op, metric
-
-client = Client()
-
-@op
-def transform_data(reviews):
-    reviews['strlen'] = reviews['review'].str.len()
-    return reviews
+### How it works
 
+Aqueduct's Python native API allows you to define ML tasks in regular Python code. You can connect Aqueduct to your existing cloud infrastructure ([docs](https://docs.aqueducthq.com/integrations)), and Aqueduct will seamlessly move your code from your laptop to the cloud or between different cloud infrastructure layers. 
 
-demo_db = client.integration("aqueduct_demo")
-reviews_table = demo_db.sql("select * from hotel_reviews;")
+<!--- TODO(vikram): Modify this once we add support for switching into/out of Databricks in a single workflow. --->
+For example, we can define a pipeline that trains a model on Kubernetes using a GPU and validates that model in AWS Lambda in a few lines of Python: 
 
-strlen_table = transform_data(reviews_table)
-strlen_table.save(demo_db.config(table="strlen_table", update_mode="replace")) 
+```python
+@op(
+  engine='eks-us-east-2', 
+  resources={'gpu_resource_name': 'nvidia.com/gpu'}
+)
+def train(features):
+  return model.train(features)
+
+@metric(engine='lambda-us-east-2')
+def validate(model):
+    return validation_test(model)
 
-client.publish_flow(name="review_strlen", artifacts=[strlen_table])
+validate(train(features))
 ```
 
-Once we've created a workflow, we can view that workflow in the Aqueduct UI: 
+Once you publish this workflow to Aqueduct, you can see it on the UI: 
+
+![image](https://user-images.githubusercontent.com/867892/228295996-4ba3de23-3106-431d-93a9-afd8d77a707b.png)
 
-![image](https://user-images.githubusercontent.com/867892/196529730-3c9582d5-8692-495d-a7df-8eb62ddf305f.png)
+To see how to build your first workflow, check out our **[quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
 ## Why Aqueduct?
 
-The engineering required to get data science & machine learning projects in production slows down data teams. Aqueduct automates away that engineering and allows you to define robust data & ML pipelines in a few lines of code and run them anywhere.
+MLOps has become a [tangled mess of siloed infrastructure](https://aqueducthq.com/post/the-mlops-knot/). Most teams need to set up and operate many different cloud infrastructure tools to run ML effectively, but these tools have disparate APIs and interoperate poorly.
+
+Aqueduct provides a single interface to running machine learning tasks on your existing cloud infrastructure — Kubernetes, Spark, Lambda, etc. From the same Python API, you can run code across any or all of these systems seamlessly and gain visibility into how your code is performing.
 
 * **Python-native pipeline API**: Aqueduct’s API allows you define your workflows in vanilla Python, so you can get code into production quickly and effectively. No more DSLs or YAML configs to worry about.
 * **Integrated with your infrastructure**: Workflows defined in Aqueduct can run on any cloud infrastructure you use, like Kubernetes, Spark, Airflow, or AWS Lambda. You can get all the benefits of Aqueduct without having to rip-and-replace your existing tooling.
 * **Centralized visibility into code, data, & metadata**: Once your workflows are in production, you need to know what’s running, whether it’s working, and when it breaks. Aqueduct gives you visibility into what code, data, metrics, and metadata are generated by each workflow run, so you can have confidence that your pipelines work as expected — and know immediately when they don’t.
-* **Runs securely in your cloud**: Aqueduct is fully open-source and runs in any Unix environment. It runs entirely in your cloud and on your infrastructure, so you can be confident that nothing is ever leaving your cloud.
+* **Runs securely in your cloud**: Aqueduct is fully open-source and runs in any Unix environment. It runs entirely in your cloud and on your infrastructure, so you can be confident that your data and code are secure.
 
 ## Overview & Examples
 
 The core abstraction in Aqueduct is a [Workflow](https://docs.aqueducthq.com/workflows), which is a sequence of [Artifacts](https://docs.aqueducthq.com/artifacts) (data) that are transformed by [Operators](https://docs.aqueducthq.com/operators) (compute). 
 The input Artifact(s) for a Workflow is typically loaded from a database, and the output Artifact(s) are typically persisted back to a database. 
 Each Workflow can either be run on a fixed schedule or triggered on-demand.
 
@@ -87,8 +107,8 @@
 * and more details on [creating workflows](https://docs.aqueducthq.com/workflows)
 
 If you have questions or comments or would like to learn more about what we're
 building, please [reach out](mailto:hello@aqueducthq.com), [join our Slack
 channel](https://join.slack.com/t/aqueductusers/shared_invite/zt-11hby91cx-cpmgfK0qfXqEYXv25hqD6A), or [start a conversation on GitHub](https://github.com/aqueducthq/aqueduct/issues/new).
 We'd love to hear from you!
 
-If you're interested in contributing, please check out our [roadmap](https://github.com/aqueducthq/aqueduct/wiki/Aqueduct-Roadmap) and join the development channel in [our community Slack](https://slack.aqueducthq.com).
+If you're interested in contributing, please check out our [roadmap](https://roadmap.aqueducthq.com) and join the development channel in [our community Slack](https://slack.aqueducthq.com).
```

### Comparing `hstestaq-0.1.9/hstestaq.egg-info/SOURCES.txt` & `hstestaq-0.2.11/hstestaq.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,32 +27,35 @@
 aqueduct_executor/operators/connectors/data/athena.py
 aqueduct_executor/operators/connectors/data/azure_sql.py
 aqueduct_executor/operators/connectors/data/bigquery.py
 aqueduct_executor/operators/connectors/data/common.py
 aqueduct_executor/operators/connectors/data/config.py
 aqueduct_executor/operators/connectors/data/connector.py
 aqueduct_executor/operators/connectors/data/execute.py
-aqueduct_executor/operators/connectors/data/execute_spark.py
 aqueduct_executor/operators/connectors/data/extract.py
 aqueduct_executor/operators/connectors/data/gcs.py
 aqueduct_executor/operators/connectors/data/load.py
 aqueduct_executor/operators/connectors/data/main.py
 aqueduct_executor/operators/connectors/data/maria_db.py
 aqueduct_executor/operators/connectors/data/models.py
 aqueduct_executor/operators/connectors/data/mongodb.py
 aqueduct_executor/operators/connectors/data/mysql.py
 aqueduct_executor/operators/connectors/data/postgres.py
 aqueduct_executor/operators/connectors/data/redshift.py
 aqueduct_executor/operators/connectors/data/relational.py
 aqueduct_executor/operators/connectors/data/s3.py
+aqueduct_executor/operators/connectors/data/s3_serialization.py
 aqueduct_executor/operators/connectors/data/snowflake.py
 aqueduct_executor/operators/connectors/data/spec.py
 aqueduct_executor/operators/connectors/data/sql_server.py
 aqueduct_executor/operators/connectors/data/sqlite.py
 aqueduct_executor/operators/connectors/data/utils.py
+aqueduct_executor/operators/connectors/data/spark/__init__.py
+aqueduct_executor/operators/connectors/data/spark/s3.py
+aqueduct_executor/operators/connectors/data/spark/snowflake.py
 aqueduct_executor/operators/connectors/tests/__init__.py
 aqueduct_executor/operators/connectors/tests/conf.py
 aqueduct_executor/operators/connectors/tests/conftest.py
 aqueduct_executor/operators/connectors/tests/test_bigquery.py
 aqueduct_executor/operators/connectors/tests/test_mariadb.py
 aqueduct_executor/operators/connectors/tests/test_mysql.py
 aqueduct_executor/operators/connectors/tests/test_postgres.py
@@ -70,14 +73,18 @@
 aqueduct_executor/operators/function_executor/set_conda_version.py
 aqueduct_executor/operators/function_executor/spec.py
 aqueduct_executor/operators/function_executor/utils.py
 aqueduct_executor/operators/param_executor/__init__.py
 aqueduct_executor/operators/param_executor/execute.py
 aqueduct_executor/operators/param_executor/main.py
 aqueduct_executor/operators/param_executor/spec.py
+aqueduct_executor/operators/spark/__init__.py
+aqueduct_executor/operators/spark/execute_data.py
+aqueduct_executor/operators/spark/execute_function.py
+aqueduct_executor/operators/spark/utils.py
 aqueduct_executor/operators/system_metric_executor/__init__.py
 aqueduct_executor/operators/system_metric_executor/execute.py
 aqueduct_executor/operators/system_metric_executor/main.py
 aqueduct_executor/operators/system_metric_executor/spec.py
 aqueduct_executor/operators/utils/__init__.py
 aqueduct_executor/operators/utils/enums.py
 aqueduct_executor/operators/utils/exceptions.py
```

### Comparing `hstestaq-0.1.9/setup.py` & `hstestaq-0.2.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = open("requirements.txt").read().strip().split("\n")
 
 readme_path = Path(os.environ["PWD"], "../../README.md")
 long_description = open(readme_path).read()
 
 setup(
     name="hstestaq",
-    version="0.1.9",
+    version="0.2.11",
     install_requires=install_requires,
     scripts=["bin/aqueduct"],
     packages=find_packages(),
     description="Prediction Infrastructure for Data Scientists",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.aqueducthq.com/",
```

