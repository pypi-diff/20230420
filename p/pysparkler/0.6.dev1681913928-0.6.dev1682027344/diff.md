# Comparing `tmp/pysparkler-0.6.dev1681913928.tar.gz` & `tmp/pysparkler-0.6.dev1682027344.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.6.dev1681913928.tar", max compression
+gzip compressed data, was "pysparkler-0.6.dev1682027344.tar", max compression
```

## Comparing `pysparkler-0.6.dev1681913928.tar` & `pysparkler-0.6.dev1682027344.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     9111 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/README.md
--rw-r--r--   0        0        0     1203 2023-04-19 14:18:48.536914 pysparkler-0.6.dev1681913928/pyproject.toml
--rw-r--r--   0        0        0      807 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/__init__.py
--rw-r--r--   0        0        0     4490 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/api.py
--rw-r--r--   0        0        0     6212 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/base.py
--rw-r--r--   0        0        0     5734 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/cli.py
--rw-r--r--   0        0        0     6077 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/pyspark_22_to_23.py
--rw-r--r--   0        0        0     2206 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10450 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3969 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     4550 2023-04-19 14:18:41.136913 pysparkler-0.6.dev1681913928/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0     9990 1970-01-01 00:00:00.000000 pysparkler-0.6.dev1681913928/PKG-INFO
+-rw-r--r--   0        0        0     9874 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/README.md
+-rw-r--r--   0        0        0     1203 2023-04-20 21:49:04.926683 pysparkler-0.6.dev1682027344/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/__init__.py
+-rw-r--r--   0        0        0     5294 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/api.py
+-rw-r--r--   0        0        0     7372 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/base.py
+-rw-r--r--   0        0        0     6398 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/cli.py
+-rw-r--r--   0        0        0     6077 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/pyspark_22_to_23.py
+-rw-r--r--   0        0        0     2206 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10561 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3969 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     4550 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0    10753 1970-01-01 00:00:00.000000 pysparkler-0.6.dev1682027344/PKG-INFO
```

### Comparing `pysparkler-0.6.dev1681913928/README.md` & `pysparkler-0.6.dev1682027344/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,20 +38,21 @@
 | Upgrading from PySpark 1.4 to 1.5               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-1-4-to-1-5)               |
 | Upgrading from PySpark 1.0-1.2 to 1.3           | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-1-0-1-2-to-1-3)           |
 
 ## Features Supported
 
 The tool supports the following features:
 
-| Feature                          | Supported |
-|----------------------------------|-----------|
-| Upgrade PySpark Python script    | ✅         |
-| Upgrade PySpark Jupyter Notebook | ✅         |
-| Dry-run Mode                     | ✅         |
-| Verbose Mode                     | ✅         |
+| Feature                                       | Supported |
+|-----------------------------------------------|-----------|
+| Upgrade PySpark Python script                 | ✅         |
+| Upgrade PySpark Jupyter Notebook              | ✅         |
+| Dry-run Mode                                  | ✅         |
+| Verbose Mode                                  | ✅         |
+| Customize code transformers using YAML config | ✅         |
 
 ### Upgrade PySpark Python script
 
 The tool can upgrade a PySpark Python script. It takes the path to the script as input and upgrades it in place:
 
 ```bash
 pysparkler upgrade --input-file /path/to/script.py
@@ -99,14 +100,34 @@
 For both the above upgrade options, to run in verbose mode, you can use the `--verbose` flag. This will print tool's
 input variables, the input file content, the output content, and a unified diff of the input and output content:
 
 ```bash
 pysparkler --verbose upgrade --input-file /path/to/script.py
 ```
 
+### Customize code transformers using YAML config
+
+The tool uses a YAML config file to customize the code transformers. The config file can be passed using the
+`--config-yaml` flag:
+
+```bash
+pysparkler --config-yaml /path/to/config.yaml upgrade --input-file /path/to/script.py
+```
+
+The config file is a YAML file with the following structure:
+
+```yaml
+pysparkler:
+  dry_run: false # Whether to run in dry-run mode
+  PY24-30-001: # The code transformer ID
+    comment: A new comment # The overriden code hint comment to be used by the code transformer
+  PY24-30-002:
+    enabled: false # Disable the code transformer
+```
+
 ## Contributing
 
 For the development, Poetry is used for packing and dependency management. You can install this using:
 
 ```bash
 pip install poetry
 ```
```

### Comparing `pysparkler-0.6.dev1681913928/pyproject.toml` & `pysparkler-0.6.dev1682027344/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.6.dev1681913928"
+version = "0.6.dev1682027344"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.6.dev1681913928/pysparkler/__init__.py` & `pysparkler-0.6.dev1682027344/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1681913928/pysparkler/api.py` & `pysparkler-0.6.dev1682027344/pysparkler/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,44 +12,64 @@
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 #
 import json
+from typing import Any
 
 import libcst as cst
 import nbformat
 
+from pysparkler.base import BaseTransformer
 from pysparkler.pyspark_22_to_23 import pyspark_22_to_23_transformers
 from pysparkler.pyspark_23_to_24 import pyspark_23_to_24_transformers
 from pysparkler.pyspark_24_to_30 import pyspark_24_to_30_transformers
 from pysparkler.pyspark_31_to_32 import pyspark_31_to_32_transformers
 from pysparkler.pyspark_32_to_33 import pyspark_32_to_33_transformers
 
 
 class PySparkler:
     """Main class for PySparkler"""
 
     def __init__(
-        self, from_pyspark: str = "2.2", to_pyspark: str = "3.3", dry_run: bool = False
+        self,
+        from_pyspark: str = "2.2",
+        to_pyspark: str = "3.3",
+        dry_run: bool = False,
+        **overrides: dict[str, Any]
     ):
         self.from_pyspark = from_pyspark
         self.to_pyspark = to_pyspark
         self.dry_run = dry_run
+        self.overrides = overrides
 
     @property
-    def transformers(self):
-        return [
+    def transformers(self) -> list[BaseTransformer]:
+        """Returns a list of transformers to be applied to the AST"""
+        all_transformers = [
             *pyspark_22_to_23_transformers(),
             *pyspark_23_to_24_transformers(),
             *pyspark_24_to_30_transformers(),
             *pyspark_31_to_32_transformers(),
             *pyspark_32_to_33_transformers(),
         ]
+        # Override the default values of the transformers with the user provided values
+        for transformer in all_transformers:
+            if transformer.transformer_id in self.overrides:
+                transformer.override(**self.overrides[transformer.transformer_id])
+
+        # Filter out disabled transformers
+        enabled_transformers = [
+            transformer for transformer in all_transformers if transformer.enabled
+        ]
+
+        # Return the list of enabled transformers
+        return enabled_transformers
 
     def upgrade_script(self, input_file: str, output_file: str | None = None) -> str:
         """Upgrade a PySpark Python script file to the latest version and provides comments as hints for manual
         changes"""
         # Parse the PySpark script written in version 2.4
         with open(input_file, encoding="utf-8") as f:
             original_code = f.read()
```

### Comparing `pysparkler-0.6.dev1681913928/pysparkler/base.py` & `pysparkler-0.6.dev1682027344/pysparkler/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,31 +11,59 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 #
+from typing import Any
+
 import libcst as cst
 import libcst.matchers as m
 
 
 class BaseTransformer(m.MatcherDecoratableTransformer):
     """Base class for all transformers.
 
-    Attributes:
+    Properties:
         transformer_id: A unique identifier for the transformer rule. Follows the format
             PY<From-Major-Version>-<To-Major-Version>-<Rule-Number>
             Important for idempotency checks and debugging.
-
+        enabled: A boolean to enable or disable the transformer rule
     """
 
-    def __init__(self, transformer_id: str):
+    def __init__(self, transformer_id: str, enabled: bool = True):
         super().__init__()
-        self.transformer_id = transformer_id
+        self._transformer_id = transformer_id
+        self._enabled = enabled
+
+    @property
+    def transformer_id(self) -> str:
+        """A unique read-only identifier for the transformer rule"""
+        return self._transformer_id
+
+    @transformer_id.setter
+    def transformer_id(self, value):
+        raise AttributeError("Cannot set the read-only transformer_id attribute")
+
+    @property
+    def enabled(self) -> bool:
+        """A boolean to enable or disable the transformer rule"""
+        return self._enabled
+
+    @enabled.setter
+    def enabled(self, value):
+        self._enabled = value
+
+    def override(self, **overrides: dict[str, Any]) -> "BaseTransformer":
+        """Override the transformer attributes with kwargs passed in"""
+        for key, value in overrides.items():
+            # Iterate over the kwargs and override the existing attributes
+            setattr(self, key, value)
+        return self
 
 
 class StatementLineCommentWriter(BaseTransformer):
     """Base class for adding comments to the end of the statement line when a matching condition is found"""
 
     def __init__(
         self,
@@ -46,14 +74,18 @@
         self._comment = comment
         self.match_found = False
 
     @property
     def comment(self):
         return self._comment
 
+    @comment.setter
+    def comment(self, value):
+        self._comment = value
+
     def leave_SimpleStatementLine(
         self,
         original_node: cst.SimpleStatementLine,  # pylint: disable=unused-argument
         updated_node: cst.SimpleStatementLine,
     ) -> cst.SimpleStatementLine:
         """Add a comment to the end of the statement line if a matching condition is found"""
         if self.match_found:
@@ -97,14 +129,18 @@
     @property
     def comment(self):
         if self._import_name is None:
             return super().comment
         else:
             return f"{super().comment} to use {self._import_name}"
 
+    @comment.setter
+    def comment(self, value):
+        self._comment = value
+
     def visit_Import(self, node: cst.Import) -> None:
         """Check if pandas_udf is being used in an import statement"""
         if m.matches(
             node,
             m.Import(
                 names=[m.ImportAlias(name=m.Attribute(attr=m.Name(self.import_name)))]
             ),
```

### Comparing `pysparkler-0.6.dev1681913928/pysparkler/cli.py` & `pysparkler-0.6.dev1682027344/pysparkler/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import difflib
 from collections.abc import Callable
 from functools import wraps
 from importlib import metadata
 from typing import Any
 
 import click
+import yaml
 from click import Context
 from rich.console import Console
 from rich.syntax import Syntax
 from rich.table import Table
 
 from pysparkler.api import PySparkler
 
@@ -51,19 +52,35 @@
         return wrapper
 
     return decorator
 
 
 @click.group()
 @click.option("-v", "--verbose", is_flag=True, help="Verbose mode")
+@click.option(
+    "-c",
+    "--config-yaml",
+    type=click.Path(exists=True, readable=True),
+    help="Config YAML to customize PySparkler behavior. Check documentation for more details.",
+)
 @click.pass_context
-def run(ctx: Context, verbose: bool) -> None:
+def run(ctx: Context, verbose: bool, config_yaml: str) -> None:
     """Pysparkler CLI - A tool to upgrade PySpark scripts to newer versions"""
     ctx.ensure_object(dict)
     ctx.obj["verbose"] = verbose
+    ctx.obj["config"] = {}
+
+    if config_yaml:
+        # Load configuration from YAML file
+        with open(config_yaml, encoding="utf-8") as file:
+            config = yaml.load(file, Loader=yaml.SafeLoader)
+
+        # Set the configuration in PySparkler
+        if "pysparkler" in config:
+            ctx.obj["config"] = config["pysparkler"]
 
 
 @run.command()
 @click.option(
     "-i",
     "--input-file",
     required=True,
@@ -105,15 +122,18 @@
     output_kernel: str | None,
 ) -> None:
     """Upgrades a PySpark script or Jupyter Notebook to the latest version, and where not context, provides comments as
     code hints for manual changes.
     """
 
     print_command_params(ctx)
-    pysparkler = PySparkler(dry_run=dry_run)
+    if "dry_run" not in ctx.obj["config"]:
+        ctx.obj["config"]["dry_run"] = dry_run
+
+    pysparkler = PySparkler(**ctx.obj["config"])
 
     file_type = file_type or input_file.split(".")[-1]
     if file_type == "ipynb":
         output_file_content = pysparkler.upgrade_notebook(
             input_file, output_file, output_kernel
         )
     else:
```

### Comparing `pysparkler-0.6.dev1681913928/pysparkler/pyspark_22_to_23.py` & `pysparkler-0.6.dev1682027344/pysparkler/pyspark_22_to_23.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1681913928/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.6.dev1682027344/pysparkler/pyspark_23_to_24.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1681913928/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.6.dev1682027344/pysparkler/pyspark_24_to_30.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,20 +92,21 @@
 class PyArrowEnabledCommentWriter(StatementLineCommentWriter):
     """In Spark 3.0, PySpark requires a PyArrow version of 0.12.1 or higher to use PyArrow related functionality, such
     as pandas_udf, toPandas and createDataFrame with “spark.sql.execution.arrow.enabled=true”, etc.
     """
 
     def __init__(
         self,
+        transformer_id: str = "PY24-30-004",
         pyspark_version: str = "3.0",
         required_dependency_name: str = "PyArrow",
         required_dependency_version: str = "0.12.1",
     ):
         super().__init__(
-            transformer_id="PY24-30-004",
+            transformer_id=transformer_id,
             comment=f"PySpark {pyspark_version} requires {required_dependency_name} version \
 {required_dependency_version} or higher when spark.sql.execution.arrow.enabled is set to true",
         )
 
     def visit_Call(self, node: cst.Call) -> None:
         """Check if spark_session.conf.set("spark.sql.execution.arrow.enabled", "true")"""
         if m.matches(
@@ -133,22 +134,25 @@
     """In PySpark, when PyArrow optimization is enabled, Arrow can perform safe type conversion when converting
     pandas.Series to an Arrow array during serialization. Arrow raises errors when detecting unsafe type conversions
     like overflow. You enable it by setting spark.sql.execution.pandas.convertToArrowArraySafely to true.
     The default setting is false.
     """
 
     def __init__(self):
-        super().__init__()
-        self.transformer_id = "PY24-30-005"
+        super().__init__(transformer_id="PY24-30-005")
 
     @property
     def comment(self):
         return "Consider setting spark.sql.execution.pandas.convertToArrowArraySafely to true to raise errors in case \
 of Integer overflow or Floating point truncation, instead of silent allows."
 
+    @comment.setter
+    def comment(self, value):
+        self._comment = value
+
 
 class CreateDataFrameVerifySchemaCommentWriter(StatementLineCommentWriter):
     """In Spark 3.0, createDataFrame(..., verifySchema=True) validates LongType as well in PySpark. Previously, LongType
     was not verified and resulted in None in case the value overflows. To restore this behavior, verifySchema can be set
     to `False` to disable the validation.
     """
```

### Comparing `pysparkler-0.6.dev1681913928/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.6.dev1682027344/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1681913928/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.6.dev1682027344/pysparkler/pyspark_32_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1681913928/PKG-INFO` & `pysparkler-0.6.dev1682027344/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.6.dev1681913928
+Version: 0.6.dev1682027344
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
@@ -60,20 +60,21 @@
 | Upgrading from PySpark 1.4 to 1.5               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-1-4-to-1-5)               |
 | Upgrading from PySpark 1.0-1.2 to 1.3           | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-1-0-1-2-to-1-3)           |
 
 ## Features Supported
 
 The tool supports the following features:
 
-| Feature                          | Supported |
-|----------------------------------|-----------|
-| Upgrade PySpark Python script    | ✅         |
-| Upgrade PySpark Jupyter Notebook | ✅         |
-| Dry-run Mode                     | ✅         |
-| Verbose Mode                     | ✅         |
+| Feature                                       | Supported |
+|-----------------------------------------------|-----------|
+| Upgrade PySpark Python script                 | ✅         |
+| Upgrade PySpark Jupyter Notebook              | ✅         |
+| Dry-run Mode                                  | ✅         |
+| Verbose Mode                                  | ✅         |
+| Customize code transformers using YAML config | ✅         |
 
 ### Upgrade PySpark Python script
 
 The tool can upgrade a PySpark Python script. It takes the path to the script as input and upgrades it in place:
 
 ```bash
 pysparkler upgrade --input-file /path/to/script.py
@@ -121,14 +122,34 @@
 For both the above upgrade options, to run in verbose mode, you can use the `--verbose` flag. This will print tool's
 input variables, the input file content, the output content, and a unified diff of the input and output content:
 
 ```bash
 pysparkler --verbose upgrade --input-file /path/to/script.py
 ```
 
+### Customize code transformers using YAML config
+
+The tool uses a YAML config file to customize the code transformers. The config file can be passed using the
+`--config-yaml` flag:
+
+```bash
+pysparkler --config-yaml /path/to/config.yaml upgrade --input-file /path/to/script.py
+```
+
+The config file is a YAML file with the following structure:
+
+```yaml
+pysparkler:
+  dry_run: false # Whether to run in dry-run mode
+  PY24-30-001: # The code transformer ID
+    comment: A new comment # The overriden code hint comment to be used by the code transformer
+  PY24-30-002:
+    enabled: false # Disable the code transformer
+```
+
 ## Contributing
 
 For the development, Poetry is used for packing and dependency management. You can install this using:
 
 ```bash
 pip install poetry
 ```
```

