# Comparing `tmp/oida-0.1.4.tar.gz` & `tmp/oida-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oida-0.1.4.tar", max compression
+gzip compressed data, was "oida-0.1.5.tar", max compression
```

## Comparing `oida-0.1.4.tar` & `oida-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3663 2023-03-22 09:37:10.229793 oida-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-03-22 09:37:10.229793 oida-0.1.4/oida/__init__.py
--rw-r--r--   0        0        0       65 2023-03-22 09:37:10.229793 oida-0.1.4/oida/__main__.py
--rw-r--r--   0        0        0      616 2023-03-22 09:37:10.229793 oida-0.1.4/oida/checkers/__init__.py
--rw-r--r--   0        0        0     1628 2023-03-22 09:37:10.229793 oida-0.1.4/oida/checkers/base.py
--rw-r--r--   0        0        0     6855 2023-03-22 09:37:10.229793 oida-0.1.4/oida/checkers/components.py
--rw-r--r--   0        0        0     4325 2023-03-22 09:37:10.229793 oida-0.1.4/oida/checkers/config.py
--rw-r--r--   0        0        0     1334 2023-03-22 09:37:10.229793 oida-0.1.4/oida/checkers/imports.py
--rw-r--r--   0        0        0      190 2023-03-22 09:37:10.229793 oida-0.1.4/oida/commands/__init__.py
--rw-r--r--   0        0        0     9456 2023-03-22 09:37:10.233793 oida-0.1.4/oida/commands/componentize.py
--rw-r--r--   0        0        0     1007 2023-03-22 09:37:10.233793 oida-0.1.4/oida/commands/config.py
--rw-r--r--   0        0        0     1177 2023-03-22 09:37:10.233793 oida-0.1.4/oida/commands/linter.py
--rw-r--r--   0        0        0     1502 2023-03-22 09:37:10.233793 oida-0.1.4/oida/config.py
--rw-r--r--   0        0        0     5568 2023-03-22 09:37:10.233793 oida-0.1.4/oida/config_generator.py
--rw-r--r--   0        0        0     1875 2023-03-22 09:37:10.233793 oida-0.1.4/oida/console.py
--rw-r--r--   0        0        0     3755 2023-03-22 09:37:10.233793 oida-0.1.4/oida/discovery.py
--rw-r--r--   0        0        0     1245 2023-03-22 09:37:10.233793 oida-0.1.4/oida/flake8.py
--rw-r--r--   0        0        0      548 2023-03-22 09:37:10.233793 oida-0.1.4/oida/module.py
--rw-r--r--   0        0        0      515 2023-03-22 09:37:10.233793 oida-0.1.4/oida/utils.py
--rw-r--r--   0        0        0     1869 2023-03-22 09:37:10.233793 oida-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 oida-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3663 2023-04-20 08:33:56.049482 oida-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 08:33:56.049482 oida-0.1.5/oida/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-20 08:33:56.049482 oida-0.1.5/oida/__main__.py
+-rw-r--r--   0        0        0      616 2023-04-20 08:33:56.049482 oida-0.1.5/oida/checkers/__init__.py
+-rw-r--r--   0        0        0     1628 2023-04-20 08:33:56.049482 oida-0.1.5/oida/checkers/base.py
+-rw-r--r--   0        0        0     6855 2023-04-20 08:33:56.049482 oida-0.1.5/oida/checkers/components.py
+-rw-r--r--   0        0        0     4325 2023-04-20 08:33:56.049482 oida-0.1.5/oida/checkers/config.py
+-rw-r--r--   0        0        0     1334 2023-04-20 08:33:56.049482 oida-0.1.5/oida/checkers/imports.py
+-rw-r--r--   0        0        0      190 2023-04-20 08:33:56.049482 oida-0.1.5/oida/commands/__init__.py
+-rw-r--r--   0        0        0     9720 2023-04-20 08:33:56.049482 oida-0.1.5/oida/commands/componentize.py
+-rw-r--r--   0        0        0     1007 2023-04-20 08:33:56.049482 oida-0.1.5/oida/commands/config.py
+-rw-r--r--   0        0        0     1177 2023-04-20 08:33:56.049482 oida-0.1.5/oida/commands/linter.py
+-rw-r--r--   0        0        0     1502 2023-04-20 08:33:56.049482 oida-0.1.5/oida/config.py
+-rw-r--r--   0        0        0     5568 2023-04-20 08:33:56.049482 oida-0.1.5/oida/config_generator.py
+-rw-r--r--   0        0        0     1875 2023-04-20 08:33:56.049482 oida-0.1.5/oida/console.py
+-rw-r--r--   0        0        0     3755 2023-04-20 08:33:56.049482 oida-0.1.5/oida/discovery.py
+-rw-r--r--   0        0        0     1245 2023-04-20 08:33:56.049482 oida-0.1.5/oida/flake8.py
+-rw-r--r--   0        0        0      548 2023-04-20 08:33:56.049482 oida-0.1.5/oida/module.py
+-rw-r--r--   0        0        0      515 2023-04-20 08:33:56.049482 oida-0.1.5/oida/utils.py
+-rw-r--r--   0        0        0     1869 2023-04-20 08:33:56.049482 oida-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 oida-0.1.5/PKG-INFO
```

### Comparing `oida-0.1.4/README.md` & `oida-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/checkers/__init__.py` & `oida-0.1.5/oida/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/checkers/base.py` & `oida-0.1.5/oida/checkers/base.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/checkers/components.py` & `oida-0.1.5/oida/checkers/components.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/checkers/config.py` & `oida-0.1.5/oida/checkers/config.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/checkers/imports.py` & `oida-0.1.5/oida/checkers/imports.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/commands/componentize.py` & `oida-0.1.5/oida/commands/componentize.py`

 * *Files 5% similar despite different names*

```diff
@@ -235,22 +235,29 @@
                 new_decorator = decorator.with_changes(decorator=new_call)
                 return new_decorator
         return decorator
 
     def leave_FunctionDef(
         self, original_node: cst.FunctionDef, updated_node: cst.FunctionDef
     ) -> BaseStatement | FlattenSentinel[BaseStatement] | RemovalSentinel:
-        celery_task_decorator = m.Decorator(
+
+        # Matching tasks defined with @app.task
+        celery_app_task_decorator = m.Decorator(
             m.Call(m.Attribute(value=m.Name("app"), attr=m.Name("task")))
         )
+        # Matching tasks defined with @coalesced_task
+        celery_coalesced_task_decorator = m.Decorator(m.Call(m.Name("coalesced_task")))
+
         # The implicit name of the task is the path to the old module concatenated with the function name.
         task_name = f'"{self.module_name}.{original_node.name.value}"'
         decorators = [
             self.update_decorator(decorator=decorator, task_name=task_name)
-            if m.matches(decorator, celery_task_decorator)
+            if m.matches(
+                decorator, celery_app_task_decorator | celery_coalesced_task_decorator
+            )
             else decorator
             for decorator in updated_node.decorators
         ]
         return updated_node.with_changes(decorators=decorators)
 
 
 def update_celery_task_names(root_module: Path, old_path: Path, new_path: Path) -> None:
```

### Comparing `oida-0.1.4/oida/commands/config.py` & `oida-0.1.5/oida/commands/config.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/commands/linter.py` & `oida-0.1.5/oida/commands/linter.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/config.py` & `oida-0.1.5/oida/config.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/config_generator.py` & `oida-0.1.5/oida/config_generator.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/console.py` & `oida-0.1.5/oida/console.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/discovery.py` & `oida-0.1.5/oida/discovery.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/flake8.py` & `oida-0.1.5/oida/flake8.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/module.py` & `oida-0.1.5/oida/module.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/oida/utils.py` & `oida-0.1.5/oida/utils.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.4/pyproject.toml` & `oida-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oida"
-version = "0.1.4"
+version = "0.1.5"
 description = "Oida is Oda's linter that enforces code style and modularization in our Django projects."
 authors = ["Oda <tech@oda.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/oida"
 repository = "https://github.com/kolonialno/oida"
 classifiers = [
```

### Comparing `oida-0.1.4/PKG-INFO` & `oida-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oida
-Version: 0.1.4
+Version: 0.1.5
 Summary: Oida is Oda's linter that enforces code style and modularization in our Django projects.
 Home-page: https://github.com/kolonialno/oida
 License: MIT
 Author: Oda
 Author-email: tech@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

