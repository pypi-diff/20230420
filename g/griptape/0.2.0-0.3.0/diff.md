# Comparing `tmp/griptape-0.2.0.tar.gz` & `tmp/griptape-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape-0.2.0.tar", max compression
+gzip compressed data, was "griptape-0.3.0.tar", max compression
```

## Comparing `griptape-0.2.0.tar` & `griptape-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     4070 2023-04-19 15:29:48.352748 griptape-0.2.0/README.md
--rw-r--r--   0        0        0       65 2023-04-18 23:10:38.312719 griptape-0.2.0/griptape/__init__.py
--rw-r--r--   0        0        0      526 2023-04-19 15:59:24.355986 griptape-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 griptape-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4198 2023-04-20 17:21:29.660292 griptape-0.3.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-18 23:10:38.312719 griptape-0.3.0/griptape/__init__.py
+-rw-r--r--   0        0        0      526 2023-04-20 17:22:17.308523 griptape-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4974 1970-01-01 00:00:00.000000 griptape-0.3.0/PKG-INFO
```

### Comparing `griptape-0.2.0/README.md` & `griptape-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # griptape
 
 [![PyPI Version](https://img.shields.io/pypi/v/griptape.svg)](https://pypi.python.org/pypi/griptape)
 [![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/gitbucket/gitbucket/blob/master/LICENSE)
+[![Griptape Discord](https://dcbadge.vercel.app/api/server/gnWRz88eym?compact=true&style=flat)](https://discord.gg/gnWRz88eym)
 
 **griptape** is a modular Python framework for LLM workflows, tools, memory, and data.
 
 With **griptape**, you can:
 
 1. 🚰 Build sequential **LLM pipelines** and sprawling **DAG workflows** for complex use cases.
 2. 🧰️ Augment LLMs with **chain of thought** capabilities and integrate **external tools**, such as calculators, web search, spreadsheet editors, and API connectors.
@@ -85,8 +86,8 @@
 
 ## Contributing
 
 Contributions in the form of bug reports, feature ideas, or pull requests are super welcome! Take a look at the current issues and if you'd like to help please submit a pull request with some tests.
 
 ## License
 
-griptape is available under the Apache 2.0 License.
+griptape is available under the Apache 2.0 License.
```

### Comparing `griptape-0.2.0/pyproject.toml` & `griptape-0.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "griptape"
-version = "0.2.0"
+version = "0.3.0"
 description = "Modular Python framework for LLM workflows, tools, memory, and data."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape"
 
 packages = [
     {include = "griptape"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-griptape-core = "~0.9.2"
+griptape-core = "~0.9.0"
 griptape-flow = "~0.11.0"
 griptape-tools = "~0.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `griptape-0.2.0/PKG-INFO` & `griptape-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: griptape
-Version: 0.2.0
+Version: 0.3.0
 Summary: Modular Python framework for LLM workflows, tools, memory, and data.
 Home-page: https://github.com/griptape-ai/griptape
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: griptape-core (>=0.9.2,<0.10.0)
+Requires-Dist: griptape-core (>=0.9.0,<0.10.0)
 Requires-Dist: griptape-flow (>=0.11.0,<0.12.0)
 Requires-Dist: griptape-tools (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/griptape-ai/griptape
 Description-Content-Type: text/markdown
 
 # griptape
 
 [![PyPI Version](https://img.shields.io/pypi/v/griptape.svg)](https://pypi.python.org/pypi/griptape)
 [![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/gitbucket/gitbucket/blob/master/LICENSE)
+[![Griptape Discord](https://dcbadge.vercel.app/api/server/gnWRz88eym?compact=true&style=flat)](https://discord.gg/gnWRz88eym)
 
 **griptape** is a modular Python framework for LLM workflows, tools, memory, and data.
 
 With **griptape**, you can:
 
 1. 🚰 Build sequential **LLM pipelines** and sprawling **DAG workflows** for complex use cases.
 2. 🧰️ Augment LLMs with **chain of thought** capabilities and integrate **external tools**, such as calculators, web search, spreadsheet editors, and API connectors.
@@ -106,7 +107,8 @@
 ## Contributing
 
 Contributions in the form of bug reports, feature ideas, or pull requests are super welcome! Take a look at the current issues and if you'd like to help please submit a pull request with some tests.
 
 ## License
 
 griptape is available under the Apache 2.0 License.
+
```

