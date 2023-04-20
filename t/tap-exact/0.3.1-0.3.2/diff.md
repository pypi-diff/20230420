# Comparing `tmp/tap_exact-0.3.1.tar.gz` & `tmp/tap_exact-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_exact-0.3.1.tar", max compression
+gzip compressed data, was "tap_exact-0.3.2.tar", max compression
```

## Comparing `tap_exact-0.3.1.tar` & `tap_exact-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      932 2023-04-20 17:57:20.449328 tap_exact-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.3.1/tap_exact/__init__.py
--rw-r--r--   0        0        0      842 2023-04-20 11:44:26.669328 tap_exact-0.3.1/tap_exact/client.py
--rw-r--r--   0        0        0    33335 2023-04-20 17:34:39.479328 tap_exact-0.3.1/tap_exact/streams.py
--rw-r--r--   0        0        0     1723 2023-04-20 17:21:53.919328 tap_exact-0.3.1/tap_exact/tap.py
--rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.3.1/tap_exact/tests/__init__.py
--rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.3.1/tap_exact/tests/test_core.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.3.1/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      932 2023-04-20 18:30:14.139328 tap_exact-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.3.2/tap_exact/__init__.py
+-rw-r--r--   0        0        0      842 2023-04-20 11:44:26.669328 tap_exact-0.3.2/tap_exact/client.py
+-rw-r--r--   0        0        0    33317 2023-04-20 18:30:06.589328 tap_exact-0.3.2/tap_exact/streams.py
+-rw-r--r--   0        0        0     1723 2023-04-20 17:21:53.919328 tap_exact-0.3.2/tap_exact/tap.py
+-rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.3.2/tap_exact/tests/__init__.py
+-rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.3.2/tap_exact/tests/test_core.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.3.2/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.3.2/PKG-INFO
```

### Comparing `tap_exact-0.3.1/pyproject.toml` & `tap_exact-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exact"
-version = "0.3.1"
+version = "0.3.2"
 description = "`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK."
 authors = ["Janick Otten"]
 keywords = [
     "ELT",
     "Exact Online",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_exact-0.3.1/tap_exact/client.py` & `tap_exact-0.3.2/tap_exact/client.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.3.1/tap_exact/streams.py` & `tap_exact-0.3.2/tap_exact/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -963,15 +963,15 @@
             "$select=UserID,FullName,Email,StartDate,EndDate,Modified"
 
         return path
 
     def get_records(self, context: Optional[dict]) -> Iterable[dict]:
         """Return a generator or row-type dictionary objects"""
         
-        resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
+        resp = self.conn.rest(GET('v1/%s' % (self.get_path(context) )))
         
         # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
         keys = ['StartDate', 'EndDate', 'Modified']
 
         for row in resp:
             
             # We loop through the keys that should be modified
```

### Comparing `tap_exact-0.3.1/tap_exact/tap.py` & `tap_exact-0.3.2/tap_exact/tap.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.3.1/tap_exact/tests/test_core.py` & `tap_exact-0.3.2/tap_exact/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.3.1/setup.py` & `tap_exact-0.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['tap-exact = tap_exact.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exact',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': '`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.',
     'long_description': 'None',
     'author': 'Janick Otten',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap_exact-0.3.1/PKG-INFO` & `tap_exact-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exact
-Version: 0.3.1
+Version: 0.3.2
 Summary: `tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Exact Online
 Author: Janick Otten
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

