# Comparing `tmp/autohooks-plugin-pylint-22.8.1.tar.gz` & `tmp/autohooks_plugin_pylint-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autohooks-plugin-pylint-22.8.1.tar", max compression
+gzip compressed data, was "autohooks_plugin_pylint-23.4.0.tar", max compression
```

## Comparing `autohooks-plugin-pylint-22.8.1.tar` & `autohooks_plugin_pylint-23.4.0.tar`

### file list

```diff
@@ -1,12 +1,9 @@
--rw-r--r--   0        0        0     2170 2022-08-09 06:09:11.149038 autohooks-plugin-pylint-22.8.1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2022-08-09 06:09:11.149038 autohooks-plugin-pylint-22.8.1/LICENSE
--rw-r--r--   0        0        0     2542 2022-08-09 06:09:11.149038 autohooks-plugin-pylint-22.8.1/README.md
--rw-r--r--   0        0        0     4145 2022-08-09 06:09:11.149038 autohooks-plugin-pylint-22.8.1/RELEASE.md
--rw-r--r--   0        0        0      763 2022-08-09 06:09:11.149038 autohooks-plugin-pylint-22.8.1/autohooks/plugins/pylint/__init__.py
--rw-r--r--   0        0        0      103 2022-08-09 06:09:11.149038 autohooks-plugin-pylint-22.8.1/autohooks/plugins/pylint/__version__.py
--rw-r--r--   0        0        0     3489 2022-08-09 06:09:11.149038 autohooks-plugin-pylint-22.8.1/autohooks/plugins/pylint/pylint.py
--rw-r--r--   0        0        0    43166 2022-08-09 06:09:11.149038 autohooks-plugin-pylint-22.8.1/poetry.lock
--rw-r--r--   0        0        0       31 2022-08-09 06:09:11.149038 autohooks-plugin-pylint-22.8.1/poetry.toml
--rw-r--r--   0        0        0     2035 2022-08-09 06:09:11.149038 autohooks-plugin-pylint-22.8.1/pyproject.toml
--rw-r--r--   0        0        0     3464 2022-08-09 06:09:23.870937 autohooks-plugin-pylint-22.8.1/setup.py
--rw-r--r--   0        0        0     3688 2022-08-09 06:09:23.871366 autohooks-plugin-pylint-22.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-20 08:00:30.838663 autohooks_plugin_pylint-23.4.0/LICENSE
+-rw-r--r--   0        0        0     2520 2023-04-20 08:00:30.838663 autohooks_plugin_pylint-23.4.0/README.md
+-rw-r--r--   0        0        0      752 2023-04-20 08:00:30.838663 autohooks_plugin_pylint-23.4.0/autohooks/plugins/pylint/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-20 08:00:30.838663 autohooks_plugin_pylint-23.4.0/autohooks/plugins/pylint/__version__.py
+-rw-r--r--   0        0        0     3815 2023-04-20 08:00:30.838663 autohooks_plugin_pylint-23.4.0/autohooks/plugins/pylint/pylint.py
+-rw-r--r--   0        0        0    62334 2023-04-20 08:00:30.838663 autohooks_plugin_pylint-23.4.0/poetry.lock
+-rw-r--r--   0        0        0       31 2023-04-20 08:00:30.838663 autohooks_plugin_pylint-23.4.0/poetry.toml
+-rw-r--r--   0        0        0     2075 2023-04-20 08:00:30.838663 autohooks_plugin_pylint-23.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 autohooks_plugin_pylint-23.4.0/PKG-INFO
```

### Comparing `autohooks-plugin-pylint-22.8.1/LICENSE` & `autohooks_plugin_pylint-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autohooks-plugin-pylint-22.8.1/README.md` & `autohooks_plugin_pylint-23.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,22 +60,22 @@
 
 [tool.autohooks.plugins.pylint]
 arguments = ["--rcfile=/path/to/pylintrc", "-s", "n"]
 ```
 
 ## Maintainer
 
-This project is maintained by [Greenbone Networks GmbH](https://www.greenbone.net/).
+This project is maintained by [Greenbone AG](https://www.greenbone.net/).
 
 ## Contributing
 
 Your contributions are highly appreciated. Please
 [create a pull request](https://github.com/greenbone/autohooks-plugin-pylint/pulls)
 on GitHub. Bigger changes need to be discussed with the development team via the
 [issues section at GitHub](https://github.com/greenbone/autohooks-plugin-pylint/issues)
 first.
 
 ## License
 
-Copyright (C) 2019 - 2022 [Greenbone Networks GmbH](https://www.greenbone.net/)
+Copyright (C) 2019 - 2022 [Greenbone AG](https://www.greenbone.net/)
 
 Licensed under the [GNU General Public License v3.0 or later](LICENSE).
```

### Comparing `autohooks-plugin-pylint-22.8.1/autohooks/plugins/pylint/__init__.py` & `autohooks_plugin_pylint-23.4.0/autohooks/plugins/pylint/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2022 Greenbone Networks GmbH
+# Copyright (C) 2019-2022 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `autohooks-plugin-pylint-22.8.1/autohooks/plugins/pylint/pylint.py` & `autohooks_plugin_pylint-23.4.0/autohooks/plugins/pylint/pylint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2022 Greenbone Networks GmbH
+# Copyright (C) 2019-2022 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -13,71 +13,76 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import subprocess
 import sys
+from typing import Iterable, List, Optional, Union
 
 from autohooks.api import error, ok, out
 from autohooks.api.git import get_staged_status, stash_unstaged_changes
 from autohooks.api.path import match
+from autohooks.config import Config
+from autohooks.precommit.run import ReportProgress
 
 DEFAULT_INCLUDE = ("*.py",)
 DEFAULT_ARGUMENTS = ["--output-format=colorized"]
 
 
-def check_pylint_installed():
+def check_pylint_installed() -> None:
     try:
         import pylint  # pylint: disable=import-outside-toplevel, disable=unused-import
     except ImportError as e:
-        raise Exception(
+        raise RuntimeError(
             "Could not find pylint. Please add pylint to your python "
             "environment"
         ) from e
 
 
-def get_pylint_config(config):
+def get_pylint_config(config: Config) -> Config:
     return config.get("tool").get("autohooks").get("plugins").get("pylint")
 
 
-def ensure_iterable(value):
+def ensure_iterable(value: Union[str, List[str]]) -> List[str]:
     if isinstance(value, str):
         return [value]
 
     return value
 
 
-def get_include_from_config(config):
+def get_include_from_config(config: Optional[Config]) -> Iterable[str]:
     if not config:
         return DEFAULT_INCLUDE
 
     pylint_config = get_pylint_config(config)
     include = ensure_iterable(
         pylint_config.get_value("include", DEFAULT_INCLUDE)
     )
 
     return include
 
 
-def get_pylint_arguments(config):
+def get_pylint_arguments(config: Optional[Config]) -> Iterable[str]:
     if not config:
         return DEFAULT_ARGUMENTS
 
     pylint_config = get_pylint_config(config)
     arguments = ensure_iterable(
         pylint_config.get_value("arguments", DEFAULT_ARGUMENTS)
     )
 
     return arguments
 
 
 def precommit(
-    config=None, report_progress=None, **kwargs
-):  # pylint: disable=unused-argument
+    config: Optional[Config] = None,
+    report_progress: Optional[ReportProgress] = None,
+    **kwargs,  # pylint: disable=unused-argument
+) -> int:
     check_pylint_installed()
 
     include = get_include_from_config(config)
 
     files = [f for f in get_staged_status() if match(f.path, include)]
 
     if not files:
```

### Comparing `autohooks-plugin-pylint-22.8.1/pyproject.toml` & `autohooks_plugin_pylint-23.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,63 @@
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
-authors = ["Greenbone Networks GmbH <info@greenbone.net>"]
-readme = "README.md"
-license = "AGPL-3.0-or-later"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "autohooks-plugin-pylint"
-version = "22.8.1"
+version = "23.4.0"
 description = "An autohooks plugin for python code linting via pylint"
 license = "GPL-3.0-or-later"
-authors = ["Greenbone Networks GmbH <info@greenbone.net>"]
+authors = ["Greenbone AG <info@greenbone.net>"]
 readme = "README.md"
 homepage = "https://github.com/greenbone/autohooks-plugin-pylint"
 repository = "https://github.com/greenbone/autohooks-plugin-pylint"
 documentation = ""
 # Full list: https://pypi.org/pypi?%3Aaction=list_classifiers
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
   { include = "autohooks" },
-  { include = "CHANGELOG.md", format = "sdist"},
-  { include = "RELEASE.md", format = "sdist"},
   { include = "poetry.lock", format = "sdist"},
   { include = "poetry.toml", format = "sdist"},
 ]
 keywords = [
   "git",
   "formatting",
   "linting",
   "hooks",
   "pylint",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pylint = "^2.8.3"
+python = "^3.7.2"
+pylint = ">=2.8.3"
 autohooks = ">=2.2.0"
 
 [tool.poetry.dev-dependencies]
+coverage = "^7.2.3"
+mypy = ">=0.981"
 pontos = ">=22.8.1"
 autohooks-plugin-black = ">=22.7.0"
-
+autohooks-plugin-isort = ">=22.8.0"
 
 [tool.black]
 line-length = 80
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 exclude = '''
 /(
     \.git
   | \.hg
   | \.venv
   | \.circleci
   | \.github
@@ -67,14 +65,20 @@
   | _build
   | build
   | dist
   | docs
 )/
 '''
 
+[tool.isort]
+profile = "black"
+line_length = 80
+
 [tool.autohooks]
 mode = "poetry"
-pre-commit = ['autohooks.plugins.black', 'autohooks.plugins.pylint']
-
+pre-commit = ['autohooks.plugins.black', 'autohooks.plugins.isort', 'autohooks.plugins.pylint']
 
 [tool.pontos.version]
 version-module-file = "autohooks/plugins/pylint/__version__.py"
+
+[tool.mypy]
+ignore_missing_imports = true
```

### Comparing `autohooks-plugin-pylint-22.8.1/PKG-INFO` & `autohooks_plugin_pylint-23.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: autohooks-plugin-pylint
-Version: 22.8.1
+Version: 23.4.0
 Summary: An autohooks plugin for python code linting via pylint
 Home-page: https://github.com/greenbone/autohooks-plugin-pylint
 License: GPL-3.0-or-later
 Keywords: git,formatting,linting,hooks,pylint
-Author: Greenbone Networks GmbH
+Author: Greenbone AG
 Author-email: info@greenbone.net
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: autohooks (>=2.2.0)
-Requires-Dist: pylint (>=2.8.3,<3.0.0)
+Requires-Dist: pylint (>=2.8.3)
 Project-URL: Repository, https://github.com/greenbone/autohooks-plugin-pylint
 Description-Content-Type: text/markdown
 
 ![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)
 
 # autohooks-plugin-pylint
 
@@ -86,23 +91,23 @@
 
 [tool.autohooks.plugins.pylint]
 arguments = ["--rcfile=/path/to/pylintrc", "-s", "n"]
 ```
 
 ## Maintainer
 
-This project is maintained by [Greenbone Networks GmbH](https://www.greenbone.net/).
+This project is maintained by [Greenbone AG](https://www.greenbone.net/).
 
 ## Contributing
 
 Your contributions are highly appreciated. Please
 [create a pull request](https://github.com/greenbone/autohooks-plugin-pylint/pulls)
 on GitHub. Bigger changes need to be discussed with the development team via the
 [issues section at GitHub](https://github.com/greenbone/autohooks-plugin-pylint/issues)
 first.
 
 ## License
 
-Copyright (C) 2019 - 2022 [Greenbone Networks GmbH](https://www.greenbone.net/)
+Copyright (C) 2019 - 2022 [Greenbone AG](https://www.greenbone.net/)
 
 Licensed under the [GNU General Public License v3.0 or later](LICENSE).
```

