# Comparing `tmp/macrometa-target-bigquery-0.0.6.tar.gz` & `tmp/macrometa-target-bigquery-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-bigquery-0.0.6.tar", last modified: Mon Apr 17 09:52:21 2023, max compression
+gzip compressed data, was "macrometa-target-bigquery-0.0.7.tar", last modified: Thu Apr 20 10:26:20 2023, max compression
```

## Comparing `macrometa-target-bigquery-0.0.6.tar` & `macrometa-target-bigquery-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:21.513465 macrometa-target-bigquery-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-17 09:52:21.513465 macrometa-target-bigquery-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:21.513465 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)    29849 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/db_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/flattening.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/stream_ref_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:21.513465 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-17 09:52:21.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 09:52:21.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:52:21.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 09:52:21.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-17 09:52:21.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 09:52:21.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:52:21.513465 macrometa-target-bigquery-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:26:20.417810 macrometa-target-bigquery-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-20 10:26:20.417810 macrometa-target-bigquery-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:26:20.417810 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)    29847 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/db_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/flattening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/stream_ref_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:26:20.417810 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-20 10:26:20.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-20 10:26:20.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:26:20.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-20 10:26:20.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-20 10:26:20.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 10:26:20.000000 macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:26:20.417810 macrometa-target-bigquery-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-20 10:26:00.000000 macrometa-target-bigquery-0.0.7/setup.py
```

### Comparing `macrometa-target-bigquery-0.0.6/LICENSE` & `macrometa-target-bigquery-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.6/PKG-INFO` & `macrometa-target-bigquery-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-bigquery
-Version: 0.0.6
+Version: 0.0.7
 Summary: Macrometa target bigquery connector for loading data to BigQuery
 Home-page: https://github.com/Macrometacorp/macrometa-target-bigquery
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-target-bigquery-0.0.6/README.md` & `macrometa-target-bigquery-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/__init__.py` & `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     def config(self) -> list[ConfigProperty]:
         """Get configuration parameters for the connector."""
         return [
             ConfigProperty('project_id', 'Project ID', ConfigAttributeType.STRING, True, False,
                            description='BigQuery project ID.',
                            placeholder_value='my_project_id'),
-            ConfigProperty('credentials_file', 'Credentials JSON file', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('credentials_file', 'Credentials JSON file', ConfigAttributeType.FILE, True, False,
                            description='Fully qualified path to client_secrets.json for your service account. See the '
                                        '"Activate the Google BigQuery API" section of the repository\'s README and '
                                        'https://cloud.google.com/docs/authentication/production.',
                            placeholder_value='credentials.json contents'),
             ConfigProperty('target_schema', 'Target Schema/Dataset', ConfigAttributeType.STRING, True, False,
                            description='Name of the schema/dataset where the tables will be created.'),
             ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, False,
```

### Comparing `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/db_sync.py` & `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/db_sync.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/exceptions.py` & `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/flattening.py` & `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/flattening.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/sql_utils.py` & `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/sql_utils.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/stream_ref_helper.py` & `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/stream_ref_helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/stream_utils.py` & `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery/stream_utils.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/PKG-INFO` & `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-bigquery
-Version: 0.0.6
+Version: 0.0.7
 Summary: Macrometa target bigquery connector for loading data to BigQuery
 Home-page: https://github.com/Macrometacorp/macrometa-target-bigquery
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/SOURCES.txt` & `macrometa-target-bigquery-0.0.7/macrometa_target_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.6/setup.py` & `macrometa-target-bigquery-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name="macrometa-target-bigquery",
-      version='0.0.6',
+      version='0.0.7',
       description="Macrometa target bigquery connector for loading data to BigQuery",
       long_description=long_description,
       long_description_content_type='text/markdown',
       author="Macrometa",
       url='https://github.com/Macrometacorp/macrometa-target-bigquery',
       classifiers=[
           'License :: OSI Approved :: Apache Software License',
```

