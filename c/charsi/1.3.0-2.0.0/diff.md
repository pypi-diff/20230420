# Comparing `tmp/charsi-1.3.0.tar.gz` & `tmp/charsi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charsi-1.3.0.tar", max compression
+gzip compressed data, was "charsi-2.0.0.tar", max compression
```

## Comparing `charsi-1.3.0.tar` & `charsi-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      911 2023-04-18 12:46:56.678839 charsi-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2970 2023-04-18 12:46:31.505531 charsi-1.3.0/README.md
--rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-1.3.0/src/charsi/__init__.py
--rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-1.3.0/src/charsi/__main__.py
--rw-r--r--   0        0        0      335 2023-04-18 12:00:37.877409 charsi-1.3.0/src/charsi/asset.py
--rw-r--r--   0        0        0      141 2023-04-18 11:06:34.749797 charsi-1.3.0/src/charsi/commands/__init__.py
--rw-r--r--   0        0        0      896 2023-04-18 12:19:32.759387 charsi-1.3.0/src/charsi/commands/build.py
--rw-r--r--   0        0        0      684 2023-04-18 12:19:40.780769 charsi-1.3.0/src/charsi/commands/build_manifest.py
--rw-r--r--   0        0        0     2404 2023-04-18 12:41:16.038897 charsi-1.3.0/src/charsi/instruction.py
--rw-r--r--   0        0        0     1278 2023-04-18 10:59:27.587548 charsi-1.3.0/src/charsi/manifest.py
--rw-r--r--   0        0        0      818 2023-04-18 12:28:26.212247 charsi-1.3.0/src/charsi/recipe.py
--rw-r--r--   0        0        0     2132 2023-04-18 03:11:57.019672 charsi-1.3.0/src/charsi/strings.py
--rw-r--r--   0        0        0      551 2023-04-18 12:27:45.093226 charsi-1.3.0/src/charsi/utils.py
--rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 charsi-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1007 2023-04-20 07:29:24.095764 charsi-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3580 2023-04-20 07:28:46.454655 charsi-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-2.0.0/src/charsi/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-2.0.0/src/charsi/__main__.py
+-rw-r--r--   0        0        0      348 2023-04-19 12:44:19.623591 charsi-2.0.0/src/charsi/asset.py
+-rw-r--r--   0        0        0      141 2023-04-18 11:06:34.749797 charsi-2.0.0/src/charsi/commands/__init__.py
+-rw-r--r--   0        0        0      896 2023-04-20 07:14:22.978166 charsi-2.0.0/src/charsi/commands/build.py
+-rw-r--r--   0        0        0      684 2023-04-18 12:19:40.780769 charsi-2.0.0/src/charsi/commands/build_manifest.py
+-rw-r--r--   0        0        0     2602 2023-04-19 12:57:54.250514 charsi-2.0.0/src/charsi/instruction.py
+-rw-r--r--   0        0        0     1278 2023-04-18 10:59:27.587548 charsi-2.0.0/src/charsi/manifest.py
+-rw-r--r--   0        0        0     1294 2023-04-20 07:13:00.354859 charsi-2.0.0/src/charsi/recipe.py
+-rw-r--r--   0        0        0     2132 2023-04-18 03:11:57.019672 charsi-2.0.0/src/charsi/strings.py
+-rw-r--r--   0        0        0      551 2023-04-18 12:27:45.093226 charsi-2.0.0/src/charsi/utils.py
+-rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 charsi-2.0.0/PKG-INFO
```

### Comparing `charsi-1.3.0/pyproject.toml` & `charsi-2.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "charsi"
-version = "1.3.0"
+version = "2.0.0"
 description = "A command-line tool to help game modders build string resources for Diablo II: Resurrected."
 authors = ["HE Yaowen <he.yaowen@hotmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/he-yaowen/charsi"
 packages = [{include = "charsi", from = "src"}]
 
@@ -21,14 +21,16 @@
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.scripts]
 charsi = "charsi.__main__:cli"
 
 [tool.poe.tasks]
+dist = "poetry run pyinstaller charsi.spec"
 init = {shell ="poetry install && poetry run pre-commit install"}
 lint = "poetry run pylint src"
+publish = {shell ="poetry build && poetry publish"}
 test = "poetry run pytest --cov=src --cov-report=term-missing"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `charsi-1.3.0/README.md` & `charsi-2.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -76,18 +76,43 @@
    ```
 
 3. Discrete
    ```
    Instruction[qey, qhr]: ... # Khalim's Eye and Heart
    ```
 
+**Built-in Instructions**
+
+* `Text`: Replace string texts
+* `Color`: Set color of string text
+
+**Customize Instructions**
+
+Instructions are implemented by Lua scripts and put in directory `/instructions`
+
+**APIs for Lua to implement instructions**
+
+* `RegisterInstruction(name, fn)`: Register a new instruction.
+* `UnregisterInstruction(name)`: Unregister an existing instruction.
+* `InstructionRegistered(name)`: Check whether instruction is registered.
+
 ### Recipe
 
 A collection of instruction for building string tables.
 
+#### Recipe Tags
+
+You can set tags of recipes in format:
+
+```
+## Tag-name: value
+```
+
+`## Language`: The default language of instructions in this recipe
+
 ### Commands
 
 Build a string table with recipe:
 
 ```
 charsi build --recipe-file=/path/to/recipe path/to/stringtable
 ```
```

### Comparing `charsi-1.3.0/src/charsi/commands/build.py` & `charsi-2.0.0/src/charsi/commands/build.py`

 * *Files identical despite different names*

### Comparing `charsi-1.3.0/src/charsi/commands/build_manifest.py` & `charsi-2.0.0/src/charsi/commands/build_manifest.py`

 * *Files identical despite different names*

### Comparing `charsi-1.3.0/src/charsi/instruction.py` & `charsi-2.0.0/src/charsi/instruction.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,15 +72,23 @@
     def is_registered(self, name: str):
         return name in self._handlers
 
     def invoke(self, inst: Instruction, text: str) -> str:
         if not self.is_registered(inst.name):
             raise InstructionUndefinedError(inst.name)
 
-        return self._handlers[inst.name](text, *inst.args).replace('{origin}', text)
+        result = self._handlers[inst.name](text, *inst.args)
+
+        if isinstance(result, str):
+            return result.replace('{origin}', text)
+
+        if isinstance(result, tuple):
+            return result[0].replace('{origin}', text)
+
+        raise TypeError(type(result))
 
     def load_lua(self, codes: str):
         self._lua.execute(codes)
 
 
 class _InstructionInvokeError(Exception):
     ...
```

### Comparing `charsi-1.3.0/src/charsi/manifest.py` & `charsi-2.0.0/src/charsi/manifest.py`

 * *Files identical despite different names*

### Comparing `charsi-1.3.0/src/charsi/strings.py` & `charsi-2.0.0/src/charsi/strings.py`

 * *Files identical despite different names*

### Comparing `charsi-1.3.0/src/charsi/utils.py` & `charsi-2.0.0/src/charsi/utils.py`

 * *Files identical despite different names*

### Comparing `charsi-1.3.0/PKG-INFO` & `charsi-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charsi
-Version: 1.3.0
+Version: 2.0.0
 Summary: A command-line tool to help game modders build string resources for Diablo II: Resurrected.
 Home-page: https://github.com/he-yaowen/charsi
 License: GPL-3.0
 Author: HE Yaowen
 Author-email: he.yaowen@hotmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -95,18 +95,43 @@
    ```
 
 3. Discrete
    ```
    Instruction[qey, qhr]: ... # Khalim's Eye and Heart
    ```
 
+**Built-in Instructions**
+
+* `Text`: Replace string texts
+* `Color`: Set color of string text
+
+**Customize Instructions**
+
+Instructions are implemented by Lua scripts and put in directory `/instructions`
+
+**APIs for Lua to implement instructions**
+
+* `RegisterInstruction(name, fn)`: Register a new instruction.
+* `UnregisterInstruction(name)`: Unregister an existing instruction.
+* `InstructionRegistered(name)`: Check whether instruction is registered.
+
 ### Recipe
 
 A collection of instruction for building string tables.
 
+#### Recipe Tags
+
+You can set tags of recipes in format:
+
+```
+## Tag-name: value
+```
+
+`## Language`: The default language of instructions in this recipe
+
 ### Commands
 
 Build a string table with recipe:
 
 ```
 charsi build --recipe-file=/path/to/recipe path/to/stringtable
 ```
```

