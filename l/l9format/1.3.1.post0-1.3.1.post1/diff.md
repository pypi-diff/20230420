# Comparing `tmp/l9format-1.3.1.post0.tar.gz` & `tmp/l9format-1.3.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l9format-1.3.1.post0.tar", max compression
+gzip compressed data, was "l9format-1.3.1.post1.tar", max compression
```

## Comparing `l9format-1.3.1.post0.tar` & `l9format-1.3.1.post1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2021-12-19 13:48:59.368064 l9format-1.3.1.post0/LICENSE
--rw-r--r--   0        0        0      996 2021-12-21 10:56:35.856023 l9format-1.3.1.post0/README.md
--rw-r--r--   0        0        0     5233 2021-12-21 09:45:39.520030 l9format-1.3.1.post0/l9format/l9format.py
--rw-r--r--   0        0        0      794 2021-12-21 11:05:22.272045 l9format-1.3.1.post0/pyproject.toml
--rw-r--r--   0        0        0     1789 2021-12-21 11:05:26.232160 l9format-1.3.1.post0/setup.py
--rw-r--r--   0        0        0     1968 2021-12-21 11:05:26.232360 l9format-1.3.1.post0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-20 12:47:08.801924 l9format-1.3.1.post1/LICENSE
+-rw-r--r--   0        0        0     1141 2023-04-20 12:47:08.801924 l9format-1.3.1.post1/README.md
+-rw-r--r--   0        0        0       24 2023-04-20 12:47:08.801924 l9format-1.3.1.post1/l9format/__init__.py
+-rw-r--r--   0        0        0     5252 2023-04-20 13:26:40.144004 l9format-1.3.1.post1/l9format/l9format.py
+-rw-r--r--   0        0        0      794 2023-04-20 13:27:12.060195 l9format-1.3.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 l9format-1.3.1.post1/PKG-INFO
```

### Comparing `l9format-1.3.1.post0/LICENSE` & `l9format-1.3.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `l9format-1.3.1.post0/README.md` & `l9format-1.3.1.post1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -13,27 +13,32 @@
 ```
 poetry install
 poetry run pytest l9format/tests/test_l9format.py
 ```
 
 ## Install
 
-Use main branch for the moment:
-```
-poetry add https://github.com/leakix/l9format-python#main
-```
+See [releases](https://github.com/LeakIX/l9format-python/releases/) for the
+different versions.
+The release `1.3.1-0` will be mapped to `1.3.1.post0`.
 
 ## Documentation
 
-```
+```python
 from l9format import l9format
 l9format.L9Event.from_dict(res)
 ```
 
 ## Versioning
 
 The versions will be synced with [l9format](https://github.com/leakix/l9format),
 suffixed by a number for bug fixes in the python implementation specifically.
 For instance, `1.3.1-0` will be the first version for `1.3.1` and follow
 https://github.com/LeakIX/l9format/releases/tag/v1.3.1. If a change is required
 for the Python package, but is the same specification than the Go
 implementation, the next release will be `1.3.1-1`.
+The version can be verified using
+
+```python
+import l9format
+l9format.__version__
+```
```

### Comparing `l9format-1.3.1.post0/l9format/l9format.py` & `l9format-1.3.1.post1/l9format/l9format.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,11 +169,11 @@
     protocol: fields.Str()
     http: fields.Nested(L9HttpEvent)
     summary: fields.Str()
     time: fields.DateTime()
     ssl: fields.Nested(L9SSLEvent)
     ssh: fields.Nested(L9SSHEvent)
     service: fields.Nested(L9ServiceEvent)
-    leak: fields.Nested(L9LeakEvent)
+    leak: fields.Optional(fields.Nested((L9LeakEvent)))
     tags: fields.Optional(fields.List(fields.Str()))
     geoip: fields.Nested(GeoLocation)
     network: fields.Nested(Network)
```

### Comparing `l9format-1.3.1.post0/pyproject.toml` & `l9format-1.3.1.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "l9format"
-version = "1.3.1-0"
+version = "1.3.1-1"
 license = "MIT"
 description = "l9format is a schema declaration targeted at interoperability between network recon tools used at LeakIX"
 authors = ["Danny Willems <danny@leakix.net>"]
 maintainers = ["Danny Willems <danny@leakix.net>"]
 readme = "README.md"
 homepage = "https://github.com/leakix/l9format-python"
 repository = "https://github.com/leakix/l9format-python"
```

### Comparing `l9format-1.3.1.post0/PKG-INFO` & `l9format-1.3.1.post1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: l9format
-Version: 1.3.1.post0
+Version: 1.3.1.post1
 Summary: l9format is a schema declaration targeted at interoperability between network recon tools used at LeakIX
 Home-page: https://github.com/leakix/l9format-python
 License: MIT
 Author: Danny Willems
 Author-email: danny@leakix.net
 Maintainer: Danny Willems
 Maintainer-email: danny@leakix.net
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: serde (>=0.8.1,<0.9.0)
 Project-URL: Bug Tracker, https://github.com/leakix/l9format-python/issues
 Project-URL: Documentation, https://github.com/leakix/l9format-python
 Project-URL: Repository, https://github.com/leakix/l9format-python
 Description-Content-Type: text/markdown
 
 l9format python
@@ -36,28 +37,33 @@
 ```
 poetry install
 poetry run pytest l9format/tests/test_l9format.py
 ```
 
 ## Install
 
-Use main branch for the moment:
-```
-poetry add https://github.com/leakix/l9format-python#main
-```
+See [releases](https://github.com/LeakIX/l9format-python/releases/) for the
+different versions.
+The release `1.3.1-0` will be mapped to `1.3.1.post0`.
 
 ## Documentation
 
-```
+```python
 from l9format import l9format
 l9format.L9Event.from_dict(res)
 ```
 
 ## Versioning
 
 The versions will be synced with [l9format](https://github.com/leakix/l9format),
 suffixed by a number for bug fixes in the python implementation specifically.
 For instance, `1.3.1-0` will be the first version for `1.3.1` and follow
 https://github.com/LeakIX/l9format/releases/tag/v1.3.1. If a change is required
 for the Python package, but is the same specification than the Go
 implementation, the next release will be `1.3.1-1`.
+The version can be verified using
+
+```python
+import l9format
+l9format.__version__
+```
```

