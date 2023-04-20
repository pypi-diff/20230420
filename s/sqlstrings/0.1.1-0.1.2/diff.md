# Comparing `tmp/sqlstrings-0.1.1.tar.gz` & `tmp/sqlstrings-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlstrings-0.1.1.tar", last modified: Thu Apr 20 11:13:55 2023, max compression
+gzip compressed data, was "sqlstrings-0.1.2.tar", last modified: Thu Apr 20 11:22:24 2023, max compression
```

## Comparing `sqlstrings-0.1.1.tar` & `sqlstrings-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 11:13:55.812013 sqlstrings-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-04-17 15:39:37.000000 sqlstrings-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      894 2023-04-20 11:13:55.811008 sqlstrings-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-19 16:09:43.000000 sqlstrings-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 11:13:55.814025 sqlstrings-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      792 2023-04-20 11:13:46.000000 sqlstrings-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 11:13:55.778009 sqlstrings-0.1.1/sqlstrings/
--rw-rw-rw-   0        0        0       67 2023-04-17 15:00:41.000000 sqlstrings-0.1.1/sqlstrings/__init__.py
--rw-rw-rw-   0        0        0     3597 2023-04-20 10:08:31.000000 sqlstrings-0.1.1/sqlstrings/csv_handling.py
--rw-rw-rw-   0        0        0     4542 2023-04-20 10:00:39.000000 sqlstrings-0.1.1/sqlstrings/postgre.py
--rw-rw-rw-   0        0        0     4175 2023-04-20 09:59:55.000000 sqlstrings-0.1.1/sqlstrings/transact.py
--rw-rw-rw-   0        0        0     2053 2023-04-20 08:23:09.000000 sqlstrings-0.1.1/sqlstrings/value_handling.py
-drwxrwxrwx   0        0        0        0 2023-04-20 11:13:55.798009 sqlstrings-0.1.1/sqlstrings.egg-info/
--rw-rw-rw-   0        0        0      894 2023-04-20 11:13:55.000000 sqlstrings-0.1.1/sqlstrings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-04-20 11:13:55.000000 sqlstrings-0.1.1/sqlstrings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 11:13:55.000000 sqlstrings-0.1.1/sqlstrings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 11:13:55.000000 sqlstrings-0.1.1/sqlstrings.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 11:13:55.810008 sqlstrings-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-04-17 15:36:45.000000 sqlstrings-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0       30 2023-03-31 16:34:51.000000 sqlstrings-0.1.1/tests/test_csv_handling.py
--rw-rw-rw-   0        0        0      163 2023-04-17 15:38:11.000000 sqlstrings-0.1.1/tests/test_main.py
--rw-rw-rw-   0        0        0     2474 2023-04-17 15:39:16.000000 sqlstrings-0.1.1/tests/test_postgre.py
--rw-rw-rw-   0        0        0     1986 2023-04-17 15:38:37.000000 sqlstrings-0.1.1/tests/test_transact.py
--rw-rw-rw-   0        0        0     1634 2023-04-17 15:38:35.000000 sqlstrings-0.1.1/tests/test_value_handling.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:22:24.410234 sqlstrings-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 15:39:37.000000 sqlstrings-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      902 2023-04-20 11:22:24.409232 sqlstrings-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-20 11:19:14.000000 sqlstrings-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 11:22:24.411236 sqlstrings-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-04-20 11:19:47.000000 sqlstrings-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:22:24.376235 sqlstrings-0.1.2/sqlstrings/
+-rw-rw-rw-   0        0        0      188 2023-04-20 11:21:31.000000 sqlstrings-0.1.2/sqlstrings/__init__.py
+-rw-rw-rw-   0        0        0     3597 2023-04-20 10:08:31.000000 sqlstrings-0.1.2/sqlstrings/csv_handling.py
+-rw-rw-rw-   0        0        0     4542 2023-04-20 10:00:39.000000 sqlstrings-0.1.2/sqlstrings/postgre.py
+-rw-rw-rw-   0        0        0     4175 2023-04-20 09:59:55.000000 sqlstrings-0.1.2/sqlstrings/transact.py
+-rw-rw-rw-   0        0        0     2053 2023-04-20 08:23:09.000000 sqlstrings-0.1.2/sqlstrings/value_handling.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:22:24.394231 sqlstrings-0.1.2/sqlstrings.egg-info/
+-rw-rw-rw-   0        0        0      902 2023-04-20 11:22:24.000000 sqlstrings-0.1.2/sqlstrings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-04-20 11:22:24.000000 sqlstrings-0.1.2/sqlstrings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 11:22:24.000000 sqlstrings-0.1.2/sqlstrings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 11:22:24.000000 sqlstrings-0.1.2/sqlstrings.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 11:22:24.407232 sqlstrings-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-17 15:36:45.000000 sqlstrings-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-03-31 16:34:51.000000 sqlstrings-0.1.2/tests/test_csv_handling.py
+-rw-rw-rw-   0        0        0      163 2023-04-17 15:38:11.000000 sqlstrings-0.1.2/tests/test_main.py
+-rw-rw-rw-   0        0        0     2474 2023-04-17 15:39:16.000000 sqlstrings-0.1.2/tests/test_postgre.py
+-rw-rw-rw-   0        0        0     1986 2023-04-17 15:38:37.000000 sqlstrings-0.1.2/tests/test_transact.py
+-rw-rw-rw-   0        0        0     1634 2023-04-17 15:38:35.000000 sqlstrings-0.1.2/tests/test_value_handling.py
```

### Comparing `sqlstrings-0.1.1/LICENSE.txt` & `sqlstrings-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.1.1/PKG-INFO` & `sqlstrings-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlstrings
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generates SQL query strings in multiple dialects.
 Home-page: https://github.com/alikellaway/sqlstrings
 Author: Ali Kellaway
 Author-email: ali.kellaway139@gmail.com
 License: MIT
 Keywords: sql strings generate query
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # sqlstrings
 Package generates SQL query strings in multiple dialects. It is also able to take in csv files and convert them into statements for easy upload of csv files into databases.
 
 # Installation
-Run the following to install:
-'''python
+Run the following command to install:
+```python
 pip install sqlstrings
-'''
+```
 
 # Contribute
 Repo: https://github.com/alikellaway/sqlstrings
```

### Comparing `sqlstrings-0.1.1/setup.py` & `sqlstrings-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from pathlib import Path
 
 setup(
     name='sqlstrings',
-    version='0.1.1',    
+    version='0.1.2',    
     description='Generates SQL query strings in multiple dialects.',
     long_description= (Path(__file__).parent / "README.md").read_text(),
     long_description_content_type = 'text/markdown',
     keywords='sql strings generate query',
     url='https://github.com/alikellaway/sqlstrings',
     author='Ali Kellaway',
     author_email='ali.kellaway139@gmail.com',
```

### Comparing `sqlstrings-0.1.1/sqlstrings/csv_handling.py` & `sqlstrings-0.1.2/sqlstrings/csv_handling.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.1.1/sqlstrings/postgre.py` & `sqlstrings-0.1.2/sqlstrings/postgre.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.1.1/sqlstrings/transact.py` & `sqlstrings-0.1.2/sqlstrings/transact.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.1.1/sqlstrings/value_handling.py` & `sqlstrings-0.1.2/sqlstrings/value_handling.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.1.1/sqlstrings.egg-info/PKG-INFO` & `sqlstrings-0.1.2/sqlstrings.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlstrings
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generates SQL query strings in multiple dialects.
 Home-page: https://github.com/alikellaway/sqlstrings
 Author: Ali Kellaway
 Author-email: ali.kellaway139@gmail.com
 License: MIT
 Keywords: sql strings generate query
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # sqlstrings
 Package generates SQL query strings in multiple dialects. It is also able to take in csv files and convert them into statements for easy upload of csv files into databases.
 
 # Installation
-Run the following to install:
-'''python
+Run the following command to install:
+```python
 pip install sqlstrings
-'''
+```
 
 # Contribute
 Repo: https://github.com/alikellaway/sqlstrings
```

### Comparing `sqlstrings-0.1.1/tests/test_postgre.py` & `sqlstrings-0.1.2/tests/test_postgre.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.1.1/tests/test_transact.py` & `sqlstrings-0.1.2/tests/test_transact.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.1.1/tests/test_value_handling.py` & `sqlstrings-0.1.2/tests/test_value_handling.py`

 * *Files identical despite different names*

