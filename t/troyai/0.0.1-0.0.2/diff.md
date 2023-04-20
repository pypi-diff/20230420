# Comparing `tmp/troyai-0.0.1.tar.gz` & `tmp/troyai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troyai-0.0.1.tar", last modified: Thu Apr 20 04:26:32 2023, max compression
+gzip compressed data, was "troyai-0.0.2.tar", last modified: Thu Apr 20 04:42:29 2023, max compression
```

## Comparing `troyai-0.0.1.tar` & `troyai-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 04:26:32.675917 troyai-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-04-18 23:26:12.000000 troyai-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      656 2023-04-20 04:26:32.674914 troyai-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       85 2023-04-18 23:26:12.000000 troyai-0.0.1/README.md
--rw-rw-rw-   0        0        0      651 2023-04-20 04:25:26.000000 troyai-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 04:26:32.676916 troyai-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-20 04:26:32.656915 troyai-0.0.1/troyai/
--rw-rw-rw-   0        0        0       68 2023-04-20 04:00:32.000000 troyai-0.0.1/troyai/__init__.py
--rw-rw-rw-   0        0        0      273 2023-04-20 03:55:48.000000 troyai-0.0.1/troyai/constants.py
--rw-rw-rw-   0        0        0      163 2023-04-20 03:54:49.000000 troyai-0.0.1/troyai/download.py
--rw-rw-rw-   0        0        0     1890 2023-04-20 03:58:07.000000 troyai-0.0.1/troyai/error_helpers.py
--rw-rw-rw-   0        0        0     1997 2023-04-20 04:12:43.000000 troyai-0.0.1/troyai/upload.py
-drwxrwxrwx   0        0        0        0 2023-04-20 04:26:32.673911 troyai-0.0.1/troyai.egg-info/
--rw-rw-rw-   0        0        0      656 2023-04-20 04:26:32.000000 troyai-0.0.1/troyai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-04-20 04:26:32.000000 troyai-0.0.1/troyai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 04:26:32.000000 troyai-0.0.1/troyai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 04:26:32.000000 troyai-0.0.1/troyai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 04:42:29.197581 troyai-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-04-18 23:26:12.000000 troyai-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      656 2023-04-20 04:42:29.196582 troyai-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2023-04-18 23:26:12.000000 troyai-0.0.2/README.md
+-rw-rw-rw-   0        0        0      651 2023-04-20 04:37:56.000000 troyai-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 04:42:29.197581 troyai-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 04:42:29.181579 troyai-0.0.2/troyai/
+-rw-rw-rw-   0        0        0       70 2023-04-20 04:33:23.000000 troyai-0.0.2/troyai/__init__.py
+-rw-rw-rw-   0        0        0      273 2023-04-20 03:55:48.000000 troyai-0.0.2/troyai/constants.py
+-rw-rw-rw-   0        0        0      171 2023-04-20 04:36:21.000000 troyai-0.0.2/troyai/download.py
+-rw-rw-rw-   0        0        0     1891 2023-04-20 04:33:29.000000 troyai-0.0.2/troyai/error_helpers.py
+-rw-rw-rw-   0        0        0     1999 2023-04-20 04:33:35.000000 troyai-0.0.2/troyai/upload.py
+drwxrwxrwx   0        0        0        0 2023-04-20 04:42:29.194584 troyai-0.0.2/troyai.egg-info/
+-rw-rw-rw-   0        0        0      656 2023-04-20 04:42:29.000000 troyai-0.0.2/troyai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-04-20 04:42:29.000000 troyai-0.0.2/troyai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 04:42:29.000000 troyai-0.0.2/troyai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 04:42:29.000000 troyai-0.0.2/troyai.egg-info/top_level.txt
```

### Comparing `troyai-0.0.1/LICENSE` & `troyai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `troyai-0.0.1/PKG-INFO` & `troyai-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troyai
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for downloading & uploading models to the Troy AI Club website.
 Author-email: Troy AI Club <troyhigh.aiclub@gmail.com>
 Project-URL: Homepage, https://github.com/TroyAI/pypitroyai
 Project-URL: Bug Tracker, https://github.com/TroyAI/pypitroyai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `troyai-0.0.1/pyproject.toml` & `troyai-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "troyai"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Troy AI Club", email="troyhigh.aiclub@gmail.com" },
 ]
 description = "A Python package for downloading & uploading models to the Troy AI Club website."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `troyai-0.0.1/troyai/error_helpers.py` & `troyai-0.0.2/troyai/error_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from constants import *
+from .constants import *
 
 def token_error(token: str) -> bool:
     if len(token) != 16 or any(character not in BASE62 for character in token):
         print(f"Error: invalid token")
         print(f"Token should be 16 characters {f'(not {len(token)}) ' if len(token) != 16 else ' '}and every character should be in this set:")
         print(BASE62 + '\n')
         return True
```

### Comparing `troyai-0.0.1/troyai/upload.py` & `troyai-0.0.2/troyai/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import requests
 import json
 import pickle
 import string
 
 from typing import Any
-from constants import *
 
-from error_helpers import (
+from .constants import *
+from .error_helpers import (
     token_error,
     name_error,
     description_error,
     score_error,
     hostname_error,
 )
```

### Comparing `troyai-0.0.1/troyai.egg-info/PKG-INFO` & `troyai-0.0.2/troyai.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troyai
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for downloading & uploading models to the Troy AI Club website.
 Author-email: Troy AI Club <troyhigh.aiclub@gmail.com>
 Project-URL: Homepage, https://github.com/TroyAI/pypitroyai
 Project-URL: Bug Tracker, https://github.com/TroyAI/pypitroyai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

