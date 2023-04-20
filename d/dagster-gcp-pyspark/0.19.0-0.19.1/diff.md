# Comparing `tmp/dagster_gcp_pyspark-0.19.0.tar.gz` & `tmp/dagster_gcp_pyspark-0.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_gcp_pyspark-0.19.0.tar", last modified: Wed Apr 19 19:13:30 2023, max compression
+gzip compressed data, was "dagster_gcp_pyspark-0.19.1.tar", last modified: Thu Apr 20 20:49:59 2023, max compression
```

## Comparing `dagster_gcp_pyspark-0.19.0.tar` & `dagster_gcp_pyspark-0.19.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:13:30.183459 dagster_gcp_pyspark-0.19.0/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-04-19 19:01:30.000000 dagster_gcp_pyspark-0.19.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-19 19:01:30.000000 dagster_gcp_pyspark-0.19.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      649 2023-04-19 19:13:30.183459 dagster_gcp_pyspark-0.19.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      143 2023-04-19 19:01:30.000000 dagster_gcp_pyspark-0.19.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:13:30.183459 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark/
--rw-r--r--   0 root         (0) root         (0)      402 2023-04-19 19:01:30.000000 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:13:30.183459 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9884 2023-04-19 19:01:30.000000 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-19 19:01:30.000000 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-19 19:01:30.000000 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:13:30.183459 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      649 2023-04-19 19:13:30.000000 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2023-04-19 19:13:30.000000 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:13:30.000000 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:13:30.000000 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-19 19:13:30.000000 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-19 19:13:30.000000 dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-19 19:13:30.187459 dagster_gcp_pyspark-0.19.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1366 2023-04-19 19:01:30.000000 dagster_gcp_pyspark-0.19.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:49:59.520701 dagster_gcp_pyspark-0.19.1/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-04-20 20:39:02.000000 dagster_gcp_pyspark-0.19.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-20 20:39:02.000000 dagster_gcp_pyspark-0.19.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      649 2023-04-20 20:49:59.520701 dagster_gcp_pyspark-0.19.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      143 2023-04-20 20:39:02.000000 dagster_gcp_pyspark-0.19.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:49:59.516701 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-04-20 20:39:02.000000 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:49:59.520701 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9884 2023-04-20 20:39:02.000000 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-20 20:39:02.000000 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-20 20:39:02.000000 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:49:59.520701 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-04-20 20:49:59.000000 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2023-04-20 20:49:59.000000 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:49:59.000000 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:49:59.000000 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 20:49:59.000000 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-20 20:49:59.000000 dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-04-20 20:49:59.520701 dagster_gcp_pyspark-0.19.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-04-20 20:39:02.000000 dagster_gcp_pyspark-0.19.1/setup.py
```

### Comparing `dagster_gcp_pyspark-0.19.0/LICENSE` & `dagster_gcp_pyspark-0.19.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_gcp_pyspark-0.19.0/PKG-INFO` & `dagster_gcp_pyspark-0.19.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_gcp_pyspark
-Version: 0.19.0
+Version: 0.19.1
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py` & `dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster_gcp_pyspark-0.19.0/dagster_gcp_pyspark.egg-info/PKG-INFO` & `dagster_gcp_pyspark-0.19.1/dagster_gcp_pyspark.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pyspark
-Version: 0.19.0
+Version: 0.19.1
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster_gcp_pyspark-0.19.0/setup.py` & `dagster_gcp_pyspark-0.19.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pyspark_tests*"]),
     install_requires=[
-        "dagster==1.3.0",
-        "dagster-gcp==0.19.0",
+        "dagster==1.3.1",
+        "dagster-gcp==0.19.1",
         "pyspark",
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

