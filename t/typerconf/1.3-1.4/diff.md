# Comparing `tmp/typerconf-1.3.tar.gz` & `tmp/typerconf-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typerconf-1.3.tar", max compression
+gzip compressed data, was "typerconf-1.4.tar", max compression
```

## Comparing `typerconf-1.3.tar` & `typerconf-1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-1.3/LICENSE
--rw-r--r--   0        0        0     1363 2023-03-24 07:02:49.103915 typerconf-1.3/README.md
--rw-r--r--   0        0        0      934 2023-04-03 09:28:30.993764 typerconf-1.3/pyproject.toml
--rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-1.3/src/typerconf/.gitignore
--rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-1.3/src/typerconf/Makefile
--rw-r--r--   0        0        0     6259 2023-04-03 09:29:07.116989 typerconf-1.3/src/typerconf/__init__.py
--rw-r--r--   0        0        0    14728 2023-04-03 09:27:38.383037 typerconf-1.3/src/typerconf/init.nw
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 typerconf-1.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-1.4/LICENSE
+-rw-r--r--   0        0        0     1363 2023-03-24 07:02:49.103915 typerconf-1.4/README.md
+-rw-r--r--   0        0        0      934 2023-04-20 07:42:25.027099 typerconf-1.4/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-1.4/src/typerconf/.gitignore
+-rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-1.4/src/typerconf/Makefile
+-rw-r--r--   0        0        0     6692 2023-04-20 07:42:46.010795 typerconf-1.4/src/typerconf/__init__.py
+-rw-r--r--   0        0        0    16558 2023-04-20 07:40:09.981015 typerconf-1.4/src/typerconf/init.nw
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 typerconf-1.4/PKG-INFO
```

### Comparing `typerconf-1.3/LICENSE` & `typerconf-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `typerconf-1.3/README.md` & `typerconf-1.4/README.md`

 * *Files identical despite different names*

### Comparing `typerconf-1.3/pyproject.toml` & `typerconf-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typerconf"
-version = "1.3"
+version = "1.4"
 description = "Library to read and write configs using API and CLI with Typer"
 authors = ["Daniel Bosk <daniel@bosk.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/typerconf"
 keywords = ["typer", "conf", "config", "git-like", "config lib", "write conf"]
 classifiers = [
```

### Comparing `typerconf-1.3/src/typerconf/__init__.py` & `typerconf-1.4/src/typerconf/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,37 +58,50 @@
     Example:
     - `value = "https://..."`,
     - `path = "courses.datintro22.url"`
     will create `{"courses": {"datintro22": {"url": "https://..."}}}`.
 
     Any part of the path that can be converted to an integer, will be converted 
     to an integer. This way we can access elements of lists too. However, we 
-    cannot create index 3 in a list if it doesn't exist.
+    cannot create index 3 in a list if it doesn't exist (we can't expand 
+    lists).
+
+    If `value` is `None`, the entry at `path` will be deleted, if it exists.
     """
     structure = self.__data
 
     parts = path.split(".")
+
     for part in parts[:-1]:
       try:
         part = int(part)
       except ValueError:
         pass
-
       try:
         structure = structure[part]
       except KeyError:
-        structure[part] = {}
-        structure = structure[part]
+        if value is None:
+          return
+        else:
+          structure[part] = {}
+          structure = structure[part]
 
     part = parts[-1]
     try:
       part = int(part)
     except ValueError:
       pass
-    structure[part] = value
+
+    if value is None:
+      try:
+        del structure[part]
+      except KeyError:
+        pass
+    else:
+      structure[part] = value
 
   def paths(self, from_root=""):
     """
     Returns all existing paths.
 
     The optional argument `from_root` is a path and the method return all 
     subpaths rooted at that point.
@@ -138,30 +151,38 @@
 
   By default, `path = ""`, which returns the entire configuration as a Config 
   object.
   """
   conf = read_config()
   return conf.get(path)
 
-def set(path: str, values: typing.List[typing.Any]):
+def set(path: str, value: typing.Any):
   """
   Sets `value` at `path` in the config. `value` will be interpreted as JSON, if 
   conversion to JSON fails, it will be used as is.
+
+  If `value` is `None`, the entry referenced by `path` will be deleted, if it 
+  exists.
   """
   conf = read_config()
-  for i in range(len(values)):
+  if isinstance(value, list):
+    for i in range(len(value)):
+      try:
+        value[i] = json.loads(value[i])
+      except:
+        pass
+    if len(value) == 1:
+      value = value[0]
+  else:
     try:
-      values[i] = json.loads(values[i])
-    except json.decoder.JSONDecodeError:
+      value = json.loads(value)
+    except:
       pass
 
-  if len(values) == 1:
-    values = values[0]
-
-  conf.set(path, values)
+  conf.set(path, value)
   write_config(conf)
 def read_config(conf_path=f"{dirs.user_config_dir}/config.json"):
   """
   Returns the config data structure (JSON).
   `conf_path` is an optional argument providing the path to the config file.
   """
   try:
```

### Comparing `typerconf-1.3/src/typerconf/init.nw` & `typerconf-1.4/src/typerconf/init.nw`

 * *Files 4% similar despite different names*

```diff
@@ -117,18 +117,21 @@
 
   By default, `path = ""`, which returns the entire configuration as a Config 
   object.
   """
   <<read config from file>>
   <<return the value at path in config>>
 
-def set(path: str, values: typing.List[typing.Any]):
+def set(path: str, value: typing.Any):
   """
   Sets `value` at `path` in the config. `value` will be interpreted as JSON, if 
   conversion to JSON fails, it will be used as is.
+
+  If `value` is `None`, the entry referenced by `path` will be deleted, if it 
+  exists.
   """
   <<read config from file>>
   <<set the value at path in config>>
   <<write config back to file>>
 @
 
 Let's start with reading and writing the config file.
@@ -146,24 +149,35 @@
 
 Now, to set a value, we have several cases.
 If the user supplied more than one value, we want a list.
 If only one value, we don't want to store a list with only one value in it.
 Also, we want to try interpret any value as JSON.
 If that fails, we'll use the value as-is.
 <<set the value at path in config>>=
-for i in range(len(values)):
+if isinstance(value, list):
+  <<try to convert each element to JSON>>
+  if len(value) == 1:
+    value = value[0]
+else:
   try:
-    values[i] = json.loads(values[i])
-  except json.decoder.JSONDecodeError:
+    value = json.loads(value)
+  except:
     pass
 
-if len(values) == 1:
-  values = values[0]
+conf.set(path, value)
+@
 
-conf.set(path, values)
+When we try to convert each element to JSON, we do it in place; hence iterate 
+over the index rather than the elements directly.
+<<try to convert each element to JSON>>=
+for i in range(len(value)):
+  try:
+    value[i] = json.loads(value[i])
+  except:
+    pass
 @
 
 Now let's cover [[read_config]], [[write_config]], [[set_path]] and 
 [[get_path]] below.
 
 
 \section{Reading and writing the config file}\label{ConfigFile}
@@ -308,15 +322,18 @@
     Example:
     - `value = "https://..."`,
     - `path = "courses.datintro22.url"`
     will create `{"courses": {"datintro22": {"url": "https://..."}}}`.
 
     Any part of the path that can be converted to an integer, will be converted 
     to an integer. This way we can access elements of lists too. However, we 
-    cannot create index 3 in a list if it doesn't exist.
+    cannot create index 3 in a list if it doesn't exist (we can't expand 
+    lists).
+
+    If `value` is `None`, the entry at `path` will be deleted, if it exists.
     """
     <<set value at path>>
 
   def paths(self, from_root=""):
     """
     Returns all existing paths.
 
@@ -346,15 +363,30 @@
   path = "courses.datintro22.TAs.0"
   conf.set(path, value)
   assert conf.get(path) == value
 
   value = ["Asse", "Assa", "Asselina"]
   path = "courses.prgx22.TAs"
   conf.set(path, value)
-  assert len(conf.get(path)) == len(value)
+  gotten_value = conf.get(path)
+  assert isinstance(gotten_value, list)
+  assert len(gotten_value) == len(value)
+
+  value = {"A": 1, "B": 2}
+  conf.set("test", value)
+  gotten_value = conf.get("test")
+  assert value == gotten_value
+
+  conf.set("test", None)
+  try:
+    conf.get("test")
+  except KeyError:
+    assert True
+  else:
+    assert False
 
 def test_paths():
   assert "courses.datintro22.TAs" in conf.paths()
   for path in conf.paths():
     assert conf.get(path)
 @
 
@@ -382,36 +414,68 @@
 @
 
 \subsection{Setting values}
 
 To set a value is a bit more complex.
 We want to be able to specify a path and create all parents along the path if 
 they don't exist.
+However, if the value is [[None]], we don't want to create an entry that 
+doesn't exist, but we want to delete one if it already exists.
 <<set value at path>>=
 structure = self.__data
 
 parts = path.split(".")
-for part in parts[:-1]:
+
+<<update structure to parent node, create parents if they don't exist>>
+
+part = parts[-1]
+try:
+  part = int(part)
+except ValueError:
+  pass
+
+if value is None:
   try:
-    part = int(part)
-  except ValueError:
+    del structure[part]
+  except KeyError:
     pass
+else:
+  structure[part] = value
+@
 
+We want to traverse the tree, we want to go to the immediate parent of the leaf 
+that we want to set a value for (or delete).
+We iterate through the path.
+<<update structure to parent node, create parents if they don't exist>>=
+for part in parts[:-1]:
+  <<check if part is an integer, if so, convert it>>
   try:
     structure = structure[part]
   except KeyError:
-    structure[part] = {}
-    structure = structure[part]
+    <<handle node that doesn't exist>>
+@
 
-part = parts[-1]
+To handle integers on the path, we do it in the pythonic way: we try to convert 
+it, if it fails, we just continue with the non-integer value.
+<<check if part is an integer, if so, convert it>>=
 try:
   part = int(part)
 except ValueError:
   pass
-structure[part] = value
+@
+
+If a node along the path doesn't exist, we want to create it.
+However, if [[value]] is [[None]], we actually want to delete the leaf, then we 
+don't create the parents if they don't exist either.
+<<handle node that doesn't exist>>=
+if value is None:
+  return
+else:
+  structure[part] = {}
+  structure = structure[part]
 @
 
 \subsection{All existing paths}
 
 Lastly, what we want to do is to create a list containing all paths in the 
 config.
 We will simply traverse the config tree and add paths as we go.
```

### Comparing `typerconf-1.3/PKG-INFO` & `typerconf-1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typerconf
-Version: 1.3
+Version: 1.4
 Summary: Library to read and write configs using API and CLI with Typer
 Home-page: https://github.com/dbosk/typerconf
 License: MIT
 Keywords: typer,conf,config,git-like,config lib,write conf
 Author: Daniel Bosk
 Author-email: daniel@bosk.se
 Requires-Python: >=3.7,<4.0
```

