# Comparing `tmp/slim-compose-1.0.0.tar.gz` & `tmp/slim-compose-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slim-compose-1.0.0.tar", last modified: Thu Apr 20 03:34:41 2023, max compression
+gzip compressed data, was "slim-compose-1.0.1.tar", last modified: Thu Apr 20 06:35:38 2023, max compression
```

## Comparing `slim-compose-1.0.0.tar` & `slim-compose-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 03:34:41.012913 slim-compose-1.0.0/
--rw-r--r--   0 foobar    (1000) foobar    (1000)     1056 2023-04-20 02:33:29.000000 slim-compose-1.0.0/LICENSE
--rw-r--r--   0 foobar    (1000) foobar    (1000)     1792 2023-04-20 03:34:41.012913 slim-compose-1.0.0/PKG-INFO
--rw-r--r--   0 foobar    (1000) foobar    (1000)       54 2023-04-20 02:31:29.000000 slim-compose-1.0.0/README.md
--rw-r--r--   0 foobar    (1000) foobar    (1000)      582 2023-04-20 03:34:30.000000 slim-compose-1.0.0/pyproject.toml
--rw-r--r--   0 foobar    (1000) foobar    (1000)       38 2023-04-20 03:34:41.012913 slim-compose-1.0.0/setup.cfg
-drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 03:34:41.012913 slim-compose-1.0.0/src/
-drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 03:34:41.012913 slim-compose-1.0.0/src/slim_compose.egg-info/
--rw-r--r--   0 foobar    (1000) foobar    (1000)     1792 2023-04-20 03:34:41.000000 slim-compose-1.0.0/src/slim_compose.egg-info/PKG-INFO
--rw-r--r--   0 foobar    (1000) foobar    (1000)      255 2023-04-20 03:34:41.000000 slim-compose-1.0.0/src/slim_compose.egg-info/SOURCES.txt
--rw-r--r--   0 foobar    (1000) foobar    (1000)        1 2023-04-20 03:34:41.000000 slim-compose-1.0.0/src/slim_compose.egg-info/dependency_links.txt
--rw-r--r--   0 foobar    (1000) foobar    (1000)       51 2023-04-20 03:34:41.000000 slim-compose-1.0.0/src/slim_compose.egg-info/entry_points.txt
--rw-r--r--   0 foobar    (1000) foobar    (1000)       13 2023-04-20 03:34:41.000000 slim-compose-1.0.0/src/slim_compose.egg-info/top_level.txt
--rwxr-xr-x   0 foobar    (1000) foobar    (1000)    13162 2023-04-20 02:54:34.000000 slim-compose-1.0.0/src/slim_compose.py
+drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 06:35:38.850344 slim-compose-1.0.1/
+-rw-r--r--   0 foobar    (1000) foobar    (1000)     1056 2023-04-20 02:33:29.000000 slim-compose-1.0.1/LICENSE
+-rw-r--r--   0 foobar    (1000) foobar    (1000)     1913 2023-04-20 06:35:38.850344 slim-compose-1.0.1/PKG-INFO
+-rw-r--r--   0 foobar    (1000) foobar    (1000)      174 2023-04-20 06:35:13.000000 slim-compose-1.0.1/README.md
+-rw-r--r--   0 foobar    (1000) foobar    (1000)      582 2023-04-20 06:35:26.000000 slim-compose-1.0.1/pyproject.toml
+-rw-r--r--   0 foobar    (1000) foobar    (1000)       38 2023-04-20 06:35:38.850344 slim-compose-1.0.1/setup.cfg
+drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 06:35:38.850344 slim-compose-1.0.1/src/
+drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 06:35:38.850344 slim-compose-1.0.1/src/slim_compose.egg-info/
+-rw-r--r--   0 foobar    (1000) foobar    (1000)     1913 2023-04-20 06:35:38.000000 slim-compose-1.0.1/src/slim_compose.egg-info/PKG-INFO
+-rw-r--r--   0 foobar    (1000) foobar    (1000)      255 2023-04-20 06:35:38.000000 slim-compose-1.0.1/src/slim_compose.egg-info/SOURCES.txt
+-rw-r--r--   0 foobar    (1000) foobar    (1000)        1 2023-04-20 06:35:38.000000 slim-compose-1.0.1/src/slim_compose.egg-info/dependency_links.txt
+-rw-r--r--   0 foobar    (1000) foobar    (1000)       51 2023-04-20 06:35:38.000000 slim-compose-1.0.1/src/slim_compose.egg-info/entry_points.txt
+-rw-r--r--   0 foobar    (1000) foobar    (1000)       13 2023-04-20 06:35:38.000000 slim-compose-1.0.1/src/slim_compose.egg-info/top_level.txt
+-rwxr-xr-x   0 foobar    (1000) foobar    (1000)    13171 2023-04-20 06:30:20.000000 slim-compose-1.0.1/src/slim_compose.py
```

### Comparing `slim-compose-1.0.0/LICENSE` & `slim-compose-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slim-compose-1.0.0/PKG-INFO` & `slim-compose-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slim-compose
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple management tool for podman pods
 Author-email: xfoobar <xfoobar@outlook.com>
 License: MIT License
         
         Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,8 +32,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # slim-compose
-Simple management tool for podman pods
+Simple management tool for podman pods.  
+written by pure Python, no third-party dependencies.
+
+## install
+```
+pipx isntall slim-compose
+```
+
+## usage
+```
+
+```
```

### Comparing `slim-compose-1.0.0/pyproject.toml` & `slim-compose-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "slim-compose"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="xfoobar", email="xfoobar@outlook.com" },
 ]
 description = "Simple management tool for podman pods"
 keywords = ["podman", "compose"]
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `slim-compose-1.0.0/src/slim_compose.egg-info/PKG-INFO` & `slim-compose-1.0.1/src/slim_compose.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slim-compose
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple management tool for podman pods
 Author-email: xfoobar <xfoobar@outlook.com>
 License: MIT License
         
         Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,8 +32,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # slim-compose
-Simple management tool for podman pods
+Simple management tool for podman pods.  
+written by pure Python, no third-party dependencies.
+
+## install
+```
+pipx isntall slim-compose
+```
+
+## usage
+```
+
+```
```

### Comparing `slim-compose-1.0.0/src/slim_compose.py` & `slim-compose-1.0.1/src/slim_compose.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 from pathlib import Path
 import os
 import subprocess
 import json
 import argparse
 
-APP_VERSION = '1.0.0'
+APP_VERSION = '1.0.1'
 
 ENCODING = 'utf-8'
 
 
 def nvl(*args):
     """
     return first non-null value
@@ -353,15 +353,15 @@
         entity_types = ['pod', 'container', 'network', 'volume']
     for entity_type in entity_types:
         entities = list_relevant_entity(entity_type=entity_type)
         for e in entities:
             # stop pod and container
             if entity_type in ('pod', 'container'):
                 cmd = ['podman', entity_type, 'stop', e]
-                exec_cmd(cmd=cmd, ignore_error=False)
+                exec_cmd(cmd=cmd, ignore_error=False, dry=dry)
             cmd = ['podman', entity_type, 'rm', e]
             exec_cmd(cmd=cmd, ignore_error=False, dry=dry)
     print('Finished.')
 
 
 def pod_operate(op: str, dry: bool):
     """
```

