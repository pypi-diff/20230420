# Comparing `tmp/prettypy-0.2.0.tar.gz` & `tmp/prettypy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettypy-0.2.0.tar", last modified: Thu Feb 16 15:01:18 2023, max compression
+gzip compressed data, was "prettypy-0.2.1.tar", last modified: Thu Apr 20 14:52:18 2023, max compression
```

## Comparing `prettypy-0.2.0.tar` & `prettypy-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:01:18.228358 prettypy-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-16 15:01:07.000000 prettypy-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-02-16 15:01:18.228358 prettypy-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-02-16 15:01:07.000000 prettypy-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:01:18.228358 prettypy-0.2.0/prettypy/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-16 15:01:07.000000 prettypy-0.2.0/prettypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-02-16 15:01:07.000000 prettypy-0.2.0/prettypy/composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-02-16 15:01:07.000000 prettypy-0.2.0/prettypy/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-02-16 15:01:07.000000 prettypy-0.2.0/prettypy/pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-02-16 15:01:07.000000 prettypy-0.2.0/prettypy/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:01:18.228358 prettypy-0.2.0/prettypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-02-16 15:01:18.000000 prettypy-0.2.0/prettypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-16 15:01:18.000000 prettypy-0.2.0/prettypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 15:01:18.000000 prettypy-0.2.0/prettypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-16 15:01:18.000000 prettypy-0.2.0/prettypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-16 15:01:07.000000 prettypy-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-16 15:01:18.228358 prettypy-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:52:18.611119 prettypy-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 14:52:07.000000 prettypy-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-20 14:52:18.611119 prettypy-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-20 14:52:07.000000 prettypy-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:52:18.611119 prettypy-0.2.1/prettypy/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-20 14:52:07.000000 prettypy-0.2.1/prettypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-04-20 14:52:07.000000 prettypy-0.2.1/prettypy/composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-20 14:52:07.000000 prettypy-0.2.1/prettypy/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-20 14:52:07.000000 prettypy-0.2.1/prettypy/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-20 14:52:07.000000 prettypy-0.2.1/prettypy/pretty_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-20 14:52:07.000000 prettypy-0.2.1/prettypy/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:52:18.611119 prettypy-0.2.1/prettypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-20 14:52:18.000000 prettypy-0.2.1/prettypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-20 14:52:18.000000 prettypy-0.2.1/prettypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:52:18.000000 prettypy-0.2.1/prettypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 14:52:18.000000 prettypy-0.2.1/prettypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 14:52:07.000000 prettypy-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-20 14:52:18.611119 prettypy-0.2.1/setup.cfg
```

### Comparing `prettypy-0.2.0/LICENSE` & `prettypy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prettypy-0.2.0/prettypy/composer.py` & `prettypy-0.2.1/prettypy/composer.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     "negative": {
         "prefix": ["[", "red", "reset", "reset"],
         "text": ["-", "red", "reset", "reset"],
         "suffix": ["]", "red", "reset", "reset"],
     },
     "neutral": {
         "prefix": ["[", "reset", "reset", "reset"],
-        "text": ["~", "reset", "reset", "reset"],
+        "text": [" ", "reset", "reset", "reset"],
         "suffix": ["]", "reset", "reset", "reset"],
     },
 }
 
 
 class Composer:
     def __init__(self, no_color: bool = False) -> None:
@@ -127,15 +127,15 @@
     def get(self, name: str) -> Layout:
         """
         Get a layout from the composer.
         :param name: Name of the layout to get
         """
         return self._layouts.get(name)
 
-    def list(self) -> list:
+    def list_modes(self) -> list:
         """
         List all layouts.
         """
         return list(self._layouts.keys())
 
     def remove(self, item):
         """
```

### Comparing `prettypy-0.2.0/prettypy/layout.py` & `prettypy-0.2.1/prettypy/layout.py`

 * *Files identical despite different names*

### Comparing `prettypy-0.2.0/prettypy/style.py` & `prettypy-0.2.1/prettypy/style.py`

 * *Files identical despite different names*

### Comparing `prettypy-0.2.0/setup.cfg` & `prettypy-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prettypy
-version = 0.2.0
+version = 0.2.1
 author = zerodata
 author_email = zerodata@amissum.de
 description = A Python library to create pretty terminal output
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/uss-zerodata/prettypy
 project_urls =
```

