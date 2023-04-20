# Comparing `tmp/SIOTCommon-0.0.9.6.tar.gz` & `tmp/SIOTCommon-0.0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.0.9.6.tar", last modified: Thu Apr 20 13:30:11 2023, max compression
+gzip compressed data, was "SIOTCommon-0.0.9.7.tar", last modified: Thu Apr 20 13:34:18 2023, max compression
```

## Comparing `SIOTCommon-0.0.9.6.tar` & `SIOTCommon-0.0.9.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 13:30:11.335346 SIOTCommon-0.0.9.6/
--rw-rw-rw-   0        0        0      341 2023-04-20 13:30:11.334347 SIOTCommon-0.0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.9.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 13:30:11.312349 SIOTCommon-0.0.9.6/SIOTC/
--rw-rw-rw-   0        0        0     1843 2023-04-20 13:29:33.000000 SIOTCommon-0.0.9.6/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0     7680 2023-04-20 13:23:27.000000 SIOTCommon-0.0.9.6/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.9.6/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     2648 2023-04-20 13:27:13.000000 SIOTCommon-0.0.9.6/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-04-20 13:30:11.331364 SIOTCommon-0.0.9.6/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      341 2023-04-20 13:30:11.000000 SIOTCommon-0.0.9.6/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-20 13:30:11.000000 SIOTCommon-0.0.9.6/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 13:30:11.000000 SIOTCommon-0.0.9.6/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      636 2023-04-20 13:30:11.000000 SIOTCommon-0.0.9.6/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 13:30:11.000000 SIOTCommon-0.0.9.6/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 13:30:11.335346 SIOTCommon-0.0.9.6/setup.cfg
--rw-rw-rw-   0        0        0      583 2023-04-20 13:29:57.000000 SIOTCommon-0.0.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 13:34:18.704012 SIOTCommon-0.0.9.7/
+-rw-rw-rw-   0        0        0      341 2023-04-20 13:34:18.704012 SIOTCommon-0.0.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.9.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 13:34:18.685014 SIOTCommon-0.0.9.7/SIOTC/
+-rw-rw-rw-   0        0        0     1843 2023-04-20 13:29:33.000000 SIOTCommon-0.0.9.7/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0     7635 2023-04-20 13:33:17.000000 SIOTCommon-0.0.9.7/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      484 2023-04-20 13:32:21.000000 SIOTCommon-0.0.9.7/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     2648 2023-04-20 13:27:13.000000 SIOTCommon-0.0.9.7/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-04-20 13:34:18.702013 SIOTCommon-0.0.9.7/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      341 2023-04-20 13:34:18.000000 SIOTCommon-0.0.9.7/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-20 13:34:18.000000 SIOTCommon-0.0.9.7/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 13:34:18.000000 SIOTCommon-0.0.9.7/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      636 2023-04-20 13:34:18.000000 SIOTCommon-0.0.9.7/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 13:34:18.000000 SIOTCommon-0.0.9.7/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 13:34:18.705013 SIOTCommon-0.0.9.7/setup.cfg
+-rw-rw-rw-   0        0        0      583 2023-04-20 13:34:15.000000 SIOTCommon-0.0.9.7/setup.py
```

### Comparing `SIOTCommon-0.0.9.6/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.0.9.7/SIOTC/DatabaseLayer.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.6/SIOTC/Operations.py` & `SIOTCommon-0.0.9.7/SIOTC/Operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from SIOTC import DatabaseLayer
-from DatabaseLayer import CreateTableObject
 from sqlalchemy.exc import SQLAlchemyError, IntegrityError
 dl = DatabaseLayer
 
 def executeQuery(query_func, *args, **kwargs):
     # Get a database session and the SQLAlchemy Base object
     session, base = dl.GetSession()
     try:
```

### Comparing `SIOTCommon-0.0.9.6/SIOTC/helperhttps.py` & `SIOTCommon-0.0.9.7/SIOTC/helperhttps.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.6/SIOTCommon.egg-info/requires.txt` & `SIOTCommon-0.0.9.7/SIOTCommon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.6/setup.py` & `SIOTCommon-0.0.9.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.0.9.6',
+    version='0.0.9.7',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```

