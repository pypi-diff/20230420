# Comparing `tmp/dequeai-0.734.tar.gz` & `tmp/dequeai-0.736.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.734.tar", last modified: Thu Apr 20 21:02:52 2023, max compression
+gzip compressed data, was "dequeai-0.736.tar", last modified: Thu Apr 20 21:04:44 2023, max compression
```

## Comparing `dequeai-0.734.tar` & `dequeai-0.736.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:02:52.052342 dequeai-0.734/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 21:02:52.052342 dequeai-0.734/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:02:52.052342 dequeai-0.734/dequeai/
--rw-r--r--   0 root         (0) root         (0)      367 2023-04-19 19:09:51.000000 dequeai-0.734/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.734/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.734/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.734/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-04-20 20:33:33.000000 dequeai-0.734/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    24554 2023-04-20 21:02:32.000000 dequeai-0.734/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.734/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.734/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.734/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.734/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:02:52.052342 dequeai-0.734/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 21:02:51.000000 dequeai-0.734/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 21:02:52.000000 dequeai-0.734/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 21:02:51.000000 dequeai-0.734/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 21:02:51.000000 dequeai-0.734/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 21:02:51.000000 dequeai-0.734/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 21:02:52.052342 dequeai-0.734/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 21:02:32.000000 dequeai-0.734/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:04:44.504947 dequeai-0.736/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 21:04:44.504947 dequeai-0.736/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:04:44.504947 dequeai-0.736/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      398 2023-04-20 21:04:18.000000 dequeai-0.736/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.736/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.736/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.736/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-04-20 20:33:33.000000 dequeai-0.736/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    24554 2023-04-20 21:02:32.000000 dequeai-0.736/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.736/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.736/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.736/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.736/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:04:44.504947 dequeai-0.736/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 21:04:44.000000 dequeai-0.736/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 21:04:44.000000 dequeai-0.736/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 21:04:44.000000 dequeai-0.736/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 21:04:44.000000 dequeai-0.736/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 21:04:44.000000 dequeai-0.736/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 21:04:44.504947 dequeai-0.736/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 21:04:26.000000 dequeai-0.736/setup.py
```

### Comparing `dequeai-0.734/dequeai/datatypes.py` & `dequeai-0.736/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.734/dequeai/dequeai.py` & `dequeai-0.736/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.734/dequeai/dequeai_run.py` & `dequeai-0.736/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.734/dequeai/parsing_service.py` & `dequeai-0.736/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.734/dequeai/rest_connect.py` & `dequeai-0.736/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.734/dequeai/util.py` & `dequeai-0.736/dequeai/util.py`

 * *Files identical despite different names*

