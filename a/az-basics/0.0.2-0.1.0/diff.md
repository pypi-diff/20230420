# Comparing `tmp/az_basics-0.0.2.tar.gz` & `tmp/az_basics-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "az_basics-0.0.2.tar", max compression
+gzip compressed data, was "az_basics-0.1.0.tar", max compression
```

## Comparing `az_basics-0.0.2.tar` & `az_basics-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0       50 2023-04-18 12:34:37.931466 az_basics-0.0.2/az_basics/__init__.py
--rw-r--r--   0        0        0      108 2023-04-18 12:27:26.192839 az_basics-0.0.2/az_basics/toy.py
--rw-r--r--   0        0        0      482 2023-04-18 14:20:08.599334 az_basics-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       45 2023-04-18 13:32:09.541025 az_basics-0.0.2/README.md
--rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 az_basics-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       45 2023-04-20 06:16:42.000000 az_basics-0.1.0/az_basics/__init__.py
+-rw-r--r--   0        0        0     3905 2023-04-20 14:02:28.000000 az_basics-0.1.0/az_basics/connection_string_based.py
+-rw-r--r--   0        0        0     3168 2023-04-20 14:47:46.000000 az_basics-0.1.0/az_basics/sas_token_based.py
+-rw-r--r--   0        0        0      108 2023-04-18 12:27:26.192839 az_basics-0.1.0/az_basics/toy.py
+-rw-r--r--   0        0        0      515 2023-04-20 17:14:55.839040 az_basics-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-04-18 13:32:09.541025 az_basics-0.1.0/README.md
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 az_basics-0.1.0/PKG-INFO
```

### Comparing `az_basics-0.0.2/PKG-INFO` & `az_basics-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: az-basics
-Version: 0.0.2
+Version: 0.1.0
 Summary: A python library to perform azure blob operations such as list, delete, upload and download
 Author: Prithivee
 Author-email: getprithivee@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

