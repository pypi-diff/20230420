# Comparing `tmp/autohooks_plugin_pytest-23.1.0.tar.gz` & `tmp/autohooks_plugin_pytest-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autohooks_plugin_pytest-23.1.0.tar", max compression
+gzip compressed data, was "autohooks_plugin_pytest-23.4.0.tar", max compression
```

## Comparing `autohooks_plugin_pytest-23.1.0.tar` & `autohooks_plugin_pytest-23.4.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-01-05 13:03:17.723749 autohooks_plugin_pytest-23.1.0/LICENSE
--rw-r--r--   0        0        0     2389 2023-01-05 13:03:17.723749 autohooks_plugin_pytest-23.1.0/README.md
--rw-r--r--   0        0        0      822 2023-01-05 13:03:17.723749 autohooks_plugin_pytest-23.1.0/autohooks/plugins/pytest/__init__.py
--rw-r--r--   0        0        0      103 2023-01-05 13:03:17.723749 autohooks_plugin_pytest-23.1.0/autohooks/plugins/pytest/__version__.py
--rw-r--r--   0        0        0     2624 2023-01-05 13:03:17.723749 autohooks_plugin_pytest-23.1.0/autohooks/plugins/pytest/pytest.py
--rw-r--r--   0        0        0     1955 2023-01-05 13:03:17.723749 autohooks_plugin_pytest-23.1.0/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 autohooks_plugin_pytest-23.1.0/setup.py
--rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 autohooks_plugin_pytest-23.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-20 08:11:38.765496 autohooks_plugin_pytest-23.4.0/LICENSE
+-rw-r--r--   0        0        0     2367 2023-04-20 08:11:38.765496 autohooks_plugin_pytest-23.4.0/README.md
+-rw-r--r--   0        0        0      811 2023-04-20 08:11:38.765496 autohooks_plugin_pytest-23.4.0/autohooks/plugins/pytest/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-20 08:11:38.765496 autohooks_plugin_pytest-23.4.0/autohooks/plugins/pytest/__version__.py
+-rw-r--r--   0        0        0     2617 2023-04-20 08:11:38.765496 autohooks_plugin_pytest-23.4.0/autohooks/plugins/pytest/pytest.py
+-rw-r--r--   0        0        0     1901 2023-04-20 08:11:38.765496 autohooks_plugin_pytest-23.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3734 1970-01-01 00:00:00.000000 autohooks_plugin_pytest-23.4.0/PKG-INFO
```

### Comparing `autohooks_plugin_pytest-23.1.0/LICENSE` & `autohooks_plugin_pytest-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autohooks_plugin_pytest-23.1.0/README.md` & `autohooks_plugin_pytest-23.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -56,22 +56,22 @@
 
 [tool.autohooks.plugins.pytest]
 arguments = ["--rcfile=/path/to/pytestrc", "-s", "n"]
 ```
 
 ## Maintainer
 
-This project is maintained by [Greenbone Networks GmbH](https://www.greenbone.net/).
+This project is maintained by [Greenbone AG](https://www.greenbone.net/).
 
 ## Contributing
 
 Your contributions are highly appreciated. Please
 [create a pull request](https://github.com/greenbone/autohooks-plugin-pytest/pulls)
 on GitHub. Bigger changes need to be discussed with the development team via the
 [issues section at GitHub](https://github.com/greenbone/autohooks-plugin-pytest/issues)
 first.
 
 ## License
 
-Copyright (C) 2021-2022 [Greenbone Networks GmbH](https://www.greenbone.net/)
+Copyright (C) 2021-2022 [Greenbone AG](https://www.greenbone.net/)
 
 Licensed under the [GNU General Public License v3.0 or later](LICENSE).
```

### Comparing `autohooks_plugin_pytest-23.1.0/autohooks/plugins/pytest/__init__.py` & `autohooks_plugin_pytest-23.4.0/autohooks/plugins/pytest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2022 Greenbone Networks GmbH
+# Copyright (C) 2021-2022 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `autohooks_plugin_pytest-23.1.0/autohooks/plugins/pytest/pytest.py` & `autohooks_plugin_pytest-23.4.0/autohooks/plugins/pytest/pytest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2022 Greenbone Networks GmbH
+# Copyright (C) 2021-2022 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,31 +11,31 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Provides precommit function for pytest autohook plugin."""
+"""Provides precommit function for pytest autohooks plugin."""
 
 import subprocess
 import sys
-from typing import Iterable, List, Union, Optional
+from typing import Iterable, List, Optional, Union
 
 from autohooks.api import error, ok, out
 from autohooks.config import Config
 
 DEFAULT_ARGUMENTS = ["-ra", "--color=yes", "-q"]
 
 
 def _check_pytest_installed() -> None:
     try:
         import pytest  # pylint: disable=import-outside-toplevel, disable=unused-import
     except ImportError as e:
-        raise Exception(
+        raise RuntimeError(
             "Could not find pytest. Please add pytest to your python "
             "environment"
         ) from e
 
 
 def _get_pytest_config(config: Config) -> Config:
     return config.get("tool").get("autohooks").get("plugins").get("pytest")
```

### Comparing `autohooks_plugin_pytest-23.1.0/pyproject.toml` & `autohooks_plugin_pytest-23.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
-authors = ["Greenbone Networks GmbH <info@greenbone.net>"]
-readme = "README.md"
-license = "AGPL-3.0-or-later"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "autohooks-plugin-pytest"
-version = "23.1.0"
+version = "23.4.0"
 description = "An autohooks plugin for pytest"
 license = "GPL-3.0-or-later"
-authors = ["Greenbone Networks GmbH <info@greenbone.net>"]
+authors = ["Greenbone AG <info@greenbone.net>"]
 readme = "README.md"
 homepage = "https://github.com/greenbone/autohooks-plugin-pytest"
 repository = "https://github.com/greenbone/autohooks-plugin-pytest"
 documentation = ""
 classifiers = [
   # Full list: https://pypi.org/pypi?%3Aaction=list_classifiers
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
 ]
 keywords = [
@@ -36,29 +34,29 @@
   "formatting",
   "linting",
   "hooks",
   "pytest",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-flake8 = ">=4.0.1"
+python = "^3.7.2"
 autohooks = ">=21.3"
 pytest = "^7.1.2"
 
 [tool.poetry.dev-dependencies]
 mypy = ">=0.981"
 pontos = ">=22.7.2"
 autohooks-plugin-black = ">=22.7.0"
 autohooks-plugin-pylint = ">=21.2.0"
 autohooks-plugin-isort = ">=22.3.0"
+coverage = "^7.2.3"
 
 [tool.black]
 line-length = 79
-target-version = ["py37", "py38", "py39", "py310"]
+target-version = ["py37", "py38", "py39", "py310", "py311"]
 exclude = '''
 /(
     \.git
 )/
 '''
 
 [tool.isort]
```

### Comparing `autohooks_plugin_pytest-23.1.0/PKG-INFO` & `autohooks_plugin_pytest-23.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: autohooks-plugin-pytest
-Version: 23.1.0
+Version: 23.4.0
 Summary: An autohooks plugin for pytest
 Home-page: https://github.com/greenbone/autohooks-plugin-pytest
 License: GPL-3.0-or-later
 Keywords: git,formatting,linting,hooks,pytest
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
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: autohooks (>=21.3)
-Requires-Dist: flake8 (>=4.0.1)
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
 Project-URL: Repository, https://github.com/greenbone/autohooks-plugin-pytest
 Description-Content-Type: text/markdown
 
 ![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)
 
 # autohooks-plugin-pytest
@@ -88,23 +87,23 @@
 
 [tool.autohooks.plugins.pytest]
 arguments = ["--rcfile=/path/to/pytestrc", "-s", "n"]
 ```
 
 ## Maintainer
 
-This project is maintained by [Greenbone Networks GmbH](https://www.greenbone.net/).
+This project is maintained by [Greenbone AG](https://www.greenbone.net/).
 
 ## Contributing
 
 Your contributions are highly appreciated. Please
 [create a pull request](https://github.com/greenbone/autohooks-plugin-pytest/pulls)
 on GitHub. Bigger changes need to be discussed with the development team via the
 [issues section at GitHub](https://github.com/greenbone/autohooks-plugin-pytest/issues)
 first.
 
 ## License
 
-Copyright (C) 2021-2022 [Greenbone Networks GmbH](https://www.greenbone.net/)
+Copyright (C) 2021-2022 [Greenbone AG](https://www.greenbone.net/)
 
 Licensed under the [GNU General Public License v3.0 or later](LICENSE).
```

