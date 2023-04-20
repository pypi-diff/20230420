# Comparing `tmp/poc_poetry_partifact_plugin-0.7.0.tar.gz` & `tmp/poc_poetry_partifact_plugin-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poc_poetry_partifact_plugin-0.7.0.tar", max compression
+gzip compressed data, was "poc_poetry_partifact_plugin-0.8.0.tar", max compression
```

## Comparing `poc_poetry_partifact_plugin-0.7.0.tar` & `poc_poetry_partifact_plugin-0.8.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        3 2023-04-20 19:11:13.591302 poc_poetry_partifact_plugin-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-04-20 19:11:13.591302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 19:11:13.591302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/__init__.py
--rw-r--r--   0        0        0     1478 2023-04-20 19:11:13.591302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/auth_token.py
--rw-r--r--   0        0        0     4479 2023-04-20 19:11:13.591302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/config.py
--rw-r--r--   0        0        0     1156 2023-04-20 19:11:13.591302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/main.py
--rw-r--r--   0        0        0     2089 2023-04-20 19:11:13.595302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/shell_commands.py
--rw-r--r--   0        0        0     3856 2023-04-20 19:11:13.595302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/plugin.py
--rw-r--r--   0        0        0     1088 2023-04-20 19:11:14.291314 poc_poetry_partifact_plugin-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 poc_poetry_partifact_plugin-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0        3 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/__init__.py
+-rw-r--r--   0        0        0     1478 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/auth_token.py
+-rw-r--r--   0        0        0     4479 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/config.py
+-rw-r--r--   0        0        0     1156 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/main.py
+-rw-r--r--   0        0        0     2089 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/shell_commands.py
+-rw-r--r--   0        0        0     4701 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/plugin.py
+-rw-r--r--   0        0        0     1088 2023-04-20 19:28:05.709350 poc_poetry_partifact_plugin-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 poc_poetry_partifact_plugin-0.8.0/PKG-INFO
```

### Comparing `poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/auth_token.py` & `poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/auth_token.py`

 * *Files identical despite different names*

### Comparing `poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/config.py` & `poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/config.py`

 * *Files identical despite different names*

### Comparing `poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/main.py` & `poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/main.py`

 * *Files identical despite different names*

### Comparing `poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/shell_commands.py` & `poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/shell_commands.py`

 * *Files identical despite different names*

### Comparing `poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/plugin.py` & `poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import subprocess
 from pathlib import Path
 from typing import Optional
 
-from cleo.events.console_events import TERMINATE
+from cleo.events.console_command_event import ConsoleCommandEvent
+from cleo.events.console_events import COMMAND, TERMINATE
 from cleo.events.console_terminate_event import ConsoleTerminateEvent
 from cleo.events.event_dispatcher import EventDispatcher
 from cleo.io.io import IO
 from cleo.io.outputs.output import Verbosity
 from poetry.console.application import Application
 from poetry.console.commands.add import AddCommand
 from poetry.console.commands.install import InstallCommand
@@ -15,20 +16,43 @@
 
 from poc_poetry_partifact_plugin.partifact.main import login
 
 
 class PocPartifactPlugin(ApplicationPlugin):  # type: ignore
     def activate(self, application: Application) -> None:
         application.event_dispatcher.add_listener(TERMINATE, self._handle_post_command)
+        application.event_dispatcher.add_listener(COMMAND, self._handle_pre_command)
+
+    def _handle_pre_command(
+        self, event: ConsoleCommandEvent, event_name: str, dispatcher: EventDispatcher
+    ) -> None:
+        """Run partifact.login before any Install or Add Commands"""
+        command = event.command
+        io = event.io
+
+        if isinstance(command, SelfCommand):
+            io.write_line(
+                "<info>Poetry pre-commit plugin does not run for 'self' command.</info>",
+                verbosity=Verbosity.DEBUG,
+            )
+            return
+
+        if not any(isinstance(command, t) for t in [InstallCommand, AddCommand]):
+            # Only run the plugin for install and add commands
+            return
+
+        # run a codeartifact login command
+        login(repository="aws", profile="amino-shared")
 
     def _handle_post_command(
         self, event: ConsoleTerminateEvent, event_name: str, dispatcher: EventDispatcher
     ) -> None:
         if event.exit_code != 0:
             # The command failed, so the plugin shouldn't do anything
+            # if the event was a "HTTPSConnectionPool" error, then try to login
             return
 
         command = event.command
         io = event.io
 
         if isinstance(command, SelfCommand):
             io.write_line(
@@ -37,18 +61,14 @@
             )
             return
 
         if not any(isinstance(command, t) for t in [InstallCommand, AddCommand]):
             # Only run the plugin for install and add commands
             return
 
-        # run a codeartifact login command.....
-        raise RuntimeError("hey thats enough")
-        # login(repository="aws", profile="amino-shared")
-
         if not self._is_pre_commit_package_installed():
             return
 
         if self._get_git_directory_path() is None:
             # Not in a git repository - can't install hooks
             return
```

### Comparing `poc_poetry_partifact_plugin-0.7.0/pyproject.toml` & `poc_poetry_partifact_plugin-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poc-poetry-partifact-plugin"
-version = "0.7.0"
+version = "0.8.0"
 description = "A POC poetry plugin that configure partifact"
 authors = ["timothestes <timothestes@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "poc_poetry_partifact_plugin" },
 ]
 homepage = "https://github.com/timothestes/poc-poetry-partifact-plugin"
```

### Comparing `poc_poetry_partifact_plugin-0.7.0/PKG-INFO` & `poc_poetry_partifact_plugin-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poc-poetry-partifact-plugin
-Version: 0.7.0
+Version: 0.8.0
 Summary: A POC poetry plugin that configure partifact
 Home-page: https://github.com/timothestes/poc-poetry-partifact-plugin
 Author: timothestes
 Author-email: timothestes@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

