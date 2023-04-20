# Comparing `tmp/sentry-redis-tools-0.1.3.tar.gz` & `tmp/sentry-redis-tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-redis-tools-0.1.3.tar", last modified: Tue Apr 18 16:10:53 2023, max compression
+gzip compressed data, was "sentry-redis-tools-0.1.4.tar", last modified: Thu Apr 20 15:13:19 2023, max compression
```

## Comparing `sentry-redis-tools-0.1.3.tar` & `sentry-redis-tools-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:10:53.712222 sentry-redis-tools-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-18 16:10:51.000000 sentry-redis-tools-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-18 16:10:53.712222 sentry-redis-tools-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 16:10:51.000000 sentry-redis-tools-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:10:53.708222 sentry-redis-tools-0.1.3/sentry_redis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:10:51.000000 sentry-redis-tools-0.1.3/sentry_redis_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-18 16:10:51.000000 sentry-redis-tools-0.1.3/sentry_redis_tools/failover_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:10:53.712222 sentry-redis-tools-0.1.3/sentry_redis_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-18 16:10:53.000000 sentry-redis-tools-0.1.3/sentry_redis_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-18 16:10:53.000000 sentry-redis-tools-0.1.3/sentry_redis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:10:53.000000 sentry-redis-tools-0.1.3/sentry_redis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:10:53.000000 sentry-redis-tools-0.1.3/sentry_redis_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 16:10:53.000000 sentry-redis-tools-0.1.3/sentry_redis_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 16:10:53.000000 sentry-redis-tools-0.1.3/sentry_redis_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:10:53.712222 sentry-redis-tools-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-18 16:10:51.000000 sentry-redis-tools-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:13:19.563357 sentry-redis-tools-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-20 15:13:15.000000 sentry-redis-tools-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-20 15:13:19.563357 sentry-redis-tools-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 15:13:15.000000 sentry-redis-tools-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:13:19.563357 sentry-redis-tools-0.1.4/sentry_redis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:13:15.000000 sentry-redis-tools-0.1.4/sentry_redis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-20 15:13:15.000000 sentry-redis-tools-0.1.4/sentry_redis_tools/failover_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:13:19.563357 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-20 15:13:19.000000 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-20 15:13:19.000000 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:13:19.000000 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:13:19.000000 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 15:13:19.000000 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 15:13:19.000000 sentry-redis-tools-0.1.4/sentry_redis_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:13:19.563357 sentry-redis-tools-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-20 15:13:15.000000 sentry-redis-tools-0.1.4/setup.py
```

### Comparing `sentry-redis-tools-0.1.3/LICENSE` & `sentry-redis-tools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.3/sentry_redis_tools/failover_redis.py` & `sentry-redis-tools-0.1.4/sentry_redis_tools/failover_redis.py`

 * *Files identical despite different names*

### Comparing `sentry-redis-tools-0.1.3/setup.py` & `sentry-redis-tools-0.1.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import find_packages, setup
 
 from typing import Sequence
 
 
 setup(
     name="sentry-redis-tools",
-    version="0.1.3",
+    version="0.1.4",
     author="Sentry",
     author_email="oss@sentry.io",
     url="https://github.com/getsentry/sentry-redis-tools",
     description="Common utilities related to how Sentry uses Redis",
     zip_safe=False,
-    install_requires=['redis>=4.0'],
+    install_requires=['redis>=3.0'],
     packages=find_packages(exclude=("tests", "tests.*")),
     package_data={"sentry_redis_tools": ["py.typed"]},
     include_package_data=True,
     options={"bdist_wheel": {"universal": "1"}},
 )
```

