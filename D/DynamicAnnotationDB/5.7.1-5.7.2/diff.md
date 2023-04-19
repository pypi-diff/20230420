# Comparing `tmp/DynamicAnnotationDB-5.7.1.tar.gz` & `tmp/DynamicAnnotationDB-5.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DynamicAnnotationDB-5.7.1.tar", last modified: Wed Apr 12 18:44:53 2023, max compression
+gzip compressed data, was "DynamicAnnotationDB-5.7.2.tar", last modified: Wed Apr 19 23:49:19 2023, max compression
```

## Comparing `DynamicAnnotationDB-5.7.1.tar` & `DynamicAnnotationDB-5.7.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 derrickb  (1000) derrickb  (1000)        0 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/
-drwxrwxr-x   0 derrickb  (1000) derrickb  (1000)        0 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/DynamicAnnotationDB.egg-info/
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     1000 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/DynamicAnnotationDB.egg-info/PKG-INFO
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     1821 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/DynamicAnnotationDB.egg-info/SOURCES.txt
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)        1 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/DynamicAnnotationDB.egg-info/dependency_links.txt
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)      125 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/DynamicAnnotationDB.egg-info/requires.txt
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)       26 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/DynamicAnnotationDB.egg-info/top_level.txt
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)       36 2020-06-13 21:21:04.000000 DynamicAnnotationDB-5.7.1/MANIFEST.in
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     1000 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/PKG-INFO
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)      474 2022-02-04 23:36:22.000000 DynamicAnnotationDB-5.7.1/README.md
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)       67 2021-04-21 20:52:01.000000 DynamicAnnotationDB-5.7.1/doc_requirements.txt
-drwxrwxr-x   0 derrickb  (1000) derrickb  (1000)        0 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)       72 2023-04-12 18:44:36.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/__init__.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)    18140 2023-04-12 18:10:07.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/annotation.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)    13198 2023-04-12 18:43:56.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/database.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     2064 2023-02-14 22:10:55.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/errors.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     5969 2023-04-12 18:43:56.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/interface.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     1139 2022-06-23 21:43:50.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/key_utils.py
-drwxrwxr-x   0 derrickb  (1000) derrickb  (1000)        0 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)      166 2023-04-12 18:44:36.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/__init__.py
-drwxrwxr-x   0 derrickb  (1000) derrickb  (1000)        0 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)        0 2022-09-14 17:13:01.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/__init__.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     2373 2023-04-12 18:10:07.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/env.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     1100 2022-09-14 17:13:01.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/run.py
-drwxrwxr-x   0 derrickb  (1000) derrickb  (1000)        0 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)      747 2023-03-17 19:19:28.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/309cf493a1e2_adding_warning_field.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)      969 2023-03-17 19:19:28.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/5a1d7c0ad006_add_status_column.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)      515 2023-03-17 19:19:28.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/6e7f580ff680_add_error_msg.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     1255 2023-04-12 18:10:07.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/7c79eff751b4_add_parent_version_column.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     1063 2023-03-17 19:19:28.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/814d72d74e3b_add_version_error_table.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     2066 2023-03-17 19:19:28.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/8fdc843fc202_adding_permission_and_last_modified.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)      685 2023-03-17 19:19:28.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/975a79461cab_add_is_merged.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)        0 2022-09-14 17:13:01.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/__init__.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     4403 2023-04-12 18:10:07.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/ef5c2d7f96d8_initial_live_db_models.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     1102 2023-03-17 19:26:14.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/fac66b439033_add_view_model.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)    23089 2023-04-12 18:10:07.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/migrate.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     6017 2023-03-17 20:05:33.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/models.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     8351 2022-11-21 00:59:20.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/schema.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)    13779 2022-11-18 17:02:46.000000 DynamicAnnotationDB-5.7.1/dynamicannotationdb/segmentation.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)      124 2023-02-21 20:56:32.000000 DynamicAnnotationDB-5.7.1/requirements.txt
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)      140 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/setup.cfg
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     1303 2023-03-30 20:08:54.000000 DynamicAnnotationDB-5.7.1/setup.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)       68 2021-04-21 20:50:16.000000 DynamicAnnotationDB-5.7.1/test_requirements.txt
-drwxrwxr-x   0 derrickb  (1000) derrickb  (1000)        0 2023-04-12 18:44:53.000000 DynamicAnnotationDB-5.7.1/tests/
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)        0 2022-04-22 22:35:44.000000 DynamicAnnotationDB-5.7.1/tests/__init__.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     3308 2023-02-14 22:10:43.000000 DynamicAnnotationDB-5.7.1/tests/conftest.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     7393 2023-02-14 20:55:19.000000 DynamicAnnotationDB-5.7.1/tests/test_annotation.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     3799 2023-02-21 20:56:32.000000 DynamicAnnotationDB-5.7.1/tests/test_database.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     1433 2023-02-14 20:40:14.000000 DynamicAnnotationDB-5.7.1/tests/test_errors.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)      391 2022-06-23 21:43:50.000000 DynamicAnnotationDB-5.7.1/tests/test_interface.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     3982 2023-02-21 22:18:07.000000 DynamicAnnotationDB-5.7.1/tests/test_schema.py
--rw-rw-r--   0 derrickb  (1000) derrickb  (1000)     5705 2023-02-14 20:55:19.000000 DynamicAnnotationDB-5.7.1/tests/test_segmentation.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.337492 DynamicAnnotationDB-5.7.2/
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.325642 DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/
+-rw-r--r--   0 forrestc   (503) staff       (20)      920 2023-04-19 23:49:19.000000 DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)     1821 2023-04-19 23:49:19.000000 DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-04-19 23:49:19.000000 DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      125 2023-04-19 23:49:19.000000 DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/requires.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       26 2023-04-19 23:49:19.000000 DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/top_level.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       36 2020-06-11 04:40:08.000000 DynamicAnnotationDB-5.7.2/MANIFEST.in
+-rw-r--r--   0 forrestc   (503) staff       (20)      920 2023-04-19 23:49:19.337657 DynamicAnnotationDB-5.7.2/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      474 2022-02-12 21:27:58.000000 DynamicAnnotationDB-5.7.2/README.md
+-rw-r--r--   0 forrestc   (503) staff       (20)       67 2021-06-03 21:07:33.000000 DynamicAnnotationDB-5.7.2/doc_requirements.txt
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.328553 DynamicAnnotationDB-5.7.2/dynamicannotationdb/
+-rw-r--r--   0 forrestc   (503) staff       (20)       72 2023-04-19 23:49:15.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18140 2023-04-19 14:20:52.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    13198 2023-04-18 17:23:16.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/database.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2064 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/errors.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     5969 2023-04-18 17:23:16.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/interface.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1139 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/key_utils.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.329157 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/
+-rw-r--r--   0 forrestc   (503) staff       (20)      166 2023-04-19 23:49:15.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/__init__.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.329951 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2373 2023-04-06 22:59:46.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/env.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1100 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/run.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.334107 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/
+-rw-r--r--   0 forrestc   (503) staff       (20)      747 2022-10-25 16:40:35.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/309cf493a1e2_adding_warning_field.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      969 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/5a1d7c0ad006_add_status_column.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      515 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/6e7f580ff680_add_error_msg.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1255 2023-04-06 22:59:46.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/7c79eff751b4_add_parent_version_column.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1063 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/814d72d74e3b_add_version_error_table.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2066 2022-10-25 19:07:59.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/8fdc843fc202_adding_permission_and_last_modified.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      685 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/975a79461cab_add_is_merged.py
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     4403 2023-04-06 22:59:46.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/ef5c2d7f96d8_initial_live_db_models.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1102 2023-03-14 16:48:52.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/fac66b439033_add_view_model.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    22717 2023-04-19 23:49:05.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/migrate.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6017 2023-04-19 14:20:52.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/models.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     8351 2023-02-18 02:07:45.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/schema.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    13779 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/segmentation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      124 2022-11-21 01:05:53.000000 DynamicAnnotationDB-5.7.2/requirements.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      140 2023-04-19 23:49:19.338162 DynamicAnnotationDB-5.7.2/setup.cfg
+-rw-r--r--   0 forrestc   (503) staff       (20)     1303 2022-02-12 21:27:58.000000 DynamicAnnotationDB-5.7.2/setup.py
+-rw-r--r--   0 forrestc   (503) staff       (20)       68 2021-06-03 21:07:33.000000 DynamicAnnotationDB-5.7.2/test_requirements.txt
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.337201 DynamicAnnotationDB-5.7.2/tests/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-02-19 03:45:38.000000 DynamicAnnotationDB-5.7.2/tests/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3308 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.7.2/tests/conftest.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     7393 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.7.2/tests/test_annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3799 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.7.2/tests/test_database.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1433 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.7.2/tests/test_errors.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      391 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.7.2/tests/test_interface.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3982 2022-09-13 20:07:43.000000 DynamicAnnotationDB-5.7.2/tests/test_schema.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     5705 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.7.2/tests/test_segmentation.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `DynamicAnnotationDB-5.7.1/DynamicAnnotationDB.egg-info/PKG-INFO` & `DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: DynamicAnnotationDB
-Version: 5.7.1
+Version: 5.7.2
 Summary: Annotation Database pendant to the chunkedgraph
 Home-page: https://github.com/seung-lab/DynamicAnnotationDB
 Author: Sven Dorkenwald, Derrick Brittain
 Author-email: sdorkenw@princeton.edu
-License: UNKNOWN
-Description: [![Actions Status](https://github.com/seung-lab/DynamicAnnotationDB/workflows/DynamicAnnotationDB/badge.svg)](https://github.com/seung-lab/DynamicAnnotationDB/actions)
-        [![PyPI version](https://badge.fury.io/py/DynamicAnnotationDB.svg)](https://badge.fury.io/py/DynamicAnnotationDB)
-        [![Documentation Status](https://readthedocs.org/projects/dynamicannotationdb/badge/?version=latest)](https://dynamicannotationdb.readthedocs.io/en/latest/?badge=latest)
-        # DynamicAnnotationDB
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
+
+[![Actions Status](https://github.com/seung-lab/DynamicAnnotationDB/workflows/DynamicAnnotationDB/badge.svg)](https://github.com/seung-lab/DynamicAnnotationDB/actions)
+[![PyPI version](https://badge.fury.io/py/DynamicAnnotationDB.svg)](https://badge.fury.io/py/DynamicAnnotationDB)
+[![Documentation Status](https://readthedocs.org/projects/dynamicannotationdb/badge/?version=latest)](https://dynamicannotationdb.readthedocs.io/en/latest/?badge=latest)
+# DynamicAnnotationDB
```

### Comparing `DynamicAnnotationDB-5.7.1/DynamicAnnotationDB.egg-info/SOURCES.txt` & `DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/PKG-INFO` & `DynamicAnnotationDB-5.7.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: DynamicAnnotationDB
-Version: 5.7.1
+Version: 5.7.2
 Summary: Annotation Database pendant to the chunkedgraph
 Home-page: https://github.com/seung-lab/DynamicAnnotationDB
 Author: Sven Dorkenwald, Derrick Brittain
 Author-email: sdorkenw@princeton.edu
-License: UNKNOWN
-Description: [![Actions Status](https://github.com/seung-lab/DynamicAnnotationDB/workflows/DynamicAnnotationDB/badge.svg)](https://github.com/seung-lab/DynamicAnnotationDB/actions)
-        [![PyPI version](https://badge.fury.io/py/DynamicAnnotationDB.svg)](https://badge.fury.io/py/DynamicAnnotationDB)
-        [![Documentation Status](https://readthedocs.org/projects/dynamicannotationdb/badge/?version=latest)](https://dynamicannotationdb.readthedocs.io/en/latest/?badge=latest)
-        # DynamicAnnotationDB
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
+
+[![Actions Status](https://github.com/seung-lab/DynamicAnnotationDB/workflows/DynamicAnnotationDB/badge.svg)](https://github.com/seung-lab/DynamicAnnotationDB/actions)
+[![PyPI version](https://badge.fury.io/py/DynamicAnnotationDB.svg)](https://badge.fury.io/py/DynamicAnnotationDB)
+[![Documentation Status](https://readthedocs.org/projects/dynamicannotationdb/badge/?version=latest)](https://dynamicannotationdb.readthedocs.io/en/latest/?badge=latest)
+# DynamicAnnotationDB
```

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/annotation.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/annotation.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/database.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/database.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/errors.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/errors.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/interface.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/interface.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/key_utils.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/key_utils.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/env.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/run.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/run.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/309cf493a1e2_adding_warning_field.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/309cf493a1e2_adding_warning_field.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/5a1d7c0ad006_add_status_column.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/5a1d7c0ad006_add_status_column.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/6e7f580ff680_add_error_msg.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/6e7f580ff680_add_error_msg.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/7c79eff751b4_add_parent_version_column.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/7c79eff751b4_add_parent_version_column.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/814d72d74e3b_add_version_error_table.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/814d72d74e3b_add_version_error_table.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/8fdc843fc202_adding_permission_and_last_modified.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/8fdc843fc202_adding_permission_and_last_modified.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/975a79461cab_add_is_merged.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/975a79461cab_add_is_merged.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/ef5c2d7f96d8_initial_live_db_models.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/ef5c2d7f96d8_initial_live_db_models.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/alembic/versions/fac66b439033_add_view_model.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/fac66b439033_add_view_model.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/migration/migrate.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,19 +208,23 @@
         metadata = MetaData(bind=self.target_database.engine)
         metadata.reflect(bind=self.target_database.engine)
         fkey_mappings = []
         for table in metadata.tables:
             table_metadata = self.target_database.get_table_metadata(table)
             if table_metadata:
                 table = metadata.tables[table]
-            try:
-                fkey_mapping = self.add_cascade_delete_to_fkey(table, dry_run)
-                fkey_mappings.append(fkey_mapping)
-            except Exception as error:
-                raise error
+                try:
+                    fkey_mapping = self.add_cascade_delete_to_fkey(table, dry_run)
+                    if fkey_mapping:
+                        fkey_mappings.append(fkey_mapping)
+                except Exception as error:
+                    raise error
+        if not fkey_mappings:
+            logging.info("No tables to migrate fkey constraints")
+            return None
         return fkey_mappings
 
     def add_cascade_delete_to_fkey(self, table: Table, dry_run: bool = True):
         table_name = table.name
         fkeys_to_drop = {}
         fkey_to_add = {}
         for fk in self.target_inspector.get_foreign_keys(table_name):
@@ -231,52 +235,40 @@
                     [table.c[c] for c in fk["constrained_columns"]],
                     [fk["referred_table"] + "." + c for c in fk["referred_columns"]],
                     name=fk["name"],
                 )
                 drop_constraint = DropConstraint(fkey)
                 fkeys_to_drop[fkey.name] = str(drop_constraint)
 
-                if not dry_run:
-                    with self.target_database.engine.connect() as conn:
-                        try:
-                            conn.execute(drop_constraint)
-                        except ProgrammingError as error:
-                            logging.error(f"{fkey.name} not present in the database: {error}")
-
                 # create a new foreign key constraint with the specified 'ondelete' option
                 new_fkey = ForeignKeyConstraint(
                     [table.c[c] for c in fk["constrained_columns"]],
                     [fk["referred_table"] + "." + c for c in fk["referred_columns"]],
                     name=fk["name"],
                     ondelete="CASCADE",
                 )
                 add_constraint = AddConstraint(new_fkey)
 
                 fkey_to_add[new_fkey.name] = str(add_constraint)
 
                 if not dry_run:
-                    with self.target_database.engine.connect() as conn:
-                        # start a transaction
-                        trans = conn.begin()
-
-                        try:
-                            conn.execute(add_constraint)
-                            trans.commit()
-                            logging.info(
-                                f"Table {table_name} altered with CASCADE DELETE"
-                            )
-                        except Exception as error:
-                            trans.rollback()
-                            raise error
-        return {
-            f"Table Name: {table_name}": {
-                "Fkeys to drop": fkeys_to_drop,
-                "Fkeys to add": fkey_to_add,
+                    with self.target_database.engine.begin() as conn:
+                        conn.execute(drop_constraint)
+                        conn.execute(add_constraint)
+                        logging.info(f"Table {table_name} altered with CASCADE DELETE")
+        return (
+            {
+                f"Table Name: {table_name}": {
+                    "Fkeys to drop": fkeys_to_drop,
+                    "Fkeys to add": fkey_to_add,
+                }
             }
-        }
+            if fkeys_to_drop or fkey_to_add
+            else None
+        )
 
     def upgrade_annotation_models(self, dry_run: bool = True):
         """Upgrades annotation models present in the database
         if underlying schemas have changed.
 
         Raises
         ------
```

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/models.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/models.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/schema.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/schema.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/dynamicannotationdb/segmentation.py` & `DynamicAnnotationDB-5.7.2/dynamicannotationdb/segmentation.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/setup.py` & `DynamicAnnotationDB-5.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/tests/conftest.py` & `DynamicAnnotationDB-5.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/tests/test_annotation.py` & `DynamicAnnotationDB-5.7.2/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/tests/test_database.py` & `DynamicAnnotationDB-5.7.2/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/tests/test_errors.py` & `DynamicAnnotationDB-5.7.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/tests/test_schema.py` & `DynamicAnnotationDB-5.7.2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.1/tests/test_segmentation.py` & `DynamicAnnotationDB-5.7.2/tests/test_segmentation.py`

 * *Files identical despite different names*

