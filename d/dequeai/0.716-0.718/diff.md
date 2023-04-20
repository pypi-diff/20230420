# Comparing `tmp/dequeai-0.716.tar.gz` & `tmp/dequeai-0.718.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.716.tar", last modified: Wed Apr 19 19:10:33 2023, max compression
+gzip compressed data, was "dequeai-0.718.tar", last modified: Thu Apr 20 16:42:51 2023, max compression
```

## Comparing `dequeai-0.716.tar` & `dequeai-0.718.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:10:33.045097 dequeai-0.716/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-19 19:10:33.045097 dequeai-0.716/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:10:33.045097 dequeai-0.716/dequeai/
--rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.716/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.716/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.716/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.716/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      735 2023-04-19 19:09:20.000000 dequeai-0.716/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    19998 2023-04-19 19:08:35.000000 dequeai-0.716/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.716/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.716/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.716/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.716/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:10:33.045097 dequeai-0.716/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-19 19:10:32.000000 dequeai-0.716/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-19 19:10:33.000000 dequeai-0.716/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:10:32.000000 dequeai-0.716/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-19 19:10:32.000000 dequeai-0.716/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 19:10:32.000000 dequeai-0.716/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 19:10:33.045097 dequeai-0.716/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      470 2023-04-19 19:10:17.000000 dequeai-0.716/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 16:42:51.395542 dequeai-0.718/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 16:42:51.395542 dequeai-0.718/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 16:42:51.395542 dequeai-0.718/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.718/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.718/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.718/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.718/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-04-19 19:09:20.000000 dequeai-0.718/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    20259 2023-04-20 16:42:15.000000 dequeai-0.718/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.718/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.718/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.718/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.718/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 16:42:51.395542 dequeai-0.718/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 16:42:50.000000 dequeai-0.718/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 16:42:51.000000 dequeai-0.718/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 16:42:50.000000 dequeai-0.718/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 16:42:51.000000 dequeai-0.718/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 16:42:51.000000 dequeai-0.718/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 16:42:51.395542 dequeai-0.718/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 16:42:36.000000 dequeai-0.718/setup.py
```

### Comparing `dequeai-0.716/dequeai/datatypes.py` & `dequeai-0.718/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.716/dequeai/dequeai.py` & `dequeai-0.718/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.716/dequeai/dequeai_run.py` & `dequeai-0.718/dequeai/dequeai_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 import requests
 import glob
 import time
 import psutil
 import GPUtil
 import socket
 import types
-import pandas as pd
+from IPython.display import display,HTML
+from tabulate import tabulate
+
+
 
 _RESOURCE_MONITORING_INTERVAL = 60
 
 class Run:
 
     def __init__(self):
         self.user_name = None
@@ -396,17 +399,19 @@
         req_data = {
             "user_name": self.user_name,
             "run_ids": run_ids
         }
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/compare/", json=req_data)
         res = resp.json()
         # convert res to a dataframe
-        res_df = pd.DataFrame(res)
-        print(res_df)
-        return res_df
+        headers = res[0].keys()
+        rows = [list(x.values()) for x in res]
+        html_table = tabulate(rows, headers, tablefmt="html")
+        scrollable_table = f'<div style="width: 100%; height: 200px; overflow: auto;">{html_table}</div>'
+        display(HTML(scrollable_table))
 
     def search_runs(self,filter_dict):
         if self.user_name is None:
             raise ValueError("Please initialize using dequeai.init() before calling search_runs")
         req_data = {
             "user_name": self.user_name,
             "filter_dict": filter_dict
```

### Comparing `dequeai-0.716/dequeai/parsing_service.py` & `dequeai-0.718/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.716/dequeai/rest_connect.py` & `dequeai-0.718/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.716/dequeai/util.py` & `dequeai-0.718/dequeai/util.py`

 * *Files identical despite different names*

