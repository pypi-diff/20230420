# Comparing `tmp/dbm_database_service-0.2.1.tar.gz` & `tmp/dbm_database_service-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbm_database_service-0.2.1.tar", max compression
+gzip compressed data, was "dbm_database_service-0.2.2.tar", max compression
```

## Comparing `dbm_database_service-0.2.1.tar` & `dbm_database_service-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-04-12 14:45:46.980021 dbm_database_service-0.2.1/dbm_database_service/__init__.py
--rw-r--r--   0        0        0     6676 2023-04-17 21:03:44.747568 dbm_database_service-0.2.1/dbm_database_service/connectors.py
--rw-r--r--   0        0        0     3208 2023-04-17 21:00:23.708163 dbm_database_service-0.2.1/dbm_database_service/managers.py
--rw-r--r--   0        0        0        0 2023-04-14 20:01:03.393096 dbm_database_service-0.2.1/dbm_database_service/models/__init__.py
--rw-r--r--   0        0        0     1612 2023-04-17 21:13:25.033005 dbm_database_service-0.2.1/dbm_database_service/models/column.py
--rw-r--r--   0        0        0      849 2023-04-17 21:13:25.022589 dbm_database_service-0.2.1/dbm_database_service/models/config.py
--rw-r--r--   0        0        0     1232 2023-04-17 21:13:25.043780 dbm_database_service-0.2.1/dbm_database_service/models/datatype.py
--rw-r--r--   0        0        0     1000 2023-04-17 21:13:25.053962 dbm_database_service-0.2.1/dbm_database_service/models/table.py
--rw-r--r--   0        0        0      655 2023-04-18 09:42:17.827994 dbm_database_service-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    13467 2023-04-18 09:36:53.242538 dbm_database_service-0.2.1/README.md
--rw-r--r--   0        0        0    13586 1970-01-01 00:00:00.000000 dbm_database_service-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-12 14:45:46.980021 dbm_database_service-0.2.2/dbm_database_service/__init__.py
+-rw-r--r--   0        0        0     6676 2023-04-17 21:03:44.747568 dbm_database_service-0.2.2/dbm_database_service/connectors.py
+-rw-r--r--   0        0        0     3336 2023-04-20 18:48:50.609857 dbm_database_service-0.2.2/dbm_database_service/managers.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:01:03.393096 dbm_database_service-0.2.2/dbm_database_service/models/__init__.py
+-rw-r--r--   0        0        0     1612 2023-04-17 21:13:25.033005 dbm_database_service-0.2.2/dbm_database_service/models/column.py
+-rw-r--r--   0        0        0      849 2023-04-17 21:13:25.022589 dbm_database_service-0.2.2/dbm_database_service/models/config.py
+-rw-r--r--   0        0        0     1232 2023-04-17 21:13:25.043780 dbm_database_service-0.2.2/dbm_database_service/models/datatype.py
+-rw-r--r--   0        0        0      932 2023-04-20 19:25:36.272678 dbm_database_service-0.2.2/dbm_database_service/models/table.py
+-rw-r--r--   0        0        0      655 2023-04-20 19:26:33.933196 dbm_database_service-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    13467 2023-04-18 09:36:53.242538 dbm_database_service-0.2.2/README.md
+-rw-r--r--   0        0        0    13586 1970-01-01 00:00:00.000000 dbm_database_service-0.2.2/PKG-INFO
```

### Comparing `dbm_database_service-0.2.1/dbm_database_service/connectors.py` & `dbm_database_service-0.2.2/dbm_database_service/connectors.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.1/dbm_database_service/managers.py` & `dbm_database_service-0.2.2/dbm_database_service/managers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from contextlib import contextmanager
 from mysql.connector import Error
 
 from dbm_database_service.models.column import Column
 from dbm_database_service.models.table import Table
+from dbm_database_service.connectors import get_connection_pool
+
+from pathlib import Path
 
 
 class MySQLDatabaseManager:
     def __init__(self, connection_pool) -> None:
         self._connection_pool = connection_pool
 
     @contextmanager
@@ -70,7 +73,9 @@
 
     def dev_console(self, sql: str) -> None:
         """ Utility made for custom development using sql syntax"""
         with self._get_cursor_object() as cur:
             cur.execute(str(sql))
             return cur.fetchall()
 
+dbm = MySQLDatabaseManager(get)
+
```

### Comparing `dbm_database_service-0.2.1/dbm_database_service/models/column.py` & `dbm_database_service-0.2.2/dbm_database_service/models/column.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.1/dbm_database_service/models/config.py` & `dbm_database_service-0.2.2/dbm_database_service/models/config.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.1/dbm_database_service/models/datatype.py` & `dbm_database_service-0.2.2/dbm_database_service/models/datatype.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.1/dbm_database_service/models/table.py` & `dbm_database_service-0.2.2/dbm_database_service/models/table.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,15 @@
     name: str
     columns: list[Column]
     if_not_exist: bool = False
     temporary: bool = False
 
     def __str__(self) -> str:
         """ Will be parsed in other objects. Outcome is valid SQL Create Table expression """
-        return f"create{' temporary' if self.temporary else ''} table" \
-               f"{' if not exists' if self.if_not_exist else ''}" \
-               f" {self.name}(" \
-               f"{', '.join([str(c) for c in self.columns])});" \
+        return f"create{' temporary' if self.temporary else ''} table{' if not exists' if self.if_not_exist else ''} {self.name}({', '.join([str(c) for c in self.columns])});"
 
 
     def drop_statement(self) -> str:
         """ Auxiliary method, that returns expression of sql drop table if exist with name stored in instance """
         return f"drop table if exists {self.name}"
 
     def alter_statement(self) -> str:
```

### Comparing `dbm_database_service-0.2.1/pyproject.toml` & `dbm_database_service-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbm-database-service"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Smolke <d.smolczynski1@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dbm_database_service"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dbm_database_service-0.2.1/README.md` & `dbm_database_service-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.1/PKG-INFO` & `dbm_database_service-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-database-service
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Smolke
 Author-email: d.smolczynski1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: easyvalid-data-validator (>=0.1.1,<0.2.0)
```

