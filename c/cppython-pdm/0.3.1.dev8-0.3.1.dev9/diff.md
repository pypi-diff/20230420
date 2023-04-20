# Comparing `tmp/cppython-pdm-0.3.1.dev8.tar.gz` & `tmp/cppython-pdm-0.3.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppython-pdm-0.3.1.dev8.tar", last modified: Tue Oct 25 13:41:42 2022, max compression
+gzip compressed data, was "cppython-pdm-0.3.1.dev9.tar", last modified: Sat Mar 11 17:43:24 2023, max compression
```

## Comparing `cppython-pdm-0.3.1.dev8.tar` & `cppython-pdm-0.3.1.dev9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-25 13:41:06.730475 cppython-pdm-0.3.1.dev8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-10-25 13:41:06.730475 cppython-pdm-0.3.1.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 13:41:06.730475 cppython-pdm-0.3.1.dev8/cppython_pdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-10-25 13:41:06.730475 cppython-pdm-0.3.1.dev8/cppython_pdm/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 13:41:06.730475 cppython-pdm-0.3.1.dev8/cppython_pdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-10-25 13:41:06.730475 cppython-pdm-0.3.1.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-25 13:41:06.730475 cppython-pdm-0.3.1.dev8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-25 13:41:06.730475 cppython-pdm-0.3.1.dev8/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-10-25 13:41:06.730475 cppython-pdm-0.3.1.dev8/tests/integration/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-25 13:41:06.730475 cppython-pdm-0.3.1.dev8/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-10-25 13:41:06.730475 cppython-pdm-0.3.1.dev8/tests/unit/test_interface.py
--rw-------   0 runner    (1001) docker     (121)      474 2022-10-25 13:41:42.210692 cppython-pdm-0.3.1.dev8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-11 17:43:04.119766 cppython-pdm-0.3.1.dev9/LICENSE.md
+-rw-r--r--   0        0        0       71 2023-03-11 17:43:04.119766 cppython-pdm-0.3.1.dev9/README.md
+-rw-r--r--   0        0        0        0 2023-03-11 17:43:04.119766 cppython-pdm-0.3.1.dev9/cppython_pdm/__init__.py
+-rw-r--r--   0        0        0     1814 2023-03-11 17:43:04.119766 cppython-pdm-0.3.1.dev9/cppython_pdm/plugin.py
+-rw-r--r--   0        0        0        0 2023-03-11 17:43:04.119766 cppython-pdm-0.3.1.dev9/cppython_pdm/py.typed
+-rw-r--r--   0        0        0     2210 2023-03-11 17:43:04.119766 cppython-pdm-0.3.1.dev9/pyproject.toml
+-rw-r--r--   0        0        0        3 2023-03-11 17:43:04.119766 cppython-pdm-0.3.1.dev9/tests/__init__.py
+-rw-r--r--   0        0        0        3 2023-03-11 17:43:04.119766 cppython-pdm-0.3.1.dev9/tests/integration/__init__.py
+-rw-r--r--   0        0        0      966 2023-03-11 17:43:04.119766 cppython-pdm-0.3.1.dev9/tests/integration/test_interface.py
+-rw-r--r--   0        0        0        3 2023-03-11 17:43:04.119766 cppython-pdm-0.3.1.dev9/tests/unit/__init__.py
+-rw-r--r--   0        0        0      829 2023-03-11 17:43:04.119766 cppython-pdm-0.3.1.dev9/tests/unit/test_interface.py
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 cppython-pdm-0.3.1.dev9/PKG-INFO
```

### Comparing `cppython-pdm-0.3.1.dev8/LICENSE.md` & `cppython-pdm-0.3.1.dev9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cppython-pdm-0.3.1.dev8/cppython_pdm/plugin.py` & `cppython-pdm-0.3.1.dev9/cppython_pdm/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 """Implementation of the PDM Interface Plugin
 """
 
+from logging import getLogger
 from typing import Any
 
 from cppython.project import Project as CPPythonProject
-from cppython_core.plugin_schema.interface import Interface
-from cppython_core.schema import ProjectConfiguration
+from cppython_core.schema import Interface, ProjectConfiguration
 from pdm.core import Core
 from pdm.project.core import Project
 from pdm.signals import post_install
 
 
 class CPPythonPlugin(Interface):
     """Implementation of the PDM Interface Plugin"""
 
     def __init__(self, _core: Core) -> None:
         post_install.connect(self.on_post_install, weak=False)
-
-    @staticmethod
-    def name() -> str:
-        """Name of the plugin
-
-        Returns:
-            The name
-        """
-        return "pdm"
+        self.logger = getLogger("cppython.interface.pdm")
 
     def write_pyproject(self) -> None:
         """Write to file"""
 
+    def write_configuration(self) -> None:
+        """Write to configuration"""
+
     def on_post_install(self, project: Project, dry_run: bool, **_kwargs: Any) -> None:
         """Called after a pdm install command is called
 
         Args:
             project: The input PDM project
             dry_run: If true, won't perform any actions
             _kwargs: Sink for unknown arguments
         """
 
-        pyproject_file = project.pyproject_file.absolute()
+        pyproject_file = project.root.absolute() / project.PYPROJECT_FILENAME
 
         # Attach configuration for CPPythonPlugin callbacks
-        project_configuration = ProjectConfiguration(pyproject_file=pyproject_file, version=project.meta.version)
-        project_configuration.verbosity = project.core.ui.verbosity
+        version = project.pyproject.metadata.get("version")
+        verbosity = project.core.ui.verbosity
+
+        project_configuration = ProjectConfiguration(
+            pyproject_file=pyproject_file, verbosity=verbosity, version=version
+        )
 
-        logger = self.logger()
-        logger.info("CPPython: Entered 'on_post_install'")
+        self.logger.info("CPPython: Entered 'on_post_install'")
 
-        if (pdm_pyproject := project.pyproject) is None:
-            logger.info("CPPython: Project data was not available")
+        if (pdm_pyproject := project.pyproject.read()) is None:
+            self.logger.info("CPPython: Project data was not available")
             return
 
         cppython_project = CPPythonProject(project_configuration, self, pdm_pyproject)
 
         if not dry_run:
             cppython_project.install()
```

### Comparing `cppython-pdm-0.3.1.dev8/pyproject.toml` & `cppython-pdm-0.3.1.dev9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 dynamic = []
 requires-python = ">=3.11"
 dependencies = [
     "cppython>=0.7.1.dev20",
     "pdm>=2.1.5",
 ]
-version = "0.3.1.dev8"
+version = "0.3.1.dev9"
 
 [project.license-files]
 paths = [
     "LICENSE.md",
 ]
 
 [project.urls]
```

### Comparing `cppython-pdm-0.3.1.dev8/tests/integration/test_interface.py` & `cppython-pdm-0.3.1.dev9/tests/integration/test_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 """Integration tests for the interface
 """
 
 import pytest
 from pdm.core import Core
-from pytest_cppython.plugin import InterfaceIntegrationTests
 from pytest_mock import MockerFixture
 
 from cppython_pdm.plugin import CPPythonPlugin
 
 
-class TestCPPythonInterface(InterfaceIntegrationTests[CPPythonPlugin]):
+class TestCPPythonInterface:
     """The tests for the PDM interface"""
 
-    @pytest.fixture(name="plugin_type")
-    def fixture_plugin_type(self) -> type[CPPythonPlugin]:
-        """A required testing hook that allows type generation
-
-        Returns:
-            The plugin type
-        """
-        return CPPythonPlugin
-
     @pytest.fixture(name="interface")
     def fixture_interface(self, plugin_type: type[CPPythonPlugin]) -> CPPythonPlugin:
         """A hook allowing implementations to override the fixture
 
         Args:
             plugin_type: An input interface type
```

### Comparing `cppython-pdm-0.3.1.dev8/tests/unit/test_interface.py` & `cppython-pdm-0.3.1.dev9/tests/unit/test_interface.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,33 @@
 """Unit tests for the interface
 """
 
-from pathlib import Path
-
 import pytest
-from cppython_core.exceptions import PluginError
-from cppython_core.schema import PyProject
 from pdm.core import Core
-from pytest_cppython.plugin import InterfaceUnitTests
-from pytest_mock.plugin import MockerFixture
+from pdm.project.core import Project
 
 from cppython_pdm.plugin import CPPythonPlugin
 
 
-class TestCPPythonInterface(InterfaceUnitTests[CPPythonPlugin]):
+class TestCPPythonInterface:
     """The tests for the PDM interface"""
 
-    @pytest.fixture(name="plugin_type")
-    def fixture_plugin_type(self) -> type[CPPythonPlugin]:
-        """A required testing hook that allows type generation
-
-        Returns:
-            The plugin type
-        """
-
-        return CPPythonPlugin
-
     @pytest.fixture(name="interface")
     def fixture_interface(self, plugin_type: type[CPPythonPlugin]) -> CPPythonPlugin:
         """A hook allowing implementations to override the fixture
 
         Args:
             plugin_type: An input interface type
 
         Returns:
             A newly constructed interface
         """
         return plugin_type(Core())
 
-    def test_install(self, project: PyProject, interface: CPPythonPlugin, mocker: MockerFixture) -> None:
-        """Tests the post install path
-
-        Args:
-            project: Mock project
-            interface: The constructed plugin
-            mocker: Mocker fixture for project mocking
-        """
+    def test_pdm_project(self) -> None:
+        """Verify that this PDM won't return empty data"""
 
-        pdm_project = mocker.MagicMock()
-        pdm_project.core.ui.verbosity = 0
-        pdm_project.meta.version = "1.0.0"
-        pdm_project.pyproject_file = Path("pyproject.toml")
-        pdm_project.pyproject = project.dict(by_alias=True)
+        core = Core()
+        core.load_plugins()
+        pdm_project = Project(core, root_path=None)
 
-        with pytest.raises(PluginError):
-            interface.on_post_install(project=pdm_project, candidates={}, dry_run=False)
+        assert pdm_project
```

