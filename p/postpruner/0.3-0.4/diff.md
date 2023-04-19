# Comparing `tmp/postpruner-0.3.tar.gz` & `tmp/postpruner-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postpruner-0.3.tar", last modified: Wed Apr 19 23:06:55 2023, max compression
+gzip compressed data, was "postpruner-0.4.tar", last modified: Wed Apr 19 23:11:31 2023, max compression
```

## Comparing `postpruner-0.3.tar` & `postpruner-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:06:55.830639 postpruner-0.3/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:06:55.830639 postpruner-0.3/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-0.3/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:06:55.830639 postpruner-0.3/postpruner.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:06:55.000000 postpruner-0.3/postpruner.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      224 2023-04-19 23:06:55.000000 postpruner-0.3/postpruner.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:06:55.000000 postpruner-0.3/postpruner.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-19 23:06:55.000000 postpruner-0.3/postpruner.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-19 23:06:55.000000 postpruner-0.3/postpruner.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:06:55.000000 postpruner-0.3/postpruner.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-19 23:06:55.830639 postpruner-0.3/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      407 2023-04-19 23:06:52.000000 postpruner-0.3/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:11:31.522399 postpruner-0.4/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:11:31.522399 postpruner-0.4/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3648 2023-04-19 22:11:32.000000 postpruner-0.4/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:11:31.522399 postpruner-0.4/postpruner.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-19 23:11:31.000000 postpruner-0.4/postpruner.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      224 2023-04-19 23:11:31.000000 postpruner-0.4/postpruner.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:11:31.000000 postpruner-0.4/postpruner.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-19 23:11:31.000000 postpruner-0.4/postpruner.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-19 23:11:31.000000 postpruner-0.4/postpruner.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-19 23:11:31.000000 postpruner-0.4/postpruner.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-19 23:11:31.526399 postpruner-0.4/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      407 2023-04-19 23:11:29.000000 postpruner-0.4/setup.py
```

### Comparing `postpruner-0.3/README.md` & `postpruner-0.4/README.md`

 * *Files identical despite different names*

