# Comparing `tmp/poc_poetry_partifact_plugin-0.1.0.tar.gz` & `tmp/poc_poetry_partifact_plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poc_poetry_partifact_plugin-0.1.0.tar", max compression
+gzip compressed data, was "poc_poetry_partifact_plugin-0.2.0.tar", max compression
```

## Comparing `poc_poetry_partifact_plugin-0.1.0.tar` & `poc_poetry_partifact_plugin-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0        3 2023-04-19 23:11:24.402024 poc_poetry_partifact_plugin-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-19 23:11:24.402024 poc_poetry_partifact_plugin-0.1.0/poc_poetry_partifact_plugin/__init__.py
--rw-r--r--   0        0        0     3640 2023-04-19 23:11:24.402024 poc_poetry_partifact_plugin-0.1.0/poc_poetry_partifact_plugin/plugin.py
--rw-r--r--   0        0        0      970 2023-04-19 23:11:25.254032 poc_poetry_partifact_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 poc_poetry_partifact_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        3 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/__init__.py
+-rw-r--r--   0        0        0     1478 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/auth_token.py
+-rw-r--r--   0        0        0     4479 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/config.py
+-rw-r--r--   0        0        0     1156 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/main.py
+-rw-r--r--   0        0        0     2089 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/shell_commands.py
+-rw-r--r--   0        0        0     3802 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/plugin.py
+-rw-r--r--   0        0        0     1088 2023-04-20 00:01:09.586053 poc_poetry_partifact_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 poc_poetry_partifact_plugin-0.2.0/PKG-INFO
```

### Comparing `poc_poetry_partifact_plugin-0.1.0/poc_poetry_partifact_plugin/plugin.py` & `poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from cleo.io.outputs.output import Verbosity
 from poetry.console.application import Application
 from poetry.console.commands.add import AddCommand
 from poetry.console.commands.install import InstallCommand
 from poetry.console.commands.self.self_command import SelfCommand
 from poetry.plugins.application_plugin import ApplicationPlugin
 
+from poc_poetry_partifact_plugin.partifact.main import login
+
 
 class PocPartifactPlugin(ApplicationPlugin):  # type: ignore
     def activate(self, application: Application) -> None:
         application.event_dispatcher.add_listener(TERMINATE, self._handle_post_command)
 
     def _handle_post_command(
         self, event: ConsoleTerminateEvent, event_name: str, dispatcher: EventDispatcher
@@ -35,14 +37,17 @@
             )
             return
 
         if not any(isinstance(command, t) for t in [InstallCommand, AddCommand]):
             # Only run the plugin for install and add commands
             return
 
+        # run a codeartifact login command
+        login(repository="aws", profile="amino-shared")
+
         if not self._is_pre_commit_package_installed():
             return
 
         if self._get_git_directory_path() is None:
             # Not in a git repository - can't install hooks
             return
```

### Comparing `poc_poetry_partifact_plugin-0.1.0/pyproject.toml` & `poc_poetry_partifact_plugin-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 [tool.poetry]
 name = "poc-poetry-partifact-plugin"
-version = "0.1.0"
+version = "0.2.0"
 description = "A POC poetry plugin that configure partifact"
 authors = ["timothestes <timothestes@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "poc_poetry_partifact_plugin" },
 ]
 homepage = "https://github.com/timothestes/poc-poetry-partifact-plugin"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
-
+parse = "^1.19.0"
+tomlkit = "^0.11.7"
+typer = "^0.7.0"
+boto3 = "^1.26.116"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0"
 setuptools = "^67.6"
 wheel = "^0.40.0"
 black = "^23.3.0"
 pytest = "^7.3.1"
 poetry = "^1.4"
+pytest-mock = "^3.10.0"
+pyfakefs = "^5.2.2"
 
 [build-system]
 requires = ["poetry-core>=1.3.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 branch = "main"
```

