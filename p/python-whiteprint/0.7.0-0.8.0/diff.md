# Comparing `tmp/python_whiteprint-0.7.0.tar.gz` & `tmp/python_whiteprint-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_whiteprint-0.7.0.tar", max compression
+gzip compressed data, was "python_whiteprint-0.8.0.tar", max compression
```

## Comparing `python_whiteprint-0.7.0.tar` & `python_whiteprint-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0        0        0        0 2023-04-13 14:51:43.711629 python_whiteprint-0.7.0/LICENSES/
--rw-r--r--   0        0        0     2917 2023-04-13 14:51:43.711629 python_whiteprint-0.7.0/README.md
--rw-r--r--   0        0        0    30179 2023-04-13 14:52:09.680444 python_whiteprint-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      223 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/__init__.py
--rw-r--r--   0        0        0      162 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/__init__.py
--rwxr-xr-x   0        0        0      222 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/__main__.py
--rw-r--r--   0        0        0      786 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/_callback.py
--rw-r--r--   0        0        0      624 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/_click_app.py
--rw-r--r--   0        0        0     1198 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/_logging.py
--rw-r--r--   0        0        0     2130 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/entrypoint.py
--rw-r--r--   0        0        0    16875 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/init.py
--rw-r--r--   0        0        0      417 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/type.py
--rw-r--r--   0        0        0      322 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/console.py
--rw-r--r--   0        0        0     2789 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/git.py
--rw-r--r--   0        0        0      474 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/loc.py
--rw-r--r--   0        0        0      286 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/locale/base.pot
--rw-r--r--   0        0        0      100 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/locale/base.pot.license
--rw-r--r--   0        0        0      420 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/locale/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      100 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/locale/fr_FR/LC_MESSAGES/messages.po.license
--rw-r--r--   0        0        0     3137 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/nox.py
--rw-r--r--   0        0        0      882 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/poetry.py
--rw-r--r--   0        0        0      199 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/py.typed
--rw-r--r--   0        0        0      294 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/version.py
--rw-r--r--   0        0        0     4709 1970-01-01 00:00:00.000000 python_whiteprint-0.7.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-20 15:19:14.678068 python_whiteprint-0.8.0/LICENSES/
+-rw-r--r--   0        0        0     4299 2023-04-20 15:19:14.678068 python_whiteprint-0.8.0/README.md
+-rw-r--r--   0        0        0    30239 2023-04-20 15:19:35.018393 python_whiteprint-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      223 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/__init__.py
+-rw-r--r--   0        0        0      162 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/__init__.py
+-rwxr-xr-x   0        0        0      222 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/__main__.py
+-rw-r--r--   0        0        0      786 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/_callback.py
+-rw-r--r--   0        0        0      624 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/_click_app.py
+-rw-r--r--   0        0        0     1198 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/_logging.py
+-rw-r--r--   0        0        0     2130 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/entrypoint.py
+-rw-r--r--   0        0        0    18375 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/init.py
+-rw-r--r--   0        0        0      417 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/cli/type.py
+-rw-r--r--   0        0        0      322 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/console.py
+-rw-r--r--   0        0        0      912 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/filesystem.py
+-rw-r--r--   0        0        0     5306 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/git.py
+-rw-r--r--   0        0        0      474 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/loc.py
+-rw-r--r--   0        0        0      286 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/locale/base.pot
+-rw-r--r--   0        0        0      100 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/locale/base.pot.license
+-rw-r--r--   0        0        0      420 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/locale/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      100 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/locale/fr_FR/LC_MESSAGES/messages.po.license
+-rw-r--r--   0        0        0     2402 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/nox.py
+-rw-r--r--   0        0        0     1111 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/poetry.py
+-rw-r--r--   0        0        0      199 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/py.typed
+-rw-r--r--   0        0        0      294 2023-04-20 15:19:14.682068 python_whiteprint-0.8.0/src/python_whiteprint/version.py
+-rw-r--r--   0        0        0     6219 1970-01-01 00:00:00.000000 python_whiteprint-0.8.0/PKG-INFO
```

### Comparing `python_whiteprint-0.7.0/pyproject.toml` & `python_whiteprint-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 # SPDX-FileCopyrightText: © 2023 Romain Brault <mail@romainbrault.com>
 #
 # SPDX-License-Identifier: MIT
 
 [tool.poetry]
 name = "python_whiteprint"
-version = "0.7.0"
+version = "0.8.0"
 description = "Generating Python projects using best practices"
 authors = [
     "Romain Brault <mail@romainbrault.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/RomainBrault/python-whiteprint"
 repository = "https://github.com/RomainBrault/python-whiteprint.git"
 documentation = "https://RomainBrault.github.io/python-whiteprint/"
-keywords = ["Python", "Cookiecutter"]
+keywords = [
+    "Python", "Cookiecutter", "copier", "template", "rich", "typer", "nox",
+    "poetry", "beartype", "oci-image", "container", "docker", "podman", "ruff",
+]
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 3 - Alpha",
+    "Environment :: Console",
     "Intended Audience :: Developers",
+    "License :: OSI Approved",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Natural Language :: English",
     "Typing :: Typed",
 ]
 packages = [
     { include =  "python_whiteprint", from = "src" },
 ]
 include = [
     { path = "src/python_whiteprint/locale/**/*.mo", format = ["wheel"] },
 ]
 
 [tool.poetry.dependencies]
 # Some packages, such as scipy, constrain their upper bound of Python versions
 # they support. Without also constraining the upper bound here, Poetry will not
 # select those versions and will result in an old version being
 # resolved/locked.
-python = ">=3.8, <3.12"
+python = ">=3.8, <3.12, !=3.11.0"  # scalene does not support 3.11.0
 rich = ">=12.5.0"
 typer = ">=0.7.0"
 colorama = ">=0.4.3"
 shellingham = ">=1.3.0"
 beartype = ">=0.13.0"
 copier = ">=7.1.0"
 jinja2-time = ">=0.2.0"
 pygit2 = ">=1.11.1"
 python-slugify = ">=8.0.1"
-nox-poetry = ">=1.0.2"
-poetry = ">=1.4.2"
-virtualenv = "=20.16.5"
 typing-extensions = ">=4.5.0"
+platformdirs = ">=3.2.0"
+pygithub = ">=1.58.1"
 
 [tool.poetry.group.localization.dependencies]
 Babel = ">=2.12.0"
 
 [tool.poetry.group.test.dependencies]
 xdoctest = ">=1.1.0"
 hypothesis = ">=6.71.0"
@@ -207,16 +211,14 @@
 filterwarnings = [
     # When running tests, treat warnings as errors (e.g. -Werror). See:
     # https://docs.pytest.org/en/latest/reference/reference.html#confval-filterwarnings
     "error",
     # Add additional warning supressions as needed here. For example, if a
     # third-party library is throwing a deprecation warning that needs to be
     # fixed upstream:
-    "ignore:read_binary is deprecated:DeprecationWarning:",
-    # Concerns only python 3.11. Poetry need to update virtualenv dependency...
 ]
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
```

### Comparing `python_whiteprint-0.7.0/src/python_whiteprint/cli/_callback.py` & `python_whiteprint-0.8.0/src/python_whiteprint/cli/_callback.py`

 * *Files identical despite different names*

### Comparing `python_whiteprint-0.7.0/src/python_whiteprint/cli/_click_app.py` & `python_whiteprint-0.8.0/src/python_whiteprint/cli/_click_app.py`

 * *Files identical despite different names*

### Comparing `python_whiteprint-0.7.0/src/python_whiteprint/cli/_logging.py` & `python_whiteprint-0.8.0/src/python_whiteprint/cli/_logging.py`

 * *Files identical despite different names*

### Comparing `python_whiteprint-0.7.0/src/python_whiteprint/cli/entrypoint.py` & `python_whiteprint-0.8.0/src/python_whiteprint/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `python_whiteprint-0.7.0/src/python_whiteprint/cli/init.py` & `python_whiteprint-0.8.0/src/python_whiteprint/cli/init.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 from typer import params
 from typing_extensions import TypeGuard
 
 from python_whiteprint.loc import _
 
 
 YAML_EXT = [".yaml", ".yml"]
+COPIER_ANSWER_FILE = ".copier-answers.yml"
+LABEL_FILE = ".github/labels.yml"
 
 
 @beartype
 class UnsupportedTypeInMapping(exceptions.UsageError):
     """The given type is not supported."""
 
     def __init__(self) -> None:
@@ -54,14 +56,42 @@
     VIRTUALENV = "VIRTUALENV"
     CONDA = "CONDA"
     MAMBA = "MAMBA"
     VENV = "VENV"
 
 
 @beartype
+def read_yaml(data: pathlib.Path) -> Dict[str, Union[str, int]]:
+    """Read a yaml file.
+
+    Use PyYAML `safe_load`.
+
+    Args:
+        data: path to the YAML file. The file must exists.
+
+    Returns:
+        The content of the YAML file.
+    """
+    if not data.is_file():
+        return {}
+
+    yaml = importlib.import_module("yaml")
+    with data.open("r") as data_file:
+        try:
+            copier_data = yaml.safe_load(data_file)
+        except yaml.parser.ParserError as parser_error:
+            raise NotAValidYAML(data, str(parser_error)) from parser_error
+
+        if _check_dict(copier_data):
+            return copier_data
+
+    raise UnsupportedTypeInMapping
+
+
+@beartype
 def _copy_license_to_project_root(destination: pathlib.Path) -> None:
     """Add the license to the COPYING file.
 
     Forward the license or copyright header from the LICENSE directory to the
     COPYING file.
 
     Args:
@@ -99,15 +129,15 @@
     )
     try:
         nox.run(
             destination=destination,
             args=[
                 "--default-venv-backend",
                 default_venv_backend.value.lower(),
-                *(("--force-python", python) if python is not None else ()),
+                *(("--force-python", python) if python else ()),
                 "--session",
                 "pre-commit",
             ],
         )
     except nox.NoxError as nox_error:
         logger = logging.getLogger(__name__)
         logger.debug(
@@ -136,15 +166,15 @@
         __package__,
     )
     nox.run(
         destination=destination,
         args=[
             "--default-venv-backend",
             default_venv_backend.value.lower(),
-            *(("--force-python", python) if python is not None else ()),
+            *(("--force-python", python) if python else ()),
             "--session",
             "reuse",
             "--",
             "download",
             "--all",
         ],
     )
@@ -155,23 +185,26 @@
 @beartype
 def _post_processing(
     destination: pathlib.Path,
     *,
     default_venv_backend: DefaultVenvBackend,
     skip_tests: bool,
     python: Optional[str],
+    github_token: Optional[str],
 ) -> None:
     """Apply post processing steps after rendering the template wit Copier.
 
     Args:
         destination: path to the python project.
         default_venv_backend: default virtual environment backend for Nox.
         skip_tests: skip the Nox tests step.
         python: force using the given python interpreter for the post
             processing.
+        github_token: Github Token to push the newly created repository to
+            Github. The token must have writing permissions.
     """
     git = importlib.import_module(
         "python_whiteprint.git",
         __package__,
     )
     nox = importlib.import_module(
         "python_whiteprint.nox",
@@ -186,51 +219,64 @@
     poetry.lock(destination)
     repository = git.init_and_commit(destination)
 
     # Download the required licenses.
     _download_licenses(
         destination, default_venv_backend=default_venv_backend, python=python
     )
-    git.add_and_commit(repository, message="chore: maybe download license(s).")
+    git.add_and_commit(repository, message="chore: 📃 download license(s).")
 
     # Generate the dependencies table.
     nox.run(
         destination=destination,
         args=[
             "--default-venv-backend",
             default_venv_backend.value.lower(),
-            *(("--force-python", python) if python is not None else ()),
+            *(("--force-python", python) if python else ()),
             "--session",
             "licenses",
             "--",
             "--from=mixed",
             "--with-urls",
             "--format=markdown",
             "--output-file=DEPENDENCIES.md",
         ],
     )
-    git.add_and_commit(repository, message="docs: add depencencies.")
+    git.add_and_commit(repository, message="docs: 📚 add depencencies.")
 
     # Fixes with pre-commit.
     _format_code(
         destination, default_venv_backend=default_venv_backend, python=python
     )
-    git.add_and_commit(repository, message="chore: format code.")
+    git.add_and_commit(repository, message="chore: 🔨 format code.")
 
     # Check that nox passes.
     if not skip_tests:
         nox.run(
             destination=destination,
             args=[
                 "--default-venv-backend",
                 default_venv_backend.value.lower(),
-                *(("--force-python", python) if python is not None else ()),
+                *(("--force-python", python) if python else ()),
             ],
         )
 
+    if github_token:
+        copier_answers = read_yaml(destination / COPIER_ANSWER_FILE)
+        git.setup_github_repository(
+            repository,
+            project_slug=copier_answers["project_slug"],
+            github_token=github_token,
+            labels=destination / LABEL_FILE,
+        )
+        git.protect_repository(
+            project_slug=copier_answers["project_slug"],
+            github_token=github_token,
+        )
+
 
 @beartype
 def _autocomplete_suffix(incomplete: pathlib.Path) -> List[str]:
     """Autocomplete by listing files with a YAML extension.
 
     Args:
         incomplete: the incomplete argument to complete. Must be a path to a
@@ -445,20 +491,30 @@
     help=_("User data."),
 )
 """see `python_whiteprint.cli.init.init` option `user_data`."""
 _option_python = params.Option(
     os.environ.get("WHITEPRINT_PYTHON"),
     "--python",
     "-p",
+    envvar="WHITEPRINT_PYTHON",
     help=_(
         "force using the given python interpreter for the post processing."
     ),
-    envvar="WHITEPRINT_PYTHON",
 )
 """see `python_whiteprint.cli.init.init` option `python`."""
+_option_github_token = params.Option(
+    os.environ.get("WHITEPRINT_GITHUB_TOKEN"),
+    "--github-token",
+    help=_(
+        "Github Token to push the newly created repository to Github. The"
+        " token must have writing permissions."
+    ),
+    envvar="WHITEPRINT_GITHUB_TOKEN",
+)
+"""see `python_whiteprint.cli.init.init` option `github_token`."""
 
 
 @beartype
 def _check_dict(data: Dict[str, Any]) -> TypeGuard[Dict[str, Union[str, int]]]:
     """Check if the values type of a given dictionary are strings or integers.
 
     Args:
@@ -468,42 +524,14 @@
         a boolean (type guard) indicating whether the values are all strings or
         integers.
     """
     return all(isinstance(v, (str, int)) for v in data.values())
 
 
 @beartype
-def read_yaml(data: pathlib.Path) -> Dict[str, Union[str, int]]:
-    """Read a yaml file.
-
-    Use PyYAML `safe_load`.
-
-    Args:
-        data: path to the YAML file. The file must exists.
-
-    Returns:
-        The content of the YAML file.
-    """
-    if not data.is_file():
-        return {}
-
-    yaml = importlib.import_module("yaml")
-    with data.open("r") as data_file:
-        try:
-            copier_data = yaml.safe_load(data_file)
-        except yaml.parser.ParserError as parser_error:
-            raise NotAValidYAML(data, str(parser_error)) from parser_error
-
-        if _check_dict(copier_data):
-            return copier_data
-
-    raise UnsupportedTypeInMapping
-
-
-@beartype
 def init(  # pylint: disable=too-many-locals
     *,
     destination: pathlib.Path = _argument_destination,
     src_path: str = _option_src_path,
     vcs_ref: Optional[str] = _option_vcs_ref,
     exclude: List[str] = _option_exclude,
     use_prereleases: bool = _option_use_prereleases,
@@ -515,14 +543,15 @@
     quiet: bool = _option_quiet,
     default_venv_backend: DefaultVenvBackend = _option_default_venv_backend,
     skip_tests: bool = _option_skip_tests,
     data: pathlib.Path = _option_data,
     no_data: bool = _option_no_data,
     user_defaults: Optional[pathlib.Path] = _option_user_defaults,
     python: Optional[str] = _option_python,
+    github_token: Optional[str] = _option_github_token,
 ) -> None:
     """Initalize a new Python project.
 
     This command mostly forwards copier's CLI. For more details see
     https://copier.readthedocs.io/en/stable/reference/cli/#copier.cli.CopierApp.
 
     Args:
@@ -548,33 +577,47 @@
         default_venv_backend: default virtual environment backend for Nox.
         skip_tests: skip tests after initializing the repository.
         data: user data used to answer questions.
         no_data: force not using `--data`.
         user_defaults: user defaults choices.
         python: force using the given python interpreter for the post
             processing.
+        github_token: Github Token to push the newly created repository to
+            Github. The token must have writing permissions.
     """
+    data_dict = {} if no_data or data is None else read_yaml(data)
+    data_dict.update(
+        {
+            "git_platform": (
+                "no_git_platform" if github_token is None else "github"
+            )
+        }
+    )
+    user_defaults_dict = (
+        {"project_name": destination.name}
+        if user_defaults is None
+        else read_yaml(user_defaults)
+    )
     importlib.import_module("copier.main").Worker(
         src_path=src_path,
         dst_path=destination,
-        answers_file=".copier-answers.yml",
+        answers_file=COPIER_ANSWER_FILE,
         vcs_ref=vcs_ref,
-        data=({} if no_data or data is None else read_yaml(data)),
+        data=data_dict,
         exclude=exclude,
         use_prereleases=use_prereleases,
         skip_if_exists=skip_if_exists,
         cleanup_on_error=cleanup_on_error,
         defaults=defaults,
-        user_defaults=(
-            {} if user_defaults is None else read_yaml(user_defaults)
-        ),
+        user_defaults=user_defaults_dict,
         overwrite=overwrite,
         pretend=pretend,
         quiet=quiet,
     ).run_copy()
 
     _post_processing(
         destination,
         default_venv_backend=default_venv_backend,
         skip_tests=skip_tests,
         python=python,
+        github_token=github_token,
     )
```

### Comparing `python_whiteprint-0.7.0/PKG-INFO` & `python_whiteprint-0.8.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,295 +1,389 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7468  : 2.1.Name: pyth
 00000020: 6f6e 2d77 6869 7465 7072 696e 740a 5665  on-whiteprint.Ve
-00000030: 7273 696f 6e3a 2030 2e37 2e30 0a53 756d  rsion: 0.7.0.Sum
+00000030: 7273 696f 6e3a 2030 2e38 2e30 0a53 756d  rsion: 0.8.0.Sum
 00000040: 6d61 7279 3a20 4765 6e65 7261 7469 6e67  mary: Generating
 00000050: 2050 7974 686f 6e20 7072 6f6a 6563 7473   Python projects
 00000060: 2075 7369 6e67 2062 6573 7420 7072 6163   using best prac
 00000070: 7469 6365 730a 486f 6d65 2d70 6167 653a  tices.Home-page:
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000090: 636f 6d2f 526f 6d61 696e 4272 6175 6c74  com/RomainBrault
 000000a0: 2f70 7974 686f 6e2d 7768 6974 6570 7269  /python-whitepri
 000000b0: 6e74 0a4c 6963 656e 7365 3a20 4d49 540a  nt.License: MIT.
 000000c0: 4b65 7977 6f72 6473 3a20 5079 7468 6f6e  Keywords: Python
-000000d0: 2c43 6f6f 6b69 6563 7574 7465 720a 4175  ,Cookiecutter.Au
-000000e0: 7468 6f72 3a20 526f 6d61 696e 2042 7261  thor: Romain Bra
-000000f0: 756c 740a 4175 7468 6f72 2d65 6d61 696c  ult.Author-email
-00000100: 3a20 6d61 696c 4072 6f6d 6169 6e62 7261  : mail@romainbra
-00000110: 756c 742e 636f 6d0a 5265 7175 6972 6573  ult.com.Requires
-00000120: 2d50 7974 686f 6e3a 203e 3d33 2e38 2c3c  -Python: >=3.8,<
-00000130: 332e 3132 0a43 6c61 7373 6966 6965 723a  3.12.Classifier:
-00000140: 2044 6576 656c 6f70 6d65 6e74 2053 7461   Development Sta
-00000150: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
-00000160: 6374 696f 6e2f 5374 6162 6c65 0a43 6c61  ction/Stable.Cla
-00000170: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-00000180: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-00000190: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
-000001a0: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
-000001b0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-000001c0: 4d49 5420 4c69 6365 6e73 650a 436c 6173  MIT License.Clas
-000001d0: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
-000001e0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-000001f0: 6e64 6570 656e 6465 6e74 0a43 6c61 7373  ndependent.Class
-00000200: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000220: 7974 686f 6e0a 436c 6173 7369 6669 6572  ython.Classifier
-00000230: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000240: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000250: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
-00000260: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000270: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000280: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
-00000290: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-000002a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002b0: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
-000002c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000002d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002e0: 7468 6f6e 203a 3a20 332e 3130 0a43 6c61  thon :: 3.10.Cla
-000002f0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000300: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000310: 2050 7974 686f 6e20 3a3a 2033 2e31 310a   Python :: 3.11.
-00000320: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000330: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000340: 203a 3a20 5079 7468 6f6e 203a 3a20 330a   :: Python :: 3.
-00000350: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000360: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000370: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
-00000380: 3a3a 204f 6e6c 790a 436c 6173 7369 6669  :: Only.Classifi
-00000390: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-000003a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000003b0: 6f6e 203a 3a20 332e 3130 0a43 6c61 7373  on :: 3.10.Class
-000003c0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000003d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000003e0: 7974 686f 6e20 3a3a 2033 2e31 310a 436c  ython :: 3.11.Cl
-000003f0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000400: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000410: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
-00000420: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000430: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000440: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000450: 390a 436c 6173 7369 6669 6572 3a20 5479  9.Classifier: Ty
-00000460: 7069 6e67 203a 3a20 5479 7065 640a 5265  ping :: Typed.Re
-00000470: 7175 6972 6573 2d44 6973 743a 2062 6561  quires-Dist: bea
-00000480: 7274 7970 6520 283e 3d30 2e31 332e 3029  rtype (>=0.13.0)
-00000490: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000004a0: 636f 6c6f 7261 6d61 2028 3e3d 302e 342e  colorama (>=0.4.
-000004b0: 3329 0a52 6571 7569 7265 732d 4469 7374  3).Requires-Dist
-000004c0: 3a20 636f 7069 6572 2028 3e3d 372e 312e  : copier (>=7.1.
-000004d0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
-000004e0: 3a20 6a69 6e6a 6132 2d74 696d 6520 283e  : jinja2-time (>
-000004f0: 3d30 2e32 2e30 290a 5265 7175 6972 6573  =0.2.0).Requires
-00000500: 2d44 6973 743a 206e 6f78 2d70 6f65 7472  -Dist: nox-poetr
-00000510: 7920 283e 3d31 2e30 2e32 290a 5265 7175  y (>=1.0.2).Requ
-00000520: 6972 6573 2d44 6973 743a 2070 6f65 7472  ires-Dist: poetr
-00000530: 7920 283e 3d31 2e34 2e32 290a 5265 7175  y (>=1.4.2).Requ
-00000540: 6972 6573 2d44 6973 743a 2070 7967 6974  ires-Dist: pygit
-00000550: 3220 283e 3d31 2e31 312e 3129 0a52 6571  2 (>=1.11.1).Req
-00000560: 7569 7265 732d 4469 7374 3a20 7079 7468  uires-Dist: pyth
-00000570: 6f6e 2d73 6c75 6769 6679 2028 3e3d 382e  on-slugify (>=8.
-00000580: 302e 3129 0a52 6571 7569 7265 732d 4469  0.1).Requires-Di
-00000590: 7374 3a20 7269 6368 2028 3e3d 3132 2e35  st: rich (>=12.5
-000005a0: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-000005b0: 743a 2073 6865 6c6c 696e 6768 616d 2028  t: shellingham (
-000005c0: 3e3d 312e 332e 3029 0a52 6571 7569 7265  >=1.3.0).Require
-000005d0: 732d 4469 7374 3a20 7479 7065 7220 283e  s-Dist: typer (>
-000005e0: 3d30 2e37 2e30 290a 5265 7175 6972 6573  =0.7.0).Requires
-000005f0: 2d44 6973 743a 2074 7970 696e 672d 6578  -Dist: typing-ex
-00000600: 7465 6e73 696f 6e73 2028 3e3d 342e 352e  tensions (>=4.5.
-00000610: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
-00000620: 3a20 7669 7274 7561 6c65 6e76 2028 3d3d  : virtualenv (==
-00000630: 3230 2e31 362e 3529 0a50 726f 6a65 6374  20.16.5).Project
-00000640: 2d55 524c 3a20 446f 6375 6d65 6e74 6174  -URL: Documentat
-00000650: 696f 6e2c 2068 7474 7073 3a2f 2f52 6f6d  ion, https://Rom
-00000660: 6169 6e42 7261 756c 742e 6769 7468 7562  ainBrault.github
-00000670: 2e69 6f2f 7079 7468 6f6e 2d77 6869 7465  .io/python-white
-00000680: 7072 696e 742f 0a50 726f 6a65 6374 2d55  print/.Project-U
-00000690: 524c 3a20 5265 706f 7369 746f 7279 2c20  RL: Repository, 
-000006a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000006b0: 6f6d 2f52 6f6d 6169 6e42 7261 756c 742f  om/RomainBrault/
-000006c0: 7079 7468 6f6e 2d77 6869 7465 7072 696e  python-whiteprin
-000006d0: 742e 6769 740a 4465 7363 7269 7074 696f  t.git.Descriptio
-000006e0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000006f0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a3c  text/markdown..<
-00000700: 212d 2d0a 5350 4458 2d46 696c 6543 6f70  !--.SPDX-FileCop
-00000710: 7972 6967 6874 5465 7874 3a20 c2a9 2032  yrightText: .. 2
-00000720: 3032 3320 526f 6d61 696e 2042 7261 756c  023 Romain Braul
-00000730: 7420 3c6d 6169 6c40 726f 6d61 696e 6272  t <mail@romainbr
-00000740: 6175 6c74 2e63 6f6d 3e0a 0a53 5044 582d  ault.com>..SPDX-
-00000750: 4c69 6365 6e73 652d 4964 656e 7469 6669  License-Identifi
-00000760: 6572 3a20 4d49 540a 2d2d 3e0a 0a23 2050  er: MIT.-->..# P
-00000770: 7974 686f 6e20 5768 6974 6570 7269 6e74  ython Whiteprint
-00000780: 0a0a 5b21 5b50 7950 4920 5665 7273 696f  ..[![PyPI Versio
-00000790: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
-000007a0: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-000007b0: 2f70 7974 686f 6e2d 7768 6974 6570 7269  /python-whitepri
-000007c0: 6e74 2e73 7667 295d 2868 7474 7073 3a2f  nt.svg)](https:/
-000007d0: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
-000007e0: 2f70 7970 692f 7079 7468 6f6e 2d77 6869  /pypi/python-whi
-000007f0: 7465 7072 696e 7429 0a5b 215b 446f 6375  teprint).[![Docu
-00000800: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-00000810: 3a2f 2f72 6561 6474 6865 646f 6373 2e6f  ://readthedocs.o
-00000820: 7267 2f70 726f 6a65 6374 732f 7079 7468  rg/projects/pyth
-00000830: 6f6e 2d77 6869 7465 7072 696e 742f 6261  on-whiteprint/ba
-00000840: 6467 652f 3f76 6572 7369 6f6e 3d6c 6174  dge/?version=lat
-00000850: 6573 7429 5d28 6874 7470 733a 2f2f 7079  est)](https://py
-00000860: 7468 6f6e 2d77 6869 7465 7072 696e 742e  thon-whiteprint.
-00000870: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00000880: 6e2f 6c61 7465 7374 2f3f 6261 6467 653d  n/latest/?badge=
-00000890: 6c61 7465 7374 290a 5b21 5b54 6573 7473  latest).[![Tests
-000008a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000008b0: 2e63 6f6d 2f52 6f6d 6169 6e42 7261 756c  .com/RomainBraul
-000008c0: 742f 7079 7468 6f6e 2d77 6869 7465 7072  t/python-whitepr
-000008d0: 696e 742f 6163 7469 6f6e 732f 776f 726b  int/actions/work
-000008e0: 666c 6f77 732f 7465 7374 732e 796d 6c2f  flows/tests.yml/
-000008f0: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
-00000900: 3d6d 6169 6e29 5d28 6874 7470 733a 2f2f  =main)](https://
-00000910: 6769 7468 7562 2e63 6f6d 2f52 6f6d 6169  github.com/Romai
-00000920: 6e42 7261 756c 742f 7079 7468 6f6e 2d77  nBrault/python-w
-00000930: 6869 7465 7072 696e 742f 6163 7469 6f6e  hiteprint/action
-00000940: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
-00000950: 732e 796d 6c29 0a5b 215b 636f 6465 636f  s.yml).[![codeco
-00000960: 765d 2868 7474 7073 3a2f 2f63 6f64 6563  v](https://codec
-00000970: 6f76 2e69 6f2f 6768 2f52 6f6d 6169 6e42  ov.io/gh/RomainB
-00000980: 7261 756c 742f 7079 7468 6f6e 2d77 6869  rault/python-whi
-00000990: 7465 7072 696e 742f 6272 616e 6368 2f6d  teprint/branch/m
-000009a0: 6169 6e2f 6772 6170 682f 6261 6467 652e  ain/graph/badge.
-000009b0: 7376 673f 746f 6b65 6e3d 4753 5953 3756  svg?token=GSYS7V
-000009c0: 5542 3552 295d 2868 7474 7073 3a2f 2f63  UB5R)](https://c
-000009d0: 6f64 6563 6f76 2e69 6f2f 6768 2f52 6f6d  odecov.io/gh/Rom
-000009e0: 6169 6e42 7261 756c 742f 7079 7468 6f6e  ainBrault/python
-000009f0: 2d77 6869 7465 7072 696e 7429 0a5b 215b  -whiteprint).[![
-00000a00: 436f 6465 2073 7479 6c65 3a20 626c 6163  Code style: blac
-00000a10: 6b5d 5b62 6c61 636b 2d62 6164 6765 5d5d  k][black-badge]]
-00000a20: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000a30: 636f 6d2f 7073 662f 626c 6163 6b29 0a5b  com/psf/black).[
-00000a40: 215b 5479 7065 2063 6865 636b 6564 2077  ![Type checked w
-00000a50: 6974 6820 6d79 7079 5d5b 6d79 7079 2d62  ith mypy][mypy-b
-00000a60: 6164 6765 5d5d 2868 7474 7073 3a2f 2f6d  adge]](https://m
-00000a70: 7970 792d 6c61 6e67 2e6f 7267 2f29 0a5b  ypy-lang.org/).[
-00000a80: 215b 7072 652d 636f 6d6d 6974 2065 6e61  ![pre-commit ena
-00000a90: 626c 6564 5d5b 7072 652d 636f 6d6d 6974  bled][pre-commit
-00000aa0: 2062 6164 6765 5d5d 2868 7474 7073 3a2f   badge]](https:/
-00000ab0: 2f70 7265 2d63 6f6d 6d69 742e 636f 6d2f  /pre-commit.com/
-00000ac0: 290a 5b21 5b4c 6963 656e 7365 5d5b 6c69  ).[![License][li
-00000ad0: 6365 6e73 6520 6261 6467 655d 5d28 6874  cense badge]](ht
-00000ae0: 7470 733a 2f2f 6f70 656e 736f 7572 6365  tps://opensource
-00000af0: 2e6f 7267 2f6c 6963 656e 7365 732f 4d49  .org/licenses/MI
-00000b00: 5429 0a5b 215b 436f 6e74 7269 6275 746f  T).[![Contributo
-00000b10: 7220 436f 7665 6e61 6e74 5d5b 636f 6e74  r Covenant][cont
-00000b20: 7269 6275 746f 7220 636f 7665 6e61 6e74  ributor covenant
-00000b30: 2062 6164 6765 5d5d 2868 7474 7073 3a2f   badge]](https:/
-00000b40: 2f77 7777 2e63 6f6e 7472 6962 7574 6f72  /www.contributor
-00000b50: 2d63 6f76 656e 616e 742e 6f72 672f 7665  -covenant.org/ve
-00000b60: 7273 696f 6e2f 322f 312f 636f 6465 5f6f  rsion/2/1/code_o
-00000b70: 665f 636f 6e64 7563 742f 290a 0a5b 626c  f_conduct/)..[bl
-00000b80: 6163 6b2d 6261 6467 655d 3a20 6874 7470  ack-badge]: http
-00000b90: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000ba0: 696f 2f62 6164 6765 2f63 6f64 6525 3230  io/badge/code%20
-00000bb0: 7374 796c 652d 626c 6163 6b2d 3030 3030  style-black-0000
-00000bc0: 3030 2e73 7667 0a5b 6d79 7079 2d62 6164  00.svg.[mypy-bad
-00000bd0: 6765 5d3a 2068 7474 7073 3a2f 2f77 7777  ge]: https://www
-00000be0: 2e6d 7970 792d 6c61 6e67 2e6f 7267 2f73  .mypy-lang.org/s
-00000bf0: 7461 7469 632f 6d79 7079 5f62 6164 6765  tatic/mypy_badge
-00000c00: 2e73 7667 0a5b 7072 652d 636f 6d6d 6974  .svg.[pre-commit
-00000c10: 2062 6164 6765 5d3a 2068 7474 7073 3a2f   badge]: https:/
-00000c20: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000c30: 6261 6467 652f 7072 652d 2d63 6f6d 6d69  badge/pre--commi
-00000c40: 742d 656e 6162 6c65 642d 6272 6967 6874  t-enabled-bright
-00000c50: 6772 6565 6e3f 6c6f 676f 3d70 7265 2d63  green?logo=pre-c
-00000c60: 6f6d 6d69 7426 6c6f 676f 436f 6c6f 723d  ommit&logoColor=
-00000c70: 7768 6974 650a 5b6c 6963 656e 7365 2062  white.[license b
-00000c80: 6164 6765 5d3a 2068 7474 7073 3a2f 2f69  adge]: https://i
-00000c90: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-00000ca0: 7468 7562 2f6c 6963 656e 7365 2f52 6f6d  thub/license/Rom
-00000cb0: 6169 6e42 7261 756c 742f 7079 7468 6f6e  ainBrault/python
-00000cc0: 2d77 6869 7465 7072 696e 740a 5b63 6f6e  -whiteprint.[con
-00000cd0: 7472 6962 7574 6f72 2063 6f76 656e 616e  tributor covenan
-00000ce0: 7420 6261 6467 655d 3a20 6874 7470 733a  t badge]: https:
-00000cf0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000d00: 2f62 6164 6765 2f43 6f6e 7472 6962 7574  /badge/Contribut
-00000d10: 6f72 2532 3043 6f76 656e 616e 742d 322e  or%20Covenant-2.
-00000d20: 312d 3462 6161 6161 2e73 7667 0a0a 436f  1-4baaaa.svg..Co
-00000d30: 6f6b 6965 6375 7474 6572 2074 6f20 6372  okiecutter to cr
-00000d40: 6561 7465 2061 2050 7974 686f 6e20 7061  eate a Python pa
-00000d50: 636b 6167 6520 7573 696e 6720 6d6f 6465  ckage using mode
-00000d60: 726e 2050 7974 686f 6e20 7465 7374 696e  rn Python testin
-00000d70: 672c 0a6c 696e 7469 6e67 2c20 616e 6420  g,.linting, and 
-00000d80: 7479 7065 2063 6865 636b 696e 6720 746f  type checking to
-00000d90: 6f6c 696e 672e 0a0a 2323 2059 6574 2061  oling...## Yet a
-00000da0: 6e6f 7468 6572 2050 7974 686f 6e20 5072  nother Python Pr
-00000db0: 6f6a 6563 7420 636f 6f6b 6965 6375 7474  oject cookiecutt
-00000dc0: 6572 3f0a 0a59 6573 2e0a 0a54 6869 7320  er?..Yes...This 
-00000dd0: 7072 6f6a 6563 7420 6275 696c 6420 7570  project build up
-00000de0: 6f6e 2074 6865 2065 7863 656c 6c65 6e74  on the excellent
-00000df0: 7320 5b63 6f6f 6b69 6563 7574 7465 722d  s [cookiecutter-
-00000e00: 6879 7065 726d 6f64 6572 6e2d 7079 7468  hypermodern-pyth
-00000e10: 6f6e 5d20 6279 0a5b 4063 6a6f 6c6f 7769  on] by.[@cjolowi
-00000e20: 637a 5d28 6874 7470 733a 2f2f 6769 7468  cz](https://gith
-00000e30: 7562 2e63 6f6d 2f63 6a6f 6c6f 7769 637a  ub.com/cjolowicz
-00000e40: 2920 6173 2077 656c 6c20 6173 205b 7079  ) as well as [py
-00000e50: 7468 6f6e 2d62 6c75 6570 7269 6e74 5d20  thon-blueprint] 
-00000e60: 6279 0a5b 406a 6f68 6e74 6861 6765 6e5d  by.[@johnthagen]
-00000e70: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000e80: 636f 6d2f 6a6f 686e 7468 6167 656e 292e  com/johnthagen).
-00000e90: 0a0a 596f 7520 6d69 6768 7420 7761 6e74  ..You might want
-00000ea0: 2074 6f20 6368 6563 6b20 7468 6573 6520   to check these 
-00000eb0: 7072 6f6a 6563 7420 6173 2074 6865 7920  project as they 
-00000ec0: 6d69 6768 7420 6265 206d 6f72 6520 7375  might be more su
-00000ed0: 6974 6564 2074 6f20 796f 7572 0a6e 6565  ited to your.nee
-00000ee0: 6473 2e0a 0a23 2320 4469 6666 6572 656e  ds...## Differen
-00000ef0: 6365 7320 636f 6d70 6172 6564 2074 6f20  ces compared to 
-00000f00: 5b63 6f6f 6b69 6563 7574 7465 722d 6879  [cookiecutter-hy
-00000f10: 7065 726d 6f64 6572 6e2d 7079 7468 6f6e  permodern-python
-00000f20: 5d0a 0a2d 205b 205d 2055 7365 205b 636f  ]..- [ ] Use [co
-00000f30: 7069 6572 5d28 6874 7470 733a 2f2f 636f  pier](https://co
-00000f40: 7069 6572 2e72 6561 6474 6865 646f 6373  pier.readthedocs
-00000f50: 2e69 6f2f 656e 2f6c 6174 6573 742f 2920  .io/en/latest/) 
-00000f60: 696e 7374 6561 6420 6f66 2074 6865 0a20  instead of the. 
-00000f70: 2020 2020 2075 6e6d 6169 6e74 6564 2063       unmainted c
-00000f80: 6f6f 6b69 6563 7574 7465 722c 0a2d 205b  ookiecutter,.- [
-00000f90: 205d 2074 7765 616b 7320 696e 2074 6865   ] tweaks in the
-00000fa0: 2067 656e 6572 6174 6564 2070 726f 6a65   generated proje
-00000fb0: 6374 2028 6e6f 6e20 6578 6861 7573 7469  ct (non exhausti
-00000fc0: 7665 6c79 3a20 434c 4920 7769 7468 2054  vely: CLI with T
-00000fd0: 7970 6572 0a20 2020 2020 2069 6e73 7465  yper.      inste
-00000fe0: 6164 206f 6620 436c 6963 6b2c 2064 796e  ad of Click, dyn
-00000ff0: 616d 6963 2074 7970 6520 6368 6563 6b69  amic type checki
-00001000: 6e67 2077 6974 6820 6265 6172 7479 7065  ng with beartype
-00001010: 2c20 5b61 7574 6f2d 4150 490a 2020 2020  , [auto-API.    
-00001020: 2020 646f 6375 6d65 6e74 6174 696f 6e5d    documentation]
-00001030: 2868 7474 7073 3a2f 2f73 7068 696e 782d  (https://sphinx-
-00001040: 6175 746f 6170 692e 7265 6164 7468 6564  autoapi.readthed
-00001050: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00001060: 2f29 292c 0a2d 205b 205d 206d 616e 6167  /)),.- [ ] manag
-00001070: 6520 6c69 6365 6e73 6573 2077 6974 6820  e licenses with 
-00001080: 5b52 6575 7365 5d28 6874 7470 733a 2f2f  [Reuse](https://
-00001090: 7265 7573 652e 736f 6674 7761 7265 2f29  reuse.software/)
-000010a0: 2c0a 2d20 5b20 5d20 6d6f 7265 2047 6974  ,.- [ ] more Git
-000010b0: 6875 6220 4163 7469 6f6e 7320 616e 6420  hub Actions and 
-000010c0: 436f 6d6d 756e 6974 7920 5374 616e 6461  Community Standa
-000010d0: 7264 7320 616e 6420 436f 6d6d 756e 6974  rds and Communit
-000010e0: 7920 5374 616e 6461 7264 732c 0a2d 205b  y Standards,.- [
-000010f0: 205d 2052 7566 6620 696e 7374 6561 6420   ] Ruff instead 
-00001100: 6f66 2046 6c61 6b65 3820 746f 2066 6978  of Flake8 to fix
-00001110: 2061 206d 6178 696d 756d 206f 6620 636f   a maximum of co
-00001120: 6465 2073 6d65 6c6c 732c 0a2d 205b 205d  de smells,.- [ ]
-00001130: 2073 7472 6963 7420 6c69 6e74 696e 6720   strict linting 
-00001140: 7769 7468 2070 796c 696e 742c 0a2d 205b  with pylint,.- [
-00001150: 205d 204f 4349 2043 6f6e 7461 696e 6572   ] OCI Container
-00001160: 2069 6d61 6765 732c 0a2d 205b 205d 2062   images,.- [ ] b
-00001170: 6173 6963 2047 6974 4c61 6220 7375 7070  asic GitLab supp
-00001180: 6f72 742c 0a2d 205b 205d 204c 6174 6578  ort,.- [ ] Latex
-00001190: 2074 656d 706c 6174 6520 7769 7468 2070   template with p
-000011a0: 7974 686f 6e20 696e 7465 6772 6174 696f  ython integratio
-000011b0: 6e2e 0a0a 5b63 6f6f 6b69 6563 7574 7465  n...[cookiecutte
-000011c0: 722d 6879 7065 726d 6f64 6572 6e2d 7079  r-hypermodern-py
-000011d0: 7468 6f6e 5d3a 2068 7474 7073 3a2f 2f63  thon]: https://c
-000011e0: 6f6f 6b69 6563 7574 7465 722d 6879 7065  ookiecutter-hype
-000011f0: 726d 6f64 6572 6e2d 7079 7468 6f6e 2e72  rmodern-python.r
-00001200: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00001210: 2f32 3032 322e 362e 332e 706f 7374 312f  /2022.6.3.post1/
-00001220: 0a5b 7079 7468 6f6e 2d62 6c75 6570 7269  .[python-bluepri
-00001230: 6e74 5d3a 2068 7474 7073 3a2f 2f67 6974  nt]: https://git
-00001240: 6875 622e 636f 6d2f 6a6f 686e 7468 6167  hub.com/johnthag
-00001250: 656e 2f70 7974 686f 6e2d 626c 7565 7072  en/python-bluepr
-00001260: 696e 740a 0a                             int..
+000000d0: 2c43 6f6f 6b69 6563 7574 7465 722c 636f  ,Cookiecutter,co
+000000e0: 7069 6572 2c74 656d 706c 6174 652c 7269  pier,template,ri
+000000f0: 6368 2c74 7970 6572 2c6e 6f78 2c70 6f65  ch,typer,nox,poe
+00000100: 7472 792c 6265 6172 7479 7065 2c6f 6369  try,beartype,oci
+00000110: 2d69 6d61 6765 2c63 6f6e 7461 696e 6572  -image,container
+00000120: 2c64 6f63 6b65 722c 706f 646d 616e 2c72  ,docker,podman,r
+00000130: 7566 660a 4175 7468 6f72 3a20 526f 6d61  uff.Author: Roma
+00000140: 696e 2042 7261 756c 740a 4175 7468 6f72  in Brault.Author
+00000150: 2d65 6d61 696c 3a20 6d61 696c 4072 6f6d  -email: mail@rom
+00000160: 6169 6e62 7261 756c 742e 636f 6d0a 5265  ainbrault.com.Re
+00000170: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
+00000180: 3d33 2e38 2c20 213d 322e 372e 2a2c 2021  =3.8, !=2.7.*, !
+00000190: 3d33 2e30 2e2a 2c20 213d 332e 312e 2a2c  =3.0.*, !=3.1.*,
+000001a0: 2021 3d33 2e32 2e2a 2c20 213d 332e 332e   !=3.2.*, !=3.3.
+000001b0: 2a2c 2021 3d33 2e34 2e2a 2c20 213d 332e  *, !=3.4.*, !=3.
+000001c0: 352e 2a2c 2021 3d33 2e36 2e2a 2c20 213d  5.*, !=3.6.*, !=
+000001d0: 332e 372e 2a0a 436c 6173 7369 6669 6572  3.7.*.Classifier
+000001e0: 3a20 4465 7665 6c6f 706d 656e 7420 5374  : Development St
+000001f0: 6174 7573 203a 3a20 3320 2d20 416c 7068  atus :: 3 - Alph
+00000200: 610a 436c 6173 7369 6669 6572 3a20 456e  a.Classifier: En
+00000210: 7669 726f 6e6d 656e 7420 3a3a 2043 6f6e  vironment :: Con
+00000220: 736f 6c65 0a43 6c61 7373 6966 6965 723a  sole.Classifier:
+00000230: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
+00000240: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+00000250: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+00000260: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000270: 6f76 6564 0a43 6c61 7373 6966 6965 723a  oved.Classifier:
+00000280: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
+00000290: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+000002a0: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
+000002b0: 6572 3a20 4e61 7475 7261 6c20 4c61 6e67  er: Natural Lang
+000002c0: 7561 6765 203a 3a20 456e 676c 6973 680a  uage :: English.
+000002d0: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
+000002e0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+000002f0: 4f53 2049 6e64 6570 656e 6465 6e74 0a43  OS Independent.C
+00000300: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000310: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000320: 3a3a 2050 7974 686f 6e0a 436c 6173 7369  :: Python.Classi
+00000330: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000340: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000350: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
+00000360: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000370: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000380: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
+00000390: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000003a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000003b0: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
+000003c0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000003d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000003e0: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+000003f0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000400: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000410: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000420: 203a 3a20 4f6e 6c79 0a43 6c61 7373 6966   :: Only.Classif
+00000430: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000440: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000450: 686f 6e20 3a3a 2033 2e31 300a 436c 6173  hon :: 3.10.Clas
+00000460: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000470: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000480: 5079 7468 6f6e 203a 3a20 332e 3131 0a43  Python :: 3.11.C
+00000490: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000004a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000004b0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+000004c0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000004d0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000004e0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000004f0: 2e39 0a43 6c61 7373 6966 6965 723a 2054  .9.Classifier: T
+00000500: 7970 696e 6720 3a3a 2054 7970 6564 0a52  yping :: Typed.R
+00000510: 6571 7569 7265 732d 4469 7374 3a20 6265  equires-Dist: be
+00000520: 6172 7479 7065 2028 3e3d 302e 3133 2e30  artype (>=0.13.0
+00000530: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+00000540: 2063 6f6c 6f72 616d 6120 283e 3d30 2e34   colorama (>=0.4
+00000550: 2e33 290a 5265 7175 6972 6573 2d44 6973  .3).Requires-Dis
+00000560: 743a 2063 6f70 6965 7220 283e 3d37 2e31  t: copier (>=7.1
+00000570: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
+00000580: 743a 206a 696e 6a61 322d 7469 6d65 2028  t: jinja2-time (
+00000590: 3e3d 302e 322e 3029 0a52 6571 7569 7265  >=0.2.0).Require
+000005a0: 732d 4469 7374 3a20 706c 6174 666f 726d  s-Dist: platform
+000005b0: 6469 7273 2028 3e3d 332e 322e 3029 0a52  dirs (>=3.2.0).R
+000005c0: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+000005d0: 6769 7432 2028 3e3d 312e 3131 2e31 290a  git2 (>=1.11.1).
+000005e0: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+000005f0: 7967 6974 6875 6220 283e 3d31 2e35 382e  ygithub (>=1.58.
+00000600: 3129 0a52 6571 7569 7265 732d 4469 7374  1).Requires-Dist
+00000610: 3a20 7079 7468 6f6e 2d73 6c75 6769 6679  : python-slugify
+00000620: 2028 3e3d 382e 302e 3129 0a52 6571 7569   (>=8.0.1).Requi
+00000630: 7265 732d 4469 7374 3a20 7269 6368 2028  res-Dist: rich (
+00000640: 3e3d 3132 2e35 2e30 290a 5265 7175 6972  >=12.5.0).Requir
+00000650: 6573 2d44 6973 743a 2073 6865 6c6c 696e  es-Dist: shellin
+00000660: 6768 616d 2028 3e3d 312e 332e 3029 0a52  gham (>=1.3.0).R
+00000670: 6571 7569 7265 732d 4469 7374 3a20 7479  equires-Dist: ty
+00000680: 7065 7220 283e 3d30 2e37 2e30 290a 5265  per (>=0.7.0).Re
+00000690: 7175 6972 6573 2d44 6973 743a 2074 7970  quires-Dist: typ
+000006a0: 696e 672d 6578 7465 6e73 696f 6e73 2028  ing-extensions (
+000006b0: 3e3d 342e 352e 3029 0a50 726f 6a65 6374  >=4.5.0).Project
+000006c0: 2d55 524c 3a20 446f 6375 6d65 6e74 6174  -URL: Documentat
+000006d0: 696f 6e2c 2068 7474 7073 3a2f 2f52 6f6d  ion, https://Rom
+000006e0: 6169 6e42 7261 756c 742e 6769 7468 7562  ainBrault.github
+000006f0: 2e69 6f2f 7079 7468 6f6e 2d77 6869 7465  .io/python-white
+00000700: 7072 696e 742f 0a50 726f 6a65 6374 2d55  print/.Project-U
+00000710: 524c 3a20 5265 706f 7369 746f 7279 2c20  RL: Repository, 
+00000720: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000730: 6f6d 2f52 6f6d 6169 6e42 7261 756c 742f  om/RomainBrault/
+00000740: 7079 7468 6f6e 2d77 6869 7465 7072 696e  python-whiteprin
+00000750: 742e 6769 740a 4465 7363 7269 7074 696f  t.git.Descriptio
+00000760: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00000770: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a3c  text/markdown..<
+00000780: 212d 2d0a 5350 4458 2d46 696c 6543 6f70  !--.SPDX-FileCop
+00000790: 7972 6967 6874 5465 7874 3a20 c2a9 2032  yrightText: .. 2
+000007a0: 3032 3320 526f 6d61 696e 2042 7261 756c  023 Romain Braul
+000007b0: 7420 3c6d 6169 6c40 726f 6d61 696e 6272  t <mail@romainbr
+000007c0: 6175 6c74 2e63 6f6d 3e0a 0a53 5044 582d  ault.com>..SPDX-
+000007d0: 4c69 6365 6e73 652d 4964 656e 7469 6669  License-Identifi
+000007e0: 6572 3a20 4d49 540a 2d2d 3e0a 0a3c 6831  er: MIT.-->..<h1
+000007f0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000800: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000810: 733a 2f2f 7079 7468 6f6e 2d77 6869 7465  s://python-white
+00000820: 7072 696e 742e 7265 6164 7468 6564 6f63  print.readthedoc
+00000830: 732e 696f 2f22 3e3c 696d 6720 7372 633d  s.io/"><img src=
+00000840: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00000850: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000860: 6f6d 2f52 6f6d 6169 6e42 7261 756c 742f  om/RomainBrault/
+00000870: 7079 7468 6f6e 2d77 6869 7465 7072 696e  python-whiteprin
+00000880: 742f 6d61 696e 2f64 6f63 732f 696d 6167  t/main/docs/imag
+00000890: 6573 2f6c 6f67 6f2e 706e 6722 2061 6c74  es/logo.png" alt
+000008a0: 3d22 7079 7468 6f6e 2077 6869 7465 7072  ="python whitepr
+000008b0: 696e 7422 3e3c 2f61 3e0a 3c2f 6831 3e0a  int"></a>.</h1>.
+000008c0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+000008d0: 223e 0a20 2020 203c 656d 3e50 7974 686f  ">.    <em>Pytho
+000008e0: 6e20 5768 6974 6570 7269 6e74 2c20 6765  n Whiteprint, ge
+000008f0: 6e65 7261 7465 2065 6173 696c 7920 5079  nerate easily Py
+00000900: 7468 6f6e 2070 726f 6a65 6374 7320 7769  thon projects wi
+00000910: 7468 2028 6f70 696e 696f 6e61 7465 6429  th (opinionated)
+00000920: 2062 6573 7420 7072 6163 7469 6365 732e   best practices.
+00000930: 3c2f 656d 3e0a 3c2f 703e 0a3c 7020 616c  </em>.</p>.<p al
+00000940: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000950: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000960: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
+00000970: 2f70 7970 692f 7079 7468 6f6e 2d77 6869  /pypi/python-whi
+00000980: 7465 7072 696e 7422 3e0a 2020 2020 3c69  teprint">.    <i
+00000990: 6d67 2061 6c74 3d22 5079 5049 2220 7372  mg alt="PyPI" sr
+000009a0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000009b0: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+000009c0: 2f70 7974 686f 6e2d 7768 6974 6570 7269  /python-whitepri
+000009d0: 6e74 2e73 7667 222f 3e0a 2020 3c2f 613e  nt.svg"/>.  </a>
+000009e0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+000009f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f52  s://github.com/R
+00000a00: 6f6d 6169 6e42 7261 756c 742f 7079 7468  omainBrault/pyth
+00000a10: 6f6e 2d77 6869 7465 7072 696e 742f 6163  on-whiteprint/ac
+00000a20: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000a30: 7465 7374 732e 796d 6c22 3e0a 2020 2020  tests.yml">.    
+00000a40: 3c69 6d67 2061 6c74 3d22 5079 5049 2220  <img alt="PyPI" 
+00000a50: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00000a60: 6875 622e 636f 6d2f 526f 6d61 696e 4272  hub.com/RomainBr
+00000a70: 6175 6c74 2f70 7974 686f 6e2d 7768 6974  ault/python-whit
+00000a80: 6570 7269 6e74 2f61 6374 696f 6e73 2f77  eprint/actions/w
+00000a90: 6f72 6b66 6c6f 7773 2f74 6573 7473 2e79  orkflows/tests.y
+00000aa0: 6d6c 2f62 6164 6765 2e73 7667 3f62 7261  ml/badge.svg?bra
+00000ab0: 6e63 683d 6d61 696e 222f 3e0a 2020 3c2f  nch=main"/>.  </
+00000ac0: 613e 0a20 203c 6120 6872 6566 3d22 6874  a>.  <a href="ht
+00000ad0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000ae0: 2f67 682f 526f 6d61 696e 4272 6175 6c74  /gh/RomainBrault
+00000af0: 2f70 7974 686f 6e2d 7768 6974 6570 7269  /python-whitepri
+00000b00: 6e74 223e 0a20 2020 203c 696d 6720 616c  nt">.    <img al
+00000b10: 743d 2270 7970 6922 2073 7263 3d22 6874  t="pypi" src="ht
+00000b20: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000b30: 2f67 682f 526f 6d61 696e 4272 6175 6c74  /gh/RomainBrault
+00000b40: 2f70 7974 686f 6e2d 7768 6974 6570 7269  /python-whitepri
+00000b50: 6e74 2f62 7261 6e63 682f 6d61 696e 2f67  nt/branch/main/g
+00000b60: 7261 7068 2f62 6164 6765 2e73 7667 3f74  raph/badge.svg?t
+00000b70: 6f6b 656e 3d47 5359 5337 5655 4235 5222  oken=GSYS7VUB5R"
+00000b80: 2f3e 0a20 203c 2f61 3e0a 2020 3c61 2068  />.  </a>.  <a h
+00000b90: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000ba0: 6875 622e 636f 6d2f 7073 662f 626c 6163  hub.com/psf/blac
+00000bb0: 6b22 3e0a 2020 2020 3c69 6d67 2061 6c74  k">.    <img alt
+00000bc0: 3d22 7079 7069 2220 7372 633d 2268 7474  ="pypi" src="htt
+00000bd0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000be0: 2e69 6f2f 6261 6467 652f 636f 6465 2532  .io/badge/code%2
+00000bf0: 3073 7479 6c65 2d62 6c61 636b 2d30 3030  0style-black-000
+00000c00: 3030 302e 7376 6722 2f3e 0a20 203c 2f61  000.svg"/>.  </a
+00000c10: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
+00000c20: 7073 3a2f 2f6d 7970 792d 6c61 6e67 2e6f  ps://mypy-lang.o
+00000c30: 7267 2f22 3e0a 2020 2020 3c69 6d67 2061  rg/">.    <img a
+00000c40: 6c74 3d22 7079 7069 2220 7372 633d 2268  lt="pypi" src="h
+00000c50: 7474 7073 3a2f 2f77 7777 2e6d 7970 792d  ttps://www.mypy-
+00000c60: 6c61 6e67 2e6f 7267 2f73 7461 7469 632f  lang.org/static/
+00000c70: 6d79 7079 5f62 6164 6765 2e73 7667 222f  mypy_badge.svg"/
+00000c80: 3e0a 2020 3c2f 613e 0a20 203c 6120 6872  >.  </a>.  <a hr
+00000c90: 6566 3d22 6874 7470 733a 2f2f 7072 652d  ef="https://pre-
+00000ca0: 636f 6d6d 6974 2e63 6f6d 2f22 3e0a 2020  commit.com/">.  
+00000cb0: 2020 3c69 6d67 2061 6c74 3d22 7079 7069    <img alt="pypi
+00000cc0: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000cd0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000ce0: 6467 652f 7072 652d 2d63 6f6d 6d69 742d  dge/pre--commit-
+00000cf0: 656e 6162 6c65 642d 6272 6967 6874 6772  enabled-brightgr
+00000d00: 6565 6e3f 6c6f 676f 3d70 7265 2d63 6f6d  een?logo=pre-com
+00000d10: 6d69 7426 6c6f 676f 436f 6c6f 723d 7768  mit&logoColor=wh
+00000d20: 6974 6522 2f3e 0a20 203c 2f61 3e0a 2020  ite"/>.  </a>.  
+00000d30: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000d40: 2f6f 7065 6e73 6f75 7263 652e 6f72 672f  /opensource.org/
+00000d50: 6c69 6365 6e73 6573 2f4d 4954 223e 0a20  licenses/MIT">. 
+00000d60: 2020 203c 696d 6720 616c 743d 2270 7970     <img alt="pyp
+00000d70: 6922 2073 7263 3d22 6874 7470 733a 2f2f  i" src="https://
+00000d80: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+00000d90: 6974 6875 622f 6c69 6365 6e73 652f 526f  ithub/license/Ro
+00000da0: 6d61 696e 4272 6175 6c74 2f70 7974 686f  mainBrault/pytho
+00000db0: 6e2d 7768 6974 6570 7269 6e74 222f 3e0a  n-whiteprint"/>.
+00000dc0: 2020 3c2f 613e 0a20 203c 6120 6872 6566    </a>.  <a href
+00000dd0: 3d22 6874 7470 733a 2f2f 7777 772e 636f  ="https://www.co
+00000de0: 6e74 7269 6275 746f 722d 636f 7665 6e61  ntributor-covena
+00000df0: 6e74 2e6f 7267 2f76 6572 7369 6f6e 2f32  nt.org/version/2
+00000e00: 2f31 2f63 6f64 655f 6f66 5f63 6f6e 6475  /1/code_of_condu
+00000e10: 6374 2f22 3e0a 2020 2020 3c69 6d67 2061  ct/">.    <img a
+00000e20: 6c74 3d22 7079 7069 2220 7372 633d 2268  lt="pypi" src="h
+00000e30: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000e40: 6473 2e69 6f2f 6261 6467 652f 436f 6e74  ds.io/badge/Cont
+00000e50: 7269 6275 746f 7225 3230 436f 7665 6e61  ributor%20Covena
+00000e60: 6e74 2d32 2e31 2d34 6261 6161 612e 7376  nt-2.1-4baaaa.sv
+00000e70: 6722 2f3e 0a20 203c 2f61 3e0a 3c2f 703e  g"/>.  </a>.</p>
+00000e80: 0a0a 2d2d 2d0a 0a2a 2a44 6f63 756d 656e  ..---..**Documen
+00000e90: 7461 7469 6f6e 2a2a 3a20 3c61 2068 7265  tation**: <a hre
+00000ea0: 663d 2268 7474 7073 3a2f 2f70 7974 686f  f="https://pytho
+00000eb0: 6e2d 7768 6974 6570 7269 6e74 2e72 6561  n-whiteprint.rea
+00000ec0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00000ed0: 6174 6573 742f 2220 7461 7267 6574 3d22  atest/" target="
+00000ee0: 5f62 6c61 6e6b 223e 6874 7470 733a 2f2f  _blank">https://
+00000ef0: 7079 7468 6f6e 2d77 6869 7465 7072 696e  python-whiteprin
+00000f00: 742e 7265 6164 7468 6564 6f63 732e 696f  t.readthedocs.io
+00000f10: 2f65 6e2f 6c61 7465 7374 2f3c 2f61 3e0a  /en/latest/</a>.
+00000f20: 0a2a 2a53 6f75 7263 6520 436f 6465 2a2a  .**Source Code**
+00000f30: 3a20 3c61 2068 7265 663d 2268 7474 7073  : <a href="https
+00000f40: 3a2f 2f67 6974 6875 622e 636f 6d2f 526f  ://github.com/Ro
+00000f50: 6d61 696e 4272 6175 6c74 2f70 7974 686f  mainBrault/pytho
+00000f60: 6e2d 7768 6974 6570 7269 6e74 2220 7461  n-whiteprint" ta
+00000f70: 7267 6574 3d22 5f62 6c61 6e6b 223e 6874  rget="_blank">ht
+00000f80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000f90: 2f52 6f6d 6169 6e42 7261 756c 742f 7079  /RomainBrault/py
+00000fa0: 7468 6f6e 2d77 6869 7465 7072 696e 743c  thon-whiteprint<
+00000fb0: 2f61 3e0a 0a2d 2d2d 0a0a 2320 496e 7374  /a>..---..# Inst
+00000fc0: 616c 6c61 7469 6f6e 0a0a 456e 7375 7265  allation..Ensure
+00000fd0: 2074 6861 7420 796f 7520 6861 7665 205b   that you have [
+00000fe0: 6769 745d 2868 7474 7073 3a2f 2f67 6974  git](https://git
+00000ff0: 2d73 636d 2e63 6f6d 2f29 2061 6e64 0a5b  -scm.com/) and.[
+00001000: 7079 7468 6f6e 335d 2868 7474 7073 3a2f  python3](https:/
+00001010: 2f77 7777 2e70 7974 686f 6e2e 6f72 672f  /www.python.org/
+00001020: 2920 696e 7374 616c 6c65 642e 0a0a 5468  ) installed...Th
+00001030: 656e 2069 6e73 7461 6c6c 2074 6865 2072  en install the r
+00001040: 6571 7569 7265 6420 5079 7468 6f6e 2074  equired Python t
+00001050: 6f6f 6c73 3a0a 0a60 6060 636f 6e73 6f6c  ools:..```consol
+00001060: 650a 2420 7079 7468 6f6e 3320 2d6d 2070  e.$ python3 -m p
+00001070: 6970 2069 6e73 7461 6c6c 202d 2d75 7365  ip install --use
+00001080: 7220 2d2d 7570 6772 6164 6520 7069 7078  r --upgrade pipx
+00001090: 0a24 2070 6970 7820 696e 7374 616c 6c20  .$ pipx install 
+000010a0: 706f 6574 7279 0a24 2070 6970 7820 696e  poetry.$ pipx in
+000010b0: 7374 616c 6c20 6e6f 780a 2420 7069 7078  stall nox.$ pipx
+000010c0: 2069 6e6a 6563 7420 6e6f 7820 6e6f 782d   inject nox nox-
+000010d0: 706f 6574 7279 2072 6963 680a 6060 600a  poetry rich.```.
+000010e0: 0a45 7665 6e74 7561 6c6c 7920 696e 7374  .Eventually inst
+000010f0: 616c 6c20 5079 7468 6f6e 2057 6869 7465  all Python White
+00001100: 7072 696e 743a 0a0a 6060 6063 6f6e 736f  print:..```conso
+00001110: 6c65 0a24 2070 6970 7820 696e 7374 616c  le.$ pipx instal
+00001120: 6c20 7079 7468 6f6e 2d77 6869 7465 7072  l python-whitepr
+00001130: 696e 740a 6060 600a 0a23 2045 7861 6d70  int.```..# Examp
+00001140: 6c65 0a0a 4372 6561 7465 2061 206c 6f63  le..Create a loc
+00001150: 616c 2070 726f 6a65 6374 0a0a 6060 6063  al project..```c
+00001160: 6f6e 736f 6c65 0a24 2077 6869 7465 7072  onsole.$ whitepr
+00001170: 696e 7420 696e 6974 203c 6d79 5f70 726f  int init <my_pro
+00001180: 6a65 6374 3e0a 6060 600a 0a43 7265 6174  ject>.```..Creat
+00001190: 6520 6120 4769 7448 7562 2070 726f 6a65  e a GitHub proje
+000011a0: 6374 0a0a 6060 6063 6f6e 736f 6c65 0a24  ct..```console.$
+000011b0: 2077 6869 7465 7072 696e 7420 696e 6974   whiteprint init
+000011c0: 203c 6d79 5f70 726f 6a65 6374 3e20 2d2d   <my_project> --
+000011d0: 6769 7468 7562 2d74 6f6b 656e 203c 6d79  github-token <my
+000011e0: 5f67 6974 6875 625f 746f 6b65 6e3e 0a60  _github_token>.`
+000011f0: 6060 0a0a 4e6f 7465 2074 6861 7420 7468  ``..Note that th
+00001200: 6520 4769 7448 7562 2074 6f6b 656e 206d  e GitHub token m
+00001210: 7573 7420 6861 7665 2072 6570 6f73 6974  ust have reposit
+00001220: 6f72 792c 2077 6f72 6b66 6c6f 7773 2061  ory, workflows a
+00001230: 6e64 2070 6163 6b61 6765 730a 7065 726d  nd packages.perm
+00001240: 6973 7369 6f6e 732e 0a0a 2320 5965 7420  issions...# Yet 
+00001250: 616e 6f74 6865 7220 5079 7468 6f6e 2050  another Python P
+00001260: 726f 6a65 6374 2073 6361 6666 6f6c 642f  roject scaffold/
+00001270: 636f 6f6b 6965 6375 7474 6572 2f67 656e  cookiecutter/gen
+00001280: 6572 6174 6f72 3f0a 0a3c 7020 616c 6967  erator?..<p alig
+00001290: 6e3d 2263 656e 7465 7222 3e3c 656d 3e0a  n="center"><em>.
+000012a0: 5965 732e 0a3c 2f65 6d3e 3c2f 703e 0a0a  Yes..</em></p>..
+000012b0: 5468 6973 2070 726f 6a65 6374 2062 7569  This project bui
+000012c0: 6c64 2075 706f 6e20 7468 6520 6578 6365  ld upon the exce
+000012d0: 6c6c 656e 7473 205b 636f 6f6b 6965 6375  llents [cookiecu
+000012e0: 7474 6572 2d68 7970 6572 6d6f 6465 726e  tter-hypermodern
+000012f0: 2d70 7974 686f 6e5d 2062 790a 5b40 636a  -python] by.[@cj
+00001300: 6f6c 6f77 6963 7a5d 2868 7474 7073 3a2f  olowicz](https:/
+00001310: 2f67 6974 6875 622e 636f 6d2f 636a 6f6c  /github.com/cjol
+00001320: 6f77 6963 7a29 2061 7320 7765 6c6c 2061  owicz) as well a
+00001330: 7320 5b70 7974 686f 6e2d 626c 7565 7072  s [python-bluepr
+00001340: 696e 745d 2062 790a 5b40 6a6f 686e 7468  int] by.[@johnth
+00001350: 6167 656e 5d28 6874 7470 733a 2f2f 6769  agen](https://gi
+00001360: 7468 7562 2e63 6f6d 2f6a 6f68 6e74 6861  thub.com/johntha
+00001370: 6765 6e29 2e0a 0a59 6f75 206d 6967 6874  gen)...You might
+00001380: 2077 616e 7420 746f 2063 6865 636b 2074   want to check t
+00001390: 6865 7365 2070 726f 6a65 6374 7320 6173  hese projects as
+000013a0: 2074 6865 7920 6d69 6768 7420 6265 206d   they might be m
+000013b0: 6f72 6520 7375 6974 6564 2074 6f20 796f  ore suited to yo
+000013c0: 7572 0a6e 6565 6473 2e0a 0a54 6865 2064  ur.needs...The d
+000013d0: 6f63 756d 656e 7461 7469 6f6e 206f 6620  ocumentation of 
+000013e0: 7468 6973 2070 726f 6a65 6374 2069 7320  this project is 
+000013f0: 6865 6176 696c 7920 696e 7370 6972 6564  heavily inspired
+00001400: 2066 726f 6d20 4063 6a6f 6c6f 7769 637a   from @cjolowicz
+00001410: 2773 2077 6f72 6b2e 0a57 6520 616c 736f  's work..We also
+00001420: 2072 6563 6f6d 6d65 6e64 2072 6561 6469   recommend readi
+00001430: 6e67 7320 4063 6a6f 6c6f 7769 637a 2773  ngs @cjolowicz's
+00001440: 205b 6775 6964 6520 6f6e 206d 6f64 6572   [guide on moder
+00001450: 6e20 5079 7468 6f6e 0a74 6f6f 6c69 6e67  n Python.tooling
+00001460: 5d28 6874 7470 733a 2f2f 636a 6f6c 6f77  ](https://cjolow
+00001470: 6963 7a2e 6769 7468 7562 2e69 6f2f 706f  icz.github.io/po
+00001480: 7374 732f 6879 7065 726d 6f64 6572 6e2d  sts/hypermodern-
+00001490: 7079 7468 6f6e 2d30 312d 7365 7475 702f  python-01-setup/
+000014a0: 292e 0a0a 2320 4469 6666 6572 656e 6365  )...# Difference
+000014b0: 7320 636f 6d70 6172 6564 2074 6f20 5b63  s compared to [c
+000014c0: 6f6f 6b69 6563 7574 7465 722d 6879 7065  ookiecutter-hype
+000014d0: 726d 6f64 6572 6e2d 7079 7468 6f6e 5d0a  rmodern-python].
+000014e0: 0a2d 2055 7365 205b 636f 7069 6572 5d28  .- Use [copier](
+000014f0: 6874 7470 733a 2f2f 636f 7069 6572 2e72  https://copier.r
+00001500: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00001510: 2f6c 6174 6573 742f 2920 696e 7374 6561  /latest/) instea
+00001520: 6420 6f66 2074 6865 0a20 2063 6f6f 6b69  d of the.  cooki
+00001530: 6563 7574 7465 7220 7072 6f6a 6563 742c  ecutter project,
+00001540: 0a2d 2074 7765 616b 7320 696e 2074 6865  .- tweaks in the
+00001550: 2067 656e 6572 6174 6564 2070 726f 6a65   generated proje
+00001560: 6374 2028 6e6f 6e20 6578 6861 7573 7469  ct (non exhausti
+00001570: 7665 6c79 3a20 434c 4920 7769 7468 2054  vely: CLI with T
+00001580: 7970 6572 0a20 2069 6e73 7465 6164 206f  yper.  instead o
+00001590: 6620 436c 6963 6b2c 2064 796e 616d 6963  f Click, dynamic
+000015a0: 2074 7970 6520 6368 6563 6b69 6e67 2077   type checking w
+000015b0: 6974 6820 6265 6172 7479 7065 2c20 5b61  ith beartype, [a
+000015c0: 7574 6f2d 4150 490a 2020 646f 6375 6d65  uto-API.  docume
+000015d0: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
+000015e0: 2f73 7068 696e 782d 6175 746f 6170 692e  /sphinx-autoapi.
+000015f0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00001600: 6e2f 6c61 7465 7374 2f29 292c 0a2d 206d  n/latest/)),.- m
+00001610: 616e 6167 6520 6c69 6365 6e73 6573 2077  anage licenses w
+00001620: 6974 6820 5b52 6575 7365 5d28 6874 7470  ith [Reuse](http
+00001630: 733a 2f2f 7265 7573 652e 736f 6674 7761  s://reuse.softwa
+00001640: 7265 2f29 2c0a 2d20 6d6f 7265 2047 6974  re/),.- more Git
+00001650: 6875 6220 4163 7469 6f6e 7320 616e 6420  hub Actions and 
+00001660: 436f 6d6d 756e 6974 7920 5374 616e 6461  Community Standa
+00001670: 7264 7320 616e 6420 436f 6d6d 756e 6974  rds and Communit
+00001680: 7920 5374 616e 6461 7264 732c 0a2d 205b  y Standards,.- [
+00001690: 5275 6666 5d28 6874 7470 733a 2f2f 6265  Ruff](https://be
+000016a0: 7461 2e72 7566 662e 7273 2f64 6f63 732f  ta.ruff.rs/docs/
+000016b0: 2920 696e 7374 6561 6420 6f66 2046 6c61  ) instead of Fla
+000016c0: 6b65 3820 746f 2061 7574 6f2d 6669 7820  ke8 to auto-fix 
+000016d0: 6120 6d61 7869 6d75 6d20 6f66 0a20 2063  a maximum of.  c
+000016e0: 6f64 6520 736d 656c 6c73 2c0a 2d20 7374  ode smells,.- st
+000016f0: 7269 6374 206c 696e 7469 6e67 2077 6974  rict linting wit
+00001700: 6820 5b70 796c 696e 745d 2868 7474 7073  h [pylint](https
+00001710: 3a2f 2f70 796c 696e 742e 7265 6164 7468  ://pylint.readth
+00001720: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00001730: 7374 2f29 2c0a 2d20 4f43 4920 436f 6e74  st/),.- OCI Cont
+00001740: 6169 6e65 7220 696d 6167 6573 2c0a 2d20  ainer images,.- 
+00001750: 6c6f 6361 6c69 7a61 7469 6f6e 2077 6974  localization wit
+00001760: 6820 5b42 6162 656c 5d28 6874 7470 733a  h [Babel](https:
+00001770: 2f2f 6261 6265 6c2e 706f 636f 6f2e 6f72  //babel.pocoo.or
+00001780: 672f 656e 2f6c 6174 6573 742f 696e 6465  g/en/latest/inde
+00001790: 782e 6874 6d6c 292e 0a0a 5b63 6f6f 6b69  x.html)...[cooki
+000017a0: 6563 7574 7465 722d 6879 7065 726d 6f64  ecutter-hypermod
+000017b0: 6572 6e2d 7079 7468 6f6e 5d3a 2068 7474  ern-python]: htt
+000017c0: 7073 3a2f 2f63 6f6f 6b69 6563 7574 7465  ps://cookiecutte
+000017d0: 722d 6879 7065 726d 6f64 6572 6e2d 7079  r-hypermodern-py
+000017e0: 7468 6f6e 2e72 6561 6474 6865 646f 6373  thon.readthedocs
+000017f0: 2e69 6f2f 656e 2f32 3032 322e 362e 332e  .io/en/2022.6.3.
+00001800: 706f 7374 312f 0a5b 7079 7468 6f6e 2d62  post1/.[python-b
+00001810: 6c75 6570 7269 6e74 5d3a 2068 7474 7073  lueprint]: https
+00001820: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a6f  ://github.com/jo
+00001830: 686e 7468 6167 656e 2f70 7974 686f 6e2d  hnthagen/python-
+00001840: 626c 7565 7072 696e 740a 0a              blueprint..
```

