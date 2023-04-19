# Comparing `tmp/postpruner-0.8.tar.gz` & `tmp/postpruner-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postpruner-0.8.tar", last modified: Wed Apr 19 23:19:18 2023, max compression
+gzip compressed data, was "postpruner-0.9.tar", last modified: Wed Apr 19 23:23:22 2023, max compression
```

## Comparing `postpruner-0.8.tar` & `postpruner-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:19:18.409993 postpruner-0.8/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:19:18.409993 postpruner-0.8/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-0.8/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:19:18.409993 postpruner-0.8/postpruner/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:14:28.000000 postpruner-0.8/postpruner/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1679 2023-04-19 23:17:05.000000 postpruner-0.8/postpruner/__main__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4996 2023-04-19 22:11:32.000000 postpruner-0.8/postpruner/generate_lut.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7983 2023-04-19 23:19:06.000000 postpruner-0.8/postpruner/postpruner.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:19:18.409993 postpruner-0.8/postpruner.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:19:18.000000 postpruner-0.8/postpruner.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      322 2023-04-19 23:19:18.000000 postpruner-0.8/postpruner.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:19:18.000000 postpruner-0.8/postpruner.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-19 23:19:18.000000 postpruner-0.8/postpruner.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-19 23:19:18.000000 postpruner-0.8/postpruner.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-19 23:19:18.000000 postpruner-0.8/postpruner.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-19 23:19:18.409993 postpruner-0.8/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      407 2023-04-19 23:19:15.000000 postpruner-0.8/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:23:22.893780 postpruner-0.9/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:23:22.893780 postpruner-0.9/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-0.9/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:23:22.893780 postpruner-0.9/postpruner/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:14:28.000000 postpruner-0.9/postpruner/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1680 2023-04-19 23:23:13.000000 postpruner-0.9/postpruner/__main__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4996 2023-04-19 22:11:32.000000 postpruner-0.9/postpruner/generate_lut.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7983 2023-04-19 23:19:06.000000 postpruner-0.9/postpruner/postpruner.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:23:22.893780 postpruner-0.9/postpruner.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:23:22.000000 postpruner-0.9/postpruner.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      322 2023-04-19 23:23:22.000000 postpruner-0.9/postpruner.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:23:22.000000 postpruner-0.9/postpruner.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-19 23:23:22.000000 postpruner-0.9/postpruner.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-19 23:23:22.000000 postpruner-0.9/postpruner.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-19 23:23:22.000000 postpruner-0.9/postpruner.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-19 23:23:22.893780 postpruner-0.9/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      407 2023-04-19 23:23:21.000000 postpruner-0.9/setup.py
```

### Comparing `postpruner-0.8/README.md` & `postpruner-0.9/README.md`

 * *Files identical despite different names*

### Comparing `postpruner-0.8/postpruner/__main__.py` & `postpruner-0.9/postpruner/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # __main__.py
 
 import sys
-from postpruner import run
+from .postpruner import run
 
 def main():
     import argparse
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--model_name", type=str, required=True)
     parser.add_argument("--task_name", type=str, required=True, choices=[
```

### Comparing `postpruner-0.8/postpruner/generate_lut.py` & `postpruner-0.9/postpruner/generate_lut.py`

 * *Files identical despite different names*

### Comparing `postpruner-0.8/postpruner/postpruner.py` & `postpruner-0.9/postpruner/postpruner.py`

 * *Files identical despite different names*

