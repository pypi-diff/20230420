# Comparing `tmp/mountainsort4-1.0.3.tar.gz` & `tmp/mountainsort4-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mountainsort4-1.0.3.tar", last modified: Fri Jul 29 03:58:25 2022, max compression
+gzip compressed data, was "mountainsort4-1.0.4.tar", last modified: Thu Apr 20 11:07:07 2023, max compression
```

## Comparing `mountainsort4-1.0.3.tar` & `mountainsort4-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-29 03:58:25.889449 mountainsort4-1.0.3/
--rw-rw-r--   0 magland   (1000) magland   (1000)      507 2022-07-29 03:58:25.889449 mountainsort4-1.0.3/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)      194 2022-07-08 17:52:52.000000 mountainsort4-1.0.3/README.md
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-29 03:58:25.889449 mountainsort4-1.0.3/mountainsort4/
--rw-rw-r--   0 magland   (1000) magland   (1000)       74 2022-07-29 03:57:38.000000 mountainsort4-1.0.3/mountainsort4/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)    16106 2022-07-08 17:52:52.000000 mountainsort4-1.0.3/mountainsort4/_mdaio_impl.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2274 2022-07-29 03:57:38.000000 mountainsort4-1.0.3/mountainsort4/mountainsort4.py
--rw-rw-r--   0 magland   (1000) magland   (1000)    37463 2022-07-29 03:57:38.000000 mountainsort4-1.0.3/mountainsort4/ms4alg.py
--rw-rw-r--   0 magland   (1000) magland   (1000)       97 2022-07-29 03:58:04.000000 mountainsort4-1.0.3/mountainsort4/version.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-29 03:58:25.889449 mountainsort4-1.0.3/mountainsort4.egg-info/
--rw-rw-r--   0 magland   (1000) magland   (1000)      507 2022-07-29 03:58:25.000000 mountainsort4-1.0.3/mountainsort4.egg-info/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)      347 2022-07-29 03:58:25.000000 mountainsort4-1.0.3/mountainsort4.egg-info/SOURCES.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        1 2022-07-29 03:58:25.000000 mountainsort4-1.0.3/mountainsort4.egg-info/dependency_links.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       73 2022-07-29 03:58:25.000000 mountainsort4-1.0.3/mountainsort4.egg-info/requires.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       14 2022-07-29 03:58:25.000000 mountainsort4-1.0.3/mountainsort4.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)      481 2022-07-29 03:58:25.893449 mountainsort4-1.0.3/setup.cfg
--rw-rw-r--   0 magland   (1000) magland   (1000)      277 2022-07-08 17:52:52.000000 mountainsort4-1.0.3/setup.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-04-20 11:07:07.840206 mountainsort4-1.0.4/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      462 2023-04-20 11:07:07.840206 mountainsort4-1.0.4/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)      194 2023-03-17 21:02:55.000000 mountainsort4-1.0.4/README.md
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-04-20 11:07:07.840206 mountainsort4-1.0.4/mountainsort4/
+-rw-rw-r--   0 magland   (1000) magland   (1000)       74 2023-03-17 21:02:55.000000 mountainsort4-1.0.4/mountainsort4/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)    16106 2023-03-17 21:02:55.000000 mountainsort4-1.0.4/mountainsort4/_mdaio_impl.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2274 2023-03-17 21:02:55.000000 mountainsort4-1.0.4/mountainsort4/mountainsort4.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)    37463 2023-03-17 21:02:55.000000 mountainsort4-1.0.4/mountainsort4/ms4alg.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)       97 2023-04-20 11:06:43.000000 mountainsort4-1.0.4/mountainsort4/version.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-04-20 11:07:07.840206 mountainsort4-1.0.4/mountainsort4.egg-info/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      462 2023-04-20 11:07:07.000000 mountainsort4-1.0.4/mountainsort4.egg-info/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)      347 2023-04-20 11:07:07.000000 mountainsort4-1.0.4/mountainsort4.egg-info/SOURCES.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        1 2023-04-20 11:07:07.000000 mountainsort4-1.0.4/mountainsort4.egg-info/dependency_links.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       78 2023-04-20 11:07:07.000000 mountainsort4-1.0.4/mountainsort4.egg-info/requires.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       14 2023-04-20 11:07:07.000000 mountainsort4-1.0.4/mountainsort4.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)      481 2023-04-20 11:07:07.840206 mountainsort4-1.0.4/setup.cfg
+-rw-rw-r--   0 magland   (1000) magland   (1000)      282 2023-04-20 11:06:25.000000 mountainsort4-1.0.4/setup.py
```

### Comparing `mountainsort4-1.0.3/mountainsort4/_mdaio_impl.py` & `mountainsort4-1.0.4/mountainsort4/_mdaio_impl.py`

 * *Files identical despite different names*

### Comparing `mountainsort4-1.0.3/mountainsort4/mountainsort4.py` & `mountainsort4-1.0.4/mountainsort4/mountainsort4.py`

 * *Files identical despite different names*

### Comparing `mountainsort4-1.0.3/mountainsort4/ms4alg.py` & `mountainsort4-1.0.4/mountainsort4/ms4alg.py`

 * *Files identical despite different names*

