# Comparing `tmp/dequeai-0.718.tar.gz` & `tmp/dequeai-0.720.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.718.tar", last modified: Thu Apr 20 16:42:51 2023, max compression
+gzip compressed data, was "dequeai-0.720.tar", last modified: Thu Apr 20 17:23:01 2023, max compression
```

## Comparing `dequeai-0.718.tar` & `dequeai-0.720.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 16:42:51.395542 dequeai-0.718/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 16:42:51.395542 dequeai-0.718/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 16:42:51.395542 dequeai-0.718/dequeai/
--rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.718/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.718/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.718/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.718/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      735 2023-04-19 19:09:20.000000 dequeai-0.718/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    20259 2023-04-20 16:42:15.000000 dequeai-0.718/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.718/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.718/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.718/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.718/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 16:42:51.395542 dequeai-0.718/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 16:42:50.000000 dequeai-0.718/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 16:42:51.000000 dequeai-0.718/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 16:42:50.000000 dequeai-0.718/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 16:42:51.000000 dequeai-0.718/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 16:42:51.000000 dequeai-0.718/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 16:42:51.395542 dequeai-0.718/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 16:42:36.000000 dequeai-0.718/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:23:01.192436 dequeai-0.720/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 17:23:01.192436 dequeai-0.720/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:23:01.192436 dequeai-0.720/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.720/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.720/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.720/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.720/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-04-19 19:09:20.000000 dequeai-0.720/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    20284 2023-04-20 17:22:48.000000 dequeai-0.720/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.720/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.720/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.720/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.720/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:23:01.192436 dequeai-0.720/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 17:23:00.000000 dequeai-0.720/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 17:23:01.000000 dequeai-0.720/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 17:23:00.000000 dequeai-0.720/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 17:23:01.000000 dequeai-0.720/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 17:23:01.000000 dequeai-0.720/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 17:23:01.192436 dequeai-0.720/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 17:22:48.000000 dequeai-0.720/setup.py
```

### Comparing `dequeai-0.718/dequeai/datatypes.py` & `dequeai-0.720/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.718/dequeai/dequeai.py` & `dequeai-0.720/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.718/dequeai/dequeai_run.py` & `dequeai-0.720/dequeai/dequeai_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,16 +398,17 @@
             raise ValueError("Please initialize using dequeai.init() before calling compare_runs")
         req_data = {
             "user_name": self.user_name,
             "run_ids": run_ids
         }
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/compare/", json=req_data)
         res = resp.json()
+        print(res)
         # convert res to a dataframe
-        headers = res[0].keys()
+        headers = list(res)[0].keys()
         rows = [list(x.values()) for x in res]
         html_table = tabulate(rows, headers, tablefmt="html")
         scrollable_table = f'<div style="width: 100%; height: 200px; overflow: auto;">{html_table}</div>'
         display(HTML(scrollable_table))
 
     def search_runs(self,filter_dict):
         if self.user_name is None:
```

### Comparing `dequeai-0.718/dequeai/parsing_service.py` & `dequeai-0.720/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.718/dequeai/rest_connect.py` & `dequeai-0.720/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.718/dequeai/util.py` & `dequeai-0.720/dequeai/util.py`

 * *Files identical despite different names*

