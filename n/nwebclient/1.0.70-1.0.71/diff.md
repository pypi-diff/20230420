# Comparing `tmp/nwebclient-1.0.70.tar.gz` & `tmp/nwebclient-1.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.70.tar", last modified: Thu Apr 20 09:37:50 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.71.tar", last modified: Thu Apr 20 09:43:35 2023, max compression
```

## Comparing `nwebclient-1.0.70.tar` & `nwebclient-1.0.71.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 09:37:50.789594 nwebclient-1.0.70/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.70/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 09:37:50.789594 nwebclient-1.0.70/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.70/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 09:37:50.789594 nwebclient-1.0.70/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.70/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.70/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3104 2023-03-29 20:50:31.000000 nwebclient-1.0.70/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7262 2023-04-20 09:36:53.000000 nwebclient-1.0.70/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5582 2023-03-29 09:33:58.000000 nwebclient-1.0.70/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3218 2023-03-27 16:42:32.000000 nwebclient-1.0.70/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 09:37:50.789594 nwebclient-1.0.70/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 09:37:50.000000 nwebclient-1.0.70/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-20 09:37:50.000000 nwebclient-1.0.70/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-20 09:37:50.000000 nwebclient-1.0.70/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       84 2023-04-20 09:37:50.000000 nwebclient-1.0.70/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-20 09:37:50.000000 nwebclient-1.0.70/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-20 09:37:50.000000 nwebclient-1.0.70/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-20 09:37:50.789594 nwebclient-1.0.70/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      829 2023-04-20 09:37:46.000000 nwebclient-1.0.70/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 09:43:35.053888 nwebclient-1.0.71/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.71/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 09:43:35.053888 nwebclient-1.0.71/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.71/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 09:43:35.053888 nwebclient-1.0.71/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.71/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.71/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3104 2023-03-29 20:50:31.000000 nwebclient-1.0.71/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7262 2023-04-20 09:43:18.000000 nwebclient-1.0.71/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5582 2023-03-29 09:33:58.000000 nwebclient-1.0.71/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3218 2023-03-27 16:42:32.000000 nwebclient-1.0.71/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-20 09:43:35.053888 nwebclient-1.0.71/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-20 09:43:34.000000 nwebclient-1.0.71/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-20 09:43:34.000000 nwebclient-1.0.71/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-20 09:43:34.000000 nwebclient-1.0.71/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       84 2023-04-20 09:43:34.000000 nwebclient-1.0.71/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-20 09:43:34.000000 nwebclient-1.0.71/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-20 09:43:34.000000 nwebclient-1.0.71/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-20 09:43:35.053888 nwebclient-1.0.71/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      829 2023-04-20 09:43:30.000000 nwebclient-1.0.71/setup.py
```

### Comparing `nwebclient-1.0.70/LICENSE` & `nwebclient-1.0.71/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.70/PKG-INFO` & `nwebclient-1.0.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.70
+Version: 1.0.71
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.70/README.md` & `nwebclient-1.0.71/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.70/nwebclient/__init__.py` & `nwebclient-1.0.71/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.70/nwebclient/__main__.py` & `nwebclient-1.0.71/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.70/nwebclient/crypt.py` & `nwebclient-1.0.71/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.70/nwebclient/sd.py` & `nwebclient-1.0.71/nwebclient/sd.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.70/nwebclient/sdb.py` & `nwebclient-1.0.71/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.70/nwebclient/ticker.py` & `nwebclient-1.0.71/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.70/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.71/nwebclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.70
+Version: 1.0.71
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.70/setup.py` & `nwebclient-1.0.71/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.70",
+    version="1.0.71",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

