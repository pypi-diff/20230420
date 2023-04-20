# Comparing `tmp/easycheck_doiteasy-0.0.4.tar.gz` & `tmp/easycheck_doiteasy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycheck_doiteasy-0.0.4.tar", last modified: Wed Apr 19 17:25:55 2023, max compression
+gzip compressed data, was "easycheck_doiteasy-0.0.5.tar", last modified: Wed Apr 19 22:54:33 2023, max compression
```

## Comparing `easycheck_doiteasy-0.0.4.tar` & `easycheck_doiteasy-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-19 17:25:55.317326 easycheck_doiteasy-0.0.4/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1061 2023-04-11 19:56:22.000000 easycheck_doiteasy-0.0.4/LICENSE.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-19 17:25:55.317326 easycheck_doiteasy-0.0.4/PKG-INFO
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1292 2023-04-11 17:30:51.000000 easycheck_doiteasy-0.0.4/README.md
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-19 17:25:55.317326 easycheck_doiteasy-0.0.4/easycheck_doiteasy/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 15:17:56.000000 easycheck_doiteasy-0.0.4/easycheck_doiteasy/__init__.py
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     4854 2023-04-19 17:15:15.000000 easycheck_doiteasy-0.0.4/easycheck_doiteasy/easycheck_doiteasy.py
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-19 17:25:55.317326 easycheck_doiteasy-0.0.4/easycheck_doiteasy.egg-info/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-19 17:25:55.000000 easycheck_doiteasy-0.0.4/easycheck_doiteasy.egg-info/PKG-INFO
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      286 2023-04-19 17:25:55.000000 easycheck_doiteasy-0.0.4/easycheck_doiteasy.egg-info/SOURCES.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        1 2023-04-19 17:25:55.000000 easycheck_doiteasy-0.0.4/easycheck_doiteasy.egg-info/dependency_links.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       19 2023-04-19 17:25:55.000000 easycheck_doiteasy-0.0.4/easycheck_doiteasy.egg-info/top_level.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       84 2023-04-12 16:58:48.000000 easycheck_doiteasy-0.0.4/pyproject.toml
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      670 2023-04-19 17:25:55.321326 easycheck_doiteasy-0.0.4/setup.cfg
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-19 22:54:33.899768 easycheck_doiteasy-0.0.5/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1061 2023-04-11 19:56:22.000000 easycheck_doiteasy-0.0.5/LICENSE.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-19 22:54:33.899768 easycheck_doiteasy-0.0.5/PKG-INFO
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1292 2023-04-11 17:30:51.000000 easycheck_doiteasy-0.0.5/README.md
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-19 22:54:33.895768 easycheck_doiteasy-0.0.5/easycheck_doiteasy/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 15:17:56.000000 easycheck_doiteasy-0.0.5/easycheck_doiteasy/__init__.py
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     5150 2023-04-19 22:53:12.000000 easycheck_doiteasy-0.0.5/easycheck_doiteasy/easycheck_doiteasy.py
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-19 22:54:33.899768 easycheck_doiteasy-0.0.5/easycheck_doiteasy.egg-info/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-19 22:54:33.000000 easycheck_doiteasy-0.0.5/easycheck_doiteasy.egg-info/PKG-INFO
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      286 2023-04-19 22:54:33.000000 easycheck_doiteasy-0.0.5/easycheck_doiteasy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        1 2023-04-19 22:54:33.000000 easycheck_doiteasy-0.0.5/easycheck_doiteasy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       19 2023-04-19 22:54:33.000000 easycheck_doiteasy-0.0.5/easycheck_doiteasy.egg-info/top_level.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       84 2023-04-12 16:58:48.000000 easycheck_doiteasy-0.0.5/pyproject.toml
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      670 2023-04-19 22:54:33.899768 easycheck_doiteasy-0.0.5/setup.cfg
```

### Comparing `easycheck_doiteasy-0.0.4/LICENSE.txt` & `easycheck_doiteasy-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easycheck_doiteasy-0.0.4/PKG-INFO` & `easycheck_doiteasy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycheck_doiteasy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple Python package example
 Home-page: https://etlcheck.com/
 Author: Jesus Rojas
 Author-email: jora2415@gmailc.om
 Project-URL: Bug Tracker, https://github.com/kamicase24/easycheck/-/issues
 Project-URL: repository, https://github.com/kamicase24/easycheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easycheck_doiteasy-0.0.4/README.md` & `easycheck_doiteasy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `easycheck_doiteasy-0.0.4/easycheck_doiteasy/easycheck_doiteasy.py` & `easycheck_doiteasy-0.0.5/easycheck_doiteasy/easycheck_doiteasy.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         token (str): The authentication token for the ETLCheck API.
         Attributes:
         token (str): The provided authentication token.
         domain (str): The default domain URL for API calls.
         """
         self.token = token
         self.domain = 'https://etlcheck.com'
+        self.ejecution_line_ids = []
 
 
     def send_ejecution(self, name, duration, start_datetime, end_datetime, destination, total_register, successful):
         """
         Sends execution data to a specified API endpoint.
 
         Parameters:
@@ -47,14 +48,18 @@
             'start_datetime': start_datetime,
             'end_datetime': end_datetime,
             'destination': destination,
             'total_register': total_register,
             'successful': successful,
             'register_token': self.token
         }
+
+        if len(self.ejecution_line_ids) > 0:
+            data.update({'ejecution_line_ids': self.ejecution_line_ids})
+        self.ejecution_line_ids = []
         try:
             requests.post(url, data=data, headers=headers)
         except Exception as e:
             logging.error(e)
 
     
     def send_subejecution(self, name, duration, start_datetime, end_datetime, total_register, successful):
@@ -84,15 +89,17 @@
             'start_datetime': start_datetime,
             'end_datetime': end_datetime,
             'total_register': total_register,
             'successful': successful,
             'register_token': self.token
         }
         try:
-            requests.post(url, data=data, headers=headers)
+            res = requests.post(url, data=data, headers=headers)
+            if res.status_code == 200:
+                self.ejecution_line_ids.append(res['id'])
         except Exception as e:
             logging.error(e)
 
 
 
     def update_logs_directories(self, logs_dir):
```

### Comparing `easycheck_doiteasy-0.0.4/easycheck_doiteasy.egg-info/PKG-INFO` & `easycheck_doiteasy-0.0.5/easycheck_doiteasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycheck-doiteasy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple Python package example
 Home-page: https://etlcheck.com/
 Author: Jesus Rojas
 Author-email: jora2415@gmailc.om
 Project-URL: Bug Tracker, https://github.com/kamicase24/easycheck/-/issues
 Project-URL: repository, https://github.com/kamicase24/easycheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easycheck_doiteasy-0.0.4/setup.cfg` & `easycheck_doiteasy-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easycheck_doiteasy
-version = 0.0.4
+version = 0.0.5
 author = Jesus Rojas
 author_email = jora2415@gmailc.om
 description = A simple Python package example
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://etlcheck.com/
 project_urls =
```

