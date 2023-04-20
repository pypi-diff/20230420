# Comparing `tmp/vutils-testing-1.0.1.tar.gz` & `tmp/vutils-testing-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vutils-testing-1.0.1.tar", last modified: Tue Apr 18 22:34:43 2023, max compression
+gzip compressed data, was "vutils-testing-1.0.2.tar", last modified: Thu Apr 20 20:30:40 2023, max compression
```

## Comparing `vutils-testing-1.0.1.tar` & `vutils-testing-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.923689 vutils-testing-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-18 22:34:43.923689 vutils-testing-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-18 22:34:43.923689 vutils-testing-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.915689 vutils-testing-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.915689 vutils-testing-1.0.1/src/vutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.919689 vutils-testing-1.0.1/src/vutils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/src/vutils/testing/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.919689 vutils-testing-1.0.1/src/vutils_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-18 22:34:43.000000 vutils-testing-1.0.1/src/vutils_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-18 22:34:43.000000 vutils-testing-1.0.1/src/vutils_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:34:43.000000 vutils-testing-1.0.1/src/vutils_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:34:43.000000 vutils-testing-1.0.1/src/vutils_testing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 22:34:43.000000 vutils-testing-1.0.1/src/vutils_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 22:34:43.000000 vutils-testing-1.0.1/src/vutils_testing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.915689 vutils-testing-1.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:43.923689 vutils-testing-1.0.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tests/unit/test_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tests/unit/test_testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tests/unit/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-18 22:34:23.000000 vutils-testing-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:30:40.787747 vutils-testing-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-20 20:30:40.787747 vutils-testing-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-20 20:30:40.787747 vutils-testing-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:30:40.783748 vutils-testing-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:30:40.783748 vutils-testing-1.0.2/src/vutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:30:40.783748 vutils-testing-1.0.2/src/vutils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/src/vutils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/src/vutils/testing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/src/vutils/testing/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/src/vutils/testing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/src/vutils/testing/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/src/vutils/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/src/vutils/testing/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:30:40.787747 vutils-testing-1.0.2/src/vutils_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-20 20:30:40.000000 vutils-testing-1.0.2/src/vutils_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-20 20:30:40.000000 vutils-testing-1.0.2/src/vutils_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:30:40.000000 vutils-testing-1.0.2/src/vutils_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:30:40.000000 vutils-testing-1.0.2/src/vutils_testing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 20:30:40.000000 vutils-testing-1.0.2/src/vutils_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 20:30:40.000000 vutils-testing-1.0.2/src/vutils_testing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:30:40.783748 vutils-testing-1.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:30:40.787747 vutils-testing-1.0.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/tests/unit/test_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/tests/unit/test_testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/tests/unit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-20 20:30:26.000000 vutils-testing-1.0.2/tox.ini
```

### Comparing `vutils-testing-1.0.1/ChangeLog.md` & `vutils-testing-1.0.2/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Change Log
 
+## 1.0.2
+
+* Fix doc strings, slim imports
+
 ## 1.0.1
 
 * Remove unused `pytest-order` from `tox.ini`
 
 ## 1.0.0
 
 * Move the development status to production/stable
```

### Comparing `vutils-testing-1.0.1/LICENSE` & `vutils-testing-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.1/PKG-INFO` & `vutils-testing-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-testing
-Version: 1.0.1
+Version: 1.0.2
 Summary: Auxiliary library for writing tests
 Home-page: https://github.com/i386x/vutils-testing
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-testing/issues
 Project-URL: Source, https://github.com/i386x/vutils-testing
```

### Comparing `vutils-testing-1.0.1/README.md` & `vutils-testing-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.1/pyproject.toml` & `vutils-testing-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.1/setup.cfg` & `vutils-testing-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.1/src/vutils/testing/__init__.pyi` & `vutils-testing-1.0.2/src/vutils/testing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.1/src/vutils/testing/mock.py` & `vutils-testing-1.0.2/src/vutils/testing/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 # Project: vutils-testing: Auxiliary library for writing tests
 #
 # SPDX-License-Identifier: MIT
 #
 """Mocking utilities."""
 
 import unittest.mock
-from typing import TYPE_CHECKING, Iterable
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
+    from typing import Iterable
     from unittest.mock import Mock
 
     from vutils.testing import (
         KwArgsType,
         MockableType,
         PatchType,
         ReturnsType,
@@ -114,15 +115,15 @@
 
     :ivar __patchers: The list of patchers
     """
 
     __patchers: "list[PatchType]"
     __slots__ = ("__patchers",)
 
-    def __init__(self, patchers: Iterable["PatchType"]) -> None:
+    def __init__(self, patchers: "Iterable[PatchType]") -> None:
         """
         Initialize the context manager.
 
         :param patchers: The list of patchers
         """
         self.__patchers = list(patchers)
 
@@ -136,15 +137,15 @@
             patcher.start()
         return self
 
     def __exit__(self, *args: object) -> None:
         """
         Revert applied patches in reverse order.
 
-        :param args: Unused arguments
+        :param args: Unused positional arguments
         """
         for patcher in reversed(self.__patchers):
             patcher.stop()
 
 
 class PatcherFactory:
     r"""
```

### Comparing `vutils-testing-1.0.1/src/vutils/testing/testcase.py` & `vutils-testing-1.0.2/src/vutils/testing/testcase.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.1/src/vutils/testing/utils.py` & `vutils-testing-1.0.2/src/vutils/testing/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 # Project: vutils-testing: Auxiliary library for writing tests
 #
 # SPDX-License-Identifier: MIT
 #
 """Miscellaneous utilities."""
 
 import importlib
-from typing import TYPE_CHECKING, Iterable, cast
+from typing import TYPE_CHECKING, cast
 
 from vutils.testing.mock import PatcherFactory
 
 if TYPE_CHECKING:
     from types import ModuleType
+    from typing import Iterable
     from unittest import TestCase
 
     from vutils.testing import (
         ArgsType,
         BasesType,
         ExcSpecType,
         FuncType,
@@ -171,30 +172,31 @@
 
 class LazyInstance:
     r"""
     Support lazy initialization.
 
     :ivar __cache: The lazy instance proxy to the instance mapping
     :ivar __klass: The class of the instance
-    :ivar __initialize_once: When :obj:`False`, :meth:`.get_instance` creates
-        a new instance every time when called
+    :ivar __initialize_once: When :obj:`False`,
+        :meth:`~.LazyInstance.get_instance` creates a new instance every time
+        when called
 
     Object is constructed/initialized at time when its member function is
     called. Example::
 
         foo_factory = LazyInstance(Foo, initialize_once=False)
         foo = foo_factory.create(1, bar=2)
         test(foo.quux)
 
     when ``test`` calls ``foo.quux``, ``Foo(1, bar=2)`` is invoked first
     to make the instance of ``Foo`` and to cache the instance inside
     ``foo_factory``. Then, from this instance, ``quux`` is invoked. Since
-    ``foo_factory`` was created with :attr:`.__initialize_once` property set
-    to :obj:`False`, ``foo`` is initialized every time when ``foo.quux`` is
-    invoked.
+    ``foo_factory`` was created with :attr:`~.LazyInstance.__initialize_once`
+    property set to :obj:`False`, ``foo`` is initialized every time when
+    ``foo.quux`` is invoked.
 
     The story behind :class:`.LazyInstance`: consider the following snippet of
     code::
 
         class Foo:
             def __init__(self):
                 self.stream = sys.stderr
@@ -376,15 +378,15 @@
 
     __slots__ = ()
 
     def setup(self) -> None:
         """Set up the patcher."""
         self.add_spec("typing.TYPE_CHECKING", new=True)
 
-    def extend(self, target: str, symbols: Iterable[str]) -> None:
+    def extend(self, target: str, symbols: "Iterable[str]") -> None:
         """
         Specify patches for :arg:`target`.
 
         :param target: The target module
         :param symbols: The list of symbols to be patched in the :arg:`target`
         """
         for symbol in symbols:
@@ -401,15 +403,15 @@
         Return the class-like symbol name.
 
         :return: the class-like symbol name
         """
         return cls.__name__
 
 
-def cover_typing(name: str, symbols: Iterable[str]) -> None:
+def cover_typing(name: str, symbols: "Iterable[str]") -> None:
     """
     Cover the ``if typing.TYPE_CHECKING`` branch.
 
     :param name: The module name
     :param symbols: The list of symbols
 
     To make the code like ::
```

### Comparing `vutils-testing-1.0.1/src/vutils_testing.egg-info/PKG-INFO` & `vutils-testing-1.0.2/src/vutils_testing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-testing
-Version: 1.0.1
+Version: 1.0.2
 Summary: Auxiliary library for writing tests
 Home-page: https://github.com/i386x/vutils-testing
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-testing/issues
 Project-URL: Source, https://github.com/i386x/vutils-testing
```

### Comparing `vutils-testing-1.0.1/src/vutils_testing.egg-info/SOURCES.txt` & `vutils-testing-1.0.2/src/vutils_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.1/tests/unit/test_mock.py` & `vutils-testing-1.0.2/tests/unit/test_mock.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.1/tests/unit/test_testcase.py` & `vutils-testing-1.0.2/tests/unit/test_testcase.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.1/tests/unit/test_utils.py` & `vutils-testing-1.0.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.1/tests/unit/test_version.py` & `vutils-testing-1.0.2/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.1/tests/unit/utils.py` & `vutils-testing-1.0.2/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `vutils-testing-1.0.1/tox.ini` & `vutils-testing-1.0.2/tox.ini`

 * *Files identical despite different names*

