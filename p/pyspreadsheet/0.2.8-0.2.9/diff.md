# Comparing `tmp/pyspreadsheet-0.2.8.tar.gz` & `tmp/pyspreadsheet-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyspreadsheet-0.2.8.tar", last modified: Mon Apr 19 10:12:13 2021, max compression
+gzip compressed data, was "dist/pyspreadsheet-0.2.9.tar", last modified: Wed Apr 21 17:17:05 2021, max compression
```

## Comparing `pyspreadsheet-0.2.8.tar` & `pyspreadsheet-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2021-04-19 10:12:13.000000 pyspreadsheet-0.2.8/
--rw-r--r--   0 vincent    (501) staff       (20)      345 2021-04-19 10:12:13.000000 pyspreadsheet-0.2.8/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)     1278 2018-12-14 14:57:40.000000 pyspreadsheet-0.2.8/LICENSE
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2021-04-19 10:12:13.000000 pyspreadsheet-0.2.8/pyspreadsheet/
--rw-r--r--   0 vincent    (501) staff       (20)    16792 2021-04-19 10:11:51.000000 pyspreadsheet-0.2.8/pyspreadsheet/Spreadsheet.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2021-04-19 10:12:13.000000 pyspreadsheet-0.2.8/pyspreadsheet/core/
--rw-r--r--   0 vincent    (501) staff       (20)     1341 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.8/pyspreadsheet/core/manage_sheet.py
--rw-r--r--   0 vincent    (501) staff       (20)     1439 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.8/pyspreadsheet/core/write.py
--rw-r--r--   0 vincent    (501) staff       (20)        0 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.8/pyspreadsheet/core/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      876 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.8/pyspreadsheet/core/tool.py
--rw-r--r--   0 vincent    (501) staff       (20)     2125 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.8/pyspreadsheet/core/read.py
--rw-r--r--   0 vincent    (501) staff       (20)       50 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.8/pyspreadsheet/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)       15 2018-12-14 14:57:40.000000 pyspreadsheet-0.2.8/MANIFEST.in
--rw-r--r--   0 vincent    (501) staff       (20)      706 2021-04-19 10:11:58.000000 pyspreadsheet-0.2.8/setup.py
--rw-r--r--   0 vincent    (501) staff       (20)       38 2021-04-19 10:12:13.000000 pyspreadsheet-0.2.8/setup.cfg
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2021-04-19 10:12:13.000000 pyspreadsheet-0.2.8/pyspreadsheet.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      345 2021-04-19 10:12:12.000000 pyspreadsheet-0.2.8/pyspreadsheet.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      426 2021-04-19 10:12:12.000000 pyspreadsheet-0.2.8/pyspreadsheet.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)      123 2021-04-19 10:12:12.000000 pyspreadsheet-0.2.8/pyspreadsheet.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)       14 2021-04-19 10:12:12.000000 pyspreadsheet-0.2.8/pyspreadsheet.egg-info/top_level.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2021-04-19 10:12:12.000000 pyspreadsheet-0.2.8/pyspreadsheet.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)       15 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.8/README.rst
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2021-04-21 17:17:05.000000 pyspreadsheet-0.2.9/
+-rw-r--r--   0 vincent    (501) staff       (20)      345 2021-04-21 17:17:05.000000 pyspreadsheet-0.2.9/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)     1278 2018-12-14 14:57:40.000000 pyspreadsheet-0.2.9/LICENSE
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2021-04-21 17:17:05.000000 pyspreadsheet-0.2.9/pyspreadsheet/
+-rw-r--r--   0 vincent    (501) staff       (20)    17663 2021-04-21 17:16:33.000000 pyspreadsheet-0.2.9/pyspreadsheet/Spreadsheet.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2021-04-21 17:17:05.000000 pyspreadsheet-0.2.9/pyspreadsheet/core/
+-rw-r--r--   0 vincent    (501) staff       (20)     1341 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.9/pyspreadsheet/core/manage_sheet.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1439 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.9/pyspreadsheet/core/write.py
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.9/pyspreadsheet/core/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      876 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.9/pyspreadsheet/core/tool.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2125 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.9/pyspreadsheet/core/read.py
+-rw-r--r--   0 vincent    (501) staff       (20)       50 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.9/pyspreadsheet/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)       15 2018-12-14 14:57:40.000000 pyspreadsheet-0.2.9/MANIFEST.in
+-rw-r--r--   0 vincent    (501) staff       (20)      732 2021-04-21 17:16:33.000000 pyspreadsheet-0.2.9/setup.py
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2021-04-21 17:17:05.000000 pyspreadsheet-0.2.9/setup.cfg
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2021-04-21 17:17:05.000000 pyspreadsheet-0.2.9/pyspreadsheet.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      345 2021-04-21 17:17:05.000000 pyspreadsheet-0.2.9/pyspreadsheet.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      426 2021-04-21 17:17:05.000000 pyspreadsheet-0.2.9/pyspreadsheet.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)      138 2021-04-21 17:17:05.000000 pyspreadsheet-0.2.9/pyspreadsheet.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       14 2021-04-21 17:17:05.000000 pyspreadsheet-0.2.9/pyspreadsheet.egg-info/top_level.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2021-04-21 17:17:05.000000 pyspreadsheet-0.2.9/pyspreadsheet.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       15 2021-04-05 12:49:20.000000 pyspreadsheet-0.2.9/README.rst
```

### Comparing `pyspreadsheet-0.2.8/LICENSE` & `pyspreadsheet-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspreadsheet-0.2.8/pyspreadsheet/Spreadsheet.py` & `pyspreadsheet-0.2.9/pyspreadsheet/Spreadsheet.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import copy
 import json
 
 import pygsheets
 import requests
 import googleapiclient
 import yaml
+import jinja2
 from googleauthentication import GoogleAuthentication
 from dbstream import DBStream
 
 from pyspreadsheet.core import write
 from pyspreadsheet.core.manage_sheet import add_worksheet
 
 from pyspreadsheet.core.read import check_availability_column
@@ -44,21 +45,23 @@
 
 class Spreadsheet:
     def __init__(self,
                  googleauthentication: GoogleAuthentication,
                  dbstream: DBStream = None,
                  dbstream_spreadsheet_schema_name=None,
                  data_collection_config_path=None,
+                 data_collection_config_params_path=None,
                  include_collection_in_table_name=False):
         self.googleauthentication = googleauthentication
         self.dbstream = dbstream
         self.account = googleauthentication.get_account("sheets").spreadsheets()
         self.dbstream_spreadsheet_schema_name = "spreadsheet" if dbstream_spreadsheet_schema_name is None \
             else dbstream_spreadsheet_schema_name
         self.data_collection_config_path = data_collection_config_path
+        self.data_collection_config_params_path = data_collection_config_params_path
         self.include_collection_in_table_name = include_collection_in_table_name
 
     def send(self, sheet_id, data):
         try:
             available_response = check_availability_column(self, sheet_id, data)
         except googleapiclient.errors.HttpError:
             add_worksheet(self, sheet_id, data["worksheet_name"])
@@ -195,15 +198,23 @@
             fileId=spreadsheet_id,
             fields="lastModifyingUser,modifiedTime",
             supportsAllDrives=True
         ).execute()
         return r["modifiedTime"], r["lastModifyingUser"].get("emailAddress")
 
     def get_info_from_worksheet(self, key, **kwargs):
-        config = yaml.load(open(self.data_collection_config_path), Loader=yaml.FullLoader)
+        jinja_env = jinja2.Environment()
+        params = {}
+        if self.data_collection_config_params_path:
+            params = yaml.load(
+                jinja_env.from_string(open(self.data_collection_config_params_path).read()).render(),
+                Loader=yaml.FullLoader)
+        config = yaml.load(
+            jinja_env.from_string(open(self.data_collection_config_path).read()).render(params),
+            Loader=yaml.FullLoader)
         key_config = config[key]
         worksheet_name = key_config['worksheet_name']
         spreadsheet_id = key_config['sheet_id']
         last_spreadsheet_update_time, last_spreadsheet_update_by = self.get_last_spreadsheet_update_time(
             spreadsheet_id)
         print(last_spreadsheet_update_time, last_spreadsheet_update_by)
         loaded_sheet_table = "_loaded_sheets"
@@ -352,15 +363,23 @@
         except Exception as e:
             raise Exception(
                 "error to treat and/or send %s which ID is %s in schema %s : %s" % (
                     str(worksheet_name), str(spreadsheet_id), str(table_name), str(e))
             )
 
     def get_info_from_worksheets(self, **kwargs):
-        config = yaml.load(open(self.data_collection_config_path), Loader=yaml.FullLoader)
+        jinja_env = jinja2.Environment()
+        params = {}
+        if self.data_collection_config_params_path:
+            params = yaml.load(
+                jinja_env.from_string(open(self.data_collection_config_params_path).read()).render(),
+                Loader=yaml.FullLoader)
+        config = yaml.load(
+            jinja_env.from_string(open(self.data_collection_config_path).read()).render(params),
+            Loader=yaml.FullLoader)
         dict_error = dict()
         for key in config:
             try:
                 self.get_info_from_worksheet(key, **kwargs)
             except Exception as e:
                 dict_error[key] = str(e)
                 pass
```

### Comparing `pyspreadsheet-0.2.8/pyspreadsheet/core/manage_sheet.py` & `pyspreadsheet-0.2.9/pyspreadsheet/core/manage_sheet.py`

 * *Files identical despite different names*

### Comparing `pyspreadsheet-0.2.8/pyspreadsheet/core/write.py` & `pyspreadsheet-0.2.9/pyspreadsheet/core/write.py`

 * *Files identical despite different names*

### Comparing `pyspreadsheet-0.2.8/pyspreadsheet/core/tool.py` & `pyspreadsheet-0.2.9/pyspreadsheet/core/tool.py`

 * *Files identical despite different names*

### Comparing `pyspreadsheet-0.2.8/pyspreadsheet/core/read.py` & `pyspreadsheet-0.2.9/pyspreadsheet/core/read.py`

 * *Files identical despite different names*

### Comparing `pyspreadsheet-0.2.8/setup.py` & `pyspreadsheet-0.2.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 with open('README.rst') as f:
     readme = f.read()
 
 setup(
     name='pyspreadsheet',
-    version='0.2.8',
+    version='0.2.9',
     description='Easily send data to Google Sheets',
     long_description=readme,
     author='Dacker',
     author_email='hello@dacker.co',
     url='https://github.com/dacker-team/pyspreadsheet',
     keywords='send data google spreadsheet sheets easy',
     packages=find_packages(exclude=('tests', 'docs')),
     python_requires='>=3',
     install_requires=[
         "googleauthentication>=0.0.10",
         "dbstream>=0.0.12",
         "google-api-python-client>=1.6.6",
         "pygsheets==2.0.2",
         "pyyaml>=5.3.1",
-        "google-auth>="
+        "google-auth>=",
+        "jinja2>=2.11.3"
     ],
 )
```

