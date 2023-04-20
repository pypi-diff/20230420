# Comparing `tmp/tap_exact-0.2.2.tar.gz` & `tmp/tap_exact-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_exact-0.2.2.tar", max compression
+gzip compressed data, was "tap_exact-0.2.3.tar", max compression
```

## Comparing `tap_exact-0.2.2.tar` & `tap_exact-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      932 2023-04-20 12:48:50.209328 tap_exact-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.2.2/tap_exact/__init__.py
--rw-r--r--   0        0        0      842 2023-04-20 11:44:26.669328 tap_exact-0.2.2/tap_exact/client.py
--rw-r--r--   0        0        0    30364 2023-04-20 12:47:01.959328 tap_exact-0.2.2/tap_exact/streams.py
--rw-r--r--   0        0        0     1677 2023-04-19 14:49:52.622465 tap_exact-0.2.2/tap_exact/tap.py
--rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.2.2/tap_exact/tests/__init__.py
--rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.2.2/tap_exact/tests/test_core.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.2.2/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      932 2023-04-20 13:26:22.089328 tap_exact-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.2.3/tap_exact/__init__.py
+-rw-r--r--   0        0        0      842 2023-04-20 11:44:26.669328 tap_exact-0.2.3/tap_exact/client.py
+-rw-r--r--   0        0        0    30438 2023-04-20 13:26:14.609328 tap_exact-0.2.3/tap_exact/streams.py
+-rw-r--r--   0        0        0     1677 2023-04-19 14:49:52.622465 tap_exact-0.2.3/tap_exact/tap.py
+-rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.2.3/tap_exact/tests/__init__.py
+-rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.2.3/tap_exact/tests/test_core.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.2.3/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.2.3/PKG-INFO
```

### Comparing `tap_exact-0.2.2/pyproject.toml` & `tap_exact-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exact"
-version = "0.2.2"
+version = "0.2.3"
 description = "`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK."
 authors = ["Janick Otten"]
 keywords = [
     "ELT",
     "Exact Online",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_exact-0.2.2/tap_exact/client.py` & `tap_exact-0.2.3/tap_exact/client.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.2.2/tap_exact/streams.py` & `tap_exact-0.2.3/tap_exact/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
 
         # This stream should disregard the start_date as earliest starting timestamp
         if datetime.strptime(self.config.get("start_date"), '%Y-%m-%d').strftime('%Y-%m-%d') != self.get_starting_timestamp(context).strftime('%Y-%m-%d'):
             replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
             
             filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
                 
-        path = f"/financial/GLAccounts?{filter_path}" \
+        path = f"/financial/GLAccounts?{filter_path if 'filter_path' in locals() else ''}" \
             "$select=ID,Code,Description,Costcenter,CostcenterDescription,Costunit,CostunitDescription,Modified"
 
         return path
 
     def get_records(self, context: Optional[dict]) -> Iterable[dict]:
         """Return a generator or row-type dictionary objects"""
         
@@ -874,15 +874,15 @@
 
         # This stream should disregard the start_date as earliest starting timestamp
         if datetime.strptime(self.config.get("start_date"), '%Y-%m-%d').strftime('%Y-%m-%d') != self.get_starting_timestamp(context).strftime('%Y-%m-%d'):
             replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
             
             filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
         
-        path = f"/crm/Accounts?{filter_path}" \
+        path = f"/crm/Accounts?{filter_path if 'filter_path' in locals() else ''}" \
             "$select=ID,AccountManager,AccountManagerFullName,Code,City,CountryName,Latitude,Longitude,Name,SearchCode,Modified"
 
         return path
 
     def get_records(self, context: Optional[dict]) -> Iterable[dict]:
         """Return a generator or row-type dictionary objects"""
```

### Comparing `tap_exact-0.2.2/tap_exact/tap.py` & `tap_exact-0.2.3/tap_exact/tap.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.2.2/tap_exact/tests/test_core.py` & `tap_exact-0.2.3/tap_exact/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.2.2/setup.py` & `tap_exact-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['tap-exact = tap_exact.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exact',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': '`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.',
     'long_description': 'None',
     'author': 'Janick Otten',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap_exact-0.2.2/PKG-INFO` & `tap_exact-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exact
-Version: 0.2.2
+Version: 0.2.3
 Summary: `tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Exact Online
 Author: Janick Otten
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

