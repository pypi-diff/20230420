# Comparing `tmp/crowdcores-1.0.1.tar.gz` & `tmp/crowdcores-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdcores-1.0.1.tar", last modified: Wed Apr 19 22:55:35 2023, max compression
+gzip compressed data, was "crowdcores-1.0.2.tar", last modified: Wed Apr 19 22:58:54 2023, max compression
```

## Comparing `crowdcores-1.0.1.tar` & `crowdcores-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:55:35.119571 crowdcores-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 22:40:47.000000 crowdcores-1.0.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-19 22:55:35.119571 crowdcores-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      754 2023-04-19 22:48:59.000000 crowdcores-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:55:35.119571 crowdcores-1.0.1/crowdcores.egg-info/
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-19 22:55:35.000000 crowdcores-1.0.1/crowdcores.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2023-04-19 22:55:35.000000 crowdcores-1.0.1/crowdcores.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 22:55:35.000000 crowdcores-1.0.1/crowdcores.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-19 22:55:35.000000 crowdcores-1.0.1/crowdcores.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-19 22:55:35.000000 crowdcores-1.0.1/crowdcores.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:55:35.119571 crowdcores-1.0.1/pipeline/
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-19 22:54:59.000000 crowdcores-1.0.1/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)      835 2023-04-19 22:47:45.000000 crowdcores-1.0.1/pipeline/pipeline.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 22:55:35.119571 crowdcores-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      176 2023-04-19 22:55:23.000000 crowdcores-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:58:54.974852 crowdcores-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 22:40:47.000000 crowdcores-1.0.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-19 22:58:54.974852 crowdcores-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      754 2023-04-19 22:48:59.000000 crowdcores-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:58:54.974852 crowdcores-1.0.2/crowdcores/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-19 22:58:43.000000 crowdcores-1.0.2/crowdcores/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      835 2023-04-19 22:47:45.000000 crowdcores-1.0.2/crowdcores/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 22:58:54.974852 crowdcores-1.0.2/crowdcores.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-19 22:58:54.000000 crowdcores-1.0.2/crowdcores.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2023-04-19 22:58:54.000000 crowdcores-1.0.2/crowdcores.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 22:58:54.000000 crowdcores-1.0.2/crowdcores.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-19 22:58:54.000000 crowdcores-1.0.2/crowdcores.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-19 22:58:54.000000 crowdcores-1.0.2/crowdcores.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 22:58:54.974852 crowdcores-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      176 2023-04-19 22:58:50.000000 crowdcores-1.0.2/setup.py
```

### Comparing `crowdcores-1.0.1/LICENSE.txt` & `crowdcores-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdcores-1.0.1/README.md` & `crowdcores-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `crowdcores-1.0.1/pipeline/pipeline.py` & `crowdcores-1.0.2/crowdcores/pipeline.py`

 * *Files identical despite different names*

