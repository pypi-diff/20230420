# Comparing `tmp/syncanysql-0.0.8.tar.gz` & `tmp/syncanysql-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanysql-0.0.8.tar", last modified: Thu Apr 20 08:48:07 2023, max compression
+gzip compressed data, was "syncanysql-0.0.9.tar", last modified: Thu Apr 20 10:16:18 2023, max compression
```

## Comparing `syncanysql-0.0.8.tar` & `syncanysql-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:48:07.617983 syncanysql-0.0.8/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.0.8/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3908 2023-04-20 08:48:07.619984 syncanysql-0.0.8/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2645 2023-03-29 06:12:04.000000 syncanysql-0.0.8/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-20 08:48:07.628422 syncanysql-0.0.8/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2011 2023-04-20 03:40:42.000000 syncanysql-0.0.8/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:48:06.334191 syncanysql-0.0.8/syncanysql/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8404 2023-03-29 07:10:45.000000 syncanysql-0.0.8/syncanysql/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:48:06.764651 syncanysql-0.0.8/syncanysql/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1050 2023-03-25 04:42:07.000000 syncanysql-0.0.8/syncanysql/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.0.8/syncanysql/calculaters/aggregate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1045 2023-04-20 03:00:29.000000 syncanysql-0.0.8/syncanysql/calculaters/mysql_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:48:07.078580 syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10157 2023-04-20 04:07:01.000000 syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/json_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6201 2023-04-20 03:05:35.000000 syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/number_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6413 2023-04-20 03:54:47.000000 syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/string_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)   119835 2023-04-20 03:19:47.000000 syncanysql-0.0.8/syncanysql/compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12011 2023-03-27 03:03:08.000000 syncanysql-0.0.8/syncanysql/config.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.0.8/syncanysql/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7245 2023-03-29 02:06:08.000000 syncanysql-0.0.8/syncanysql/executor.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3590 2023-03-25 04:39:43.000000 syncanysql-0.0.8/syncanysql/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.0.8/syncanysql/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7259 2023-04-19 08:39:44.000000 syncanysql-0.0.8/syncanysql/prompt.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:48:07.573555 syncanysql-0.0.8/syncanysql/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.0.8/syncanysql/taskers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.0.8/syncanysql/taskers/delete.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1513 2023-03-29 02:06:08.000000 syncanysql-0.0.8/syncanysql/taskers/execute.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1394 2023-03-29 02:07:07.000000 syncanysql-0.0.8/syncanysql/taskers/explain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3519 2023-03-29 02:07:07.000000 syncanysql-0.0.8/syncanysql/taskers/into.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    18357 2023-03-29 02:07:07.000000 syncanysql-0.0.8/syncanysql/taskers/query.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.0.8/syncanysql/taskers/set.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.0.8/syncanysql/taskers/show.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1173 2023-03-29 02:06:08.000000 syncanysql-0.0.8/syncanysql/taskers/use.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.0.8/syncanysql/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-04-20 02:31:24.000000 syncanysql-0.0.8/syncanysql/version.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:48:06.608222 syncanysql-0.0.8/syncanysql.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3908 2023-04-20 08:48:05.000000 syncanysql-0.0.8/syncanysql.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1119 2023-04-20 08:48:05.000000 syncanysql-0.0.8/syncanysql.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-20 08:48:05.000000 syncanysql-0.0.8/syncanysql.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-04-20 08:48:05.000000 syncanysql-0.0.8/syncanysql.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-02-25 12:53:08.000000 syncanysql-0.0.8/syncanysql.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-04-20 08:48:05.000000 syncanysql-0.0.8/syncanysql.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-04-20 08:48:05.000000 syncanysql-0.0.8/syncanysql.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 10:16:18.409983 syncanysql-0.0.9/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.0.9/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4234 2023-04-20 10:16:18.410984 syncanysql-0.0.9/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2955 2023-04-20 10:10:41.000000 syncanysql-0.0.9/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-20 10:16:18.420008 syncanysql-0.0.9/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2011 2023-04-20 10:04:48.000000 syncanysql-0.0.9/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 10:16:17.231680 syncanysql-0.0.9/syncanysql/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8404 2023-03-29 07:10:45.000000 syncanysql-0.0.9/syncanysql/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 10:16:17.686006 syncanysql-0.0.9/syncanysql/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1050 2023-03-25 04:42:07.000000 syncanysql-0.0.9/syncanysql/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.0.9/syncanysql/calculaters/aggregate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1045 2023-04-20 03:00:29.000000 syncanysql-0.0.9/syncanysql/calculaters/mysql_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 10:16:17.951983 syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10157 2023-04-20 04:07:01.000000 syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/json_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6201 2023-04-20 03:05:35.000000 syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/number_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6413 2023-04-20 03:54:47.000000 syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/string_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)   120732 2023-04-20 09:54:00.000000 syncanysql-0.0.9/syncanysql/compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12011 2023-03-27 03:03:08.000000 syncanysql-0.0.9/syncanysql/config.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.0.9/syncanysql/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7245 2023-03-29 02:06:08.000000 syncanysql-0.0.9/syncanysql/executor.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3590 2023-03-25 04:39:43.000000 syncanysql-0.0.9/syncanysql/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.0.9/syncanysql/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7259 2023-04-19 08:39:44.000000 syncanysql-0.0.9/syncanysql/prompt.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 10:16:18.367013 syncanysql-0.0.9/syncanysql/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.0.9/syncanysql/taskers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.0.9/syncanysql/taskers/delete.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1513 2023-03-29 02:06:08.000000 syncanysql-0.0.9/syncanysql/taskers/execute.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1394 2023-03-29 02:07:07.000000 syncanysql-0.0.9/syncanysql/taskers/explain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3519 2023-03-29 02:07:07.000000 syncanysql-0.0.9/syncanysql/taskers/into.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    18357 2023-03-29 02:07:07.000000 syncanysql-0.0.9/syncanysql/taskers/query.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.0.9/syncanysql/taskers/set.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.0.9/syncanysql/taskers/show.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1173 2023-03-29 02:06:08.000000 syncanysql-0.0.9/syncanysql/taskers/use.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.0.9/syncanysql/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-04-20 10:04:48.000000 syncanysql-0.0.9/syncanysql/version.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 10:16:17.518855 syncanysql-0.0.9/syncanysql.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4234 2023-04-20 10:16:16.000000 syncanysql-0.0.9/syncanysql.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1119 2023-04-20 10:16:16.000000 syncanysql-0.0.9/syncanysql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-20 10:16:16.000000 syncanysql-0.0.9/syncanysql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-04-20 10:16:16.000000 syncanysql-0.0.9/syncanysql.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-02-25 12:53:08.000000 syncanysql-0.0.9/syncanysql.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-04-20 10:16:16.000000 syncanysql-0.0.9/syncanysql.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-04-20 10:16:16.000000 syncanysql-0.0.9/syncanysql.egg-info/top_level.txt
```

### Comparing `syncanysql-0.0.8/LICENSE` & `syncanysql-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/PKG-INFO` & `syncanysql-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
+        [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
+        [![GitHub Repo stars](https://img.shields.io/github/stars/snower/syncany-sql?style=social)](https://github.com/snower/syncany-sql/stargazers)
         
         简单易用的SQL执行引擎。
         
         - 可在本地运行MySQL语法结构的SQL
         - 支持查询常用mysql、mongodb、postgresql、sqlserver、elasticsearch、influxdb、clickhouse、sqlite数据库及execl、csv、json和普通文本文件
         - 支持本地临时数据表逻辑做中间结果保存
         - 数据库数据加载使用简单条件过滤及IN条件查询
```

### Comparing `syncanysql-0.0.8/README.md` & `syncanysql-0.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Syncany-SQL
+[![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
+[![GitHub Repo stars](https://img.shields.io/github/stars/snower/syncany-sql?style=social)](https://github.com/snower/syncany-sql/stargazers)
 
 简单易用的SQL执行引擎。
 
 - 可在本地运行MySQL语法结构的SQL
 - 支持查询常用mysql、mongodb、postgresql、sqlserver、elasticsearch、influxdb、clickhouse、sqlite数据库及execl、csv、json和普通文本文件
 - 支持本地临时数据表逻辑做中间结果保存
 - 数据库数据加载使用简单条件过滤及IN条件查询
```

### Comparing `syncanysql-0.0.8/setup.py` & `syncanysql-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.0.8"
+version = "0.0.9"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
```

### Comparing `syncanysql-0.0.8/syncanysql/__init__.py` & `syncanysql-0.0.9/syncanysql/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/calculaters/__init__.py` & `syncanysql-0.0.9/syncanysql/calculaters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/calculaters/aggregate_calculater.py` & `syncanysql-0.0.9/syncanysql/calculaters/aggregate_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/calculaters/mysql_calculater.py` & `syncanysql-0.0.9/syncanysql/calculaters/mysql_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/datetime_funcs.py` & `syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/datetime_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/json_funcs.py` & `syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/json_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/number_funcs.py` & `syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/number_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/calculaters/mysql_funcs/string_funcs.py` & `syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/string_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/compiler.py` & `syncanysql-0.0.9/syncanysql/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 # 2023/2/8
 # create by: snower
 
 import os
 import copy
 import uuid
+
+import sqlglot.expressions
 from sqlglot import maybe_parse, ParseError
 from sqlglot import expressions as sqlglot_expressions
 from sqlglot.dialects import Dialect
 from sqlglot import tokens
 from .errors import SyncanySqlCompileException
 from .calculaters import is_mysql_func, find_aggregate_calculater, CalculaterUnknownException
 from .config import CONST_CONFIG_KEYS
@@ -87,16 +89,20 @@
                 return query_tasker
             if not isinstance(expression, sqlglot_expressions.Select):
                 raise SyncanySqlCompileException('unknown into, related sql "%s"' % self.to_sql(expression))
             return IntoTasker(query_tasker, self.compile_select_into(expression.args.get("into"), arguments))
         elif isinstance(expression, sqlglot_expressions.Command):
             if expression.args["this"].lower() == "explain" and self.is_const(expression.args["expression"], {}, arguments):
                 return ExplainTasker(self.compile(self.parse_const(expression.args["expression"], {}, arguments)["value"], arguments))
-            if expression.args["this"].lower() == "set" and self.is_const(expression.args["expression"], {}, arguments):
-                value = self.parse_const(expression.args["expression"], {}, arguments)["value"].split("=")
+            if expression.args["this"].lower() == "set" and (isinstance(expression.args["expression"], str)
+                                                             or self.is_const(expression.args["expression"], {}, arguments)):
+                if isinstance(expression.args["expression"], str):
+                    value = expression.args["expression"].split("=")
+                else:
+                    value = self.parse_const(expression.args["expression"], {}, arguments)["value"].split("=")
                 config = {"key": value[0].strip(), "value": "=".join(value[1:]).strip()}
                 return SetCommandTasker(config)
             if expression.args["this"].lower() == "execute" and self.is_const(expression.args["expression"], {}, arguments):
                 filename = self.parse_const(expression.args["expression"], {}, arguments)["value"]
                 if filename and filename[0] == '`':
                     filename = filename[1:-1]
                 if filename in self.mapping:
@@ -105,14 +111,20 @@
             if expression.args["this"].lower() == "show" and self.is_const(expression.args["expression"], {}, arguments):
                 return ShowCommandTasker({"key": self.parse_const(expression.args["expression"], {}, arguments)["value"]})
         elif isinstance(expression, sqlglot_expressions.Use):
             use_info = expression.args["this"].args["this"].name
             if use_info in self.mapping:
                 use_info = self.mapping[use_info]
             return UseCommandTasker({"use": use_info})
+        elif isinstance(expression, sqlglot.expressions.Set) and expression.args.get("expressions") and len(expression.args.get("expressions")) == 1:
+            set_item_expression = expression.args.get("expressions")[0]
+            if isinstance(set_item_expression, sqlglot_expressions.SetItem) and isinstance(set_item_expression.args["this"], sqlglot_expressions.EQ):
+                value = str(set_item_expression.args["this"]).split("=")
+                config = {"key": value[0].strip(), "value": "=".join(value[1:]).strip()}
+                return SetCommandTasker(config)
         raise SyncanySqlCompileException('unknown sql "%s"' % self.to_sql(expression))
 
     def compile_delete(self, expression, arguments):
         config = copy.deepcopy(self.config)
         config.update({
             "input": "&.--.__subquery_null_" + str(uuid.uuid1().int) + "::id",
             "output": "&.-.&1::id",
```

### Comparing `syncanysql-0.0.8/syncanysql/config.py` & `syncanysql-0.0.9/syncanysql/config.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/executor.py` & `syncanysql-0.0.9/syncanysql/executor.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/main.py` & `syncanysql-0.0.9/syncanysql/main.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/parser.py` & `syncanysql-0.0.9/syncanysql/parser.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/prompt.py` & `syncanysql-0.0.9/syncanysql/prompt.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/taskers/delete.py` & `syncanysql-0.0.9/syncanysql/taskers/delete.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/taskers/execute.py` & `syncanysql-0.0.9/syncanysql/taskers/execute.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/taskers/explain.py` & `syncanysql-0.0.9/syncanysql/taskers/explain.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/taskers/into.py` & `syncanysql-0.0.9/syncanysql/taskers/into.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/taskers/query.py` & `syncanysql-0.0.9/syncanysql/taskers/query.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/taskers/set.py` & `syncanysql-0.0.9/syncanysql/taskers/set.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/taskers/show.py` & `syncanysql-0.0.9/syncanysql/taskers/show.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/taskers/use.py` & `syncanysql-0.0.9/syncanysql/taskers/use.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql/utils.py` & `syncanysql-0.0.9/syncanysql/utils.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.8/syncanysql.egg-info/PKG-INFO` & `syncanysql-0.0.9/syncanysql.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
+        [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
+        [![GitHub Repo stars](https://img.shields.io/github/stars/snower/syncany-sql?style=social)](https://github.com/snower/syncany-sql/stargazers)
         
         简单易用的SQL执行引擎。
         
         - 可在本地运行MySQL语法结构的SQL
         - 支持查询常用mysql、mongodb、postgresql、sqlserver、elasticsearch、influxdb、clickhouse、sqlite数据库及execl、csv、json和普通文本文件
         - 支持本地临时数据表逻辑做中间结果保存
         - 数据库数据加载使用简单条件过滤及IN条件查询
```

### Comparing `syncanysql-0.0.8/syncanysql.egg-info/SOURCES.txt` & `syncanysql-0.0.9/syncanysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

