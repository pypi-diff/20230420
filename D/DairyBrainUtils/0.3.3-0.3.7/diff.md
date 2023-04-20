# Comparing `tmp/DairyBrainUtils-0.3.3.tar.gz` & `tmp/DairyBrainUtils-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DairyBrainUtils-0.3.3.tar", last modified: Mon Nov  8 22:05:39 2021, max compression
+gzip compressed data, was "DairyBrainUtils-0.3.7.tar", last modified: Thu Apr 20 17:48:58 2023, max compression
```

## Comparing `DairyBrainUtils-0.3.3.tar` & `DairyBrainUtils-0.3.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 stevewangen   (502) staff       (20)        0 2021-11-08 22:05:39.320981 DairyBrainUtils-0.3.3/
-drwxr-xr-x   0 stevewangen   (502) staff       (20)        0 2021-11-08 22:05:39.318710 DairyBrainUtils-0.3.3/DairyBrainUtils/
--rw-r--r--   0 stevewangen   (502) staff       (20)     8852 2021-11-08 22:03:38.000000 DairyBrainUtils-0.3.3/DairyBrainUtils/__init__.py
-drwxr-xr-x   0 stevewangen   (502) staff       (20)        0 2021-11-08 22:05:39.320371 DairyBrainUtils-0.3.3/DairyBrainUtils.egg-info/
--rw-r--r--   0 stevewangen   (502) staff       (20)     5814 2021-11-08 22:05:39.000000 DairyBrainUtils-0.3.3/DairyBrainUtils.egg-info/PKG-INFO
--rw-r--r--   0 stevewangen   (502) staff       (20)      210 2021-11-08 22:05:39.000000 DairyBrainUtils-0.3.3/DairyBrainUtils.egg-info/SOURCES.txt
--rw-r--r--   0 stevewangen   (502) staff       (20)        1 2021-11-08 22:05:39.000000 DairyBrainUtils-0.3.3/DairyBrainUtils.egg-info/dependency_links.txt
--rw-r--r--   0 stevewangen   (502) staff       (20)       16 2021-11-08 22:05:39.000000 DairyBrainUtils-0.3.3/DairyBrainUtils.egg-info/top_level.txt
--rw-r--r--   0 stevewangen   (502) staff       (20)     1095 2021-11-08 21:51:07.000000 DairyBrainUtils-0.3.3/LICENSE
--rw-r--r--   0 stevewangen   (502) staff       (20)     5814 2021-11-08 22:05:39.320700 DairyBrainUtils-0.3.3/PKG-INFO
--rw-r--r--   0 stevewangen   (502) staff       (20)     5219 2021-11-08 22:04:31.000000 DairyBrainUtils-0.3.3/README.md
--rw-r--r--   0 stevewangen   (502) staff       (20)       38 2021-11-08 22:05:39.321094 DairyBrainUtils-0.3.3/setup.cfg
--rw-r--r--   0 stevewangen   (502) staff       (20)      774 2021-11-08 22:02:14.000000 DairyBrainUtils-0.3.3/setup.py
+drwxr-xr-x   0 stevenwangen   (501) staff       (20)        0 2023-04-20 17:48:58.892456 DairyBrainUtils-0.3.7/
+drwxr-xr-x   0 stevenwangen   (501) staff       (20)        0 2023-04-20 17:48:58.889407 DairyBrainUtils-0.3.7/DairyBrainUtils/
+-rw-r--r--   0 stevenwangen   (501) staff       (20)     8689 2023-04-20 17:46:20.000000 DairyBrainUtils-0.3.7/DairyBrainUtils/__init__.py
+drwxr-xr-x   0 stevenwangen   (501) staff       (20)        0 2023-04-20 17:48:58.891694 DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/
+-rw-r--r--   0 stevenwangen   (501) staff       (20)     5793 2023-04-20 17:48:58.000000 DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/PKG-INFO
+-rw-r--r--   0 stevenwangen   (501) staff       (20)      248 2023-04-20 17:48:58.000000 DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 stevenwangen   (501) staff       (20)        1 2023-04-20 17:48:58.000000 DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 stevenwangen   (501) staff       (20)       28 2023-04-20 17:48:58.000000 DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/requires.txt
+-rw-r--r--   0 stevenwangen   (501) staff       (20)       16 2023-04-20 17:48:58.000000 DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/top_level.txt
+-rw-r--r--   0 stevenwangen   (501) staff       (20)     1095 2023-04-20 17:24:08.000000 DairyBrainUtils-0.3.7/LICENSE
+-rw-r--r--   0 stevenwangen   (501) staff       (20)     5793 2023-04-20 17:48:58.892123 DairyBrainUtils-0.3.7/PKG-INFO
+-rw-r--r--   0 stevenwangen   (501) staff       (20)     5219 2023-04-20 17:24:08.000000 DairyBrainUtils-0.3.7/README.md
+-rw-r--r--   0 stevenwangen   (501) staff       (20)       38 2023-04-20 17:48:58.892563 DairyBrainUtils-0.3.7/setup.cfg
+-rw-r--r--   0 stevenwangen   (501) staff       (20)      873 2023-04-20 17:47:20.000000 DairyBrainUtils-0.3.7/setup.py
```

### Comparing `DairyBrainUtils-0.3.3/DairyBrainUtils/__init__.py` & `DairyBrainUtils-0.3.7/DairyBrainUtils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import sys
-from sqlalchemy import create_engine
+import csv
+from sqlalchemy import create_engine, inspect
 from sqlalchemy.sql import text
-from sqlalchemy_utils.functions import database_exists
 
 logger = logging.getLogger(__name__)
+logger.setLevel('DEBUG')
 
 
 def get_engine(credentials):
     """
     Use sqlalchemy to create an engine instance for future database connection
     :param credentials: Dictionary with the following keys: [dialect, user, password, host, port, db_name, log]
     :return: An engine instance
@@ -30,23 +31,14 @@
         )
     except:
         logger.error("Can't connect to database: " + str(sys.exc_info()))
         sys.exit(1)
     return db_engine
 
 
-def check_if_database_exists(db_engine):
-    """
-    Use existing sqlalchemy functionality to check if the database exists.
-    :param db_engine: Specifies the connection to the database
-    :return: True if database exists, False otherwise
-    """
-    return database_exists(db_engine.url)
-
-
 def create_table_if_doesnt_exist(db_engine, table_name, sql_statement):
     """
     Creates a table with table_name in the database if a table with the given name doesn't exist.
     :param db_engine: Specifies the connection to the database
     :param table_name: Name of the table that needs to be created
     :param sql_statement: SQL statement with the column headers of the table. They are strings that are stored in the
     animal_import and event_import scripts.
@@ -166,16 +158,18 @@
     # adapted to sqlalchemy using https://stackoverflow.com/questions/13125236/sqlalchemy-psycopg2-and-postgresql-copy
     with db_engine.connect() as con:
         # isolate a connection
         connection = db_engine.connect().connection
 
         # get the cursor
         cursor = connection.cursor()
+        #import pdb; pdb.set_trace()
 
         try:
+            cursor.execute('SET search_path TO dairy_comp, public')
             with open(csv_location, 'r') as f:
                 next(f)  # Skip the header row.
                 cursor.copy_from(f, table_name, sep=',', null='')
             connection.commit()
 
         except Exception as e:
             logger.error(
@@ -224,11 +218,12 @@
 def has_table(table_name, db_engine):
     """
     Checks if a table with table_name is in the database
     :param table_name: Name of the table that needs to be checked
     :param db_engine: Specifies the connection to the database
     :return: True if table with table_name is in the database, False otherwise
     """
+    inspector = inspect(db_engine)
     if '.' in table_name:  # received schema.table_name
-        return db_engine.has_table(table_name.split('.')[1], schema=table_name.split('.')[0])
+        return inspector.has_table(table_name.split('.')[1], schema=table_name.split('.')[0])
     else:  # received plain table_name
-        return db_engine.has_table(table_name)
+        return inspector.has_table(table_name)
```

### Comparing `DairyBrainUtils-0.3.3/DairyBrainUtils.egg-info/PKG-INFO` & `DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: DairyBrainUtils
-Version: 0.3.3
+Version: 0.3.7
 Summary: A set of functions that interacts with a database. It contains some basic functionalities along with some other Dairy-Brain-specific functionalities.
 Home-page: https://github.com/DairyBrain/AgDH_DairyBrainUtils
-Author: Rui Pan
-Author-email: rpan33@wisc.edu
-License: UNKNOWN
-Platform: UNKNOWN
+Author: Rui Pan, Steve Wangen
+Author-email: srwangen@wisc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -138,9 +136,7 @@
 For uploading the distribution packages to TestPyPI, do:
 ```
 python3 -m pip install --upgrade twine
 python3 -m twine upload --repository testpypi dist/*
 ```
 
 Use `__token__` when prompted to enter the username. For the password, use the token value, including the `pypi-` prefix.
-
-
```

### Comparing `DairyBrainUtils-0.3.3/LICENSE` & `DairyBrainUtils-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `DairyBrainUtils-0.3.3/PKG-INFO` & `DairyBrainUtils-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: DairyBrainUtils
-Version: 0.3.3
+Version: 0.3.7
 Summary: A set of functions that interacts with a database. It contains some basic functionalities along with some other Dairy-Brain-specific functionalities.
 Home-page: https://github.com/DairyBrain/AgDH_DairyBrainUtils
-Author: Rui Pan
-Author-email: rpan33@wisc.edu
-License: UNKNOWN
-Platform: UNKNOWN
+Author: Rui Pan, Steve Wangen
+Author-email: srwangen@wisc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -138,9 +136,7 @@
 For uploading the distribution packages to TestPyPI, do:
 ```
 python3 -m pip install --upgrade twine
 python3 -m twine upload --repository testpypi dist/*
 ```
 
 Use `__token__` when prompted to enter the username. For the password, use the token value, including the `pypi-` prefix.
-
-
```

### Comparing `DairyBrainUtils-0.3.3/README.md` & `DairyBrainUtils-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `DairyBrainUtils-0.3.3/setup.py` & `DairyBrainUtils-0.3.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="DairyBrainUtils",
-    version="0.3.3",
-    author="Rui Pan",
-    author_email="rpan33@wisc.edu",
+    version="0.3.7",
+    author="Rui Pan, Steve Wangen",
+    author_email="srwangen@wisc.edu",
     description="A set of functions that interacts with a database. It contains some basic functionalities along with some other Dairy-Brain-specific functionalities.",
+    install_requires=[
+        'SQLAlchemy',
+        'sqlalchemy_utils'
+        ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DairyBrain/AgDH_DairyBrainUtils",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

