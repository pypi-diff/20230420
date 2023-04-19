# Comparing `tmp/postpruner-0.6.tar.gz` & `tmp/postpruner-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postpruner-0.6.tar", last modified: Wed Apr 19 23:14:39 2023, max compression
+gzip compressed data, was "postpruner-0.7.tar", last modified: Wed Apr 19 23:16:03 2023, max compression
```

## Comparing `postpruner-0.6.tar` & `postpruner-0.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:14:39.662236 postpruner-0.6/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:14:39.662236 postpruner-0.6/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-0.6/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:14:39.662236 postpruner-0.6/postpruner/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:14:28.000000 postpruner-0.6/postpruner/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1680 2023-04-19 22:18:09.000000 postpruner-0.6/postpruner/__main__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7974 2023-04-19 22:19:26.000000 postpruner-0.6/postpruner/postpruner.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:14:39.662236 postpruner-0.6/postpruner.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:14:39.000000 postpruner-0.6/postpruner.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      295 2023-04-19 23:14:39.000000 postpruner-0.6/postpruner.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:14:39.000000 postpruner-0.6/postpruner.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-19 23:14:39.000000 postpruner-0.6/postpruner.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-19 23:14:39.000000 postpruner-0.6/postpruner.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-19 23:14:39.000000 postpruner-0.6/postpruner.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-19 23:14:39.662236 postpruner-0.6/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      407 2023-04-19 23:14:38.000000 postpruner-0.6/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:16:03.754163 postpruner-0.7/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:16:03.754163 postpruner-0.7/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-0.7/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:16:03.754163 postpruner-0.7/postpruner/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:14:28.000000 postpruner-0.7/postpruner/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1680 2023-04-19 22:18:09.000000 postpruner-0.7/postpruner/__main__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4996 2023-04-19 22:11:32.000000 postpruner-0.7/postpruner/generate_lut.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7974 2023-04-19 22:19:26.000000 postpruner-0.7/postpruner/postpruner.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:16:03.754163 postpruner-0.7/postpruner.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:16:03.000000 postpruner-0.7/postpruner.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      322 2023-04-19 23:16:03.000000 postpruner-0.7/postpruner.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:16:03.000000 postpruner-0.7/postpruner.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-19 23:16:03.000000 postpruner-0.7/postpruner.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-19 23:16:03.000000 postpruner-0.7/postpruner.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-19 23:16:03.000000 postpruner-0.7/postpruner.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-19 23:16:03.754163 postpruner-0.7/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      407 2023-04-19 23:15:59.000000 postpruner-0.7/setup.py
```

### Comparing `postpruner-0.6/README.md` & `postpruner-0.7/README.md`

 * *Files identical despite different names*

### Comparing `postpruner-0.6/postpruner/__main__.py` & `postpruner-0.7/postpruner/__main__.py`

 * *Files identical despite different names*

### Comparing `postpruner-0.6/postpruner/postpruner.py` & `postpruner-0.7/postpruner/postpruner.py`

 * *Files identical despite different names*

