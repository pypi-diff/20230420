# Comparing `tmp/exampleData-3.0.tar.gz` & `tmp/exampleData-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exampleData-3.0.tar", last modified: Thu Apr 20 09:03:52 2023, max compression
+gzip compressed data, was "exampleData-4.0.tar", last modified: Thu Apr 20 09:08:19 2023, max compression
```

## Comparing `exampleData-3.0.tar` & `exampleData-4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 09:03:52.146703 exampleData-3.0/
--rw-rw-rw-   0        0        0      300 2023-04-20 09:03:52.146703 exampleData-3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-20 09:03:52.140818 exampleData-3.0/exampleData/
--rw-rw-rw-   0        0        0       18 2023-04-20 08:30:44.000000 exampleData-3.0/exampleData/__init__.py
--rw-rw-rw-   0        0        0     2395 2023-04-16 02:11:42.000000 exampleData-3.0/exampleData/data.py
-drwxrwxrwx   0        0        0        0 2023-04-20 09:03:52.145281 exampleData-3.0/exampleData.egg-info/
--rw-rw-rw-   0        0        0      300 2023-04-20 09:03:52.000000 exampleData-3.0/exampleData.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-04-20 09:03:52.000000 exampleData-3.0/exampleData.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 09:03:52.000000 exampleData-3.0/exampleData.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-20 09:03:52.000000 exampleData-3.0/exampleData.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-20 09:03:52.000000 exampleData-3.0/exampleData.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 09:03:52.146703 exampleData-3.0/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-04-20 09:03:34.000000 exampleData-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:08:19.995416 exampleData-4.0/
+-rw-rw-rw-   0        0        0      300 2023-04-20 09:08:19.995416 exampleData-4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-20 09:08:19.979936 exampleData-4.0/exampleData/
+-rw-rw-rw-   0        0        0      163 2023-04-20 09:07:09.000000 exampleData-4.0/exampleData/__init__.py
+-rw-rw-rw-   0        0        0     2395 2023-04-16 02:11:42.000000 exampleData-4.0/exampleData/getdata.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:08:19.994313 exampleData-4.0/exampleData.egg-info/
+-rw-rw-rw-   0        0        0      300 2023-04-20 09:08:19.000000 exampleData-4.0/exampleData.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-04-20 09:08:19.000000 exampleData-4.0/exampleData.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 09:08:19.000000 exampleData-4.0/exampleData.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-20 09:08:19.000000 exampleData-4.0/exampleData.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 09:08:19.000000 exampleData-4.0/exampleData.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 09:08:19.995416 exampleData-4.0/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-04-20 09:07:29.000000 exampleData-4.0/setup.py
```

### Comparing `exampleData-3.0/exampleData/data.py` & `exampleData-4.0/exampleData/getdata.py`

 * *Files identical despite different names*

