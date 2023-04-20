# Comparing `tmp/pygoogalytics-0.2.8.tar.gz` & `tmp/pygoogalytics-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygoogalytics-0.2.8.tar", last modified: Thu Apr 13 10:58:45 2023, max compression
+gzip compressed data, was "pygoogalytics-0.3.0.tar", last modified: Thu Apr 20 08:36:08 2023, max compression
```

## Comparing `pygoogalytics-0.2.8.tar` & `pygoogalytics-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 10:58:45.685303 pygoogalytics-0.2.8/
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.2.8/LICENCE.txt
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.2.8/LICENSE
--rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-13 10:58:45.685149 pygoogalytics-0.2.8/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     4882 2023-02-23 08:04:27.000000 pygoogalytics-0.2.8/README.md
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 10:58:45.683525 pygoogalytics-0.2.8/pygoogalytics/
--rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-04-13 10:58:25.000000 pygoogalytics-0.2.8/pygoogalytics/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     5911 2023-04-13 08:54:19.000000 pygoogalytics-0.2.8/pygoogalytics/client.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 10:58:45.684742 pygoogalytics-0.2.8/pygoogalytics/data/
--rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.2.8/pygoogalytics/data/country_iso_codes.csv
--rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.2.8/pygoogalytics/data/google_ads_location_ids.csv
--rw-r--r--   0 joshua     (501) staff       (20)    36784 2023-04-13 07:30:02.000000 pygoogalytics-0.2.8/pygoogalytics/googalytics_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)    32322 2023-02-21 11:27:36.000000 pygoogalytics-0.2.8/pygoogalytics/googlepandas.py
--rw-r--r--   0 joshua     (501) staff       (20)    42080 2023-04-13 10:54:44.000000 pygoogalytics-0.2.8/pygoogalytics/kwp_wrappers.py
--rw-r--r--   0 joshua     (501) staff       (20)     2409 2023-03-07 19:50:49.000000 pygoogalytics-0.2.8/pygoogalytics/resource_utils.py
--rw-r--r--   0 joshua     (501) staff       (20)     2064 2023-02-20 08:31:45.000000 pygoogalytics-0.2.8/pygoogalytics/utils.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 10:58:45.684227 pygoogalytics-0.2.8/pygoogalytics.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-13 10:58:45.000000 pygoogalytics-0.2.8/pygoogalytics.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      512 2023-04-13 10:58:45.000000 pygoogalytics-0.2.8/pygoogalytics.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2023-04-13 10:58:45.000000 pygoogalytics-0.2.8/pygoogalytics.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)      113 2023-04-13 10:58:45.000000 pygoogalytics-0.2.8/pygoogalytics.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)       14 2023-04-13 10:58:45.000000 pygoogalytics-0.2.8/pygoogalytics.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2023-04-13 10:58:45.685344 pygoogalytics-0.2.8/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-04-13 10:58:25.000000 pygoogalytics-0.2.8/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-20 08:36:08.271873 pygoogalytics-0.3.0/
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.3.0/LICENCE.txt
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.3.0/LICENSE
+-rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-20 08:36:08.271757 pygoogalytics-0.3.0/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     4882 2023-02-23 08:04:27.000000 pygoogalytics-0.3.0/README.md
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-20 08:36:08.270323 pygoogalytics-0.3.0/pygoogalytics/
+-rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-04-20 08:35:10.000000 pygoogalytics-0.3.0/pygoogalytics/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5386 2023-04-20 08:34:21.000000 pygoogalytics-0.3.0/pygoogalytics/client.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-20 08:36:08.271448 pygoogalytics-0.3.0/pygoogalytics/data/
+-rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.3.0/pygoogalytics/data/country_iso_codes.csv
+-rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.3.0/pygoogalytics/data/google_ads_location_ids.csv
+-rw-r--r--   0 joshua     (501) staff       (20)    36784 2023-04-13 07:30:02.000000 pygoogalytics-0.3.0/pygoogalytics/googalytics_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)    32322 2023-02-21 11:27:36.000000 pygoogalytics-0.3.0/pygoogalytics/googlepandas.py
+-rw-r--r--   0 joshua     (501) staff       (20)    42080 2023-04-13 10:54:44.000000 pygoogalytics-0.3.0/pygoogalytics/kwp_wrappers.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2484 2023-04-20 08:33:27.000000 pygoogalytics-0.3.0/pygoogalytics/resource_utils.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2064 2023-02-20 08:31:45.000000 pygoogalytics-0.3.0/pygoogalytics/utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-20 08:36:08.270965 pygoogalytics-0.3.0/pygoogalytics.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-20 08:36:08.000000 pygoogalytics-0.3.0/pygoogalytics.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      512 2023-04-20 08:36:08.000000 pygoogalytics-0.3.0/pygoogalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2023-04-20 08:36:08.000000 pygoogalytics-0.3.0/pygoogalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)      113 2023-04-20 08:36:08.000000 pygoogalytics-0.3.0/pygoogalytics.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       14 2023-04-20 08:36:08.000000 pygoogalytics-0.3.0/pygoogalytics.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2023-04-20 08:36:08.271905 pygoogalytics-0.3.0/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-04-20 08:35:19.000000 pygoogalytics-0.3.0/setup.py
```

### Comparing `pygoogalytics-0.2.8/LICENCE.txt` & `pygoogalytics-0.3.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.8/LICENSE` & `pygoogalytics-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.8/PKG-INFO` & `pygoogalytics-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.2.8
+Version: 0.3.0
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.2.8/README.md` & `pygoogalytics-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.8/pygoogalytics/__init__.py` & `pygoogalytics-0.3.0/pygoogalytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   sc_domain='<search-console-domain>',
   view_id='<ga3-view-id>',
   ga4_property_id='<ga4-property-id>'
 )
 ```
 """
 
-__version__ = "0.2.8"
+__version__ = "0.3.0"
 __author__ = 'Joshua Prettyman'
 __credits__ = 'Blink SEO'
 
 import os
 import csv
 import logging
```

### Comparing `pygoogalytics-0.2.8/pygoogalytics/client.py` & `pygoogalytics-0.3.0/pygoogalytics/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from .resource_utils import resources_from_json, resources_from_key_file, \
+from .resource_utils import get_analytics_resources, \
     googleads_client_from_yaml, googleads_client_from_key_file
 from .googalytics_wrapper import GoogalyticsWrapper
 from .kwp_wrappers import KeywordPlanIdeaService, KeywordPlanService
 from . import pga_logger
 
 
 class GoogalyticsClient:
@@ -14,40 +14,29 @@
 
     example implementation:
     from pygoogalytics.client import Client
     googalytics_client = Client(key_file_path='<path-to-your-key-file>')
     """
 
     def __init__(self,
-                 key_file_path: str = None,
-                 key_file_json: str = None
+                 gsc_resource=None,
+                 ga3_resource=None,
+                 ga4_resource=None
                  ):
 
-        self.gsc_resource = None
-        self.ga3_resource = None
-        self.ga4_resource = None
-
-        if key_file_json:
-            self._build_from_json(json_string=key_file_json)
-            pga_logger.info(f"initialised PyGoogalytics Client object from key file")
-        elif key_file_path:
-            self._build_from_key_file(path=key_file_path)
-            pga_logger.info(f"initialised PyGoogalytics Client object from JSON string")
-
-    def _build_from_json(self, json_string: str):
-        _ga3_resource, _ga4_resource, _gsc_resource = resources_from_json(json_string=json_string)
-        self.gsc_resource = _gsc_resource
-        self.ga3_resource = _ga3_resource
-        self.ga4_resource = _ga4_resource
-
-    def _build_from_key_file(self, path: str):
-        _ga3_resource, _ga4_resource, _gsc_resource = resources_from_key_file(path=path)
-        self.gsc_resource = _gsc_resource
-        self.ga3_resource = _ga3_resource
-        self.ga4_resource = _ga4_resource
+        self.gsc_resource = gsc_resource
+        self.ga3_resource = ga3_resource
+        self.ga4_resource = ga4_resource
+
+    @classmethod
+    def build(cls, api_key: str = None, key_file_path: str = None):
+        _ga3_resource, _ga4_resource, _gsc_resource = get_analytics_resources(
+            json_api_key=api_key, key_file_path=key_file_path
+        )
+        return cls(gsc_resource=_gsc_resource, ga3_resource=_ga3_resource,  ga4_resource=_ga4_resource)
 
     def wrapper(self,
                 sc_domain: str = None,
                 view_id: str = None,
                 ga4_property_id: str = None,
                 ) -> GoogalyticsWrapper:
         """
@@ -140,8 +129,7 @@
             customer_id = self.default_customer_id
 
         return KeywordPlanIdeaService(googleads_client=self.googleads_client,
                                       customer_id=customer_id,
                                       site_url=site_url,
                                       location_codes=location_codes,
                                       language_id=language_id)
-
```

### Comparing `pygoogalytics-0.2.8/pygoogalytics/data/country_iso_codes.csv` & `pygoogalytics-0.3.0/pygoogalytics/data/country_iso_codes.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.8/pygoogalytics/data/google_ads_location_ids.csv` & `pygoogalytics-0.3.0/pygoogalytics/data/google_ads_location_ids.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.8/pygoogalytics/googalytics_wrapper.py` & `pygoogalytics-0.3.0/pygoogalytics/googalytics_wrapper.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.8/pygoogalytics/googlepandas.py` & `pygoogalytics-0.3.0/pygoogalytics/googlepandas.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.8/pygoogalytics/kwp_wrappers.py` & `pygoogalytics-0.3.0/pygoogalytics/kwp_wrappers.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.8/pygoogalytics/resource_utils.py` & `pygoogalytics-0.3.0/pygoogalytics/resource_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,35 +18,34 @@
 def googleads_client_from_yaml(googleads_yaml_string: str) -> Tuple[GoogleAdsClient, str]:
     googleads_yaml_dict = yaml.safe_load(googleads_yaml_string)
     default_customer_id = str(googleads_yaml_dict.get('default_customer_id'))
     googleads_client = GoogleAdsClient.load_from_string(yaml_str=googleads_yaml_string, version="v12")
     return googleads_client, default_customer_id
 
 
-def resources_from_key_file(path: str):
-    with open(path, 'rb') as _file:
-        _json_string = _file.read().decode('utf8')
-    return resources_from_json(json_string=_json_string)
-
-
-def resources_from_json(json_string: str):
-    _secrets = json.loads(json_string)
-    _project_credentials = get_analytics_project_credentials(secrets=_secrets)
-    return get_analytics_resources(analytics_project_credentials=_project_credentials)
+def get_analytics_resources(json_api_key: str = None, key_file_path: str = None):
+    if key_file_path and not json_api_key:
+        with open(path, 'rb') as _file:
+            json_api_key = _file.read().decode('utf8')
+    if json_api_key:
+        project_credentials = get_analytics_project_credentials(secrets=json.loads(json_string))
+    else:
+        project_credentials = None
+    return build_analytics_resources(analytics_project_credentials=project_credentials)
 
 
 def get_analytics_project_credentials(secrets: dict):
     analytics_project_scopes = ['https://www.googleapis.com/auth/analytics.readonly',
                                 'https://www.googleapis.com/auth/webmasters.readonly',
                                 'https://www.googleapis.com/auth/webmasters',
                                 'https://www.googleapis.com/auth/cloud-platform']
 
     project_credentials = service_account.Credentials.from_service_account_info(
         info=secrets).with_scopes(scopes=analytics_project_scopes)
     return project_credentials
 
 
-def get_analytics_resources(analytics_project_credentials):
+def build_analytics_resources(analytics_project_credentials: service_account.Credentials = None):
     ga3_resource = discovery.build('analyticsreporting', 'v4', credentials=analytics_project_credentials)
     gsc_resource = discovery.build('searchconsole', 'v1', credentials=analytics_project_credentials)
     ga4_data_client = BetaAnalyticsDataClient(credentials=analytics_project_credentials)
     return ga3_resource, ga4_data_client, gsc_resource
```

### Comparing `pygoogalytics-0.2.8/pygoogalytics/utils.py` & `pygoogalytics-0.3.0/pygoogalytics/utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.8/pygoogalytics.egg-info/PKG-INFO` & `pygoogalytics-0.3.0/pygoogalytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.2.8
+Version: 0.3.0
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.2.8/pygoogalytics.egg-info/SOURCES.txt` & `pygoogalytics-0.3.0/pygoogalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.8/setup.py` & `pygoogalytics-0.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # twine upload dist/*
 
 _desc = """PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 in the form of a pandas dataframe."""
 
 setup(
     name='pygoogalytics',
-    version='0.2.8',
+    version='0.3.0',
     description=_desc,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Blink-SEO/pygoogalytics',
     author='Joshua Prettyman',
     author_email='joshua@blinkseo.co.uk',
     license='MIT',
```

