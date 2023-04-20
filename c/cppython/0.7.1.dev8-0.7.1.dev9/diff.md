# Comparing `tmp/cppython-0.7.1.dev8.tar.gz` & `tmp/cppython-0.7.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppython-0.7.1.dev8.tar", last modified: Wed Sep  7 12:50:00 2022, max compression
+gzip compressed data, was "cppython-0.7.1.dev9.tar", last modified: Sun Sep 25 18:09:20 2022, max compression
```

## Comparing `cppython-0.7.1.dev8.tar` & `cppython-0.7.1.dev9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/cppython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/cppython/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/cppython/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3044 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/cppython/console/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/cppython/console/vcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/cppython/console/vcs/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/cppython/console/vcs/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     6692 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/cppython/project.py
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/cppython/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/cppython/utility.py
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/tests/integration/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2557 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/tests/unit/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     7032 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/tests/unit/test_project.py
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/tests/unit/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-09-07 12:49:46.668950 cppython-0.7.1.dev8/tests/unit/test_vcs.py
--rw-------   0 runner    (1001) docker     (121)      511 2022-09-07 12:50:00.345126 cppython-0.7.1.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/cppython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5823 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/cppython/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/cppython/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4262 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/cppython/console/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/cppython/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/cppython/plugins/git.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5351 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/cppython/project.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/cppython/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/cppython/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2453 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/tests/data/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/tests/integration/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/tests/integration/test_version_control.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/tests/unit/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5046 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/tests/unit/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-09-25 18:09:09.160613 cppython-0.7.1.dev9/tests/unit/test_version_control.py
+-rw-------   0 runner    (1001) docker     (121)      452 2022-09-25 18:09:20.837433 cppython-0.7.1.dev9/PKG-INFO
```

### Comparing `cppython-0.7.1.dev8/LICENSE.md` & `cppython-0.7.1.dev9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cppython-0.7.1.dev8/tests/integration/test_interface.py` & `cppython-0.7.1.dev9/tests/integration/test_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-"""
-Test the integrations related to the internal interface implementation and the 'Interface' interface itself
+"""Test the integrations related to the internal interface implementation and the 'Interface' interface itself
 """
 
 import pytest
 from cppython_core.schema import InterfaceConfiguration
 from pytest_cppython.plugin import InterfaceIntegrationTests
 
 from cppython.console.interface import ConsoleInterface
 
 
-class TestCLIInterface(InterfaceIntegrationTests):
-    """
-    The tests for our CLI interface
-    """
+class TestCLIInterface(InterfaceIntegrationTests[ConsoleInterface]):
+    """The tests for our CLI interface"""
 
     @pytest.fixture(name="interface")
-    def fixture_interface(self):
-        """
-        Override of the plugin provided interface fixture.
+    def fixture_interface(
+        self, interface_type: type[ConsoleInterface], interface_configuration: InterfaceConfiguration
+    ) -> ConsoleInterface:
+        """Override of the plugin provided interface fixture.
+
+        Args:
+            interface_type: The input interface type
+            interface_configuration: Interface configuration for construction
 
         Returns:
             ConsoleInterface -- The Interface object to use for the CPPython defined tests
         """
         configuration = InterfaceConfiguration()
         return ConsoleInterface(configuration)
```

