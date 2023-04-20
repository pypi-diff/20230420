# Comparing `tmp/openlimit-0.0.1.tar.gz` & `tmp/openlimit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlimit-0.0.1.tar", last modified: Thu Apr 20 02:29:09 2023, max compression
+gzip compressed data, was "openlimit-0.1.0.tar", last modified: Thu Apr 20 02:31:11 2023, max compression
```

## Comparing `openlimit-0.0.1.tar` & `openlimit-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-20 02:29:09.922962 openlimit-0.0.1/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-20 02:29:09.922843 openlimit-0.0.1/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)     2953 2023-04-20 02:04:04.000000 openlimit-0.0.1/README.md
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-20 02:29:09.921987 openlimit-0.0.1/openlimit/
--rw-r--r--   0 jshobrook   (501) staff       (20)      206 2023-04-19 18:27:50.000000 openlimit-0.0.1/openlimit/__init__.py
--rw-r--r--   0 jshobrook   (501) staff       (20)      937 2023-04-20 02:10:59.000000 openlimit-0.0.1/openlimit/main.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1744 2023-04-20 01:19:55.000000 openlimit-0.0.1/openlimit/rate_limiters.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     2834 2023-04-20 01:36:17.000000 openlimit-0.0.1/openlimit/redis_rate_limiters.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-20 02:29:09.922698 openlimit-0.0.1/openlimit.egg-info/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-20 02:29:09.000000 openlimit-0.0.1/openlimit.egg-info/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)      282 2023-04-20 02:29:09.000000 openlimit-0.0.1/openlimit.egg-info/SOURCES.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-04-20 02:29:09.000000 openlimit-0.0.1/openlimit.egg-info/dependency_links.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-04-20 02:29:09.000000 openlimit-0.0.1/openlimit.egg-info/requires.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-04-20 02:29:09.000000 openlimit-0.0.1/openlimit.egg-info/top_level.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-04-20 02:29:09.923003 openlimit-0.0.1/setup.cfg
--rw-r--r--   0 jshobrook   (501) staff       (20)      515 2023-04-20 02:28:55.000000 openlimit-0.0.1/setup.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-20 02:31:11.172664 openlimit-0.1.0/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-20 02:31:11.172551 openlimit-0.1.0/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)     2953 2023-04-20 02:04:04.000000 openlimit-0.1.0/README.md
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-20 02:31:11.171694 openlimit-0.1.0/openlimit/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      206 2023-04-19 18:27:50.000000 openlimit-0.1.0/openlimit/__init__.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1774 2023-04-20 02:30:45.000000 openlimit-0.1.0/openlimit/rate_limiters.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     2864 2023-04-20 02:30:35.000000 openlimit-0.1.0/openlimit/redis_rate_limiters.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-20 02:31:11.172388 openlimit-0.1.0/openlimit.egg-info/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-20 02:31:11.000000 openlimit-0.1.0/openlimit.egg-info/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)      264 2023-04-20 02:31:11.000000 openlimit-0.1.0/openlimit.egg-info/SOURCES.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-04-20 02:31:11.000000 openlimit-0.1.0/openlimit.egg-info/dependency_links.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-04-20 02:31:11.000000 openlimit-0.1.0/openlimit.egg-info/requires.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-04-20 02:31:11.000000 openlimit-0.1.0/openlimit.egg-info/top_level.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-04-20 02:31:11.172706 openlimit-0.1.0/setup.cfg
+-rw-r--r--   0 jshobrook   (501) staff       (20)      515 2023-04-20 02:31:04.000000 openlimit-0.1.0/setup.py
```

### Comparing `openlimit-0.0.1/README.md` & `openlimit-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openlimit-0.0.1/openlimit/rate_limiters.py` & `openlimit-0.1.0/openlimit/rate_limiters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Standard library
 import asyncio
 
 # Local
-import utilities.token_counters as tc
-import utilities.context_decorators as cd
-from buckets import Bucket
+import openlimit.utilities.token_counters as tc
+import openlimit.utilities.context_decorators as cd
+from openlimit.buckets import Bucket
 
 
 ############
 # BASE CLASS
 ############
```

### Comparing `openlimit-0.0.1/openlimit/redis_rate_limiters.py` & `openlimit-0.1.0/openlimit/redis_rate_limiters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Standard library
 import asyncio
 
 # Third party
 from redis import asyncio as aioredis
 
 # Local
-import utilities.token_counters as tc
-import utilities.context_decorators as cd
-from buckets import RedisBucket
+import openlimit.utilities.token_counters as tc
+import openlimit.utilities.context_decorators as cd
+from openlimit.buckets import RedisBucket
 
 
 ############
 # BASE CLASS
 ############
```

### Comparing `openlimit-0.0.1/setup.py` & `openlimit-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from setuptools import setup
 
 setup(
     name="openlimit",
     description="Rate limiter for the OpenAI API",
-    version="v0.0.1",
+    version="v0.1.0",
     packages=["openlimit"],
     python_requires=">=3",
     url="https://github.com/shobrook/openlimit",
     author="shobrook",
     author_email="shobrookj@gmail.com",
     # classifiers=[],
     install_requires=["redis", "tiktoken"],
```

