# Comparing `tmp/danielutils-0.8.3.tar.gz` & `tmp/danielutils-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.8.3.tar", last modified: Thu Apr 20 16:14:01 2023, max compression
+gzip compressed data, was "danielutils-0.8.5.tar", last modified: Thu Apr 20 20:48:55 2023, max compression
```

## Comparing `danielutils-0.8.3.tar` & `danielutils-0.8.5.tar`

### file list

```diff
@@ -1,60 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 16:14:01.443238 danielutils-0.8.3/
--rw-rw-rw-   0        0        0      939 2023-04-20 16:14:01.443238 danielutils-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-20 16:14:01.000000 danielutils-0.8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 16:14:01.411418 danielutils-0.8.3/danielutils/
-drwxrwxrwx   0        0        0        0 2023-04-20 16:14:01.430628 danielutils-0.8.3/danielutils/Classes/
--rw-rw-rw-   0        0        0      103 2023-04-02 21:16:20.000000 danielutils-0.8.3/danielutils/Classes/Convenience.py
--rw-rw-rw-   0        0        0     1694 2023-04-02 21:17:25.000000 danielutils-0.8.3/danielutils/Classes/DataStructures.py
--rw-rw-rw-   0        0        0     3489 2023-04-11 21:22:44.000000 danielutils-0.8.3/danielutils/Classes/TypedBuiltins.py
--rw-rw-rw-   0        0        0      117 2023-03-30 21:30:39.000000 danielutils-0.8.3/danielutils/Classes/__init__.py
--rw-rw-rw-   0        0        0      904 2023-03-30 21:22:39.000000 danielutils-0.8.3/danielutils/Classes/frange.py
--rw-rw-rw-   0        0        0     1968 2023-04-11 20:58:21.000000 danielutils-0.8.3/danielutils/Colors.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:14:01.431626 danielutils-0.8.3/danielutils/Conversions/
--rw-rw-rw-   0        0        0     1797 2023-04-11 21:02:02.000000 danielutils-0.8.3/danielutils/Conversions/MainConversions.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:14:01.433625 danielutils-0.8.3/danielutils/Conversions/SpecializedConversions/
--rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.8.3/danielutils/Conversions/SpecializedConversions/__init__.py
--rw-rw-rw-   0        0        0      454 2022-10-14 16:32:03.000000 danielutils-0.8.3/danielutils/Conversions/SpecializedConversions/to_hex.py
--rw-rw-rw-   0        0        0      389 2022-10-28 08:08:26.000000 danielutils-0.8.3/danielutils/Conversions/SpecializedConversions/to_int.py
--rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.8.3/danielutils/Conversions/__init__.py
--rw-rw-rw-   0        0        0      270 2023-04-11 20:59:09.000000 danielutils-0.8.3/danielutils/Data.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:14:01.439229 danielutils-0.8.3/danielutils/DataStructures/
--rw-rw-rw-   0        0        0      781 2023-04-19 18:35:04.000000 danielutils-0.8.3/danielutils/DataStructures/Comparer.py
--rw-rw-rw-   0        0        0     2503 2023-04-11 21:02:02.000000 danielutils-0.8.3/danielutils/DataStructures/Graph.py
--rw-rw-rw-   0        0        0     2558 2023-04-18 23:54:19.000000 danielutils-0.8.3/danielutils/DataStructures/Heap.py
--rw-rw-rw-   0        0        0     7883 2023-04-20 16:13:07.000000 danielutils-0.8.3/danielutils/DataStructures/Interface.py
--rw-rw-rw-   0        0        0     2564 2023-04-11 21:26:28.000000 danielutils-0.8.3/danielutils/DataStructures/MarkovChain.py
--rw-rw-rw-   0        0        0      309 2023-04-19 18:35:04.000000 danielutils-0.8.3/danielutils/DataStructures/Node.py
--rw-rw-rw-   0        0        0     1417 2023-04-19 18:35:04.000000 danielutils-0.8.3/danielutils/DataStructures/Queue.py
--rw-rw-rw-   0        0        0      165 2023-04-19 18:35:04.000000 danielutils-0.8.3/danielutils/DataStructures/__init__.py
--rw-rw-rw-   0        0        0      281 2023-04-18 23:56:59.000000 danielutils-0.8.3/danielutils/DataStructures/functions.py
--rw-rw-rw-   0        0        0    19818 2023-04-20 13:12:08.000000 danielutils-0.8.3/danielutils/Decorators.py
--rw-rw-rw-   0        0        0     1122 2023-04-03 14:02:27.000000 danielutils-0.8.3/danielutils/Exceptions.py
--rw-rw-rw-   0        0        0     8193 2023-04-03 11:53:26.000000 danielutils-0.8.3/danielutils/Functions.py
--rw-rw-rw-   0        0        0     7503 2023-04-18 20:35:49.000000 danielutils-0.8.3/danielutils/IO.py
--rw-rw-rw-   0        0        0     1259 2023-04-11 21:00:13.000000 danielutils-0.8.3/danielutils/Internet.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:14:01.442237 danielutils-0.8.3/danielutils/Math/
--rw-rw-rw-   0        0        0     6036 2022-10-28 20:26:06.000000 danielutils-0.8.3/danielutils/Math/Constants.py
--rw-rw-rw-   0        0        0      205 2023-04-11 21:02:02.000000 danielutils-0.8.3/danielutils/Math/Functions.py
--rw-rw-rw-   0        0        0      860 2023-04-03 18:56:27.000000 danielutils-0.8.3/danielutils/Math/MathPrint.py
--rw-rw-rw-   0        0        0     6485 2023-04-02 21:11:12.000000 danielutils-0.8.3/danielutils/Math/MathSymbols.py
--rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.8.3/danielutils/Math/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-01-12 01:01:37.000000 danielutils-0.8.3/danielutils/Path.py
--rw-rw-rw-   0        0        0     2686 2023-04-11 13:05:54.000000 danielutils-0.8.3/danielutils/Print.py
--rw-rw-rw-   0        0        0     1357 2023-01-05 22:01:09.000000 danielutils-0.8.3/danielutils/Serialization.py
--rw-rw-rw-   0        0        0     6061 2023-04-17 13:50:25.000000 danielutils-0.8.3/danielutils/System.py
--rw-rw-rw-   0        0        0     6699 2023-04-11 21:23:44.000000 danielutils-0.8.3/danielutils/Testing.py
--rw-rw-rw-   0        0        0     2895 2023-04-11 21:02:02.000000 danielutils-0.8.3/danielutils/Text.py
--rw-rw-rw-   0        0        0      423 2023-04-18 23:27:35.000000 danielutils-0.8.3/danielutils/Threading.py
--rw-rw-rw-   0        0        0      426 2023-04-11 21:07:07.000000 danielutils-0.8.3/danielutils/Time.py
--rw-rw-rw-   0        0        0      649 2023-01-18 20:34:53.000000 danielutils-0.8.3/danielutils/Typing.py
--rw-rw-rw-   0        0        0     1248 2023-04-02 14:10:39.000000 danielutils-0.8.3/danielutils/Windows.py
--rw-rw-rw-   0        0        0      480 2023-04-03 18:57:22.000000 danielutils-0.8.3/danielutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:14:01.427017 danielutils-0.8.3/danielutils.egg-info/
--rw-rw-rw-   0        0        0      939 2023-04-20 16:14:01.000000 danielutils-0.8.3/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1534 2023-04-20 16:14:01.000000 danielutils-0.8.3/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 16:14:01.000000 danielutils-0.8.3/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-20 16:14:01.000000 danielutils-0.8.3/danielutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-20 16:14:01.000000 danielutils-0.8.3/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      728 2023-04-20 16:14:01.000000 danielutils-0.8.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 16:14:01.444238 danielutils-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-04-20 16:14:01.000000 danielutils-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.962430 danielutils-0.8.5/
+-rw-rw-rw-   0        0        0      939 2023-04-20 20:48:55.962430 danielutils-0.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-04-20 20:48:55.000000 danielutils-0.8.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.930903 danielutils-0.8.5/danielutils/
+drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.947604 danielutils-0.8.5/danielutils/Classes/
+-rw-rw-rw-   0        0        0      210 2023-04-20 17:59:42.000000 danielutils-0.8.5/danielutils/Classes/Convenience.py
+-rw-rw-rw-   0        0        0     3904 2023-04-20 20:37:29.000000 danielutils-0.8.5/danielutils/Classes/TypedBuiltins.py
+-rw-rw-rw-   0        0        0      107 2023-04-20 18:11:11.000000 danielutils-0.8.5/danielutils/Classes/__init__.py
+-rw-rw-rw-   0        0        0     1027 2023-04-20 20:24:10.000000 danielutils-0.8.5/danielutils/Classes/frange.py
+-rw-rw-rw-   0        0        0     3983 2023-04-20 17:12:55.000000 danielutils-0.8.5/danielutils/Colors.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.949101 danielutils-0.8.5/danielutils/Conversions/
+-rw-rw-rw-   0        0        0     2227 2023-04-20 19:56:42.000000 danielutils-0.8.5/danielutils/Conversions/MainConversions.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.952538 danielutils-0.8.5/danielutils/Conversions/SpecializedConversions/
+-rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.8.5/danielutils/Conversions/SpecializedConversions/__init__.py
+-rw-rw-rw-   0        0        0      476 2023-04-20 20:15:32.000000 danielutils-0.8.5/danielutils/Conversions/SpecializedConversions/to_hex.py
+-rw-rw-rw-   0        0        0      407 2023-04-20 17:57:46.000000 danielutils-0.8.5/danielutils/Conversions/SpecializedConversions/to_int.py
+-rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.8.5/danielutils/Conversions/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-04-20 17:15:00.000000 danielutils-0.8.5/danielutils/Data.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.957603 danielutils-0.8.5/danielutils/DataStructures/
+-rw-rw-rw-   0        0        0     1569 2023-04-20 20:36:21.000000 danielutils-0.8.5/danielutils/DataStructures/Comparer.py
+-rw-rw-rw-   0        0        0     3299 2023-04-20 20:00:10.000000 danielutils-0.8.5/danielutils/DataStructures/Heap.py
+-rw-rw-rw-   0        0        0    10238 2023-04-20 20:35:30.000000 danielutils-0.8.5/danielutils/DataStructures/Interface.py
+-rw-rw-rw-   0        0        0      412 2023-04-20 20:11:14.000000 danielutils-0.8.5/danielutils/DataStructures/Node.py
+-rw-rw-rw-   0        0        0     4364 2023-04-20 20:34:31.000000 danielutils-0.8.5/danielutils/DataStructures/Queue.py
+-rw-rw-rw-   0        0        0      115 2023-04-20 20:05:37.000000 danielutils-0.8.5/danielutils/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-04-20 20:07:14.000000 danielutils-0.8.5/danielutils/DataStructures/functions.py
+-rw-rw-rw-   0        0        0    16029 2023-04-20 20:29:28.000000 danielutils-0.8.5/danielutils/Decorators.py
+-rw-rw-rw-   0        0        0     2127 2023-04-20 19:47:46.000000 danielutils-0.8.5/danielutils/Exceptions.py
+-rw-rw-rw-   0        0        0     5372 2023-04-20 20:44:36.000000 danielutils-0.8.5/danielutils/Functions.py
+-rw-rw-rw-   0        0        0     9251 2023-04-20 19:48:57.000000 danielutils-0.8.5/danielutils/IO.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.960923 danielutils-0.8.5/danielutils/Math/
+-rw-rw-rw-   0        0        0     7682 2023-04-20 20:14:55.000000 danielutils-0.8.5/danielutils/Math/Constants.py
+-rw-rw-rw-   0        0        0      347 2023-04-20 20:10:18.000000 danielutils-0.8.5/danielutils/Math/Functions.py
+-rw-rw-rw-   0        0        0     1045 2023-04-20 18:34:15.000000 danielutils-0.8.5/danielutils/Math/MathPrint.py
+-rw-rw-rw-   0        0        0     3779 2023-04-20 17:25:45.000000 danielutils-0.8.5/danielutils/Math/MathSymbols.py
+-rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.8.5/danielutils/Math/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-01-12 01:01:37.000000 danielutils-0.8.5/danielutils/Path.py
+-rw-rw-rw-   0        0        0     2686 2023-04-11 13:05:54.000000 danielutils-0.8.5/danielutils/Print.py
+-rw-rw-rw-   0        0        0     6089 2023-04-20 19:51:00.000000 danielutils-0.8.5/danielutils/System.py
+-rw-rw-rw-   0        0        0     4204 2023-04-20 18:50:09.000000 danielutils-0.8.5/danielutils/Text.py
+-rw-rw-rw-   0        0        0      612 2023-04-20 19:52:02.000000 danielutils-0.8.5/danielutils/Threading.py
+-rw-rw-rw-   0        0        0      426 2023-04-11 21:07:07.000000 danielutils-0.8.5/danielutils/Time.py
+-rw-rw-rw-   0        0        0     2138 2023-04-20 19:32:32.000000 danielutils-0.8.5/danielutils/Windows.py
+-rw-rw-rw-   0        0        0      555 2023-04-20 20:23:42.000000 danielutils-0.8.5/danielutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:48:55.945605 danielutils-0.8.5/danielutils.egg-info/
+-rw-rw-rw-   0        0        0      939 2023-04-20 20:48:55.000000 danielutils-0.8.5/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1320 2023-04-20 20:48:55.000000 danielutils-0.8.5/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 20:48:55.000000 danielutils-0.8.5/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-20 20:48:55.000000 danielutils-0.8.5/danielutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 20:48:55.000000 danielutils-0.8.5/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      728 2023-04-20 20:48:55.000000 danielutils-0.8.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 20:48:55.962430 danielutils-0.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-04-20 20:48:55.000000 danielutils-0.8.5/setup.py
```

### Comparing `danielutils-0.8.3/PKG-INFO` & `danielutils-0.8.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.8.3
+Version: 0.8.5
 Summary: A python utils library for things I find useful
 Home-page: https://github.com/danielnachumdev/danielutils
 Author: danielnachumdev
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/danielnachumdev/danielutils
 Project-URL: Bug Tracker, https://github.com/danielnachumdev/danielutils/issues
@@ -12,12 +12,12 @@
 Platform: All
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.10.5
 Description-Content-Type: text/markdown
 
-# danielutils v=0.8.3
+# danielutils v=0.8.5
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
```

### Comparing `danielutils-0.8.3/danielutils/Classes/TypedBuiltins.py` & `danielutils-0.8.5/danielutils/Classes/TypedBuiltins.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,103 +1,119 @@
 from __future__ import annotations
-from ..Typing import Any, Union, Iterable
+from typing import Any, Iterable
 from ..Decorators import validate, overload
 from ..Functions import isoftype
 
 
 class tlist(list):
     """tlist is same as builtin python list but with added type restriction
 
     Args:
         type (type): the allowed type, can be nested type
         iterable (Iterable, optional): the value to create the tlist from. Defaults to None.
     """
 
-    def get_type_error_msg(self, v: Any):
-        return f"A value is of the wrong type:\n'{v}' is of type '{type(v)}' but should be of type '{self.type}'"
+    def _get_error_msg(self, v: Any) -> str:
+        """generates the generic error message
+
+        Args:
+            v (Any): value to include in the message
+
+        Returns:
+            str: the error message
+        """
+        return f"A value is of the wrong type:\n'{v}' is of type '{type(v)}' but should be of type '{self.T}'"
 
     @validate
-    def __init__(self: Any, type: type, iterable: Iterable = None):
+    def __init__(self, T: type, iterable: Iterable = None):
         """_summary_
 
         Args:
             type (type): the allowed type, can be nested type
-        ietrable (Iterable, optional): the value to create the tlist from. Defaults to None.
+        iterable (Iterable, optional): the value to create the tlist from. Defaults to None.
 
         Raises:
             TypeError: _description_
         """
-        self.type = type
+        self.T = T
         if iterable is not None:
             for v in iterable:
-                if not isoftype(v, type):
-                    raise TypeError(self.get_type_error_msg(v))
+                if not isoftype(v, T):
+                    raise TypeError(self._get_error_msg(v))
                 super().append(v)
 
     def __setitem__(self, index: int, value: Any) -> None:
-        if not isoftype(value, self.type):
-            raise TypeError(self.get_type_error_msg(value))
+        if not isoftype(value, self.T):
+            raise TypeError(self._get_error_msg(value))
         super()[index] = value
 
     def append(self, value: Any) -> None:
-        if not isoftype(value, self.type):
-            raise TypeError(self.get_type_error_msg(value))
+        if not isoftype(value, self.T):
+            raise TypeError(self._get_error_msg(value))
         super().append(value)
 
     @validate
-    def extend(self: Any, iterable: Iterable) -> None:
+    def extend(self, iterable: Iterable) -> None:
         for v in iterable:
             self.append(v)
 
-    def __add__(self, other) -> tlist:
-        pass
+    # TODO implement this function
+    def __add__(self, other: tlist | list) -> tlist:
+        raise NotImplementedError("Should be implemented")
 
 
 class tdict(dict):
+    """like builtin dict but only a specif type is allowed
+    """
     @overload(None, type, type)
     def __init__(self, key_t: type, val_t: type):
         self.key_t = key_t
         self.val_t = val_t
         super().__init__()
 
     @overload(None, type, type, Iterable)
     def __init__(self, keyt: type, val_t: type, iterable: Iterable[tuple]):
         self.key_t = keyt
         self.val_t = val_t
         super().__init__(iterable)
 
     @overload(None, type, type, dict)
-    def __init__(self, keyt: type, val_t: type, ** kwargs):
+    def __init__(self, key_t: type, val_t: type, ** kwargs):
         """dict(type,type) -> new empty dictionary dict(mapping) -> new dictionary initialized from a mapping object's
     (key, value) pairs
 dict(type,type,iterable) -> new dictionary initialized as if via:
     d = {} for k, v in iterable:
         d[k] = v
 dict(type,type,**kwargs) -> new dictionary initialized with the name=value pairs
     in the keyword argument list. For example: dict(one=1, two=2)
         """
-        self.key_t = keyt
+        self.key_t = key_t
         self.val_t = val_t
         super().__init__(**kwargs)
 
     def __setitem__(self, key, value) -> None:
         if not isoftype(key, self.key_t):
             raise TypeError(
-                f"In class 'tdict' error creating new key-value pair as key = '{key}' is not of type '{self.key_t}'")
+                f"In class 'tdict' error creating new key-value pair as"
+                f" key = '{key}' is not of type '{self.key_t}'")
         if not isoftype(value, self.val_t):
             raise TypeError(
-                f"In class 'tdict' error creating new key-value pair as value = '{value}' is not of type '{ self.val_t}'")
+                f"In class 'tdict' error creating new key-value pair"
+                f" as value = '{value}' is not of type '{ self.val_t}'")
         super().__setitem__(key, value)
 
     def __str__(self):
         return f"dict[{self.key_t.__name__}, {self.val_t.__name__}]: {super().__str__()}"
 
 
 # TODO tset
 class tset(set):
+    """like builtin set but only allows specified type
+    """
+
     def __init__(self):
         pass
 
 
 __all__ = [
     "tlist",
     "tdict"
```

### Comparing `danielutils-0.8.3/danielutils/Conversions/MainConversions.py` & `danielutils-0.8.5/danielutils/Conversions/MainConversions.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,24 +77,48 @@
         str: _description_
     """
     return int_to_hex(num)
 
 
 @validate
 def int_to_hex(num: int) -> str:
+    """converts an int to it's hex representation
+
+    Args:
+        num (int): int to convert
+
+    Returns:
+        str: the hex representation of the int
+    """
     return hex(num)
 
 
 @validate
 def bytes_to_str(b: bytes) -> str:
+    """decodes bytes to str
+
+    Args:
+        b (bytes): bytes to decode
+
+    Returns:
+        str: result
+    """
     return b.decode("utf-8")
 
 
 @validate
 def str_to_bytes(s: str) -> bytes:
+    """encodes a string to bytes
+
+    Args:
+        s (str): the string to encode
+
+    Returns:
+        bytes: result
+    """
     return bytes(s, encoding='utf-8')
 
 
 __all__ = [
     "char_to_int",
     "int_to_char",
     "hex_to_char",
```

### Comparing `danielutils-0.8.3/danielutils/Decorators.py` & `danielutils-0.8.5/danielutils/Decorators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-import traceback
 import re
-from .Typing import Callable, Any, Union
+import traceback
 import functools
-import threading
 import inspect
-from .Functions import areoneof, isoneof, isoneof_strict, isoftype
+import threading
+from typing import Callable, Any
+from .Functions import isoneof, isoneof_strict, isoftype
 from .Exceptions import *
 
 
 def validate(func: Callable) -> Callable:
-    """A decorator that validates the annotations and types of the arguments and return value of a function.
+    """A decorator that validates the annotations and types of the arguments and return
+    value of a function.
 
         * 'None' is allowed as default value for everything
-        * Because of their use in classes, the generally accepted keywords 'self' and 'cls' are not validated to not break intellisense when using 'Any'
+        * Because of their use in classes, the generally accepted keywords 'self' and 'cls'
+        are not validated to not break intellisense when using 'Any'
 
     Args:
         func (Callable): The function to be decorated.
 
     Raises:
         TypeError: if the decorated object is nto a Callable
         EmptyAnnotationException: If an argument is not annotated.
@@ -45,158 +47,73 @@
         if default_value != inspect.Parameter.empty:
             # allow everything to be set to None as default
             if default_value is None:
                 continue
             # if it does, check the type of the default value
             if not isoftype(default_value, arg_type):
                 raise InvalidDefaultValueException(
-                    f"In {func_name}, argument '{arg_name}'s default value is annotated as {arg_type} but got '{default_value}' which is {type(default_value)}")
+                    f"In {func_name}, argument '{arg_name}'s default value is annotated \
+                    as {arg_type} but got '{default_value}' which is {type(default_value)}")
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         """wrapper function for the type validating - will run on each call independently
         """
         # check all arguments
         bound = signature.bind(*args, **kwargs)
         for variable_name, variable_value in bound.arguments.items():
             annotated_type = signature.parameters[variable_name].annotation
             expected_type = func.__annotations__[variable_name]
             if not isoftype(variable_value, expected_type):
                 raise ValidationException(
-                    f"In {func_name}, argument '{variable_name}' is annotated as {annotated_type} but got '{variable_value}' which is {type(variable_value)}")
+                    f"In {func_name}, argument '{variable_name}' is annotated as \
+                        {annotated_type} but got '{variable_value}' which is {type(variable_value)}")
 
         # call the function
         result = func(*args, **kwargs)
 
         # check the return type
         return_type = type(None) if ("inspect._empty" in str(signature.return_annotation)
                                      or signature.return_annotation is None) else signature.return_annotation
         if not isoftype(result, return_type):
             raise InvalidReturnValueException(
-                f"In function {func_name}, the return type is annotated as {return_type} but got '{result}' which is {type(result)}")
+                f"In function {func_name}, the return type is annotated as \
+                {return_type} but got '{result}' which is {type(result)}")
         return result
     return wrapper
 
 
-# __validation_set = set()
-# __validation_instantiation_rule = dict()
-
+# @validate
+# def NotImplemented(func: Callable) -> Callable:
+#     """decorator to mark function as not implemented for development purposes
 
-# def __validate_type(func: Callable, v: Any, T: type, validation_func: Callable[[Any], bool] = isoftype, msg: str = None) -> None:
-#     if not validation_func(v, T):
-#         raise ValidationTypeError(
-#             msg or f"In {func.__module__}.{func.__qualname__}(...)\nThe argument is: '{ v.__qualname__ if hasattr(v, '__qualname__') else v}'\nIt has the type of '{type(v)}'\nIt is marked as type(s): '{T}'")
-
-
-# def __validate_condition(func: Callable, v: Any, constraint: Callable[[Any], bool], msg: str = None) -> None:
-#     if not constraint(v):
-#         raise ValidationValueError(
-#             msg or f"In {func.__module__}.{func.__qualname__}(...)\nThe argument '{str(v)}' has failed provided constraint\nConstraint in {constraint.__module__}.{constraint.__qualname__}")
-
-
-# def __validate_arg(func: Callable, curr_arg: Any, curr_inner_arg: Any) -> None:
-#     if isoneof(curr_arg, [list, tuple]):
-#         # multiple type only:
-#         if areoneof(curr_arg, [type]):
-#             __validate_type(func, curr_inner_arg, curr_arg, isoneof)
-
-#         else:  # maybe with condition:
-#             class_type, constraint = curr_arg[0], curr_arg[1]
-
-#             # Type validation
-#             if isoneof(class_type, [list, tuple]):
-#                 __validate_type(func, curr_inner_arg, class_type, isoneof)
-#             else:
-#                 __validate_type(func, curr_inner_arg, class_type, isinstance)
-
-#             # constraints validation
-#             if constraint is not None:
-#                 message = curr_arg[2] if len(curr_arg) > 2 else None
-#                 __validate_condition(func, curr_inner_arg, constraint, message)
-#     else:
-#         __validate_type(func, curr_inner_arg, curr_arg)
-
-
-# def validate_explicit(*args, return_type=None, can_instantiate_multiple_times: bool = False) -> Callable:
-#     """validate decorator
-
-#         Is passed types of variables to perform type checking over\n
-#         The arguments must be passed in the same order\n
-
-#     for each parameter respectively you can choose one of four options:\n
-#         1. None - to skip\n
-#         2. Type - a type to check \n
-#         3. Sequence of Type to check if the type is contained in the sequence\n
-#         4. Sequence that contains three arguments:\n
-#             4.1 a Type or Sequence[Type]\n
-#             4.2 a function to call on argument\n
-#             4.3 a str to display in a ValueError iff the condition from 4.2 fails\n
-#     In addition you can use keyword 'return_type' for the returned value same as specified in 1,2,3
+#     Args:
+#         func (Callable): the function to decorate
 #     """
-#     from .Exceptions import ValidationDuplicationError, ValidationTypeError, ValidationValueError, ValidationReturnTypeError
-
-#     def deco(func: Callable) -> Callable:
-#         if not isinstance(func, Callable):
-#             raise ValueError("validate decorator must decorate a callable")
-#         global __validation_set, __validation_instantiation_rule
-#         func_id = f"{func.__module__}.{func.__qualname__}"
-
-#         if func_id not in __validation_instantiation_rule:
-#             __validation_instantiation_rule[func_id] = can_instantiate_multiple_times
-#         assert can_instantiate_multiple_times == __validation_instantiation_rule[
-#             func_id], "can't change instantiation status on runtime"
-
-#         if func_id not in __validation_set:
-#             __validation_set.add(func_id)
-#         else:
-#             if not __validation_instantiation_rule[func_id]:
-#                 raise ValidationDuplicationError(
-#                     "validate decorator is being used on two functions in the same module with the same name\nmaybe use @overload instead")
-
-#         @ functools.wraps(func)
-#         def wrapper(*inner_args, **inner_kwargs) -> Any:
-#             for i in range(min(len(args), len(inner_args))):
-#                 if args[i] is not None:
-#                     __validate_arg(func, args[i], inner_args[i])
-#             res = func(*inner_args, **inner_kwargs)
-#             if return_type is not None:
-#                 msg = f"In {func.__module__}.{func.__qualname__}(...)\nThe returned value is: '{ res.__qualname__ if hasattr(res, '__qualname__') else res}'\nIt has the type of '{type(res)}'\nIt is marked as type(s): '{return_type}'"
-#                 __validate_type(func, res, return_type, msg=msg)
-#             return res
-#         return wrapper
-#     return deco
-
-
-@validate
-def NotImplemented(func: Callable) -> Callable:
-    """decorator to mark function as not implemented for development purposes
-
-    Args:
-        func (Callable): the function to decorate
-    """
-    @ functools.wraps(func)
-    def wrapper(*args, **kwargs) -> Any:
-        raise NotImplementedError(
-            f"As marked by the developer {func.__module__}.{func.__qualname__} is not implemented yet..")
-    return wrapper
+#     @ functools.wraps(func)
+#     def wrapper(*args, **kwargs) -> Any:
+#         raise NotImplementedError(
+#             f"As marked by the developer {func.__module__}.{func.__qualname__} is not implemented yet..")
+#     return wrapper
 
 
 @validate
 def PartiallyImplemented(func: Callable) -> Callable:
     """decorator to mark function as not fully implemented for development purposes
 
     Args:
         func (Callable): the function to decorate
     """
     from .Colors import warning
 
     @ functools.wraps(func)
     def wrapper(*args, **kwargs) -> Any:
         warning(
-            f"As marked by the developer, {func.__module__}.{func.__qualname__} may not be fully implemented and might not work properly")
+            f"As marked by the developer, {func.__module__}.{func.__qualname__} "
+            "may not be fully implemented and might not work properly.")
         return func(*args, **kwargs)
     return wrapper
 
 
 @validate
 def memo(func: Callable) -> Callable:
     """decorator to memorize function calls in order to improve performance by using more memory
@@ -210,35 +127,38 @@
     def wrapper(*args, **kwargs):
         if (args, *kwargs.items()) not in cache:
             cache[(args, *kwargs.items())] = func(*args, **kwargs)
         return cache[(args, *kwargs.items())]
     return wrapper
 
 
-__overload_dict: dict[str, dict[tuple, Callable]] = dict()
+__overload_dict: dict[str, dict[tuple, Callable]] = {}
 
 
 def overload(*types) -> Callable:
     """decorator for overloading functions\n
     Usage\n-------\n
     @overload(str,str)\n
     def print_info(name,color):
         ...\n\n
     @overload(str,[int,float]))\n
     def print_info(name,age):
         ...\n\n
 
     * use None to skip argument
     * use no arguments to mark as default function
-    * you should overload in decreasing order of specificity! e.g @overload(int) should appear in the code before @overload(Any)
+    * you should overload in decreasing order of specificity! e.g 
+    @overload(int) should appear in the code before @overload(Any)
 
     \n\n\n
     \nRaises:
-        OverloadDuplication: if a functions is overloaded twice (or more) with same argument types
-        OverloadNotFound: if an overloaded function is called with types that has no variant of the function
+        OverloadDuplication: if a functions is overloaded twice (or more)
+        with same argument types
+        OverloadNotFound: if an overloaded function is called with 
+        types that has no variant of the function
 
     \nNotice:
         The function's __doc__ will hold the value of the last variant only
     """
     # make sure to use unique global dictionary
     if len(types) == 1 and type(types[0]).__name__ == "function":
         raise ValueError("can't create an overload without defining types")
@@ -256,15 +176,15 @@
         if not isinstance(func, Callable):
             raise TypeError("overload decorator must be used on a callable")
 
         # assign current overload to overload dictionary
         name = f"{func.__module__}.{func.__qualname__}"
 
         if name not in __overload_dict:
-            __overload_dict[name] = dict()
+            __overload_dict[name] = {}
 
         if types in __overload_dict[name]:
             # raise if current overload already exists for current function
             raise OverloadDuplication(
                 f"{name} has duplicate overloading for type(s): {types}")
 
         __overload_dict[name][types] = func
@@ -274,17 +194,16 @@
             default_func = None
             # select correct overload
             for variable_types, curr_func in __overload_dict[f"{func.__module__}.{func.__qualname__}"].items():
                 if len(variable_types) == 0:
                     if default_func is None:
                         default_func = curr_func
                         continue
-                    else:
-                        # will not reach here because of duplicate overloading so this is redundant
-                        raise ValueError("Can't have two default functions")
+                    # will not reach here because of duplicate overloading so this is redundant
+                    raise ValueError("Can't have two default functions")
 
                 if len(variable_types) != len(args):
                     continue
 
                 for i, variable_type in enumerate(variable_types):
                     if variable_type is not None:
                         if isoneof(variable_type, [list, tuple]):
@@ -310,24 +229,25 @@
 def abstractmethod(func: Callable) -> Callable:
     """A decorator to mark a function to be 'pure virtual' / 'abstract'
 
     Args:
         func (Callable): the function to mark
 
     Raises:
-        NotImplementedError: the error that will rise when the marked function will be called if not overridden in a derived class
+        NotImplementedError: the error that will rise when the marked function
+        will be called if not overridden in a derived class
     """
     @ functools.wraps(func)
     def wrapper(*args, **kwargs):
         raise NotImplementedError(
             f"{func.__module__}.{func.__qualname__} MUST be overridden in a child class")
     return wrapper
 
 
-# __virtualization_tables = dict()
+# __virtualization_tables = {}
 
 
 # @NotImplemented
 # def virtual(func: Callable) -> Callable:
 #     def wrapper(*args, **kwargs):
 #         return func(*args, **kwargs)
 #     return wrapper
@@ -378,14 +298,23 @@
 #             return func(*args, **kwargs)
 #         return wrapper
 #     return deco
 
 
 @validate
 def atomic(func: Callable) -> Callable:
+    """will make function thread safe by making it
+    accessible for only one thread at one time
+
+    Args:
+        func (Callable): function to make thread safe
+
+    Returns:
+        Callable: the thread safe function
+    """
     lock = threading.Lock()
 
     @ functools.wraps(func)
     def wrapper(*args, **kwargs):
         with lock:
             return func(*args, **kwargs)
     return wrapper
@@ -405,36 +334,37 @@
     from .Colors import warning
 
     def deco(func):
         @ functools.wraps(func)
         def wrapper(*args, **kwargs):
             depth = functools.reduce(
                 lambda count, line:
-                    count + 1 if re.search(f"{func.__name__}\(.*\)$", line)
+                    count + 1 if re.search(rf"{func.__name__}\(.*\)$", line)
                     else count,
                 traceback.format_stack(), 0
             )
             if depth >= max_depth:
                 if not quiet:
                     warning(
-                        f"limit_recursion has limited the number of calls for {func.__module__}.{func.__qualname__} to {max_depth}")
+                        "limit_recursion has limited the number of calls for "
+                        f"{func.__module__}.{func.__qualname__} to {max_depth}")
                 if return_value:
                     return return_value
                 return args, kwargs
             return func(*args, **kwargs)
         return wrapper
     return deco
 
 
 @validate
-def timeout(timeout: int | float) -> Callable:
+def timeout(duration: int | float) -> Callable:
     """A decorator to limit runtime for a function
 
     Args:
-        timeout (int | float): allowed runtime duration
+        duration (int | float): allowed runtime duration
 
     Raises:
         thread_error: if there is a thread related error
         function_error: if there is an error in the decorated function
 
     Returns:
         Callable: The decorated function
@@ -443,37 +373,50 @@
     def timeout_deco(func: Callable) -> Callable:
         if not isinstance(func, Callable):
             raise ValueError("timeout must decorate a function")
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             res = [
-                TimeoutError(f'{func.__module__}.{func.__qualname__} timed out after {timeout} seconds!')]
+                TimeoutError(f'{func.__module__}.{func.__qualname__} timed out after {duration} seconds!')]
 
             def timeout_wrapper() -> None:
                 try:
                     res[0] = func(*args, **kwargs)
                 except Exception as function_error:
                     res[0] = function_error
 
             t = threading.Thread(target=timeout_wrapper, daemon=True)
             try:
                 t.start()
-                t.join(timeout)
+                t.join(duration)
             except Exception as thread_error:
                 raise thread_error
             if isinstance(res[0], BaseException):
                 raise res[0]
             return res[0]
         return wrapper
     return timeout_deco
 
 
 @validate
 def attach(before: Callable = None, after: Callable = None) -> Callable:
+    """attaching functions to a function
+
+    Args:
+        before (Callable, optional): function to call before. Defaults to None.
+        after (Callable, optional): function to call after. Defaults to None.
+
+    Raises:
+        ValueError: if both before and after are none
+        ValueError: if the decorated object is not a Callable
+
+    Returns:
+        Callable: the decorated result
+    """
     if before is None and after is None:
         raise ValueError("You must supply at least one function")
 
     def attach_deco(func: Callable):
         if not isinstance(func, Callable):
             raise ValueError("attach must decorate a function")
 
@@ -487,15 +430,15 @@
             return res
         return wrapper
     return attach_deco
 
 
 __all__ = [
     "validate",
-    "NotImplemented",
+    # "NotImplemented",
     "PartiallyImplemented",
     "memo",
     "overload",
     "abstractmethod",
     # "virtual",
     # "override",
     # "deprecate",
```

### Comparing `danielutils-0.8.3/danielutils/IO.py` & `danielutils-0.8.5/danielutils/IO.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,14 @@
 # -*- coding: utf-8 -*-
-from typing import IO
+import subprocess
+from typing import IO, Iterator, Generator
 import shutil
+from pathlib import Path
 import os
 from .Decorators import validate
-from typing import Union
-from pathlib import Path
-
-
-@validate
-def write_to_file(path: str, lines: Union[list[str], list[bytes]], write_bytes: bool = False) -> None:
-    """clear and then write data to file
-
-    Args:
-        path (str): path of file
-        lines (list[str]): data to write
-    """
-
-    try:
-        if write_bytes:
-            with open(path, "wb") as f:
-                f.writelines(lines)
-        else:
-            with open(path, "w", encoding="utf-8") as f:
-                f.writelines(lines)
-    except Exception as e:
-        if isinstance(e, TypeError):
-            raise Exception(
-                "'lines' contains a 'bytes' object.\nTo use with bytes use: write_bytes = True ")
-        raise e
 
 
 @validate
 def path_exists(path: str) -> bool:
     """checks whether a path exists
 
     Args:
@@ -95,16 +72,16 @@
             with open(path, "rb") as f:
                 return f.readlines()
         else:
             with open(path, "r", encoding="mbcs") as f:
                 return f.readlines()
     except Exception as e:
         if isinstance(e, UnicodeDecodeError):
-            raise Exception(
-                f"Can't read byte in file.\nTo use with bytes use: read_bytes = True ")
+            raise UnicodeDecodeError(
+                "Can't read byte in file.\nTo use with bytes use: read_bytes = True ") from e
         raise e
 
 
 @validate
 def is_file(path: str) -> bool:
     """return whether a path represents a file
 
@@ -177,109 +154,194 @@
     if is_directory(path):
         clear_directory(path)
         os.rmdir(path)
 
 
 @validate
 def clear_directory(path: str) -> None:
+    """clears the content of a directory
+
+    Args:
+        path (str): the path of the directory to clean
+    """
     for file in get_files(path):
         delete_file(f"{path}\\{file}")
-    for dir in get_directories(path):
-        delete_directory(f"{path}\\{dir}")
+    for subdir in get_directories(path):
+        delete_directory(f"{path}\\{subdir}")
 
 
 @validate
 def create_directory(path: str) -> None:
     """create a directory at the specified path if it doesn't already exists
 
     Args:
         path (str): the path to create a directory at
     """
     if not directory_exists(path):
         os.makedirs(path)
 
 
 @validate
-def get_file_type_from_directory(path: str, file_type: str) -> list[str]:
-    return list(
-        filter(
-            lambda name: Path(f"{path}\\{name}").suffix == file_type,
-            get_files(path)
-        )
+def get_file_type_from_directory(path: str, file_type: str) -> Iterator[str]:
+    """returns all file with specific type from a directory
+
+    Args:
+        path (str): path of directory
+        file_type (str): the desired file type. eg: ".png"
+
+    Returns:
+        list[str]: result
+    """
+    return filter(
+        lambda name: Path(f"{path}\\{name}").suffix == file_type,
+        get_files(path)
     )
 
 
 @validate
-def get_file_type_from_directory_recursively(path: str, file_type: str):
-    res = []
-    for dir in get_directories(path):
-        res.extend(f"{dir}\\{v}" for v in get_file_type_from_directory_recursively(
-            f"{path}\\{dir}", file_type))
-    res.extend(list(
-        filter(
-            lambda name: Path(f"{path}\\{name}").suffix == file_type,
-            get_files(path)
-        )
-    ))
-    return res
+def get_file_type_from_directory_recursively(path: str, file_type: str) -> Generator[str, None, None]:
+    """_summary_
+
+    Args:
+        path (str): _description_
+        file_type (str): _description_
+
+    Returns:
+        _type_: _description_
+    """
+    yield from filter(
+        lambda name: Path(f"{path}\\{name}").suffix == file_type,
+        get_files(path)
+    )
+    for subdir in get_directories(path):
+        for v in get_file_type_from_directory_recursively(f"{path}\\{subdir}", file_type):
+            yield f"{subdir}\\{v}"
 
 
 def rename_file(path: str, new_name: str) -> None:
+    """renames a file
+
+    Args:
+        path (str): file to rename
+        new_name (str): the desired new name
+    """
     new_path = "./" + \
         "/".join(Path(path).parts[:-1])+"/"+new_name+Path(path).suffix
     move_file(path, new_path)
 
 
 def move_file(old_path: str, new_path: str) -> None:
+    """moves a file
+
+    Args:
+        old_path (str): old path
+        new_path (str): new path
+    """
     os.rename(old_path, new_path)
 
 
-async def open_file(file_path: str, application_path: str):
-    import subprocess
-    p = subprocess.Popen([application_path, file_path])
-    return_code = p.wait()
+async def open_file(file_path: str, application_path: str) -> int:
+    """open a file with the specified application
+
+    Args:
+        file_path (str): the file to open
+        application_path (str): the application to open with
+    Returns:
+        int: return code
+    """
+    with subprocess.Popen([application_path, file_path]) as p:
+        return p.wait()
 
 
 def move_directory(old_path: str, new_path: str) -> None:
+    """moves a directory
+
+    Args:
+        old_path (str): old path
+        new_path (str): new path
+    """
     shutil.move(old_path, new_path)
 
 
 def copy_file(src: str, dest: str) -> None:
+    """copies file from src to dest
+
+    Args:
+        src (str): src
+        dest (str): dest
+    """
     shutil.copy(src, dest)
 
 
 def copy_directory(src: str, dest: str) -> None:
+    """copies a directory from src to dest
+
+    Args:
+        src (str): stc
+        dest (str): dest
+    """
     shutil.copy(src, dest)
 
 
 class IndentedWriter:
-    def __init__(self, output_stream: IO = None, indent_char: str = "\t"):
+    """every class that will inherit this class will have the following functions available
+        write() with the same arguments a builtin print()
+        indent()
+        undent()
+
+        also, it is expected in the __init__ function to call super().__init__()
+        also, the output_stream must be set whether by the first argument io super().__init__(...)
+        or by set_stream() explicitly somewhere else.
+
+        this class will not function properly is the output_stream is not set!
+
+    """
+
+    def __init__(self, output_stream: IO = None, indent_value: str = "\t"):
         self.indent_level = 0
         self.output_stream: IO = output_stream
-        self.indent_char = indent_char
+        self.indent_value = indent_value
 
     def write(self, *args, sep=" ", end="\n"):
+        """writes the supplied arguments to the output_stream
+
+        Args:
+            sep (str, optional): the str to use as a separator between arguments. Defaults to " ".
+            end (str, optional): the str to use as the final value. Defaults to "\n".
+
+        Raises:
+            ValueError: _description_
+        """
         if self.output_stream is None:
             raise ValueError(
                 "Can't write to an empty stream. the stream must not be None either by set_stream or by initialization")
         self.output_stream.write(
-            self.indent_level*self.indent_char + sep.join(args)+end)
+            self.indent_level*self.indent_value + sep.join(args)+end)
+
+    def set_stream(self, stream: IO):
+        """explicitly sets the stream
 
-    def set_stream(self, stream):
+        Args:
+            stream (IO): stream
+        """
         self.output_stream = stream
 
-    def indent(self):
+    def indent(self) -> None:
+        """indents the preceding output with write() by one quantity more
+        """
         self.indent_level += 1
 
-    def undent(self):
+    def undent(self) -> None:
+        """un-dents the preceding output with write() by one quantity less
+            has a minimum value of 0
+        """
         self.indent_level = max(0, self.indent_level-1)
 
 
 __all__ = [
-    "write_to_file",
     "path_exists",
     "file_exists",
     "directory_exists",
     "delete_file",
     "read_file",
     "is_file",
     "is_directory",
```

### Comparing `danielutils-0.8.3/danielutils/Math/MathPrint.py` & `danielutils-0.8.5/danielutils/Math/MathPrint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,30 @@
-import sys
 from .MathSymbols import subscript_dict, superscript_dict
 
 
 def mprint_parse_one(s: str) -> str:
+    """a helper function that parses "mathematically" one string
+
+    Args:
+        s (str): the string to parse with math symbols
+
+    Returns:
+        str: the result
+    """
 
     def inner(res, index, dct):
         start = index
         while index < len(s) and s[index] not in {' ', '*', '+', '-', '/', '_', '^'}:
             index += 1
         end = index
-        for c in s[start:end]:
-            if c in dct:
-                res += dct[c]
+        for char in s[start:end]:
+            if char in dct:
+                res += dct[char]
             else:
-                res += c
+                res += char
         index -= 1
         return res, index
     res: str = ""
     i = 0
     while i < len(s):
         c = s[i]
         if c == "^":
```

### Comparing `danielutils-0.8.3/danielutils/Path.py` & `danielutils-0.8.5/danielutils/Path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.3/danielutils/Print.py` & `danielutils-0.8.5/danielutils/Print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.3/danielutils/System.py` & `danielutils-0.8.5/danielutils/System.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from typing import Generator
-import os
-from math import inf
-from .Decorators import overload, timeout, validate
-from .Typing import IO
-from .Exceptions import TimeoutError
-from .Conversions import str_to_bytes
-from .Functions import areoneof
+from typing import IO
 from pathlib import Path
 import subprocess
 import time
+from .Decorators import timeout, validate
+from .Conversions import str_to_bytes
 
 
 def cm(*args, shell: bool = True) -> tuple[int, bytes, bytes]:
     """Execute windows shell command and return output
 
     Args:
         command or args:\n
@@ -28,15 +24,16 @@
     """
     if not isinstance(shell, bool):
         raise TypeError(
             "In function 'cm' param 'shell' must be of type bool")
     for i, arg in enumerate(args):
         if Path(args[i]).is_file() or Path(args[i]).is_dir():
             args = (*args[:i], f"\"{arg}\"", *args[i+1:])
-    res = subprocess.run(" ".join(args), shell=shell, capture_output=True)
+    res = subprocess.run(" ".join(args), shell=shell,
+                         capture_output=True, check=False)
     return res.returncode, res.stdout, res.stderr
 
 
 @validate
 def sleep(seconds: int | float) -> None:
     """make current thread sleep
 
@@ -53,38 +50,42 @@
     b_args = str_to_bytes(sep).join(str_to_bytes(v) for v in args)
     b_end = str_to_bytes(end)
     p.stdin.write(b_args+b_end)
     p.stdin.flush()
 
 
 @validate
-def acm(command: str, inputs: list[str] = None, i_timeout: float = 0.01, shell: bool = False, use_write_helper: bool = True, cwd: str = None, env: str = None) -> tuple[int, list[bytes] | None, list[bytes] | None]:
+def acm(command: str, inputs: list[str] = None, i_timeout: float = 0.01,
+        shell: bool = False, use_write_helper: bool = True, cwd: str = None,
+        env: str = None) -> tuple[int, list[bytes] | None, list[bytes] | None]:
     """Advanced command
 
     Args:
         command (str): The command to execute\n
         inputs (list[str]): the inputs to give to the program from the command. Defaults to None.\n
         i_timeout (float, optional): An individual timeout for every step of the execution. Defaults to 0.01.\n
         cwd (?, optional): Current working directory. Defaults to None.\n
         env (?, optional): Environment variables. Defaults to None.\n
         shell (bool, optional): whether to execute the command through shell. Defaults to False.\n
-        use_write_helper (bool, optional): whether to parse each input as it would have been parse with builtin print() or to use raw text. Defaults to True.
+        use_write_helper (bool, optional): whether to parse each input as it
+        would have been parse with builtin print() or to use raw text. Defaults to True.
 
     Raises:
         If @timeout will raise something other than TimeoutError.\n
         If the subprocess input and output handling will raise an exception.
 
     Returns:
         tuple[int, list[bytes] | None, list[bytes] | None]: return code, stdout, stderr
     """
 
     if inputs is None:
         inputs = []
     p = None
     try:
+        # TODO with ... as p:
         p = subprocess.Popen(command, stdout=subprocess.PIPE,
                              stdin=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=cwd, env=env, shell=shell)
 
         @timeout(i_timeout)
         def readlines(s: IO, l: list):
             l.extend(s.readlines())
 
@@ -97,25 +98,25 @@
                     # break
                     pass
                 except BaseException as e1:
                     raise e1
 
         stdout: list[bytes] = []
         stderr: list[bytes] = []
-        for input in inputs:
+        for curr_input in inputs:
             if p.stdin.writable():
                 if use_write_helper:
-                    __acm_write(input, p=p)
+                    __acm_write(curr_input, p=p)
                 else:
-                    __acm_write(input, p=p, sep="", end="")
-            extend_from_stream(p.stdout, stdout)
-            extend_from_stream(p.stderr, stderr)
-        else:
+                    __acm_write(curr_input, p=p, sep="", end="")
             extend_from_stream(p.stdout, stdout)
             extend_from_stream(p.stderr, stderr)
+        # else:
+        #     extend_from_stream(p.stdout, stdout)
+        #     extend_from_stream(p.stderr, stderr)
         p.stdin.close()
         p.stdout.close()
         if p.stderr is not None:
             p.stderr.close()
         returncode = p.wait()
         return returncode, stdout, stderr
     except BaseException as e2:
@@ -149,21 +150,20 @@
     # Quote the arguments that represent file or directory paths.
     for i, arg in enumerate(args):
         if Path(args[i]).is_file() or Path(args[i]).is_dir():
             args = (*args[:i], f"\"{arg}\"", *args[i+1:])
 
     # Join the arguments into a command string and execute the command.
     cmd = " ".join(args)
-    process = subprocess.Popen(
-        cmd, shell=shell, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-
-    # Yield stdout and stderr in real-time.
-    while process.poll() is None:
-        yield from process.stderr
-        yield from process.stdout
+    with subprocess.Popen(
+            cmd, shell=shell, stdout=subprocess.PIPE, stderr=subprocess.PIPE) as process:
+        # Yield stdout and stderr in real-time.
+        while process.poll() is None:
+            yield from process.stderr
+            yield from process.stdout
 
 
 __all__ = [
     "cm",
     "acm",
     "sleep",
     "cmrt"
```

### Comparing `danielutils-0.8.3/danielutils/Text.py` & `danielutils-0.8.5/danielutils/Text.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,161 @@
 # -*- coding: utf-8 -*-
+from typing import Union, TypeGuard
 from .Decorators import validate
 from .Functions import check_foreach
-from .Typing import Union, TypeGuard
-HEBREW_LETTERS = ['\u05D0', '\u2135', '\uFB21', '\uFB2E', '\uFB2F', '\uFB30', '\uFB4F', '\u05D1', '\u2136', '\uFB31', '\uFB4C', '\u05D2', '\u2137', '\uFB32', '\u05D3', '\u2138', '\uFB22', '\uFB33', '\u05D4', '\uFB23', '\uFB34', '\u05D5', '\uFB4B', '\uFB35', '\u05F0', '\u05F1', '\u05D6', '\uFB36', '\u05D7', '\u05D8', '\uFB38', '\u05D9', '\uFB1D', '\uFB39', '\u05EF', '\u05F2', '\uFB1F', '\u05DB', '\uFB24',
-                  '\u05DA', '\uFB3B', '\uFB3A', '\uFB4D', '\u05DC', '\uFB25', '\uFB3C', '\u05DE', '\uFB26', '\u05DD', '\uFB3E', '\u05E0', '\u05DF', '\uFB40', '\u05E1', '\uFB41', '\u05E2', '\uFB20', '\u05E4', '\u05E3', '\uFB44', '\uFB43', '\uFB4E', '\u05E6', '\u05E5', '\uFB46', '\u05E7', '\uFB47', '\u05E8', '\uFB27', '\uFB48', '\u05E9', '\uFB2B', '\uFB2A', '\uFB49', '\uFB2D', '\uFB2C', '\u05EA', '\uFB28', '\uFB4A']
+HEBREW_LETTERS = ['\u05D0', '\u2135', '\uFB21', '\uFB2E', '\uFB2F',
+                  '\uFB30', '\uFB4F', '\u05D1', '\u2136', '\uFB31',
+                  '\uFB4C', '\u05D2', '\u2137', '\uFB32', '\u05D3',
+                  '\u2138', '\uFB22', '\uFB33', '\u05D4', '\uFB23',
+                  '\uFB34', '\u05D5', '\uFB4B', '\uFB35', '\u05F0',
+                  '\u05F1', '\u05D6', '\uFB36', '\u05D7', '\u05D8',
+                  '\uFB38', '\u05D9', '\uFB1D', '\uFB39', '\u05EF',
+                  '\u05F2', '\uFB1F', '\u05DB', '\uFB24', '\u05DA',
+                  '\uFB3B', '\uFB3A', '\uFB4D', '\u05DC', '\uFB25',
+                  '\uFB3C', '\u05DE', '\uFB26', '\u05DD', '\uFB3E',
+                  '\u05E0', '\u05DF', '\uFB40', '\u05E1', '\uFB41',
+                  '\u05E2', '\uFB20', '\u05E4', '\u05E3', '\uFB44',
+                  '\uFB43', '\uFB4E', '\u05E6', '\u05E5', '\uFB46',
+                  '\u05E7', '\uFB47', '\u05E8', '\uFB27', '\uFB48',
+                  '\u05E9', '\uFB2B', '\uFB2A', '\uFB49', '\uFB2D',
+                  '\uFB2C', '\u05EA', '\uFB28', '\uFB4A']
+
+
 HEBREW_LETTERS_DEC = [ord(v) for v in HEBREW_LETTERS]
 HEBREW_LETTERS_HEX = [hex(v) for v in HEBREW_LETTERS_DEC]
 ENGLISH_LETTERS = [chr(v) for v in range(65, 91)]+[chr(v)
                                                    for v in range(97, 123)]
 ENGLISH_LETTERS_DEC = [ord(v) for v in ENGLISH_LETTERS]
 ENGLISH_LETTERS_HEX = [hex(v) for v in ENGLISH_LETTERS_DEC]
 
 
 @validate
 def is_english(s: str) -> TypeGuard[str]:
+    """returns whether the specified string is in the english language
+
+    Args:
+        s (str): the string to check
+
+    Returns:
+        TypeGuard[str]: returns true if the string is in english
+    """
     return check_foreach(s, lambda c: c in ENGLISH_LETTERS)
-    # try:
-    #     s.encode(encoding='utf-8').decode('ascii')
-    # except UnicodeDecodeError:
-    #     return False
-    # else:
-    #     return True
 
 
 @validate
-def is_str_number(text: str) -> bool:
-    return text.isnumeric()
+def is_number(s: str) -> TypeGuard[int | float]:
+    """checks if a string is a number
+
+    Args:
+        text (str): string to check
+
+    Returns:
+        TypeGuard[int | float]: true if string is a number
+    """
+    return s.isnumeric()
 
 
 @validate
 def is_int(num: Union[int, float]) -> TypeGuard[int]:
+    """_summary_
+
+    Args:
+        num (Union[int, float]): is a number an int
+
+    Returns:
+        TypeGuard[int]: return true if num is a while number
+    """
     if isinstance(num, int):
         return True
 
     return int(num) == num
 
 
 @validate
-def is_float(text: str) -> TypeGuard[float]:
+def is_float(s: str) -> TypeGuard[float]:
+    """checks whether a string has a float value
+
+    Args:
+        s (str): string to check
+
+    Returns:
+        TypeGuard[float]: result
+    """
     try:
-        float(text)
+        float(s)
         return True
     except ValueError:
         return False
 
 
 @validate
-def is_number(text: str) -> bool:
-    return is_float(text)
+def is_hebrew(s: str) -> TypeGuard[str]:
+    """checks if a string is in hebrew
 
+    Args:
+        text (str): string to check
 
-@validate
-def is_hebrew(text: str) -> TypeGuard[str]:
-    return check_foreach(text, lambda c: c in HEBREW_LETTERS)
+    Returns:
+        TypeGuard[str]: true iff all chars are in hebrew
+    """
+    return check_foreach(s, lambda c: c in HEBREW_LETTERS)
 
 
 @validate
-def is_binary(text: str) -> bool:
-    return check_foreach(text, lambda c: c in [0, 1])
+def is_binary(s: str) -> bool:
+    """checks if s string has a binary value
+
+    Args:
+        s (str): string to check
+
+    Returns:
+        bool: result
+    """
+    return check_foreach(s, lambda c: c in {0, 1})
 
 
 @validate
-def is_decimal(text: str) -> bool:
-    return check_foreach(text, lambda c: c in range(10))
+def is_decimal(s: str) -> bool:
+    """checks if a string has a decimal number
+
+    Args:
+        s (str): string to check
+
+    Returns:
+        bool: result
+    """
+    return check_foreach(s, lambda c: c in range(10))
 
 
 @validate
-def is_hex(h: str) -> bool:
+def is_hex(s: str) -> bool:
+    """checks if a string has a hexadecimal value
+
+    Args:
+        s (str): string to check
+
+    Returns:
+        bool: result
+    """
     try:
-        int(h, 16)
+        int(s, 16)
         return True
     except ValueError:
         return False
 
 
 __all__ = [
     "HEBREW_LETTERS",
     "HEBREW_LETTERS_DEC",
     "HEBREW_LETTERS_HEX",
     "ENGLISH_LETTERS",
     "ENGLISH_LETTERS_DEC",
     "ENGLISH_LETTERS_HEX",
     "is_english",
-    "is_str_number",
+    "is_number",
     "is_int",
     "is_float",
-    "is_number",
     "is_hebrew",
     "is_binary",
     "is_decimal",
     "is_hex"
 ]
```

### Comparing `danielutils-0.8.3/danielutils/Windows.py` & `danielutils-0.8.5/danielutils/Windows.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,66 @@
+from functools import partial
 from screeninfo import get_monitors
 import pyautogui
 from PIL import ImageGrab, Image
-import PIL
-from functools import partial
 ImageGrab.grab = partial(ImageGrab.grab, all_screens=True)
 
 
 def screenshot(xy: tuple[int, int] = (0, 0), wh: tuple[int, int] = None) -> Image:
+    """creates a screenshot of the screen in an arbitrary location and size
+
+    Args:
+        xy (tuple[int, int], optional): the top left location of the screenshot. Defaults to (0, 0).
+        wh (tuple[int, int], optional): the size of the screenshot in pixels. Defaults to None. if None will 
+        create a screen shot of all monitors
+    Returns:
+        Image: _description_
+    """
     if wh is None:
         wh = (0, 0)
         for monitor_index in range(get_monitor_count()):
             size = get_monitor_size(monitor_index)
             wh = (wh[0]+size[0], wh[1]+size[1])
     return pyautogui.screenshot(None, (xy[0], xy[1], wh[0], wh[1]))
 
 
 def screenshot_monitor(index: int) -> Image:
+    """creates a screenshot of the monitor
+
+    Args:
+        index (int): the monitor's index
+
+    Returns:
+        Image: the screenshot
+    """
     return screenshot(get_monitor_location(index), get_monitor_size(index))
 
 
 def get_monitor_size(index: int) -> tuple[int, int]:
+    """returns the size of the monitor
+
+    Args:
+        index (int): the monitor's index
+
+    Returns:
+        tuple[int, int]: the size
+    """
     monitor = get_monitors()[index]
     return monitor.width, monitor.height
 
 
-def get_monitor_location(index) -> tuple[int, int]:
+def get_monitor_location(index: int) -> tuple[int, int]:
+    """returns the coordinates of the location of the monitor
+
+    Args:
+        index (int): the monitor's index
+
+    Returns:
+        tuple[int, int]: the coordinates
+    """
     monitor = get_monitors()[index]
     return monitor.x, monitor.y
 
 
 def get_monitor_count() -> int:
     """return the number of displays connected to this computer
```

### Comparing `danielutils-0.8.3/danielutils.egg-info/PKG-INFO` & `danielutils-0.8.5/danielutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.8.3
+Version: 0.8.5
 Summary: A python utils library for things I find useful
 Home-page: https://github.com/danielnachumdev/danielutils
 Author: danielnachumdev
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/danielnachumdev/danielutils
 Project-URL: Bug Tracker, https://github.com/danielnachumdev/danielutils/issues
@@ -12,12 +12,12 @@
 Platform: All
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.10.5
 Description-Content-Type: text/markdown
 
-# danielutils v=0.8.3
+# danielutils v=0.8.5
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
```

### Comparing `danielutils-0.8.3/danielutils.egg-info/SOURCES.txt` & `danielutils-0.8.5/danielutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,46 +3,39 @@
 setup.py
 danielutils/Colors.py
 danielutils/Data.py
 danielutils/Decorators.py
 danielutils/Exceptions.py
 danielutils/Functions.py
 danielutils/IO.py
-danielutils/Internet.py
 danielutils/Path.py
 danielutils/Print.py
-danielutils/Serialization.py
 danielutils/System.py
-danielutils/Testing.py
 danielutils/Text.py
 danielutils/Threading.py
 danielutils/Time.py
-danielutils/Typing.py
 danielutils/Windows.py
 danielutils/__init__.py
 danielutils.egg-info/PKG-INFO
 danielutils.egg-info/SOURCES.txt
 danielutils.egg-info/dependency_links.txt
 danielutils.egg-info/requires.txt
 danielutils.egg-info/top_level.txt
 danielutils/Classes/Convenience.py
-danielutils/Classes/DataStructures.py
 danielutils/Classes/TypedBuiltins.py
 danielutils/Classes/__init__.py
 danielutils/Classes/frange.py
 danielutils/Conversions/MainConversions.py
 danielutils/Conversions/__init__.py
 danielutils/Conversions/SpecializedConversions/__init__.py
 danielutils/Conversions/SpecializedConversions/to_hex.py
 danielutils/Conversions/SpecializedConversions/to_int.py
 danielutils/DataStructures/Comparer.py
-danielutils/DataStructures/Graph.py
 danielutils/DataStructures/Heap.py
 danielutils/DataStructures/Interface.py
-danielutils/DataStructures/MarkovChain.py
 danielutils/DataStructures/Node.py
 danielutils/DataStructures/Queue.py
 danielutils/DataStructures/__init__.py
 danielutils/DataStructures/functions.py
 danielutils/Math/Constants.py
 danielutils/Math/Functions.py
 danielutils/Math/MathPrint.py
```

### Comparing `danielutils-0.8.3/pyproject.toml` & `danielutils-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "danielutils"
-version = "0.8.3"
+version = "0.8.5"
 authors = [
   { name="danielnachumdev", email="danielnachumdev@gmail.com" },
 ]
 description = "A python utils library for things I find useful"
 readme = "README.md"
 requires-python = ">=3.10.5"
 classifiers = [
```

### Comparing `danielutils-0.8.3/setup.py` & `danielutils-0.8.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def read_file(path: str) -> "list[str]":
     with codecs.open(path, 'r', 'utf-8') as f:
         return [l.strip() for l in f.readlines()]
 
 
 README_PATH = 'README.md'
 DESCRIPTION = 'A python utils library for things I find useful'
-VERSION = "0.8.3"
+VERSION = "0.8.5"
 LONG_DESCRIPTION = '\n'.join(read_file(README_PATH))
 setup(
     name="danielutils",
     version=VERSION,
     author="danielnachumdev",
     author_email="<danielnachumdev@gmail.com>",
     description=DESCRIPTION,
```

