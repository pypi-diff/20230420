# Comparing `tmp/pyGuardPoint-0.8.5.tar.gz` & `tmp/pyGuardPoint-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.8.5.tar", last modified: Fri Apr 14 14:00:54 2023, max compression
+gzip compressed data, was "pyGuardPoint-0.8.6.tar", last modified: Thu Apr 20 11:52:10 2023, max compression
```

## Comparing `pyGuardPoint-0.8.5.tar` & `pyGuardPoint-0.8.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 14:00:54.819346 pyGuardPoint-0.8.5/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.8.5/LICENSE.txt
--rw-rw-rw-   0        0        0     5743 2023-04-14 14:00:54.819346 pyGuardPoint-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     5480 2023-04-14 14:00:11.000000 pyGuardPoint-0.8.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-14 14:00:54.810320 pyGuardPoint-0.8.5/pyGuardPoint/
--rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.8.5/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11213 2023-04-13 12:36:08.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5306 2023-04-13 10:30:08.000000 pyGuardPoint-0.8.5/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.8.5/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.8.5/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:00:54.818328 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0     5743 2023-04-14 14:00:54.000000 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2023-04-14 14:00:54.000000 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 14:00:54.000000 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-14 14:00:54.000000 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-14 14:00:54.000000 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 14:00:54.820320 pyGuardPoint-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-04-14 14:00:27.000000 pyGuardPoint-0.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:52:10.518737 pyGuardPoint-0.8.6/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.8.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     5739 2023-04-20 11:52:10.517738 pyGuardPoint-0.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5480 2023-04-14 14:00:11.000000 pyGuardPoint-0.8.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-20 11:52:10.504847 pyGuardPoint-0.8.6/pyGuardPoint/
+-rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.8.6/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    11213 2023-04-13 12:36:08.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5586 2023-04-20 11:51:01.000000 pyGuardPoint-0.8.6/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.8.6/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.8.6/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:52:10.516739 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0     5739 2023-04-20 11:52:10.000000 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-04-20 11:52:10.000000 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 11:52:10.000000 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-04-20 11:52:10.000000 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-20 11:52:10.000000 pyGuardPoint-0.8.6/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 11:52:10.518737 pyGuardPoint-0.8.6/setup.cfg
+-rw-rw-rw-   0        0        0      549 2023-04-20 11:49:49.000000 pyGuardPoint-0.8.6/setup.py
```

### Comparing `pyGuardPoint-0.8.5/LICENSE.txt` & `pyGuardPoint-0.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/PKG-INFO` & `pyGuardPoint-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.8.5
-Summary: Easy-to-use Python module implementing GuardPoint's WebAPI
+Version: 0.8.6
+Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
 ===============
```

### Comparing `pyGuardPoint-0.8.5/README.rst` & `pyGuardPoint-0.8.6/README.rst`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-0.8.6/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-0.8.6/pyGuardPoint/_odata_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from datetime import datetime
+
+import validators
+
 from .guardpoint_dataclasses import Area, Cardholder, CardholderPersonalDetail
 from urllib.parse import quote
 
 
 def _compose_expand(ignore_list, include_list):
     expand_attribs = ['cardholderType', 'cards', 'cardholderPersonalDetail', 'cardholderCustomizedField', 'insideArea',
                       'securityGroup']
@@ -75,17 +78,22 @@
                     filter_expired=False,
                     earliest_last_pass=None,
                     exact_match=None):
     filter_phrases = []
 
     if exact_match:
         if isinstance(exact_match, dict):
-            for k,v in exact_match.items():
-                if isinstance(v, (str, bool, int)):
-                    filter_phrases.append(f"({k}%20eq%20'{quote(v)}')")
+            for k, v in exact_match.items():
+                if isinstance(v, str):
+                    if validators.uuid(v):
+                        filter_phrases.append(f"({k}%20eq%20{quote(v)})")
+                    else:
+                        filter_phrases.append(f"({k}%20eq%20'{quote(v)}')")
+                if isinstance(v, (bool, int)):
+                    filter_phrases.append(f"({k}%20eq%20{quote(v)})")
                 if k == "cardholderPersonalDetail" and v.__class__.__name__ == "CardholderPersonalDetail":
                     details = v.dict(changed_only=True)
                     for dk, dv in details.items():
                         filter_phrases.append(f"(CardholderPersonalDetail/{dk}%20eq%20'{quote(dv)}')")
 
     if earliest_last_pass:
         if isinstance(earliest_last_pass, datetime):
```

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-0.8.6/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/guardpoint.py` & `pyGuardPoint-0.8.6/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-0.8.6/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint.egg-info/PKG-INFO` & `pyGuardPoint-0.8.6/pyGuardPoint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.8.5
-Summary: Easy-to-use Python module implementing GuardPoint's WebAPI
+Version: 0.8.6
+Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
 ===============
```

### Comparing `pyGuardPoint-0.8.5/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-0.8.6/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.5/setup.py` & `pyGuardPoint-0.8.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
-      version="0.8.5",
+      version="0.8.6",
       author="John Owen",
-      description="Easy-to-use Python module implementing GuardPoint's WebAPI",
+      description="Python wrapper for GuardPoint 10 Access Control System",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
       install_requires=['validators', 'fuzzywuzzy', 'Levenshtein'],
       packages=['pyGuardPoint'],
       license_files=('LICENSE.txt',),
       zip_safe=False)
```

