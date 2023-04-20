# Comparing `tmp/dequeai-0.732.tar.gz` & `tmp/dequeai-0.734.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.732.tar", last modified: Thu Apr 20 20:58:53 2023, max compression
+gzip compressed data, was "dequeai-0.734.tar", last modified: Thu Apr 20 21:02:52 2023, max compression
```

## Comparing `dequeai-0.732.tar` & `dequeai-0.734.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:58:53.667024 dequeai-0.732/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 20:58:53.667024 dequeai-0.732/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:58:53.667024 dequeai-0.732/dequeai/
--rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.732/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.732/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.732/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.732/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-04-20 20:33:33.000000 dequeai-0.732/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    23887 2023-04-20 20:57:09.000000 dequeai-0.732/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.732/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.732/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.732/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.732/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:58:53.667024 dequeai-0.732/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 20:58:53.000000 dequeai-0.732/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 20:58:53.000000 dequeai-0.732/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:58:53.000000 dequeai-0.732/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 20:58:53.000000 dequeai-0.732/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 20:58:53.000000 dequeai-0.732/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 20:58:53.667024 dequeai-0.732/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 20:58:40.000000 dequeai-0.732/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:02:52.052342 dequeai-0.734/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 21:02:52.052342 dequeai-0.734/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:02:52.052342 dequeai-0.734/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.734/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.734/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.734/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.734/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-04-20 20:33:33.000000 dequeai-0.734/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    24554 2023-04-20 21:02:32.000000 dequeai-0.734/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.734/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.734/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.734/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.734/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:02:52.052342 dequeai-0.734/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 21:02:51.000000 dequeai-0.734/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 21:02:52.000000 dequeai-0.734/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 21:02:51.000000 dequeai-0.734/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 21:02:51.000000 dequeai-0.734/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 21:02:51.000000 dequeai-0.734/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 21:02:52.052342 dequeai-0.734/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 21:02:32.000000 dequeai-0.734/setup.py
```

### Comparing `dequeai-0.732/dequeai/datatypes.py` & `dequeai-0.734/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.732/dequeai/dequeai.py` & `dequeai-0.734/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.732/dequeai/dequeai_run.py` & `dequeai-0.734/dequeai/dequeai_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -443,33 +443,42 @@
 
         req_data = {
             "user_name": self.user_name,
             "project_name": project_name,
             "metric_key": metric_key
         }
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/best/read/", json=req_data)
-        res = resp.json()
-        print(res)
-        # convert res to a dataframe
-        runs = res['runs']
-        run_data = []
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
+        first_run_data_keys = list(data_list['runs'][0]['best_experiment_data']['data'].keys())
+        headers = ['Run ID', 'Best Metric Key', 'Best Metric'] + [f'{key}.{sub_key}' for key in first_run_data_keys for
+                                                                  sub_key in
+                                                                  data_list['runs'][0]['best_experiment_data']['data'][
+                                                                      key]]
+
+        # Extract rows
+        rows = []
+        for run in data_list['runs']:
+            best_metric = self._get_nested_value(run['best_experiment_data']['data'], metric_key)
+            row = [run['run_id'], metric_key, best_metric]
+            for key in first_run_data_keys:
+                row.extend(run['best_experiment_data']['data'][key].values())
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
 
+
     def search_runs(self,filter_dict):
         if self.user_name is None:
             raise ValueError("Please initialize using dequeai.init() before calling search_runs")
         req_data = {
             "user_name": self.user_name,
             "filter_dict": filter_dict
         }
```

### Comparing `dequeai-0.732/dequeai/parsing_service.py` & `dequeai-0.734/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.732/dequeai/rest_connect.py` & `dequeai-0.734/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.732/dequeai/util.py` & `dequeai-0.734/dequeai/util.py`

 * *Files identical despite different names*

