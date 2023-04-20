# Comparing `tmp/opendatacrawler-1.0.5.tar.gz` & `tmp/opendatacrawler-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendatacrawler-1.0.5.tar", last modified: Thu Apr 20 15:15:47 2023, max compression
+gzip compressed data, was "opendatacrawler-1.0.6.tar", last modified: Thu Apr 20 15:17:29 2023, max compression
```

## Comparing `opendatacrawler-1.0.5.tar` & `opendatacrawler-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:15:47.984380 opendatacrawler-1.0.5/
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1070 2023-02-03 16:41:45.000000 opendatacrawler-1.0.5/LICENSE
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:15:47.982351 opendatacrawler-1.0.5/PKG-INFO
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7205 2023-03-08 15:49:21.000000 opendatacrawler-1.0.5/README.md
-drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:15:47.954681 opendatacrawler-1.0.5/opendatacrawler/
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4613 2023-04-20 15:15:12.000000 opendatacrawler-1.0.5/opendatacrawler/CkanCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3936 2023-03-28 15:04:53.000000 opendatacrawler-1.0.5/opendatacrawler/INECrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4648 2023-04-20 15:13:59.000000 opendatacrawler-1.0.5/opendatacrawler/OpenDataSoftCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1935 2023-04-20 15:14:34.000000 opendatacrawler-1.0.5/opendatacrawler/SocrataCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3196 2023-02-03 16:41:45.000000 opendatacrawler-1.0.5/opendatacrawler/ZenodoCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       95 2023-04-20 15:15:35.000000 opendatacrawler-1.0.5/opendatacrawler/__init__.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9194 2023-04-20 15:13:21.000000 opendatacrawler-1.0.5/opendatacrawler/__main__.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     6212 2023-03-29 09:05:49.000000 opendatacrawler-1.0.5/opendatacrawler/datosgobescrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3099 2023-02-03 16:41:45.000000 opendatacrawler-1.0.5/opendatacrawler/eurostatcrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9661 2023-04-20 15:13:47.000000 opendatacrawler-1.0.5/opendatacrawler/odcrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1938 2023-03-16 09:49:44.000000 opendatacrawler-1.0.5/opendatacrawler/opendatacrawlerInterface.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      881 2023-02-03 16:41:45.000000 opendatacrawler-1.0.5/opendatacrawler/setup_logger.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     5119 2023-04-20 15:11:35.000000 opendatacrawler-1.0.5/opendatacrawler/utils.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     2480 2023-04-20 15:14:50.000000 opendatacrawler-1.0.5/opendatacrawler/worldbankcrawler.py
-drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:15:47.981177 opendatacrawler-1.0.5/opendatacrawler.egg-info/
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:15:47.000000 opendatacrawler-1.0.5/opendatacrawler.egg-info/PKG-INFO
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      723 2023-04-20 15:15:47.000000 opendatacrawler-1.0.5/opendatacrawler.egg-info/SOURCES.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)        1 2023-04-20 15:15:47.000000 opendatacrawler-1.0.5/opendatacrawler.egg-info/dependency_links.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       58 2023-04-20 15:15:47.000000 opendatacrawler-1.0.5/opendatacrawler.egg-info/entry_points.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       12 2023-04-20 15:15:47.000000 opendatacrawler-1.0.5/opendatacrawler.egg-info/requires.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       16 2023-04-20 15:15:47.000000 opendatacrawler-1.0.5/opendatacrawler.egg-info/top_level.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       38 2023-04-20 15:15:47.984464 opendatacrawler-1.0.5/setup.cfg
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      988 2023-04-20 15:15:38.000000 opendatacrawler-1.0.5/setup.py
+drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:17:29.744357 opendatacrawler-1.0.6/
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1070 2023-02-03 16:41:45.000000 opendatacrawler-1.0.6/LICENSE
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:17:29.743696 opendatacrawler-1.0.6/PKG-INFO
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7205 2023-03-08 15:49:21.000000 opendatacrawler-1.0.6/README.md
+drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:17:29.714578 opendatacrawler-1.0.6/opendatacrawler/
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4613 2023-04-20 15:15:12.000000 opendatacrawler-1.0.6/opendatacrawler/CkanCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3936 2023-03-28 15:04:53.000000 opendatacrawler-1.0.6/opendatacrawler/INECrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4648 2023-04-20 15:13:59.000000 opendatacrawler-1.0.6/opendatacrawler/OpenDataSoftCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1935 2023-04-20 15:14:34.000000 opendatacrawler-1.0.6/opendatacrawler/SocrataCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3196 2023-02-03 16:41:45.000000 opendatacrawler-1.0.6/opendatacrawler/ZenodoCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       95 2023-04-20 15:17:05.000000 opendatacrawler-1.0.6/opendatacrawler/__init__.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9194 2023-04-20 15:13:21.000000 opendatacrawler-1.0.6/opendatacrawler/__main__.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     6212 2023-03-29 09:05:49.000000 opendatacrawler-1.0.6/opendatacrawler/datosgobescrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3099 2023-02-03 16:41:45.000000 opendatacrawler-1.0.6/opendatacrawler/eurostatcrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9669 2023-04-20 15:16:58.000000 opendatacrawler-1.0.6/opendatacrawler/odcrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1938 2023-03-16 09:49:44.000000 opendatacrawler-1.0.6/opendatacrawler/opendatacrawlerInterface.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      881 2023-02-03 16:41:45.000000 opendatacrawler-1.0.6/opendatacrawler/setup_logger.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     5119 2023-04-20 15:11:35.000000 opendatacrawler-1.0.6/opendatacrawler/utils.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     2480 2023-04-20 15:14:50.000000 opendatacrawler-1.0.6/opendatacrawler/worldbankcrawler.py
+drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:17:29.742718 opendatacrawler-1.0.6/opendatacrawler.egg-info/
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:17:29.000000 opendatacrawler-1.0.6/opendatacrawler.egg-info/PKG-INFO
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      723 2023-04-20 15:17:29.000000 opendatacrawler-1.0.6/opendatacrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)        1 2023-04-20 15:17:29.000000 opendatacrawler-1.0.6/opendatacrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       58 2023-04-20 15:17:29.000000 opendatacrawler-1.0.6/opendatacrawler.egg-info/entry_points.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       12 2023-04-20 15:17:29.000000 opendatacrawler-1.0.6/opendatacrawler.egg-info/requires.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       16 2023-04-20 15:17:29.000000 opendatacrawler-1.0.6/opendatacrawler.egg-info/top_level.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       38 2023-04-20 15:17:29.744422 opendatacrawler-1.0.6/setup.cfg
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      988 2023-04-20 15:17:09.000000 opendatacrawler-1.0.6/setup.py
```

### Comparing `opendatacrawler-1.0.5/LICENSE` & `opendatacrawler-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/PKG-INFO` & `opendatacrawler-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendatacrawler
-Version: 1.0.5
+Version: 1.0.6
 Summary: Crawler for open data portals
 Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor
 Author-email: alberto.berenguer@ua.es
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.5 Summary: Crawler for
+Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.6 Summary: Crawler for
 open data portals Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor Author-email: alberto.berenguer@ua.es License:
 MIT Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
```

### Comparing `opendatacrawler-1.0.5/README.md` & `opendatacrawler-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler/CkanCrawler.py` & `opendatacrawler-1.0.6/opendatacrawler/CkanCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler/INECrawler.py` & `opendatacrawler-1.0.6/opendatacrawler/INECrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler/OpenDataSoftCrawler.py` & `opendatacrawler-1.0.6/opendatacrawler/OpenDataSoftCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler/SocrataCrawler.py` & `opendatacrawler-1.0.6/opendatacrawler/SocrataCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler/ZenodoCrawler.py` & `opendatacrawler-1.0.6/opendatacrawler/ZenodoCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler/__main__.py` & `opendatacrawler-1.0.6/opendatacrawler/__main__.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler/datosgobescrawler.py` & `opendatacrawler-1.0.6/opendatacrawler/datosgobescrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler/eurostatcrawler.py` & `opendatacrawler-1.0.6/opendatacrawler/eurostatcrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler/odcrawler.py` & `opendatacrawler-1.0.6/opendatacrawler/odcrawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 import urllib3
 import json
-import utils
+from .utils import *
 import re
 import os
 from .SocrataCrawler import SocrataCrawler
 from .CkanCrawler import CkanCrawler
 from .worldbankcrawler import WorldBankCrawler
 from .eurostatcrawler import EurostatCrawler
 from .datosgobescrawler import datosGobEsCrawler
```

### Comparing `opendatacrawler-1.0.5/opendatacrawler/opendatacrawlerInterface.py` & `opendatacrawler-1.0.6/opendatacrawler/opendatacrawlerInterface.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler/setup_logger.py` & `opendatacrawler-1.0.6/opendatacrawler/setup_logger.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler/utils.py` & `opendatacrawler-1.0.6/opendatacrawler/utils.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler/worldbankcrawler.py` & `opendatacrawler-1.0.6/opendatacrawler/worldbankcrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/opendatacrawler.egg-info/PKG-INFO` & `opendatacrawler-1.0.6/opendatacrawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendatacrawler
-Version: 1.0.5
+Version: 1.0.6
 Summary: Crawler for open data portals
 Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor
 Author-email: alberto.berenguer@ua.es
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.5 Summary: Crawler for
+Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.6 Summary: Crawler for
 open data portals Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor Author-email: alberto.berenguer@ua.es License:
 MIT Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
```

### Comparing `opendatacrawler-1.0.5/opendatacrawler.egg-info/SOURCES.txt` & `opendatacrawler-1.0.6/opendatacrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.5/setup.py` & `opendatacrawler-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="opendatacrawler",
-    version="1.0.5",
+    version="1.0.6",
     description="Crawler for open data portals",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/aberenguerpas/OpenDataCrawler/",
     author="Alberto Berenguer Pastor",
     author_email="alberto.berenguer@ua.es",
     license="MIT",
```

