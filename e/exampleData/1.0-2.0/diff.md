# Comparing `tmp/exampleData-1.0.tar.gz` & `tmp/exampleData-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exampleData-1.0.tar", last modified: Thu Apr 20 07:41:19 2023, max compression
+gzip compressed data, was "exampleData-2.0.tar", last modified: Thu Apr 20 08:44:34 2023, max compression
```

## Comparing `exampleData-1.0.tar` & `exampleData-2.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 07:41:19.181140 exampleData-1.0/
--rw-rw-rw-   0        0        0      300 2023-04-20 07:41:19.181140 exampleData-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-20 07:41:19.179850 exampleData-1.0/exampleData.egg-info/
--rw-rw-rw-   0        0        0      300 2023-04-20 07:41:19.000000 exampleData-1.0/exampleData.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-20 07:41:19.000000 exampleData-1.0/exampleData.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 07:41:19.000000 exampleData-1.0/exampleData.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-20 07:41:19.000000 exampleData-1.0/exampleData.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 07:41:19.000000 exampleData-1.0/exampleData.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 07:41:19.181140 exampleData-1.0/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-04-20 07:41:16.000000 exampleData-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:44:34.350335 exampleData-2.0/
+-rw-rw-rw-   0        0        0      300 2023-04-20 08:44:34.349335 exampleData-2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-20 08:44:34.342947 exampleData-2.0/exampleData/
+-rw-rw-rw-   0        0        0       18 2023-04-20 08:30:44.000000 exampleData-2.0/exampleData/__init__.py
+-rw-rw-rw-   0        0        0     2395 2023-04-16 02:11:42.000000 exampleData-2.0/exampleData/data.py
+drwxrwxrwx   0        0        0        0 2023-04-20 08:44:34.348333 exampleData-2.0/exampleData.egg-info/
+-rw-rw-rw-   0        0        0      300 2023-04-20 08:44:34.000000 exampleData-2.0/exampleData.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-20 08:44:34.000000 exampleData-2.0/exampleData.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 08:44:34.000000 exampleData-2.0/exampleData.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-20 08:44:34.000000 exampleData-2.0/exampleData.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 08:44:34.000000 exampleData-2.0/exampleData.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 08:44:34.350335 exampleData-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-04-20 08:41:58.000000 exampleData-2.0/setup.py
```

