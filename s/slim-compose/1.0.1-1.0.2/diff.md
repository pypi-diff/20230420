# Comparing `tmp/slim-compose-1.0.1.tar.gz` & `tmp/slim-compose-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slim-compose-1.0.1.tar", last modified: Thu Apr 20 06:35:38 2023, max compression
+gzip compressed data, was "slim-compose-1.0.2.tar", last modified: Thu Apr 20 06:57:56 2023, max compression
```

## Comparing `slim-compose-1.0.1.tar` & `slim-compose-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 06:35:38.850344 slim-compose-1.0.1/
--rw-r--r--   0 foobar    (1000) foobar    (1000)     1056 2023-04-20 02:33:29.000000 slim-compose-1.0.1/LICENSE
--rw-r--r--   0 foobar    (1000) foobar    (1000)     1913 2023-04-20 06:35:38.850344 slim-compose-1.0.1/PKG-INFO
--rw-r--r--   0 foobar    (1000) foobar    (1000)      174 2023-04-20 06:35:13.000000 slim-compose-1.0.1/README.md
--rw-r--r--   0 foobar    (1000) foobar    (1000)      582 2023-04-20 06:35:26.000000 slim-compose-1.0.1/pyproject.toml
--rw-r--r--   0 foobar    (1000) foobar    (1000)       38 2023-04-20 06:35:38.850344 slim-compose-1.0.1/setup.cfg
-drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 06:35:38.850344 slim-compose-1.0.1/src/
-drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 06:35:38.850344 slim-compose-1.0.1/src/slim_compose.egg-info/
--rw-r--r--   0 foobar    (1000) foobar    (1000)     1913 2023-04-20 06:35:38.000000 slim-compose-1.0.1/src/slim_compose.egg-info/PKG-INFO
--rw-r--r--   0 foobar    (1000) foobar    (1000)      255 2023-04-20 06:35:38.000000 slim-compose-1.0.1/src/slim_compose.egg-info/SOURCES.txt
--rw-r--r--   0 foobar    (1000) foobar    (1000)        1 2023-04-20 06:35:38.000000 slim-compose-1.0.1/src/slim_compose.egg-info/dependency_links.txt
--rw-r--r--   0 foobar    (1000) foobar    (1000)       51 2023-04-20 06:35:38.000000 slim-compose-1.0.1/src/slim_compose.egg-info/entry_points.txt
--rw-r--r--   0 foobar    (1000) foobar    (1000)       13 2023-04-20 06:35:38.000000 slim-compose-1.0.1/src/slim_compose.egg-info/top_level.txt
--rwxr-xr-x   0 foobar    (1000) foobar    (1000)    13171 2023-04-20 06:30:20.000000 slim-compose-1.0.1/src/slim_compose.py
+drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 06:57:56.092924 slim-compose-1.0.2/
+-rw-r--r--   0 foobar    (1000) foobar    (1000)     1056 2023-04-20 02:33:29.000000 slim-compose-1.0.2/LICENSE
+-rw-r--r--   0 foobar    (1000) foobar    (1000)     2183 2023-04-20 06:57:56.092924 slim-compose-1.0.2/PKG-INFO
+-rw-r--r--   0 foobar    (1000) foobar    (1000)      472 2023-04-20 06:49:18.000000 slim-compose-1.0.2/README.md
+-rw-r--r--   0 foobar    (1000) foobar    (1000)      553 2023-04-20 06:56:39.000000 slim-compose-1.0.2/pyproject.toml
+-rw-r--r--   0 foobar    (1000) foobar    (1000)       38 2023-04-20 06:57:56.092924 slim-compose-1.0.2/setup.cfg
+drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 06:57:56.092924 slim-compose-1.0.2/src/
+drwxr-xr-x   0 foobar    (1000) foobar    (1000)        0 2023-04-20 06:57:56.092924 slim-compose-1.0.2/src/slim_compose.egg-info/
+-rw-r--r--   0 foobar    (1000) foobar    (1000)     2183 2023-04-20 06:57:56.000000 slim-compose-1.0.2/src/slim_compose.egg-info/PKG-INFO
+-rw-r--r--   0 foobar    (1000) foobar    (1000)      255 2023-04-20 06:57:56.000000 slim-compose-1.0.2/src/slim_compose.egg-info/SOURCES.txt
+-rw-r--r--   0 foobar    (1000) foobar    (1000)        1 2023-04-20 06:57:56.000000 slim-compose-1.0.2/src/slim_compose.egg-info/dependency_links.txt
+-rw-r--r--   0 foobar    (1000) foobar    (1000)       51 2023-04-20 06:57:56.000000 slim-compose-1.0.2/src/slim_compose.egg-info/entry_points.txt
+-rw-r--r--   0 foobar    (1000) foobar    (1000)       13 2023-04-20 06:57:56.000000 slim-compose-1.0.2/src/slim_compose.egg-info/top_level.txt
+-rwxr-xr-x   0 foobar    (1000) foobar    (1000)    13171 2023-04-20 06:56:29.000000 slim-compose-1.0.2/src/slim_compose.py
```

### Comparing `slim-compose-1.0.1/LICENSE` & `slim-compose-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slim-compose-1.0.1/PKG-INFO` & `slim-compose-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: slim-compose
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple management tool for podman pods
-Author-email: xfoobar <xfoobar@outlook.com>
+Author: xfoobar
 License: MIT License
         
         Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -32,19 +32,32 @@
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # slim-compose
-Simple management tool for podman pods.  
-written by pure Python, no third-party dependencies.
+Simple management tool for podman pods, written by pure Python, no third-party dependencies.
+
+## requirements
+- Podman 4.4.2 ( networkBackend: netavark )
+- Python 3.10
+
 
 ## install
 ```
-pipx isntall slim-compose
+pipx install slim-compose
 ```
 
 ## usage
-```
-
+```sh
+# create config file
+slim-compose template
+# edit config file
+vim slim-compose-template.json
+# rename config file
+mv slim-compose-template.json slim-compose.json
+# deploy pod
+slim-compose up
+# destroy pod
+slim-compose down
 ```
```

### Comparing `slim-compose-1.0.1/pyproject.toml` & `slim-compose-1.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "slim-compose"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
-  { name="xfoobar", email="xfoobar@outlook.com" },
+  { name="xfoobar"},
 ]
 description = "Simple management tool for podman pods"
 keywords = ["podman", "compose"]
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
 classifiers = [
@@ -16,8 +16,8 @@
     "Environment :: Console"
 ]
 
 [project.scripts]
 slim-compose = "slim_compose:main"
 
 [project.urls]
-"Homepage" = "https://github.com/xfoobar/slim-compose"
+"Homepage" = "https://github.com/xfoobar/slim-compose"
```

### Comparing `slim-compose-1.0.1/src/slim_compose.egg-info/PKG-INFO` & `slim-compose-1.0.2/src/slim_compose.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: slim-compose
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple management tool for podman pods
-Author-email: xfoobar <xfoobar@outlook.com>
+Author: xfoobar
 License: MIT License
         
         Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -32,19 +32,32 @@
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # slim-compose
-Simple management tool for podman pods.  
-written by pure Python, no third-party dependencies.
+Simple management tool for podman pods, written by pure Python, no third-party dependencies.
+
+## requirements
+- Podman 4.4.2 ( networkBackend: netavark )
+- Python 3.10
+
 
 ## install
 ```
-pipx isntall slim-compose
+pipx install slim-compose
 ```
 
 ## usage
-```
-
+```sh
+# create config file
+slim-compose template
+# edit config file
+vim slim-compose-template.json
+# rename config file
+mv slim-compose-template.json slim-compose.json
+# deploy pod
+slim-compose up
+# destroy pod
+slim-compose down
 ```
```

### Comparing `slim-compose-1.0.1/src/slim_compose.py` & `slim-compose-1.0.2/src/slim_compose.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 from pathlib import Path
 import os
 import subprocess
 import json
 import argparse
 
-APP_VERSION = '1.0.1'
+APP_VERSION = '1.0.2'
 
 ENCODING = 'utf-8'
 
 
 def nvl(*args):
     """
     return first non-null value
```

