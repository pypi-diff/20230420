# Comparing `tmp/wicked_expressions-0.5.1.tar.gz` & `tmp/wicked_expressions-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicked_expressions-0.5.1.tar", max compression
+gzip compressed data, was "wicked_expressions-0.5.2.tar", max compression
```

## Comparing `wicked_expressions-0.5.1.tar` & `wicked_expressions-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1061 2023-04-20 15:55:23.467849 wicked_expressions-0.5.1/LICENSE
--rw-r--r--   0        0        0     2119 2023-04-20 15:55:23.467849 wicked_expressions-0.5.1/README.md
--rw-r--r--   0        0        0     1219 2023-04-20 15:56:42.338174 wicked_expressions-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      321 2023-04-20 15:56:42.318173 wicked_expressions-0.5.1/wicked_expressions/__init__.py
--rw-r--r--   0        0        0      783 2023-04-20 15:55:23.475849 wicked_expressions-0.5.1/wicked_expressions/modules/api.bolt
--rw-r--r--   0        0        0     7975 2023-04-20 15:55:23.475849 wicked_expressions-0.5.1/wicked_expressions/modules/comparison.bolt
--rw-r--r--   0        0        0      304 2023-04-20 15:55:23.475849 wicked_expressions-0.5.1/wicked_expressions/modules/config.bolt
--rw-r--r--   0        0        0     8309 2023-04-20 15:55:23.475849 wicked_expressions-0.5.1/wicked_expressions/modules/datastash.bolt
--rw-r--r--   0        0        0     1998 2023-04-20 15:55:23.475849 wicked_expressions-0.5.1/wicked_expressions/modules/internal_api.bolt
--rw-r--r--   0        0        0      341 2023-04-20 15:55:23.475849 wicked_expressions-0.5.1/wicked_expressions/modules/nbtlib.bolt
--rw-r--r--   0        0        0     8524 2023-04-20 15:55:23.475849 wicked_expressions-0.5.1/wicked_expressions/modules/raw_operations.bolt
--rw-r--r--   0        0        0     3127 2023-04-20 15:55:23.475849 wicked_expressions-0.5.1/wicked_expressions/modules/sources.bolt
--rw-r--r--   0        0        0     1181 2023-04-20 15:55:23.475849 wicked_expressions-0.5.1/wicked_expressions/modules/utils.bolt
--rw-r--r--   0        0        0     1220 2023-04-20 15:55:23.475849 wicked_expressions-0.5.1/wicked_expressions/modules/var.bolt
--rw-r--r--   0        0        0     5701 2023-04-20 15:55:23.475849 wicked_expressions-0.5.1/wicked_expressions/modules/var_sources.bolt
--rw-r--r--   0        0        0        0 2023-04-20 15:55:23.475849 wicked_expressions-0.5.1/wicked_expressions/py.typed
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-20 20:02:14.128563 wicked_expressions-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2119 2023-04-20 20:02:14.128563 wicked_expressions-0.5.2/README.md
+-rw-r--r--   0        0        0     1219 2023-04-20 20:03:24.614335 wicked_expressions-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-04-20 20:03:24.594334 wicked_expressions-0.5.2/wicked_expressions/__init__.py
+-rw-r--r--   0        0        0      783 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/api.bolt
+-rw-r--r--   0        0        0     7975 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/comparison.bolt
+-rw-r--r--   0        0        0      304 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/config.bolt
+-rw-r--r--   0        0        0     8309 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/datastash.bolt
+-rw-r--r--   0        0        0     1924 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/internal_api.bolt
+-rw-r--r--   0        0        0      341 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/nbtlib.bolt
+-rw-r--r--   0        0        0     8524 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/raw_operations.bolt
+-rw-r--r--   0        0        0     3127 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/sources.bolt
+-rw-r--r--   0        0        0     1181 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/utils.bolt
+-rw-r--r--   0        0        0     1220 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/var.bolt
+-rw-r--r--   0        0        0     5701 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/var_sources.bolt
+-rw-r--r--   0        0        0        0 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/py.typed
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.5.2/PKG-INFO
```

### Comparing `wicked_expressions-0.5.1/LICENSE` & `wicked_expressions-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.1/README.md` & `wicked_expressions-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.1/pyproject.toml` & `wicked_expressions-0.5.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wicked_expressions"
-version = "0.5.1"
+version = "0.5.2"
 description = "Extension of bolt-expressions written in Bolt."
 authors = ["Yeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/wicked-expressions"
 readme = "README.md"
```

### Comparing `wicked_expressions-0.5.1/wicked_expressions/modules/api.bolt` & `wicked_expressions-0.5.2/wicked_expressions/modules/api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.1/wicked_expressions/modules/comparison.bolt` & `wicked_expressions-0.5.2/wicked_expressions/modules/comparison.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.1/wicked_expressions/modules/datastash.bolt` & `wicked_expressions-0.5.2/wicked_expressions/modules/datastash.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.1/wicked_expressions/modules/internal_api.bolt` & `wicked_expressions-0.5.2/wicked_expressions/modules/internal_api.bolt`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,14 @@
             self.create_objective(name, criteria, display_name)
 
         return Score(self, name)
 
     def create_objective(self, objective_id: str, criteria: str, display_name: str | dict):
         setup_path = f"{Config.ROOT_LOCAL}/scoreboard_setup"
 
-        if display_name == None:
-            display_name = objective_id
-
         if isinstance(display_name, str):
             display_name = display_name
 
         merge function_tag minecraft:load {"values": [setup_path]}
         append function setup_path:
             if display_name is None:
                 scoreboard objectives add objective_id criteria
```

### Comparing `wicked_expressions-0.5.1/wicked_expressions/modules/raw_operations.bolt` & `wicked_expressions-0.5.2/wicked_expressions/modules/raw_operations.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.1/wicked_expressions/modules/sources.bolt` & `wicked_expressions-0.5.2/wicked_expressions/modules/sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.1/wicked_expressions/modules/utils.bolt` & `wicked_expressions-0.5.2/wicked_expressions/modules/utils.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.1/wicked_expressions/modules/var.bolt` & `wicked_expressions-0.5.2/wicked_expressions/modules/var.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.1/wicked_expressions/modules/var_sources.bolt` & `wicked_expressions-0.5.2/wicked_expressions/modules/var_sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.1/PKG-INFO` & `wicked_expressions-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicked-expressions
-Version: 0.5.1
+Version: 0.5.2
 Summary: Extension of bolt-expressions written in Bolt.
 Home-page: https://github.com/reapermc/wicked-expressions
 License: MIT
 Keywords: beet,bolt,minecraft,minecraft-commands,mcfunction
 Author: Yeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

