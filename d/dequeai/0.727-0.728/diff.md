# Comparing `tmp/dequeai-0.727.tar.gz` & `tmp/dequeai-0.728.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.727.tar", last modified: Thu Apr 20 20:33:53 2023, max compression
+gzip compressed data, was "dequeai-0.728.tar", last modified: Thu Apr 20 20:42:36 2023, max compression
```

## Comparing `dequeai-0.727.tar` & `dequeai-0.728.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:33:53.451086 dequeai-0.727/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 20:33:53.451086 dequeai-0.727/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:33:53.451086 dequeai-0.727/dequeai/
--rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.727/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.727/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.727/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.727/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-04-20 20:33:33.000000 dequeai-0.727/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    23222 2023-04-20 20:33:33.000000 dequeai-0.727/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.727/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.727/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.727/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.727/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:33:53.451086 dequeai-0.727/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 20:33:52.000000 dequeai-0.727/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 20:33:53.000000 dequeai-0.727/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:33:52.000000 dequeai-0.727/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 20:33:53.000000 dequeai-0.727/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 20:33:53.000000 dequeai-0.727/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 20:33:53.451086 dequeai-0.727/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 20:33:40.000000 dequeai-0.727/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:42:36.305944 dequeai-0.728/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 20:42:36.305944 dequeai-0.728/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:42:36.305944 dequeai-0.728/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.728/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.728/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.728/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.728/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-04-20 20:33:33.000000 dequeai-0.728/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    23392 2023-04-20 20:42:21.000000 dequeai-0.728/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.728/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.728/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.728/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.728/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:42:36.305944 dequeai-0.728/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 20:42:35.000000 dequeai-0.728/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 20:42:36.000000 dequeai-0.728/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:42:35.000000 dequeai-0.728/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 20:42:36.000000 dequeai-0.728/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 20:42:36.000000 dequeai-0.728/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 20:42:36.305944 dequeai-0.728/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 20:42:21.000000 dequeai-0.728/setup.py
```

### Comparing `dequeai-0.727/dequeai/datatypes.py` & `dequeai-0.728/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.727/dequeai/dequeai.py` & `dequeai-0.728/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.727/dequeai/dequeai_run.py` & `dequeai-0.728/dequeai/dequeai_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,32 +402,34 @@
 
         req_data = {
             "user_name": self.user_name,
             "project_name": project_name,
             "metric_key": metric_key
         }
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/compare/", json=req_data)
-        res = resp.json()
-        print(res)
-        # convert res to a dataframe
-        runs = res['runs']
-        run_data = []
-
-
-        for run in runs:
-            if "data" not in run:
-                continue
-
-            rows = [list(x.values()) for x in run['data']]
-            run_data.append(rows)
-        filtered_data = self._filter_dicts_by_keys(run_data, metric_key)
-        headers = filtered_data.keys()
-        print(filtered_data)
-        html_table = tabulate(filtered_data, headers, tablefmt="html")
+        data_list = resp.json()
+        print(data_list)
+        # Extract header names
+        headers = ['Run ID', 'Best Metric'] + list(
+            data_list['runs'][0]['best_experiment_data']['data'][metric_key].keys())
+
+        # Extract rows
+        rows = []
+        for run in data_list['runs']:
+            row = [run['run_id'], run['best_metric']] + list(
+                run['best_experiment_data']['data'][metric_key].values())
+            rows.append(row)
+
+        # Use tabulate to generate the HTML table
+        html_table = tabulate(rows, headers=headers, tablefmt="html")
+
+        # Wrap the table in a scrollable div
         scrollable_table = f'<div style="width: 100%; height: 200px; overflow: auto;">{html_table}</div>'
+
+        # Display the scrollable table in the notebook
         display(HTML(scrollable_table))
 
     def read_best_run(self, project_name, metric_key):
 
         if self.user_name is None:
             raise ValueError("Please initialize using dequeai.init() before calling compare_runs")
```

### Comparing `dequeai-0.727/dequeai/parsing_service.py` & `dequeai-0.728/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.727/dequeai/rest_connect.py` & `dequeai-0.728/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.727/dequeai/util.py` & `dequeai-0.728/dequeai/util.py`

 * *Files identical despite different names*

