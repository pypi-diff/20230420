# Comparing `tmp/leakix-0.1.5.tar.gz` & `tmp/leakix-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leakix-0.1.5.tar", max compression
+gzip compressed data, was "leakix-0.1.6.tar", max compression
```

## Comparing `leakix-0.1.5.tar` & `leakix-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-02-16 21:37:48.489430 leakix-0.1.5/LICENSE
--rw-r--r--   0        0        0      202 2023-02-16 21:37:48.493430 leakix-0.1.5/leakix/__init__.py
--rw-r--r--   0        0        0     3623 2023-02-17 19:19:16.649369 leakix-0.1.5/leakix/client.py
--rw-r--r--   0        0        0     1950 2023-02-17 19:18:32.211069 leakix-0.1.5/leakix/field.py
--rw-r--r--   0        0        0     1999 2023-02-16 21:37:48.493430 leakix-0.1.5/leakix/plugin.py
--rw-r--r--   0        0        0      876 2023-02-16 21:37:48.493430 leakix-0.1.5/leakix/query.py
--rw-r--r--   0        0        0     1201 2023-02-17 18:53:20.035647 leakix-0.1.5/leakix/response.py
--rw-r--r--   0        0        0      460 2023-02-17 19:24:37.393095 leakix-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 leakix-0.1.5/setup.py
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 leakix-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-18 18:11:59.120818 leakix-0.1.6/LICENSE
+-rw-r--r--   0        0        0      202 2023-04-18 18:11:59.120818 leakix-0.1.6/leakix/__init__.py
+-rw-r--r--   0        0        0     3623 2023-04-20 13:25:58.427754 leakix-0.1.6/leakix/client.py
+-rw-r--r--   0        0        0     1950 2023-04-18 18:11:59.120818 leakix-0.1.6/leakix/field.py
+-rw-r--r--   0        0        0     1999 2023-04-18 18:11:59.120818 leakix-0.1.6/leakix/plugin.py
+-rw-r--r--   0        0        0      876 2023-04-18 18:11:59.120818 leakix-0.1.6/leakix/query.py
+-rw-r--r--   0        0        0     1201 2023-04-18 18:11:59.120818 leakix-0.1.6/leakix/response.py
+-rw-r--r--   0        0        0      462 2023-04-20 14:12:22.688286 leakix-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 leakix-0.1.6/PKG-INFO
```

### Comparing `leakix-0.1.5/LICENSE` & `leakix-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `leakix-0.1.5/leakix/client.py` & `leakix-0.1.6/leakix/client.py`

 * *Files identical despite different names*

### Comparing `leakix-0.1.5/leakix/field.py` & `leakix-0.1.6/leakix/field.py`

 * *Files identical despite different names*

### Comparing `leakix-0.1.5/leakix/plugin.py` & `leakix-0.1.6/leakix/plugin.py`

 * *Files identical despite different names*

### Comparing `leakix-0.1.5/leakix/query.py` & `leakix-0.1.6/leakix/query.py`

 * *Files identical despite different names*

### Comparing `leakix-0.1.5/leakix/response.py` & `leakix-0.1.6/leakix/response.py`

 * *Files identical despite different names*

### Comparing `leakix-0.1.5/PKG-INFO` & `leakix-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: leakix
-Version: 0.1.5
+Version: 0.1.6
 Summary: Official python client for LeakIX (https://leakix.net)
 Author: Danny Willems
 Author-email: danny@leakix.net
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: l9format (>=1.3.1,<2.0.0)
+Requires-Dist: l9format (==1.3.1a1)
 Requires-Dist: requests
```

