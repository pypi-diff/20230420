# Comparing `tmp/makey-cli-1.3.0.tar.gz` & `tmp/makey-cli-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makey-cli-1.3.0.tar", last modified: Wed Apr 19 21:19:36 2023, max compression
+gzip compressed data, was "makey-cli-1.3.1.tar", last modified: Thu Apr 20 15:25:49 2023, max compression
```

## Comparing `makey-cli-1.3.0.tar` & `makey-cli-1.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       66 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.flake8
--rw-r--r--   0        0        0     1193 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.github/workflows/docs-publish.yml
--rw-r--r--   0        0        0     1090 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1303 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      338 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.gitignore
--rw-r--r--   0        0        0      211 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.markdownlint.yaml
--rw-r--r--   0        0        0     1408 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1071 2023-04-19 21:19:27.002957 makey-cli-1.3.0/LICENSE
--rw-r--r--   0        0        0     1764 2023-04-19 21:19:27.002957 makey-cli-1.3.0/README.md
--rw-r--r--   0        0        0      249 2023-04-19 21:19:27.002957 makey-cli-1.3.0/codecov.yml
--rw-r--r--   0        0        0        0 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/.nojekyll
--rw-r--r--   0        0        0      121 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/_404.md
--rw-r--r--   0        0        0      363 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/_coverpage.md
--rw-r--r--   0        0        0     1068 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/_homepage.md
--rw-r--r--   0        0        0      265 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/_sidebar.md
--rw-r--r--   0        0        0     1682 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/changelog.md
--rw-r--r--   0        0        0     1830 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/index.html
--rw-r--r--   0        0        0     1117 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/install.md
--rw-r--r--   0        0        0      309 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/issues.md
--rw-r--r--   0        0        0      402 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/styles.css
--rw-r--r--   0        0        0     1082 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/usage.md
--rw-r--r--   0        0        0      907 2023-04-19 21:19:27.002957 makey-cli-1.3.0/justfile
--rw-r--r--   0        0        0     1040 2023-04-19 21:19:27.002957 makey-cli-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      122 2023-04-19 21:19:27.006957 makey-cli-1.3.0/src/makey/__init__.py
--rw-r--r--   0        0        0     1364 2023-04-19 21:19:27.006957 makey-cli-1.3.0/src/makey/makey.py
--rw-r--r--   0        0        0        0 2023-04-19 21:19:27.006957 makey-cli-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1744 2023-04-19 21:19:27.006957 makey-cli-1.3.0/tests/test_makey.py
--rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 makey-cli-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-04-20 15:25:40.990386 makey-cli-1.3.1/.flake8
+-rw-r--r--   0        0        0     1197 2023-04-20 15:25:40.990386 makey-cli-1.3.1/.github/workflows/docs-publish.yml
+-rw-r--r--   0        0        0     1090 2023-04-20 15:25:40.990386 makey-cli-1.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1303 2023-04-20 15:25:40.990386 makey-cli-1.3.1/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      338 2023-04-20 15:25:40.990386 makey-cli-1.3.1/.gitignore
+-rw-r--r--   0        0        0      211 2023-04-20 15:25:40.990386 makey-cli-1.3.1/.markdownlint.yaml
+-rw-r--r--   0        0        0     1408 2023-04-20 15:25:40.990386 makey-cli-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1071 2023-04-20 15:25:40.990386 makey-cli-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1761 2023-04-20 15:25:40.990386 makey-cli-1.3.1/README.md
+-rw-r--r--   0        0        0      249 2023-04-20 15:25:40.990386 makey-cli-1.3.1/codecov.yml
+-rw-r--r--   0        0        0        0 2023-04-20 15:25:40.990386 makey-cli-1.3.1/docs/.nojekyll
+-rw-r--r--   0        0        0      121 2023-04-20 15:25:40.990386 makey-cli-1.3.1/docs/_404.md
+-rw-r--r--   0        0        0      363 2023-04-20 15:25:40.990386 makey-cli-1.3.1/docs/_coverpage.md
+-rw-r--r--   0        0        0     1068 2023-04-20 15:25:40.990386 makey-cli-1.3.1/docs/_homepage.md
+-rw-r--r--   0        0        0      265 2023-04-20 15:25:40.990386 makey-cli-1.3.1/docs/_sidebar.md
+-rw-r--r--   0        0        0     1827 2023-04-20 15:25:40.990386 makey-cli-1.3.1/docs/changelog.md
+-rw-r--r--   0        0        0     1830 2023-04-20 15:25:40.990386 makey-cli-1.3.1/docs/index.html
+-rw-r--r--   0        0        0     1117 2023-04-20 15:25:40.990386 makey-cli-1.3.1/docs/install.md
+-rw-r--r--   0        0        0      309 2023-04-20 15:25:40.990386 makey-cli-1.3.1/docs/issues.md
+-rw-r--r--   0        0        0      402 2023-04-20 15:25:40.990386 makey-cli-1.3.1/docs/styles.css
+-rw-r--r--   0        0        0     1082 2023-04-20 15:25:40.990386 makey-cli-1.3.1/docs/usage.md
+-rw-r--r--   0        0        0      907 2023-04-20 15:25:40.990386 makey-cli-1.3.1/justfile
+-rw-r--r--   0        0        0     1040 2023-04-20 15:25:40.990386 makey-cli-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-04-20 15:25:40.990386 makey-cli-1.3.1/src/makey/__init__.py
+-rw-r--r--   0        0        0     1493 2023-04-20 15:25:40.990386 makey-cli-1.3.1/src/makey/makey.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:25:40.990386 makey-cli-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1684 2023-04-20 15:25:40.990386 makey-cli-1.3.1/tests/test_makey.py
+-rw-r--r--   0        0        0     2734 1970-01-01 00:00:00.000000 makey-cli-1.3.1/PKG-INFO
```

### Comparing `makey-cli-1.3.0/.github/workflows/docs-publish.yml` & `makey-cli-1.3.1/.github/workflows/docs-publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Simple workflow for deploying static content to GitHub Pages
 name: Deploy Docs to GitHub Pages
 
 on:
-  push:
-    branches: [$default-branch]
+  # push:
+  #   branches: [$default-branch]
   release:
     types: [published]
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 # Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
```

### Comparing `makey-cli-1.3.0/.github/workflows/python-publish.yml` & `makey-cli-1.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `makey-cli-1.3.0/.github/workflows/python-test.yml` & `makey-cli-1.3.1/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `makey-cli-1.3.0/.pre-commit-config.yaml` & `makey-cli-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `makey-cli-1.3.0/LICENSE` & `makey-cli-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `makey-cli-1.3.0/README.md` & `makey-cli-1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 ## Usage
 
 ```zsh
 makey
 ```
 
-New passkey is copied to your clipboard!
+New passkey copied to your clipboard!
 
 > For more usage details, read the **makey-cli** [usage guide](https://boldandbrad.github.io/makey-cli/#/usage).
 
 ## License
 
 Copyright (c) 2021 Bradley Wojcik. Released under the MIT License. See
 [LICENSE](LICENSE) for details.
```

### Comparing `makey-cli-1.3.0/docs/_homepage.md` & `makey-cli-1.3.1/docs/_homepage.md`

 * *Files identical despite different names*

### Comparing `makey-cli-1.3.0/docs/changelog.md` & `makey-cli-1.3.1/docs/changelog.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 The format is based on
 [Keep a Changelog](https://keepachangelog.com/en/1.1.0/ "Keep a Changelog"),
 and this project adheres to
 [Semantic Versioning](https://semver.org/spec/v2.0.0.html "Semantic Versioning").
 
 ## [Unreleased]
 
+## [1.3.1] - 2023-04-20
+
+### Changed
+
+- `makey`: `-h/--help`
+  - Output default value for `--exclude` option.
+  - Consistent output formatting.
+
 ## [1.3.0] - 2023-04-19
 
 ### Added
 
 - `CI` - GitHub Actions CI.
   - `python-test` - Lint and Test package, and publish test coverage to Codecov.
   - `python-publish` - Publish package to PYPI.
```

### Comparing `makey-cli-1.3.0/docs/index.html` & `makey-cli-1.3.1/docs/index.html`

 * *Files identical despite different names*

### Comparing `makey-cli-1.3.0/docs/install.md` & `makey-cli-1.3.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `makey-cli-1.3.0/docs/usage.md` & `makey-cli-1.3.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `makey-cli-1.3.0/justfile` & `makey-cli-1.3.1/justfile`

 * *Files identical despite different names*

### Comparing `makey-cli-1.3.0/pyproject.toml` & `makey-cli-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `makey-cli-1.3.0/src/makey/makey.py` & `makey-cli-1.3.1/src/makey/makey.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import string
 from secrets import choice
 
 import click
 import pyperclip
 
 ALWAYS_EXCLUDE = "\"'"
+COPIED_MESSAGE = "\tNew passkey copied to clipboard!"
 DEFAULT_LENGTH = 16
 
 
 @click.command(help="CLI passkey maker.")
 @click.option(
     "-e",
     "--exclude",
     default="",
     is_flag=False,
-    help="Characters to exclude.",
+    help="Characters to exclude. (default \"')",
 )
 @click.option(
     "-l",
     "--length",
     default=DEFAULT_LENGTH,
     is_flag=False,
-    help="Desired passkey length (default 16).",
+    help="Desired passkey length. (default 16)",
 )
 @click.option(
     "-s",
     "--show",
     default=False,
     is_flag=True,
-    help="Print passkey to stdout - not recommended (default False).",
+    help="Print passkey to stdout. Not recommended. (default False)",
 )
 @click.help_option("-h", "--help")
 @click.version_option(
     None,  # use version auto discovery via setuptools
     "-v",
     "--version",
     package_name="makey-cli",
@@ -49,11 +50,12 @@
 
     # make passkey
     passkey = "".join(choice(characters) for _ in range(length))
 
     # copy passkey to clipboard
     pyperclip.copy(passkey)
 
+    # print passkey to stdout if --show given, otherwise print copy success message
     if show:
         print(passkey)
     else:
-        print("\tNew passkey copied to clipboard!")
+        print(COPIED_MESSAGE)
```

### Comparing `makey-cli-1.3.0/tests/test_makey.py` & `makey-cli-1.3.1/tests/test_makey.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import pyperclip
 from click.testing import CliRunner
 
-from makey.makey import DEFAULT_LENGTH, cli
-
-COPIED_STDOUT = "\tNew passkey copied to clipboard!\n"
+from makey.makey import COPIED_MESSAGE, DEFAULT_LENGTH, cli
 
 
 def test_makey(mocker):
     mocker.patch("pyperclip.copy")
 
     runner = CliRunner()
     result = runner.invoke(cli, [])
 
     assert result.exit_code == 0
     pyperclip.copy.assert_called_once()
-    assert result.stdout == COPIED_STDOUT
+    assert result.stdout.rstrip() == COPIED_MESSAGE
 
 
 def test_makey_default_length(mocker):
     mocker.patch("pyperclip.copy")
 
     runner = CliRunner()
     result = runner.invoke(cli, ["--show"])
@@ -43,15 +41,14 @@
     pyperclip.copy.assert_called_once()
 
     passkey = result.stdout.rstrip()
 
     assert len(passkey) == DEFAULT_LENGTH
     assert "'" not in passkey
     assert '"' not in passkey
-    assert "&" not in passkey
 
 
 def test_makey_length(mocker):
     mocker.patch("pyperclip.copy")
 
     runner = CliRunner()
     result = runner.invoke(cli, ["--show", "-l", 20])
```

### Comparing `makey-cli-1.3.0/PKG-INFO` & `makey-cli-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makey-cli
-Version: 1.3.0
+Version: 1.3.1
 Summary: A simple and lightweight tool for making secure passkeys in your terminal.
 Author-email: Bradley Wojcik <bradleycwojcik@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: click>=8
 Requires-Dist: pyperclip>=1.8
@@ -63,15 +63,15 @@
 
 ## Usage
 
 ```zsh
 makey
 ```
 
-New passkey is copied to your clipboard!
+New passkey copied to your clipboard!
 
 > For more usage details, read the **makey-cli** [usage guide](https://boldandbrad.github.io/makey-cli/#/usage).
 
 ## License
 
 Copyright (c) 2021 Bradley Wojcik. Released under the MIT License. See
 [LICENSE](LICENSE) for details.
```

