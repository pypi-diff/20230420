# Comparing `tmp/specialist-0.4.2.tar.gz` & `tmp/specialist-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specialist-0.4.2.tar", last modified: Mon Oct 24 07:09:26 2022, max compression
+gzip compressed data, was "specialist-0.5.0.tar", last modified: Thu Apr 20 19:16:06 2023, max compression
```

## Comparing `specialist-0.4.2.tar` & `specialist-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 07:09:26.683460 specialist-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-10-24 07:09:11.000000 specialist-0.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     8632 2022-10-24 07:09:26.683460 specialist-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8296 2022-10-24 07:09:11.000000 specialist-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-24 07:09:26.683460 specialist-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-10-24 07:09:11.000000 specialist-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 07:09:26.679460 specialist-0.4.2/specialist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8632 2022-10-24 07:09:26.000000 specialist-0.4.2/specialist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-10-24 07:09:26.000000 specialist-0.4.2/specialist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 07:09:26.000000 specialist-0.4.2/specialist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-24 07:09:26.000000 specialist-0.4.2/specialist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-24 07:09:26.000000 specialist-0.4.2/specialist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17667 2022-10-24 07:09:11.000000 specialist-0.4.2/specialist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:16:06.639860 specialist-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-20 19:15:59.000000 specialist-0.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-20 19:16:06.639860 specialist-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-04-20 19:15:59.000000 specialist-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:16:06.639860 specialist-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-20 19:15:59.000000 specialist-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:16:06.639860 specialist-0.5.0/specialist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-20 19:16:06.000000 specialist-0.5.0/specialist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-20 19:16:06.000000 specialist-0.5.0/specialist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:16:06.000000 specialist-0.5.0/specialist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 19:16:06.000000 specialist-0.5.0/specialist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 19:16:06.000000 specialist-0.5.0/specialist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19758 2023-04-20 19:15:59.000000 specialist-0.5.0/specialist.py
```

### Comparing `specialist-0.4.2/LICENSE.md` & `specialist-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `specialist-0.4.2/PKG-INFO` & `specialist-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specialist
-Version: 0.4.2
+Version: 0.5.0
 Summary: Visualize CPython 3.11's specializing, adaptive interpreter.
 Home-page: https://github.com/brandtbucher/specialist
 Author: Brandt Bucher
 Author-email: brandt@python.org
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 <div align=center>
 
 
 Specialist
 ==========
 
-[![latest version](https://img.shields.io/github/release-pre/brandtbucher/specialist.svg?style=for-the-badge&label=latest)![latest release date](https://img.shields.io/github/release-date-pre/brandtbucher/specialist.svg?style=for-the-badge&label=released)](https://github.com/brandtbucher/specialist/releases)[![build status](https://img.shields.io/github/workflow/status/brandtbucher/specialist/CI/main.svg?style=for-the-badge)](https://github.com/brandtbucher/specialist/actions)[![issues](https://img.shields.io/github/issues-raw/brandtbucher/specialist.svg?label=issues&style=for-the-badge)](https://github.com/brandtbucher/specialist/issues)
+[![latest version](https://img.shields.io/github/release-pre/brandtbucher/specialist.svg?style=for-the-badge&label=latest)![latest release date](https://img.shields.io/github/release-date-pre/brandtbucher/specialist.svg?style=for-the-badge&label=released)](https://github.com/brandtbucher/specialist/releases)[![build status](https://img.shields.io/github/actions/workflow/status/brandtbucher/specialist/ci.yml.svg?style=for-the-badge&branch=main)](https://github.com/brandtbucher/specialist/actions)[![issues](https://img.shields.io/github/issues-raw/brandtbucher/specialist.svg?label=issues&style=for-the-badge)](https://github.com/brandtbucher/specialist/issues)
 
 <br>
 
 </div>
 
 <div align=justify>
```

### Comparing `specialist-0.4.2/README.md` & `specialist-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div align=center>
 
 
 Specialist
 ==========
 
-[![latest version](https://img.shields.io/github/release-pre/brandtbucher/specialist.svg?style=for-the-badge&label=latest)![latest release date](https://img.shields.io/github/release-date-pre/brandtbucher/specialist.svg?style=for-the-badge&label=released)](https://github.com/brandtbucher/specialist/releases)[![build status](https://img.shields.io/github/workflow/status/brandtbucher/specialist/CI/main.svg?style=for-the-badge)](https://github.com/brandtbucher/specialist/actions)[![issues](https://img.shields.io/github/issues-raw/brandtbucher/specialist.svg?label=issues&style=for-the-badge)](https://github.com/brandtbucher/specialist/issues)
+[![latest version](https://img.shields.io/github/release-pre/brandtbucher/specialist.svg?style=for-the-badge&label=latest)![latest release date](https://img.shields.io/github/release-date-pre/brandtbucher/specialist.svg?style=for-the-badge&label=released)](https://github.com/brandtbucher/specialist/releases)[![build status](https://img.shields.io/github/actions/workflow/status/brandtbucher/specialist/ci.yml.svg?style=for-the-badge&branch=main)](https://github.com/brandtbucher/specialist/actions)[![issues](https://img.shields.io/github/issues-raw/brandtbucher/specialist.svg?label=issues&style=for-the-badge)](https://github.com/brandtbucher/specialist/issues)
 
 <br>
 
 </div>
 
 <div align=justify>
 
@@ -221,8 +221,8 @@
 green-yellow-orange-red one.
 
 ### `-d`/`--dark`
 
 Use light text on a dark background. Some users may find a dark scheme makes
 them feel cooler than the default light one.
 
-</div>
+</div>
```

### Comparing `specialist-0.4.2/setup.py` & `specialist-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     license="MIT",
     long_description=README.read_text(),
     long_description_content_type="text/markdown",
     name="specialist",
     py_modules=["specialist"],
     python_requires=">=3.11",
     url="https://github.com/brandtbucher/specialist",
-    version="0.4.2",
+    version="0.5.0",
 )
```

### Comparing `specialist-0.4.2/specialist.egg-info/PKG-INFO` & `specialist-0.5.0/specialist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specialist
-Version: 0.4.2
+Version: 0.5.0
 Summary: Visualize CPython 3.11's specializing, adaptive interpreter.
 Home-page: https://github.com/brandtbucher/specialist
 Author: Brandt Bucher
 Author-email: brandt@python.org
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 <div align=center>
 
 
 Specialist
 ==========
 
-[![latest version](https://img.shields.io/github/release-pre/brandtbucher/specialist.svg?style=for-the-badge&label=latest)![latest release date](https://img.shields.io/github/release-date-pre/brandtbucher/specialist.svg?style=for-the-badge&label=released)](https://github.com/brandtbucher/specialist/releases)[![build status](https://img.shields.io/github/workflow/status/brandtbucher/specialist/CI/main.svg?style=for-the-badge)](https://github.com/brandtbucher/specialist/actions)[![issues](https://img.shields.io/github/issues-raw/brandtbucher/specialist.svg?label=issues&style=for-the-badge)](https://github.com/brandtbucher/specialist/issues)
+[![latest version](https://img.shields.io/github/release-pre/brandtbucher/specialist.svg?style=for-the-badge&label=latest)![latest release date](https://img.shields.io/github/release-date-pre/brandtbucher/specialist.svg?style=for-the-badge&label=released)](https://github.com/brandtbucher/specialist/releases)[![build status](https://img.shields.io/github/actions/workflow/status/brandtbucher/specialist/ci.yml.svg?style=for-the-badge&branch=main)](https://github.com/brandtbucher/specialist/actions)[![issues](https://img.shields.io/github/issues-raw/brandtbucher/specialist.svg?label=issues&style=for-the-badge)](https://github.com/brandtbucher/specialist/issues)
 
 <br>
 
 </div>
 
 <div align=justify>
```

### Comparing `specialist-0.4.2/specialist.py` & `specialist-0.5.0/specialist.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 import html
 import http.server
 import importlib.util
 import itertools
 import opcode
 import os
 import runpy
+import shlex
+import sysconfig
 import tempfile
 import threading
 import typing
 import webbrowser
 
 _FIRST_POSTION = (1, 0)
 _LAST_POSITION = (sys.maxsize, 0)
@@ -68,14 +70,20 @@
         "PRECALL_NO_KW_STR_1",
         "PRECALL_NO_KW_TUPLE_1",
         "PRECALL_NO_KW_TYPE_1",
         "STORE_FAST__LOAD_FAST",
         "STORE_FAST__STORE_FAST",
     }
 )
+_LIB = pathlib.Path(
+    os.path.commonpath([sysconfig.get_path("stdlib"), sysconfig.get_path("purelib")])
+).resolve()
+assert _LIB.is_dir()
+_TMP = pathlib.Path(tempfile.gettempdir()).resolve()
+assert _TMP.is_dir()
 
 
 class _HTMLWriter:
     """Write HTML for a source code view."""
 
     def __init__(self, *, blue: bool, dark: bool) -> None:
         self._blue = blue
@@ -120,40 +128,49 @@
         # Always fully saturate the color:
         saturation = 1
         rgb = colorsys.hls_to_rgb(hue, lightness, saturation)
         return f"#{int(255 * rgb[0]):02x}{int(255 * rgb[1]):02x}{int(255 * rgb[2]):02x}"
 
 
 def _stderr(*args: object) -> None:
-    """Print to stdout."""
+    """Print to stderr."""
     print("specialist:", *args, file=sys.stderr, flush=True)
 
 
 def _is_superinstruction(instruction: dis.Instruction | None) -> bool:
     """Check if an instruction is a superinstruction."""
     return instruction is not None and instruction.opname in _SUPERINSTRUCTIONS
 
 
 def _is_superduperinstruction(instruction: dis.Instruction | None) -> bool:
     """Check if an instruction is a superduperinstruction."""
     return instruction is not None and instruction.opname in _SUPERDUPERINSTRUCTIONS
 
 
+def _adaptive_counter_value(instruction: dis.Instruction, raw_bytecode: bytes) -> int:
+    """Get the value of the adaptive counter for this instruction."""
+    next_code_unit = raw_bytecode[instruction.offset + 2 : instruction.offset + 4]
+    counter = int.from_bytes(next_code_unit, sys.byteorder)
+    return counter >> 4
+
+
 def _score_instruction(
     instruction: dis.Instruction,
     previous: dis.Instruction | None,
     previous_previous: dis.Instruction | None,
+    raw_bytecode: bytes,
 ) -> "_Stats":
     """Return stats for the given instruction."""
     if _is_superinstruction(previous) or _is_superduperinstruction(previous_previous):
         return _Stats(specialized=True)
     if instruction.opname in _SPECIALIZED_INSTRUCTIONS:
-        if instruction.opname.endswith("_ADAPTIVE"):
+        if not instruction.opname.endswith("_ADAPTIVE"):
+            return _Stats(specialized=True)
+        if _adaptive_counter_value(instruction, raw_bytecode):
             return _Stats(adaptive=True)
-        return _Stats(specialized=True)
     return _Stats(unquickened=True)
 
 
 @contextlib.contextmanager
 def _catch_exceptions() -> typing.Generator[list[BaseException], None, None]:
     """Suppress exceptions, and gather them into a list."""
     caught: list[BaseException] = []
@@ -182,15 +199,15 @@
     if spec.submodule_search_locations is not None:
         spec = importlib.util.find_spec(f"{module}.__main__")
         if spec is None:
             return None
     if not spec.has_location:
         return None
     assert spec.origin is not None
-    return pathlib.Path(spec.origin)
+    return pathlib.Path(spec.origin).resolve()
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
 class _Stats:
     """Statistics about a source chunk."""
 
     specialized: int = 0
@@ -238,27 +255,30 @@
     events: collections.defaultdict[tuple[int, int], _Stats] = collections.defaultdict(
         _Stats
     )
     events[_FIRST_POSTION] = _Stats()
     events[_LAST_POSITION] = _Stats()
     previous_previous = previous = None
     for child in _walk_code(code):
+        raw_bytecode = child._co_code_adaptive  # type: ignore [attr-defined]  # pylint: disable = protected-access
         for instruction in dis.get_instructions(child, adaptive=True):
             if instruction.is_jump_target:
                 previous_previous = previous = None
             if instruction.positions is None or None in instruction.positions:
                 previous_previous = previous
                 previous = instruction
                 continue
             lineno, end_lineno, col_offset, end_col_offset = instruction.positions
             assert lineno is not None
             assert end_lineno is not None
             assert col_offset is not None
             assert end_col_offset is not None
-            stats = _score_instruction(instruction, previous, previous_previous)
+            stats = _score_instruction(
+                instruction, previous, previous_previous, raw_bytecode
+            )
             events[lineno, col_offset] += stats
             events[end_lineno, end_col_offset] -= stats
             previous_previous = previous
             previous = instruction
     stats = _Stats()
     for (start, event), (stop, _) in itertools.pairwise(sorted(events.items())):
         stats += event
@@ -305,36 +325,67 @@
 def _view(
     path: pathlib.Path,
     *,
     blue: bool = False,
     dark: bool = False,
     out: pathlib.Path | None = None,
     name: str | None = None,
-) -> None:
+) -> bool:
     """View a code object's source code."""
     writer = _HTMLWriter(blue=blue, dark=dark)
     quickened = False
     for source, stats in _source_and_stats(path):
         if stats.specialized or stats.adaptive:
             quickened = True
         writer.add(source, stats)
     if not quickened:
         _stderr(
             f"No quickened code found in {name or path}! Try modifying it to run "
             f"longer, or use the --targets option to analyze different source files."
         )
-        return
+        return False
     written = writer.emit()
     if out is not None:
         out.parent.mkdir(parents=True, exist_ok=True)
         out.unlink(missing_ok=True)
         out.write_text(written)
         _stderr(path, "->", out)
     else:
         _browse(written)
+    return True
+
+
+def _suggest_target_glob(args: typing.Sequence[str]) -> None:
+    """Suggest possible glob patterns for targets."""
+    paths = [
+        path
+        for path in _code
+        # Also filter these for containing quickend code?
+        if path.is_file() and _TMP not in path.parents and _LIB not in path.parents
+    ]
+    if not paths:
+        return
+    if len(paths) == 1:
+        glob = paths[0]
+    else:
+        common = pathlib.Path(os.path.commonpath(paths)).resolve()
+        assert common.is_dir()
+        assert _LIB not in common.parents
+        if common in _LIB.parents:
+            return  # pragma: no cover
+        longest = max(len(path.parts) for path in paths)
+        if len(common.parts) == longest - 1:
+            glob = common / "*"
+        else:
+            glob = common / "**" / "*"
+    cwd = pathlib.Path.cwd().resolve()
+    if glob.is_relative_to(cwd):  # pragma: no cover
+        glob = glob.relative_to(cwd)
+    suggestion = shlex.join(["--targets", str(glob), *args])
+    _stderr(f"Did you mean {suggestion}?")
 
 
 def _browse(page: str) -> None:
     """Open a web browser to display a page."""
 
     class RequestHandler(http.server.BaseHTTPRequestHandler):
         """A simple handler for a single web page."""
@@ -429,21 +480,20 @@
     return typing.cast(_Args, vars(parser.parse_args(args)))
 
 
 def main(args: typing.Sequence[str] | None = None) -> None:
     """Run the main program."""
     parsed = _parse_args(args)
     output = parsed["output"]
-    targets = parsed["targets"]
     path: pathlib.Path | None
     with tempfile.TemporaryDirectory() as work:
         match parsed:
             case {"command": [source, *argv], "module": [], "file": []}:
-                path = pathlib.Path(work) / "__main__.py"
-                path.write_text(source)
+                path = pathlib.Path(work, "__main__.py").resolve()
+                path.write_text(source, encoding="utf-8")
                 name: str | None = "the provided command"
                 with _patch_sys_argv(argv), _catch_exceptions() as caught:
                     runpy.run_path(  # pylint: disable = no-member
                         str(path), run_name="__main__"
                     )
             case {"command": [], "module": [source, *argv], "file": []}:
                 with _patch_sys_argv(argv), _catch_exceptions() as caught:
@@ -453,26 +503,26 @@
                 path = _main_file_for_module(source)
                 name = source
             case {"command": [], "module": [], "file": [source, *argv]}:
                 with _patch_sys_argv(argv), _catch_exceptions() as caught:
                     runpy.run_path(  # pylint: disable = no-member
                         source, run_name="__main__"
                     )
-                path = pathlib.Path(source)
+                path = pathlib.Path(source).resolve()
                 name = source
             case _:  # pragma: no cover
                 assert False, parsed
         paths: list[pathlib.Path] = []
-        if targets is not None:
+        if parsed["targets"] is not None:
             name = None
-            for match in pathlib.Path().glob(targets):
+            for match in pathlib.Path().resolve().glob(parsed["targets"]):
                 if match.resolve() in _code:
                     paths.append(match.resolve())
-        elif path is not None:
-            paths.append(path.resolve())
+        elif path is not None and path in _code:
+            paths.append(path)
         if not paths:
             _stderr("No source files found!")
         else:
             if output is not None:
                 common = pathlib.Path(
                     os.path.commonpath(paths)  # pylint: disable = no-member
                 ).resolve()
@@ -484,17 +534,20 @@
                     tuple[pathlib.Path, pathlib.Path | None], None, None
                 ] = (
                     (path, output / path.relative_to(common).with_suffix(".html"))
                     for path in paths
                 )
             else:
                 path_and_out = ((path, None) for path in paths)
+            found = False
             for path, out in sorted(path_and_out):
-                _view(
+                found |= _view(
                     path, blue=parsed["blue"], dark=parsed["dark"], out=out, name=name
                 )
+            if not found and not parsed["targets"]:
+                _suggest_target_glob(args or sys.argv[1:])
         if caught:
             raise caught[0] from None
 
 
 if __name__ == "__main__":  # pragma: no cover
     main(sys.argv[1:])
```

