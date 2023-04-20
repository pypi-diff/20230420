# Comparing `tmp/lucidtech-las-8.8.0.tar.gz` & `tmp/lucidtech-las-8.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucidtech-las-8.8.0.tar", last modified: Mon Feb 27 12:31:50 2023, max compression
+gzip compressed data, was "lucidtech-las-8.9.0.tar", last modified: Wed Mar  1 15:24:39 2023, max compression
```

## Comparing `lucidtech-las-8.8.0.tar` & `lucidtech-las-8.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:31:50.463681 lucidtech-las-8.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-02-27 12:31:40.000000 lucidtech-las-8.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-27 12:31:40.000000 lucidtech-las-8.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-02-27 12:31:50.463681 lucidtech-las-8.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-02-27 12:31:40.000000 lucidtech-las-8.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:31:50.463681 lucidtech-las-8.8.0/las/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-02-27 12:31:40.000000 lucidtech-las-8.8.0/las/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-27 12:31:40.000000 lucidtech-las-8.8.0/las/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    96232 2023-02-27 12:31:40.000000 lucidtech-las-8.8.0/las/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-02-27 12:31:40.000000 lucidtech-las-8.8.0/las/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:31:50.463681 lucidtech-las-8.8.0/lucidtech_las.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-02-27 12:31:50.000000 lucidtech-las-8.8.0/lucidtech_las.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-27 12:31:50.000000 lucidtech-las-8.8.0/lucidtech_las.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 12:31:50.000000 lucidtech-las-8.8.0/lucidtech_las.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-27 12:31:50.000000 lucidtech-las-8.8.0/lucidtech_las.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-27 12:31:50.000000 lucidtech-las-8.8.0/lucidtech_las.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-27 12:31:40.000000 lucidtech-las-8.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-27 12:31:50.463681 lucidtech-las-8.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-02-27 12:31:40.000000 lucidtech-las-8.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:24:39.788257 lucidtech-las-8.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-01 15:24:39.788257 lucidtech-las-8.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:24:39.784257 lucidtech-las-8.9.0/las/
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/las/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/las/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96232 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/las/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/las/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:24:39.788257 lucidtech-las-8.9.0/lucidtech_las.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-01 15:24:39.000000 lucidtech-las-8.9.0/lucidtech_las.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-01 15:24:39.000000 lucidtech-las-8.9.0/lucidtech_las.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 15:24:39.000000 lucidtech-las-8.9.0/lucidtech_las.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-01 15:24:39.000000 lucidtech-las-8.9.0/lucidtech_las.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-01 15:24:39.000000 lucidtech-las-8.9.0/lucidtech_las.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-01 15:24:39.788257 lucidtech-las-8.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-01 15:24:29.000000 lucidtech-las-8.9.0/setup.py
```

### Comparing `lucidtech-las-8.8.0/LICENSE.md` & `lucidtech-las-8.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lucidtech-las-8.8.0/PKG-INFO` & `lucidtech-las-8.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidtech-las
-Version: 8.8.0
+Version: 8.9.0
 Summary: Python SDK for Lucidtech AI Services
 Home-page: https://github.com/LucidtechAI/las-sdk-python
 Author: Lucidtech
 Author-email: hello@lucidtech.ai
 Maintainer: Magnus Aarskaug Rud
 Maintainer-email: magnus@lucidtech.ai
 License: Apache 2.0
```

### Comparing `lucidtech-las-8.8.0/README.md` & `lucidtech-las-8.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lucidtech-las-8.8.0/las/client.py` & `lucidtech-las-8.9.0/las/client.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-8.8.0/las/credentials.py` & `lucidtech-las-8.9.0/las/credentials.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-8.8.0/lucidtech_las.egg-info/PKG-INFO` & `lucidtech-las-8.9.0/lucidtech_las.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidtech-las
-Version: 8.8.0
+Version: 8.9.0
 Summary: Python SDK for Lucidtech AI Services
 Home-page: https://github.com/LucidtechAI/las-sdk-python
 Author: Lucidtech
 Author-email: hello@lucidtech.ai
 Maintainer: Magnus Aarskaug Rud
 Maintainer-email: magnus@lucidtech.ai
 License: Apache 2.0
```

### Comparing `lucidtech-las-8.8.0/setup.py` & `lucidtech-las-8.9.0/setup.py`

 * *Files identical despite different names*

