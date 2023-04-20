# Comparing `tmp/macrometa-source-postgres-0.0.43.tar.gz` & `tmp/macrometa-source-postgres-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-postgres-0.0.43.tar", max compression
+gzip compressed data, was "macrometa-source-postgres-0.0.44.tar", max compression
```

## Comparing `macrometa-source-postgres-0.0.43.tar` & `macrometa-source-postgres-0.0.44.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11899 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/LICENSE
--rw-r--r--   0        0        0    35128 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/__init__.py
--rw-r--r--   0        0        0     8580 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/connection.py
--rw-r--r--   0        0        0    20349 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/helper.py
--rw-r--r--   0        0        0        0 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/common.py
--rw-r--r--   0        0        0     8974 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/full_table.py
--rw-r--r--   0        0        0    28921 2023-04-19 07:19:31.330522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/log_based.py
--rw-r--r--   0        0        0     3698 2023-04-19 07:19:31.334522 macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1512 2023-04-19 07:19:31.582520 macrometa-source-postgres-0.0.43/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.43/setup.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.43/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-04-20 05:38:16.566442 macrometa-source-postgres-0.0.44/LICENSE
+-rw-r--r--   0        0        0    35128 2023-04-20 05:38:16.566442 macrometa-source-postgres-0.0.44/macrometa_source_postgres/__init__.py
+-rw-r--r--   0        0        0     8580 2023-04-20 05:38:16.566442 macrometa-source-postgres-0.0.44/macrometa_source_postgres/connection.py
+-rw-r--r--   0        0        0    20349 2023-04-20 05:38:16.566442 macrometa-source-postgres-0.0.44/macrometa_source_postgres/helper.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:38:16.566442 macrometa-source-postgres-0.0.44/macrometa_source_postgres/sync_strategies/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-20 05:38:16.566442 macrometa-source-postgres-0.0.44/macrometa_source_postgres/sync_strategies/common.py
+-rw-r--r--   0        0        0     9290 2023-04-20 05:38:16.566442 macrometa-source-postgres-0.0.44/macrometa_source_postgres/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    28921 2023-04-20 05:38:16.566442 macrometa-source-postgres-0.0.44/macrometa_source_postgres/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     3698 2023-04-20 05:38:16.566442 macrometa-source-postgres-0.0.44/macrometa_source_postgres/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1512 2023-04-20 05:38:16.810444 macrometa-source-postgres-0.0.44/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.44/setup.py
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.44/PKG-INFO
```

### Comparing `macrometa-source-postgres-0.0.43/LICENSE` & `macrometa-source-postgres-0.0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.43/macrometa_source_postgres/__init__.py` & `macrometa-source-postgres-0.0.44/macrometa_source_postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.43/macrometa_source_postgres/connection.py` & `macrometa-source-postgres-0.0.44/macrometa_source_postgres/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.43/macrometa_source_postgres/helper.py` & `macrometa-source-postgres-0.0.44/macrometa_source_postgres/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/common.py` & `macrometa-source-postgres-0.0.44/macrometa_source_postgres/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/full_table.py` & `macrometa-source-postgres-0.0.44/macrometa_source_postgres/sync_strategies/full_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,22 @@
     :param dict state: dictionary representing the state of the replication process
     :param list desired_columns: list of desired columns for the table
     :param dict md_map: dictionary mapping metadata to the relevant stream
     :return: updated state dictionary representing the state of the replication process
     """
     time_extracted = utils.now()
 
+    #TODO: remove this test
+    print(f"Current state: {state}")
+    print("Logging state message")
+    state = singer.write_bookmark(state, "state-test", 'version', '1000')
+    singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
+    print("Logged state message")
+    print(f"New state: {state}")
+
     # check the version if it already exists
     first_run = singer.get_bookmark(state, stream['tap_stream_id'], 'version') is None
 
     # xmin indicates that we were interrupted last time
     if singer.get_bookmark(state, stream['tap_stream_id'], 'xmin') is None:
         nascent_stream_version = int(time.time() * 1000)
     else:
```

### Comparing `macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/log_based.py` & `macrometa-source-postgres-0.0.44/macrometa_source_postgres/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.43/macrometa_source_postgres/sync_strategies/sample_data.py` & `macrometa-source-postgres-0.0.44/macrometa_source_postgres/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.43/pyproject.toml` & `macrometa-source-postgres-0.0.44/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-postgres"
-version='0.0.43'
+version='0.0.44'
 description = "Macrometa Source for extracting data from PostgreSQL."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-postgres-0.0.43/setup.py` & `macrometa-source-postgres-0.0.44/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-postgres = '
                      'macrometa_source_postgres:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-postgres',
-    'version': '0.0.43',
+    'version': '0.0.44',
     'description': 'Macrometa Source for extracting data from PostgreSQL.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-postgres-0.0.43/PKG-INFO` & `macrometa-source-postgres-0.0.44/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-postgres
-Version: 0.0.43
+Version: 0.0.44
 Summary: Macrometa Source for extracting data from PostgreSQL.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,PostgreSQL,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

