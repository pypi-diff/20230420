# Comparing `tmp/opendatacrawler-1.0.3.tar.gz` & `tmp/opendatacrawler-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendatacrawler-1.0.3.tar", last modified: Thu Apr 20 15:07:26 2023, max compression
+gzip compressed data, was "opendatacrawler-1.0.4.tar", last modified: Thu Apr 20 15:12:06 2023, max compression
```

## Comparing `opendatacrawler-1.0.3.tar` & `opendatacrawler-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:07:26.833624 opendatacrawler-1.0.3/
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1070 2023-02-03 16:41:45.000000 opendatacrawler-1.0.3/LICENSE
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:07:26.832976 opendatacrawler-1.0.3/PKG-INFO
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7205 2023-03-08 15:49:21.000000 opendatacrawler-1.0.3/README.md
-drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:07:26.798674 opendatacrawler-1.0.3/opendatacrawler/
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4603 2023-03-29 09:05:49.000000 opendatacrawler-1.0.3/opendatacrawler/CkanCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3936 2023-03-28 15:04:53.000000 opendatacrawler-1.0.3/opendatacrawler/INECrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4646 2023-03-28 15:04:53.000000 opendatacrawler-1.0.3/opendatacrawler/OpenDataSoftCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1943 2023-02-03 16:41:45.000000 opendatacrawler-1.0.3/opendatacrawler/SocrataCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3196 2023-02-03 16:41:45.000000 opendatacrawler-1.0.3/opendatacrawler/ZenodoCrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       95 2023-04-20 14:41:14.000000 opendatacrawler-1.0.3/opendatacrawler/__init__.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9192 2023-04-20 15:06:16.000000 opendatacrawler-1.0.3/opendatacrawler/__main__.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     6212 2023-03-29 09:05:49.000000 opendatacrawler-1.0.3/opendatacrawler/datosgobescrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3099 2023-02-03 16:41:45.000000 opendatacrawler-1.0.3/opendatacrawler/eurostatcrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9652 2023-03-29 09:05:49.000000 opendatacrawler-1.0.3/opendatacrawler/odcrawler.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1938 2023-03-16 09:49:44.000000 opendatacrawler-1.0.3/opendatacrawler/opendatacrawlerInterface.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      881 2023-02-03 16:41:45.000000 opendatacrawler-1.0.3/opendatacrawler/setup_logger.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     5118 2023-03-29 09:05:49.000000 opendatacrawler-1.0.3/opendatacrawler/utils.py
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     2470 2023-02-03 16:41:45.000000 opendatacrawler-1.0.3/opendatacrawler/worldbankcrawler.py
-drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:07:26.831939 opendatacrawler-1.0.3/opendatacrawler.egg-info/
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:07:26.000000 opendatacrawler-1.0.3/opendatacrawler.egg-info/PKG-INFO
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      723 2023-04-20 15:07:26.000000 opendatacrawler-1.0.3/opendatacrawler.egg-info/SOURCES.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)        1 2023-04-20 15:07:26.000000 opendatacrawler-1.0.3/opendatacrawler.egg-info/dependency_links.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       58 2023-04-20 15:07:26.000000 opendatacrawler-1.0.3/opendatacrawler.egg-info/entry_points.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       12 2023-04-20 15:07:26.000000 opendatacrawler-1.0.3/opendatacrawler.egg-info/requires.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       16 2023-04-20 15:07:26.000000 opendatacrawler-1.0.3/opendatacrawler.egg-info/top_level.txt
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       38 2023-04-20 15:07:26.833708 opendatacrawler-1.0.3/setup.cfg
--rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      988 2023-04-20 15:07:23.000000 opendatacrawler-1.0.3/setup.py
+drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:12:06.305585 opendatacrawler-1.0.4/
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1070 2023-02-03 16:41:45.000000 opendatacrawler-1.0.4/LICENSE
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:12:06.304900 opendatacrawler-1.0.4/PKG-INFO
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7205 2023-03-08 15:49:21.000000 opendatacrawler-1.0.4/README.md
+drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:12:06.284780 opendatacrawler-1.0.4/opendatacrawler/
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4603 2023-03-29 09:05:49.000000 opendatacrawler-1.0.4/opendatacrawler/CkanCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3936 2023-03-28 15:04:53.000000 opendatacrawler-1.0.4/opendatacrawler/INECrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     4646 2023-03-28 15:04:53.000000 opendatacrawler-1.0.4/opendatacrawler/OpenDataSoftCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1943 2023-02-03 16:41:45.000000 opendatacrawler-1.0.4/opendatacrawler/SocrataCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3196 2023-02-03 16:41:45.000000 opendatacrawler-1.0.4/opendatacrawler/ZenodoCrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       95 2023-04-20 15:11:54.000000 opendatacrawler-1.0.4/opendatacrawler/__init__.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9192 2023-04-20 15:06:16.000000 opendatacrawler-1.0.4/opendatacrawler/__main__.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     6212 2023-03-29 09:05:49.000000 opendatacrawler-1.0.4/opendatacrawler/datosgobescrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     3099 2023-02-03 16:41:45.000000 opendatacrawler-1.0.4/opendatacrawler/eurostatcrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     9652 2023-03-29 09:05:49.000000 opendatacrawler-1.0.4/opendatacrawler/odcrawler.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     1938 2023-03-16 09:49:44.000000 opendatacrawler-1.0.4/opendatacrawler/opendatacrawlerInterface.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      881 2023-02-03 16:41:45.000000 opendatacrawler-1.0.4/opendatacrawler/setup_logger.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     5119 2023-04-20 15:11:35.000000 opendatacrawler-1.0.4/opendatacrawler/utils.py
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     2470 2023-02-03 16:41:45.000000 opendatacrawler-1.0.4/opendatacrawler/worldbankcrawler.py
+drwxr-xr-x   0 albertoberenguerpastor   (501) staff       (20)        0 2023-04-20 15:12:06.304167 opendatacrawler-1.0.4/opendatacrawler.egg-info/
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)     7660 2023-04-20 15:12:06.000000 opendatacrawler-1.0.4/opendatacrawler.egg-info/PKG-INFO
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      723 2023-04-20 15:12:06.000000 opendatacrawler-1.0.4/opendatacrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)        1 2023-04-20 15:12:06.000000 opendatacrawler-1.0.4/opendatacrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       58 2023-04-20 15:12:06.000000 opendatacrawler-1.0.4/opendatacrawler.egg-info/entry_points.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       12 2023-04-20 15:12:06.000000 opendatacrawler-1.0.4/opendatacrawler.egg-info/requires.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       16 2023-04-20 15:12:06.000000 opendatacrawler-1.0.4/opendatacrawler.egg-info/top_level.txt
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)       38 2023-04-20 15:12:06.305830 opendatacrawler-1.0.4/setup.cfg
+-rw-r--r--   0 albertoberenguerpastor   (501) staff       (20)      988 2023-04-20 15:12:00.000000 opendatacrawler-1.0.4/setup.py
```

### Comparing `opendatacrawler-1.0.3/LICENSE` & `opendatacrawler-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/PKG-INFO` & `opendatacrawler-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendatacrawler
-Version: 1.0.3
+Version: 1.0.4
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
-Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.3 Summary: Crawler for
+Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.4 Summary: Crawler for
 open data portals Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor Author-email: alberto.berenguer@ua.es License:
 MIT Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
```

### Comparing `opendatacrawler-1.0.3/README.md` & `opendatacrawler-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler/CkanCrawler.py` & `opendatacrawler-1.0.4/opendatacrawler/CkanCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler/INECrawler.py` & `opendatacrawler-1.0.4/opendatacrawler/INECrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler/OpenDataSoftCrawler.py` & `opendatacrawler-1.0.4/opendatacrawler/OpenDataSoftCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler/SocrataCrawler.py` & `opendatacrawler-1.0.4/opendatacrawler/SocrataCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler/ZenodoCrawler.py` & `opendatacrawler-1.0.4/opendatacrawler/ZenodoCrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler/__main__.py` & `opendatacrawler-1.0.4/opendatacrawler/__main__.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler/datosgobescrawler.py` & `opendatacrawler-1.0.4/opendatacrawler/datosgobescrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler/eurostatcrawler.py` & `opendatacrawler-1.0.4/opendatacrawler/eurostatcrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler/odcrawler.py` & `opendatacrawler-1.0.4/opendatacrawler/odcrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler/opendatacrawlerInterface.py` & `opendatacrawler-1.0.4/opendatacrawler/opendatacrawlerInterface.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler/setup_logger.py` & `opendatacrawler-1.0.4/opendatacrawler/setup_logger.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler/utils.py` & `opendatacrawler-1.0.4/opendatacrawler/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 import json
 import requests
 import traceback
 import hashlib
 from w3lib.url import url_query_cleaner
 from url_normalize import url_normalize
-from setup_logger import logger
+from .setup_logger import logger
 
 timer = 0
 # Funtions to control a timer for ZenodoCrawler calls to the API
 def timer_start():
     global timer
     # Starts if == 0, else it continues
     if timer == 0:
```

### Comparing `opendatacrawler-1.0.3/opendatacrawler/worldbankcrawler.py` & `opendatacrawler-1.0.4/opendatacrawler/worldbankcrawler.py`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/opendatacrawler.egg-info/PKG-INFO` & `opendatacrawler-1.0.4/opendatacrawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendatacrawler
-Version: 1.0.3
+Version: 1.0.4
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
-Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.3 Summary: Crawler for
+Metadata-Version: 2.1 Name: opendatacrawler Version: 1.0.4 Summary: Crawler for
 open data portals Home-page: https://github.com/aberenguerpas/OpenDataCrawler/
 Author: Alberto Berenguer Pastor Author-email: alberto.berenguer@ua.es License:
 MIT Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
```

### Comparing `opendatacrawler-1.0.3/opendatacrawler.egg-info/SOURCES.txt` & `opendatacrawler-1.0.4/opendatacrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opendatacrawler-1.0.3/setup.py` & `opendatacrawler-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="opendatacrawler",
-    version="1.0.3",
+    version="1.0.4",
     description="Crawler for open data portals",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/aberenguerpas/OpenDataCrawler/",
     author="Alberto Berenguer Pastor",
     author_email="alberto.berenguer@ua.es",
     license="MIT",
```

