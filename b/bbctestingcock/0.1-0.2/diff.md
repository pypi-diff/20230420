# Comparing `tmp/bbctestingcock-0.1.tar.gz` & `tmp/bbctestingcock-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbctestingcock-0.1.tar", last modified: Thu Apr 20 17:40:37 2023, max compression
+gzip compressed data, was "bbctestingcock-0.2.tar", last modified: Thu Apr 20 17:44:09 2023, max compression
```

## Comparing `bbctestingcock-0.1.tar` & `bbctestingcock-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 17:40:37.760185 bbctestingcock-0.1/
--rw-rw-rw-   0        0        0       92 2023-04-20 17:40:37.760185 bbctestingcock-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-20 17:40:37.751002 bbctestingcock-0.1/bbctestingcock/
--rw-rw-rw-   0        0        0      182 2023-04-20 17:39:28.000000 bbctestingcock-0.1/bbctestingcock/install.py
-drwxrwxrwx   0        0        0        0 2023-04-20 17:40:37.759688 bbctestingcock-0.1/bbctestingcock.egg-info/
--rw-rw-rw-   0        0        0       92 2023-04-20 17:40:37.000000 bbctestingcock-0.1/bbctestingcock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-20 17:40:37.000000 bbctestingcock-0.1/bbctestingcock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 17:40:37.000000 bbctestingcock-0.1/bbctestingcock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-04-20 17:40:37.000000 bbctestingcock-0.1/bbctestingcock.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-20 17:40:37.000000 bbctestingcock-0.1/bbctestingcock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 17:40:37.760185 bbctestingcock-0.1/setup.cfg
--rw-rw-rw-   0        0        0      304 2023-04-20 17:40:28.000000 bbctestingcock-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:44:09.339982 bbctestingcock-0.2/
+-rw-rw-rw-   0        0        0       92 2023-04-20 17:44:09.339487 bbctestingcock-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-20 17:44:09.332797 bbctestingcock-0.2/bbctestingcock/
+-rw-rw-rw-   0        0        0      182 2023-04-20 17:39:28.000000 bbctestingcock-0.2/bbctestingcock/install.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:44:09.338991 bbctestingcock-0.2/bbctestingcock.egg-info/
+-rw-rw-rw-   0        0        0       92 2023-04-20 17:44:09.000000 bbctestingcock-0.2/bbctestingcock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-20 17:44:09.000000 bbctestingcock-0.2/bbctestingcock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 17:44:09.000000 bbctestingcock-0.2/bbctestingcock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-04-20 17:44:09.000000 bbctestingcock-0.2/bbctestingcock.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-20 17:44:09.000000 bbctestingcock-0.2/bbctestingcock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 17:44:09.339982 bbctestingcock-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      304 2023-04-20 17:43:56.000000 bbctestingcock-0.2/setup.py
```

