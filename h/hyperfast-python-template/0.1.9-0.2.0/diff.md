# Comparing `tmp/hyperfast_python_template-0.1.9.tar.gz` & `tmp/hyperfast_python_template-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.1.9.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.2.0.tar", max compression
```

## Comparing `hyperfast_python_template-0.1.9.tar` & `hyperfast_python_template-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1071 2023-03-01 04:32:19.614018 hyperfast_python_template-0.1.9/LICENSE
--rw-r--r--   0        0        0     6175 2023-03-01 04:32:06.322205 hyperfast_python_template-0.1.9/README.md
--rw-r--r--   0        0        0     2837 2023-03-01 04:32:20.546008 hyperfast_python_template-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     6709 1970-01-01 00:00:00.000000 hyperfast_python_template-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-20 03:12:20.884006 hyperfast_python_template-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5698 2023-04-20 03:12:16.171950 hyperfast_python_template-0.2.0/README.md
+-rw-r--r--   0        0        0     2882 2023-04-20 03:12:37.928256 hyperfast_python_template-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6232 1970-01-01 00:00:00.000000 hyperfast_python_template-0.2.0/PKG-INFO
```

### Comparing `hyperfast_python_template-0.1.9/LICENSE` & `hyperfast_python_template-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.1.9/README.md` & `hyperfast_python_template-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,86 +3,72 @@
 [![license-image]][license-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![conventional-commits-image]][conventional commits]
 [![jupyter-book-image]][jupyter book]
 
 <!-- Links: -->
-[hyperfast python template]: https://github.com/entelecheia/hyperfast-python-template
 
+[hyperfast python template]: https://github.com/entelecheia/hyperfast-python-template
 [license-image]: https://img.shields.io/github/license/entelecheia/hyperfast-python-template
 [license-url]: https://github.com/entelecheia/hyperfast-python-template/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyperfast-python-template?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyperfast-python-template
 [release-url]: https://github.com/entelecheia/hyperfast-python-template/releases
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
-
 [repo-url]: https://github.com/entelecheia/hyperfast-python-template
 [pypi-url]: https://pypi.org/project/hyperfast-python-template
 [docs-url]: https://hyperfast-python.entelecheia.cc
 [changelog]: https://github.com/entelecheia/hyperfast-python-template/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyperfast-python-template/blob/main/CONTRIBUTING.md
+
 <!-- Links: -->
 
 A python template that helps you jump start your project
 
 - Documentation: [https://hyperfast-python.entelecheia.cc][docs-url]
 - GitHub: [https://github.com/entelecheia/hyperfast-python-template][repo-url]
 - PyPI: [https://pypi.org/project/hyperfast-python-template][pypi-url]
 
-Hyperfast Python Template is a self-contained template that helps you initialize your Python project inside the template. It is hyperfast in the sense that the template itself is converted into a Python project in the blink of an eye. It is also hyperfast in the sense that it helps you jump start your project with the best practices in the Python community.
+Hyperfast Python Template is a self-contained template that helps you initialize your Python project inside the template. It is hyperfast in the sense that it helps you jump start your project with the best practices in the Python community.
 
 ## Quickstart
 
-There are three ways to use this project:
+There are two ways to use this project:
 
-- Use [Hyperfast Python Template] to create a new repository
 - Use [Copier] to create a project to your local machine directly
 - Inject [Hyperfast Python Template] into an existing project
 
-### I. Use the template
-
-1. Click the `Use this template` button
-2. Enter a name for your repository
-3. Click `Create repository from template`
-4. Clone your new repository to your local machine
-5. Initialize your project
-    ```bash
-    make init-project
-    ```
-6. Do your work
-
-### II. Use Copier
+### I. Use Copier
 
 1. Install Copier
-    ```bash
-    pipx install copier
-    ```
+   ```bash
+   pipx install copier
+   ```
 2. Run
-    ```bash
-    copier gh:entelecheia/hyperfast-python-template path/to/destination
-    ```
+   ```bash
+   copier gh:entelecheia/hyperfast-python-template path/to/destination
+   ```
 3. Do your work
 
-### III. Inject the template
+### II. Inject the template
 
 1. Install Copier
-    ```bash
-    pipx install copier
-    ```
+   ```bash
+   pipx install copier
+   ```
 2. From the root of your project, run
-    ```bash
-    copier gh:entelecheia/hyperfast-python-template .
-    ```
+   ```bash
+   copier gh:entelecheia/hyperfast-python-template .
+   ```
 3. Do your work
 
 ## Features
 
-
 - [x] Automated changelog with [Conventional Commits] and [Python Semantic Release]
 - [x] Automated dependency updates with [Dependabot]
 - [x] Automated semantic versioning with [Python Semantic Release]
 - [x] Automated uploads to [PyPI] and [TestPyPI]
 - [x] Code coverage with [Pytest-Cov]
 - [x] Code formatting with [Black] and [Prettier]
 - [x] Continuous integration with [GitHub Actions]
```

### Comparing `hyperfast_python_template-0.1.9/pyproject.toml` & `hyperfast_python_template-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.1.9"
+version = "0.2.0"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
 
 [tool.poetry.scripts]
@@ -28,14 +28,15 @@
 exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.isort]
 profile = "black"
 skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.flake8]
+ignore = ['F401', 'E501', 'W503']
 exclude = ["node_modules", "_build", "docs", "tests", "venv", ".copier-template", ".refs"]
 per-file-ignores = ['__init__.py:F401', '_version.py:W292']
 
 [tool.mypy]
 namespace_packages = true
 exclude = ["node_modules", "build", "_build", "dist", "docs", "tests", "venv", ".copier-template", ".refs"]
 # 3rd party import
@@ -87,13 +88,13 @@
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
-build_command = "pip install poetry && poetry build"
+build_command = "poetry build --no-cache"
 hvcs = "github" # hosting version control system, gitlab is also supported
 
 [build-system]
-requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
+requires = ["poetry-core>=1.0.0", "setuptools>=45", "setuptools_scm[toml]>=6.2"]
 build-backend = 'setuptools.build_meta'
```

### Comparing `hyperfast_python_template-0.1.9/PKG-INFO` & `hyperfast_python_template-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.1.9
+Version: 0.2.0
 Summary: A python template that helps you jump start your project
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,86 +18,72 @@
 [![license-image]][license-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![conventional-commits-image]][conventional commits]
 [![jupyter-book-image]][jupyter book]
 
 <!-- Links: -->
-[hyperfast python template]: https://github.com/entelecheia/hyperfast-python-template
 
+[hyperfast python template]: https://github.com/entelecheia/hyperfast-python-template
 [license-image]: https://img.shields.io/github/license/entelecheia/hyperfast-python-template
 [license-url]: https://github.com/entelecheia/hyperfast-python-template/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyperfast-python-template?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyperfast-python-template
 [release-url]: https://github.com/entelecheia/hyperfast-python-template/releases
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
-
 [repo-url]: https://github.com/entelecheia/hyperfast-python-template
 [pypi-url]: https://pypi.org/project/hyperfast-python-template
 [docs-url]: https://hyperfast-python.entelecheia.cc
 [changelog]: https://github.com/entelecheia/hyperfast-python-template/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyperfast-python-template/blob/main/CONTRIBUTING.md
+
 <!-- Links: -->
 
 A python template that helps you jump start your project
 
 - Documentation: [https://hyperfast-python.entelecheia.cc][docs-url]
 - GitHub: [https://github.com/entelecheia/hyperfast-python-template][repo-url]
 - PyPI: [https://pypi.org/project/hyperfast-python-template][pypi-url]
 
-Hyperfast Python Template is a self-contained template that helps you initialize your Python project inside the template. It is hyperfast in the sense that the template itself is converted into a Python project in the blink of an eye. It is also hyperfast in the sense that it helps you jump start your project with the best practices in the Python community.
+Hyperfast Python Template is a self-contained template that helps you initialize your Python project inside the template. It is hyperfast in the sense that it helps you jump start your project with the best practices in the Python community.
 
 ## Quickstart
 
-There are three ways to use this project:
+There are two ways to use this project:
 
-- Use [Hyperfast Python Template] to create a new repository
 - Use [Copier] to create a project to your local machine directly
 - Inject [Hyperfast Python Template] into an existing project
 
-### I. Use the template
-
-1. Click the `Use this template` button
-2. Enter a name for your repository
-3. Click `Create repository from template`
-4. Clone your new repository to your local machine
-5. Initialize your project
-    ```bash
-    make init-project
-    ```
-6. Do your work
-
-### II. Use Copier
+### I. Use Copier
 
 1. Install Copier
-    ```bash
-    pipx install copier
-    ```
+   ```bash
+   pipx install copier
+   ```
 2. Run
-    ```bash
-    copier gh:entelecheia/hyperfast-python-template path/to/destination
-    ```
+   ```bash
+   copier gh:entelecheia/hyperfast-python-template path/to/destination
+   ```
 3. Do your work
 
-### III. Inject the template
+### II. Inject the template
 
 1. Install Copier
-    ```bash
-    pipx install copier
-    ```
+   ```bash
+   pipx install copier
+   ```
 2. From the root of your project, run
-    ```bash
-    copier gh:entelecheia/hyperfast-python-template .
-    ```
+   ```bash
+   copier gh:entelecheia/hyperfast-python-template .
+   ```
 3. Do your work
 
 ## Features
 
-
 - [x] Automated changelog with [Conventional Commits] and [Python Semantic Release]
 - [x] Automated dependency updates with [Dependabot]
 - [x] Automated semantic versioning with [Python Semantic Release]
 - [x] Automated uploads to [PyPI] and [TestPyPI]
 - [x] Code coverage with [Pytest-Cov]
 - [x] Code formatting with [Black] and [Prettier]
 - [x] Continuous integration with [GitHub Actions]
```

