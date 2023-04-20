# Comparing `tmp/batch_ingestion_client_py-1.0.1.tar.gz` & `tmp/batch_ingestion_client_py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch_ingestion_client_py-1.0.1.tar", last modified: Thu Apr 20 14:11:22 2023, max compression
+gzip compressed data, was "batch_ingestion_client_py-1.0.2.tar", last modified: Thu Apr 20 14:13:10 2023, max compression
```

## Comparing `batch_ingestion_client_py-1.0.1.tar` & `batch_ingestion_client_py-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-20 14:11:22.538839 batch_ingestion_client_py-1.0.1/
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     4077 2023-04-20 14:11:22.538839 batch_ingestion_client_py-1.0.1/PKG-INFO
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     3441 2023-04-20 13:20:45.000000 batch_ingestion_client_py-1.0.1/README.md
-drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-20 14:11:22.534839 batch_ingestion_client_py-1.0.1/batch_ingestion_client_py/
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      265 2023-04-20 14:08:41.000000 batch_ingestion_client_py-1.0.1/batch_ingestion_client_py/__init__.py
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     5750 2023-04-20 13:08:39.000000 batch_ingestion_client_py-1.0.1/batch_ingestion_client_py/data.py
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      642 2023-04-20 14:08:52.000000 batch_ingestion_client_py-1.0.1/batch_ingestion_client_py/main.py
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1422 2023-04-20 13:08:18.000000 batch_ingestion_client_py-1.0.1/batch_ingestion_client_py/response.py
-drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-20 14:11:22.538839 batch_ingestion_client_py-1.0.1/batch_ingestion_client_py.egg-info/
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     4077 2023-04-20 14:11:22.000000 batch_ingestion_client_py-1.0.1/batch_ingestion_client_py.egg-info/PKG-INFO
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      406 2023-04-20 14:11:22.000000 batch_ingestion_client_py-1.0.1/batch_ingestion_client_py.egg-info/SOURCES.txt
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)        1 2023-04-20 14:11:22.000000 batch_ingestion_client_py-1.0.1/batch_ingestion_client_py.egg-info/dependency_links.txt
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)        9 2023-04-20 14:11:22.000000 batch_ingestion_client_py-1.0.1/batch_ingestion_client_py.egg-info/requires.txt
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)       26 2023-04-20 14:11:22.000000 batch_ingestion_client_py-1.0.1/batch_ingestion_client_py.egg-info/top_level.txt
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)       38 2023-04-20 14:11:22.538839 batch_ingestion_client_py-1.0.1/setup.cfg
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1102 2023-04-20 14:11:07.000000 batch_ingestion_client_py-1.0.1/setup.py
+drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-20 14:13:10.418461 batch_ingestion_client_py-1.0.2/
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     4092 2023-04-20 14:13:10.418461 batch_ingestion_client_py-1.0.2/PKG-INFO
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     3456 2023-04-20 14:12:30.000000 batch_ingestion_client_py-1.0.2/README.md
+drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-20 14:13:10.414461 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      265 2023-04-20 14:08:41.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/__init__.py
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     5750 2023-04-20 13:08:39.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/data.py
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      642 2023-04-20 14:08:52.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/main.py
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1422 2023-04-20 13:08:18.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/response.py
+drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-20 14:13:10.418461 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     4092 2023-04-20 14:13:10.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/PKG-INFO
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      406 2023-04-20 14:13:10.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)        1 2023-04-20 14:13:10.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)        9 2023-04-20 14:13:10.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/requires.txt
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)       26 2023-04-20 14:13:10.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/top_level.txt
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)       38 2023-04-20 14:13:10.418461 batch_ingestion_client_py-1.0.2/setup.cfg
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1102 2023-04-20 14:12:56.000000 batch_ingestion_client_py-1.0.2/setup.py
```

### Comparing `batch_ingestion_client_py-1.0.1/PKG-INFO` & `batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: batch_ingestion_client_py
-Version: 1.0.1
+Name: batch-ingestion-client-py
+Version: 1.0.2
 Summary: A client for the BatchIngestion mediawiki API
 Home-page: UNKNOWN
 Author: QuentinJanuel
 Author-email: <quentinjanuelkij@gmail.com>
 License: UNKNOWN
 Keywords: python,mediawiki,batchingestion,wikidata,wikibase,api,client
 Platform: UNKNOWN
@@ -22,15 +22,15 @@
 This is a Python client library for the [BatchIngestion](https://gitlab.the-qa-company.com/FrozenMink/batchingestionextension) MediaWiki extension, which provides an API to ingest many entities at once. This library allows you to easily ingest entities in bulk, either by parsing them from JSON or by creating them using Python objects.
 
 ## Installation
 
 You can install this library using pip:
 
 ```bash
-pip install batch-ingestion-client
+pip install pip install batch-ingestion-client-py
 ```
 
 ## Usage
 
 You first need to instantiate a `BatchIngestor` object, passing in the URL of the MediaWiki instance you want to use:
 
 ```python
```

### Comparing `batch_ingestion_client_py-1.0.1/README.md` & `batch_ingestion_client_py-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This is a Python client library for the [BatchIngestion](https://gitlab.the-qa-company.com/FrozenMink/batchingestionextension) MediaWiki extension, which provides an API to ingest many entities at once. This library allows you to easily ingest entities in bulk, either by parsing them from JSON or by creating them using Python objects.
 
 ## Installation
 
 You can install this library using pip:
 
 ```bash
-pip install batch-ingestion-client
+pip install pip install batch-ingestion-client-py
 ```
 
 ## Usage
 
 You first need to instantiate a `BatchIngestor` object, passing in the URL of the MediaWiki instance you want to use:
 
 ```python
```

### Comparing `batch_ingestion_client_py-1.0.1/batch_ingestion_client_py/data.py` & `batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/data.py`

 * *Files identical despite different names*

### Comparing `batch_ingestion_client_py-1.0.1/batch_ingestion_client_py/main.py` & `batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/main.py`

 * *Files identical despite different names*

### Comparing `batch_ingestion_client_py-1.0.1/batch_ingestion_client_py/response.py` & `batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/response.py`

 * *Files identical despite different names*

### Comparing `batch_ingestion_client_py-1.0.1/batch_ingestion_client_py.egg-info/PKG-INFO` & `batch_ingestion_client_py-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: batch-ingestion-client-py
-Version: 1.0.1
+Name: batch_ingestion_client_py
+Version: 1.0.2
 Summary: A client for the BatchIngestion mediawiki API
 Home-page: UNKNOWN
 Author: QuentinJanuel
 Author-email: <quentinjanuelkij@gmail.com>
 License: UNKNOWN
 Keywords: python,mediawiki,batchingestion,wikidata,wikibase,api,client
 Platform: UNKNOWN
@@ -22,15 +22,15 @@
 This is a Python client library for the [BatchIngestion](https://gitlab.the-qa-company.com/FrozenMink/batchingestionextension) MediaWiki extension, which provides an API to ingest many entities at once. This library allows you to easily ingest entities in bulk, either by parsing them from JSON or by creating them using Python objects.
 
 ## Installation
 
 You can install this library using pip:
 
 ```bash
-pip install batch-ingestion-client
+pip install pip install batch-ingestion-client-py
 ```
 
 ## Usage
 
 You first need to instantiate a `BatchIngestor` object, passing in the URL of the MediaWiki instance you want to use:
 
 ```python
```

### Comparing `batch_ingestion_client_py-1.0.1/setup.py` & `batch_ingestion_client_py-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DESCRIPTION = "A client for the BatchIngestion mediawiki API"
 
 setup(
     name="batch_ingestion_client_py",
     version=VERSION,
     author="QuentinJanuel",
     author_email="<quentinjanuelkij@gmail.com>",
```

