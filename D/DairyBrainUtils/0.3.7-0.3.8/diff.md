# Comparing `tmp/DairyBrainUtils-0.3.7.tar.gz` & `tmp/DairyBrainUtils-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DairyBrainUtils-0.3.7.tar", last modified: Thu Apr 20 17:48:58 2023, max compression
+gzip compressed data, was "DairyBrainUtils-0.3.8.tar", last modified: Thu Apr 20 18:18:28 2023, max compression
```

## Comparing `DairyBrainUtils-0.3.7.tar` & `DairyBrainUtils-0.3.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 stevenwangen   (501) staff       (20)        0 2023-04-20 17:48:58.892456 DairyBrainUtils-0.3.7/
-drwxr-xr-x   0 stevenwangen   (501) staff       (20)        0 2023-04-20 17:48:58.889407 DairyBrainUtils-0.3.7/DairyBrainUtils/
--rw-r--r--   0 stevenwangen   (501) staff       (20)     8689 2023-04-20 17:46:20.000000 DairyBrainUtils-0.3.7/DairyBrainUtils/__init__.py
-drwxr-xr-x   0 stevenwangen   (501) staff       (20)        0 2023-04-20 17:48:58.891694 DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/
--rw-r--r--   0 stevenwangen   (501) staff       (20)     5793 2023-04-20 17:48:58.000000 DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/PKG-INFO
--rw-r--r--   0 stevenwangen   (501) staff       (20)      248 2023-04-20 17:48:58.000000 DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/SOURCES.txt
--rw-r--r--   0 stevenwangen   (501) staff       (20)        1 2023-04-20 17:48:58.000000 DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/dependency_links.txt
--rwxrwxrwx   0 stevenwangen   (501) staff       (20)       28 2023-04-20 17:48:58.000000 DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/requires.txt
--rw-r--r--   0 stevenwangen   (501) staff       (20)       16 2023-04-20 17:48:58.000000 DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/top_level.txt
--rw-r--r--   0 stevenwangen   (501) staff       (20)     1095 2023-04-20 17:24:08.000000 DairyBrainUtils-0.3.7/LICENSE
--rw-r--r--   0 stevenwangen   (501) staff       (20)     5793 2023-04-20 17:48:58.892123 DairyBrainUtils-0.3.7/PKG-INFO
--rw-r--r--   0 stevenwangen   (501) staff       (20)     5219 2023-04-20 17:24:08.000000 DairyBrainUtils-0.3.7/README.md
--rw-r--r--   0 stevenwangen   (501) staff       (20)       38 2023-04-20 17:48:58.892563 DairyBrainUtils-0.3.7/setup.cfg
--rw-r--r--   0 stevenwangen   (501) staff       (20)      873 2023-04-20 17:47:20.000000 DairyBrainUtils-0.3.7/setup.py
+drwxr-xr-x   0 stevenwangen   (501) staff       (20)        0 2023-04-20 18:18:28.285986 DairyBrainUtils-0.3.8/
+drwxr-xr-x   0 stevenwangen   (501) staff       (20)        0 2023-04-20 18:18:28.283275 DairyBrainUtils-0.3.8/DairyBrainUtils/
+-rw-r--r--   0 stevenwangen   (501) staff       (20)     8697 2023-04-20 18:18:07.000000 DairyBrainUtils-0.3.8/DairyBrainUtils/__init__.py
+drwxr-xr-x   0 stevenwangen   (501) staff       (20)        0 2023-04-20 18:18:28.285195 DairyBrainUtils-0.3.8/DairyBrainUtils.egg-info/
+-rw-r--r--   0 stevenwangen   (501) staff       (20)     5793 2023-04-20 18:18:28.000000 DairyBrainUtils-0.3.8/DairyBrainUtils.egg-info/PKG-INFO
+-rw-r--r--   0 stevenwangen   (501) staff       (20)      248 2023-04-20 18:18:28.000000 DairyBrainUtils-0.3.8/DairyBrainUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 stevenwangen   (501) staff       (20)        1 2023-04-20 18:18:28.000000 DairyBrainUtils-0.3.8/DairyBrainUtils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 stevenwangen   (501) staff       (20)       28 2023-04-20 18:18:28.000000 DairyBrainUtils-0.3.8/DairyBrainUtils.egg-info/requires.txt
+-rw-r--r--   0 stevenwangen   (501) staff       (20)       16 2023-04-20 18:18:28.000000 DairyBrainUtils-0.3.8/DairyBrainUtils.egg-info/top_level.txt
+-rw-r--r--   0 stevenwangen   (501) staff       (20)     1095 2023-04-20 17:24:08.000000 DairyBrainUtils-0.3.8/LICENSE
+-rw-r--r--   0 stevenwangen   (501) staff       (20)     5793 2023-04-20 18:18:28.285637 DairyBrainUtils-0.3.8/PKG-INFO
+-rw-r--r--   0 stevenwangen   (501) staff       (20)     5219 2023-04-20 17:24:08.000000 DairyBrainUtils-0.3.8/README.md
+-rw-r--r--   0 stevenwangen   (501) staff       (20)       38 2023-04-20 18:18:28.286087 DairyBrainUtils-0.3.8/setup.cfg
+-rw-r--r--   0 stevenwangen   (501) staff       (20)      873 2023-04-20 18:18:14.000000 DairyBrainUtils-0.3.8/setup.py
```

### Comparing `DairyBrainUtils-0.3.7/DairyBrainUtils/__init__.py` & `DairyBrainUtils-0.3.8/DairyBrainUtils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     if not has_table(table_name, db_engine):
         logger.debug("Table {} not found - creating...".format(table_name))
 
         with db_engine.connect() as con:
             try:
                 logger.info("Creating table " + table_name + " in " + db_engine.url.database + " database...")
                 logger.debug('create_temp_table_statement = ' + str(sql_statement.format(table_name)))
-                con.execute(str(sql_statement.format(table_name)))
+                con.execute(text(sql_statement.format(table_name)))
             except Exception as e:
                 print("The exception is " + str(e))
                 logger.error("Error creating the table " + table_name + " in " + db_engine.url.database + " database!")
                 logger.error(e.args)
                 exit(1)
 
 
@@ -73,15 +73,15 @@
     drop_table(table_name, db_engine)
 
     # create new temp table
     with db_engine.connect() as con:
         try:
             logger.info("Creating table " + table_name + " in " + db_engine.url.database + " database...")
             logger.debug('create_temp_table_statement = ' + str(sql_statement.format(table_name)))
-            con.execute(str(sql_statement.format(table_name)))
+            con.execute(text(sql_statement.format(table_name)))
         except Exception as e:
             print("The exception is " + str(e))
             logger.error("Error creating the table " + table_name + " in " + db_engine.url.database + " database!")
             logger.error(e.args)
             exit(1)
 
 
@@ -204,15 +204,15 @@
     """
     if has_table(table_name, db_engine):
         logger.debug("Deleting old (pre-existing) table: " + table_name + "...")
         statement = str("DROP TABLE IF EXISTS {};")
 
         with db_engine.connect() as con:
             try:
-                con.execute(statement.format(table_name))
+                con.execute(text(statement.format(table_name)))
             except Exception as e:
                 logger.error("Error deleting table " + table_name + " from database!")
                 logger.error(e.args)
                 exit(1)
 
 
 def has_table(table_name, db_engine):
```

### Comparing `DairyBrainUtils-0.3.7/DairyBrainUtils.egg-info/PKG-INFO` & `DairyBrainUtils-0.3.8/DairyBrainUtils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DairyBrainUtils
-Version: 0.3.7
+Version: 0.3.8
 Summary: A set of functions that interacts with a database. It contains some basic functionalities along with some other Dairy-Brain-specific functionalities.
 Home-page: https://github.com/DairyBrain/AgDH_DairyBrainUtils
 Author: Rui Pan, Steve Wangen
 Author-email: srwangen@wisc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DairyBrainUtils-0.3.7/LICENSE` & `DairyBrainUtils-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `DairyBrainUtils-0.3.7/PKG-INFO` & `DairyBrainUtils-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DairyBrainUtils
-Version: 0.3.7
+Version: 0.3.8
 Summary: A set of functions that interacts with a database. It contains some basic functionalities along with some other Dairy-Brain-specific functionalities.
 Home-page: https://github.com/DairyBrain/AgDH_DairyBrainUtils
 Author: Rui Pan, Steve Wangen
 Author-email: srwangen@wisc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DairyBrainUtils-0.3.7/README.md` & `DairyBrainUtils-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `DairyBrainUtils-0.3.7/setup.py` & `DairyBrainUtils-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="DairyBrainUtils",
-    version="0.3.7",
+    version="0.3.8",
     author="Rui Pan, Steve Wangen",
     author_email="srwangen@wisc.edu",
     description="A set of functions that interacts with a database. It contains some basic functionalities along with some other Dairy-Brain-specific functionalities.",
     install_requires=[
         'SQLAlchemy',
         'sqlalchemy_utils'
         ],
```

