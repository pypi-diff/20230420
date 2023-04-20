# Comparing `tmp/poc_poetry_partifact_plugin-0.2.0.tar.gz` & `tmp/poc_poetry_partifact_plugin-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poc_poetry_partifact_plugin-0.2.0.tar", max compression
+gzip compressed data, was "poc_poetry_partifact_plugin-0.7.0.tar", max compression
```

## Comparing `poc_poetry_partifact_plugin-0.2.0.tar` & `poc_poetry_partifact_plugin-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        3 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/__init__.py
--rw-r--r--   0        0        0     1478 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/auth_token.py
--rw-r--r--   0        0        0     4479 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/config.py
--rw-r--r--   0        0        0     1156 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/main.py
--rw-r--r--   0        0        0     2089 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/shell_commands.py
--rw-r--r--   0        0        0     3802 2023-04-20 00:01:08.890054 poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/plugin.py
--rw-r--r--   0        0        0     1088 2023-04-20 00:01:09.586053 poc_poetry_partifact_plugin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 poc_poetry_partifact_plugin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        3 2023-04-20 19:11:13.591302 poc_poetry_partifact_plugin-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 19:11:13.591302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 19:11:13.591302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/__init__.py
+-rw-r--r--   0        0        0     1478 2023-04-20 19:11:13.591302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/auth_token.py
+-rw-r--r--   0        0        0     4479 2023-04-20 19:11:13.591302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/config.py
+-rw-r--r--   0        0        0     1156 2023-04-20 19:11:13.591302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/main.py
+-rw-r--r--   0        0        0     2089 2023-04-20 19:11:13.595302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/shell_commands.py
+-rw-r--r--   0        0        0     3856 2023-04-20 19:11:13.595302 poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/plugin.py
+-rw-r--r--   0        0        0     1088 2023-04-20 19:11:14.291314 poc_poetry_partifact_plugin-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 poc_poetry_partifact_plugin-0.7.0/PKG-INFO
```

### Comparing `poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/auth_token.py` & `poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/auth_token.py`

 * *Files identical despite different names*

### Comparing `poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/config.py` & `poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/config.py`

 * *Files identical despite different names*

### Comparing `poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/main.py` & `poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/main.py`

 * *Files identical despite different names*

### Comparing `poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/partifact/shell_commands.py` & `poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/partifact/shell_commands.py`

 * *Files identical despite different names*

### Comparing `poc_poetry_partifact_plugin-0.2.0/poc_poetry_partifact_plugin/plugin.py` & `poc_poetry_partifact_plugin-0.7.0/poc_poetry_partifact_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,17 @@
             )
             return
 
         if not any(isinstance(command, t) for t in [InstallCommand, AddCommand]):
             # Only run the plugin for install and add commands
             return
 
-        # run a codeartifact login command
-        login(repository="aws", profile="amino-shared")
+        # run a codeartifact login command.....
+        raise RuntimeError("hey thats enough")
+        # login(repository="aws", profile="amino-shared")
 
         if not self._is_pre_commit_package_installed():
             return
 
         if self._get_git_directory_path() is None:
             # Not in a git repository - can't install hooks
             return
```

### Comparing `poc_poetry_partifact_plugin-0.2.0/pyproject.toml` & `poc_poetry_partifact_plugin-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poc-poetry-partifact-plugin"
-version = "0.2.0"
+version = "0.7.0"
 description = "A POC poetry plugin that configure partifact"
 authors = ["timothestes <timothestes@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "poc_poetry_partifact_plugin" },
 ]
 homepage = "https://github.com/timothestes/poc-poetry-partifact-plugin"
```

### Comparing `poc_poetry_partifact_plugin-0.2.0/PKG-INFO` & `poc_poetry_partifact_plugin-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poc-poetry-partifact-plugin
-Version: 0.2.0
+Version: 0.7.0
 Summary: A POC poetry plugin that configure partifact
 Home-page: https://github.com/timothestes/poc-poetry-partifact-plugin
 Author: timothestes
 Author-email: timothestes@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

