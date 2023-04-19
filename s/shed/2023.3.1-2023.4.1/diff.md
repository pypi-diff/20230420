# Comparing `tmp/shed-2023.3.1.tar.gz` & `tmp/shed-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shed-2023.3.1.tar", last modified: Sun Mar  5 08:55:12 2023, max compression
+gzip compressed data, was "shed-2023.4.1.tar", last modified: Wed Apr 19 23:32:28 2023, max compression
```

## Comparing `shed-2023.3.1.tar` & `shed-2023.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 08:55:12.703142 shed-2023.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-05 08:55:02.000000 shed-2023.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-03-05 08:55:12.703142 shed-2023.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-03-05 08:55:02.000000 shed-2023.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 08:55:12.703142 shed-2023.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-05 08:55:02.000000 shed-2023.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 08:55:12.699141 shed-2023.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 08:55:12.699141 shed-2023.3.1/src/shed/
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-03-05 08:55:02.000000 shed-2023.3.1/src/shed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-05 08:55:02.000000 shed-2023.3.1/src/shed/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-03-05 08:55:02.000000 shed-2023.3.1/src/shed/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-03-05 08:55:02.000000 shed-2023.3.1/src/shed/_codemods.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 08:55:02.000000 shed-2023.3.1/src/shed/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 08:55:12.699141 shed-2023.3.1/src/shed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-03-05 08:55:12.000000 shed-2023.3.1/src/shed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-05 08:55:12.000000 shed-2023.3.1/src/shed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 08:55:12.000000 shed-2023.3.1/src/shed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-05 08:55:12.000000 shed-2023.3.1/src/shed.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-05 08:55:12.000000 shed-2023.3.1/src/shed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-05 08:55:12.000000 shed-2023.3.1/src/shed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 08:55:12.699141 shed-2023.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-05 08:55:02.000000 shed-2023.3.1/tests/test_expected_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-03-05 08:55:02.000000 shed-2023.3.1/tests/test_shed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-03-05 08:55:02.000000 shed-2023.3.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:32:28.381337 shed-2023.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-19 23:32:17.000000 shed-2023.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-19 23:32:28.381337 shed-2023.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-19 23:32:17.000000 shed-2023.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:32:28.381337 shed-2023.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-19 23:32:17.000000 shed-2023.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:32:28.381337 shed-2023.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:32:28.381337 shed-2023.4.1/src/shed/
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-04-19 23:32:17.000000 shed-2023.4.1/src/shed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-19 23:32:17.000000 shed-2023.4.1/src/shed/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-19 23:32:17.000000 shed-2023.4.1/src/shed/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27062 2023-04-19 23:32:17.000000 shed-2023.4.1/src/shed/_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:32:17.000000 shed-2023.4.1/src/shed/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:32:28.381337 shed-2023.4.1/src/shed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-19 23:32:28.000000 shed-2023.4.1/src/shed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-19 23:32:28.000000 shed-2023.4.1/src/shed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:32:28.000000 shed-2023.4.1/src/shed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 23:32:28.000000 shed-2023.4.1/src/shed.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-19 23:32:28.000000 shed-2023.4.1/src/shed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 23:32:28.000000 shed-2023.4.1/src/shed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:32:28.381337 shed-2023.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-19 23:32:17.000000 shed-2023.4.1/tests/test_expected_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-19 23:32:17.000000 shed-2023.4.1/tests/test_shed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-19 23:32:17.000000 shed-2023.4.1/tests/test_version.py
```

### Comparing `shed-2023.3.1/LICENSE` & `shed-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shed-2023.3.1/PKG-INFO` & `shed-2023.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shed
-Version: 2023.3.1
+Version: 2023.4.1
 Summary: `shed` canonicalises Python code.
 Home-page: https://github.com/Zac-HD/shed
 Author: Zac Hatfield-Dodds
 Author-email: zac@zhd.dev
 License: AGPL-3.0
 Project-URL: Source, https://github.com/Zac-HD/shed/
 Project-URL: Changelog, https://github.com/Zac-HD/shed/blob/master/CHANGELOG.md
@@ -77,15 +77,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with Shed by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/Zac-HD/shed
-  rev: 2023.3.1
+  rev: 2023.4.1
   hooks:
     - id: shed
       # args: [--refactor, --py39-plus]
       types_or: [python, pyi, markdown, rst]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
```

### Comparing `shed-2023.3.1/README.md` & `shed-2023.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with Shed by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/Zac-HD/shed
-  rev: 2023.3.1
+  rev: 2023.4.1
   hooks:
     - id: shed
       # args: [--refactor, --py39-plus]
       types_or: [python, pyi, markdown, rst]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
```

### Comparing `shed-2023.3.1/setup.py` & `shed-2023.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `shed-2023.3.1/src/shed/__init__.py` & `shed-2023.4.1/src/shed/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import black
 import isort
 import pyupgrade._main
 from black.mode import TargetVersion
 from black.parsing import lib2to3_parse
 from isort.exceptions import FileSkipComment
 
-__version__ = "2023.3.1"
+__version__ = "2023.4.1"
 __all__ = ["shed", "docshed"]
 
 # Conditionally imported in refactor mode to reduce startup latency in the common case
 com2ann: Any = None
 _run_codemods: Any = None
 
 _version_map = {
```

### Comparing `shed-2023.3.1/src/shed/_cli.py` & `shed-2023.4.1/src/shed/_cli.py`

 * *Files identical despite different names*

### Comparing `shed-2023.3.1/src/shed/_codemods.py` & `shed-2023.4.1/src/shed/_codemods.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,42 @@
 These are mostly based on flake8, flake8-comprehensions, and some personal
 nitpicks about typing unions and literals.
 """
 
 import os
 import re
 from ast import literal_eval
+from functools import wraps
 from typing import List, Tuple
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.codemod import VisitorBasedCodemodCommand
 
 
+def leave(matcher):
+    """Wrap `libcst.matchers.leave` for fixed behaviour.
+
+    This works around https://github.com/Instagram/LibCST/issues/888
+    by checking if the updated node matches the matcher.
+    """
+
+    def inner(fn):
+        @wraps(fn)
+        @m.leave(matcher)
+        def wrapped(self, original_node, updated_node):
+            if not m.matches(updated_node, matcher):
+                return updated_node
+            return fn(self, original_node, updated_node)
+
+        return wrapped
+
+    return inner
+
+
 def attempt_hypothesis_codemods(context, mod):  # pragma: no cover
     try:
         from hypothesis.extra.codemods import (
             HypothesisFixComplexMinMagnitude,
             HypothesisFixPositionalKeywonlyArgs,
         )
     except ImportError:
@@ -130,20 +151,20 @@
             return cst.RemovalSentinel.REMOVE
         if updated_node.msg is None:
             return cst.Raise(cst.Name("AssertionError"))
         return cst.Raise(
             cst.Call(cst.Name("AssertionError"), args=[cst.Arg(updated_node.msg)])
         )
 
-    @m.leave(m.ComparisonTarget(comparator=m.Name("None"), operator=m.Equal()))
+    @leave(m.ComparisonTarget(comparator=m.Name("None"), operator=m.Equal()))
     def convert_none_cmp(self, _, updated_node):
         """Inspired by Pybetter."""
         return updated_node.with_changes(operator=cst.Is())
 
-    @m.leave(
+    @leave(
         m.UnaryOperation(
             operator=m.Not(),
             expression=m.Comparison(comparisons=[m.ComparisonTarget(operator=m.In())]),
         )
     )
     def replace_not_in_condition(self, _, updated_node):
         """Also inspired by Pybetter."""
@@ -151,15 +172,15 @@
         return cst.Comparison(
             left=expr.left,
             lpar=updated_node.lpar,
             rpar=updated_node.rpar,
             comparisons=[expr.comparisons[0].with_changes(operator=cst.NotIn())],
         )
 
-    @m.leave(
+    @leave(
         m.Call(
             lpar=[m.AtLeastN(n=1, matcher=m.LeftParen())],
             rpar=[m.AtLeastN(n=1, matcher=m.RightParen())],
         )
     )
     def remove_pointless_parens_around_call(self, _, updated_node):
         # Don't remove whitespace if it includes comments
@@ -170,31 +191,35 @@
         noparens = updated_node.with_changes(lpar=[], rpar=[])
         try:
             compile(self.module.code_for_node(noparens), "<string>", "eval")
             return noparens
         except SyntaxError:
             return updated_node
 
-    @m.leave(m.Call(func=oneof_names("dict", "list", "tuple"), args=[]))
+    @leave(m.Call(func=oneof_names("dict", "list", "tuple"), args=[]))
     def replace_builtin_with_literal(self, _, updated_node):
         if updated_node.func.value == "dict":
             return cst.Dict([])
         elif updated_node.func.value == "list":
             return cst.List([])
         else:
             assert updated_node.func.value == "tuple"
             return cst.Tuple([])
 
-    @m.leave(
+    @leave(
         m.Call(
             func=oneof_names("dict", "list", "tuple"),
             args=[m.Arg(m.Dict([]) | m.List([]) | m.SimpleString() | m.Tuple([]))],
         )
     )
     def replace_builtin_empty_collection(self, _, updated_node):
+        # If there is a keyword argument either this is a dict (and thus
+        # not empty) or the user has made an error we shouldn't mask.
+        if updated_node.args[0].keyword:
+            return updated_node
         val = updated_node.args[0].value
         val_is_empty_seq = (
             isinstance(val, (cst.Dict, cst.List, cst.Tuple)) and not val.elements
         )
         val_is_empty_str = (
             isinstance(val, cst.SimpleString) and val.evaluated_value == ""
         )
@@ -206,26 +231,26 @@
             return cst.List([])
         else:
             assert updated_node.func.value == "tuple"
             return cst.Tuple([])
 
     # The following methods fix https://pypi.org/project/flake8-comprehensions/
 
-    @m.leave(m.Call(func=m.Name("list"), args=[m.Arg(m.GeneratorExp())]))
+    @leave(m.Call(func=m.Name("list"), args=[m.Arg(m.GeneratorExp())]))
     def replace_generator_in_call_with_comprehension(self, _, updated_node):
         """Fix flake8-comprehensions C400-402 and 403-404.
 
         C400-402: Unnecessary generator - rewrite as a <list/set/dict> comprehension.
         Note that set and dict conversions are handled by pyupgrade!
         """
         return cst.ListComp(
             elt=updated_node.args[0].value.elt, for_in=updated_node.args[0].value.for_in
         )
 
-    @m.leave(
+    @leave(
         m.Call(func=m.Name("list"), args=[m.Arg(m.ListComp(), star="")])
         | m.Call(func=m.Name("set"), args=[m.Arg(m.SetComp(), star="")])
         | m.Call(
             func=m.Name("list"),
             args=[m.Arg(m.Call(func=oneof_names("sorted", "list")), star="")],
         )
     )
@@ -238,15 +263,15 @@
         for lists and sets.
         """
         return updated_node.args[0].value
 
     _sets = oneof_names("set", "frozenset")
     _seqs = oneof_names("list", "sorted", "tuple")
 
-    @m.leave(
+    @leave(
         m.Call(
             func=_sets,
             args=[m.Arg(m.Call(func=_sets | _seqs | m.Name("reversed")), star="")],
         )
         | m.Call(
             func=oneof_names("list", "tuple"),
             args=[m.Arg(m.Call(func=oneof_names("list", "tuple")), star="")],
@@ -277,30 +302,30 @@
             return updated_node
 
         return updated_node.with_changes(
             args=[cst.Arg(updated_node.args[0].value.args[0].value)]
             + list(updated_node.args[1:]),
         )
 
-    @m.leave(
+    @leave(
         m.Call(
             func=oneof_names("reversed", "set", "sorted"),
             args=[m.Arg(m.Subscript(slice=[m.SubscriptElement(ALL_ELEMS_SLICE)]))],
         )
     )
     def replace_unnecessary_subscript_reversal(self, _, updated_node):
         """Fix flake8-comprehensions C415.
 
         Unnecessary subscript reversal of iterable within <reversed/set/sorted>().
         """
         return updated_node.with_changes(
             args=[cst.Arg(updated_node.args[0].value.value)],
         )
 
-    @m.leave(
+    @leave(
         multi(
             m.ListComp,
             m.SetComp,
             elt=m.Name(),
             for_in=m.CompFor(
                 target=m.Name(), ifs=[], inner_for_in=None, asynchronous=None
             ),
@@ -312,39 +337,39 @@
         Unnecessary <list/set> comprehension - rewrite using <list/set>().
         """
         if updated_node.elt.value == updated_node.for_in.target.value:
             func = cst.Name("list" if isinstance(updated_node, cst.ListComp) else "set")
             return cst.Call(func=func, args=[cst.Arg(updated_node.for_in.iter)])
         return updated_node
 
-    @m.leave(m.Subscript(oneof_names("Union", "Literal")))
+    @leave(m.Subscript(oneof_names("Union", "Literal")))
     def reorder_union_literal_contents_none_last(self, _, updated_node):
         subscript = list(updated_node.slice)
         try:
             has_comma = isinstance(subscript[-1].comma, cst.Comma)
             subscript.sort(key=lambda elt: elt.slice.value.value == "None")
             if not has_comma:
                 subscript[-1] = remove_trailing_comma(subscript[-1])
             return updated_node.with_changes(slice=subscript)
         except Exception:  # Single-element literals are not slices, etc.
             return updated_node
 
-    @m.leave(
+    @leave(
         m.Subscript(
             m.Name("Optional"),
             [m.SubscriptElement(m.Index(m.Subscript(value=m.Name("Union"))))],
         )
     )
     def reorder_merge_optional_union(self, _, updated_node):
         union = updated_node.slice[0].slice.value
         none = [cst.SubscriptElement(cst.Index(cst.Name("None")))]
         return union.with_changes(slice=list(union.slice) + none)
 
     @m.call_if_inside(m.Annotation(annotation=m.BinaryOperation()))
-    @m.leave(
+    @leave(
         m.BinaryOperation(
             left=m.Name("None") | m.BinaryOperation(),
             operator=m.BitOr(),
             right=m.DoNotCare(),
         )
     )
     def reorder_union_operator_contents_none_last(self, _, updated_node):
@@ -358,25 +383,25 @@
 
         node_left = updated_node.left
         if _has_none(node_left):
             return updated_node.with_changes(left=updated_node.right, right=node_left)
         else:
             return updated_node
 
-    @m.leave(m.Subscript(value=m.Name("Literal")))
+    @leave(m.Subscript(value=m.Name("Literal")))
     def flatten_literal_subscript(self, _, updated_node):
         new_slice = []
         for item in updated_node.slice:
             if m.matches(item.slice.value, m.Subscript(m.Name("Literal"))):
                 new_slice += item.slice.value.slice
             else:
                 new_slice.append(item)
         return updated_node.with_changes(slice=new_slice)
 
-    @m.leave(m.Subscript(value=m.Name("Union")))
+    @leave(m.Subscript(value=m.Name("Union")))
     def flatten_union_subscript(self, _, updated_node):
         new_slice = []
         has_none = False
         for item in updated_node.slice:
             if m.matches(item.slice.value, m.Subscript(m.Name("Optional"))):
                 new_slice += item.slice.value.slice  # peel off "Optional"
                 has_none = True
@@ -388,24 +413,24 @@
                 has_none = True
             else:
                 new_slice.append(item)
         if has_none:
             new_slice.append(cst.SubscriptElement(slice=cst.Index(cst.Name("None"))))
         return updated_node.with_changes(slice=new_slice)
 
-    @m.leave(m.Else(m.IndentedBlock([m.SimpleStatementLine([m.Pass()])])))
+    @leave(m.Else(m.IndentedBlock([m.SimpleStatementLine([m.Pass()])])))
     def discard_empty_else_blocks(self, _, updated_node):
         # An `else: pass` block can always simply be discarded, and libcst ensures
         # that an Else node can only ever occur attached to an If, While, For, or Try
         # node; in each case `None` is the valid way to represent "no else block".
         if m.findall(updated_node, m.Comment()):
             return updated_node  # If there are any comments, keep the node
         return cst.RemoveFromParent()
 
-    @m.leave(
+    @leave(
         m.Lambda(
             params=m.MatchIfTrue(
                 lambda node: (
                     node.star_kwarg is None
                     and not node.kwonly_params
                     and not node.posonly_params
                     and isinstance(node.star_arg, cst.MaybeSentinel)
@@ -419,15 +444,15 @@
             m.Arg(m.Name(param.name.value), star="", keyword=None)
             for param in updated_node.params.params
         ]
         if m.matches(updated_node.body, m.Call(args=same_args)):
             return cst.ensure_type(updated_node.body, cst.Call).func
         return updated_node
 
-    @m.leave(
+    @leave(
         m.BooleanOperation(
             left=m.Call(m.Name("isinstance"), [m.Arg(), m.Arg()]),
             operator=m.Or(),
             right=m.Call(m.Name("isinstance"), [m.Arg(), m.Arg()]),
         )
     )
     def collapse_isinstance_checks(self, _, updated_node):
@@ -538,15 +563,15 @@
                     comments.append(line.comment)
         comments.extend(old_comments)
         # remaining comments are handled by the caller afterwards
 
         return nodes
 
     # split `assert a and b` into `assert a` and `assert b`
-    @m.leave(
+    @leave(
         m.SimpleStatementLine(
             body=[m.Assert(msg=None, test=m.BooleanOperation(operator=m.And()))]
         )
     )
     def split_assert_and(self, _, updated_node):
         # the simple statements trailing whitespace may be on the same line
         # as the first assert, or if there's sufficient comments within the assert
@@ -580,52 +605,58 @@
             nodes.append(
                 cst.SimpleStatementLine(
                     [cst.Pass()],  # pointless-pass is removed by autoflake later
                     [cst.EmptyLine(comment=c) for c in comments],
                     cst.TrailingWhitespace(whitespace=cst.SimpleWhitespace(" ")),
                 )
             )
+        # work around https://github.com/Instagram/LibCST/issues/911
+        try:
+            cst.parse_module(cst.Module([*nodes]).code)
+        except Exception:
+            return updated_node
         return cst.FlattenSentinel(nodes)
 
     # Remove unnecessary len() and bool() calls in tests
     # we can't use call_if_inside since it matches on any parents, which breaks on
     # complicated nested cases - so we have to split into different leave's
     # len/bool inside boolops (and/or) can only be removed if the boolop is inside a test
     # otherwise `print(False or bool(5))` changes functionality (prints `True` vs `5`)
-    @m.leave(
+    @leave(
         multi(
             m.If,
             m.IfExp,
             m.While,
             test=_collapsible_expression(),
         )
     )
     def remove_unnecessary_call_test(self, _, updated_node):
         return self._collapse_attribute(updated_node, "test")
 
     # remove not:ed len/bool
     # `not len(foo)` -> `not foo`
-    @m.leave(m.UnaryOperation(operator=m.Not(), expression=_collapsible_expression()))
+    @leave(m.UnaryOperation(operator=m.Not(), expression=_collapsible_expression()))
     def remove_unnecessary_call_expression(self, _, updated_node):
         return self._collapse_attribute(updated_node, "expression")
 
     # used by the above functions
     @classmethod
     def _collapse_attribute(cls, node, attr):
         child_node = getattr(node, attr)
+
         # if the attribute is a boolop, recurse through it and replace len/bool that are
         # direct child nodes to (a chain of) boolops
         if isinstance(child_node, cst.BooleanOperation):
             return node.with_changes(**{attr: cls._remove_recursive_helper(child_node)})
         # otherwise just remove the len/bool
         return node.with_changes(**{attr: child_node.args[0]})
 
     # remove len/bool inside bool()
     # `bool(len(foo))` or `bool(bool(foo))` -> `bool(foo)`
-    @m.leave(m.Call(func=m.Name("bool"), args=[m.Arg(value=_collapsible_expression())]))
+    @leave(m.Call(func=m.Name("bool"), args=[m.Arg(value=_collapsible_expression())]))
     def remove_unnecessary_call2(self, _, updated_node):
         collapse_node = updated_node.args[0].value
         if isinstance(collapse_node, cst.BooleanOperation):
             return updated_node.with_deep_changes(
                 updated_node.args[0], value=self._remove_recursive_helper(collapse_node)
             )
```

### Comparing `shed-2023.3.1/src/shed.egg-info/PKG-INFO` & `shed-2023.4.1/src/shed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shed
-Version: 2023.3.1
+Version: 2023.4.1
 Summary: `shed` canonicalises Python code.
 Home-page: https://github.com/Zac-HD/shed
 Author: Zac Hatfield-Dodds
 Author-email: zac@zhd.dev
 License: AGPL-3.0
 Project-URL: Source, https://github.com/Zac-HD/shed/
 Project-URL: Changelog, https://github.com/Zac-HD/shed/blob/master/CHANGELOG.md
@@ -77,15 +77,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with Shed by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/Zac-HD/shed
-  rev: 2023.3.1
+  rev: 2023.4.1
   hooks:
     - id: shed
       # args: [--refactor, --py39-plus]
       types_or: [python, pyi, markdown, rst]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
```

### Comparing `shed-2023.3.1/tests/test_expected_output.py` & `shed-2023.4.1/tests/test_expected_output.py`

 * *Files identical despite different names*

### Comparing `shed-2023.3.1/tests/test_shed.py` & `shed-2023.4.1/tests/test_shed.py`

 * *Files identical despite different names*

### Comparing `shed-2023.3.1/tests/test_version.py` & `shed-2023.4.1/tests/test_version.py`

 * *Files identical despite different names*

