# Comparing `tmp/ibm_db_sa-0.3.9.tar.gz` & `tmp/ibm_db_sa-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm_db_sa-0.3.9.tar", last modified: Thu Mar  2 07:29:29 2023, max compression
+gzip compressed data, was "ibm_db_sa-0.4.0.tar", last modified: Thu Apr 20 11:24:53 2023, max compression
```

## Comparing `ibm_db_sa-0.3.9.tar` & `ibm_db_sa-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 07:29:29.455815 ibm_db_sa-0.3.9/
--rw-rw-rw-   0        0        0     3907 2023-02-27 10:10:01.000000 ibm_db_sa-0.3.9/CHANGES.md
--rw-rw-rw-   0        0        0     9219 2023-02-27 09:44:15.000000 ibm_db_sa-0.3.9/LICENSE
--rw-rw-rw-   0        0        0      100 2023-02-27 09:44:15.000000 ibm_db_sa-0.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4608 2023-03-02 07:29:29.457848 ibm_db_sa-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     3882 2023-02-27 09:44:15.000000 ibm_db_sa-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 07:29:29.397763 ibm_db_sa-0.3.9/ibm_db_sa/
--rw-rw-rw-   0        0        0     1857 2023-02-27 10:10:01.000000 ibm_db_sa-0.3.9/ibm_db_sa/__init__.py
--rw-rw-rw-   0        0        0    33924 2023-02-27 09:44:15.000000 ibm_db_sa-0.3.9/ibm_db_sa/base.py
--rw-rw-rw-   0        0        0     9602 2023-02-27 09:44:15.000000 ibm_db_sa-0.3.9/ibm_db_sa/ibm_db.py
--rw-rw-rw-   0        0        0      379 2023-02-27 09:44:15.000000 ibm_db_sa-0.3.9/ibm_db_sa/ibm_db_as400.py
--rw-rw-rw-   0        0        0     6676 2023-02-27 09:44:15.000000 ibm_db_sa-0.3.9/ibm_db_sa/pyodbc.py
--rw-rw-rw-   0        0        0    56621 2023-02-27 09:44:15.000000 ibm_db_sa-0.3.9/ibm_db_sa/reflection.py
--rw-rw-rw-   0        0        0     2373 2023-02-27 09:44:15.000000 ibm_db_sa-0.3.9/ibm_db_sa/requirements.py
--rw-rw-rw-   0        0        0     4209 2023-02-27 09:44:15.000000 ibm_db_sa-0.3.9/ibm_db_sa/zxjdbc.py
-drwxrwxrwx   0        0        0        0 2023-03-02 07:29:29.434753 ibm_db_sa-0.3.9/ibm_db_sa.egg-info/
--rw-rw-rw-   0        0        0     4608 2023-03-02 07:29:29.000000 ibm_db_sa-0.3.9/ibm_db_sa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      544 2023-03-02 07:29:29.000000 ibm_db_sa-0.3.9/ibm_db_sa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 07:29:29.000000 ibm_db_sa-0.3.9/ibm_db_sa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      633 2023-03-02 07:29:29.000000 ibm_db_sa-0.3.9/ibm_db_sa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-02 07:29:29.000000 ibm_db_sa-0.3.9/ibm_db_sa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       32 2023-03-02 07:29:29.000000 ibm_db_sa-0.3.9/ibm_db_sa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-02 07:29:29.000000 ibm_db_sa-0.3.9/ibm_db_sa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      551 2023-02-27 09:44:15.000000 ibm_db_sa-0.3.9/run_tests.py
--rw-rw-rw-   0        0        0      360 2023-03-02 07:29:29.463832 ibm_db_sa-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     2627 2023-03-02 07:25:43.000000 ibm_db_sa-0.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-02 07:29:29.451807 ibm_db_sa-0.3.9/test/
--rw-rw-rw-   0        0        0        0 2023-02-27 09:44:16.000000 ibm_db_sa-0.3.9/test/__init__.py
--rw-rw-rw-   0        0        0     1312 2023-02-27 09:44:16.000000 ibm_db_sa-0.3.9/test/test_out_parameters.py
--rw-rw-rw-   0        0        0       42 2023-02-27 09:44:16.000000 ibm_db_sa-0.3.9/test/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:24:53.182203 ibm_db_sa-0.4.0/
+-rw-rw-rw-   0        0        0     4714 2023-04-20 10:31:41.000000 ibm_db_sa-0.4.0/CHANGES.md
+-rw-rw-rw-   0        0        0     9219 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      100 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5256 2023-04-20 11:24:53.184273 ibm_db_sa-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4530 2023-04-20 10:29:22.000000 ibm_db_sa-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 11:24:53.103208 ibm_db_sa-0.4.0/ibm_db_sa/
+-rw-rw-rw-   0        0        0     1857 2023-04-20 10:29:41.000000 ibm_db_sa-0.4.0/ibm_db_sa/__init__.py
+-rw-rw-rw-   0        0        0    33995 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/ibm_db_sa/base.py
+-rw-rw-rw-   0        0        0    10140 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/ibm_db_sa/ibm_db.py
+-rw-rw-rw-   0        0        0      587 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/ibm_db_sa/ibm_db_as400.py
+-rw-rw-rw-   0        0        0     6676 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/ibm_db_sa/pyodbc.py
+-rw-rw-rw-   0        0        0    55827 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/ibm_db_sa/reflection.py
+-rw-rw-rw-   0        0        0     2373 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/ibm_db_sa/requirements.py
+-rw-rw-rw-   0        0        0     4209 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/ibm_db_sa/zxjdbc.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:24:53.156207 ibm_db_sa-0.4.0/ibm_db_sa.egg-info/
+-rw-rw-rw-   0        0        0     5256 2023-04-20 11:24:52.000000 ibm_db_sa-0.4.0/ibm_db_sa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2023-04-20 11:24:52.000000 ibm_db_sa-0.4.0/ibm_db_sa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 11:24:52.000000 ibm_db_sa-0.4.0/ibm_db_sa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      633 2023-04-20 11:24:52.000000 ibm_db_sa-0.4.0/ibm_db_sa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-20 11:24:52.000000 ibm_db_sa-0.4.0/ibm_db_sa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       32 2023-04-20 11:24:52.000000 ibm_db_sa-0.4.0/ibm_db_sa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-20 11:24:52.000000 ibm_db_sa-0.4.0/ibm_db_sa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      551 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/run_tests.py
+-rw-rw-rw-   0        0        0      360 2023-04-20 11:24:53.188695 ibm_db_sa-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2627 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:24:53.177319 ibm_db_sa-0.4.0/test/
+-rw-rw-rw-   0        0        0        0 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/test/__init__.py
+-rw-rw-rw-   0        0        0     1312 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/test/test_out_parameters.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 09:09:43.000000 ibm_db_sa-0.4.0/test/test_suite.py
```

### Comparing `ibm_db_sa-0.3.9/LICENSE` & `ibm_db_sa-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm_db_sa-0.3.9/PKG-INFO` & `ibm_db_sa-0.4.0/ibm_db_sa.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ibm_db_sa
-Version: 0.3.9
+Name: ibm-db-sa
+Version: 0.4.0
 Summary: SQLAlchemy support for IBM Data Servers
 Home-page: http://pypi.python.org/pypi/ibm_db_sa/
 Download-URL: http://code.google.com/p/ibm-db/downloads/list
 Author: IBM Application Development Team
 Author-email: opendev@us.ibm.com
 License: Apache License 2.0
 Keywords: sqlalchemy database interface IBM Data Servers DB2 Informix IDS
@@ -20,20 +20,20 @@
 IBM_DB_SA
 =========
 
 The IBM_DB_SA adapter provides the Python/SQLAlchemy interface to IBM Data Servers.
 
 Version
 --------
-0.3.9 (2023/02/27)
+0.4.0 (2023/04/20)
 
 Prerequisites
 --------------
 1. Install Python 2.7 or newer versions except python 3.3 or Jython 2.5.x .
-2. SQLAlchemy version between 0.7.3 - 1.4.x.
+2. SQLAlchemy version between 0.7.3 - 2.0.x.
 3. IBM_DB driver and IBM_DB_DBI wrapper 1.0.1 or higher.
 ```
    Install ibm_db driver with below commands:
 	    Linux and Windows: 
 	   	   pip install ibm_db
 	    Mac:
 		   pip install --no-cache-dir ibm_db
@@ -101,14 +101,32 @@
 Supported Databases
 -------------------
 - IBM DB2 Universal Database for Linux/Unix/Windows versions 9.7 onwards 
 - IBM Db2 on Cloud
 - IBM Db2 on ZOS
 - IBM Db2 on Iseries
 
+Note
+-------------------------------------------------------------
+By default, all tables and schemas stored in a Db2 database are created
+using capital letters only.
+However, if you have a table name in lowercase letters, you can still reference
+it by enclosing the name in single quotes inside double quotes.
+For example
+```
+	if users table is in small letter inside database
+	So, you can use single quotes "'users'".
+	If you will not use single quotes such as "users", it will
+	be refered as "USERS".
+
+	metadata = sqlalchemy.MetaData(schema="schema1")
+	table = sqlalchemy.Table("'users'", metadata, autoload_with=engine)
+
+```
+
 Known Limitations in ibm_db_sa adapter for DB2 databases
 -------------------------------------------------------------
 1) Non-standard SQL queries are not supported. e.g. "SELECT ? FROM TAB1"
 2) For updations involving primary/foreign key references, the entries should be made in correct order. Integrity check is always on and thus the primary keys referenced by the foreign keys in the referencing tables should always exist in the parent table.
 3) Unique key which contains nullable column not supported
 4) UPDATE CASCADE for foreign keys not supported
 5) DEFERRABLE INITIALLY deferred not supported
```

### Comparing `ibm_db_sa-0.3.9/README.md` & `ibm_db_sa-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 IBM_DB_SA
 =========
 
 The IBM_DB_SA adapter provides the Python/SQLAlchemy interface to IBM Data Servers.
 
 Version
 --------
-0.3.9 (2023/02/27)
+0.4.0 (2023/04/20)
 
 Prerequisites
 --------------
 1. Install Python 2.7 or newer versions except python 3.3 or Jython 2.5.x .
-2. SQLAlchemy version between 0.7.3 - 1.4.x.
+2. SQLAlchemy version between 0.7.3 - 2.0.x.
 3. IBM_DB driver and IBM_DB_DBI wrapper 1.0.1 or higher.
 ```
    Install ibm_db driver with below commands:
 	    Linux and Windows: 
 	   	   pip install ibm_db
 	    Mac:
 		   pip install --no-cache-dir ibm_db
@@ -82,14 +82,32 @@
 Supported Databases
 -------------------
 - IBM DB2 Universal Database for Linux/Unix/Windows versions 9.7 onwards 
 - IBM Db2 on Cloud
 - IBM Db2 on ZOS
 - IBM Db2 on Iseries
 
+Note
+-------------------------------------------------------------
+By default, all tables and schemas stored in a Db2 database are created
+using capital letters only.
+However, if you have a table name in lowercase letters, you can still reference
+it by enclosing the name in single quotes inside double quotes.
+For example
+```
+	if users table is in small letter inside database
+	So, you can use single quotes "'users'".
+	If you will not use single quotes such as "users", it will
+	be refered as "USERS".
+
+	metadata = sqlalchemy.MetaData(schema="schema1")
+	table = sqlalchemy.Table("'users'", metadata, autoload_with=engine)
+
+```
+
 Known Limitations in ibm_db_sa adapter for DB2 databases
 -------------------------------------------------------------
 1) Non-standard SQL queries are not supported. e.g. "SELECT ? FROM TAB1"
 2) For updations involving primary/foreign key references, the entries should be made in correct order. Integrity check is always on and thus the primary keys referenced by the foreign keys in the referencing tables should always exist in the parent table.
 3) Unique key which contains nullable column not supported
 4) UPDATE CASCADE for foreign keys not supported
 5) DEFERRABLE INITIALLY deferred not supported
```

### Comparing `ibm_db_sa-0.3.9/ibm_db_sa/__init__.py` & `ibm_db_sa-0.4.0/ibm_db_sa/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # | KIND, either express or implied. See the License for the specific        |
 # | language governing permissions and limitations under the License.        |
 # +--------------------------------------------------------------------------+
 # | Authors: Alex Pitigoi, Abhigyan Agrawal, Rahul Priyadarshi               |
 # | Contributors: Jaimy Azle, Mike Bayer                                     |
 # +--------------------------------------------------------------------------+
 
-__version__ = '0.3.9'
+__version__ = '0.4.0'
 
 from . import ibm_db, pyodbc, base
 
 
 # default dialect
 base.dialect = ibm_db.dialect
```

### Comparing `ibm_db_sa-0.3.9/ibm_db_sa/base.py` & `ibm_db_sa-0.4.0/ibm_db_sa/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -667,16 +667,18 @@
     colspecs = colspecs
     ischema_names = ischema_names
     supports_char_length = False
     supports_unicode_statements = False
     supports_unicode_binds = False
     if SA_Version < [1, 4]:
         returns_unicode_strings = False
-    else:
+    elif SA_Version < [2, 0]:
         returns_unicode_strings = sa_types.String.RETURNS_CONDITIONAL
+    else:
+        returns_unicode_strings = True
     postfetch_lastrowid = True
     supports_sane_rowcount = True
     supports_sane_multi_rowcount = True
     supports_native_decimal = False
     supports_native_boolean = False
     supports_statement_cache = False
     preexecute_sequences = False
```

### Comparing `ibm_db_sa-0.3.9/ibm_db_sa/ibm_db.py` & `ibm_db_sa-0.4.0/ibm_db_sa/ibm_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,38 +13,50 @@
 # | KIND, either express or implied. See the License for the specific        |
 # | language governing permissions and limitations under the License.        |
 # +--------------------------------------------------------------------------+
 # | Authors: Alex Pitigoi, Abhigyan Agrawal, Rahul Priyadarshi,Abhinav Radke |
 # | Contributors: Jaimy Azle, Mike Bayer,Hemlata Bhatt                       |
 # +--------------------------------------------------------------------------+
 
-from .base import DB2ExecutionContext, DB2Dialect
-from sqlalchemy import processors, types as sa_types, util
 from sqlalchemy import __version__ as SA_Version
+SA_Version = [int(ver_token) for ver_token in SA_Version.split('.')[0:2]]
+
+from .base import DB2ExecutionContext, DB2Dialect
+
+if SA_Version < [2,0]:
+    from sqlalchemy import processors, types as sa_types, util
+else:
+    from sqlalchemy import types as sa_types, util
+    from sqlalchemy.engine import processors
+
 from sqlalchemy.exc import ArgumentError
 
-SA_Version = [int(ver_token) for ver_token in SA_Version.split('.')[0:2]]
 SQL_TXN_READ_UNCOMMITTED = 1
 SQL_TXN_READ_COMMITTED = 2
 SQL_TXN_REPEATABLE_READ = 4
 SQL_TXN_SERIALIZABLE = 8
 SQL_ATTR_TXN_ISOLATION = 108
 
 if SA_Version < [0, 8]:
     from sqlalchemy.engine import base
 else:
     from sqlalchemy.engine import result as _result
 
 
 class _IBM_Numeric_ibm_db(sa_types.Numeric):
     def result_processor(self, dialect, coltype):
+        def to_float(value):
+            if value is None:
+                return None
+            else:
+                return float(value)
         if self.asdecimal:
             return None
         else:
-            return processors.to_float
+            return to_float
 
 
 class DB2ExecutionContext_ibm_db(DB2ExecutionContext):
     _callproc_result = None
     _out_parameters = None
 
     def get_lastrowid(self):
@@ -99,20 +111,28 @@
     colspecs = util.update_copy(
         DB2Dialect.colspecs,
         {
             sa_types.Numeric: _IBM_Numeric_ibm_db
         }
     )
 
-    @classmethod
-    def dbapi(cls):
-        """ Returns: the underlying DBAPI driver module
-        """
-        import ibm_db_dbi as module
-        return module
+    if SA_Version < [2, 0]:
+        @classmethod
+        def dbapi(cls):
+            """ Returns: the underlying DBAPI driver module
+            """
+            import ibm_db_dbi as module
+            return module
+    else:
+        @classmethod
+        def import_dbapi(cls):
+            """ Returns: the underlying DBAPI driver module
+            """
+            import ibm_db_dbi as module
+            return module
 
     def do_execute(self, cursor, statement, parameters, context=None):
         if context and context._out_parameters:
             statement = statement.split('(', 1)[0].split()[1]
             context._callproc_result = cursor.callproc(statement, parameters)
         else:
             cursor.execute(statement, parameters)
```

### Comparing `ibm_db_sa-0.3.9/ibm_db_sa/pyodbc.py` & `ibm_db_sa-0.4.0/ibm_db_sa/pyodbc.py`

 * *Files identical despite different names*

### Comparing `ibm_db_sa-0.3.9/ibm_db_sa/reflection.py` & `ibm_db_sa-0.4.0/ibm_db_sa/reflection.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # | Contributors: Jaimy Azle, Mike Bayer,Hemlata Bhatt                       |
 # +--------------------------------------------------------------------------+
 import sys
 from sqlalchemy import types as sa_types
 from sqlalchemy import sql, util, join
 from sqlalchemy import Table, MetaData, Column
 from sqlalchemy.engine import reflection
+from sqlalchemy import *
 import re
 import codecs
 from sys import version_info
 
 
 class CoerceUnicode(sa_types.TypeDecorator):
     impl = sa_types.Unicode
@@ -171,114 +172,115 @@
       Column("SEQSCHEMA", CoerceUnicode, key="seqschema"),
       Column("SEQNAME", CoerceUnicode, key="seqname"),
       schema="SYSCAT")
 
     def has_table(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(
                             schema or self.default_schema_name)
-        table_name = self.denormalize_name(table_name)
+        if table_name.startswith("'") and table_name.endswith("'"):
+            table_name = table_name.replace("'", "")
+            table_name = self.normalize_name(table_name)
+        else:
+            table_name = self.denormalize_name(table_name)
         if current_schema:
             whereclause = sql.and_(self.sys_tables.c.tabschema == current_schema,
                                    self.sys_tables.c.tabname == table_name)
         else:
             whereclause = self.sys_tables.c.tabname == table_name
-        s = sql.select([self.sys_tables.c.tabname], whereclause)
+        s = sql.select(self.sys_tables.c.tabname).where(whereclause)
         c = connection.execute(s)
         return c.first() is not None
 
     def has_sequence(self, connection, sequence_name, schema=None):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         sequence_name = self.denormalize_name(sequence_name)
         if current_schema:
             whereclause = sql.and_(self.sys_sequences.c.seqschema == current_schema,
                                    self.sys_sequences.c.seqname == sequence_name)
         else:
             whereclause = self.sys_sequences.c.seqname == sequence_name
-        s = sql.select([self.sys_sequences.c.seqname], whereclause)
+        s = sql.select(self.sys_sequences.c.seqname).where(whereclause)
         c = connection.execute(s)
         return c.first() is not None
 
     @reflection.cache
     def get_sequence_names(self, connection, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         sys_sequence = self.sys_sequences
-        query = sql.select([sys_sequence.c.seqname],
-                           sys_sequence.c.seqschema == current_schema,
-                           order_by=[sys_sequence.c.seqschema, sys_sequence.c.seqname])
+        query = sql.select(sys_sequence.c.seqname).\
+            where(sys_sequence.c.seqschema == current_schema).\
+            order_by(sys_sequence.c.seqschema, sys_sequence.c.seqname)
         return [self.normalize_name(r[0]) for r in connection.execute(query)]
 
     @reflection.cache
     def get_schema_names(self, connection, **kw):
         sysschema = self.sys_schemas
-        query = sql.select([sysschema.c.schemaname],
-            sql.not_(sysschema.c.schemaname.like('SYS%')),
-            order_by=[sysschema.c.schemaname]
-        )
+        query = sql.select(sysschema.c.schemaname).\
+            where(not_(sysschema.c.schemaname.like('SYS%'))).\
+            order_by(sysschema.c.schemaname)
         return [self.normalize_name(r[0]) for r in connection.execute(query)]
 
     @reflection.cache
     def get_table_names(self, connection, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         systbl = self.sys_tables
-        query = sql.select([systbl.c.tabname]).\
-                    where(systbl.c.type == 'T').\
-                    where(systbl.c.tabschema == current_schema).\
-                    order_by(systbl.c.tabname)
+        query = sql.select(systbl.c.tabname).\
+            where(systbl.c.type == 'T').\
+            where(systbl.c.tabschema == current_schema).\
+            order_by(systbl.c.tabname)
         return [self.normalize_name(r[0]) for r in connection.execute(query)]
 
     @reflection.cache
     def get_table_comment(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         systbl = self.sys_tables
-        query = sql.select([systbl.c.remarks]). \
-            where(systbl.c.type == 'T'). \
-            where(systbl.c.tabschema == current_schema). \
+        query = sql.select(systbl.c.remarks).\
+            where(systbl.c.type == 'T').\
+            where(systbl.c.tabschema == current_schema).\
             where(systbl.c.tabname == table_name)
         c = connection.execute(query)
         return {'text': c.first()}
 
     @reflection.cache
     def get_view_names(self, connection, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
 
-        query = sql.select([self.sys_views.c.viewname]).\
+        query = sql.select(self.sys_views.c.viewname).\
             where(self.sys_views.c.viewschema == current_schema).\
             order_by(self.sys_views.c.viewname)
 
         return [self.normalize_name(r[0]) for r in connection.execute(query)]
 
     @reflection.cache
     def get_view_definition(self, connection, viewname, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         viewname = self.denormalize_name(viewname)
 
-        query = sql.select([self.sys_views.c.text]).\
+        query = sql.select(self.sys_views.c.text).\
             where(self.sys_views.c.viewschema == current_schema).\
             where(self.sys_views.c.viewname == viewname)
 
         return connection.execute(query).scalar()
 
     @reflection.cache
     def get_columns(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         syscols = self.sys_columns
 
-        query = sql.select([syscols.c.colname, syscols.c.typename,
+        query = sql.select(syscols.c.colname, syscols.c.typename,
                             syscols.c.defaultval, syscols.c.nullable,
                             syscols.c.length, syscols.c.scale,
-                            syscols.c.identity, syscols.c.generated, 
-                            syscols.c.remarks],
-              sql.and_(
+                            syscols.c.identity, syscols.c.generated,
+                            syscols.c.remarks).\
+            where(and_(
                   syscols.c.tabschema == current_schema,
-                  syscols.c.tabname == table_name
-                ),
-              order_by=[syscols.c.colno]
-            )
+                  syscols.c.tabname == table_name)).\
+            order_by(syscols.c.colno)
         sa_columns = []
         for r in connection.execute(query):
             coltype = r[1].upper()
             if coltype in ['DECIMAL', 'NUMERIC']:
                 coltype = self.ischema_names.get(coltype)(int(r[4]), int(r[5]))
             elif coltype in ['CHARACTER', 'CHAR', 'VARCHAR',
                             'GRAPHIC', 'VARGRAPHIC']:
@@ -303,20 +305,19 @@
 
     @reflection.cache
     def get_pk_constraint(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         sysindexes = self.sys_indexes
         col_finder = re.compile("(\w+)")
-        query = sql.select([sysindexes.c.colnames, sysindexes.c.indname],
-                           sql.and_(
-                               sysindexes.c.tabschema == current_schema,
-                               sysindexes.c.tabname == table_name,
-                               sysindexes.c.uniquerule == 'P'),
-                           order_by=[sysindexes.c.tabschema, sysindexes.c.tabname])
+        query = sql.select(sysindexes.c.colnames, sysindexes.c.indname).\
+            where(and_(sysindexes.c.tabschema == current_schema,
+                       sysindexes.c.tabname == table_name,
+                       sysindexes.c.uniquerule == 'P')).\
+            order_by(sysindexes.c.tabschema, sysindexes.c.tabname)
         pk_columns = []
         pk_name = None
         for r in connection.execute(query):
             cols = col_finder.findall(r[0])
             pk_columns.extend(cols)
             if not pk_name:
                 pk_name = self.normalize_name(r[1])
@@ -326,47 +327,45 @@
 
     @reflection.cache
     def get_primary_keys(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         syscols = self.sys_columns
         col_finder = re.compile("(\w+)")
-        query = sql.select([syscols.c.colname],
-              sql.and_(
+        query = sql.select(syscols.c.colname).\
+            where(and_(
                   syscols.c.tabschema == current_schema,
                   syscols.c.tabname == table_name,
                   syscols.c.keyseq > 0
-                ),
-              order_by=[syscols.c.tabschema, syscols.c.tabname]
-            )
+                )).\
+            order_by(syscols.c.tabschema, syscols.c.tabname)
         pk_columns = []
         for r in connection.execute(query):
             cols = col_finder.findall(r[0])
             pk_columns.extend(cols)
         return [self.normalize_name(col) for col in pk_columns]
 
     @reflection.cache
     def get_foreign_keys(self, connection, table_name, schema=None, **kw):
         default_schema = self.default_schema_name
         current_schema = self.denormalize_name(schema or default_schema)
         default_schema = self.normalize_name(default_schema)
         table_name = self.denormalize_name(table_name)
         sysfkeys = self.sys_foreignkeys
         systbl = self.sys_tables
-        query = sql.select([sysfkeys.c.fkname, sysfkeys.c.fktabschema, \
-                            sysfkeys.c.fktabname, sysfkeys.c.fkcolname, \
-                            sysfkeys.c.pkname, sysfkeys.c.pktabschema, \
-                            sysfkeys.c.pktabname, sysfkeys.c.pkcolname]) \
-            .select_from(
+        query = sql.select(sysfkeys.c.fkname, sysfkeys.c.fktabschema,
+                            sysfkeys.c.fktabname, sysfkeys.c.fkcolname,
+                            sysfkeys.c.pkname, sysfkeys.c.pktabschema,
+                            sysfkeys.c.pktabname, sysfkeys.c.pkcolname).\
+            select_from(
                 join(systbl,sysfkeys, systbl.c.tabname == sysfkeys.c.pktabname)
-            ) \
-            .where(systbl.c.type == 'T') \
-            .where(systbl.c.tabschema == current_schema) \
-            .where(sysfkeys.c.fktabname == table_name) \
-            .order_by(systbl.c.tabname)
+            ).where(systbl.c.type == 'T').\
+            where(systbl.c.tabschema == current_schema).\
+            where(sysfkeys.c.fktabname == table_name).\
+            order_by(systbl.c.tabname)
 
         fschema = {}
         for r in connection.execute(query):
             if not (r[0]) in fschema:
                 referred_schema = self.normalize_name(r[5])
 
                 # if no schema specified and referred schema here is the
@@ -389,24 +388,23 @@
     @reflection.cache
     def get_incoming_foreign_keys(self, connection, table_name, schema=None, **kw):
         default_schema = self.default_schema_name
         current_schema = self.denormalize_name(schema or default_schema)
         default_schema = self.normalize_name(default_schema)
         table_name = self.denormalize_name(table_name)
         sysfkeys = self.sys_foreignkeys
-        query = sql.select([sysfkeys.c.fkname, sysfkeys.c.fktabschema, \
-                            sysfkeys.c.fktabname, sysfkeys.c.fkcolname, \
-                            sysfkeys.c.pkname, sysfkeys.c.pktabschema, \
-                            sysfkeys.c.pktabname, sysfkeys.c.pkcolname],
-            sql.and_(
+        query = sql.select(sysfkeys.c.fkname, sysfkeys.c.fktabschema,
+                            sysfkeys.c.fktabname, sysfkeys.c.fkcolname,
+                            sysfkeys.c.pkname, sysfkeys.c.pktabschema,
+                            sysfkeys.c.pktabname, sysfkeys.c.pkcolname).\
+            where(and_(
               sysfkeys.c.pktabschema == current_schema,
               sysfkeys.c.pktabname == table_name
-            ),
-            order_by=[sysfkeys.c.colno]
-          )
+            )).\
+            order_by(sysfkeys.c.colno)
 
         fschema = {}
         for r in connection.execute(query):
             if not fschema.has_key(r[0]):
                 constrained_schema = self.normalize_name(r[1])
 
                 # if no schema specified and referred schema here is the
@@ -429,18 +427,18 @@
         return [value for key, value in fschema.items()]
 
     @reflection.cache
     def get_indexes(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         sysidx = self.sys_indexes
-        query = sql.select([sysidx.c.indname, sysidx.c.colnames,
-                            sysidx.c.uniquerule, sysidx.c.system_required],
-                           sql.and_(sysidx.c.tabschema == current_schema,sysidx.c.tabname == table_name),
-                           order_by=[sysidx.c.tabname])
+        query = sql.select(sysidx.c.indname, sysidx.c.colnames,
+                            sysidx.c.uniquerule, sysidx.c.system_required).\
+            where(and_(sysidx.c.tabschema == current_schema,sysidx.c.tabname == table_name)).\
+            order_by(sysidx.c.tabname)
         indexes = []
         col_finder = re.compile("(\w+)")
         for r in connection.execute(query):
             if r[2] != 'P':
                 if r[2] == 'U' and r[3] != 0:
                     continue
                 if 'sqlnotapplicable' in r[1].lower():
@@ -455,23 +453,21 @@
 
     @reflection.cache
     def get_unique_constraints(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         syskeycol = self.sys_keycoluse
         sysconst = self.sys_tabconst
-        query = sql.select([syskeycol.c.constname, syskeycol.c.colname],
-            sql.and_(
+        query = sql.select(syskeycol.c.constname, syskeycol.c.colname).\
+            where(and_(
               syskeycol.c.constname == sysconst.c.constname,
               sysconst.c.tabname == table_name,
               sysconst.c.tabschema == current_schema,
-              sysconst.c.type == 'U'
-            ),
-            order_by=[syskeycol.c.constname]
-          )
+              sysconst.c.type == 'U')).\
+            order_by(syskeycol.c.constname)
         uniqueConsts = []
         currConst = None
         for r in connection.execute(query):
             if currConst == r[0]:
                 uniqueConsts[-1]['column_names'].append(self.normalize_name(r[1]))
             else:
                 currConst = r[0]
@@ -575,105 +571,100 @@
         table_name = self.denormalize_name(table_name)
         if current_schema:
                 whereclause = sql.and_(
                             self.sys_tables.c.tabschema == current_schema,
                             self.sys_tables.c.tabname == table_name)
         else:
                 whereclause = self.sys_tables.c.tabname == table_name
-        s = sql.select([self.sys_tables], whereclause)
+        s = sql.select(self.sys_tables).where(whereclause)
         c = connection.execute(s)
         return c.first() is not None
 
     def has_sequence(self, connection, sequence_name, schema=None):
         current_schema = self.denormalize_name(
                                 schema or self.default_schema_name)
         sequence_name = self.denormalize_name(sequence_name)
         if current_schema:
                 whereclause = sql.and_(
                             self.sys_sequences.c.seqschema == current_schema,
                             self.sys_sequences.c.seqname == sequence_name)
         else:
                 whereclause = self.sys_sequences.c.seqname == sequence_name
-        s = sql.select([self.sys_sequences.c.seqname], whereclause)
+        s = sql.select(self.sys_sequences.c.seqname).where(whereclause)
         c = connection.execute(s)
         return c.first() is not None
 
     def get_table_comment(self, connection, table_name, schema=None, **kw):
         raise NotImplementedError()
 
     @reflection.cache
     def get_sequence_names(self, connection, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         sys_sequence = self.sys_sequences
-        query = sql.select([sys_sequence.c.seqname],
-                           sys_sequence.c.seqschema == current_schema,
-                           order_by=[sys_sequence.c.seqschema, sys_sequence.c.seqname])
+        query = sql.select(sys_sequence.c.seqname).\
+            where(sys_sequence.c.seqschema == current_schema).\
+            order_by(sys_sequence.c.seqschema, sys_sequence.c.seqname)
         return [self.normalize_name(r[0]) for r in connection.execute(query)]
 
     @reflection.cache
     def get_schema_names(self, connection, **kw):
         sysschema = self.sys_schemas
-        query = sql.select([sysschema.c.schemaname]).\
-                where(~sysschema.c.schemaname.like(unicode('Q%'))).\
-                where(~sysschema.c.schemaname.like(unicode('SYS%'))).\
-                order_by(sysschema.c.schemaname)
+        query = sql.select(sysschema.c.schemaname).\
+            where(~sysschema.c.schemaname.like(unicode('Q%'))).\
+            where(~sysschema.c.schemaname.like(unicode('SYS%'))).\
+            order_by(sysschema.c.schemaname)
         return [self.normalize_name(r[0]) for r in connection.execute(query)]
 
     # Retrieves a list of table names for a given schema
     @reflection.cache
     def get_table_names(self, connection, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         systbl = self.sys_tables
-        query = sql.select([systbl.c.tabname]).\
-                where(systbl.c.tabtype == unicode('T')).\
-                where(systbl.c.tabschema == current_schema).\
-                order_by(systbl.c.tabname)
+        query = not sql.select(systbl.c.tabname).\
+            where(systbl.c.tabtype == unicode('T')).\
+            where(systbl.c.tabschema == current_schema).\
+            order_by(systbl.c.tabname)
         return [self.normalize_name(r[0]) for r in connection.execute(query)]
 
     @reflection.cache
     def get_view_names(self, connection, schema=None, **kw):
         current_schema = self.denormalize_name(
                                 schema or self.default_schema_name)
 
-        query = sql.select([self.sys_views.c.viewname],
-                self.sys_views.c.viewschema == current_schema,
-                order_by=[self.sys_views.c.viewname]
-            )
+        query = sql.select(self.sys_views.c.viewname).\
+            where(self.sys_views.c.viewschema == current_schema).\
+            order_by(self.sys_views.c.viewname)
         return [self.normalize_name(r[0]) for r in connection.execute(query)]
 
     @reflection.cache
     def get_view_definition(self, connection, viewname, schema=None, **kw):
         current_schema = self.denormalize_name(
                                 schema or self.default_schema_name)
         viewname = self.denormalize_name(viewname)
 
-        query = sql.select([self.sys_views.c.text],
-                self.sys_views.c.viewschema == current_schema,
-                self.sys_views.c.viewname == viewname
-            )
+        query = sql.select(self.sys_views.c.text).\
+            where(self.sys_views.c.viewschema == current_schema).\
+            where(self.sys_views.c.viewname == viewname)
         return connection.execute(query).scalar()
 
     @reflection.cache
     def get_columns(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         syscols = self.sys_columns
 
-        query = sql.select([syscols.c.colname,
-                                syscols.c.typename,
-                                syscols.c.defaultval, syscols.c.nullable,
-                                syscols.c.length, syscols.c.scale,
-                                syscols.c.isid, syscols.c.idgenerate, 
-                                syscols.c.remark],
-                    sql.and_(
-                            syscols.c.tabschema == current_schema,
-                            syscols.c.tabname == table_name
-                        ),
-                    order_by=[syscols.c.colno]
-                )
+        query = sql.select(syscols.c.colname,syscols.c.typename,
+                           syscols.c.defaultval, syscols.c.nullable,
+                           syscols.c.length, syscols.c.scale,
+                           syscols.c.isid, syscols.c.idgenerate,
+                           syscols.c.remark).\
+            where(and_(
+                syscols.c.tabschema == current_schema,
+                syscols.c.tabname == table_name)).\
+            order_by(syscols.c.colno)
         sa_columns = []
         for r in connection.execute(query):
             coltype = r[1].upper()
             if coltype in ['DECIMAL', 'NUMERIC']:
                 coltype = self.ischema_names.get(coltype)(int(r[4]), int(r[5]))
             elif coltype in ['CHARACTER', 'CHAR', 'VARCHAR',
                                 'GRAPHIC', 'VARGRAPHIC']:
@@ -700,22 +691,22 @@
     def get_pk_constraint(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(
             schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         sysconst = self.sys_table_constraints
         syskeyconst = self.sys_key_constraints
 
-        query = sql.select([syskeyconst.c.colname, sysconst.c.tabname, sysconst.c.conname],
-                           sql.and_(
-                               syskeyconst.c.conschema == sysconst.c.conschema,
-                               syskeyconst.c.conname == sysconst.c.conname,
-                               sysconst.c.tabschema == current_schema,
-                               sysconst.c.tabname == table_name,
-                               sysconst.c.contype == 'PRIMARY KEY'
-                           ), order_by=[syskeyconst.c.colno])
+        query = sql.select(syskeyconst.c.colname, sysconst.c.tabname, sysconst.c.conname).\
+            where(and_(
+                syskeyconst.c.conschema == sysconst.c.conschema,
+                syskeyconst.c.conname == sysconst.c.conname,
+                sysconst.c.tabschema == current_schema,
+                sysconst.c.tabname == table_name,
+                sysconst.c.contype == 'PRIMARY KEY')).\
+            order_by(syskeyconst.c.colno)
 
         pk_columns = []
         pk_name = None
         for key in connection.execute(query):
             pk_columns.append(self.normalize_name(key[0]))
             if not pk_name:
                 pk_name = self.normalize_name(key[2])
@@ -725,43 +716,41 @@
     def get_primary_keys(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(
                                     schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         sysconst = self.sys_table_constraints
         syskeyconst = self.sys_key_constraints
 
-        query = sql.select([syskeyconst.c.colname, sysconst.c.tabname],
-                sql.and_(
-                    syskeyconst.c.conschema == sysconst.c.conschema,
-                    syskeyconst.c.conname == sysconst.c.conname,
-                    sysconst.c.tabschema == current_schema,
-                    sysconst.c.tabname == table_name,
-                    sysconst.c.contype == unicode('PRIMARY KEY')
-            ), order_by=[syskeyconst.c.colno])
+        query = sql.select(syskeyconst.c.colname, sysconst.c.tabname).\
+            where(and_(
+                syskeyconst.c.conschema == sysconst.c.conschema,
+                syskeyconst.c.conname == sysconst.c.conname,
+                sysconst.c.tabschema == current_schema,
+                sysconst.c.tabname == table_name,
+                sysconst.c.contype == unicode('PRIMARY KEY'))).\
+            order_by(syskeyconst.c.colno)
 
         return [self.normalize_name(key[0])
                     for key in connection.execute(query)]
 
     @reflection.cache
     def get_foreign_keys(self, connection, table_name, schema=None, **kw):
         default_schema = self.default_schema_name
         current_schema = self.denormalize_name(schema or default_schema)
         default_schema = self.normalize_name(default_schema)
         table_name = self.denormalize_name(table_name)
         sysfkeys = self.sys_foreignkeys
-        query = sql.select([sysfkeys.c.fkname, sysfkeys.c.fktabschema, \
-                                sysfkeys.c.fktabname, sysfkeys.c.fkcolname, \
-                                sysfkeys.c.pkname, sysfkeys.c.pktabschema, \
-                                sysfkeys.c.pktabname, sysfkeys.c.pkcolname],
-                sql.and_(
-                    sysfkeys.c.fktabschema == current_schema,
-                    sysfkeys.c.fktabname == table_name
-                ),
-                order_by=[sysfkeys.c.colno]
-            )
+        query = sql.select(sysfkeys.c.fkname, sysfkeys.c.fktabschema,
+                           sysfkeys.c.fktabname, sysfkeys.c.fkcolname,
+                           sysfkeys.c.pkname, sysfkeys.c.pktabschema,
+                           sysfkeys.c.pktabname, sysfkeys.c.pkcolname).\
+            where(and_(
+                sysfkeys.c.fktabschema == current_schema,
+                sysfkeys.c.fktabname == table_name)).\
+            order_by(sysfkeys.c.colno)
         fschema = {}
         for r in connection.execute(query):
             if r[0] not in fschema:
                 referred_schema = self.normalize_name(r[5])
 
                 # if no schema specified and referred schema here is the
                 # default, then set to None
@@ -785,22 +774,22 @@
         current_schema = self.denormalize_name(
                                     schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         
         sysidx = self.sys_indexes
         syskey = self.sys_keys
 
-        query = sql.select([sysidx.c.indname,
-                            sysidx.c.uniquerule, syskey.c.colname], sql.and_(
-                    syskey.c.indschema == sysidx.c.indschema,
-                    syskey.c.indname == sysidx.c.indname,
-                    sysidx.c.tabschema == current_schema,
-                    sysidx.c.tabname == table_name
-                ), order_by=[syskey.c.indname, syskey.c.colno]
-            )
+        query = sql.select(sysidx.c.indname,sysidx.c.uniquerule,
+                           syskey.c.colname).\
+            where(and_(
+                syskey.c.indschema == sysidx.c.indschema,
+                syskey.c.indname == sysidx.c.indname,
+                sysidx.c.tabschema == current_schema,
+                sysidx.c.tabname == table_name)).\
+            order_by(syskey.c.indname, syskey.c.colno)
         indexes = {}
         for r in connection.execute(query):
             key = r[0].upper()
             if key in indexes:
                 indexes[key]['column_names'].append(self.normalize_name(r[2]))
             else:
                 indexes[key] = {
@@ -905,97 +894,95 @@
                             schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         if current_schema:
             whereclause = sql.and_(self.sys_tables.c.tabschema == current_schema,
                                    self.sys_tables.c.tabname == table_name)
         else:
             whereclause = self.sys_tables.c.tabname == table_name
-        s = sql.select([self.sys_tables.c.tabname], whereclause)
+        s = sql.select(self.sys_tables.c.tabname).where(whereclause)
         c = connection.execute(s)
         return c.first() is not None
 
     def has_sequence(self, connection, sequence_name, schema=None):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         sequence_name = self.denormalize_name(sequence_name)
         if current_schema:
             whereclause = sql.and_(self.sys_sequences.c.seqschema == current_schema,
                                    self.sys_sequences.c.seqname == sequence_name)
         else:
             whereclause = self.sys_sequences.c.seqname == sequence_name
-        s = sql.select([self.sys_sequences.c.seqname], whereclause)
+        s = sql.select(self.sys_sequences.c.seqname).where(whereclause)
         c = connection.execute(s)
         return c.first() is not None
 
     @reflection.cache
     def get_sequence_names(self, connection, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         sys_sequence = self.sys_sequences
-        query = sql.select([sys_sequence.c.seqname],
-                           sys_sequence.c.seqschema == current_schema,
-                           order_by=[sys_sequence.c.seqschema, sys_sequence.c.seqname])
+        query = sql.select(sys_sequence.c.seqname).\
+            where(sys_sequence.c.seqschema == current_schema).\
+            order_by(sys_sequence.c.seqschema, sys_sequence.c.seqname)
         return [self.normalize_name(r[0]) for r in connection.execute(query)]
 
     @reflection.cache
     def get_schema_names(self, connection, **kw):
         sysschema = self.sys_tables
-        query = sql.select([sysschema.c.tabschema],
-                           sql.not_(sysschema.c.tabschema.like('SYS%')),
-                           distinct=[sysschema.c.tabschema])
+        query = sql.select(sysschema.c.tabschema).\
+            where(not_(sysschema.c.tabschema.like('SYS%'))).\
+            distinct(sysschema.c.tabschema)
         return [self.normalize_name(r[0]) for r in connection.execute(query)]
 
     def get_table_comment(self, connection, table_name, schema=None, **kw):
         raise NotImplementedError()
 
     @reflection.cache
     def get_table_names(self, connection, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         systbl = self.sys_tables
-        query = sql.select([systbl.c.tabname]).\
-                    where(systbl.c.type == 'T').\
-                    where(systbl.c.tabschema == current_schema).\
-                    order_by(systbl.c.tabname)
+        query = sql.select(systbl.c.tabname).\
+            where(systbl.c.type == 'T').\
+            where(systbl.c.tabschema == current_schema).\
+            order_by(systbl.c.tabname)
         return [self.normalize_name(r[0]) for r in connection.execute(query)]
 
     @reflection.cache
     def get_view_names(self, connection, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
 
-        query = sql.select([self.sys_views.c.viewname]).\
+        query = sql.select(self.sys_views.c.viewname).\
             where(self.sys_views.c.viewschema == current_schema).\
             order_by(self.sys_views.c.viewname)
 
         return [self.normalize_name(r[0]) for r in connection.execute(query)]
 
     @reflection.cache
     def get_view_definition(self, connection, viewname, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         viewname = self.denormalize_name(viewname)
 
-        query = sql.select([self.sys_views.c.text]).\
+        query = sql.select(self.sys_views.c.text).\
             where(self.sys_views.c.viewschema == current_schema).\
             where(self.sys_views.c.viewname == viewname)
 
         return connection.execute(query).scalar()
 
     @reflection.cache
     def get_columns(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         syscols = self.sys_columns
 
-        query = sql.select([syscols.c.colname, syscols.c.typename,
-                            syscols.c.defaultval, syscols.c.nullable,
-                            syscols.c.length, syscols.c.scale,
-                            syscols.c.generated, syscols.c.remark],
-              sql.and_(
-                  syscols.c.tabschema == current_schema,
-                  syscols.c.tabname == table_name
-                ),
-              order_by=[syscols.c.colno]
-            )
+        query = sql.select(syscols.c.colname, syscols.c.typename,
+                           syscols.c.defaultval, syscols.c.nullable,
+                           syscols.c.length, syscols.c.scale,
+                           syscols.c.generated, syscols.c.remark).\
+            where(and_(
+                syscols.c.tabschema == current_schema,
+                syscols.c.tabname == table_name)).\
+            order_by(syscols.c.colno)
         sa_columns = []
         for r in connection.execute(query):
             coltype = r[1].upper()
             if coltype in ['DECIMAL', 'NUMERIC']:
                 coltype = self.ischema_names.get(coltype)(int(r[4]), int(r[5]))
             elif coltype in ['CHARACTER', 'CHAR', 'VARCHAR',
                             'GRAPHIC', 'VARGRAPHIC']:
@@ -1020,40 +1007,38 @@
 
     @reflection.cache
     def get_pk_constraint(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         sysindexes = self.sys_columns
         col_finder = re.compile("(\w+)")
-        query = sql.select([sysindexes.c.colname],
-                           sql.and_(
-                               sysindexes.c.tabschema == current_schema,
-                               sysindexes.c.tabname == table_name,
-                               sysindexes.c.keyseq > 0),
-                           order_by=[sysindexes.c.tabschema, sysindexes.c.tabname])
+        query = sql.select(sysindexes.c.colname).\
+            where(and_(
+                sysindexes.c.tabschema == current_schema,
+                sysindexes.c.tabname == table_name,
+                sysindexes.c.keyseq > 0)).\
+            order_by(sysindexes.c.tabschema, sysindexes.c.tabname)
         pk_columns = []
         for r in connection.execute(query):
             cols = col_finder.findall(r[0])
             pk_columns.extend(cols)
         return {"constrained_columns": [self.normalize_name(col) for col in pk_columns], "name": None}
 
     @reflection.cache
     def get_primary_keys(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         sysindexes = self.sys_columns
         col_finder = re.compile("(\w+)")
-        query = sql.select([sysindexes.c.colname],
-              sql.and_(
-                  sysindexes.c.tabschema == current_schema,
-                  sysindexes.c.tabname == table_name,
-                  sysindexes.c.keyseq > 0
-                ),
-              order_by=[sysindexes.c.tabschema, sysindexes.c.tabname]
-            )
+        query = sql.select(sysindexes.c.colname).\
+            where(and_(
+                sysindexes.c.tabschema == current_schema,
+                sysindexes.c.tabname == table_name,
+                sysindexes.c.keyseq > 0)).\
+            order_by(sysindexes.c.tabschema, sysindexes.c.tabname)
         pk_columns = []
         for r in connection.execute(query):
             cols = col_finder.findall(r[0])
             pk_columns.extend(cols)
         return [self.normalize_name(col) for col in pk_columns]
 
     @reflection.cache
@@ -1062,28 +1047,25 @@
         current_schema = self.denormalize_name(schema or default_schema)
         default_schema = self.normalize_name(default_schema)
         table_name = self.denormalize_name(table_name)
         sysfkeys = self.sys_foreignkeys
         sysrels = self.sys_rels
         syscolspk = self.sys_columns
         sysindex = self.sys_indexes
-        query = sql.select([sysrels.c.fkname, sysrels.c.fktabschema, \
-                            sysrels.c.fktabname, sysfkeys.c.fkcolname, \
-                            sysindex.c.indname, sysrels.c.pktabschema, \
-                            sysrels.c.pktabname, syscolspk.c.colname],
-            sql.and_(
-              sysrels.c.fktabschema == current_schema,
-              sysrels.c.fktabname == table_name,
-              sysrels.c.fktabname == sysfkeys.c.fktabname,
-              sysrels.c.pktabname == syscolspk.c.tabname,
-              syscolspk.c.tabname == sysindex.c.tabname,
-              syscolspk.c.keyseq > 0
-            ),
-            order_by=[sysfkeys.c.colno]
-          )
+        query = sql.select(sysrels.c.fkname, sysrels.c.fktabschema,
+                           sysrels.c.fktabname, sysfkeys.c.fkcolname,
+                           sysindex.c.indname, sysrels.c.pktabschema,
+                           sysrels.c.pktabname, syscolspk.c.colname).\
+            where(and_(
+                sysrels.c.fktabschema == current_schema,
+                sysrels.c.fktabname == table_name,
+                sysrels.c.fktabname == sysfkeys.c.fktabname,
+                sysrels.c.pktabname == syscolspk.c.tabname,
+                syscolspk.c.tabname == sysindex.c.tabname,syscolspk.c.keyseq > 0)).\
+            order_by(sysfkeys.c.colno)
 
         fschema = {}
         for r in connection.execute(query):
             if not (r[0]) in fschema:
                 referred_schema = self.normalize_name(r[5])
 
                 # if no schema specified and referred schema here is the
@@ -1109,28 +1091,26 @@
         current_schema = self.denormalize_name(schema or default_schema)
         default_schema = self.normalize_name(default_schema)
         table_name = self.denormalize_name(table_name)
         sysfkeys = self.sys_foreignkeys
         sysrels = self.sys_rels
         syscolspk = self.sys_columns
         sysindex = self.sys_indexes
-        query = sql.select([sysrels.c.fkname, sysrels.c.fktabschema, \
-                            sysrels.c.fktabname, sysfkeys.c.fkcolname, \
-                            sysindex.c.indname, sysrels.c.pktabschema, \
-                            sysrels.c.pktabname, syscolspk.c.colname],
-            sql.and_(
-              syscolspk.c.tabschema == current_schema,
-              syscolspk.c.tabname == table_name,
-              sysrels.c.fktabname == sysfkeys.c.fktabname,
-              sysrels.c.pktabname == syscolspk.c.tabname,
-              syscolspk.c.tabname == sysindex.c.tabname,
-              syscolspk.c.keyseq > 0
-            ),
-            order_by=[sysfkeys.c.colno]
-          )
+        query = sql.select(sysrels.c.fkname, sysrels.c.fktabschema,
+                           sysrels.c.fktabname, sysfkeys.c.fkcolname,
+                           sysindex.c.indname, sysrels.c.pktabschema,
+                           sysrels.c.pktabname, syscolspk.c.colname).\
+            where(and_(
+                syscolspk.c.tabschema == current_schema,
+                syscolspk.c.tabname == table_name,
+                sysrels.c.fktabname == sysfkeys.c.fktabname,
+                sysrels.c.pktabname == syscolspk.c.tabname,
+                syscolspk.c.tabname == sysindex.c.tabname,
+                syscolspk.c.keyseq > 0)).\
+            order_by(sysfkeys.c.colno)
 
         fschema = {}
         for r in connection.execute(query):
             if not fschema.has_key(r[0]):
                 constrained_schema = self.normalize_name(r[1])
 
                 # if no schema specified and referred schema here is the
@@ -1154,23 +1134,21 @@
 
     @reflection.cache
     def get_indexes(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         sysidx = self.sys_indexes
         syscolpk = self.sys_columns
-        query = sql.select([sysidx.c.indname, syscolpk.c.colname, sysidx.c.uniquerule, sysidx.c.system_required],
-            sql.and_(
-              sysidx.c.tabschema == current_schema,
-              sysidx.c.tabname == table_name,
-              syscolpk.c.colname == sysidx.c.tabname,
-              syscolpk.c.keyseq > 0
-            ),
-            order_by=[sysidx.c.tabname]
-          )
+        query = sql.select(sysidx.c.indname, syscolpk.c.colname, sysidx.c.uniquerule, sysidx.c.system_required).\
+            where(and_(
+                sysidx.c.tabschema == current_schema,
+                sysidx.c.tabname == table_name,
+                syscolpk.c.colname == sysidx.c.tabname,
+                syscolpk.c.keyseq > 0)).\
+            order_by(sysidx.c.tabname)
         indexes = []
         col_finder = re.compile("(\w+)")
         for r in connection.execute(query):
             if r[2] != 'P':
                 if r[2] == 'U' and r[3] != 0:
                     continue
                 indexes.append({
@@ -1183,23 +1161,21 @@
 
     @reflection.cache
     def get_unique_constraints(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         syskeycol = self.sys_keycoluse
         sysconst = self.sys_tabconst
-        query = sql.select([syskeycol.c.constname, syskeycol.c.colname],
-            sql.and_(
-              syskeycol.c.constname == sysconst.c.constname,
-              sysconst.c.tabname == table_name,
-              sysconst.c.tabschema == current_schema,
-              sysconst.c.type == 'U'
-            ),
-            order_by=[syskeycol.c.constname]
-          )
+        query = sql.select(syskeycol.c.constname, syskeycol.c.colname).\
+            where(and_(
+                syskeycol.c.constname == sysconst.c.constname,
+                sysconst.c.tabname == table_name,
+                sysconst.c.tabschema == current_schema,
+                sysconst.c.type == 'U')).\
+            order_by(syskeycol.c.constname)
         uniqueConsts = []
         currConst = None
         for r in connection.execute(query):
             if currConst == r[0]:
                 uniqueConsts[-1]['column_names'].append(self.normalize_name(r[1]))
             else:
                 currConst = r[0]
```

### Comparing `ibm_db_sa-0.3.9/ibm_db_sa/requirements.py` & `ibm_db_sa-0.4.0/ibm_db_sa/requirements.py`

 * *Files identical despite different names*

### Comparing `ibm_db_sa-0.3.9/ibm_db_sa/zxjdbc.py` & `ibm_db_sa-0.4.0/ibm_db_sa/zxjdbc.py`

 * *Files identical despite different names*

### Comparing `ibm_db_sa-0.3.9/ibm_db_sa.egg-info/PKG-INFO` & `ibm_db_sa-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ibm-db-sa
-Version: 0.3.9
+Name: ibm_db_sa
+Version: 0.4.0
 Summary: SQLAlchemy support for IBM Data Servers
 Home-page: http://pypi.python.org/pypi/ibm_db_sa/
 Download-URL: http://code.google.com/p/ibm-db/downloads/list
 Author: IBM Application Development Team
 Author-email: opendev@us.ibm.com
 License: Apache License 2.0
 Keywords: sqlalchemy database interface IBM Data Servers DB2 Informix IDS
@@ -20,20 +20,20 @@
 IBM_DB_SA
 =========
 
 The IBM_DB_SA adapter provides the Python/SQLAlchemy interface to IBM Data Servers.
 
 Version
 --------
-0.3.9 (2023/02/27)
+0.4.0 (2023/04/20)
 
 Prerequisites
 --------------
 1. Install Python 2.7 or newer versions except python 3.3 or Jython 2.5.x .
-2. SQLAlchemy version between 0.7.3 - 1.4.x.
+2. SQLAlchemy version between 0.7.3 - 2.0.x.
 3. IBM_DB driver and IBM_DB_DBI wrapper 1.0.1 or higher.
 ```
    Install ibm_db driver with below commands:
 	    Linux and Windows: 
 	   	   pip install ibm_db
 	    Mac:
 		   pip install --no-cache-dir ibm_db
@@ -101,14 +101,32 @@
 Supported Databases
 -------------------
 - IBM DB2 Universal Database for Linux/Unix/Windows versions 9.7 onwards 
 - IBM Db2 on Cloud
 - IBM Db2 on ZOS
 - IBM Db2 on Iseries
 
+Note
+-------------------------------------------------------------
+By default, all tables and schemas stored in a Db2 database are created
+using capital letters only.
+However, if you have a table name in lowercase letters, you can still reference
+it by enclosing the name in single quotes inside double quotes.
+For example
+```
+	if users table is in small letter inside database
+	So, you can use single quotes "'users'".
+	If you will not use single quotes such as "users", it will
+	be refered as "USERS".
+
+	metadata = sqlalchemy.MetaData(schema="schema1")
+	table = sqlalchemy.Table("'users'", metadata, autoload_with=engine)
+
+```
+
 Known Limitations in ibm_db_sa adapter for DB2 databases
 -------------------------------------------------------------
 1) Non-standard SQL queries are not supported. e.g. "SELECT ? FROM TAB1"
 2) For updations involving primary/foreign key references, the entries should be made in correct order. Integrity check is always on and thus the primary keys referenced by the foreign keys in the referencing tables should always exist in the parent table.
 3) Unique key which contains nullable column not supported
 4) UPDATE CASCADE for foreign keys not supported
 5) DEFERRABLE INITIALLY deferred not supported
```

### Comparing `ibm_db_sa-0.3.9/ibm_db_sa.egg-info/SOURCES.txt` & `ibm_db_sa-0.4.0/ibm_db_sa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm_db_sa-0.3.9/ibm_db_sa.egg-info/entry_points.txt` & `ibm_db_sa-0.4.0/ibm_db_sa.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ibm_db_sa-0.3.9/run_tests.py` & `ibm_db_sa-0.4.0/run_tests.py`

 * *Files identical despite different names*

### Comparing `ibm_db_sa-0.3.9/setup.py` & `ibm_db_sa-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `ibm_db_sa-0.3.9/test/test_out_parameters.py` & `ibm_db_sa-0.4.0/test/test_out_parameters.py`

 * *Files identical despite different names*

