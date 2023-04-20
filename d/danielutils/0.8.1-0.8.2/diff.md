# Comparing `tmp/danielutils-0.8.1.tar.gz` & `tmp/danielutils-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.8.1.tar", last modified: Sun Apr 16 09:32:56 2023, max compression
+gzip compressed data, was "danielutils-0.8.2.tar", last modified: Thu Apr 20 14:02:09 2023, max compression
```

## Comparing `danielutils-0.8.1.tar` & `danielutils-0.8.2.tar`

### file list

```diff
@@ -1,54 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.416437 danielutils-0.8.1/
--rw-rw-rw-   0        0        0      939 2023-04-16 09:32:56.416437 danielutils-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-16 09:32:55.000000 danielutils-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.385174 danielutils-0.8.1/danielutils/
-drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.400813 danielutils-0.8.1/danielutils/Classes/
--rw-rw-rw-   0        0        0      103 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Classes/Convenience.py
--rw-rw-rw-   0        0        0     1694 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Classes/DataStructures.py
--rw-rw-rw-   0        0        0     3489 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Classes/TypedBuiltins.py
--rw-rw-rw-   0        0        0      117 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Classes/__init__.py
--rw-rw-rw-   0        0        0      904 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Classes/frange.py
--rw-rw-rw-   0        0        0     1968 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Colors.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.400813 danielutils-0.8.1/danielutils/Conversions/
--rw-rw-rw-   0        0        0     1797 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Conversions/MainConversions.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.400813 danielutils-0.8.1/danielutils/Conversions/SpecializedConversions/
--rw-rw-rw-   0        0        0       46 2022-10-25 07:33:55.000000 danielutils-0.8.1/danielutils/Conversions/SpecializedConversions/__init__.py
--rw-rw-rw-   0        0        0      454 2022-10-25 07:33:55.000000 danielutils-0.8.1/danielutils/Conversions/SpecializedConversions/to_hex.py
--rw-rw-rw-   0        0        0      389 2022-10-31 15:04:29.000000 danielutils-0.8.1/danielutils/Conversions/SpecializedConversions/to_int.py
--rw-rw-rw-   0        0        0       71 2022-10-25 07:33:55.000000 danielutils-0.8.1/danielutils/Conversions/__init__.py
--rw-rw-rw-   0        0        0      270 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Data.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.416437 danielutils-0.8.1/danielutils/DataStructures/
--rw-rw-rw-   0        0        0     2503 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/DataStructures/Graph.py
--rw-rw-rw-   0        0        0     2564 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/DataStructures/MarkovChain.py
--rw-rw-rw-   0        0        0       50 2022-10-26 11:35:28.000000 danielutils-0.8.1/danielutils/DataStructures/__init__.py
--rw-rw-rw-   0        0        0    19824 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Decorators.py
--rw-rw-rw-   0        0        0     1122 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Exceptions.py
--rw-rw-rw-   0        0        0     8193 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Functions.py
--rw-rw-rw-   0        0        0     7503 2023-04-16 09:29:30.000000 danielutils-0.8.1/danielutils/IO.py
--rw-rw-rw-   0        0        0     1259 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Internet.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.416437 danielutils-0.8.1/danielutils/Math/
--rw-rw-rw-   0        0        0     6036 2022-10-31 15:04:29.000000 danielutils-0.8.1/danielutils/Math/Constants.py
--rw-rw-rw-   0        0        0      205 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Math/Functions.py
--rw-rw-rw-   0        0        0      860 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Math/MathPrint.py
--rw-rw-rw-   0        0        0     6485 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Math/MathSymbols.py
--rw-rw-rw-   0        0        0       80 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Math/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-01-19 11:44:27.000000 danielutils-0.8.1/danielutils/Path.py
--rw-rw-rw-   0        0        0     2686 2023-04-11 14:28:24.000000 danielutils-0.8.1/danielutils/Print.py
--rw-rw-rw-   0        0        0     1357 2023-01-11 17:24:17.000000 danielutils-0.8.1/danielutils/Serialization.py
--rw-rw-rw-   0        0        0     4801 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/System.py
--rw-rw-rw-   0        0        0     6699 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Testing.py
--rw-rw-rw-   0        0        0     2895 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Text.py
--rw-rw-rw-   0        0        0      137 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Threading.py
--rw-rw-rw-   0        0        0      426 2023-04-16 08:31:50.000000 danielutils-0.8.1/danielutils/Time.py
--rw-rw-rw-   0        0        0      649 2023-01-19 11:44:27.000000 danielutils-0.8.1/danielutils/Typing.py
--rw-rw-rw-   0        0        0     1248 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/Windows.py
--rw-rw-rw-   0        0        0      480 2023-04-11 14:27:34.000000 danielutils-0.8.1/danielutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:32:56.400813 danielutils-0.8.1/danielutils.egg-info/
--rw-rw-rw-   0        0        0      939 2023-04-16 09:32:56.000000 danielutils-0.8.1/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1309 2023-04-16 09:32:56.000000 danielutils-0.8.1/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 09:32:56.000000 danielutils-0.8.1/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-16 09:32:56.000000 danielutils-0.8.1/danielutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-16 09:32:56.000000 danielutils-0.8.1/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      728 2023-04-16 09:32:55.000000 danielutils-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 09:32:56.416437 danielutils-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-04-16 09:32:55.000000 danielutils-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:02:09.348070 danielutils-0.8.2/
+-rw-rw-rw-   0        0        0      939 2023-04-20 14:02:09.348070 danielutils-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-04-20 14:02:08.000000 danielutils-0.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 14:02:09.317871 danielutils-0.8.2/danielutils/
+drwxrwxrwx   0        0        0        0 2023-04-20 14:02:09.334861 danielutils-0.8.2/danielutils/Classes/
+-rw-rw-rw-   0        0        0      103 2023-04-02 21:16:20.000000 danielutils-0.8.2/danielutils/Classes/Convenience.py
+-rw-rw-rw-   0        0        0     1694 2023-04-02 21:17:25.000000 danielutils-0.8.2/danielutils/Classes/DataStructures.py
+-rw-rw-rw-   0        0        0     3489 2023-04-11 21:22:44.000000 danielutils-0.8.2/danielutils/Classes/TypedBuiltins.py
+-rw-rw-rw-   0        0        0      117 2023-03-30 21:30:39.000000 danielutils-0.8.2/danielutils/Classes/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-03-30 21:22:39.000000 danielutils-0.8.2/danielutils/Classes/frange.py
+-rw-rw-rw-   0        0        0     1968 2023-04-11 20:58:21.000000 danielutils-0.8.2/danielutils/Colors.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:02:09.336758 danielutils-0.8.2/danielutils/Conversions/
+-rw-rw-rw-   0        0        0     1797 2023-04-11 21:02:02.000000 danielutils-0.8.2/danielutils/Conversions/MainConversions.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:02:09.338904 danielutils-0.8.2/danielutils/Conversions/SpecializedConversions/
+-rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.8.2/danielutils/Conversions/SpecializedConversions/__init__.py
+-rw-rw-rw-   0        0        0      454 2022-10-14 16:32:03.000000 danielutils-0.8.2/danielutils/Conversions/SpecializedConversions/to_hex.py
+-rw-rw-rw-   0        0        0      389 2022-10-28 08:08:26.000000 danielutils-0.8.2/danielutils/Conversions/SpecializedConversions/to_int.py
+-rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.8.2/danielutils/Conversions/__init__.py
+-rw-rw-rw-   0        0        0      270 2023-04-11 20:59:09.000000 danielutils-0.8.2/danielutils/Data.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:02:09.344171 danielutils-0.8.2/danielutils/DataStructures/
+-rw-rw-rw-   0        0        0      781 2023-04-19 18:35:04.000000 danielutils-0.8.2/danielutils/DataStructures/Comparer.py
+-rw-rw-rw-   0        0        0     2503 2023-04-11 21:02:02.000000 danielutils-0.8.2/danielutils/DataStructures/Graph.py
+-rw-rw-rw-   0        0        0     2558 2023-04-18 23:54:19.000000 danielutils-0.8.2/danielutils/DataStructures/Heap.py
+-rw-rw-rw-   0        0        0     7170 2023-04-20 13:56:43.000000 danielutils-0.8.2/danielutils/DataStructures/Interface.py
+-rw-rw-rw-   0        0        0     2564 2023-04-11 21:26:28.000000 danielutils-0.8.2/danielutils/DataStructures/MarkovChain.py
+-rw-rw-rw-   0        0        0      309 2023-04-19 18:35:04.000000 danielutils-0.8.2/danielutils/DataStructures/Node.py
+-rw-rw-rw-   0        0        0     1417 2023-04-19 18:35:04.000000 danielutils-0.8.2/danielutils/DataStructures/Queue.py
+-rw-rw-rw-   0        0        0      165 2023-04-19 18:35:04.000000 danielutils-0.8.2/danielutils/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-04-18 23:56:59.000000 danielutils-0.8.2/danielutils/DataStructures/functions.py
+-rw-rw-rw-   0        0        0    19818 2023-04-20 13:12:08.000000 danielutils-0.8.2/danielutils/Decorators.py
+-rw-rw-rw-   0        0        0     1122 2023-04-03 14:02:27.000000 danielutils-0.8.2/danielutils/Exceptions.py
+-rw-rw-rw-   0        0        0     8193 2023-04-03 11:53:26.000000 danielutils-0.8.2/danielutils/Functions.py
+-rw-rw-rw-   0        0        0     7503 2023-04-18 20:35:49.000000 danielutils-0.8.2/danielutils/IO.py
+-rw-rw-rw-   0        0        0     1259 2023-04-11 21:00:13.000000 danielutils-0.8.2/danielutils/Internet.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:02:09.347045 danielutils-0.8.2/danielutils/Math/
+-rw-rw-rw-   0        0        0     6036 2022-10-28 20:26:06.000000 danielutils-0.8.2/danielutils/Math/Constants.py
+-rw-rw-rw-   0        0        0      205 2023-04-11 21:02:02.000000 danielutils-0.8.2/danielutils/Math/Functions.py
+-rw-rw-rw-   0        0        0      860 2023-04-03 18:56:27.000000 danielutils-0.8.2/danielutils/Math/MathPrint.py
+-rw-rw-rw-   0        0        0     6485 2023-04-02 21:11:12.000000 danielutils-0.8.2/danielutils/Math/MathSymbols.py
+-rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.8.2/danielutils/Math/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-01-12 01:01:37.000000 danielutils-0.8.2/danielutils/Path.py
+-rw-rw-rw-   0        0        0     2686 2023-04-11 13:05:54.000000 danielutils-0.8.2/danielutils/Print.py
+-rw-rw-rw-   0        0        0     1357 2023-01-05 22:01:09.000000 danielutils-0.8.2/danielutils/Serialization.py
+-rw-rw-rw-   0        0        0     6061 2023-04-17 13:50:25.000000 danielutils-0.8.2/danielutils/System.py
+-rw-rw-rw-   0        0        0     6699 2023-04-11 21:23:44.000000 danielutils-0.8.2/danielutils/Testing.py
+-rw-rw-rw-   0        0        0     2895 2023-04-11 21:02:02.000000 danielutils-0.8.2/danielutils/Text.py
+-rw-rw-rw-   0        0        0      423 2023-04-18 23:27:35.000000 danielutils-0.8.2/danielutils/Threading.py
+-rw-rw-rw-   0        0        0      426 2023-04-11 21:07:07.000000 danielutils-0.8.2/danielutils/Time.py
+-rw-rw-rw-   0        0        0      649 2023-01-18 20:34:53.000000 danielutils-0.8.2/danielutils/Typing.py
+-rw-rw-rw-   0        0        0     1248 2023-04-02 14:10:39.000000 danielutils-0.8.2/danielutils/Windows.py
+-rw-rw-rw-   0        0        0      480 2023-04-03 18:57:22.000000 danielutils-0.8.2/danielutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:02:09.331875 danielutils-0.8.2/danielutils.egg-info/
+-rw-rw-rw-   0        0        0      939 2023-04-20 14:02:09.000000 danielutils-0.8.2/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1534 2023-04-20 14:02:09.000000 danielutils-0.8.2/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 14:02:09.000000 danielutils-0.8.2/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-20 14:02:09.000000 danielutils-0.8.2/danielutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 14:02:09.000000 danielutils-0.8.2/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      728 2023-04-20 14:02:08.000000 danielutils-0.8.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 14:02:09.349084 danielutils-0.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-04-20 14:02:08.000000 danielutils-0.8.2/setup.py
```

### Comparing `danielutils-0.8.1/PKG-INFO` & `danielutils-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.8.1
+Version: 0.8.2
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
 
-# danielutils v=0.8.1
+# danielutils v=0.8.2
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
```

### Comparing `danielutils-0.8.1/danielutils/Classes/DataStructures.py` & `danielutils-0.8.2/danielutils/Classes/DataStructures.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Classes/TypedBuiltins.py` & `danielutils-0.8.2/danielutils/Classes/TypedBuiltins.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Classes/frange.py` & `danielutils-0.8.2/danielutils/Classes/frange.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Colors.py` & `danielutils-0.8.2/danielutils/Colors.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Conversions/MainConversions.py` & `danielutils-0.8.2/danielutils/Conversions/MainConversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/DataStructures/Graph.py` & `danielutils-0.8.2/danielutils/DataStructures/Graph.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/DataStructures/MarkovChain.py` & `danielutils-0.8.2/danielutils/DataStructures/MarkovChain.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Decorators.py` & `danielutils-0.8.2/danielutils/Decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import traceback
+import re
 from .Typing import Callable, Any, Union
 import functools
 import threading
 import inspect
 from .Functions import areoneof, isoneof, isoneof_strict, isoftype
 from .Exceptions import *
 
@@ -395,16 +397,15 @@
 
     Args:
         max_depth (int): max recursion depth which is allowed for this function
         return_value (_type_, optional): The value to return when the limit is reached. Defaults to None.
             if is None, will return the last (args, kwargs)
         quiet (bool, optional): whether to print a warning message. Defaults to True.
     """
-    import traceback
-    import re
+
     from .Colors import warning
 
     def deco(func):
         @ functools.wraps(func)
         def wrapper(*args, **kwargs):
             depth = functools.reduce(
                 lambda count, line:
```

### Comparing `danielutils-0.8.1/danielutils/Exceptions.py` & `danielutils-0.8.2/danielutils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Functions.py` & `danielutils-0.8.2/danielutils/Functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/IO.py` & `danielutils-0.8.2/danielutils/IO.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Internet.py` & `danielutils-0.8.2/danielutils/Internet.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Math/Constants.py` & `danielutils-0.8.2/danielutils/Math/Constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Math/MathPrint.py` & `danielutils-0.8.2/danielutils/Math/MathPrint.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Math/MathSymbols.py` & `danielutils-0.8.2/danielutils/Math/MathSymbols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Path.py` & `danielutils-0.8.2/danielutils/Path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Print.py` & `danielutils-0.8.2/danielutils/Print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Serialization.py` & `danielutils-0.8.2/danielutils/Serialization.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/System.py` & `danielutils-0.8.2/danielutils/System.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Generator
 import os
 from math import inf
 from .Decorators import overload, timeout, validate
 from .Typing import IO
 from .Exceptions import TimeoutError
 from .Conversions import str_to_bytes
 from .Functions import areoneof
@@ -125,12 +126,45 @@
                 p.stdin.close()
             if p.stderr is not None:
                 p.stderr.close()
             if p.stdout is not None:
                 p.stdout.close()
 
 
+def cmrt(*args, shell: bool = True) -> Generator[bytes, None, None]:
+    """Executes a command and yields stdout and stderr in real-time.
+
+    Args:
+        *args: A sequence of strings representing the command and its arguments.
+        shell (bool, optional): If True, the command is executed through the shell. Defaults to True.
+
+    Raises:
+        TypeError: If `shell` argument is not a boolean.
+
+    Yields:
+        An iterator that yields bytes for stdout and stderr lines in real-time.
+    """
+    if not isinstance(shell, bool):
+        raise TypeError("The 'shell' parameter must be of type bool.")
+
+    # Quote the arguments that represent file or directory paths.
+    for i, arg in enumerate(args):
+        if Path(args[i]).is_file() or Path(args[i]).is_dir():
+            args = (*args[:i], f"\"{arg}\"", *args[i+1:])
+
+    # Join the arguments into a command string and execute the command.
+    cmd = " ".join(args)
+    process = subprocess.Popen(
+        cmd, shell=shell, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+
+    # Yield stdout and stderr in real-time.
+    while process.poll() is None:
+        yield from process.stderr
+        yield from process.stdout
+
+
 __all__ = [
     "cm",
     "acm",
-    "sleep"
+    "sleep",
+    "cmrt"
 ]
```

### Comparing `danielutils-0.8.1/danielutils/Testing.py` & `danielutils-0.8.2/danielutils/Testing.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Text.py` & `danielutils-0.8.2/danielutils/Text.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Typing.py` & `danielutils-0.8.2/danielutils/Typing.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils/Windows.py` & `danielutils-0.8.2/danielutils/Windows.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.1/danielutils.egg-info/PKG-INFO` & `danielutils-0.8.2/danielutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.8.1
+Version: 0.8.2
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
 
-# danielutils v=0.8.1
+# danielutils v=0.8.2
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
```

### Comparing `danielutils-0.8.1/danielutils.egg-info/SOURCES.txt` & `danielutils-0.8.2/danielutils.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,21 @@
 danielutils/Classes/__init__.py
 danielutils/Classes/frange.py
 danielutils/Conversions/MainConversions.py
 danielutils/Conversions/__init__.py
 danielutils/Conversions/SpecializedConversions/__init__.py
 danielutils/Conversions/SpecializedConversions/to_hex.py
 danielutils/Conversions/SpecializedConversions/to_int.py
+danielutils/DataStructures/Comparer.py
 danielutils/DataStructures/Graph.py
+danielutils/DataStructures/Heap.py
+danielutils/DataStructures/Interface.py
 danielutils/DataStructures/MarkovChain.py
+danielutils/DataStructures/Node.py
+danielutils/DataStructures/Queue.py
 danielutils/DataStructures/__init__.py
+danielutils/DataStructures/functions.py
 danielutils/Math/Constants.py
 danielutils/Math/Functions.py
 danielutils/Math/MathPrint.py
 danielutils/Math/MathSymbols.py
 danielutils/Math/__init__.py
```

### Comparing `danielutils-0.8.1/pyproject.toml` & `danielutils-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "danielutils"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
   { name="danielnachumdev", email="danielnachumdev@gmail.com" },
 ]
 description = "A python utils library for things I find useful"
 readme = "README.md"
 requires-python = ">=3.10.5"
 classifiers = [
```

### Comparing `danielutils-0.8.1/setup.py` & `danielutils-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def read_file(path: str) -> "list[str]":
     with codecs.open(path, 'r', 'utf-8') as f:
         return [l.strip() for l in f.readlines()]
 
 
 README_PATH = 'README.md'
 DESCRIPTION = 'A python utils library for things I find useful'
-VERSION = "0.8.1"
+VERSION = "0.8.2"
 LONG_DESCRIPTION = '\n'.join(read_file(README_PATH))
 setup(
     name="danielutils",
     version=VERSION,
     author="danielnachumdev",
     author_email="<danielnachumdev@gmail.com>",
     description=DESCRIPTION,
```

