# Comparing `tmp/funcs-0.2.4.tar.gz` & `tmp/funcs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs-0.2.4.tar", max compression
+gzip compressed data, was "funcs-0.3.0.tar", max compression
```

## Comparing `funcs-0.2.4.tar` & `funcs-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1092 2023-04-18 12:18:39.584657 funcs-0.2.4/LICENSE
--rw-r--r--   0        0        0     2872 2023-04-18 12:18:39.584657 funcs-0.2.4/README.md
--rw-r--r--   0        0        0     1664 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/__init__.py
--rw-r--r--   0        0        0      883 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/application.py
--rw-r--r--   0        0        0      563 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/callers.py
--rw-r--r--   0        0        0     4121 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/composition.py
--rw-r--r--   0        0        0      431 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/debug.py
--rw-r--r--   0        0        0      166 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/decorators.py
--rw-r--r--   0        0        0     3595 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/flow.py
--rw-r--r--   0        0        0      899 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/functions.py
--rw-r--r--   0        0        0      418 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/getters.py
--rw-r--r--   0        0        0      264 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/primitives.py
--rw-r--r--   0        0        0        0 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/py.typed
--rw-r--r--   0        0        0      492 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/reduction.py
--rw-r--r--   0        0        0      475 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/types.py
--rw-r--r--   0        0        0     3482 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/typing.py
--rw-r--r--   0        0        0     1369 2023-04-18 12:18:39.584657 funcs-0.2.4/funcs/unpacking.py
--rw-r--r--   0        0        0     3022 2023-04-18 12:18:39.584657 funcs-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 funcs-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-20 10:46:51.302748 funcs-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2872 2023-04-20 10:46:51.302748 funcs-0.3.0/README.md
+-rw-r--r--   0        0        0     1690 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/__init__.py
+-rw-r--r--   0        0        0      883 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/application.py
+-rw-r--r--   0        0        0      563 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/callers.py
+-rw-r--r--   0        0        0     4121 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/composition.py
+-rw-r--r--   0        0        0      431 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/debug.py
+-rw-r--r--   0        0        0      166 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/decorators.py
+-rw-r--r--   0        0        0     3595 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/flow.py
+-rw-r--r--   0        0        0     1139 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/functions.py
+-rw-r--r--   0        0        0      418 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/getters.py
+-rw-r--r--   0        0        0      264 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/primitives.py
+-rw-r--r--   0        0        0        0 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/py.typed
+-rw-r--r--   0        0        0      492 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/reduction.py
+-rw-r--r--   0        0        0      475 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/types.py
+-rw-r--r--   0        0        0     3482 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/typing.py
+-rw-r--r--   0        0        0     1369 2023-04-20 10:46:51.302748 funcs-0.3.0/funcs/unpacking.py
+-rw-r--r--   0        0        0     3022 2023-04-20 10:46:51.302748 funcs-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 funcs-0.3.0/PKG-INFO
```

### Comparing `funcs-0.2.4/LICENSE` & `funcs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs-0.2.4/README.md` & `funcs-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.2.4"
+funcs = "^0.3.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

### Comparing `funcs-0.2.4/funcs/__init__.py` & `funcs-0.3.0/funcs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 __description__ = "Functional programming in Python."
 __url__ = "https://github.com/nekitdev/funcs"
 
 __title__ = "funcs"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.2.4"
+__version__ = "0.3.0"
 
 from funcs.application import apply, partial
 from funcs.callers import caller, method_caller
 from funcs.composition import compose, compose_once, pipe, pipe_once
 from funcs.debug import tap
 from funcs.decorators import wraps
 from funcs.flow import once, post_processing, reraise, reraise_with, suppress, wrap_with
-from funcs.functions import always, complement, flip, identity, raises
+from funcs.functions import always, asyncify, complement, flip, identity, raises
 from funcs.getters import attribute_getter, item_getter
 from funcs.primitives import decrement, increment, is_even, is_odd
 from funcs.reduction import fold, reduce
 from funcs.unpacking import (
     unpack_binary,
     unpack_nullary,
     unpack_quaternary,
@@ -46,14 +46,15 @@
     "once",
     "reraise",
     "reraise_with",
     "suppress",
     "post_processing",
     "wrap_with",
     # functions
+    "asyncify",
     "identity",
     "always",
     "raises",
     "flip",
     "complement",
     # getters
     "attribute_getter",
```

### Comparing `funcs-0.2.4/funcs/application.py` & `funcs-0.3.0/funcs/application.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.4/funcs/callers.py` & `funcs-0.3.0/funcs/callers.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.4/funcs/composition.py` & `funcs-0.3.0/funcs/composition.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.4/funcs/flow.py` & `funcs-0.3.0/funcs/flow.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.4/funcs/functions.py` & `funcs-0.3.0/funcs/functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,30 @@
-from typing import TypeVar
+from typing import Callable, TypeVar
 
 from typing_extensions import Never, ParamSpec
 
-from funcs.typing import AnyError, Binary, GenericPredicate, Nullary
+from funcs.typing import AnyError, AsyncCallable, Binary, GenericPredicate, Nullary
 
-__all__ = ("identity", "always", "raises", "flip", "complement")
+__all__ = ("asyncify", "identity", "always", "raises", "flip", "complement")
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 R = TypeVar("R")
 
 P = ParamSpec("P")
 
 
+def asyncify(function: Callable[P, R]) -> AsyncCallable[P, R]:
+    async def async_function(*args: P.args, **kwargs: P.kwargs) -> R:
+        return function(*args, **kwargs)
+
+    return async_function
+
+
 def identity(item: T) -> T:
     return item
 
 
 def always(item: T) -> Nullary[T]:
     def return_item() -> T:
         return item
```

### Comparing `funcs-0.2.4/funcs/typing.py` & `funcs-0.3.0/funcs/typing.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.4/funcs/unpacking.py` & `funcs-0.3.0/funcs/unpacking.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.4/pyproject.toml` & `funcs-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funcs"
-version = "0.2.4"
+version = "0.3.0"
 description = "Functional programming in Python."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/funcs"
@@ -126,15 +126,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "funcs"
-version = "0.2.4"
+version = "0.3.0"
 url = "https://github.com/nekitdev/funcs"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `funcs-0.2.4/PKG-INFO` & `funcs-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs
-Version: 0.2.4
+Version: 0.3.0
 Summary: Functional programming in Python.
 Home-page: https://github.com/nekitdev/funcs
 License: MIT
 Keywords: python,function,functional,paradigm
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -70,15 +70,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.2.4"
+funcs = "^0.3.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

