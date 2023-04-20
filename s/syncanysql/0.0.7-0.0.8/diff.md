# Comparing `tmp/syncanysql-0.0.7.tar.gz` & `tmp/syncanysql-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanysql-0.0.7.tar", last modified: Wed Apr 19 09:46:19 2023, max compression
+gzip compressed data, was "syncanysql-0.0.8.tar", last modified: Thu Apr 20 08:48:07 2023, max compression
```

## Comparing `syncanysql-0.0.7.tar` & `syncanysql-0.0.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:46:19.974063 syncanysql-0.0.7/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.0.7/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3908 2023-04-19 09:46:19.976065 syncanysql-0.0.7/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2645 2023-03-29 06:12:04.000000 syncanysql-0.0.7/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-19 09:46:19.985341 syncanysql-0.0.7/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2011 2023-04-19 08:35:52.000000 syncanysql-0.0.7/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:46:18.607060 syncanysql-0.0.7/syncanysql/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8404 2023-03-29 07:10:45.000000 syncanysql-0.0.7/syncanysql/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:46:19.057426 syncanysql-0.0.7/syncanysql/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1050 2023-03-25 04:42:07.000000 syncanysql-0.0.7/syncanysql/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.0.7/syncanysql/calculaters/aggregate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      975 2023-04-19 08:11:25.000000 syncanysql-0.0.7/syncanysql/calculaters/mysql_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:46:19.392873 syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8741 2023-04-19 07:56:30.000000 syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5980 2023-04-19 07:56:30.000000 syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/json_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5340 2023-04-19 08:22:16.000000 syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/number_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4221 2023-04-19 08:31:29.000000 syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/string_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)   119772 2023-04-19 08:03:18.000000 syncanysql-0.0.7/syncanysql/compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12011 2023-03-27 03:03:08.000000 syncanysql-0.0.7/syncanysql/config.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.0.7/syncanysql/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7245 2023-03-29 02:06:08.000000 syncanysql-0.0.7/syncanysql/executor.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3590 2023-03-25 04:39:43.000000 syncanysql-0.0.7/syncanysql/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.0.7/syncanysql/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7259 2023-04-19 08:39:44.000000 syncanysql-0.0.7/syncanysql/prompt.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:46:19.925892 syncanysql-0.0.7/syncanysql/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.0.7/syncanysql/taskers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.0.7/syncanysql/taskers/delete.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1513 2023-03-29 02:06:08.000000 syncanysql-0.0.7/syncanysql/taskers/execute.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1394 2023-03-29 02:07:07.000000 syncanysql-0.0.7/syncanysql/taskers/explain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3519 2023-03-29 02:07:07.000000 syncanysql-0.0.7/syncanysql/taskers/into.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    18357 2023-03-29 02:07:07.000000 syncanysql-0.0.7/syncanysql/taskers/query.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.0.7/syncanysql/taskers/set.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.0.7/syncanysql/taskers/show.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1173 2023-03-29 02:06:08.000000 syncanysql-0.0.7/syncanysql/taskers/use.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.0.7/syncanysql/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-04-19 08:35:52.000000 syncanysql-0.0.7/syncanysql/version.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:46:18.891060 syncanysql-0.0.7/syncanysql.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3908 2023-04-19 09:46:17.000000 syncanysql-0.0.7/syncanysql.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1119 2023-04-19 09:46:17.000000 syncanysql-0.0.7/syncanysql.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-19 09:46:17.000000 syncanysql-0.0.7/syncanysql.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-04-19 09:46:17.000000 syncanysql-0.0.7/syncanysql.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-02-25 12:53:08.000000 syncanysql-0.0.7/syncanysql.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-04-19 09:46:17.000000 syncanysql-0.0.7/syncanysql.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-04-19 09:46:17.000000 syncanysql-0.0.7/syncanysql.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:48:07.617983 syncanysql-0.0.8/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.0.8/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3908 2023-04-20 08:48:07.619984 syncanysql-0.0.8/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2645 2023-03-29 06:12:04.000000 syncanysql-0.0.8/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-20 08:48:07.628422 syncanysql-0.0.8/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2011 2023-04-20 03:40:42.000000 syncanysql-0.0.8/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:48:06.334191 syncanysql-0.0.8/syncanysql/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8404 2023-03-29 07:10:45.000000 syncanysql-0.0.8/syncanysql/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:48:06.764651 syncanysql-0.0.8/syncanysql/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1050 2023-03-25 04:42:07.000000 syncanysql-0.0.8/syncanysql/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.0.8/syncanysql/calculaters/aggregate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1045 2023-04-20 03:00:29.000000 syncanysql-0.0.8/syncanysql/calculaters/mysql_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:48:07.078580 syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10157 2023-04-20 04:07:01.000000 syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/json_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6201 2023-04-20 03:05:35.000000 syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/number_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6413 2023-04-20 03:54:47.000000 syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/string_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)   119835 2023-04-20 03:19:47.000000 syncanysql-0.0.8/syncanysql/compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12011 2023-03-27 03:03:08.000000 syncanysql-0.0.8/syncanysql/config.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.0.8/syncanysql/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7245 2023-03-29 02:06:08.000000 syncanysql-0.0.8/syncanysql/executor.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3590 2023-03-25 04:39:43.000000 syncanysql-0.0.8/syncanysql/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.0.8/syncanysql/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7259 2023-04-19 08:39:44.000000 syncanysql-0.0.8/syncanysql/prompt.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:48:07.573555 syncanysql-0.0.8/syncanysql/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.0.8/syncanysql/taskers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.0.8/syncanysql/taskers/delete.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1513 2023-03-29 02:06:08.000000 syncanysql-0.0.8/syncanysql/taskers/execute.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1394 2023-03-29 02:07:07.000000 syncanysql-0.0.8/syncanysql/taskers/explain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3519 2023-03-29 02:07:07.000000 syncanysql-0.0.8/syncanysql/taskers/into.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    18357 2023-03-29 02:07:07.000000 syncanysql-0.0.8/syncanysql/taskers/query.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.0.8/syncanysql/taskers/set.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.0.8/syncanysql/taskers/show.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1173 2023-03-29 02:06:08.000000 syncanysql-0.0.8/syncanysql/taskers/use.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.0.8/syncanysql/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-04-20 02:31:24.000000 syncanysql-0.0.8/syncanysql/version.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:48:06.608222 syncanysql-0.0.8/syncanysql.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3908 2023-04-20 08:48:05.000000 syncanysql-0.0.8/syncanysql.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1119 2023-04-20 08:48:05.000000 syncanysql-0.0.8/syncanysql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-20 08:48:05.000000 syncanysql-0.0.8/syncanysql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-04-20 08:48:05.000000 syncanysql-0.0.8/syncanysql.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-02-25 12:53:08.000000 syncanysql-0.0.8/syncanysql.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-04-20 08:48:05.000000 syncanysql-0.0.8/syncanysql.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-04-20 08:48:05.000000 syncanysql-0.0.8/syncanysql.egg-info/top_level.txt
```

### Comparing `syncanysql-0.0.7/LICENSE` & `syncanysql-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/PKG-INFO` & `syncanysql-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
```

### Comparing `syncanysql-0.0.7/README.md` & `syncanysql-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/setup.py` & `syncanysql-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.0.7"
+version = "0.0.8"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -34,15 +34,15 @@
     author_email='sujian199@gmail.com',
     license='MIT',
     packages=find_packages(),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
         "sqlglot>=10.6.2",
-        "syncany>=0.2.4",
+        "syncany>=0.2.5",
         'Pygments>=2.14.0',
         'Pygments>=2.14.0',
         'prompt-toolkit>=3.0.36',
         "rich>=9.11.1",
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
```

### Comparing `syncanysql-0.0.7/syncanysql/__init__.py` & `syncanysql-0.0.8/syncanysql/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/calculaters/__init__.py` & `syncanysql-0.0.8/syncanysql/calculaters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/calculaters/aggregate_calculater.py` & `syncanysql-0.0.8/syncanysql/calculaters/aggregate_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/calculaters/mysql_calculater.py` & `syncanysql-0.0.8/syncanysql/calculaters/mysql_calculater.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,11 +20,13 @@
         try:
             if len(args) == 1 and isinstance(args[0], list) and args[0] and isinstance(args[0][0], dict):
                 try:
                     self.func(*tuple(args[0]))
                 except TypeError:
                     pass
             return self.func(*args)
+        except (ValueError, KeyError) as e:
+            return None
         except Exception as e:
             get_logger().warning("mysql calculater execute %s(%s) error: %s\n%s", self.name[7:], args, e,
                                  traceback.format_exc())
             return None
```

### Comparing `syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/json_funcs.py` & `syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/json_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         else:
             json_path_keys.append(json_path)
         return json_path_keys
 
 
 def get_json_path_value(json_data, json_path):
     if json_data is None:
-        return None
+        raise ValueError('value is None')
     if json_path and json_path[:2] == "$.":
         json_path = json_path[2:]
     elif json_path and json_path[0] == '$':
         json_path = json_path[1:]
 
     def get_value(json_data, json_path_keys):
         for i in range(len(json_path_keys)):
```

### Comparing `syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/string_funcs.py` & `syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/string_funcs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,190 +1,285 @@
 # -*- coding: utf-8 -*-
 # 2023/3/2
 # create by: snower
 
+import datetime
 import socket
 import base64
 import binascii
 
 def ensure_str(x):
     if isinstance(x, str):
         return x
     if x is None:
-        return ""
+        raise ValueError('value is None')
+    if not x:
+        return '0'
+    if x is True:
+        return '1'
     if isinstance(x, bytes):
         return x.decode("utf-8")
+    if isinstance(x, datetime.date):
+        if isinstance(x, datetime.datetime):
+            return x.strftime("%Y-%m-%d %H:%M:%S")
+        return x.strftime("%Y-%m-%d")
+    if isinstance(x, datetime.time):
+        return x.strftime("%H:%M:%S")
     return str(x)
 
 def mysql_bin(x):
+    if isinstance(x, (int, float)):
+        return bin(int(x))
+    if x is None:
+        return None
+    if x is True:
+        return bin(1)
+    if not x:
+        return bin(0)
     return bin(x)
 
 def mysql_hex(x):
     if isinstance(x, (int, float)):
         return hex(int(x))
+    if x is None:
+        return None
+    if x is True:
+        return hex(1)
+    if not x:
+        return hex(0)
     return binascii.b2a_hex(x.encode("utf-8")).decode("utf-8")
 
 def mysql_unhex(x):
-    return binascii.a2b_hex(x)
+    if x is None:
+        return None
+    return binascii.a2b_hex(ensure_str(x))
 
 def mysql_oct(x):
+    if x is None:
+        return None
     return oct(x)[2:]
 
 def mysql_ord(x):
-    return ord(x)
+    if x is None:
+        return None
+    return ord(ensure_str(x))
 
 def mysql_ascii(s):
-    return sum([ord(c) for c in s])
+    if s is None:
+        return None
+    return sum([ord(c) for c in ensure_str(s)])
 
 def mysql_char(*args):
     return "".join([chr(arg) for arg in args])
 
 def mysql_bit_length(s):
+    if s is None:
+        return None
     return len(s.encode("utf-8")) * 8
 
 def mysql_length(s):
+    if s is None:
+        return None
     return len(s.encode("utf-8"))
 
 def mysql_char_length(s):
-    return len(s)
+    if s is None:
+        return None
+    return len(ensure_str(s))
 
 def mysql_character_length(s):
-    return len(s)
+    if s is None:
+        return None
+    return len(ensure_str(s))
 
 def mysql_concat(*args):
     return "".join(ensure_str(arg) for arg in args)
 
 def mysql_concat_ws(sep, *args):
     return sep.join(ensure_str(arg) for arg in args)
 
 def mysql_insert(s1, x, l, s2):
     s1, s2 = ensure_str(s1), ensure_str(s2)
     return s1[: x - 1] + s2 + s1[x + l - 1:]
 
 def mysql_lower(s):
+    if s is None:
+        return None
     return ensure_str(s).lower()
 
 def mysql_upper(s):
+    if s is None:
+        return None
     return ensure_str(s).upper()
 
 def mysql_ucase(s):
+    if s is None:
+        return None
     return ensure_str(s).upper()
 
 def mysql_left(s, x):
+    if s is None:
+        return None
     return ensure_str(s)[:x]
 
 def mysql_right(s, x):
+    if s is None:
+        return None
     return ensure_str(s)[-x:]
 
 def mysql_trim(s):
+    if s is None:
+        return None
     return ensure_str(s).strip()
 
 def mysql_elt(n, *args):
     return args[n - 1] if n < len(args) else None
 
 def mysql_field(s, *args):
+    if s is None:
+        return None
     try:
         return args.index(s) + 1
     except ValueError:
         return 0
 
 def mysql_find_in_set(s, ss):
+    if s is None:
+        return None
     try:
         return ensure_str(ss).split(",").index(s) + 1
     except ValueError:
         return 0
 
 def mysql_replace(s, s1, s2):
+    if s is None:
+        return None
     return ensure_str(s).replace(s1, s2)
 
 def mysql_substring(s, n, l=None):
+    if s is None:
+        return None
     s = ensure_str(s)
     if isinstance(l, int):
         return s[n - 1: n + l - 1]
     return s[n - 1:]
 
 def mysql_substr(s, n, l=None):
+    if s is None:
+        return None
     s = ensure_str(s)
     if isinstance(l, int):
         return s[n - 1: n + l - 1]
     return s[n - 1:]
 
 def mysql_substring_index(s, d, c):
+    if s is None:
+        return None
     s, d = ensure_str(s), ensure_str(d)
     if c < 0:
         return d.join(s.split(d)[-c:])
     return d.join(s.split(d)[:c])
 
 def mysql_repeat(s, c):
+    if s is None:
+        return None
     return ensure_str(s) * c
 
 def mysql_reverse(s):
+    if s is None:
+        return None
     return ensure_str(s)[::-1]
 
 def mysql_strcmp(s1, s2):
+    if s1 is None or s2 is None:
+        return None
     s1, s2 = ensure_str(s1), ensure_str(s2)
     return 0 if s1 == s2 else (-1 if s1 < s2 else 1)
 
 def mysql_startswith(s1, s2):
+    if s1 is None or s2 is None:
+        return None
     s1, s2 = ensure_str(s1), ensure_str(s2)
     return s1.startswith(s2)
 
 def mysql_endswith(s1, s2):
+    if s1 is None or s2 is None:
+        return None
     s1, s2 = ensure_str(s1), ensure_str(s2)
     return s1.endswith(s2)
 
 def mysql_contains(s1, s2):
+    if s1 is None or s2 is None:
+        return None
     try:
         return s2 in s1
     except:
         s1, s2 = ensure_str(s1), ensure_str(s2)
         return s2 in s1
 
 def mysql_crc32(s):
+    if s is None:
+        return None
     import zlib
     return zlib.crc32(s)
 
 def mysql_from_base64(s):
+    if s is None:
+        return None
     return base64.b64decode(s.encode("utf-8")).decode("utf-8")
 
 def mysql_to_base64(s):
+    if s is None:
+        return None
     return base64.b64encode(s.encode("utf-8")).decode("utf-8")
 
 def mysql_inet4_aton(s):
+    if s is None:
+        return None
     try:
         return binascii.b2a_hex(socket.inet_aton(s)).decode("utf-8")
     except:
         return None
 
 def mysql_inet4_ntoa(b):
+    if b is None:
+        return None
     try:
         return socket.inet_ntoa(b)
     except:
         return None
 
 def mysql_is_ipv4(s):
+    if s is None:
+        return None
     try:
         socket.inet_aton(s)
         return 1
     except:
         return 0
 
 def mysql_inet6_aton(s):
+    if s is None:
+        return None
     try:
         return binascii.b2a_hex(socket.inet_pton(socket.AF_INET6, s)).decode("utf-8")
     except:
         return None
 
 def mysql_inet6_ntoa(b):
+    if b is None:
+        return None
     try:
         return socket.inet_ntop(socket.AF_INET6, b)
     except:
         return None
 
 def mysql_is_ipv6(s):
+    if s is None:
+        return None
     try:
         socket.inet_pton(socket.AF_INET6, s)
         return 1
     except:
         return 0
```

### Comparing `syncanysql-0.0.7/syncanysql/compiler.py` & `syncanysql-0.0.8/syncanysql/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -979,15 +979,15 @@
                         column.append(self.compile_const(arg_expression, config, arguments,
                                                          self.parse_const(arg_expression, config, arguments)))
                     else:
                         column.append(self.compile_calculate(arg_expression, config, arguments, primary_table, 
                                                              column_join_tables, join_index))
                 return column
 
-            if is_mysql_func(calculater_name):
+            if calculater_name not in ("add", "sub", "mul", "div", "mod") and is_mysql_func(calculater_name):
                 column = ["@mysql::" + calculater_name]
             else:
                 if calculater_name[:8] == "convert_":
                     column = ["@" + "::".join(calculater_name.split("$")) + "|" + calculater_name[8:]]
                 else:
                     column = ["@" + "::".join(calculater_name.split("$"))]
             for arg_expression in expression.args.get("expressions", []):
```

### Comparing `syncanysql-0.0.7/syncanysql/config.py` & `syncanysql-0.0.8/syncanysql/config.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/executor.py` & `syncanysql-0.0.8/syncanysql/executor.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/main.py` & `syncanysql-0.0.8/syncanysql/main.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/parser.py` & `syncanysql-0.0.8/syncanysql/parser.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/prompt.py` & `syncanysql-0.0.8/syncanysql/prompt.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/taskers/delete.py` & `syncanysql-0.0.8/syncanysql/taskers/delete.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/taskers/execute.py` & `syncanysql-0.0.8/syncanysql/taskers/execute.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/taskers/explain.py` & `syncanysql-0.0.8/syncanysql/taskers/explain.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/taskers/into.py` & `syncanysql-0.0.8/syncanysql/taskers/into.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/taskers/query.py` & `syncanysql-0.0.8/syncanysql/taskers/query.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/taskers/set.py` & `syncanysql-0.0.8/syncanysql/taskers/set.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/taskers/show.py` & `syncanysql-0.0.8/syncanysql/taskers/show.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/taskers/use.py` & `syncanysql-0.0.8/syncanysql/taskers/use.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql/utils.py` & `syncanysql-0.0.8/syncanysql/utils.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.7/syncanysql.egg-info/PKG-INFO` & `syncanysql-0.0.8/syncanysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
```

### Comparing `syncanysql-0.0.7/syncanysql.egg-info/SOURCES.txt` & `syncanysql-0.0.8/syncanysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

