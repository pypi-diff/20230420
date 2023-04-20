# Comparing `tmp/devex_sdk-1.0.0b1.tar.gz` & `tmp/devex_sdk-1.0.0b18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devex_sdk-1.0.0b1.tar", last modified: Thu Apr 20 17:06:51 2023, max compression
+gzip compressed data, was "devex_sdk-1.0.0b18.tar", last modified: Thu Apr 20 19:47:49 2023, max compression
```

## Comparing `devex_sdk-1.0.0b1.tar` & `devex_sdk-1.0.0b18.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.371764 devex_sdk-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-20 17:06:51.371764 devex_sdk-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.363764 devex_sdk-1.0.0b1/devex_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/add.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.363764 devex_sdk-1.0.0b1/devex_sdk/bucketization/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/bucketization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/bucketization/bucketization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.363764 devex_sdk-1.0.0b1/devex_sdk/circles/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/circles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/circles/circles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.363764 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.367764 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/Cluster.json
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/ClusterService.json
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/Container.json
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/ContainerFS.json
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/Node.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/NodeDiskIO.json
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/NodeFS.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/NodeNet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/Pod.json
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/PodNet.json
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/eks_raw_pyspark_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/eks_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/gz_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/nested_json_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/pandas_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/spark_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/spark_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/data_ingestion/spark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.367764 devex_sdk-1.0.0b1/devex_sdk/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/extras/divide.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/extras/multiply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.367764 devex_sdk-1.0.0b1/devex_sdk/feature_engine/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/feature_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.367764 devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/container_autoencoder_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/container_pca_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/node_autoencoder_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/node_hmm_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/node_pca_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/pod_autoencoder_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/pod_pca_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/pytest_autoencoder_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/pytest_pca_ad_features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/feature_engine/feature_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.367764 devex_sdk-1.0.0b1/devex_sdk/parity/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/parity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/parity/number_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.367764 devex_sdk-1.0.0b1/devex_sdk/project_inital_setup/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/project_inital_setup/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/project_inital_setup/console_setup_run.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      346 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/project_inital_setup/notebook_setup_run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/project_inital_setup/understanding_eks_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.367764 devex_sdk-1.0.0b1/devex_sdk/update_cwd/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/update_cwd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/devex_sdk/update_cwd/notebook_setup_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.363764 devex_sdk-1.0.0b1/devex_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-20 17:06:51.000000 devex_sdk-1.0.0b1/devex_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-20 17:06:51.000000 devex_sdk-1.0.0b1/devex_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:06:51.000000 devex_sdk-1.0.0b1/devex_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 17:06:51.000000 devex_sdk-1.0.0b1/devex_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 17:06:51.000000 devex_sdk-1.0.0b1/devex_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 17:06:51.371764 devex_sdk-1.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:51.371764 devex_sdk-1.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/tests/test_circles.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/tests/test_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/tests/test_dataframe_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/tests/test_divide.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/tests/test_eks_bucketization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/tests/test_gz_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/tests/test_multiply.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/tests/test_parity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/tests/test_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-20 17:06:39.000000 devex_sdk-1.0.0b1/tests/test_update_cwd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.429793 devex_sdk-1.0.0b18/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-20 19:47:49.429793 devex_sdk-1.0.0b18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.413793 devex_sdk-1.0.0b18/devex_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/add.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.413793 devex_sdk-1.0.0b18/devex_sdk/bucketization/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/bucketization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/bucketization/bucketization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.417793 devex_sdk-1.0.0b18/devex_sdk/circles/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/circles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/circles/circles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.417793 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.421793 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/Cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/ClusterService.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/Container.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/ContainerFS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/Node.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/NodeDiskIO.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/NodeFS.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/NodeNet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/Pod.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/PodNet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/eks_raw_pyspark_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/eks_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/gz_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/nested_json_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/pandas_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/spark_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/spark_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/data_ingestion/spark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.421793 devex_sdk-1.0.0b18/devex_sdk/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/extras/divide.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/extras/multiply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.421793 devex_sdk-1.0.0b18/devex_sdk/feature_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/feature_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.425793 devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/container_autoencoder_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/container_pca_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/node_autoencoder_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/node_hmm_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/node_pca_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/pod_autoencoder_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/pod_pca_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/pytest_autoencoder_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/pytest_pca_ad_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/feature_engine/feature_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.425793 devex_sdk-1.0.0b18/devex_sdk/parity/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/parity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/parity/number_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.425793 devex_sdk-1.0.0b18/devex_sdk/project_inital_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/project_inital_setup/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/project_inital_setup/console_setup_run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      346 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/project_inital_setup/notebook_setup_run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/project_inital_setup/understanding_eks_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.425793 devex_sdk-1.0.0b18/devex_sdk/update_cwd/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/update_cwd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/devex_sdk/update_cwd/notebook_setup_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.413793 devex_sdk-1.0.0b18/devex_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-20 19:47:49.000000 devex_sdk-1.0.0b18/devex_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-20 19:47:49.000000 devex_sdk-1.0.0b18/devex_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:47:49.000000 devex_sdk-1.0.0b18/devex_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 19:47:49.000000 devex_sdk-1.0.0b18/devex_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 19:47:49.000000 devex_sdk-1.0.0b18/devex_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:47:49.429793 devex_sdk-1.0.0b18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:47:49.429793 devex_sdk-1.0.0b18/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/tests/test_circles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/tests/test_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/tests/test_dataframe_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/tests/test_divide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/tests/test_eks_bucketization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/tests/test_gz_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/tests/test_multiply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/tests/test_parity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/tests/test_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-20 19:47:37.000000 devex_sdk-1.0.0b18/tests/test_update_cwd.py
```

### Comparing `devex_sdk-1.0.0b1/LICENSE.txt` & `devex_sdk-1.0.0b18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/PKG-INFO` & `devex_sdk-1.0.0b18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devex_sdk
-Version: 1.0.0b1
+Version: 1.0.0b18
 Summary: Dish DevEx open source SDK
 Home-page: https://git-codecommit.us-west-2.amazonaws.com/v1/repos/devex_sdk
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `devex_sdk-1.0.0b1/README.md` & `devex_sdk-1.0.0b18/README.md`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/__init__.py` & `devex_sdk-1.0.0b18/devex_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/bucketization/bucketization.py` & `devex_sdk-1.0.0b18/devex_sdk/bucketization/bucketization.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/circles/circles.py` & `devex_sdk-1.0.0b18/devex_sdk/circles/circles.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/Cluster.json` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/Cluster.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/ClusterNamespace.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/ClusterService.json` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/ClusterService.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/Container.json` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/Container.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/ContainerFS.json` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/ContainerFS.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/Node.json` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/Node.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/NodeDiskIO.json` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/NodeDiskIO.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/NodeFS.json` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/NodeFS.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/NodeNet.json` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/NodeNet.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/Pod.json` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/Pod.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/PodNet.json` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/PodNet.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/container_insights_schema/eks_raw_pyspark_schema.py` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/container_insights_schema/eks_raw_pyspark_schema.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/eks_connector.py` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/eks_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/gz_connector.py` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/gz_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/nested_json_connector.py` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/nested_json_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/pandas_data_connector.py` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/pandas_data_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/spark_config.ini` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/spark_config.ini`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/spark_data_connector.py` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/spark_data_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/data_ingestion/spark_utils.py` & `devex_sdk-1.0.0b18/devex_sdk/data_ingestion/spark_utils.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/container_autoencoder_ad_features.json` & `devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/container_autoencoder_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/container_pca_ad_features.json` & `devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/container_pca_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/node_autoencoder_ad_features.json` & `devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/node_autoencoder_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/node_hmm_ad_features.json` & `devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/node_hmm_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/node_pca_ad_features.json` & `devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/node_pca_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/pod_autoencoder_ad_features.json` & `devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/pod_autoencoder_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/pod_pca_ad_features.json` & `devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/pod_pca_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/pytest_autoencoder_ad_features.json` & `devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/pytest_autoencoder_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/feature_engine/eks_feature_store/pytest_pca_ad_features.json` & `devex_sdk-1.0.0b18/devex_sdk/feature_engine/eks_feature_store/pytest_pca_ad_features.json`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/feature_engine/feature_extractor.py` & `devex_sdk-1.0.0b18/devex_sdk/feature_engine/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/project_inital_setup/understanding_eks_setup.py` & `devex_sdk-1.0.0b18/devex_sdk/project_inital_setup/understanding_eks_setup.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk/update_cwd/notebook_setup_path.py` & `devex_sdk-1.0.0b18/devex_sdk/update_cwd/notebook_setup_path.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/devex_sdk.egg-info/PKG-INFO` & `devex_sdk-1.0.0b18/devex_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devex-sdk
-Version: 1.0.0b1
+Version: 1.0.0b18
 Summary: Dish DevEx open source SDK
 Home-page: https://git-codecommit.us-west-2.amazonaws.com/v1/repos/devex_sdk
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `devex_sdk-1.0.0b1/devex_sdk.egg-info/SOURCES.txt` & `devex_sdk-1.0.0b18/devex_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/setup.py` & `devex_sdk-1.0.0b18/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
-    name = 'devex_sdk',
-    version = 'v1.0.0-beta1',
-    description = 'Dish DevEx open source SDK',
-    url = 'https://git-codecommit.us-west-2.amazonaws.com/v1/repos/devex_sdk',
-    author_email = 'devex@dish.com',
+    name='devex_sdk',
+    version='v1.0.0-beta-18',
+    description='Dish DevEx open source SDK',
+    url='https://git-codecommit.us-west-2.amazonaws.com/v1/repos/devex_sdk',
+    author_email='devex@dish.com',
     license='Dish Wireless',
     packages=find_packages(
         include=['devex_sdk',
                  'devex_sdk.extras',
                  'devex_sdk.circles',
                  'devex_sdk.parity',
                  'devex_sdk.bucketization',
@@ -29,15 +29,15 @@
                  'devex_sdk.feature_engine.eks_feature_store',
                  'devex_sdk.feature_engine',
                  'devex_sdk.data_ingestion.gz_connector',
                  'devex_sdk.utilities'
         ]
     ),
     include_package_data=True,
-    install_requires = [
+    install_requires=[
         'pyspark',
         'pandas',
         'numpy',
         'tqdm',
         'pyspark',
         'configparser',
         'dask',
```

### Comparing `devex_sdk-1.0.0b1/tests/test_counts.py` & `devex_sdk-1.0.0b18/tests/test_counts.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/tests/test_dataframe_creation.py` & `devex_sdk-1.0.0b18/tests/test_dataframe_creation.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/tests/test_eks_bucketization.py` & `devex_sdk-1.0.0b18/tests/test_eks_bucketization.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/tests/test_gz_connector.py` & `devex_sdk-1.0.0b18/tests/test_gz_connector.py`

 * *Files identical despite different names*

### Comparing `devex_sdk-1.0.0b1/tests/test_schema.py` & `devex_sdk-1.0.0b18/tests/test_schema.py`

 * *Files identical despite different names*

