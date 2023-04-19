# Comparing `tmp/flet_pyodide-0.6.0.dev1322.tar.gz` & `tmp/flet_pyodide-0.6.0.dev1336.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_pyodide-0.6.0.dev1322.tar", max compression
+gzip compressed data, was "flet_pyodide-0.6.0.dev1336.tar", max compression
```

## Comparing `flet_pyodide-0.6.0.dev1322.tar` & `flet_pyodide-0.6.0.dev1336.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2264 2023-04-17 18:18:07.065538 flet_pyodide-0.6.0.dev1322/README.md
--rw-r--r--   0        0        0      644 2023-04-17 18:18:47.965178 flet_pyodide-0.6.0.dev1322/pyproject.toml
--rw-r--r--   0        0        0      101 2023-04-17 18:18:07.065538 flet_pyodide-0.6.0.dev1322/src/flet/__init__.py
--rw-r--r--   0        0        0     2377 2023-04-17 18:18:07.065538 flet_pyodide-0.6.0.dev1322/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-04-17 18:18:07.065538 flet_pyodide-0.6.0.dev1322/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-04-17 18:18:07.065538 flet_pyodide-0.6.0.dev1322/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3861 2023-04-17 18:18:07.065538 flet_pyodide-0.6.0.dev1322/src/flet/pyodide_connection.py
--rw-r--r--   0        0        0      103 2023-04-17 18:18:47.277181 flet_pyodide-0.6.0.dev1322/src/flet/version.py
--rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.6.0.dev1322/PKG-INFO
+-rw-r--r--   0        0        0     2264 2023-04-19 23:40:35.342384 flet_pyodide-0.6.0.dev1336/README.md
+-rw-r--r--   0        0        0      644 2023-04-19 23:41:12.155761 flet_pyodide-0.6.0.dev1336/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-04-19 23:40:35.342384 flet_pyodide-0.6.0.dev1336/src/flet/__init__.py
+-rw-r--r--   0        0        0     2377 2023-04-19 23:40:35.342384 flet_pyodide-0.6.0.dev1336/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-04-19 23:40:35.342384 flet_pyodide-0.6.0.dev1336/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-04-19 23:40:35.342384 flet_pyodide-0.6.0.dev1336/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3851 2023-04-19 23:40:35.342384 flet_pyodide-0.6.0.dev1336/src/flet/pyodide_connection.py
+-rw-r--r--   0        0        0      103 2023-04-19 23:41:11.511776 flet_pyodide-0.6.0.dev1336/src/flet/version.py
+-rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.6.0.dev1336/PKG-INFO
```

### Comparing `flet_pyodide-0.6.0.dev1322/README.md` & `flet_pyodide-0.6.0.dev1336/README.md`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.6.0.dev1322/pyproject.toml` & `flet_pyodide-0.6.0.dev1336/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-pyodide"
-version = "0.6.0.dev1322"
+version = "0.6.0.dev1336"
 description = "Flet for Pyodide - build standalone SPA in Python with Flutter UI."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.6.0.dev1322"
+flet-core = "0.6.0.dev1336"
 python = "^3.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `flet_pyodide-0.6.0.dev1322/src/flet/flet.py` & `flet_pyodide-0.6.0.dev1336/src/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.6.0.dev1322/src/flet/pyodide_connection.py` & `flet_pyodide-0.6.0.dev1336/src/flet/pyodide_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         elif msg.action == ClientActions.UPDATE_CONTROL_PROPS:
             if self.__on_event is not None:
                 asyncio.create_task(
                     self.__on_event(self._create_update_control_props_handler_arg(msg))
                 )
         else:
             # it's something else
-            raise Exception('Unknown message "{}": {}'.format(msg.action, msg.payload))
+            raise Exception(f'Unknown message "{msg.action}": {msg.payload}')
 
     async def send_command_async(self, session_id: str, command: Command):
         return self.send_command(session_id, command)
 
     def send_command(self, session_id: str, command: Command):
         result, message = self._process_command(command)
         if message:
```

### Comparing `flet_pyodide-0.6.0.dev1322/PKG-INFO` & `flet_pyodide-0.6.0.dev1336/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: flet-pyodide
-Version: 0.6.0.dev1322
+Version: 0.6.0.dev1336
 Summary: Flet for Pyodide - build standalone SPA in Python with Flutter UI.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.6.0.dev1322)
+Requires-Dist: flet-core (==0.6.0.dev1336)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet for Pyodide - build standalone Single-Page Applications (SPA) in Python with Flutter UI
```

