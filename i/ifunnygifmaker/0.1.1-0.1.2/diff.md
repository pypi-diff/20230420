# Comparing `tmp/ifunnygifmaker-0.1.1.tar.gz` & `tmp/ifunnygifmaker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifunnygifmaker-0.1.1.tar", last modified: Thu Apr 20 03:21:57 2023, max compression
+gzip compressed data, was "ifunnygifmaker-0.1.2.tar", last modified: Thu Apr 20 03:23:47 2023, max compression
```

## Comparing `ifunnygifmaker-0.1.1.tar` & `ifunnygifmaker-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.1.1/README.md
--rw-r--r--   0        0        0       24 2023-04-20 03:21:22.080087 ifunnygifmaker-0.1.1/ifunnygifmaker/__init__.py
--rw-r--r--   0        0        0     4584 2023-04-20 03:18:39.381272 ifunnygifmaker-0.1.1/ifunnygifmaker/mememaker.py
--rw-r--r--   0        0        0      416 2023-04-20 03:21:54.010278 ifunnygifmaker-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.1.2/README.md
+-rw-r--r--   0        0        0       39 2023-04-20 03:23:31.127817 ifunnygifmaker-0.1.2/ifunnygifmaker/__init__.py
+-rw-r--r--   0        0        0     4584 2023-04-20 03:18:39.381272 ifunnygifmaker-0.1.2/ifunnygifmaker/mememaker.py
+-rw-r--r--   0        0        0      416 2023-04-20 03:23:42.932258 ifunnygifmaker-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.1.2/PKG-INFO
```

### Comparing `ifunnygifmaker-0.1.1/ifunnygifmaker/mememaker.py` & `ifunnygifmaker-0.1.2/ifunnygifmaker/mememaker.py`

 * *Files identical despite different names*

