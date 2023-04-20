# Comparing `tmp/dequeai-0.722.tar.gz` & `tmp/dequeai-0.724.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.722.tar", last modified: Thu Apr 20 17:25:23 2023, max compression
+gzip compressed data, was "dequeai-0.724.tar", last modified: Thu Apr 20 18:02:56 2023, max compression
```

## Comparing `dequeai-0.722.tar` & `dequeai-0.724.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:25:23.865003 dequeai-0.722/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 17:25:23.861003 dequeai-0.722/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:25:23.861003 dequeai-0.722/dequeai/
--rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.722/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.722/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.722/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.722/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      735 2023-04-19 19:09:20.000000 dequeai-0.722/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    20288 2023-04-20 17:24:58.000000 dequeai-0.722/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.722/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.722/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.722/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.722/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 17:25:23.861003 dequeai-0.722/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 17:25:23.000000 dequeai-0.722/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 17:25:23.000000 dequeai-0.722/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 17:25:23.000000 dequeai-0.722/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 17:25:23.000000 dequeai-0.722/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 17:25:23.000000 dequeai-0.722/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 17:25:23.865003 dequeai-0.722/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 17:25:10.000000 dequeai-0.722/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:02:56.282600 dequeai-0.724/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 18:02:56.282600 dequeai-0.724/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:02:56.282600 dequeai-0.724/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.724/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.724/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.724/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.724/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-04-19 19:09:20.000000 dequeai-0.724/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    21851 2023-04-20 18:02:34.000000 dequeai-0.724/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.724/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.724/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.724/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.724/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:02:56.282600 dequeai-0.724/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 18:02:55.000000 dequeai-0.724/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 18:02:56.000000 dequeai-0.724/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 18:02:55.000000 dequeai-0.724/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 18:02:56.000000 dequeai-0.724/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 18:02:56.000000 dequeai-0.724/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 18:02:56.282600 dequeai-0.724/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 18:02:43.000000 dequeai-0.724/setup.py
```

### Comparing `dequeai-0.722/dequeai/datatypes.py` & `dequeai-0.724/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.722/dequeai/dequeai.py` & `dequeai-0.724/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.722/dequeai/dequeai_run.py` & `dequeai-0.724/dequeai/dequeai_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -389,28 +389,35 @@
         res = resp.json()
         print(res)
         if "authenticated" in res:
             return res["authenticated"]
         else:
             return False
 
-    def compare_runs(self, run_ids):
+    def compare_runs(self, run_ids,keys, values=None, operators=None):
         if self.user_name is None:
             raise ValueError("Please initialize using dequeai.init() before calling compare_runs")
         req_data = {
             "user_name": self.user_name,
             "run_ids": run_ids
         }
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/compare/", json=req_data)
         res = resp.json()
         # convert res to a dataframe
         runs = res['runs']
-        headers = runs[0].keys()
-        rows = [list(x.values()) for x in runs]
-        html_table = tabulate(rows, headers, tablefmt="html")
+        run_data = []
+
+
+        for run in runs:
+            rows = [list(x.values()) for x in run['data']]
+            run_data.append(rows)
+        filtered_data = self._filter_dicts_by_keys(run_data, keys, values, operators)
+        headers = filtered_data.keys()
+        print(filtered_data)
+        html_table = tabulate(filtered_data, headers, tablefmt="html")
         scrollable_table = f'<div style="width: 100%; height: 200px; overflow: auto;">{html_table}</div>'
         display(HTML(scrollable_table))
 
     def search_runs(self,filter_dict):
         if self.user_name is None:
             raise ValueError("Please initialize using dequeai.init() before calling search_runs")
         req_data = {
@@ -432,14 +439,59 @@
         }
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/report/create/", json=req_data)
         res = resp.json()
         print(res)
         return res
 
 
+    def _filter_dicts_by_keys(self,dicts_list, keys, values=None, operators=None):
+        filtered_dicts = []
+
+        if not values:
+            values = [None] * len(keys)
+
+        if not operators:
+            operators = ['=='] * len(keys)
+
+        for d in dicts_list:
+            match = True
+            for key, value, op in zip(keys, values, operators):
+                nested_value = self._get_nested_value(d, key)
+
+                if op == '==':
+                    if nested_value != value:
+                        match = False
+                        break
+                elif op == '>':
+                    if nested_value is None or nested_value <= value:
+                        match = False
+                        break
+                elif op == '<':
+                    if nested_value is None or nested_value >= value:
+                        match = False
+                        break
+
+            if match:
+                filtered_dicts.append(d)
+
+        return filtered_dicts
+
+
+    def _get_nested_value(self,nested_dict, key):
+        keys = key.split('.')
+        current_dict = nested_dict
+
+        for k in keys:
+            if k in current_dict:
+                current_dict = current_dict[k]
+            else:
+                return None
+
+        return current_dict
+
 if __name__ == "__main__":
     deque = Run()
     deque._validate_hyperparams({"train": {"accuracy": "1.3", "loss": "2.2"}})
     #deque.log_artifact_task(artifact_type=RESOURCES, path="//dequeapp.egg-info",
        #                     run_meta_data=None)
     # deque.init(user_name="riju@deque.app", project_name="awesome-dude")
     # for i in range(100):
```

### Comparing `dequeai-0.722/dequeai/parsing_service.py` & `dequeai-0.724/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.722/dequeai/rest_connect.py` & `dequeai-0.724/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.722/dequeai/util.py` & `dequeai-0.724/dequeai/util.py`

 * *Files identical despite different names*

