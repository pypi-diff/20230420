# Comparing `tmp/giphon-0.1.6.tar.gz` & `tmp/giphon-0.1.7.tar.gz`

## Comparing `giphon-0.1.6.tar` & `giphon-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 giphon-0.1.6/src/giphon/__about__.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 giphon-0.1.6/src/giphon/__init__.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 giphon-0.1.6/src/giphon/__main__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 giphon-0.1.6/src/giphon/git.py
--rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 giphon-0.1.6/src/giphon/gitlab.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 giphon-0.1.6/src/giphon/siphon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 giphon-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 giphon-0.1.6/tests/test_git.py
--rw-r--r--   0        0        0    10343 2020-02-02 00:00:00.000000 giphon-0.1.6/tests/test_gitlab.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 giphon-0.1.6/tests/test_siphon.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 giphon-0.1.6/tests/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 giphon-0.1.6/.gitignore
--rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 giphon-0.1.6/LICENSE
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 giphon-0.1.6/README.md
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 giphon-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 giphon-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 giphon-0.1.7/src/giphon/__about__.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 giphon-0.1.7/src/giphon/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 giphon-0.1.7/src/giphon/__main__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 giphon-0.1.7/src/giphon/git.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 giphon-0.1.7/src/giphon/gitlab.py
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 giphon-0.1.7/src/giphon/siphon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 giphon-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 giphon-0.1.7/tests/test_git.py
+-rw-r--r--   0        0        0    10343 2020-02-02 00:00:00.000000 giphon-0.1.7/tests/test_gitlab.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 giphon-0.1.7/tests/test_siphon.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 giphon-0.1.7/tests/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 giphon-0.1.7/.gitignore
+-rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 giphon-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 giphon-0.1.7/README.md
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 giphon-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 giphon-0.1.7/PKG-INFO
```

### Comparing `giphon-0.1.6/src/giphon/git.py` & `giphon-0.1.7/src/giphon/git.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.6/src/giphon/gitlab.py` & `giphon-0.1.7/src/giphon/gitlab.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         path (Path): the path to save the environment variables to
         element (Union[gitlab.v4.objects.Group, gitlab.v4.objects.Project]):
           The Gitlab group or project to get the environment variables from
         logger (Logger): the logger to use to generate logs
     """
 
     def _save_environment_variable(variable: Variable, env_path: Path) -> None:
-
         scope = variable.environment_scope
 
         key = f'{variable.key}-{scope.replace("*", "STAR").replace("/", "-")}'
 
         with open(os.path.join(env_path, f"{key}"), "w") as f:
             f.write(variable.value)
 
@@ -118,15 +117,14 @@
         archived (bool, optional): Whether to get information from archived
           projects. Defaults to False.
 
     Yields:
         Element: Gitlab group or project to be handled.
     """
     for group in groups:
-
         yield group
 
         yield from flatten_groups_tree(
             groups=[
                 gl.groups.get(subgroup.id)
                 for subgroup in group.subgroups.list(all=True)
             ],
```

### Comparing `giphon-0.1.6/tests/test_git.py` & `giphon-0.1.7/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.6/tests/test_gitlab.py` & `giphon-0.1.7/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.6/tests/test_siphon.py` & `giphon-0.1.7/tests/test_siphon.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,27 +49,27 @@
     Test the main function.
 
     I yet have no idea on how to test the main logic. Should I run an
     e2e test, directly against public gitlab?
     """
 
     with TemporaryDirectory() as temporary_directory:
-
         namespace = Path("gitlab-org/ci-cd/shared-runners")
         output = Path(temporary_directory)
 
         siphon(
             namespace=namespace,
             output=output,
             gitlab_token="",
             gitlab_url="https://gitlab.com",
             fetch_repositories=True,
             save_ci_variables=False,  # Cannot save variables on public repos
             clone_archived=False,
             clone_through_ssh=False,
+            gitlab_username="",
             verbose=False,
         )
 
         print(caplog)
 
         assert os.path.isdir(str(output / namespace / Path("homebrew/.git")))
         assert os.path.isdir(str(output / namespace / Path("macos/.git")))
```

### Comparing `giphon-0.1.6/tests/utils.py` & `giphon-0.1.7/tests/utils.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.6/.gitignore` & `giphon-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `giphon-0.1.6/LICENSE` & `giphon-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `giphon-0.1.6/README.md` & `giphon-0.1.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Logo](https://raw.githubusercontent.com/kabooboo/giphon/0.1.6/docs/assets/logo.png)
+![Logo](https://raw.githubusercontent.com/kabooboo/giphon/0.1.7/docs/assets/logo.png)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/giphon) [![Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://pypi.org/project/black/) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/kabooboo/giphon/test.yml?label=tests)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) ![PyPI](https://img.shields.io/pypi/v/giphon) ![PyPI - License](https://img.shields.io/pypi/l/giphon) ![GitHub Repo stars](https://img.shields.io/github/stars/kabooboo/giphon?style=social)
 
 ---
 
 ✨ Giphon is the contraction of 🦊 _Gitlab_ and 🫗 _siphon_. This CLI tools allows users
 to recursively clone all projects in a given Gitlab group or instance.
@@ -13,15 +13,15 @@
 structure into a directory structure.
 
 Locally cloned projects enable users to use familiar CLI tools such as `grep`
 and `sed` directly into the projects' tree structure.
 
 ## Demo
 
-![Usage GIF](https://raw.githubusercontent.com/kabooboo/giphon/0.1.6/docs/assets/usage.gif)
+![Usage GIF](https://raw.githubusercontent.com/kabooboo/giphon/0.1.7/docs/assets/usage.gif)
 
 ## Installation
 
 To install `giphon`, simply run:
 
 ```shq
 pip install --user giphon
@@ -40,14 +40,19 @@
   instance to clone the repositories from. Defaults to `"https://gitlab.com"`
 - **fetch_repositories**: (CLI: `--fetch-repositories`/`--no-fetch-repositories`):
   Whether to fetch remotes on repositories that already exist.
 - **save_ci_variables**: (CLI: `--save-ci-variables`/`--no-save-ci-variables`):
   Whether to download CI/CD variables to a .env directory.
 - **clone_archived** (CLI: `--clone-archived`/`--no-clone-archived`): Whether
   to also clone archived repository.
+- **clone_through_ssh**: (CLI: `--clone-through-ssh`/`--no-clone-through-ssh`):
+  Whether to use the SSH protocol or the HTTPS protocol to clone the git
+  repositories
+- **gitlab_username** (CLI: `--gitlab-username`, env: `GITLAB_USERNAME`): The
+  username to use, when cloning through HTTPS.
 - **verbose**: (CLI: `--verbose`/`-v`): The level of verbosity
 
 ## Running programmatically
 
 You can import the main function from `giphon` as such:
 
 ```python
```

### Comparing `giphon-0.1.6/pyproject.toml` & `giphon-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `giphon-0.1.6/PKG-INFO` & `giphon-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giphon
-Version: 0.1.6
+Version: 0.1.7
 Summary: Copy locally a Gitlab group or instance
 Project-URL: Bug Reports, https://github.com/kabooboo/giphon/issues
 Project-URL: Documentation, https://github.com/kabooboo/giphon
 Project-URL: Homepage, https://github.com/kabooboo/giphon
 Project-URL: Source Code, https://github.com/kabooboo/giphon
 Author-email: Gabriel Creti <gabrielcreti@gmail.com>
 License-File: LICENSE
@@ -26,15 +26,15 @@
 Requires-Dist: python-gitlab<4,>=3
 Requires-Dist: rich<13,>=12
 Requires-Dist: typer>=0.7
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
-![Logo](https://raw.githubusercontent.com/kabooboo/giphon/0.1.6/docs/assets/logo.png)
+![Logo](https://raw.githubusercontent.com/kabooboo/giphon/0.1.7/docs/assets/logo.png)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/giphon) [![Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://pypi.org/project/black/) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/kabooboo/giphon/test.yml?label=tests)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) ![PyPI](https://img.shields.io/pypi/v/giphon) ![PyPI - License](https://img.shields.io/pypi/l/giphon) ![GitHub Repo stars](https://img.shields.io/github/stars/kabooboo/giphon?style=social)
 
 ---
 
 ✨ Giphon is the contraction of 🦊 _Gitlab_ and 🫗 _siphon_. This CLI tools allows users
 to recursively clone all projects in a given Gitlab group or instance.
@@ -45,15 +45,15 @@
 structure into a directory structure.
 
 Locally cloned projects enable users to use familiar CLI tools such as `grep`
 and `sed` directly into the projects' tree structure.
 
 ## Demo
 
-![Usage GIF](https://raw.githubusercontent.com/kabooboo/giphon/0.1.6/docs/assets/usage.gif)
+![Usage GIF](https://raw.githubusercontent.com/kabooboo/giphon/0.1.7/docs/assets/usage.gif)
 
 ## Installation
 
 To install `giphon`, simply run:
 
 ```shq
 pip install --user giphon
@@ -72,14 +72,19 @@
   instance to clone the repositories from. Defaults to `"https://gitlab.com"`
 - **fetch_repositories**: (CLI: `--fetch-repositories`/`--no-fetch-repositories`):
   Whether to fetch remotes on repositories that already exist.
 - **save_ci_variables**: (CLI: `--save-ci-variables`/`--no-save-ci-variables`):
   Whether to download CI/CD variables to a .env directory.
 - **clone_archived** (CLI: `--clone-archived`/`--no-clone-archived`): Whether
   to also clone archived repository.
+- **clone_through_ssh**: (CLI: `--clone-through-ssh`/`--no-clone-through-ssh`):
+  Whether to use the SSH protocol or the HTTPS protocol to clone the git
+  repositories
+- **gitlab_username** (CLI: `--gitlab-username`, env: `GITLAB_USERNAME`): The
+  username to use, when cloning through HTTPS.
 - **verbose**: (CLI: `--verbose`/`-v`): The level of verbosity
 
 ## Running programmatically
 
 You can import the main function from `giphon` as such:
 
 ```python
```

