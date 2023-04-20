# Comparing `tmp/dbqq-1.3.2.tar.gz` & `tmp/dbqq-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbqq-1.3.2.tar", last modified: Tue Apr 18 09:58:53 2023, max compression
+gzip compressed data, was "dbqq-1.3.3.tar", last modified: Thu Apr 20 06:11:39 2023, max compression
```

## Comparing `dbqq-1.3.2.tar` & `dbqq-1.3.3.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.651556 dbqq-1.3.2/
--rw-rw-rw-   0        0        0    14132 2023-04-18 09:58:53.648543 dbqq-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    13402 2023-04-18 08:39:10.000000 dbqq-1.3.2/README.md
--rw-rw-rw-   0        0        0     1083 2023-04-18 08:39:10.000000 dbqq-1.3.2/license.md
--rw-rw-rw-   0        0        0     1289 2023-04-18 09:57:42.000000 dbqq-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 09:58:53.652558 dbqq-1.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.519047 dbqq-1.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.546056 dbqq-1.3.2/src/dbqq/
--rw-rw-rw-   0        0        0      134 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.578095 dbqq-1.3.2/src/dbqq/cli/
--rw-rw-rw-   0        0        0      967 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/cli/clean_connections.py
--rw-rw-rw-   0        0        0      713 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/cli/initialize_connections.py
--rw-rw-rw-   0        0        0     1422 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/cli/run_query.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.599545 dbqq-1.3.2/src/dbqq/connectors/
--rw-rw-rw-   0        0        0     1017 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/connectors/__init__.py
--rw-rw-rw-   0        0        0     7038 2023-04-18 08:39:55.000000 dbqq-1.3.2/src/dbqq/connectors/_base.py
--rw-rw-rw-   0        0        0     1778 2023-04-18 08:40:16.000000 dbqq-1.3.2/src/dbqq/connectors/_polar_connector.py
--rw-rw-rw-   0        0        0     5634 2023-04-18 09:58:15.000000 dbqq-1.3.2/src/dbqq/connectors/databricks.py
--rw-rw-rw-   0        0        0     2906 2023-04-18 09:58:15.000000 dbqq-1.3.2/src/dbqq/connectors/mssql.py
--rw-rw-rw-   0        0        0     4747 2023-04-18 09:58:15.000000 dbqq-1.3.2/src/dbqq/connectors/oracle.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.601545 dbqq-1.3.2/src/dbqq/enums/
--rw-rw-rw-   0        0        0       46 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.610534 dbqq-1.3.2/src/dbqq/enums/parsed/
--rw-rw-rw-   0        0        0       40 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/enums/parsed/__init__.py
--rw-rw-rw-   0        0        0      822 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/enums/parsed/sql.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.617548 dbqq-1.3.2/src/dbqq/security/
--rw-rw-rw-   0        0        0      112 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.633540 dbqq-1.3.2/src/dbqq/security/cli/
--rw-rw-rw-   0        0        0       54 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/cli/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/cli/decrypt_yaml.py
--rw-rw-rw-   0        0        0     1036 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/cli/encrypt_yaml.py
--rw-rw-rw-   0        0        0     1708 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/cli/write_keys.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.645549 dbqq-1.3.2/src/dbqq/security/functions/
--rw-rw-rw-   0        0        0      119 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/functions/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/functions/_functions.py
--rw-rw-rw-   0        0        0     4166 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/functions/_yaml.py
--rw-rw-rw-   0        0        0     2330 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/security/helpers.py
--rw-rw-rw-   0        0        0     5311 2023-04-18 08:39:10.000000 dbqq-1.3.2/src/dbqq/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:53.567082 dbqq-1.3.2/src/dbqq.egg-info/
--rw-rw-rw-   0        0        0    14132 2023-04-18 09:58:53.000000 dbqq-1.3.2/src/dbqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      975 2023-04-18 09:58:53.000000 dbqq-1.3.2/src/dbqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 09:58:53.000000 dbqq-1.3.2/src/dbqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      339 2023-04-18 09:58:53.000000 dbqq-1.3.2/src/dbqq.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2023-04-18 09:58:53.000000 dbqq-1.3.2/src/dbqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-18 09:58:53.000000 dbqq-1.3.2/src/dbqq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 06:11:39.170848 dbqq-1.3.3/
+-rw-rw-rw-   0        0        0    14132 2023-04-20 06:11:39.168846 dbqq-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13402 2023-04-20 05:41:23.000000 dbqq-1.3.3/README.md
+-rw-rw-rw-   0        0        0     1083 2023-04-20 05:41:23.000000 dbqq-1.3.3/license.md
+-rw-rw-rw-   0        0        0     1289 2023-04-20 06:08:09.000000 dbqq-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 06:11:39.170848 dbqq-1.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 06:11:39.028815 dbqq-1.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 06:11:39.059816 dbqq-1.3.3/src/dbqq/
+-rw-rw-rw-   0        0        0      129 2023-04-20 06:00:38.000000 dbqq-1.3.3/src/dbqq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:11:39.097824 dbqq-1.3.3/src/dbqq/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-20 06:01:06.000000 dbqq-1.3.3/src/dbqq/cli/__init__.py
+-rw-rw-rw-   0        0        0      967 2023-04-20 05:41:23.000000 dbqq-1.3.3/src/dbqq/cli/clean_connections.py
+-rw-rw-rw-   0        0        0      713 2023-04-20 05:52:12.000000 dbqq-1.3.3/src/dbqq/cli/initialize_connections.py
+-rw-rw-rw-   0        0        0     1422 2023-04-20 05:41:23.000000 dbqq-1.3.3/src/dbqq/cli/run_query.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:11:39.118836 dbqq-1.3.3/src/dbqq/connectors/
+-rw-rw-rw-   0        0        0     1017 2023-04-20 05:41:23.000000 dbqq-1.3.3/src/dbqq/connectors/__init__.py
+-rw-rw-rw-   0        0        0     7038 2023-04-20 05:41:23.000000 dbqq-1.3.3/src/dbqq/connectors/_base.py
+-rw-rw-rw-   0        0        0     1778 2023-04-20 05:41:23.000000 dbqq-1.3.3/src/dbqq/connectors/_polar_connector.py
+-rw-rw-rw-   0        0        0     5634 2023-04-20 06:10:23.000000 dbqq-1.3.3/src/dbqq/connectors/databricks.py
+-rw-rw-rw-   0        0        0     2906 2023-04-20 06:08:35.000000 dbqq-1.3.3/src/dbqq/connectors/mssql.py
+-rw-rw-rw-   0        0        0     4747 2023-04-20 06:08:35.000000 dbqq-1.3.3/src/dbqq/connectors/oracle.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:11:39.120835 dbqq-1.3.3/src/dbqq/enums/
+-rw-rw-rw-   0        0        0       46 2023-04-20 05:41:23.000000 dbqq-1.3.3/src/dbqq/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:11:39.127839 dbqq-1.3.3/src/dbqq/enums/parsed/
+-rw-rw-rw-   0        0        0       40 2023-04-20 05:41:23.000000 dbqq-1.3.3/src/dbqq/enums/parsed/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-04-20 05:41:23.000000 dbqq-1.3.3/src/dbqq/enums/parsed/sql.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:11:39.134839 dbqq-1.3.3/src/dbqq/security/
+-rw-rw-rw-   0        0        0       86 2023-04-20 06:00:52.000000 dbqq-1.3.3/src/dbqq/security/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:11:39.150842 dbqq-1.3.3/src/dbqq/security/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-20 06:01:13.000000 dbqq-1.3.3/src/dbqq/security/cli/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-20 05:47:05.000000 dbqq-1.3.3/src/dbqq/security/cli/decrypt_yaml.py
+-rw-rw-rw-   0        0        0     1036 2023-04-20 06:02:42.000000 dbqq-1.3.3/src/dbqq/security/cli/encrypt_yaml.py
+-rw-rw-rw-   0        0        0     1707 2023-04-20 06:08:48.000000 dbqq-1.3.3/src/dbqq/security/cli/write_keys.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:11:39.163847 dbqq-1.3.3/src/dbqq/security/functions/
+-rw-rw-rw-   0        0        0      119 2023-04-20 05:41:23.000000 dbqq-1.3.3/src/dbqq/security/functions/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-04-20 05:41:23.000000 dbqq-1.3.3/src/dbqq/security/functions/_functions.py
+-rw-rw-rw-   0        0        0     4166 2023-04-20 06:03:15.000000 dbqq-1.3.3/src/dbqq/security/functions/_yaml.py
+-rw-rw-rw-   0        0        0     2330 2023-04-20 05:41:23.000000 dbqq-1.3.3/src/dbqq/security/helpers.py
+-rw-rw-rw-   0        0        0     5311 2023-04-20 05:41:23.000000 dbqq-1.3.3/src/dbqq/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:11:39.082819 dbqq-1.3.3/src/dbqq.egg-info/
+-rw-rw-rw-   0        0        0    14132 2023-04-20 06:11:38.000000 dbqq-1.3.3/src/dbqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2023-04-20 06:11:39.000000 dbqq-1.3.3/src/dbqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 06:11:38.000000 dbqq-1.3.3/src/dbqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      339 2023-04-20 06:11:38.000000 dbqq-1.3.3/src/dbqq.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2023-04-20 06:11:38.000000 dbqq-1.3.3/src/dbqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-20 06:11:38.000000 dbqq-1.3.3/src/dbqq.egg-info/top_level.txt
```

### Comparing `dbqq-1.3.2/PKG-INFO` & `dbqq-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbqq
-Version: 1.3.2
+Version: 1.3.3
 Summary: quickly connect to and query databases
 Author-email: Chris Mamon <chrisam1993@live.com>
 Project-URL: Homepage, https://github.com/Chr1sC0de/database-quick-query
 Project-URL: Bug Tracker, https://github.com/Chr1sC0de/database-quick-query/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dbqq-1.3.2/README.md` & `dbqq-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/license.md` & `dbqq-1.3.3/license.md`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/pyproject.toml` & `dbqq-1.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires      = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dbqq"
 description = "quickly connect to and query databases"
-version = "1.3.2"
+version = "1.3.3"
 readme = "README.md"
 dependencies = [
   "tabulate",
   "rsa",
   "pyaml",
   "polars",
   "databricks-sql-connector",
@@ -31,13 +31,13 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Chr1sC0de/database-quick-query"
 "Bug Tracker" = "https://github.com/Chr1sC0de/database-quick-query/issues"
 
 [project.scripts]
-dbqq-write-keys = "dbqq.security.cli.write_keys:run"
-dbqq-encrypt-yaml = "dbqq.security.cli.encrypt_yaml:run"
-dbqq-decrypt-yaml = "dbqq.security.cli.decrypt_yaml:run"
 dbqq-run-sql = "dbqq.cli.run_query:run"
 dbqq-clean-connections = "dbqq.cli.clean_connections:run"
 dbqq-initialize-connections = "dbqq.cli.initialize_connections:run"
+dbqq-write-keys = "dbqq.security.cli.write_keys:run"
+dbqq-encrypt-yaml = "dbqq.security.cli.encrypt_yaml:run"
+dbqq-decrypt-yaml = "dbqq.security.cli.decrypt_yaml:run"
```

### Comparing `dbqq-1.3.2/src/dbqq/cli/clean_connections.py` & `dbqq-1.3.3/src/dbqq/cli/clean_connections.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/cli/initialize_connections.py` & `dbqq-1.3.3/src/dbqq/cli/initialize_connections.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/cli/run_query.py` & `dbqq-1.3.3/src/dbqq/cli/run_query.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/connectors/__init__.py` & `dbqq-1.3.3/src/dbqq/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/connectors/_base.py` & `dbqq-1.3.3/src/dbqq/connectors/_base.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/connectors/_polar_connector.py` & `dbqq-1.3.3/src/dbqq/connectors/_polar_connector.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/connectors/databricks.py` & `dbqq-1.3.3/src/dbqq/connectors/databricks.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/connectors/mssql.py` & `dbqq-1.3.3/src/dbqq/connectors/mssql.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/connectors/oracle.py` & `dbqq-1.3.3/src/dbqq/connectors/oracle.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/enums/parsed/sql.py` & `dbqq-1.3.3/src/dbqq/enums/parsed/sql.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/security/cli/decrypt_yaml.py` & `dbqq-1.3.3/src/dbqq/security/cli/decrypt_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/security/cli/encrypt_yaml.py` & `dbqq-1.3.3/src/dbqq/security/cli/encrypt_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/security/cli/write_keys.py` & `dbqq-1.3.3/src/dbqq/security/cli/write_keys.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 parser: argparse.ArgumentParser = argparse.ArgumentParser(
     description="generate public and private keys"
 )
 
 parser.add_argument(
-    "--key_length", "-k", type=int, default=1024, help="the length of th key"
+    "--key_length", "-k", type=int, default=512, help="the length of th key"
 )
 
 parser.add_argument(
     "--location",
     "-l",
     type=pt.Path,
     default=".",
```

### Comparing `dbqq-1.3.2/src/dbqq/security/functions/_functions.py` & `dbqq-1.3.3/src/dbqq/security/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/security/functions/_yaml.py` & `dbqq-1.3.3/src/dbqq/security/functions/_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/security/helpers.py` & `dbqq-1.3.3/src/dbqq/security/helpers.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq/utils.py` & `dbqq-1.3.3/src/dbqq/utils.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.2/src/dbqq.egg-info/PKG-INFO` & `dbqq-1.3.3/src/dbqq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbqq
-Version: 1.3.2
+Version: 1.3.3
 Summary: quickly connect to and query databases
 Author-email: Chris Mamon <chrisam1993@live.com>
 Project-URL: Homepage, https://github.com/Chr1sC0de/database-quick-query
 Project-URL: Bug Tracker, https://github.com/Chr1sC0de/database-quick-query/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dbqq-1.3.2/src/dbqq.egg-info/SOURCES.txt` & `dbqq-1.3.3/src/dbqq.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/dbqq/utils.py
 src/dbqq.egg-info/PKG-INFO
 src/dbqq.egg-info/SOURCES.txt
 src/dbqq.egg-info/dependency_links.txt
 src/dbqq.egg-info/entry_points.txt
 src/dbqq.egg-info/requires.txt
 src/dbqq.egg-info/top_level.txt
+src/dbqq/cli/__init__.py
 src/dbqq/cli/clean_connections.py
 src/dbqq/cli/initialize_connections.py
 src/dbqq/cli/run_query.py
 src/dbqq/connectors/__init__.py
 src/dbqq/connectors/_base.py
 src/dbqq/connectors/_polar_connector.py
 src/dbqq/connectors/databricks.py
```

