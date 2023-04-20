# Comparing `tmp/amlopschat-0.post0.dev1.tar.gz` & `tmp/amlopschat-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amlopschat-0.post0.dev1.tar", last modified: Wed Apr 19 18:08:58 2023, max compression
+gzip compressed data, was "amlopschat-1.0.0.tar", last modified: Thu Apr 20 13:04:40 2023, max compression
```

## Comparing `amlopschat-0.post0.dev1.tar` & `amlopschat-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:08:58.689038 amlopschat-0.post0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-19 18:08:15.000000 amlopschat-0.post0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 18:08:58.689038 amlopschat-0.post0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-19 18:08:15.000000 amlopschat-0.post0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:08:58.689038 amlopschat-0.post0.dev1/amlopschat/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-19 18:08:45.000000 amlopschat-0.post0.dev1/amlopschat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-19 18:08:45.000000 amlopschat-0.post0.dev1/amlopschat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:08:58.689038 amlopschat-0.post0.dev1/amlopschat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 18:08:58.000000 amlopschat-0.post0.dev1/amlopschat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-19 18:08:58.000000 amlopschat-0.post0.dev1/amlopschat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:08:58.000000 amlopschat-0.post0.dev1/amlopschat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 18:08:58.000000 amlopschat-0.post0.dev1/amlopschat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 18:08:58.689038 amlopschat-0.post0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-19 18:08:15.000000 amlopschat-0.post0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:08:58.689038 amlopschat-0.post0.dev1/src/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-19 18:08:58.689038 amlopschat-0.post0.dev1/src/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-19 18:08:15.000000 amlopschat-0.post0.dev1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:04:40.850665 amlopschat-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 13:04:01.000000 amlopschat-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 13:04:40.850665 amlopschat-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 13:04:01.000000 amlopschat-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:04:40.846665 amlopschat-1.0.0/amlopschat/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 13:04:29.000000 amlopschat-1.0.0/amlopschat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-20 13:04:29.000000 amlopschat-1.0.0/amlopschat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:04:40.846665 amlopschat-1.0.0/amlopschat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 13:04:40.000000 amlopschat-1.0.0/amlopschat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-20 13:04:40.000000 amlopschat-1.0.0/amlopschat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:04:40.000000 amlopschat-1.0.0/amlopschat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 13:04:40.000000 amlopschat-1.0.0/amlopschat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-20 13:04:40.850665 amlopschat-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 13:04:01.000000 amlopschat-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:04:40.850665 amlopschat-1.0.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 13:04:40.850665 amlopschat-1.0.0/src/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-20 13:04:01.000000 amlopschat-1.0.0/versioneer.py
```

### Comparing `amlopschat-0.post0.dev1/README.md` & `amlopschat-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `amlopschat-0.post0.dev1/amlopschat/_version.py` & `amlopschat-1.0.0/amlopschat/_version.py`

 * *Files identical despite different names*

### Comparing `amlopschat-0.post0.dev1/versioneer.py` & `amlopschat-1.0.0/versioneer.py`

 * *Files identical despite different names*

