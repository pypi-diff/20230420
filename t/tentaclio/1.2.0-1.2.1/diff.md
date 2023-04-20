# Comparing `tmp/tentaclio-1.2.0.tar.gz` & `tmp/tentaclio-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tentaclio-1.2.0.tar", last modified: Mon Apr 17 08:08:08 2023, max compression
+gzip compressed data, was "tentaclio-1.2.1.tar", last modified: Thu Apr 20 08:29:07 2023, max compression
```

## Comparing `tentaclio-1.2.0.tar` & `tentaclio-1.2.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.558878 tentaclio-1.2.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2023-04-17 08:07:46.000000 tentaclio-1.2.0/LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11251 2023-04-17 08:08:08.558878 tentaclio-1.2.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10286 2023-04-17 08:07:46.000000 tentaclio-1.2.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      719 2023-04-17 08:08:08.558878 tentaclio-1.2.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2445 2023-04-17 08:07:46.000000 tentaclio-1.2.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.554878 tentaclio-1.2.0/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.554878 tentaclio-1.2.0/src/tentaclio/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1457 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/__main__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.554878 tentaclio-1.2.0/src/tentaclio/clients/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      464 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1854 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/base_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      703 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/decorators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      299 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7320 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/ftp_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5661 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/http_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/importer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1749 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/local_fs_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5487 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/clients/sqla_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.558878 tentaclio-1.2.0/src/tentaclio/credentials/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      143 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/credentials/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      817 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/credentials/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1211 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/credentials/env.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4774 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/credentials/injection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3214 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/credentials/reader.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.558878 tentaclio-1.2.0/src/tentaclio/databases/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/databases/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      382 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/databases/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1366 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/databases/db_registry.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.558878 tentaclio-1.2.0/src/tentaclio/fs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      232 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3419 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1267 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/copier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      579 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/copiers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/remover.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1669 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/scanner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1170 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/fs/scanners.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.558878 tentaclio-1.2.0/src/tentaclio/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1406 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/hooks/slack_hook.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1697 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/protocols.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1120 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/registry.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.558878 tentaclio-1.2.0/src/tentaclio/streams/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      210 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/streams/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2403 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/streams/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7856 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/streams/base_stream.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2174 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/streams/csv_db_stream.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/streams/stream_client_handler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2657 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/streams/stream_registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5212 2023-04-17 08:07:46.000000 tentaclio-1.2.0/src/tentaclio/urls.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 08:08:08.554878 tentaclio-1.2.0/src/tentaclio.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11251 2023-04-17 08:08:08.000000 tentaclio-1.2.0/src/tentaclio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1450 2023-04-17 08:08:08.000000 tentaclio-1.2.0/src/tentaclio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-17 08:08:08.000000 tentaclio-1.2.0/src/tentaclio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      303 2023-04-17 08:08:08.000000 tentaclio-1.2.0/src/tentaclio.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-17 08:08:08.000000 tentaclio-1.2.0/src/tentaclio.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:29:07.269539 tentaclio-1.2.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2023-04-20 08:28:44.000000 tentaclio-1.2.1/LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11251 2023-04-20 08:29:07.269539 tentaclio-1.2.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10286 2023-04-20 08:28:44.000000 tentaclio-1.2.1/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      719 2023-04-20 08:29:07.269539 tentaclio-1.2.1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2445 2023-04-20 08:28:44.000000 tentaclio-1.2.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:29:07.261539 tentaclio-1.2.1/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:29:07.265539 tentaclio-1.2.1/src/tentaclio/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1457 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/__main__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:29:07.265539 tentaclio-1.2.1/src/tentaclio/clients/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      464 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/clients/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1854 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/clients/base_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      703 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/clients/decorators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      299 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/clients/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7320 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/clients/ftp_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5661 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/clients/http_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/clients/importer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1749 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/clients/local_fs_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5500 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/clients/sqla_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:29:07.265539 tentaclio-1.2.1/src/tentaclio/credentials/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      143 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/credentials/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      817 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/credentials/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1211 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/credentials/env.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4774 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/credentials/injection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3214 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/credentials/reader.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:29:07.265539 tentaclio-1.2.1/src/tentaclio/databases/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/databases/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      382 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/databases/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1366 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/databases/db_registry.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:29:07.265539 tentaclio-1.2.1/src/tentaclio/fs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      232 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/fs/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3419 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/fs/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1267 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/fs/copier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      579 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/fs/copiers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/fs/remover.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1669 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/fs/scanner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1170 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/fs/scanners.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:29:07.265539 tentaclio-1.2.1/src/tentaclio/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1406 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/hooks/slack_hook.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1697 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/protocols.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1120 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/registry.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:29:07.269539 tentaclio-1.2.1/src/tentaclio/streams/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      210 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/streams/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2403 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/streams/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7856 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/streams/base_stream.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2174 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/streams/csv_db_stream.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/streams/stream_client_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2657 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/streams/stream_registry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5212 2023-04-20 08:28:44.000000 tentaclio-1.2.1/src/tentaclio/urls.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-20 08:29:07.265539 tentaclio-1.2.1/src/tentaclio.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11251 2023-04-20 08:29:07.000000 tentaclio-1.2.1/src/tentaclio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1450 2023-04-20 08:29:07.000000 tentaclio-1.2.1/src/tentaclio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-20 08:29:07.000000 tentaclio-1.2.1/src/tentaclio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      303 2023-04-20 08:29:07.000000 tentaclio-1.2.1/src/tentaclio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-20 08:29:07.000000 tentaclio-1.2.1/src/tentaclio.egg-info/top_level.txt
```

### Comparing `tentaclio-1.2.0/LICENSE.txt` & `tentaclio-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/PKG-INFO` & `tentaclio-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tentaclio
-Version: 1.2.0
+Version: 1.2.1
 Summary: Unification of data connectors for distributed data tasks
 Home-page: https://github.com/octoenergy/tentaclio
 Author: Octopus Energy
 Author-email: nerds@octoenergy.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tentaclio-1.2.0/README.md` & `tentaclio-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/setup.cfg` & `tentaclio-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/setup.py` & `tentaclio-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 import sys
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 
-VERSION = "1.2.0"
+VERSION = "1.2.1"
 
 REPO_ROOT = pathlib.Path(__file__).parent
 
 with open(REPO_ROOT / "README.md", encoding="utf-8") as f:
     README = f.read()
```

### Comparing `tentaclio-1.2.0/src/tentaclio/__init__.py` & `tentaclio-1.2.1/src/tentaclio/__init__.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/__main__.py` & `tentaclio-1.2.1/src/tentaclio/__main__.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/clients/base_client.py` & `tentaclio-1.2.1/src/tentaclio/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/clients/decorators.py` & `tentaclio-1.2.1/src/tentaclio/clients/decorators.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/clients/ftp_client.py` & `tentaclio-1.2.1/src/tentaclio/clients/ftp_client.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/clients/http_client.py` & `tentaclio-1.2.1/src/tentaclio/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/clients/importer.py` & `tentaclio-1.2.1/src/tentaclio/clients/importer.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/clients/local_fs_client.py` & `tentaclio-1.2.1/src/tentaclio/clients/local_fs_client.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/clients/sqla_client.py` & `tentaclio-1.2.1/src/tentaclio/clients/sqla_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             username=self.username,
             password=self.password,
             host=self.host,
             port=self.port,
             database=self.database,
         )
         if self.url.query_string:
-            parsed_url.update_query_string(self.url.query_string)
+            parsed_url = parsed_url.update_query_string(self.url.query_string)
         if self.engine is None:
             self.engine = create_engine(
                 parsed_url,
                 execution_options=self.execution_options,
                 connect_args=self.connect_args,
             )
         return self.engine.connect()
```

### Comparing `tentaclio-1.2.0/src/tentaclio/credentials/api.py` & `tentaclio-1.2.1/src/tentaclio/credentials/api.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/credentials/env.py` & `tentaclio-1.2.1/src/tentaclio/credentials/env.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/credentials/injection.py` & `tentaclio-1.2.1/src/tentaclio/credentials/injection.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/credentials/reader.py` & `tentaclio-1.2.1/src/tentaclio/credentials/reader.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/databases/db_registry.py` & `tentaclio-1.2.1/src/tentaclio/databases/db_registry.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/fs/api.py` & `tentaclio-1.2.1/src/tentaclio/fs/api.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/fs/copier.py` & `tentaclio-1.2.1/src/tentaclio/fs/copier.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/fs/copiers.py` & `tentaclio-1.2.1/src/tentaclio/fs/copiers.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/fs/remover.py` & `tentaclio-1.2.1/src/tentaclio/fs/remover.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/fs/scanner.py` & `tentaclio-1.2.1/src/tentaclio/fs/scanner.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/fs/scanners.py` & `tentaclio-1.2.1/src/tentaclio/fs/scanners.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/hooks/slack_hook.py` & `tentaclio-1.2.1/src/tentaclio/hooks/slack_hook.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/protocols.py` & `tentaclio-1.2.1/src/tentaclio/protocols.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/registry.py` & `tentaclio-1.2.1/src/tentaclio/registry.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/streams/api.py` & `tentaclio-1.2.1/src/tentaclio/streams/api.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/streams/base_stream.py` & `tentaclio-1.2.1/src/tentaclio/streams/base_stream.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/streams/csv_db_stream.py` & `tentaclio-1.2.1/src/tentaclio/streams/csv_db_stream.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/streams/stream_client_handler.py` & `tentaclio-1.2.1/src/tentaclio/streams/stream_client_handler.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/streams/stream_registry.py` & `tentaclio-1.2.1/src/tentaclio/streams/stream_registry.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio/urls.py` & `tentaclio-1.2.1/src/tentaclio/urls.py`

 * *Files identical despite different names*

### Comparing `tentaclio-1.2.0/src/tentaclio.egg-info/PKG-INFO` & `tentaclio-1.2.1/src/tentaclio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tentaclio
-Version: 1.2.0
+Version: 1.2.1
 Summary: Unification of data connectors for distributed data tasks
 Home-page: https://github.com/octoenergy/tentaclio
 Author: Octopus Energy
 Author-email: nerds@octoenergy.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tentaclio-1.2.0/src/tentaclio.egg-info/SOURCES.txt` & `tentaclio-1.2.1/src/tentaclio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

