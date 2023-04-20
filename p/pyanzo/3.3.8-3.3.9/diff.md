# Comparing `tmp/pyanzo-3.3.8.tar.gz` & `tmp/pyanzo-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanzo-3.3.8.tar", last modified: Wed Apr 19 19:02:24 2023, max compression
+gzip compressed data, was "pyanzo-3.3.9.tar", last modified: Thu Apr 20 17:45:20 2023, max compression
```

## Comparing `pyanzo-3.3.8.tar` & `pyanzo-3.3.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:24.000040 pyanzo-3.3.8/
--rw-r--r--   0 silverfang   (501) staff       (20)     6548 2022-02-14 16:18:37.000000 pyanzo-3.3.8/CONTRIBUTING.md
--rw-r--r--   0 silverfang   (501) staff       (20)      897 2021-01-06 22:11:36.000000 pyanzo-3.3.8/HISTORY.md
--rw-r--r--   0 silverfang   (501) staff       (20)      135 2022-08-19 01:48:08.000000 pyanzo-3.3.8/LICENSE
--rw-r--r--   0 silverfang   (501) staff       (20)      251 2022-10-11 15:10:33.000000 pyanzo-3.3.8/MANIFEST.in
--rw-r--r--   0 silverfang   (501) staff       (20)      771 2023-04-19 19:02:24.000347 pyanzo-3.3.8/PKG-INFO
--rw-r--r--   0 silverfang   (501) staff       (20)     3145 2022-08-19 01:48:08.000000 pyanzo-3.3.8/README.md
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.921843 pyanzo-3.3.8/docs/
--rw-r--r--   0 silverfang   (501) staff       (20)      607 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/Makefile
--rwxr-xr-x   0 silverfang   (501) staff       (20)     4854 2022-08-17 19:11:17.000000 pyanzo-3.3.8/docs/conf.py
--rw-r--r--   0 silverfang   (501) staff       (20)       33 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/contributing.rst
--rw-r--r--   0 silverfang   (501) staff       (20)       28 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/history.rst
--rw-r--r--   0 silverfang   (501) staff       (20)      304 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/index.rst
--rw-r--r--   0 silverfang   (501) staff       (20)       74 2020-11-07 03:54:19.000000 pyanzo-3.3.8/docs/installation.rst
--rw-r--r--   0 silverfang   (501) staff       (20)      768 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/make.bat
--rw-r--r--   0 silverfang   (501) staff       (20)       55 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/modules.rst
--rw-r--r--   0 silverfang   (501) staff       (20)     1355 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/pyanzo.rst
--rw-r--r--   0 silverfang   (501) staff       (20)       26 2021-01-06 22:11:36.000000 pyanzo-3.3.8/docs/readme.rst
--rw-r--r--   0 silverfang   (501) staff       (20)     1099 2020-11-07 03:54:19.000000 pyanzo-3.3.8/docs/usage.rst
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.931159 pyanzo-3.3.8/pyanzo/
--rw-r--r--   0 silverfang   (501) staff       (20)     1061 2022-08-19 01:48:08.000000 pyanzo-3.3.8/pyanzo/__init__.py
--rw-r--r--   0 silverfang   (501) staff       (20)    19006 2023-04-19 16:08:21.000000 pyanzo-3.3.8/pyanzo/anzo_client.py
--rw-r--r--   0 silverfang   (501) staff       (20)    17025 2023-04-19 19:01:50.000000 pyanzo-3.3.8/pyanzo/anzo_request.py
--rw-r--r--   0 silverfang   (501) staff       (20)     1048 2023-03-16 20:38:35.000000 pyanzo-3.3.8/pyanzo/api_properties.py
--rw-r--r--   0 silverfang   (501) staff       (20)    11493 2023-03-16 18:26:47.000000 pyanzo-3.3.8/pyanzo/api_request.py
--rw-r--r--   0 silverfang   (501) staff       (20)    21258 2022-10-18 03:11:43.000000 pyanzo-3.3.8/pyanzo/graphmart_manager.py
--rw-r--r--   0 silverfang   (501) staff       (20)     8960 2022-08-19 01:48:08.000000 pyanzo-3.3.8/pyanzo/lds_manager.py
--rw-r--r--   0 silverfang   (501) staff       (20)    15951 2023-01-31 22:06:39.000000 pyanzo-3.3.8/pyanzo/orchestration_wrapper.py
--rw-r--r--   0 silverfang   (501) staff       (20)    18589 2023-01-31 22:13:54.000000 pyanzo-3.3.8/pyanzo/quad_store.py
--rw-r--r--   0 silverfang   (501) staff       (20)     6434 2022-08-19 01:48:08.000000 pyanzo-3.3.8/pyanzo/query_result.py
--rw-r--r--   0 silverfang   (501) staff       (20)     1998 2022-08-19 01:48:08.000000 pyanzo-3.3.8/pyanzo/uris.py
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.934708 pyanzo-3.3.8/pyanzo.egg-info/
--rw-r--r--   0 silverfang   (501) staff       (20)      771 2023-04-19 19:02:23.000000 pyanzo-3.3.8/pyanzo.egg-info/PKG-INFO
--rw-r--r--   0 silverfang   (501) staff       (20)     2729 2023-04-19 19:02:23.000000 pyanzo-3.3.8/pyanzo.egg-info/SOURCES.txt
--rw-r--r--   0 silverfang   (501) staff       (20)        1 2023-04-19 19:02:23.000000 pyanzo-3.3.8/pyanzo.egg-info/dependency_links.txt
--rw-r--r--   0 silverfang   (501) staff       (20)        1 2020-06-30 21:36:32.000000 pyanzo-3.3.8/pyanzo.egg-info/not-zip-safe
--rw-r--r--   0 silverfang   (501) staff       (20)       48 2023-04-19 19:02:23.000000 pyanzo-3.3.8/pyanzo.egg-info/requires.txt
--rw-r--r--   0 silverfang   (501) staff       (20)        7 2023-04-19 19:02:23.000000 pyanzo-3.3.8/pyanzo.egg-info/top_level.txt
--rw-r--r--   0 silverfang   (501) staff       (20)      417 2023-04-19 19:02:24.001570 pyanzo-3.3.8/setup.cfg
--rw-r--r--   0 silverfang   (501) staff       (20)     1792 2023-04-19 18:55:10.000000 pyanzo-3.3.8/setup.py
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.962310 pyanzo-3.3.8/tests/
--rw-r--r--   0 silverfang   (501) staff       (20)        0 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/__init__.py
--rw-r--r--   0 silverfang   (501) staff       (20)       40 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/query.rq
--rw-r--r--   0 silverfang   (501) staff       (20)     6146 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_add_and_remove.py
--rw-r--r--   0 silverfang   (501) staff       (20)     6676 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_advanced.py
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.972317 pyanzo-3.3.8/tests/test_assets/
--rw-r--r--   0 silverfang   (501) staff       (20)    15330 2020-11-07 03:54:19.000000 pyanzo-3.3.8/tests/test_assets/gmart.trig
--rw-r--r--   0 silverfang   (501) staff       (20)      254 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/malformed_graphmart_query.rq
--rw-r--r--   0 silverfang   (501) staff       (20)      227 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/malformed_journal_query.rq
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.974183 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/
--rw-r--r--   0 silverfang   (501) staff       (20)      102 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/.lsdir
--rw-r--r--   0 silverfang   (501) staff       (20)     3483 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/flds.trig
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.975820 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/onts/
--rw-r--r--   0 silverfang   (501) staff       (20)       50 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/onts/.ontsdir
--rw-r--r--   0 silverfang   (501) staff       (20)     3237 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.911036 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.911136 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.992402 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/
--rw-r--r--   0 silverfang   (501) staff       (20)       12 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/..jobMetadata.crc
--rw-r--r--   0 silverfang   (501) staff       (20)       12 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/..lsdir.crc
--rw-r--r--   0 silverfang   (501) staff       (20)      154 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.jobMetadata
--rw-r--r--   0 silverfang   (501) staff       (20)       39 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.lsdir
--rw-r--r--   0 silverfang   (501) staff       (20)       12 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.part-00000.gz.ttl.gz.crc
--rw-r--r--   0 silverfang   (501) staff       (20)      339 2020-11-07 03:54:19.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/part-00000.gz.ttl.gz
--rw-r--r--   0 silverfang   (501) staff       (20)      292 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/query_test_graphmart.sh
--rw-r--r--   0 silverfang   (501) staff       (20)      755 2021-04-21 23:24:42.000000 pyanzo-3.3.8/tests/test_assets/sample.json
--rw-r--r--   0 silverfang   (501) staff       (20)      194 2021-04-21 23:24:42.000000 pyanzo-3.3.8/tests/test_assets/sample.n3
--rw-r--r--   0 silverfang   (501) staff       (20)      240 2021-04-21 23:24:42.000000 pyanzo-3.3.8/tests/test_assets/sample.trig
--rw-r--r--   0 silverfang   (501) staff       (20)     1094 2021-04-21 23:24:42.000000 pyanzo-3.3.8/tests/test_assets/sample.trix
--rw-r--r--   0 silverfang   (501) staff       (20)      194 2021-04-21 23:24:42.000000 pyanzo-3.3.8/tests/test_assets/sample.ttl
--rw-r--r--   0 silverfang   (501) staff       (20)      255 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/simple_graphmart_query.rq
--rw-r--r--   0 silverfang   (501) staff       (20)      266 2020-11-07 03:54:19.000000 pyanzo-3.3.8/tests/test_assets/simple_journal_query.rq
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.999210 pyanzo-3.3.8/tests/test_assets/trig/
--rw-r--r--   0 silverfang   (501) staff       (20)     3452 2022-02-14 16:18:37.000000 pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_AZG.trig
--rwxr-xr-x   0 silverfang   (501) staff       (20)      855 2020-11-07 03:54:19.000000 pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_Graphmart_export.trig
--rwxr-xr-x   0 silverfang   (501) staff       (20)    23062 2022-02-14 16:18:37.000000 pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_Graphmart_graph.trig
--rwxr-xr-x   0 silverfang   (501) staff       (20)     3221 2022-02-14 16:18:37.000000 pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_Graphmart_registry.trig
--rw-r--r--   0 silverfang   (501) staff       (20)      493 2021-04-21 23:24:42.000000 pyanzo-3.3.8/tests/test_assets/trig_with_bnodes.trig
--rw-r--r--   0 silverfang   (501) staff       (20)     3499 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_auth.py
--rw-r--r--   0 silverfang   (501) staff       (20)    17326 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_basic.py
--rw-r--r--   0 silverfang   (501) staff       (20)      930 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_common.py
--rw-r--r--   0 silverfang   (501) staff       (20)     2869 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_execute_semantic_service.py
--rw-r--r--   0 silverfang   (501) staff       (20)     2002 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_get.py
--rw-r--r--   0 silverfang   (501) staff       (20)     8746 2022-10-13 17:19:17.000000 pyanzo-3.3.8/tests/test_graphmart_manager.py
--rw-r--r--   0 silverfang   (501) staff       (20)     6484 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_lds_manager.py
--rw-r--r--   0 silverfang   (501) staff       (20)     4695 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_orchestration_wrapper.py
--rw-r--r--   0 silverfang   (501) staff       (20)    16440 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_quad_store.py
--rw-r--r--   0 silverfang   (501) staff       (20)     9066 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_query_graphmart.py
--rw-r--r--   0 silverfang   (501) staff       (20)     8032 2022-09-06 00:47:10.000000 pyanzo-3.3.8/tests/test_query_journal.py
--rw-r--r--   0 silverfang   (501) staff       (20)     5736 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_query_lds.py
--rw-r--r--   0 silverfang   (501) staff       (20)     2066 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_query_system_tables.py
--rw-r--r--   0 silverfang   (501) staff       (20)     4618 2021-01-06 22:11:36.000000 pyanzo-3.3.8/tests/test_update_journal.py
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-20 17:45:20.587531 pyanzo-3.3.9/
+-rw-r--r--   0 silverfang   (501) staff       (20)     6548 2022-02-14 16:18:37.000000 pyanzo-3.3.9/CONTRIBUTING.md
+-rw-r--r--   0 silverfang   (501) staff       (20)      897 2021-01-06 22:11:36.000000 pyanzo-3.3.9/HISTORY.md
+-rw-r--r--   0 silverfang   (501) staff       (20)      135 2022-08-19 01:48:08.000000 pyanzo-3.3.9/LICENSE
+-rw-r--r--   0 silverfang   (501) staff       (20)      251 2022-10-11 15:10:33.000000 pyanzo-3.3.9/MANIFEST.in
+-rw-r--r--   0 silverfang   (501) staff       (20)      771 2023-04-20 17:45:20.587674 pyanzo-3.3.9/PKG-INFO
+-rw-r--r--   0 silverfang   (501) staff       (20)     3145 2022-08-19 01:48:08.000000 pyanzo-3.3.9/README.md
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-20 17:45:20.551508 pyanzo-3.3.9/docs/
+-rw-r--r--   0 silverfang   (501) staff       (20)      607 2020-06-30 21:09:10.000000 pyanzo-3.3.9/docs/Makefile
+-rwxr-xr-x   0 silverfang   (501) staff       (20)     4854 2022-08-17 19:11:17.000000 pyanzo-3.3.9/docs/conf.py
+-rw-r--r--   0 silverfang   (501) staff       (20)       33 2020-06-30 21:09:10.000000 pyanzo-3.3.9/docs/contributing.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)       28 2020-06-30 21:09:10.000000 pyanzo-3.3.9/docs/history.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)      304 2020-06-30 21:09:10.000000 pyanzo-3.3.9/docs/index.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)       74 2020-11-07 03:54:19.000000 pyanzo-3.3.9/docs/installation.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)      768 2020-06-30 21:09:10.000000 pyanzo-3.3.9/docs/make.bat
+-rw-r--r--   0 silverfang   (501) staff       (20)       55 2020-06-30 21:09:10.000000 pyanzo-3.3.9/docs/modules.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)     1355 2020-06-30 21:09:10.000000 pyanzo-3.3.9/docs/pyanzo.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)       26 2021-01-06 22:11:36.000000 pyanzo-3.3.9/docs/readme.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)     1099 2020-11-07 03:54:19.000000 pyanzo-3.3.9/docs/usage.rst
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-20 17:45:20.561761 pyanzo-3.3.9/pyanzo/
+-rw-r--r--   0 silverfang   (501) staff       (20)     1061 2022-08-19 01:48:08.000000 pyanzo-3.3.9/pyanzo/__init__.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    19006 2023-04-19 16:08:21.000000 pyanzo-3.3.9/pyanzo/anzo_client.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    17110 2023-04-20 13:34:21.000000 pyanzo-3.3.9/pyanzo/anzo_request.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     1048 2023-03-16 20:38:35.000000 pyanzo-3.3.9/pyanzo/api_properties.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    11493 2023-03-16 18:26:47.000000 pyanzo-3.3.9/pyanzo/api_request.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    21258 2022-10-18 03:11:43.000000 pyanzo-3.3.9/pyanzo/graphmart_manager.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     8960 2022-08-19 01:48:08.000000 pyanzo-3.3.9/pyanzo/lds_manager.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    15951 2023-01-31 22:06:39.000000 pyanzo-3.3.9/pyanzo/orchestration_wrapper.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    18589 2023-01-31 22:13:54.000000 pyanzo-3.3.9/pyanzo/quad_store.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     6434 2022-08-19 01:48:08.000000 pyanzo-3.3.9/pyanzo/query_result.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     1998 2022-08-19 01:48:08.000000 pyanzo-3.3.9/pyanzo/uris.py
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-20 17:45:20.564203 pyanzo-3.3.9/pyanzo.egg-info/
+-rw-r--r--   0 silverfang   (501) staff       (20)      771 2023-04-20 17:45:20.000000 pyanzo-3.3.9/pyanzo.egg-info/PKG-INFO
+-rw-r--r--   0 silverfang   (501) staff       (20)     2729 2023-04-20 17:45:20.000000 pyanzo-3.3.9/pyanzo.egg-info/SOURCES.txt
+-rw-r--r--   0 silverfang   (501) staff       (20)        1 2023-04-20 17:45:20.000000 pyanzo-3.3.9/pyanzo.egg-info/dependency_links.txt
+-rw-r--r--   0 silverfang   (501) staff       (20)        1 2020-06-30 21:36:32.000000 pyanzo-3.3.9/pyanzo.egg-info/not-zip-safe
+-rw-r--r--   0 silverfang   (501) staff       (20)       48 2023-04-20 17:45:20.000000 pyanzo-3.3.9/pyanzo.egg-info/requires.txt
+-rw-r--r--   0 silverfang   (501) staff       (20)        7 2023-04-20 17:45:20.000000 pyanzo-3.3.9/pyanzo.egg-info/top_level.txt
+-rw-r--r--   0 silverfang   (501) staff       (20)      417 2023-04-20 17:45:20.588273 pyanzo-3.3.9/setup.cfg
+-rw-r--r--   0 silverfang   (501) staff       (20)     1792 2023-04-20 17:45:06.000000 pyanzo-3.3.9/setup.py
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-20 17:45:20.573879 pyanzo-3.3.9/tests/
+-rw-r--r--   0 silverfang   (501) staff       (20)        0 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/__init__.py
+-rw-r--r--   0 silverfang   (501) staff       (20)       40 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/query.rq
+-rw-r--r--   0 silverfang   (501) staff       (20)     6146 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_add_and_remove.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     6676 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_advanced.py
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-20 17:45:20.580352 pyanzo-3.3.9/tests/test_assets/
+-rw-r--r--   0 silverfang   (501) staff       (20)    15330 2020-11-07 03:54:19.000000 pyanzo-3.3.9/tests/test_assets/gmart.trig
+-rw-r--r--   0 silverfang   (501) staff       (20)      254 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/malformed_graphmart_query.rq
+-rw-r--r--   0 silverfang   (501) staff       (20)      227 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/malformed_journal_query.rq
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-20 17:45:20.581240 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/
+-rw-r--r--   0 silverfang   (501) staff       (20)      102 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/.lsdir
+-rw-r--r--   0 silverfang   (501) staff       (20)     3483 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/flds.trig
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-20 17:45:20.582175 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/onts/
+-rw-r--r--   0 silverfang   (501) staff       (20)       50 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/onts/.ontsdir
+-rw-r--r--   0 silverfang   (501) staff       (20)     3237 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-20 17:45:20.540825 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-20 17:45:20.540920 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-20 17:45:20.584637 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/
+-rw-r--r--   0 silverfang   (501) staff       (20)       12 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/..jobMetadata.crc
+-rw-r--r--   0 silverfang   (501) staff       (20)       12 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/..lsdir.crc
+-rw-r--r--   0 silverfang   (501) staff       (20)      154 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.jobMetadata
+-rw-r--r--   0 silverfang   (501) staff       (20)       39 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.lsdir
+-rw-r--r--   0 silverfang   (501) staff       (20)       12 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.part-00000.gz.ttl.gz.crc
+-rw-r--r--   0 silverfang   (501) staff       (20)      339 2020-11-07 03:54:19.000000 pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/part-00000.gz.ttl.gz
+-rw-r--r--   0 silverfang   (501) staff       (20)      292 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/query_test_graphmart.sh
+-rw-r--r--   0 silverfang   (501) staff       (20)      755 2021-04-21 23:24:42.000000 pyanzo-3.3.9/tests/test_assets/sample.json
+-rw-r--r--   0 silverfang   (501) staff       (20)      194 2021-04-21 23:24:42.000000 pyanzo-3.3.9/tests/test_assets/sample.n3
+-rw-r--r--   0 silverfang   (501) staff       (20)      240 2021-04-21 23:24:42.000000 pyanzo-3.3.9/tests/test_assets/sample.trig
+-rw-r--r--   0 silverfang   (501) staff       (20)     1094 2021-04-21 23:24:42.000000 pyanzo-3.3.9/tests/test_assets/sample.trix
+-rw-r--r--   0 silverfang   (501) staff       (20)      194 2021-04-21 23:24:42.000000 pyanzo-3.3.9/tests/test_assets/sample.ttl
+-rw-r--r--   0 silverfang   (501) staff       (20)      255 2020-06-30 21:09:10.000000 pyanzo-3.3.9/tests/test_assets/simple_graphmart_query.rq
+-rw-r--r--   0 silverfang   (501) staff       (20)      266 2020-11-07 03:54:19.000000 pyanzo-3.3.9/tests/test_assets/simple_journal_query.rq
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-20 17:45:20.587099 pyanzo-3.3.9/tests/test_assets/trig/
+-rw-r--r--   0 silverfang   (501) staff       (20)     3452 2022-02-14 16:18:37.000000 pyanzo-3.3.9/tests/test_assets/trig/PyAnzo_AZG.trig
+-rwxr-xr-x   0 silverfang   (501) staff       (20)      855 2020-11-07 03:54:19.000000 pyanzo-3.3.9/tests/test_assets/trig/PyAnzo_Graphmart_export.trig
+-rwxr-xr-x   0 silverfang   (501) staff       (20)    23062 2022-02-14 16:18:37.000000 pyanzo-3.3.9/tests/test_assets/trig/PyAnzo_Graphmart_graph.trig
+-rwxr-xr-x   0 silverfang   (501) staff       (20)     3221 2022-02-14 16:18:37.000000 pyanzo-3.3.9/tests/test_assets/trig/PyAnzo_Graphmart_registry.trig
+-rw-r--r--   0 silverfang   (501) staff       (20)      493 2021-04-21 23:24:42.000000 pyanzo-3.3.9/tests/test_assets/trig_with_bnodes.trig
+-rw-r--r--   0 silverfang   (501) staff       (20)     3499 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_auth.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    17326 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_basic.py
+-rw-r--r--   0 silverfang   (501) staff       (20)      930 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_common.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     2869 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_execute_semantic_service.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     2002 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_get.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     8746 2022-10-13 17:19:17.000000 pyanzo-3.3.9/tests/test_graphmart_manager.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     6484 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_lds_manager.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     4695 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_orchestration_wrapper.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    16440 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_quad_store.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     9066 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_query_graphmart.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     8032 2022-09-06 00:47:10.000000 pyanzo-3.3.9/tests/test_query_journal.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     5736 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_query_lds.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     2066 2022-08-19 01:48:08.000000 pyanzo-3.3.9/tests/test_query_system_tables.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     4618 2021-01-06 22:11:36.000000 pyanzo-3.3.9/tests/test_update_journal.py
```

### Comparing `pyanzo-3.3.8/CONTRIBUTING.md` & `pyanzo-3.3.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/HISTORY.md` & `pyanzo-3.3.9/HISTORY.md`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/PKG-INFO` & `pyanzo-3.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanzo
-Version: 3.3.8
+Version: 3.3.9
 Summary: PyAnzo is a library for interacting with Anzo
 Home-page: 
 Author: Tommy Fang, William Ades, Curtis Galione, Andrew Parisi, Alex Ledger
 Author-email: info@cambridgesemantics.com
 Keywords: pyanzo
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pyanzo-3.3.8/README.md` & `pyanzo-3.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/docs/Makefile` & `pyanzo-3.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/docs/conf.py` & `pyanzo-3.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/docs/make.bat` & `pyanzo-3.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/docs/pyanzo.rst` & `pyanzo-3.3.9/docs/pyanzo.rst`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/docs/usage.rst` & `pyanzo-3.3.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/pyanzo/__init__.py` & `pyanzo-3.3.9/pyanzo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/pyanzo/anzo_client.py` & `pyanzo-3.3.9/pyanzo/anzo_client.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/pyanzo/anzo_request.py` & `pyanzo-3.3.9/pyanzo/anzo_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,23 +28,24 @@
         data: The body of the HTTP request
         timeout_seconds: Timeout for the request in seconds
     """
 
     COOKIE_KEY = "Cookie"
 
     def __init__(self, url: str, username: str, password: str, auth_token: str,
-                 headers: Dict[str, Any], data: Any,
-                 timeout_seconds: float) -> None:
+                 headers: Dict[str, Any], data: Any, timeout_seconds: float,
+                 verify: bool) -> None:
         self.url = url
         self.username = username
         self.password = password
         self.auth_token = auth_token
         self.headers = headers
         self.data = data
         self.timeout_seconds = timeout_seconds
+        self.verify = verify
 
     def execute_request(self) -> str:
         """Executes the anzo request and returns the body of the response.
 
         Returns:
             The body of the HTTP response.
 
@@ -57,26 +58,20 @@
             if self.username and self.password:
                 authorization = (self.username, self.password)
             else:
                 authorization = ("", "")
 
             if self.auth_token:
                 self.headers[self.COOKIE_KEY] = self.auth_token
-            try:
-                verify = self.ssl_verify()
-            except OSError as err:
-                print("Invalid cert path provided, setting verify=False")
-                print(err)
-                verify = False
 
             response = requests.post(self.url,
                                      headers=self.headers,
                                      data=self.data,
                                      auth=authorization,
-                                     verify=verify,
+                                     verify=self.verify,
                                      timeout=self.timeout_seconds)
 
         except requests.exceptions.ReadTimeout:
             msg = (f"Request timed out with the timeout set to "
                    f"{self.timeout_seconds} seconds")
             raise TimeoutError(msg) from None
         except Exception as e:
@@ -158,14 +153,15 @@
         self.headers: Dict[str, Any] = {}
         self.base_url = ""
         self.url_postfix = ""
         self.username = ""
         self.password = ""
         self.auth_token = ""
         self.timeout_seconds = None
+        self.verify = False
 
     def _raise_if_url_postfix_is_set(self) -> None:
         if self.url_postfix:
             raise RuntimeError("URL Postfix has already been set")
 
     def with_url(self, url: str, port: str) -> None:
         """Adds the url to the AnzoRequestBuilder.
@@ -387,18 +383,18 @@
             RuntimeError: We currently don't support skipping the cache
                    so if a user tries to do it, an error is raised.
         """
         if skip_cache:
             self.payload_dict[self.SKIP_CACHE] = "true"
 
     def ssl_verify(self):
-        verify = os.getenv('REQUESTS_CA_BUNDLE', False)
-        if verify and not os.path.isfile(verify):
-            raise IOError("Configured CA Bundle does not exist: " + verify)
-        return verify
+        self.verify = os.getenv('REQUESTS_CA_BUNDLE', False)
+        if self.verify and not os.path.isfile(self.verify):
+            raise IOError("Configured CA Bundle does not exist: " +
+                          self.verify)
 
     def build(self) -> AnzoRequest:
         """
         Combine all of the relevant components to build an AnzoRequest.
 
         Returns:
             A fully developed AnzoRequest object
@@ -424,14 +420,20 @@
 
         if self.payload_dict and self.payload_list:
             raise ValueError("Both self.payload_dict and self.payload_list"
                              "cannot be populated")
 
         if not self.timeout_seconds:
             raise ValueError("A timeout for the request must be specified")
+        try:
+            self.ssl_verify()
+        except OSError as err:
+            print("Invalid cert path provided, setting verify=False")
+            print(err)
+            self.verify = False
 
         # Set the data of the request based on the payload.
         # Python-Requests is generous with the type that data can be,
         # so we have two cases:
         # (a) The payload is a dict in which case we pass data as a dict
         # (b) the payload is a list, in which case we pass the serialied
         #     list as a string
@@ -442,8 +444,8 @@
         elif self.payload_list:
             data = json.dumps(self.payload_list)
 
         full_url = f"{self.base_url}/{self.url_postfix}"
 
         return AnzoRequest(full_url, self.username, self.password,
                            self.auth_token, self.headers, data,
-                           self.timeout_seconds)
+                           self.timeout_seconds, self.verify)
```

### Comparing `pyanzo-3.3.8/pyanzo/api_properties.py` & `pyanzo-3.3.9/pyanzo/api_properties.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/pyanzo/api_request.py` & `pyanzo-3.3.9/pyanzo/api_request.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/pyanzo/graphmart_manager.py` & `pyanzo-3.3.9/pyanzo/graphmart_manager.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/pyanzo/lds_manager.py` & `pyanzo-3.3.9/pyanzo/lds_manager.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/pyanzo/orchestration_wrapper.py` & `pyanzo-3.3.9/pyanzo/orchestration_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/pyanzo/quad_store.py` & `pyanzo-3.3.9/pyanzo/quad_store.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/pyanzo/query_result.py` & `pyanzo-3.3.9/pyanzo/query_result.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/pyanzo/uris.py` & `pyanzo-3.3.9/pyanzo/uris.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/pyanzo.egg-info/PKG-INFO` & `pyanzo-3.3.9/pyanzo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanzo
-Version: 3.3.8
+Version: 3.3.9
 Summary: PyAnzo is a library for interacting with Anzo
 Home-page: 
 Author: Tommy Fang, William Ades, Curtis Galione, Andrew Parisi, Alex Ledger
 Author-email: info@cambridgesemantics.com
 Keywords: pyanzo
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pyanzo-3.3.8/pyanzo.egg-info/SOURCES.txt` & `pyanzo-3.3.9/pyanzo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/setup.py` & `pyanzo-3.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,10 +51,10 @@
     keywords='pyanzo',
     name='pyanzo',
     packages=find_packages(include=['pyanzo', 'pyanzo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='',
-    version='3.3.8',
+    version='3.3.9',
     zip_safe=False,
 )
```

### Comparing `pyanzo-3.3.8/tests/test_add_and_remove.py` & `pyanzo-3.3.9/tests/test_add_and_remove.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_advanced.py` & `pyanzo-3.3.9/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_assets/gmart.trig` & `pyanzo-3.3.9/tests/test_assets/gmart.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/flds.trig` & `pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/flds.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig` & `pyanzo-3.3.9/tests/test_assets/pyanzo_test_dataset/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_assets/sample.json` & `pyanzo-3.3.9/tests/test_assets/sample.json`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_assets/sample.trix` & `pyanzo-3.3.9/tests/test_assets/sample.trix`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_AZG.trig` & `pyanzo-3.3.9/tests/test_assets/trig/PyAnzo_AZG.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_Graphmart_export.trig` & `pyanzo-3.3.9/tests/test_assets/trig/PyAnzo_Graphmart_export.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_Graphmart_graph.trig` & `pyanzo-3.3.9/tests/test_assets/trig/PyAnzo_Graphmart_graph.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_Graphmart_registry.trig` & `pyanzo-3.3.9/tests/test_assets/trig/PyAnzo_Graphmart_registry.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_auth.py` & `pyanzo-3.3.9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_basic.py` & `pyanzo-3.3.9/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_common.py` & `pyanzo-3.3.9/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_execute_semantic_service.py` & `pyanzo-3.3.9/tests/test_execute_semantic_service.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_get.py` & `pyanzo-3.3.9/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_graphmart_manager.py` & `pyanzo-3.3.9/tests/test_graphmart_manager.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_lds_manager.py` & `pyanzo-3.3.9/tests/test_lds_manager.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_orchestration_wrapper.py` & `pyanzo-3.3.9/tests/test_orchestration_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_quad_store.py` & `pyanzo-3.3.9/tests/test_quad_store.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_query_graphmart.py` & `pyanzo-3.3.9/tests/test_query_graphmart.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_query_journal.py` & `pyanzo-3.3.9/tests/test_query_journal.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_query_lds.py` & `pyanzo-3.3.9/tests/test_query_lds.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_query_system_tables.py` & `pyanzo-3.3.9/tests/test_query_system_tables.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.8/tests/test_update_journal.py` & `pyanzo-3.3.9/tests/test_update_journal.py`

 * *Files identical despite different names*

