# Comparing `tmp/sqlstrings-0.0.9.tar.gz` & `tmp/sqlstrings-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlstrings-0.0.9.tar", last modified: Thu Apr 20 10:26:04 2023, max compression
+gzip compressed data, was "sqlstrings-0.1.0.tar", last modified: Thu Apr 20 10:28:59 2023, max compression
```

## Comparing `sqlstrings-0.0.9.tar` & `sqlstrings-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 10:26:04.147252 sqlstrings-0.0.9/
--rw-rw-rw-   0        0        0     1091 2023-04-17 15:39:37.000000 sqlstrings-0.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0      853 2023-04-20 10:26:04.146265 sqlstrings-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-19 16:09:43.000000 sqlstrings-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 10:26:04.148253 sqlstrings-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-20 10:25:36.000000 sqlstrings-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 10:26:04.110266 sqlstrings-0.0.9/sqlstrings/
--rw-rw-rw-   0        0        0       67 2023-04-17 15:00:41.000000 sqlstrings-0.0.9/sqlstrings/__init__.py
--rw-rw-rw-   0        0        0     3597 2023-04-20 10:08:31.000000 sqlstrings-0.0.9/sqlstrings/csv_handling.py
--rw-rw-rw-   0        0        0     4542 2023-04-20 10:00:39.000000 sqlstrings-0.0.9/sqlstrings/postgre.py
--rw-rw-rw-   0        0        0     4175 2023-04-20 09:59:55.000000 sqlstrings-0.0.9/sqlstrings/transact.py
--rw-rw-rw-   0        0        0     2053 2023-04-20 08:23:09.000000 sqlstrings-0.0.9/sqlstrings/value_handling.py
-drwxrwxrwx   0        0        0        0 2023-04-20 10:26:04.131243 sqlstrings-0.0.9/sqlstrings.egg-info/
--rw-rw-rw-   0        0        0      853 2023-04-20 10:26:04.000000 sqlstrings-0.0.9/sqlstrings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-04-20 10:26:04.000000 sqlstrings-0.0.9/sqlstrings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 10:26:04.000000 sqlstrings-0.0.9/sqlstrings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 10:26:04.000000 sqlstrings-0.0.9/sqlstrings.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 10:26:04.143246 sqlstrings-0.0.9/tests/
--rw-rw-rw-   0        0        0        0 2023-04-17 15:36:45.000000 sqlstrings-0.0.9/tests/__init__.py
--rw-rw-rw-   0        0        0       30 2023-03-31 16:34:51.000000 sqlstrings-0.0.9/tests/test_csv_handling.py
--rw-rw-rw-   0        0        0      163 2023-04-17 15:38:11.000000 sqlstrings-0.0.9/tests/test_main.py
--rw-rw-rw-   0        0        0     2474 2023-04-17 15:39:16.000000 sqlstrings-0.0.9/tests/test_postgre.py
--rw-rw-rw-   0        0        0     1986 2023-04-17 15:38:37.000000 sqlstrings-0.0.9/tests/test_transact.py
--rw-rw-rw-   0        0        0     1634 2023-04-17 15:38:35.000000 sqlstrings-0.0.9/tests/test_value_handling.py
+drwxrwxrwx   0        0        0        0 2023-04-20 10:28:59.730843 sqlstrings-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 15:39:37.000000 sqlstrings-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      853 2023-04-20 10:28:59.729845 sqlstrings-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-19 16:09:43.000000 sqlstrings-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 10:28:59.730843 sqlstrings-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      791 2023-04-20 10:28:57.000000 sqlstrings-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 10:28:59.675846 sqlstrings-0.1.0/sqlstrings/
+-rw-rw-rw-   0        0        0       67 2023-04-17 15:00:41.000000 sqlstrings-0.1.0/sqlstrings/__init__.py
+-rw-rw-rw-   0        0        0     3597 2023-04-20 10:08:31.000000 sqlstrings-0.1.0/sqlstrings/csv_handling.py
+-rw-rw-rw-   0        0        0     4542 2023-04-20 10:00:39.000000 sqlstrings-0.1.0/sqlstrings/postgre.py
+-rw-rw-rw-   0        0        0     4175 2023-04-20 09:59:55.000000 sqlstrings-0.1.0/sqlstrings/transact.py
+-rw-rw-rw-   0        0        0     2053 2023-04-20 08:23:09.000000 sqlstrings-0.1.0/sqlstrings/value_handling.py
+drwxrwxrwx   0        0        0        0 2023-04-20 10:28:59.713846 sqlstrings-0.1.0/sqlstrings.egg-info/
+-rw-rw-rw-   0        0        0      853 2023-04-20 10:28:59.000000 sqlstrings-0.1.0/sqlstrings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-04-20 10:28:59.000000 sqlstrings-0.1.0/sqlstrings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 10:28:59.000000 sqlstrings-0.1.0/sqlstrings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 10:28:59.000000 sqlstrings-0.1.0/sqlstrings.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 10:28:59.728855 sqlstrings-0.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-17 15:36:45.000000 sqlstrings-0.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-03-31 16:34:51.000000 sqlstrings-0.1.0/tests/test_csv_handling.py
+-rw-rw-rw-   0        0        0      163 2023-04-17 15:38:11.000000 sqlstrings-0.1.0/tests/test_main.py
+-rw-rw-rw-   0        0        0     2474 2023-04-17 15:39:16.000000 sqlstrings-0.1.0/tests/test_postgre.py
+-rw-rw-rw-   0        0        0     1986 2023-04-17 15:38:37.000000 sqlstrings-0.1.0/tests/test_transact.py
+-rw-rw-rw-   0        0        0     1634 2023-04-17 15:38:35.000000 sqlstrings-0.1.0/tests/test_value_handling.py
```

### Comparing `sqlstrings-0.0.9/LICENSE.txt` & `sqlstrings-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.9/PKG-INFO` & `sqlstrings-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlstrings
-Version: 0.0.9
+Version: 0.1.0
 Summary: Generates SQL query strings in multiple dialects.
 Home-page: https://github.com/alikellaway/sqlstrings
 Author: Ali Kellaway
 Author-email: ali.kellaway139@gmail.com
 License: MIT
 Keywords: sql strings generate query
 Classifier: Intended Audience :: Developers
```

### Comparing `sqlstrings-0.0.9/setup.py` & `sqlstrings-0.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup
 from pathlib import Path
 
 setup(
     name='sqlstrings',
-    version='0.0.9',    
+    version='0.1.0',    
     description='Generates SQL query strings in multiple dialects.',
     long_description= (Path(__file__).parent / "README.md").read_text(),
+    long_descriptio_content_type = 'text/markdown',
     keywords='sql strings generate query',
     url='https://github.com/alikellaway/sqlstrings',
     author='Ali Kellaway',
     author_email='ali.kellaway139@gmail.com',
     license='MIT',
     # package_dir={'':''},
     packages=['sqlstrings'],
```

### Comparing `sqlstrings-0.0.9/sqlstrings/csv_handling.py` & `sqlstrings-0.1.0/sqlstrings/csv_handling.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.9/sqlstrings/postgre.py` & `sqlstrings-0.1.0/sqlstrings/postgre.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.9/sqlstrings/transact.py` & `sqlstrings-0.1.0/sqlstrings/transact.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.9/sqlstrings/value_handling.py` & `sqlstrings-0.1.0/sqlstrings/value_handling.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.9/sqlstrings.egg-info/PKG-INFO` & `sqlstrings-0.1.0/sqlstrings.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlstrings
-Version: 0.0.9
+Version: 0.1.0
 Summary: Generates SQL query strings in multiple dialects.
 Home-page: https://github.com/alikellaway/sqlstrings
 Author: Ali Kellaway
 Author-email: ali.kellaway139@gmail.com
 License: MIT
 Keywords: sql strings generate query
 Classifier: Intended Audience :: Developers
```

### Comparing `sqlstrings-0.0.9/tests/test_postgre.py` & `sqlstrings-0.1.0/tests/test_postgre.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.9/tests/test_transact.py` & `sqlstrings-0.1.0/tests/test_transact.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.9/tests/test_value_handling.py` & `sqlstrings-0.1.0/tests/test_value_handling.py`

 * *Files identical despite different names*

