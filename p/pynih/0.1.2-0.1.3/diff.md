# Comparing `tmp/pynih-0.1.2.tar.gz` & `tmp/pynih-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynih-0.1.2.tar", max compression
+gzip compressed data, was "pynih-0.1.3.tar", max compression
```

## Comparing `pynih-0.1.2.tar` & `pynih-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-20 15:11:27.766601 pynih-0.1.2/LICENSE
--rw-r--r--   0        0        0      811 2023-04-20 15:11:27.766601 pynih-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-20 15:11:27.766601 pynih-0.1.2/pynih/__init__.py
--rw-r--r--   0        0        0     3070 2023-04-20 15:11:27.766601 pynih-0.1.2/pynih/apis.py
--rw-r--r--   0        0        0      621 2023-04-20 15:11:27.766601 pynih-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 pynih-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-20 18:38:45.022628 pynih-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1881 2023-04-20 18:38:45.022628 pynih-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 18:38:45.026628 pynih-0.1.3/pynih/__init__.py
+-rw-r--r--   0        0        0     3070 2023-04-20 18:38:45.026628 pynih-0.1.3/pynih/apis.py
+-rw-r--r--   0        0        0      621 2023-04-20 18:38:45.026628 pynih-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 pynih-0.1.3/PKG-INFO
```

### Comparing `pynih-0.1.2/LICENSE` & `pynih-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynih-0.1.2/pynih/apis.py` & `pynih-0.1.3/pynih/apis.py`

 * *Files identical despite different names*

### Comparing `pynih-0.1.2/pyproject.toml` & `pynih-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynih"
-version = "0.1.2"
+version = "0.1.3"
 description = "python wrapper for nih reporter apis --> https://api.reporter.nih.gov/"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pynih"}]
 
 license = "MIT"
```

