# Comparing `tmp/thanosql-magic-0.3.6.tar.gz` & `tmp/thanosql-magic-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thanosql-magic-0.3.6.tar", last modified: Fri Mar 31 07:02:38 2023, max compression
+gzip compressed data, was "thanosql-magic-0.3.7.tar", last modified: Thu Apr 20 06:33:35 2023, max compression
```

## Comparing `thanosql-magic-0.3.6.tar` & `thanosql-magic-0.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:02:38.129135 thanosql-magic-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-31 07:02:24.000000 thanosql-magic-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-31 07:02:38.129135 thanosql-magic-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-31 07:02:24.000000 thanosql-magic-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 07:02:38.129135 thanosql-magic-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-31 07:02:24.000000 thanosql-magic-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:02:38.129135 thanosql-magic-0.3.6/thanosql/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-31 07:02:24.000000 thanosql-magic-0.3.6/thanosql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-31 07:02:24.000000 thanosql-magic-0.3.6/thanosql/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-03-31 07:02:24.000000 thanosql-magic-0.3.6/thanosql/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-31 07:02:24.000000 thanosql-magic-0.3.6/thanosql/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-03-31 07:02:24.000000 thanosql-magic-0.3.6/thanosql/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:02:38.129135 thanosql-magic-0.3.6/thanosql_magic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-31 07:02:38.000000 thanosql-magic-0.3.6/thanosql_magic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-31 07:02:38.000000 thanosql-magic-0.3.6/thanosql_magic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 07:02:38.000000 thanosql-magic-0.3.6/thanosql_magic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 07:02:37.000000 thanosql-magic-0.3.6/thanosql_magic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-31 07:02:38.000000 thanosql-magic-0.3.6/thanosql_magic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 07:02:38.000000 thanosql-magic-0.3.6/thanosql_magic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:33:35.361626 thanosql-magic-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-20 06:33:21.000000 thanosql-magic-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-20 06:33:35.361626 thanosql-magic-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-20 06:33:21.000000 thanosql-magic-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 06:33:35.361626 thanosql-magic-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-20 06:33:21.000000 thanosql-magic-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:33:35.361626 thanosql-magic-0.3.7/thanosql/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 06:33:21.000000 thanosql-magic-0.3.7/thanosql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-20 06:33:21.000000 thanosql-magic-0.3.7/thanosql/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-20 06:33:21.000000 thanosql-magic-0.3.7/thanosql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-20 06:33:21.000000 thanosql-magic-0.3.7/thanosql/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-20 06:33:21.000000 thanosql-magic-0.3.7/thanosql/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:33:35.361626 thanosql-magic-0.3.7/thanosql_magic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-20 06:33:35.000000 thanosql-magic-0.3.7/thanosql_magic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-20 06:33:35.000000 thanosql-magic-0.3.7/thanosql_magic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:33:35.000000 thanosql-magic-0.3.7/thanosql_magic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:33:35.000000 thanosql-magic-0.3.7/thanosql_magic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 06:33:35.000000 thanosql-magic-0.3.7/thanosql_magic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 06:33:35.000000 thanosql-magic-0.3.7/thanosql_magic.egg-info/top_level.txt
```

### Comparing `thanosql-magic-0.3.6/LICENSE` & `thanosql-magic-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `thanosql-magic-0.3.6/setup.py` & `thanosql-magic-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `thanosql-magic-0.3.6/thanosql/magic.py` & `thanosql-magic-0.3.7/thanosql/magic.py`

 * *Files identical despite different names*

### Comparing `thanosql-magic-0.3.6/thanosql/parse.py` & `thanosql-magic-0.3.7/thanosql/parse.py`

 * *Files identical despite different names*

### Comparing `thanosql-magic-0.3.6/thanosql/util.py` & `thanosql-magic-0.3.7/thanosql/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 def format_result(output_dict: dict):
 
     data = output_dict["data"]
     workspace_db_info = data.get("workspace_db_info")
     response_type = data.get("response_type")
 
-    query_string = text(data.get("query_string"))
-    extra_query_string = text(data.get("extra_query_string"))
+    query_string = data.get("query_string")
+    extra_query_string = data.get("extra_query_string")
 
     user = workspace_db_info.get("user")
     password = workspace_db_info.get("password")
     database = workspace_db_info.get("database")
     host = workspace_db_info.get("host")
 
     connection_string = f"postgresql://{user}:{password}@/{database}?host={host}"
@@ -28,34 +28,34 @@
         raise ThanoSQLConnectionError("Error connecting to workspace database")
 
     with engine.connect() as conn:
         result = None
 
         if response_type == "NORMAL":
             try:
-                result = pd.read_sql_query(query_string, conn)
+                result = pd.read_sql_query(text(query_string), conn)
             except ResourceClosedError:
                 """
                 ResourceClosedError will capture queries
                 like INSERT and DROP that don’t return a value.
                 This is not the best solution as we are presumptuously assuming
                 that the connection with the database will always be secure and succeed.
                 If a failure happens in the database,
                 ResourceClosedError will be raised
                 and “Success” will be printed out, which is a problem.
                 Therefore, this is subject to change in the future.
                 """
                 print("Success")
 
         elif response_type == "SELECT":
-            result = pd.read_sql_query(query_string, conn)
+            result = pd.read_sql_query(text(query_string), conn)
 
         elif response_type == "SELECT_DROP":
-            result = pd.read_sql_query(query_string, conn)
-            conn.execute(extra_query_string)
+            result = pd.read_sql_query(text(query_string), conn)
+            conn.execute(text(extra_query_string))
 
         elif response_type is None:
             print("Success")
 
     # close sqlalchemy(DB) engine
     engine.dispose()
```

