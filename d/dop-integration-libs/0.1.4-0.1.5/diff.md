# Comparing `tmp/dop_integration_libs-0.1.4.tar.gz` & `tmp/dop_integration_libs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dop_integration_libs-0.1.4.tar", max compression
+gzip compressed data, was "dop_integration_libs-0.1.5.tar", max compression
```

## Comparing `dop_integration_libs-0.1.4.tar` & `dop_integration_libs-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142210 dop_integration_libs-0.1.4/README.md
--rw-r--r--   0        0        0     1451 2023-04-20 11:57:35.314673 dop_integration_libs-0.1.4/dop_integration_libs/Logger.py
--rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142161 dop_integration_libs-0.1.4/dop_integration_libs/__init__.py
--rw-r--r--   0        0        0       31 2023-04-19 13:09:13.173725 dop_integration_libs-0.1.4/dop_integration_libs/__main__.py
--rw-r--r--   0        0        0     1724 2023-04-20 09:38:46.129610 dop_integration_libs-0.1.4/dop_integration_libs/environment.py
--rw-r--r--   0        0        0      389 2023-04-20 11:57:41.452346 dop_integration_libs-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 dop_integration_libs-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142210 dop_integration_libs-0.1.5/README.md
+-rw-r--r--   0        0        0     2264 2023-04-20 12:13:51.624660 dop_integration_libs-0.1.5/dop_integration_libs/Logger.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:06:06.142161 dop_integration_libs-0.1.5/dop_integration_libs/__init__.py
+-rw-r--r--   0        0        0       31 2023-04-19 13:09:13.173725 dop_integration_libs-0.1.5/dop_integration_libs/__main__.py
+-rw-r--r--   0        0        0     1724 2023-04-20 09:38:46.129610 dop_integration_libs-0.1.5/dop_integration_libs/environment.py
+-rw-r--r--   0        0        0      389 2023-04-20 12:14:08.255674 dop_integration_libs-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 dop_integration_libs-0.1.5/PKG-INFO
```

### Comparing `dop_integration_libs-0.1.4/dop_integration_libs/environment.py` & `dop_integration_libs-0.1.5/dop_integration_libs/environment.py`

 * *Files identical despite different names*

