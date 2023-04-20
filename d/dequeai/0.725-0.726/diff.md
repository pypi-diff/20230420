# Comparing `tmp/dequeai-0.725.tar.gz` & `tmp/dequeai-0.726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.725.tar", last modified: Thu Apr 20 18:42:28 2023, max compression
+gzip compressed data, was "dequeai-0.726.tar", last modified: Thu Apr 20 18:44:33 2023, max compression
```

## Comparing `dequeai-0.725.tar` & `dequeai-0.726.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:42:28.846494 dequeai-0.725/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 18:42:28.846494 dequeai-0.725/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:42:28.846494 dequeai-0.725/dequeai/
--rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.725/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.725/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.725/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.725/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-04-20 18:05:43.000000 dequeai-0.725/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    21851 2023-04-20 18:02:34.000000 dequeai-0.725/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.725/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.725/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.725/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.725/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:42:28.846494 dequeai-0.725/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 18:42:28.000000 dequeai-0.725/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 18:42:28.000000 dequeai-0.725/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 18:42:28.000000 dequeai-0.725/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 18:42:28.000000 dequeai-0.725/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 18:42:28.000000 dequeai-0.725/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 18:42:28.846494 dequeai-0.725/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 18:05:52.000000 dequeai-0.725/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:44:33.150353 dequeai-0.726/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 18:44:33.146353 dequeai-0.726/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:44:33.146353 dequeai-0.726/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.726/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.726/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.726/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.726/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-04-20 18:05:43.000000 dequeai-0.726/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    21911 2023-04-20 18:44:12.000000 dequeai-0.726/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.726/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.726/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.726/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.726/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:44:33.146353 dequeai-0.726/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 18:44:32.000000 dequeai-0.726/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 18:44:33.000000 dequeai-0.726/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 18:44:32.000000 dequeai-0.726/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 18:44:32.000000 dequeai-0.726/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 18:44:33.000000 dequeai-0.726/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 18:44:33.150353 dequeai-0.726/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 18:44:20.000000 dequeai-0.726/setup.py
```

### Comparing `dequeai-0.725/dequeai/datatypes.py` & `dequeai-0.726/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.725/dequeai/dequeai.py` & `dequeai-0.726/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.725/dequeai/dequeai_run.py` & `dequeai-0.726/dequeai/dequeai_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,14 +404,17 @@
         res = resp.json()
         # convert res to a dataframe
         runs = res['runs']
         run_data = []
 
 
         for run in runs:
+            if "data" not in run:
+                continue
+
             rows = [list(x.values()) for x in run['data']]
             run_data.append(rows)
         filtered_data = self._filter_dicts_by_keys(run_data, keys, values, operators)
         headers = filtered_data.keys()
         print(filtered_data)
         html_table = tabulate(filtered_data, headers, tablefmt="html")
         scrollable_table = f'<div style="width: 100%; height: 200px; overflow: auto;">{html_table}</div>'
```

### Comparing `dequeai-0.725/dequeai/parsing_service.py` & `dequeai-0.726/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.725/dequeai/rest_connect.py` & `dequeai-0.726/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.725/dequeai/util.py` & `dequeai-0.726/dequeai/util.py`

 * *Files identical despite different names*

