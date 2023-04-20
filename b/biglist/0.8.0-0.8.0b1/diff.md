# Comparing `tmp/biglist-0.8.0.tar.gz` & `tmp/biglist-0.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biglist-0.8.0.tar", last modified: Thu Apr 20 04:42:19 2023, max compression
+gzip compressed data, was "biglist-0.8.0b1.tar", last modified: Mon Apr 17 15:38:20 2023, max compression
```

## Comparing `biglist-0.8.0.tar` & `biglist-0.8.0b1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.8.0/LICENSE
--rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.8.0/README.rst
--rw-r--r--   0        0        0     1623 2023-04-15 03:17:01.146252 biglist-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2215 2023-04-20 04:36:39.247126 biglist-0.8.0/src/biglist/__init__.py
--rw-r--r--   0        0        0    17990 2023-04-15 03:17:01.146252 biglist-0.8.0/src/biglist/_base.py
--rw-r--r--   0        0        0    44414 2023-04-15 03:17:01.146252 biglist-0.8.0/src/biglist/_biglist.py
--rw-r--r--   0        0        0    34773 2023-04-18 03:17:34.278504 biglist-0.8.0/src/biglist/_parquet.py
--rw-r--r--   0        0        0    12025 2023-04-14 07:17:29.111106 biglist-0.8.0/src/biglist/_util.py
--rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.8.0/src/biglist/py.typed
--rw-r--r--   0        0        0     2203 1970-01-01 00:00:00.000000 biglist-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.8.0b1/LICENSE
+-rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.8.0b1/README.rst
+-rw-r--r--   0        0        0     1623 2023-04-15 03:17:01.146252 biglist-0.8.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2217 2023-04-17 15:35:58.651653 biglist-0.8.0b1/src/biglist/__init__.py
+-rw-r--r--   0        0        0    17990 2023-04-15 03:17:01.146252 biglist-0.8.0b1/src/biglist/_base.py
+-rw-r--r--   0        0        0    44414 2023-04-15 03:17:01.146252 biglist-0.8.0b1/src/biglist/_biglist.py
+-rw-r--r--   0        0        0    34773 2023-04-17 15:34:16.400044 biglist-0.8.0b1/src/biglist/_parquet.py
+-rw-r--r--   0        0        0    12025 2023-04-14 07:17:29.111106 biglist-0.8.0b1/src/biglist/_util.py
+-rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.8.0b1/src/biglist/py.typed
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 biglist-0.8.0b1/PKG-INFO
```

### Comparing `biglist-0.8.0/LICENSE` & `biglist-0.8.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `biglist-0.8.0/README.rst` & `biglist-0.8.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `biglist-0.8.0/pyproject.toml` & `biglist-0.8.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biglist-0.8.0/src/biglist/__init__.py` & `biglist-0.8.0b1/src/biglist/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 )
 from ._util import (
     Chain,
     Seq,
     Slicer,
 )
 
-__version__ = "0.8.0"
+__version__ = "0.8.0b1"
```

### Comparing `biglist-0.8.0/src/biglist/_base.py` & `biglist-0.8.0b1/src/biglist/_base.py`

 * *Files identical despite different names*

### Comparing `biglist-0.8.0/src/biglist/_biglist.py` & `biglist-0.8.0b1/src/biglist/_biglist.py`

 * *Files identical despite different names*

### Comparing `biglist-0.8.0/src/biglist/_parquet.py` & `biglist-0.8.0b1/src/biglist/_parquet.py`

 * *Files identical despite different names*

### Comparing `biglist-0.8.0/src/biglist/_util.py` & `biglist-0.8.0b1/src/biglist/_util.py`

 * *Files identical despite different names*

### Comparing `biglist-0.8.0/PKG-INFO` & `biglist-0.8.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biglist
-Version: 0.8.0
+Version: 0.8.0b1
 Summary: The package `biglist <https://github.com/zpz/biglist>`_ provides persisted, out-of-memory Python data structures
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

