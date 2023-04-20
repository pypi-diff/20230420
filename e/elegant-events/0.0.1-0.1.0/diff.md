# Comparing `tmp/elegant_events-0.0.1.tar.gz` & `tmp/elegant_events-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elegant_events-0.0.1.tar", last modified: Sun Apr  9 22:13:45 2023, max compression
+gzip compressed data, was "elegant_events-0.1.0.tar", last modified: Thu Apr 20 02:43:33 2023, max compression
```

## Comparing `elegant_events-0.0.1.tar` & `elegant_events-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-09 22:13:45.231292 elegant_events-0.0.1/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2480 2023-04-09 22:13:45.231135 elegant_events-0.0.1/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-09 22:13:45.229889 elegant_events-0.0.1/elegant_events/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     9674 2023-04-09 22:09:16.000000 elegant_events-0.0.1/elegant_events/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-09 22:13:45.230908 elegant_events-0.0.1/elegant_events.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2480 2023-04-09 22:13:44.000000 elegant_events-0.0.1/elegant_events.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      187 2023-04-09 22:13:45.000000 elegant_events-0.0.1/elegant_events.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-09 22:13:44.000000 elegant_events-0.0.1/elegant_events.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       15 2023-04-09 22:13:45.000000 elegant_events-0.0.1/elegant_events.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-09 22:13:45.231335 elegant_events-0.0.1/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1232 2023-04-09 21:21:22.000000 elegant_events-0.0.1/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 02:43:33.977573 elegant_events-0.1.0/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6330 2023-04-20 02:43:33.977419 elegant_events-0.1.0/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 02:43:33.976299 elegant_events-0.1.0/elegant_events/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    18421 2023-04-20 02:38:31.000000 elegant_events-0.1.0/elegant_events/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 02:43:33.977183 elegant_events-0.1.0/elegant_events.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6330 2023-04-20 02:43:33.000000 elegant_events-0.1.0/elegant_events.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      187 2023-04-20 02:43:33.000000 elegant_events-0.1.0/elegant_events.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-20 02:43:33.000000 elegant_events-0.1.0/elegant_events.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       15 2023-04-20 02:43:33.000000 elegant_events-0.1.0/elegant_events.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-20 02:43:33.977617 elegant_events-0.1.0/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1232 2023-04-09 21:21:22.000000 elegant_events-0.1.0/setup.py
```

### Comparing `elegant_events-0.0.1/setup.py` & `elegant_events-0.1.0/setup.py`

 * *Files identical despite different names*

