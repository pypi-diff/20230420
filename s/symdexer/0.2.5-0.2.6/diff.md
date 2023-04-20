# Comparing `tmp/symdexer-0.2.5.tar.gz` & `tmp/symdexer-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\AntiMach\Desktop\symdexer\dist\.tmp-i62y9un0\symdexer-0.2.5.tar", last modified: Mon Apr 17 01:28:15 2023, max compression
+gzip compressed data, was "C:\Users\AntiMach\Desktop\symdexer\dist\.tmp-m3w4mbay\symdexer-0.2.6.tar", last modified: Thu Apr 20 20:00:02 2023, max compression
```

## Comparing `symdexer-0.2.5.tar` & `symdexer-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 01:28:15.000000 symdexer-0.2.5/
--rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0      634 2023-04-17 01:28:15.000000 symdexer-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.5/README.md
--rw-rw-rw-   0        0        0      588 2023-04-17 01:22:43.000000 symdexer-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 01:28:15.000000 symdexer-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer/
--rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.5/src/symdexer/__init__.py
--rw-rw-rw-   0        0        0       74 2023-04-13 19:01:25.000000 symdexer-0.2.5/src/symdexer/__main__.py
--rw-rw-rw-   0        0        0     3052 2023-04-17 01:26:42.000000 symdexer-0.2.5/src/symdexer/cache.py
--rw-rw-rw-   0        0        0     4176 2023-04-17 01:26:35.000000 symdexer-0.2.5/src/symdexer/main.py
--rw-rw-rw-   0        0        0      791 2023-04-17 01:27:16.000000 symdexer-0.2.5/src/symdexer/modules.py
--rw-rw-rw-   0        0        0      980 2023-04-17 01:26:21.000000 symdexer-0.2.5/src/symdexer/symbols.py
--rw-rw-rw-   0        0        0      705 2023-04-17 01:26:25.000000 symdexer-0.2.5/src/symdexer/types.py
--rw-rw-rw-   0        0        0       19 2023-04-17 01:22:36.000000 symdexer-0.2.5/src/symdexer/version.py
-drwxrwxrwx   0        0        0        0 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer.egg-info/
--rw-rw-rw-   0        0        0      634 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 01:28:15.000000 symdexer-0.2.5/src/symdexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 20:00:02.000000 symdexer-0.2.6/
+-rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      634 2023-04-20 20:00:02.000000 symdexer-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.6/README.md
+-rw-rw-rw-   0        0        0      588 2023-04-20 19:19:36.000000 symdexer-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 20:00:02.000000 symdexer-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 20:00:02.000000 symdexer-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 20:00:02.000000 symdexer-0.2.6/src/symdexer/
+-rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.6/src/symdexer/__init__.py
+-rw-rw-rw-   0        0        0     1620 2023-04-20 19:57:17.000000 symdexer-0.2.6/src/symdexer/__main__.py
+-rw-rw-rw-   0        0        0       38 2023-04-20 19:19:33.000000 symdexer-0.2.6/src/symdexer/__version__.py
+-rw-rw-rw-   0        0        0     3774 2023-04-20 19:53:13.000000 symdexer-0.2.6/src/symdexer/cache.py
+-rw-rw-rw-   0        0        0     1049 2023-04-20 00:08:33.000000 symdexer-0.2.6/src/symdexer/modules.py
+-rw-rw-rw-   0        0        0     3565 2023-04-20 19:56:53.000000 symdexer-0.2.6/src/symdexer/parser.py
+-rw-rw-rw-   0        0        0     1038 2023-04-20 19:11:11.000000 symdexer-0.2.6/src/symdexer/symbols.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:00:02.000000 symdexer-0.2.6/src/symdexer.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-04-20 20:00:02.000000 symdexer-0.2.6/src/symdexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-04-20 20:00:02.000000 symdexer-0.2.6/src/symdexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 20:00:02.000000 symdexer-0.2.6/src/symdexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-20 20:00:02.000000 symdexer-0.2.6/src/symdexer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 20:00:02.000000 symdexer-0.2.6/src/symdexer.egg-info/top_level.txt
```

### Comparing `symdexer-0.2.5/LICENSE.txt` & `symdexer-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.5/PKG-INFO` & `symdexer-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.5
+Version: 0.2.6
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `symdexer-0.2.5/pyproject.toml` & `symdexer-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "symdexer"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="AntiMach", email="themachinumps@gmail.com" },
 ]
 description = "A CLI for finding and indexing symbols"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `symdexer-0.2.5/src/symdexer/cache.py` & `symdexer-0.2.6/src/symdexer/cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import sqlite3
 from pathlib import Path
-from typing import Generator
+from typing import Iterator
 
 from symdexer.symbols import iter_symbols
 from symdexer.modules import walk_modules, Module
 
 
 class Cache:
     def __init__(self, path: Path):
@@ -15,15 +15,15 @@
     def __enter__(self):
         self.db = sqlite3.connect(self.path).__enter__()
         return self
 
     def __exit__(self, *args, **kwargs):
         self.db.__exit__(*args, **kwargs)
 
-    def reset(self):
+    def init(self):
         self.db.executescript(
             """
             DROP TABLE IF EXISTS Module;
 
             DROP TABLE IF EXISTS Symbol;
 
             CREATE TABLE Module (
@@ -31,72 +31,95 @@
                 path TEXT NOT NULL,
                 changed NUMBER NOT NULL
             );
 
             CREATE TABLE Symbol (
                 name TEXT NOT NULL,
                 type TEXT NOT NULL,
-                module TEXT NOT NULL REFERENCES Module(name),
+                module TEXT NOT NULL REFERENCES Module(name) ON UPDATE CASCADE,
                 UNIQUE (name, type, module)
             );
             """
         )
 
-    def update(self, packages: list[Path]):
+    def update(self, packages: list[Path]) -> Iterator[Module]:
         for path in packages:
             for module in walk_modules(path):
-                self._cache_module(module)
+                yield module
+                self._index_module(module)
 
         self.db.commit()
 
-    def _cache_module(self, module: Module):
-        moduleInfo = module.name, str(module.path.resolve()), module.mtime
-
-        # guard clause that returns when the module being indexed
-        # hasn't changed location or mtime since last index
+    def _index_module(self, module: Module):
         if self.db.execute(
             """
-            SELECT name
-            FROM Module
+            SELECT path, changed
+            FROM module
             WHERE name = ? AND (path != ? OR changed != ?)
             """,
-            moduleInfo,
+            module.info,
         ).fetchall():
             return
 
         self.db.execute(
             """
-            INSERT OR IGNORE INTO Module (name, path, changed)
+            INSERT OR REPLACE INTO Module (name, path, changed)
             VALUES (?, ? ,?)
             """,
-            moduleInfo,
+            module.info,
         )
 
         for symbol, sym_type in iter_symbols(module.path):
             self.db.execute(
                 """
-                INSERT OR IGNORE INTO Symbol (name, type, module)
+                INSERT OR REPLACE INTO Symbol (name, type, module)
                 VALUES (?, ? ,?)
                 """,
                 (symbol, sym_type, module.name),
             )
 
-    def search(self, symbols: list[str], fuzzy: bool, types: list[str]) -> Generator[tuple[str, str, str], None, None]:
-        symbol_t = "Symbol.name LIKE ?" if fuzzy else "Symbol.name = ?"
+    def ungrouped(self, symbols: list[str], types: list[str], fuzzy: str) -> Iterator[tuple[str, str, str]]:
+        if fuzzy:
+            symbols = [f"%{s}%" for s in symbols]
+            symbol_t = "Symbol.name LIKE ?"
+        else:
+            symbol_t = "Symbol.name = ?"
+
+        symbols_t = " OR ".join(symbol_t for _ in symbols)
+        types_t = " OR ".join("type = ?" for _ in types)
+
+        cursor = self.db.execute(
+            f"""
+            SELECT Symbol.name, module, path
+            FROM Symbol
+            INNER JOIN Module ON module = Module.name
+            WHERE ({symbols_t}) AND ({types_t})
+            ORDER BY LENGTH(module) + LENGTH(Symbol.name) ASC
+            """,
+            (*symbols, *types),
+        )
+
+        return cursor.fetchall()
+
+    def grouped(self, symbols: list[str], types: list[str], fuzzy: str) -> Iterator[tuple[str, str, str]]:
+        if fuzzy:
+            symbols = [f"%{s}%" for s in symbols]
+            symbol_t = "Symbol.name LIKE ?"
+        else:
+            symbol_t = "Symbol.name = ?"
+
         symbols_t = " OR ".join(symbol_t for _ in symbols)
         types_t = " OR ".join("type = ?" for _ in types)
 
         cursor = self.db.execute(
             f"""
             SELECT GROUP_CONCAT(Symbol.name, ", ") as names, module, path
             FROM Symbol
             INNER JOIN Module ON module = Module.name
             WHERE ({symbols_t}) AND ({types_t})
-            GROUP BY
-                module
-            ORDER BY
-                LENGTH(module) + LENGTH(names) ASC
+            GROUP BY module
+            ORDER BY LENGTH(module) + LENGTH(names) ASC
             """,
             (*symbols, *types),
         )
 
         return cursor.fetchall()
```

### Comparing `symdexer-0.2.5/src/symdexer/modules.py` & `symdexer-0.2.6/src/symdexer/modules.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Generator
-from dataclasses import dataclass
+from typing import Iterator
 from functools import lru_cache
+from dataclasses import dataclass
 
 
 @dataclass(frozen=True)
 class Module:
     path: Path
     name: str
 
     @property
     @lru_cache(maxsize=None)
-    def mtime(self):
+    def path_str(self) -> str:
+        return str(self.path.resolve())
+
+    @property
+    @lru_cache(maxsize=None)
+    def mtime(self) -> int:
         return int(self.path.stat().st_mtime)
 
+    @property
+    @lru_cache(maxsize=True)
+    def info(self) -> tuple[str, str, int]:
+        return self.name, self.path_str, self.mtime
+
 
-def walk_modules(path: Path, prefix: str = "") -> Generator[Module, None, None]:
+def walk_modules(path: Path, prefix: str = "") -> Iterator[Module]:
     if not prefix:
         prefix = path.stem
 
     if path.is_file():
         if path.suffix == ".py":
             yield Module(path, prefix)
         return
```

### Comparing `symdexer-0.2.5/src/symdexer/symbols.py` & `symdexer-0.2.6/src/symdexer/symbols.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import ast
 from pathlib import Path
+from typing import Iterator
 
 
 IMPORTS = "imports"
 DEFINES = "defines"
 ASSIGNS = "assigns"
 SYM_TYPES = [IMPORTS, DEFINES, ASSIGNS]
 
@@ -30,15 +31,15 @@
     ast.FunctionDef: _defines,
     ast.ClassDef: _defines,
     ast.Import: _imports,
     ast.ImportFrom: _imports,
 }
 
 
-def iter_symbols(path: Path):
+def iter_symbols(path: Path) -> Iterator[tuple[str, str]]:
     # sourcery skip: use-named-expression
     try:
         root = ast.parse(path.read_text("utf-8"))
     except SyntaxError:
         return
 
     for node in ast.iter_child_nodes(root):
```

### Comparing `symdexer-0.2.5/src/symdexer.egg-info/PKG-INFO` & `symdexer-0.2.6/src/symdexer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.5
+Version: 0.2.6
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

