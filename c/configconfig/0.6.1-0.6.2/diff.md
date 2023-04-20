# Comparing `tmp/configconfig-0.6.1.tar.gz` & `tmp/configconfig-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configconfig-0.6.1.tar", last modified: Tue Oct  5 08:29:12 2021, max compression
+gzip compressed data, was "configconfig-0.6.2.tar", last modified: Thu Apr 20 15:27:25 2023, max compression
```

## Comparing `configconfig-0.6.1.tar` & `configconfig-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-10-05 08:29:12.132931 configconfig-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5255 2021-10-05 08:29:12.140931 configconfig-0.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-10-05 08:29:12.140931 configconfig-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7139 2021-10-05 08:29:12.168931 configconfig-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4897 2021-10-05 08:29:12.136931 configconfig-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     3914 2021-10-05 08:28:43.600556 configconfig-0.6.1/configconfig/metaclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     8022 2021-10-05 08:28:43.600556 configconfig-0.6.1/configconfig/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4206 2021-10-05 08:28:43.600556 configconfig-0.6.1/configconfig/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2021-10-05 08:28:43.600556 configconfig-0.6.1/configconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6503 2021-10-05 08:28:43.600556 configconfig-0.6.1/configconfig/configvar.py
--rw-r--r--   0 runner    (1001) docker     (121)     9755 2021-10-05 08:28:43.600556 configconfig-0.6.1/configconfig/validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6920 2021-10-05 08:28:43.600556 configconfig-0.6.1/configconfig/autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)    12871 2021-10-05 08:28:43.600556 configconfig-0.6.1/configconfig/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-05 08:28:43.600556 configconfig-0.6.1/configconfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     7243 2023-04-20 15:27:25.919394 configconfig-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4931 2023-04-20 15:27:25.915394 configconfig-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-20 15:27:25.911394 configconfig-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     5257 2023-04-20 15:27:25.915394 configconfig-0.6.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-04-20 15:27:25.915394 configconfig-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    12871 2023-04-20 15:26:53.867424 configconfig-0.6.2/configconfig/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1441 2023-04-20 15:26:53.867424 configconfig-0.6.2/configconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6503 2023-04-20 15:26:53.867424 configconfig-0.6.2/configconfig/configvar.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 15:26:53.867424 configconfig-0.6.2/configconfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     9786 2023-04-20 15:26:53.867424 configconfig-0.6.2/configconfig/validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-04-20 15:26:53.867424 configconfig-0.6.2/configconfig/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-04-20 15:26:53.867424 configconfig-0.6.2/configconfig/metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-04-20 15:26:53.867424 configconfig-0.6.2/configconfig/autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8095 2023-04-20 15:26:53.867424 configconfig-0.6.2/configconfig/utils.py
```

### Comparing `configconfig-0.6.1/LICENSE` & `configconfig-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `configconfig-0.6.1/README.rst` & `configconfig-0.6.2/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -30,48 +30,48 @@
 	* - Other
 	  - |license| |language| |requires|
 
 .. |docs| image:: https://img.shields.io/readthedocs/configconfig/latest?logo=read-the-docs
 	:target: https://configconfig.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
-.. |docs_check| image:: https://github.com/domdfcoding/configconfig/workflows/Docs%20Check/badge.svg
-	:target: https://github.com/domdfcoding/configconfig/actions?query=workflow%3A%22Docs+Check%22
+.. |docs_check| image:: https://github.com/repo-helper/configconfig/workflows/Docs%20Check/badge.svg
+	:target: https://github.com/repo-helper/configconfig/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
-.. |actions_linux| image:: https://github.com/domdfcoding/configconfig/workflows/Linux/badge.svg
-	:target: https://github.com/domdfcoding/configconfig/actions?query=workflow%3A%22Linux%22
+.. |actions_linux| image:: https://github.com/repo-helper/configconfig/workflows/Linux/badge.svg
+	:target: https://github.com/repo-helper/configconfig/actions?query=workflow%3A%22Linux%22
 	:alt: Linux Test Status
 
-.. |actions_windows| image:: https://github.com/domdfcoding/configconfig/workflows/Windows/badge.svg
-	:target: https://github.com/domdfcoding/configconfig/actions?query=workflow%3A%22Windows%22
+.. |actions_windows| image:: https://github.com/repo-helper/configconfig/workflows/Windows/badge.svg
+	:target: https://github.com/repo-helper/configconfig/actions?query=workflow%3A%22Windows%22
 	:alt: Windows Test Status
 
-.. |actions_macos| image:: https://github.com/domdfcoding/configconfig/workflows/macOS/badge.svg
-	:target: https://github.com/domdfcoding/configconfig/actions?query=workflow%3A%22macOS%22
+.. |actions_macos| image:: https://github.com/repo-helper/configconfig/workflows/macOS/badge.svg
+	:target: https://github.com/repo-helper/configconfig/actions?query=workflow%3A%22macOS%22
 	:alt: macOS Test Status
 
-.. |actions_flake8| image:: https://github.com/domdfcoding/configconfig/workflows/Flake8/badge.svg
-	:target: https://github.com/domdfcoding/configconfig/actions?query=workflow%3A%22Flake8%22
+.. |actions_flake8| image:: https://github.com/repo-helper/configconfig/workflows/Flake8/badge.svg
+	:target: https://github.com/repo-helper/configconfig/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
-.. |actions_mypy| image:: https://github.com/domdfcoding/configconfig/workflows/mypy/badge.svg
-	:target: https://github.com/domdfcoding/configconfig/actions?query=workflow%3A%22mypy%22
+.. |actions_mypy| image:: https://github.com/repo-helper/configconfig/workflows/mypy/badge.svg
+	:target: https://github.com/repo-helper/configconfig/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/configconfig/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/configconfig/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/configconfig/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/configconfig/
 	:alt: Requirements Status
 
-.. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/configconfig/master?logo=coveralls
-	:target: https://coveralls.io/github/domdfcoding/configconfig?branch=master
+.. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/configconfig/master?logo=coveralls
+	:target: https://coveralls.io/github/repo-helper/configconfig?branch=master
 	:alt: Coverage
 
-.. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/configconfig?logo=codefactor
-	:target: https://www.codefactor.io/repository/github/domdfcoding/configconfig
+.. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/configconfig?logo=codefactor
+	:target: https://www.codefactor.io/repository/github/repo-helper/configconfig
 	:alt: CodeFactor Grade
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/configconfig
 	:target: https://pypi.org/project/configconfig/
 	:alt: PyPI - Package Version
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/configconfig?logo=python&logoColor=white
@@ -90,30 +90,30 @@
 	:target: https://anaconda.org/domdfcoding/configconfig
 	:alt: Conda - Package Version
 
 .. |conda-platform| image:: https://img.shields.io/conda/pn/domdfcoding/configconfig?label=conda%7Cplatform
 	:target: https://anaconda.org/domdfcoding/configconfig
 	:alt: Conda - Platform
 
-.. |license| image:: https://img.shields.io/github/license/domdfcoding/configconfig
-	:target: https://github.com/domdfcoding/configconfig/blob/master/LICENSE
+.. |license| image:: https://img.shields.io/github/license/repo-helper/configconfig
+	:target: https://github.com/repo-helper/configconfig/blob/master/LICENSE
 	:alt: License
 
-.. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/configconfig
+.. |language| image:: https://img.shields.io/github/languages/top/repo-helper/configconfig
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/configconfig/v0.6.1
-	:target: https://github.com/domdfcoding/configconfig/pulse
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/configconfig/v0.6.2
+	:target: https://github.com/repo-helper/configconfig/pulse
 	:alt: GitHub commits since tagged version
 
-.. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/configconfig
-	:target: https://github.com/domdfcoding/configconfig/commit/master
+.. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/configconfig
+	:target: https://github.com/repo-helper/configconfig/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2021
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/configconfig
 	:target: https://pypi.org/project/configconfig/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `configconfig-0.6.1/PKG-INFO` & `configconfig-0.6.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 Metadata-Version: 2.1
 Name: configconfig
-Version: 0.6.1
+Version: 0.6.2
 Summary: Load and validate YAML configuration files.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: configuration,yaml
-Home-page: https://github.com/domdfcoding/configconfig
-Project-URL: Issue Tracker, https://github.com/domdfcoding/configconfig/issues
-Project-URL: Source Code, https://github.com/domdfcoding/configconfig
+Home-page: https://github.com/repo-helper/configconfig
+Project-URL: Issue Tracker, https://github.com/repo-helper/configconfig/issues
+Project-URL: Source Code, https://github.com/repo-helper/configconfig
 Project-URL: Documentation, https://configconfig.readthedocs.io/en/latest
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: domdf-python-tools>=0.10.0
 Requires-Dist: jsonschema>=3.2.0
-Requires-Dist: ruamel-yaml>=0.16.12
+Requires-Dist: ruamel.yaml>=0.16.12
 Requires-Dist: typing-extensions>=3.7.4.3
 Requires-Dist: typing-inspect>=0.6.0
-Provides-Extra: sphinx
 Requires-Dist: docutils; extra == 'sphinx'
 Requires-Dist: sphinx<3.4.0,>=3.0.3; extra == 'sphinx'
 Requires-Dist: sphinx-toolbox; extra == 'sphinx'
-Provides-Extra: testing
 Requires-Dist: pytest; extra == 'testing'
-Provides-Extra: all
 Requires-Dist: docutils; extra == 'all'
 Requires-Dist: pytest; extra == 'all'
 Requires-Dist: sphinx<3.4.0,>=3.0.3; extra == 'all'
 Requires-Dist: sphinx-toolbox; extra == 'all'
+Provides-Extra: sphinx
+Provides-Extra: testing
+Provides-Extra: all
 Description-Content-Type: text/x-rst
 
 
 #############
 configconfig
 #############
 
@@ -77,48 +79,48 @@
 	* - Other
 	  - |license| |language| |requires|
 
 .. |docs| image:: https://img.shields.io/readthedocs/configconfig/latest?logo=read-the-docs
 	:target: https://configconfig.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
-.. |docs_check| image:: https://github.com/domdfcoding/configconfig/workflows/Docs%20Check/badge.svg
-	:target: https://github.com/domdfcoding/configconfig/actions?query=workflow%3A%22Docs+Check%22
+.. |docs_check| image:: https://github.com/repo-helper/configconfig/workflows/Docs%20Check/badge.svg
+	:target: https://github.com/repo-helper/configconfig/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
-.. |actions_linux| image:: https://github.com/domdfcoding/configconfig/workflows/Linux/badge.svg
-	:target: https://github.com/domdfcoding/configconfig/actions?query=workflow%3A%22Linux%22
+.. |actions_linux| image:: https://github.com/repo-helper/configconfig/workflows/Linux/badge.svg
+	:target: https://github.com/repo-helper/configconfig/actions?query=workflow%3A%22Linux%22
 	:alt: Linux Test Status
 
-.. |actions_windows| image:: https://github.com/domdfcoding/configconfig/workflows/Windows/badge.svg
-	:target: https://github.com/domdfcoding/configconfig/actions?query=workflow%3A%22Windows%22
+.. |actions_windows| image:: https://github.com/repo-helper/configconfig/workflows/Windows/badge.svg
+	:target: https://github.com/repo-helper/configconfig/actions?query=workflow%3A%22Windows%22
 	:alt: Windows Test Status
 
-.. |actions_macos| image:: https://github.com/domdfcoding/configconfig/workflows/macOS/badge.svg
-	:target: https://github.com/domdfcoding/configconfig/actions?query=workflow%3A%22macOS%22
+.. |actions_macos| image:: https://github.com/repo-helper/configconfig/workflows/macOS/badge.svg
+	:target: https://github.com/repo-helper/configconfig/actions?query=workflow%3A%22macOS%22
 	:alt: macOS Test Status
 
-.. |actions_flake8| image:: https://github.com/domdfcoding/configconfig/workflows/Flake8/badge.svg
-	:target: https://github.com/domdfcoding/configconfig/actions?query=workflow%3A%22Flake8%22
+.. |actions_flake8| image:: https://github.com/repo-helper/configconfig/workflows/Flake8/badge.svg
+	:target: https://github.com/repo-helper/configconfig/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
-.. |actions_mypy| image:: https://github.com/domdfcoding/configconfig/workflows/mypy/badge.svg
-	:target: https://github.com/domdfcoding/configconfig/actions?query=workflow%3A%22mypy%22
+.. |actions_mypy| image:: https://github.com/repo-helper/configconfig/workflows/mypy/badge.svg
+	:target: https://github.com/repo-helper/configconfig/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/configconfig/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/configconfig/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/configconfig/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/configconfig/
 	:alt: Requirements Status
 
-.. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/configconfig/master?logo=coveralls
-	:target: https://coveralls.io/github/domdfcoding/configconfig?branch=master
+.. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/configconfig/master?logo=coveralls
+	:target: https://coveralls.io/github/repo-helper/configconfig?branch=master
 	:alt: Coverage
 
-.. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/configconfig?logo=codefactor
-	:target: https://www.codefactor.io/repository/github/domdfcoding/configconfig
+.. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/configconfig?logo=codefactor
+	:target: https://www.codefactor.io/repository/github/repo-helper/configconfig
 	:alt: CodeFactor Grade
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/configconfig
 	:target: https://pypi.org/project/configconfig/
 	:alt: PyPI - Package Version
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/configconfig?logo=python&logoColor=white
@@ -137,30 +139,30 @@
 	:target: https://anaconda.org/domdfcoding/configconfig
 	:alt: Conda - Package Version
 
 .. |conda-platform| image:: https://img.shields.io/conda/pn/domdfcoding/configconfig?label=conda%7Cplatform
 	:target: https://anaconda.org/domdfcoding/configconfig
 	:alt: Conda - Platform
 
-.. |license| image:: https://img.shields.io/github/license/domdfcoding/configconfig
-	:target: https://github.com/domdfcoding/configconfig/blob/master/LICENSE
+.. |license| image:: https://img.shields.io/github/license/repo-helper/configconfig
+	:target: https://github.com/repo-helper/configconfig/blob/master/LICENSE
 	:alt: License
 
-.. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/configconfig
+.. |language| image:: https://img.shields.io/github/languages/top/repo-helper/configconfig
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/configconfig/v0.6.1
-	:target: https://github.com/domdfcoding/configconfig/pulse
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/configconfig/v0.6.2
+	:target: https://github.com/repo-helper/configconfig/pulse
 	:alt: GitHub commits since tagged version
 
-.. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/configconfig
-	:target: https://github.com/domdfcoding/configconfig/commit/master
+.. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/configconfig
+	:target: https://github.com/repo-helper/configconfig/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2021
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/configconfig
 	:target: https://pypi.org/project/configconfig/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `configconfig-0.6.1/pyproject.toml` & `configconfig-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "configconfig"
-version = "0.6.1"
+version = "0.6.2"
 description = "Load and validate YAML configuration files."
 readme = "README.rst"
 keywords = [ "configuration", "yaml",]
 dynamic = []
 dependencies = [
     "domdf-python-tools>=0.10.0",
     "jsonschema>=3.2.0",
-    "ruamel-yaml>=0.16.12",
+    "ruamel.yaml>=0.16.12",
     "typing-extensions>=3.7.4.3",
     "typing-inspect>=0.6.0",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
@@ -38,17 +40,17 @@
 email = "dominic@davis-foster.co.uk"
 
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
-Homepage = "https://github.com/domdfcoding/configconfig"
-"Issue Tracker" = "https://github.com/domdfcoding/configconfig/issues"
-"Source Code" = "https://github.com/domdfcoding/configconfig"
+Homepage = "https://github.com/repo-helper/configconfig"
+"Issue Tracker" = "https://github.com/repo-helper/configconfig/issues"
+"Source Code" = "https://github.com/repo-helper/configconfig"
 Documentation = "https://configconfig.readthedocs.io/en/latest"
 
 [project.optional-dependencies]
 sphinx = [ "docutils", "sphinx<3.4.0,>=3.0.3", "sphinx-toolbox",]
 testing = [ "pytest",]
 all = [ "docutils", "pytest", "sphinx<3.4.0,>=3.0.3", "sphinx-toolbox",]
 
@@ -59,51 +61,50 @@
 [tool.whey]
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 
 [tool.sphinx-pyproject]
-github_username = "domdfcoding"
+github_username = "repo-helper"
 github_repository = "configconfig"
 author = "Dominic Davis-Foster"
 project = "configconfig"
-copyright = "2020-2021 Dominic Davis-Foster"
+copyright = "2020-2023 Dominic Davis-Foster"
 language = "en"
 package_root = "configconfig"
 extensions = [
     "sphinx_toolbox",
     "sphinx_toolbox.more_autodoc",
     "sphinx_toolbox.more_autosummary",
     "sphinx_toolbox.documentation_summary",
     "sphinx_toolbox.tweaks.param_dash",
+    "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
     "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
-    "sphinxcontrib.toctree_plus",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
-    "sphinx_toolbox_experimental.html_section",
-    "sphinx_toolbox_experimental.needspace",
+    "html_section",
     "sphinx_toolbox_experimental.missing_xref",
-    "sphinx_toolbox_experimental.autosummary_widths",
+    "sphinx_toolbox.more_autosummary.column_widths",
 ]
 sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
@@ -150,15 +151,15 @@
     "__hash__",
 ]
 
 [tool.dep_checker]
 namespace_packages = "ruamel.yaml"
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 incremental = false
```

### Comparing `configconfig-0.6.1/configconfig/metaclass.py` & `configconfig-0.6.2/configconfig/metaclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 	rtype: Type
 	required: bool
 	default: Any
 	validator: Callable
 	category: str
 	__name__: str
 
-	def __new__(cls, name: str, bases, dct: Dict):  # noqa: D102
+	def __new__(cls, name: str, bases, dct: Dict):  # noqa: D102,MAN001
 		x = cast("ConfigVar", super().__new__(cls, name, bases, dct))
 
 		def get(name, default):
 			return dct.get(name, getattr(x, name, default))
 
 		x.dtype = get("dtype", Any)
 
@@ -123,15 +123,15 @@
 
 		:rtype: See the :attr:`ConfigVar.rtype <.ConfigVar.rtype>` attribute.
 		"""
 
 		return cls.get(raw_config_vars)
 
 	@abstractmethod
-	def get(cls, raw_config_vars: Mapping[str, Any]):  # pragma: no cover  # noqa: D102
+	def get(cls, raw_config_vars: Mapping[str, Any]):  # pragma: no cover  # noqa: D102,MAN002
 		return NotImplemented
 
 	def __repr__(self) -> str:
 		"""
 		Return a string representation of the :class:`~.ConfigVarMeta` class.
 		"""
```

### Comparing `configconfig-0.6.1/configconfig/utils.py` & `configconfig-0.6.2/configconfig/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 	# stdlib
 	import collections.abc
 
 	# 3rd party
 	from typing_inspect import get_origin
 
-	def get_args(tp):
+	def get_args(tp):  # noqa: MAN001,MAN002
 		"""Get type arguments with all substitutions performed.
 
 		For unions, basic simplifications used by Union constructor are performed.
 
 		Examples::
 
 			get_args(Dict[str, int]) == (str, int)
@@ -93,20 +93,21 @@
 		"get_json_type",
 		"RawConfigVarsType",
 		]
 
 #: A literal ``TAB`` (``\t``) character for use in f-strings.
 tab = '\t'
 
-if sys.version_info < (3, 7):
-	UnionType = Any
-	GenericAliasType = Any
-else:
-	UnionType = type(Union)
-	GenericAliasType = type(List)
+# TODO: latest mypy no longer happy
+# if sys.version_info < (3, 7):
+UnionType = Any
+GenericAliasType = Any
+# else:
+# 	UnionType = type(Union)
+# 	GenericAliasType = type(List)
 
 
 def optional_getter(raw_config_vars: Dict[str, Any], cls: "ConfigVarMeta", required: bool) -> Any:
 	"""
 	Returns either the configuration value, the default,
 	or raises an error if the value is required but wasn't supplied.
 
@@ -139,15 +140,15 @@
 		bool: "Boolean",
 		list: "Sequence",
 		dict: "Mapping",
 		Any: "anything",
 		}
 
 
-def check_type(left: Type, *right: Type):
+def check_type(left: Type, *right: Type) -> bool:
 	return left in right or get_origin(left) in right
 
 
 def get_yaml_type(type_: Type) -> str:
 	r"""
 	Get the YAML type that corresponds to the given Python type.
```

### Comparing `configconfig-0.6.1/configconfig/parser.py` & `configconfig-0.6.2/configconfig/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 	"""
 
 	config_vars: List[ConfigVarMeta]
 
 	def __init__(self, allow_unknown_keys: bool = False):
 		self.allow_unknown_keys = allow_unknown_keys
 
-	def run(self, filename: PathLike):
+	def run(self, filename: PathLike) -> MutableMapping[str, Any]:
 		"""
 		Parse configuration from the given file.
 
 		:param filename: The filename of the YAML configuration file.
 		"""
 
 		filename = PathPlus(filename)
```

### Comparing `configconfig-0.6.1/configconfig/__init__.py` & `configconfig-0.6.2/configconfig/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.6.1"
+__version__: str = "0.6.2"
 __email__: str = "dominic@davis-foster.co.uk"
```

### Comparing `configconfig-0.6.1/configconfig/configvar.py` & `configconfig-0.6.2/configconfig/configvar.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 class ConfigVar(metaclass=ConfigVarMeta):
 	"""
 	Base class for ``YAML`` configuration values.
 
 	The class docstring should be the description of the config var, with an example,
 	and the name of the class should be the variable name.
 
-	If you would prefer a more Pythonic naming approach the variable name can
-	be configured with the ``name`` class variable.
+	Alternatively, for a more Pythonic naming approach, the variable name can
+	be set with the ``name`` class variable.
 
 	.. latex:vspace:: -5px
 
 	:bold-title:`Example:`
 
 	.. code-block:: python
 
@@ -157,15 +157,15 @@
 		if cls.rtype is None:
 			cls.rtype = cls.dtype
 
 		validator = Validator(cls)
 		return validator.validate(raw_config_vars)
 
 	@classmethod
-	def make_documentation(cls):
+	def make_documentation(cls) -> str:
 		"""
 		Returns the reStructuredText documentation for the :class:`~.ConfigVar`.
 		"""
 
 		docstring = cls.__doc__ or ''
 		docstring = (indent(dedent(docstring), tab))
```

### Comparing `configconfig-0.6.1/configconfig/validator.py` & `configconfig-0.6.2/configconfig/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 
 __all__ = ["Validator", "validate_files"]
 
 
 class Validator:
 	"""
 	Methods are named ``visit_<type>``.
+
+	.. autosummary-widths:: 4/10
 	"""
 
 	def __init__(self, config_var: ConfigVarMeta):
 		self.config_var = config_var
 
 	_dtypes = {
 			str: "str",
```

### Comparing `configconfig-0.6.1/configconfig/autoconfig.py` & `configconfig-0.6.2/configconfig/autoconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 	has_content: bool = True
 	required_arguments: int = 1
 	# the fully qualified name of the ConfigVar object,
 	# or the name of the module if :category: given
 	option_spec = {"category": unchanged}
 
-	def run(self) -> Sequence[nodes.Node]:  # type: ignore
+	def run(self) -> Sequence[nodes.Node]:
 		"""
 		Process the content of the directive.
 		"""
 
 		config_var: str = self.arguments[0]
 
 		if "category" in self.options:
```

### Comparing `configconfig-0.6.1/configconfig/testing.py` & `configconfig-0.6.2/configconfig/testing.py`

 * *Files identical despite different names*

