# Comparing `tmp/polyapi-5.7.0.3.tar.gz` & `tmp/polyapi-5.7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi-5.7.0.3.tar", last modified: Fri Mar 10 14:13:35 2023, max compression
+gzip compressed data, was "polyapi-5.7.0.4.tar", last modified: Thu Apr 20 09:00:46 2023, max compression
```

## Comparing `polyapi-5.7.0.3.tar` & `polyapi-5.7.0.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-03-10 14:13:35.052460 polyapi-5.7.0.3/
--rw-r--r--   0 artem     (1000) artem     (1000)     1061 2023-01-26 16:04:08.000000 polyapi-5.7.0.3/LICENSE.txt
--rw-r--r--   0 artem     (1000) artem     (1000)     1547 2023-03-10 14:13:35.052460 polyapi-5.7.0.3/PKG-INFO
--rw-r--r--   0 artem     (1000) artem     (1000)     1048 2023-01-26 16:04:08.000000 polyapi-5.7.0.3/README.txt
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-03-10 14:13:35.042460 polyapi-5.7.0.3/polyapi.egg-info/
--rw-r--r--   0 artem     (1000) artem     (1000)     1547 2023-03-10 14:13:35.000000 polyapi-5.7.0.3/polyapi.egg-info/PKG-INFO
--rw-r--r--   0 artem     (1000) artem     (1000)     1547 2023-03-10 14:13:35.000000 polyapi-5.7.0.3/polyapi.egg-info/SOURCES.txt
--rw-r--r--   0 artem     (1000) artem     (1000)        1 2023-03-10 14:13:35.000000 polyapi-5.7.0.3/polyapi.egg-info/dependency_links.txt
--rw-r--r--   0 artem     (1000) artem     (1000)       27 2023-03-10 14:13:35.000000 polyapi-5.7.0.3/polyapi.egg-info/requires.txt
--rw-r--r--   0 artem     (1000) artem     (1000)       11 2023-03-10 14:13:35.000000 polyapi-5.7.0.3/polyapi.egg-info/top_level.txt
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-03-10 14:13:35.042460 polyapi-5.7.0.3/polymatica/
--rw-r--r--   0 artem     (1000) artem     (1000)      153 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/__init__.py
--rw-r--r--   0 artem     (1000) artem     (1000)     8939 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/authorization.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3686 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/business_logic_doc.py
--rw-r--r--   0 artem     (1000) artem     (1000)   409392 2023-03-10 14:11:33.000000 polyapi-5.7.0.3/polymatica/business_scenarios.py
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-03-10 14:13:35.042460 polyapi-5.7.0.3/polymatica/commands/
--rw-r--r--   0 artem     (1000) artem     (1000)      298 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/commands/__init__.py
--rw-r--r--   0 artem     (1000) artem     (1000)     4098 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/commands/base_command.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3118 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/commands/olap_module.py
--rw-r--r--   0 artem     (1000) artem     (1000)     1884 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/commands/other_modules.py
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-03-10 14:13:35.042460 polyapi-5.7.0.3/polymatica/common/
--rw-r--r--   0 artem     (1000) artem     (1000)      353 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/common/__init__.py
--rw-r--r--   0 artem     (1000) artem     (1000)     4821 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/common/consts.py
--rw-r--r--   0 artem     (1000) artem     (1000)    18721 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/common/helper_funcs.py
--rw-r--r--   0 artem     (1000) artem     (1000)    37161 2023-03-10 14:11:33.000000 polyapi-5.7.0.3/polymatica/error_handler.py
--rw-r--r--   0 artem     (1000) artem     (1000)     4765 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/exceptions.py
--rw-r--r--   0 artem     (1000) artem     (1000)    17499 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/executor.py
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-03-10 14:13:35.042460 polyapi-5.7.0.3/polymatica/graph/
--rw-r--r--   0 artem     (1000) artem     (1000)      136 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/__init__.py
--rw-r--r--   0 artem     (1000) artem     (1000)    21693 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/base_graph.py
--rw-r--r--   0 artem     (1000) artem     (1000)    21384 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/graph_interface.py
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-03-10 14:13:35.052460 polyapi-5.7.0.3/polymatica/graph/types/
--rw-r--r--   0 artem     (1000) artem     (1000)      668 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/__init__.py
--rw-r--r--   0 artem     (1000) artem     (1000)     2485 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/areas.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3631 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/balls.py
--rw-r--r--   0 artem     (1000) artem     (1000)     2498 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/chord.py
--rw-r--r--   0 artem     (1000) artem     (1000)     4067 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/circles.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3652 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/circles_series.py
--rw-r--r--   0 artem     (1000) artem     (1000)     4641 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/corridors.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3132 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/cumulative_areas.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3518 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/cumulative_cylinders.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3603 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/cylinders.py
--rw-r--r--   0 artem     (1000) artem     (1000)     8064 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/graph.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3278 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/lines.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3972 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/pies.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3966 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/point.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3897 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/point_series.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3579 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/pools.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3403 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/pools_3d.py
--rw-r--r--   0 artem     (1000) artem     (1000)     2242 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/radar.py
--rw-r--r--   0 artem     (1000) artem     (1000)     1903 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/sankey.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3605 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/graph/types/surface.py
--rw-r--r--   0 artem     (1000) artem     (1000)    20352 2023-03-10 14:11:33.000000 polyapi-5.7.0.3/polymatica/helper.py
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-03-10 14:13:35.052460 polyapi-5.7.0.3/polymatica/versions/
--rw-r--r--   0 artem     (1000) artem     (1000)      260 2023-03-07 11:34:42.000000 polyapi-5.7.0.3/polymatica/versions/__init__.py
--rw-r--r--   0 artem     (1000) artem     (1000)    10603 2023-03-10 14:11:33.000000 polyapi-5.7.0.3/polymatica/versions/polymatica_57.py
--rw-r--r--   0 artem     (1000) artem     (1000)     1600 2023-03-10 14:11:33.000000 polyapi-5.7.0.3/polymatica/versions/versions_redirect.py
--rw-r--r--   0 artem     (1000) artem     (1000)       38 2023-03-10 14:13:35.052460 polyapi-5.7.0.3/setup.cfg
--rw-r--r--   0 artem     (1000) artem     (1000)      759 2023-03-10 14:11:33.000000 polyapi-5.7.0.3/setup.py
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.262089 polyapi-5.7.0.4/
+-rw-r--r--   0 artem     (1000) artem     (1000)     1061 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/LICENSE.txt
+-rw-r--r--   0 artem     (1000) artem     (1000)     1547 2023-04-20 09:00:46.262089 polyapi-5.7.0.4/PKG-INFO
+-rw-r--r--   0 artem     (1000) artem     (1000)     1048 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/README.txt
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.252089 polyapi-5.7.0.4/polyapi.egg-info/
+-rw-r--r--   0 artem     (1000) artem     (1000)     1547 2023-04-20 09:00:46.000000 polyapi-5.7.0.4/polyapi.egg-info/PKG-INFO
+-rw-r--r--   0 artem     (1000) artem     (1000)     1547 2023-04-20 09:00:46.000000 polyapi-5.7.0.4/polyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 artem     (1000) artem     (1000)        1 2023-04-20 09:00:46.000000 polyapi-5.7.0.4/polyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 artem     (1000) artem     (1000)       27 2023-04-20 09:00:46.000000 polyapi-5.7.0.4/polyapi.egg-info/requires.txt
+-rw-r--r--   0 artem     (1000) artem     (1000)       11 2023-04-20 09:00:46.000000 polyapi-5.7.0.4/polyapi.egg-info/top_level.txt
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.252089 polyapi-5.7.0.4/polymatica/
+-rw-r--r--   0 artem     (1000) artem     (1000)      153 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/__init__.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     8939 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/authorization.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3686 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/business_logic_doc.py
+-rw-r--r--   0 artem     (1000) artem     (1000)   411436 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/business_scenarios.py
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.252089 polyapi-5.7.0.4/polymatica/commands/
+-rw-r--r--   0 artem     (1000) artem     (1000)      298 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/commands/__init__.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     4098 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/commands/base_command.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3118 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/commands/olap_module.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     1884 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/commands/other_modules.py
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.252089 polyapi-5.7.0.4/polymatica/common/
+-rw-r--r--   0 artem     (1000) artem     (1000)      353 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/common/__init__.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     4821 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/common/consts.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    18721 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/common/helper_funcs.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    37161 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/error_handler.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     4765 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/exceptions.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    17499 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/executor.py
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.252089 polyapi-5.7.0.4/polymatica/graph/
+-rw-r--r--   0 artem     (1000) artem     (1000)      136 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/__init__.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    21693 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/base_graph.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    21384 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/graph_interface.py
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.262089 polyapi-5.7.0.4/polymatica/graph/types/
+-rw-r--r--   0 artem     (1000) artem     (1000)      668 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/__init__.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     2485 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/areas.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3631 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/balls.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     2498 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/chord.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     4067 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/circles.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3652 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/circles_series.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     4641 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/corridors.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3132 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/cumulative_areas.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3518 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/cumulative_cylinders.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3603 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/cylinders.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     8064 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/graph.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3278 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/lines.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3972 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/pies.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3966 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/point.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3897 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/point_series.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3579 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/pools.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3403 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/pools_3d.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     2242 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/radar.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     1903 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/sankey.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3605 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/surface.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    20352 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/helper.py
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.262089 polyapi-5.7.0.4/polymatica/versions/
+-rw-r--r--   0 artem     (1000) artem     (1000)      260 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/versions/__init__.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    10603 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/versions/polymatica_57.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     1600 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/versions/versions_redirect.py
+-rw-r--r--   0 artem     (1000) artem     (1000)       38 2023-04-20 09:00:46.262089 polyapi-5.7.0.4/setup.cfg
+-rw-r--r--   0 artem     (1000) artem     (1000)      759 2023-04-20 08:57:01.000000 polyapi-5.7.0.4/setup.py
```

### Comparing `polyapi-5.7.0.3/LICENSE.txt` & `polyapi-5.7.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/PKG-INFO` & `polyapi-5.7.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi
-Version: 5.7.0.3
+Version: 5.7.0.4
 Summary: Wrapper for Polymatica API
 Home-page: https://www.polymatica.ru
 Author: Polymatica Rus LLC
 Author-email: development@polymatica.com
 License: MIT
 Keywords: polymatica
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `polyapi-5.7.0.3/README.txt` & `polyapi-5.7.0.4/README.txt`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polyapi.egg-info/PKG-INFO` & `polyapi-5.7.0.4/polyapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi
-Version: 5.7.0.3
+Version: 5.7.0.4
 Summary: Wrapper for Polymatica API
 Home-page: https://www.polymatica.ru
 Author: Polymatica Rus LLC
 Author-email: development@polymatica.com
 License: MIT
 Keywords: polymatica
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `polyapi-5.7.0.3/polyapi.egg-info/SOURCES.txt` & `polyapi-5.7.0.4/polyapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/authorization.py` & `polyapi-5.7.0.4/polymatica/authorization.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/business_logic_doc.py` & `polyapi-5.7.0.4/polymatica/business_logic_doc.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/business_scenarios.py` & `polyapi-5.7.0.4/polymatica/business_scenarios.py`

 * *Files 0% similar despite different names*

```diff
@@ -1825,15 +1825,16 @@
             self.execute_manager_command(
                 command_name="user_iface", state="save_settings", module_id=self.authorization_uuid, settings=settings)
             if self.multisphere_module_id:
                 self.update_total_row()
             self.func_name = 'run_scenario'
 
     @timing
-    def run_scenario(self, scenario_id: str = None, scenario_name: str = None, scenario_path: str = None, timeout: int = None):
+    def run_scenario(self, scenario_id: str = None, scenario_name: str = None, scenario_path: str = None,
+                     timeout: int = None):
         """
         Запустить сценарий и дождаться его загрузки. В параметрах метода обязательно нужно указать либо идентификатор
         сценария, либо его название. И то, и то указывать не обязательно. Ничего не возвращает.
         Если по каким-то причинам невозможно дождаться загрузки выбранного сценария (не отвечает сервер Полиматики или
         сервер вернул невалидный статус), то будет сгенерирована ошибка.
         :param scenario_id: (str) идентификатор (uuid) сценария (необязательное значение, если задано название).
         :param scenario_name: (str) название сценария (необязательное значение, если задан идентификатор).
@@ -5822,14 +5823,47 @@
             return self._raise_exception(PolymaticaException, 'Active OLAP-module not found!', with_traceback=False)
         # суть метода: сначала меняем режим отображения тоталов, а затем меняем ещё раз
         # после второго вызова режим отображения вернётся в исходное значение, и мы сможем получить это самое значение
         self.change_total_mode()
         res = self.change_total_mode()
         return self.h.parse_result(res, 'show_inter_total')
 
+    @timing
+    def request_to_api_v2(self, url: str, method: str, headers: dict, cookies=None, data=None, json: dict = None):
+        if cookies is None:
+            cookies = {'session': self.session_id}
+
+        return requests.request(method=method, url=url, headers=headers, cookies=cookies, data=data, json=json)
+
+    @timing
+    def switch_session(self, new_owner_uuid: str) -> int:
+        """
+        Переключить владельца сессии.
+        :param new_owner_uuid: (str) UUID_4 - идентификатор пользователя, который должен стать владельцем текущей сессии
+        :return: (int) статус код:
+            Статусы ответа:
+            204 No Content - успешно.
+            401 Unauthorized - запрос от неавторизованного пользователя;
+            400 Bad Request - пустое тело запроса; content type не "application/json"; не было запрошено никаких
+                изменений, например, при передаче пустого Json-объекта в теле запроса; тип данных в полях тела
+                запроса не соответствует ожидаемому;
+            403 Forbidden - текущий пользователь не имеет роли администратора системы;
+            404 Not Found - пользователь с идентификатором new_owner не найден;
+            500 Internal server error - что-то пошло не так на стороне сервера.
+        """
+        url = self.base_url + "api/v2/sessions/current"
+        data = {"new_owner": new_owner_uuid}
+        headers = {
+            'Content-Type': 'application/json', 'Accept': '*/*',
+        }
+
+        response = self.request_to_api_v2(url=url, method="PATCH", headers=headers, json=data)
+
+        return response.status_code
+
 
 class GetDataChunk:
     """ Класс для получения данных чанками """
 
     def __init__(self, sc: BusinessLogic):
         """
         Инициализация класса GetDataChunk
```

### Comparing `polyapi-5.7.0.3/polymatica/commands/base_command.py` & `polyapi-5.7.0.4/polymatica/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/commands/olap_module.py` & `polyapi-5.7.0.4/polymatica/commands/olap_module.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/commands/other_modules.py` & `polyapi-5.7.0.4/polymatica/commands/other_modules.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/common/consts.py` & `polyapi-5.7.0.4/polymatica/common/consts.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/common/helper_funcs.py` & `polyapi-5.7.0.4/polymatica/common/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/error_handler.py` & `polyapi-5.7.0.4/polymatica/error_handler.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/exceptions.py` & `polyapi-5.7.0.4/polymatica/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/executor.py` & `polyapi-5.7.0.4/polymatica/executor.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/base_graph.py` & `polyapi-5.7.0.4/polymatica/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/graph_interface.py` & `polyapi-5.7.0.4/polymatica/graph/graph_interface.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/__init__.py` & `polyapi-5.7.0.4/polymatica/graph/types/__init__.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/areas.py` & `polyapi-5.7.0.4/polymatica/graph/types/areas.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/balls.py` & `polyapi-5.7.0.4/polymatica/graph/types/balls.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/chord.py` & `polyapi-5.7.0.4/polymatica/graph/types/chord.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/circles.py` & `polyapi-5.7.0.4/polymatica/graph/types/circles.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/circles_series.py` & `polyapi-5.7.0.4/polymatica/graph/types/circles_series.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/corridors.py` & `polyapi-5.7.0.4/polymatica/graph/types/corridors.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/cumulative_areas.py` & `polyapi-5.7.0.4/polymatica/graph/types/cumulative_areas.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/cumulative_cylinders.py` & `polyapi-5.7.0.4/polymatica/graph/types/cumulative_cylinders.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/cylinders.py` & `polyapi-5.7.0.4/polymatica/graph/types/cylinders.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/graph.py` & `polyapi-5.7.0.4/polymatica/graph/types/graph.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/lines.py` & `polyapi-5.7.0.4/polymatica/graph/types/lines.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/pies.py` & `polyapi-5.7.0.4/polymatica/graph/types/pies.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/point.py` & `polyapi-5.7.0.4/polymatica/graph/types/point.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/point_series.py` & `polyapi-5.7.0.4/polymatica/graph/types/point_series.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/pools.py` & `polyapi-5.7.0.4/polymatica/graph/types/pools.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/pools_3d.py` & `polyapi-5.7.0.4/polymatica/graph/types/pools_3d.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/radar.py` & `polyapi-5.7.0.4/polymatica/graph/types/radar.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/sankey.py` & `polyapi-5.7.0.4/polymatica/graph/types/sankey.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/graph/types/surface.py` & `polyapi-5.7.0.4/polymatica/graph/types/surface.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/helper.py` & `polyapi-5.7.0.4/polymatica/helper.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/versions/polymatica_57.py` & `polyapi-5.7.0.4/polymatica/versions/polymatica_57.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/polymatica/versions/versions_redirect.py` & `polyapi-5.7.0.4/polymatica/versions/versions_redirect.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.3/setup.py` & `polyapi-5.7.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='polyapi',
-    version='5.7.0.3',
+    version='5.7.0.4',
     description='Wrapper for Polymatica API',
     long_description=open('README.txt', encoding='utf-8').read(),
     url='https://www.polymatica.ru',
     author='Polymatica Rus LLC',
     author_email='development@polymatica.com',
     license='MIT',
     classifiers=classifiers,
```

