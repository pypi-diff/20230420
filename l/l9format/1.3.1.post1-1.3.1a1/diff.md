# Comparing `tmp/l9format-1.3.1.post1.tar.gz` & `tmp/l9format-1.3.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l9format-1.3.1.post1.tar", max compression
+gzip compressed data, was "l9format-1.3.1a1.tar", max compression
```

## Comparing `l9format-1.3.1.post1.tar` & `l9format-1.3.1a1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-04-20 12:47:08.801924 l9format-1.3.1.post1/LICENSE
--rw-r--r--   0        0        0     1141 2023-04-20 12:47:08.801924 l9format-1.3.1.post1/README.md
--rw-r--r--   0        0        0       24 2023-04-20 12:47:08.801924 l9format-1.3.1.post1/l9format/__init__.py
--rw-r--r--   0        0        0     5252 2023-04-20 13:26:40.144004 l9format-1.3.1.post1/l9format/l9format.py
--rw-r--r--   0        0        0      794 2023-04-20 13:27:12.060195 l9format-1.3.1.post1/pyproject.toml
--rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 l9format-1.3.1.post1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-20 12:47:08.801924 l9format-1.3.1a1/LICENSE
+-rw-r--r--   0        0        0     1141 2023-04-20 12:47:08.801924 l9format-1.3.1a1/README.md
+-rw-r--r--   0        0        0       24 2023-04-20 12:47:08.801924 l9format-1.3.1a1/l9format/__init__.py
+-rw-r--r--   0        0        0     5252 2023-04-20 13:26:40.144004 l9format-1.3.1a1/l9format/l9format.py
+-rw-r--r--   0        0        0      794 2023-04-20 13:39:41.500706 l9format-1.3.1a1/pyproject.toml
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 l9format-1.3.1a1/PKG-INFO
```

### Comparing `l9format-1.3.1.post1/LICENSE` & `l9format-1.3.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `l9format-1.3.1.post1/README.md` & `l9format-1.3.1a1/README.md`

 * *Files identical despite different names*

### Comparing `l9format-1.3.1.post1/l9format/l9format.py` & `l9format-1.3.1a1/l9format/l9format.py`

 * *Files identical despite different names*

### Comparing `l9format-1.3.1.post1/pyproject.toml` & `l9format-1.3.1a1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "l9format"
-version = "1.3.1-1"
+version = "1.3.1a1"
 license = "MIT"
 description = "l9format is a schema declaration targeted at interoperability between network recon tools used at LeakIX"
 authors = ["Danny Willems <danny@leakix.net>"]
 maintainers = ["Danny Willems <danny@leakix.net>"]
 readme = "README.md"
 homepage = "https://github.com/leakix/l9format-python"
 repository = "https://github.com/leakix/l9format-python"
```

### Comparing `l9format-1.3.1.post1/PKG-INFO` & `l9format-1.3.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l9format
-Version: 1.3.1.post1
+Version: 1.3.1a1
 Summary: l9format is a schema declaration targeted at interoperability between network recon tools used at LeakIX
 Home-page: https://github.com/leakix/l9format-python
 License: MIT
 Author: Danny Willems
 Author-email: danny@leakix.net
 Maintainer: Danny Willems
 Maintainer-email: danny@leakix.net
```

