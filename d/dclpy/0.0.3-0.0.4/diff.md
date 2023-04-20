# Comparing `tmp/dclpy-0.0.3.tar.gz` & `tmp/dclpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dclpy-0.0.3.tar", last modified: Thu Apr 20 08:03:47 2023, max compression
+gzip compressed data, was "dclpy-0.0.4.tar", last modified: Thu Apr 20 08:37:12 2023, max compression
```

## Comparing `dclpy-0.0.3.tar` & `dclpy-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 otobe     (1000) otobe     (1000)        0 2023-04-20 08:03:47.394459 dclpy-0.0.3/
--rw-r--r--   0 otobe     (1000) otobe     (1000)       49 2023-04-20 08:03:47.394459 dclpy-0.0.3/PKG-INFO
-drwxr-xr-x   0 otobe     (1000) otobe     (1000)        0 2023-04-20 08:03:47.394459 dclpy-0.0.3/dclpy/
--rw-r--r--   0 otobe     (1000) otobe     (1000)   583371 2023-03-30 08:08:29.000000 dclpy-0.0.3/dclpy/dclpy.c
--rw-r--r--   0 otobe     (1000) otobe     (1000)   583371 2023-04-20 08:02:19.000000 dclpy-0.0.3/dclpy/dclpy_wrapper.c
-drwxr-xr-x   0 otobe     (1000) otobe     (1000)        0 2023-04-20 08:03:47.394459 dclpy-0.0.3/dclpy.egg-info/
--rw-r--r--   0 otobe     (1000) otobe     (1000)       49 2023-04-20 08:03:47.000000 dclpy-0.0.3/dclpy.egg-info/PKG-INFO
--rw-r--r--   0 otobe     (1000) otobe     (1000)      160 2023-04-20 08:03:47.000000 dclpy-0.0.3/dclpy.egg-info/SOURCES.txt
--rw-r--r--   0 otobe     (1000) otobe     (1000)        1 2023-04-20 08:03:47.000000 dclpy-0.0.3/dclpy.egg-info/dependency_links.txt
--rw-r--r--   0 otobe     (1000) otobe     (1000)        6 2023-04-20 08:03:47.000000 dclpy-0.0.3/dclpy.egg-info/top_level.txt
--rw-r--r--   0 otobe     (1000) otobe     (1000)       38 2023-04-20 08:03:47.394459 dclpy-0.0.3/setup.cfg
--rw-r--r--   0 otobe     (1000) otobe     (1000)      529 2023-04-20 08:03:42.000000 dclpy-0.0.3/setup.py
+drwxr-xr-x   0 otobe     (1000) otobe     (1000)        0 2023-04-20 08:37:12.243228 dclpy-0.0.4/
+-rw-r--r--   0 otobe     (1000) otobe     (1000)       49 2023-04-20 08:37:12.243228 dclpy-0.0.4/PKG-INFO
+drwxr-xr-x   0 otobe     (1000) otobe     (1000)        0 2023-04-20 08:37:12.243228 dclpy-0.0.4/dclpy/
+-rw-r--r--   0 otobe     (1000) otobe     (1000)   112824 2023-03-30 08:08:29.000000 dclpy-0.0.4/dclpy/cdcl.h
+-rw-r--r--   0 otobe     (1000) otobe     (1000)     4363 2023-03-30 08:08:29.000000 dclpy-0.0.4/dclpy/cdcln.h
+-rw-r--r--   0 otobe     (1000) otobe     (1000)   583371 2023-03-30 08:08:29.000000 dclpy-0.0.4/dclpy/dclpy.c
+-rw-r--r--   0 otobe     (1000) otobe     (1000)   583371 2023-04-20 08:02:19.000000 dclpy-0.0.4/dclpy/dclpy_wrapper.c
+drwxr-xr-x   0 otobe     (1000) otobe     (1000)        0 2023-04-20 08:37:12.243228 dclpy-0.0.4/dclpy.egg-info/
+-rw-r--r--   0 otobe     (1000) otobe     (1000)       49 2023-04-20 08:37:12.000000 dclpy-0.0.4/dclpy.egg-info/PKG-INFO
+-rw-r--r--   0 otobe     (1000) otobe     (1000)      187 2023-04-20 08:37:12.000000 dclpy-0.0.4/dclpy.egg-info/SOURCES.txt
+-rw-r--r--   0 otobe     (1000) otobe     (1000)        1 2023-04-20 08:37:12.000000 dclpy-0.0.4/dclpy.egg-info/dependency_links.txt
+-rw-r--r--   0 otobe     (1000) otobe     (1000)        6 2023-04-20 08:37:12.000000 dclpy-0.0.4/dclpy.egg-info/top_level.txt
+-rw-r--r--   0 otobe     (1000) otobe     (1000)       38 2023-04-20 08:37:12.243228 dclpy-0.0.4/setup.cfg
+-rw-r--r--   0 otobe     (1000) otobe     (1000)      560 2023-04-20 08:37:10.000000 dclpy-0.0.4/setup.py
```

### Comparing `dclpy-0.0.3/dclpy/dclpy.c` & `dclpy-0.0.4/dclpy/dclpy.c`

 * *Files identical despite different names*

### Comparing `dclpy-0.0.3/dclpy/dclpy_wrapper.c` & `dclpy-0.0.4/dclpy/dclpy_wrapper.c`

 * *Files identical despite different names*

