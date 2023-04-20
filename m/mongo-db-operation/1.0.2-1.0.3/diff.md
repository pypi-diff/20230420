# Comparing `tmp/mongo-db-operation-1.0.2.tar.gz` & `tmp/mongo_db_operation-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo-db-operation-1.0.2.tar", last modified: Wed Apr 19 14:30:22 2023, max compression
+gzip compressed data, was "mongo_db_operation-1.0.3.tar", last modified: Thu Apr 20 19:47:33 2023, max compression
```

## Comparing `mongo-db-operation-1.0.2.tar` & `mongo_db_operation-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 14:30:22.541299 mongo-db-operation-1.0.2/
--rw-r--r--   0 MTeke1     (502) staff       (20)    35149 2023-04-19 13:31:34.000000 mongo-db-operation-1.0.2/LICENSE
--rw-r--r--   0 MTeke1     (502) staff       (20)     9484 2023-04-19 14:30:22.540949 mongo-db-operation-1.0.2/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)     8939 2023-04-19 14:16:52.000000 mongo-db-operation-1.0.2/README.md
--rw-r--r--   0 MTeke1     (502) staff       (20)      529 2023-04-19 14:29:56.000000 mongo-db-operation-1.0.2/pyproject.toml
--rw-r--r--   0 MTeke1     (502) staff       (20)       38 2023-04-19 14:30:22.541412 mongo-db-operation-1.0.2/setup.cfg
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 14:30:22.537249 mongo-db-operation-1.0.2/src/
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 14:30:22.539433 mongo-db-operation-1.0.2/src/mongo_db_operation/
--rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-04-19 13:39:36.000000 mongo-db-operation-1.0.2/src/mongo_db_operation/__init__.py
--rw-r--r--   0 MTeke1     (502) staff       (20)      299 2023-04-19 13:46:22.000000 mongo-db-operation-1.0.2/src/mongo_db_operation/environment.py
--rw-r--r--   0 MTeke1     (502) staff       (20)     1958 2023-04-19 14:07:50.000000 mongo-db-operation-1.0.2/src/mongo_db_operation/mongo_client.py
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-19 14:30:22.540669 mongo-db-operation-1.0.2/src/mongo_db_operation.egg-info/
--rw-r--r--   0 MTeke1     (502) staff       (20)     9484 2023-04-19 14:30:22.000000 mongo-db-operation-1.0.2/src/mongo_db_operation.egg-info/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)      328 2023-04-19 14:30:22.000000 mongo-db-operation-1.0.2/src/mongo_db_operation.egg-info/SOURCES.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)        1 2023-04-19 14:30:22.000000 mongo-db-operation-1.0.2/src/mongo_db_operation.egg-info/dependency_links.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)       19 2023-04-19 14:30:22.000000 mongo-db-operation-1.0.2/src/mongo_db_operation.egg-info/top_level.txt
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-20 19:47:33.481994 mongo_db_operation-1.0.3/
+-rw-r--r--   0 MTeke1     (502) staff       (20)      206 2023-04-20 19:47:33.481851 mongo_db_operation-1.0.3/PKG-INFO
+-rw-r--r--   0 MTeke1     (502) staff       (20)     8939 2023-04-19 14:16:52.000000 mongo_db_operation-1.0.3/README.md
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-20 19:47:33.480593 mongo_db_operation-1.0.3/mongo_db_operation.egg-info/
+-rw-r--r--   0 MTeke1     (502) staff       (20)      206 2023-04-20 19:47:33.000000 mongo_db_operation-1.0.3/mongo_db_operation.egg-info/PKG-INFO
+-rw-r--r--   0 MTeke1     (502) staff       (20)      354 2023-04-20 19:47:33.000000 mongo_db_operation-1.0.3/mongo_db_operation.egg-info/SOURCES.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)        1 2023-04-20 19:47:33.000000 mongo_db_operation-1.0.3/mongo_db_operation.egg-info/dependency_links.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)        8 2023-04-20 19:47:33.000000 mongo_db_operation-1.0.3/mongo_db_operation.egg-info/requires.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)       23 2023-04-20 19:47:33.000000 mongo_db_operation-1.0.3/mongo_db_operation.egg-info/top_level.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)      620 2023-04-20 19:46:58.000000 mongo_db_operation-1.0.3/pyproject.toml
+-rw-r--r--   0 MTeke1     (502) staff       (20)       38 2023-04-20 19:47:33.482053 mongo_db_operation-1.0.3/setup.cfg
+-rw-r--r--   0 MTeke1     (502) staff       (20)      243 2023-04-20 19:47:30.000000 mongo_db_operation-1.0.3/setup.py
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-20 19:47:33.478841 mongo_db_operation-1.0.3/src/
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-20 19:47:33.481374 mongo_db_operation-1.0.3/src/mongo_db_operation/
+-rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-04-19 13:39:36.000000 mongo_db_operation-1.0.3/src/mongo_db_operation/__init__.py
+-rw-r--r--   0 MTeke1     (502) staff       (20)      299 2023-04-19 13:46:22.000000 mongo_db_operation-1.0.3/src/mongo_db_operation/environment.py
+-rw-r--r--   0 MTeke1     (502) staff       (20)     1958 2023-04-19 14:07:50.000000 mongo_db_operation-1.0.3/src/mongo_db_operation/mongo_client.py
```

### Comparing `mongo-db-operation-1.0.2/PKG-INFO` & `mongo_db_operation-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: mongo-db-operation
-Version: 1.0.2
-Summary: A small package for CRUD operations for Mongo DB
-Author-email: Melih Teke <me@mteke.com>
-Project-URL: Homepage, https://github.com/melihteke/mongo-db-operation
-Project-URL: Bug Tracker, https://github.com/melihteke/mongo-db-operation/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## MongoDB Python CRUD Operations
 
 This project offers an easy-to-use Python interface that enables you to perform CRUD (Create, Read, Update, Delete) operations on a MongoDB database. It uses the PyMongo library and is designed to work seamlessly with a prebuilt MongoDB instance installed on your system or hosted elsewhere.
 To use this code, you'll need a prebuilt MongoDB instance that's up and running. In my case, I created a MongoDB instance through https://cloud.mongodb.com/. However, you can also run your database locally or use a different provider if you prefer. Just make sure that your MongoDB instance is configured correctly before you start working with the code.
 To ensure that the code can connect to your MongoDB instance, it's important to whitelist the appropriate IP addresses. This can be done using a mask or by specifying specific IP addresses. Before you start working with the code, make sure that your MongoDB instance is reachable via whitelisting. This will ensure that your code can access the database without any issues.
 
 ![image](https://user-images.githubusercontent.com/36086368/231573735-4af57894-d0a2-415c-ab29-8a26e4d67e06.png)
@@ -293,8 +279,8 @@
 In [19]: 
 ```
 
 
 
 
   
-  
+
```

### Comparing `mongo-db-operation-1.0.2/src/mongo_db_operation/mongo_client.py` & `mongo_db_operation-1.0.3/src/mongo_db_operation/mongo_client.py`

 * *Files identical despite different names*

