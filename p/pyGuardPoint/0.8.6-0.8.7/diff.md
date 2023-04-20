# Comparing `tmp/pyGuardPoint-0.8.6.tar.gz` & `tmp/pyGuardPoint-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.8.6.tar", last modified: Thu Apr 20 11:52:10 2023, max compression
+gzip compressed data, was "pyGuardPoint-0.8.7.tar", last modified: Thu Apr 20 13:12:17 2023, max compression
```

## Comparing `pyGuardPoint-0.8.6.tar` & `pyGuardPoint-0.8.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 11:52:10.518737 pyGuardPoint-0.8.6/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.8.6/LICENSE.txt
--rw-rw-rw-   0        0        0     5739 2023-04-20 11:52:10.517738 pyGuardPoint-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0     5480 2023-04-14 14:00:11.000000 pyGuardPoint-0.8.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-20 11:52:10.504847 pyGuardPoint-0.8.6/pyGuardPoint/
--rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.8.6/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11213 2023-04-13 12:36:08.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5586 2023-04-20 11:51:01.000000 pyGuardPoint-0.8.6/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.8.6/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.8.6/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-20 11:52:10.516739 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0     5739 2023-04-20 11:52:10.000000 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2023-04-20 11:52:10.000000 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 11:52:10.000000 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-20 11:52:10.000000 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-20 11:52:10.000000 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 11:52:10.518737 pyGuardPoint-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0      549 2023-04-20 11:49:49.000000 pyGuardPoint-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 13:12:17.480475 pyGuardPoint-0.8.7/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.8.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     5739 2023-04-20 13:12:17.480475 pyGuardPoint-0.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5480 2023-04-14 14:00:11.000000 pyGuardPoint-0.8.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-20 13:12:17.462477 pyGuardPoint-0.8.7/pyGuardPoint/
+-rw-rw-rw-   0        0        0      266 2023-04-20 12:58:39.000000 pyGuardPoint-0.8.7/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    11213 2023-04-13 12:36:08.000000 pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     1083 2023-04-20 13:02:16.000000 pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_cardholdertypes.py
+-rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5586 2023-04-20 11:51:01.000000 pyGuardPoint-0.8.7/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.8.7/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2474 2023-04-20 13:02:16.000000 pyGuardPoint-0.8.7/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.8.7/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.8.7/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    17298 2023-04-20 13:03:22.000000 pyGuardPoint-0.8.7/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.8.7/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.8.7/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-20 13:12:17.479489 pyGuardPoint-0.8.7/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0     5739 2023-04-20 13:12:17.000000 pyGuardPoint-0.8.7/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2023-04-20 13:12:17.000000 pyGuardPoint-0.8.7/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 13:12:17.000000 pyGuardPoint-0.8.7/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.8.7/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-04-20 13:12:17.000000 pyGuardPoint-0.8.7/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-20 13:12:17.000000 pyGuardPoint-0.8.7/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 13:12:17.481481 pyGuardPoint-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0      549 2023-04-20 13:11:49.000000 pyGuardPoint-0.8.7/setup.py
```

### Comparing `pyGuardPoint-0.8.6/LICENSE.txt` & `pyGuardPoint-0.8.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/PKG-INFO` & `pyGuardPoint-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.8.6
+Version: 0.8.7
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-0.8.6/README.rst` & `pyGuardPoint-0.8.7/README.rst`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-0.8.7/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-0.8.7/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-0.8.7/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/guardpoint.py` & `pyGuardPoint-0.8.7/pyGuardPoint/guardpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 
+from ._guardpoint_cardholdertypes import CardholderTypesAPI
 from ._guardpoint_scheduledmags import ScheduledMagsAPI
 from ._guardpoint_customizedfields import CustomizedFieldsAPI
 from ._guardpoint_personaldetails import PersonalDetailsAPI
 from ._guardpoint_securitygroups import SecurityGroupsAPI
 from .guardpoint_connection import GuardPointConnection, GuardPointAuthType
 from ._guardpoint_cards import CardsAPI
 from ._guardpoint_cardholders import CardholdersAPI
@@ -11,15 +12,15 @@
 from ._guardpoint_areas import AreasAPI
 from .guardpoint_utils import url_parser
 
 log = logging.getLogger(__name__)
 
 
 class GuardPoint(GuardPointConnection, CardsAPI, CardholdersAPI, AreasAPI, SecurityGroupsAPI,
-                 CustomizedFieldsAPI, PersonalDetailsAPI, ScheduledMagsAPI):
+                 CustomizedFieldsAPI, PersonalDetailsAPI, ScheduledMagsAPI, CardholderTypesAPI):
 
     def __init__(self, **kwargs):
         # Set default values if not present
         host = kwargs.get('host', "localhost")
         port = kwargs.get('port', None)
         url_components = url_parser(host)
         if url_components['host'] == '':
```

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-0.8.7/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-0.8.7/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-0.8.7/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,20 +298,24 @@
             if key not in self.changed_attributes:
                 ch.pop(key)
         return ch
 
 
 @dataclass
 class CardholderType:
+    uid: str
     typeName: str
+    defaultBPTemplate: str
+    def __init__(self, cardholder_type_dict: dict):
+        for property_name in cardholder_type_dict:
+            if isinstance(cardholder_type_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, cardholder_type_dict[property_name])
 
     def dict(self):
         return {k: str(v) for k, v in asdict(self).items()}
-
-
 @dataclass
 class Cardholder(Observable):
     uid: str = ""
     lastName: str = ""
     firstName: str = ""
     cardholderIdNumber: any = None
     status: any = None
```

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-0.8.7/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint.egg-info/PKG-INFO` & `pyGuardPoint-0.8.7/pyGuardPoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.8.6
+Version: 0.8.7
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-0.8.6/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-0.8.7/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.txt
 README.rst
 setup.py
 pyGuardPoint/__init__.py
 pyGuardPoint/_guardpoint_areas.py
 pyGuardPoint/_guardpoint_cardholders.py
+pyGuardPoint/_guardpoint_cardholdertypes.py
 pyGuardPoint/_guardpoint_cards.py
 pyGuardPoint/_guardpoint_customizedfields.py
 pyGuardPoint/_guardpoint_personaldetails.py
 pyGuardPoint/_guardpoint_scheduledmags.py
 pyGuardPoint/_guardpoint_securitygroups.py
 pyGuardPoint/_odata_filter.py
 pyGuardPoint/_str_match_algo.py
```

### Comparing `pyGuardPoint-0.8.6/setup.py` & `pyGuardPoint-0.8.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
-      version="0.8.6",
+      version="0.8.7",
       author="John Owen",
       description="Python wrapper for GuardPoint 10 Access Control System",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
       install_requires=['validators', 'fuzzywuzzy', 'Levenshtein'],
       packages=['pyGuardPoint'],
```

