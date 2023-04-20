# Comparing `tmp/motion_python-0.1.35.tar.gz` & `tmp/motion_python-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.35.tar", max compression
+gzip compressed data, was "motion_python-0.1.36.tar", max compression
```

## Comparing `motion_python-0.1.35.tar` & `motion_python-0.1.36.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3232 2023-04-19 17:21:20.053974 motion_python-0.1.35/README.md
--rw-r--r--   0        0        0      671 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/__init__.py
--rw-r--r--   0        0        0       80 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/api/__init__.py
--rw-r--r--   0        0        0     6684 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/api/api.py
--rw-r--r--   0        0        0      616 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/api/models.py
--rw-r--r--   0        0        0     3951 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/cli.py
--rw-r--r--   0        0        0    10092 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/client.py
--rw-r--r--   0        0        0    22261 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/cursor.py
--rw-r--r--   0        0        0    10037 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/entry.py
--rw-r--r--   0        0        0      214 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/basic/mconfig.py
--rw-r--r--   0        0        0        0 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/basic/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/basic/triggers/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/dashboard.py
--rw-r--r--   0        0        0      388 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/mconfig.py
--rw-r--r--   0        0        0       63 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/requirements.txt
--rw-r--r--   0        0        0       73 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/schemas/__init__.py
--rw-r--r--   0        0        0      398 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/schemas/all.py
--rw-r--r--   0        0        0     1377 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/test.py
--rw-r--r--   0        0        0      134 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/triggers/__init__.py
--rw-r--r--   0        0        0     4617 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/triggers/scrape.py
--rw-r--r--   0        0        0     5003 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/triggers/search.py
--rw-r--r--   0        0        0     2975 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/routing.py
--rw-r--r--   0        0        0     3413 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/schema.py
--rw-r--r--   0        0        0    15114 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/store.py
--rw-r--r--   0        0        0     3746 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/task.py
--rw-r--r--   0        0        0     6058 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/trigger.py
--rw-r--r--   0        0        0     1892 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/utils.py
--rw-r--r--   0        0        0     1578 2023-04-19 17:21:43.950314 motion_python-0.1.35/pyproject.toml
--rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 motion_python-0.1.35/PKG-INFO
+-rw-r--r--   0        0        0     3232 2023-04-20 00:28:04.015822 motion_python-0.1.36/README.md
+-rw-r--r--   0        0        0      671 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/api/__init__.py
+-rw-r--r--   0        0        0     6684 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/api/api.py
+-rw-r--r--   0        0        0      616 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/api/models.py
+-rw-r--r--   0        0        0     4000 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/cli.py
+-rw-r--r--   0        0        0    10092 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/client.py
+-rw-r--r--   0        0        0    22261 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/cursor.py
+-rw-r--r--   0        0        0    10037 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/entry.py
+-rw-r--r--   0        0        0      214 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/basic/mconfig.py
+-rw-r--r--   0        0        0        0 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/basic/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/basic/triggers/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/dashboard.py
+-rw-r--r--   0        0        0      388 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/mconfig.py
+-rw-r--r--   0        0        0       63 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/requirements.txt
+-rw-r--r--   0        0        0       73 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/schemas/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/schemas/all.py
+-rw-r--r--   0        0        0     1377 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/test.py
+-rw-r--r--   0        0        0      134 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/triggers/__init__.py
+-rw-r--r--   0        0        0     4617 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/triggers/scrape.py
+-rw-r--r--   0        0        0     5003 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/triggers/search.py
+-rw-r--r--   0        0        0     2975 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/routing.py
+-rw-r--r--   0        0        0     3413 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/schema.py
+-rw-r--r--   0        0        0    15114 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/store.py
+-rw-r--r--   0        0        0     3746 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/task.py
+-rw-r--r--   0        0        0     6058 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/trigger.py
+-rw-r--r--   0        0        0     1892 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/utils.py
+-rw-r--r--   0        0        0     1578 2023-04-20 00:28:24.264093 motion_python-0.1.36/pyproject.toml
+-rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 motion_python-0.1.36/PKG-INFO
```

### Comparing `motion_python-0.1.35/README.md` & `motion_python-0.1.36/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/__init__.py` & `motion_python-0.1.36/motion/__init__.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/api/api.py` & `motion_python-0.1.36/motion/api/api.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/api/models.py` & `motion_python-0.1.36/motion/api/models.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/cli.py` & `motion_python-0.1.36/motion/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,21 @@
     default="WARNING",
     help="Logging level for motion. Can be DEBUG, INFO, WARNING, ERROR, CRITICAL.",
 )
 def serve(name: str, host: str, port: int, logging_level: str) -> None:
     """Serves a Motion application."""
 
     # Check that the project is created
-    if not os.path.exists("mconfig.py"):
+    config_path = os.path.join(name, "mconfig.py")
+    if not os.path.exists(config_path):
         click.echo("Project is not created. Run `motion create` first.")
         return
 
     # Create object from mconfig.py
-    config_code = open("mconfig.py").read() + "\nMCONFIG"
+    config_code = open(config_path).read() + "\nMCONFIG"
 
     import sys
 
     sys.path.append(os.getcwd())
 
     exec(config_code)
     mconfig = locals()["MCONFIG"]
```

### Comparing `motion_python-0.1.35/motion/client.py` & `motion_python-0.1.36/motion/client.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/cursor.py` & `motion_python-0.1.36/motion/cursor.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/entry.py` & `motion_python-0.1.36/motion/entry.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/examples/cooking/dashboard.py` & `motion_python-0.1.36/motion/examples/cooking/dashboard.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/examples/cooking/test.py` & `motion_python-0.1.36/motion/examples/cooking/test.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/examples/cooking/triggers/scrape.py` & `motion_python-0.1.36/motion/examples/cooking/triggers/scrape.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/examples/cooking/triggers/search.py` & `motion_python-0.1.36/motion/examples/cooking/triggers/search.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/routing.py` & `motion_python-0.1.36/motion/routing.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/schema.py` & `motion_python-0.1.36/motion/schema.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/store.py` & `motion_python-0.1.36/motion/store.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/task.py` & `motion_python-0.1.36/motion/task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/trigger.py` & `motion_python-0.1.36/motion/trigger.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/motion/utils.py` & `motion_python-0.1.36/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.35/pyproject.toml` & `motion_python-0.1.36/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.35"
+version = "0.1.36"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.35/PKG-INFO` & `motion_python-0.1.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.35
+Version: 0.1.36
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

