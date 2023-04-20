# Comparing `tmp/exasol_toolbox-0.3.0.tar.gz` & `tmp/exasol_toolbox-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_toolbox-0.3.0.tar", max compression
+gzip compressed data, was "exasol_toolbox-0.4.0.tar", max compression
```

## Comparing `exasol_toolbox-0.3.0.tar` & `exasol_toolbox-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0     1063 2022-12-21 13:03:18.675646 exasol_toolbox-0.3.0/LICENSE
--rw-r--r--   0        0        0     1859 2022-12-21 13:03:18.675646 exasol_toolbox-0.3.0/README.rst
--rw-r--r--   0        0        0      629 2022-12-21 13:03:18.675646 exasol_toolbox-0.3.0/doc/changelog.rst
--rw-r--r--   0        0        0        0 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/__init__.py
--rw-r--r--   0        0        0        0 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/nox/__init__.py
--rw-r--r--   0        0        0     8178 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/nox/tasks.py
--rw-r--r--   0        0        0        0 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/pre_commit_hooks/__init__.py
--rw-r--r--   0        0        0     4021 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/pre_commit_hooks/package_version.py
--rw-r--r--   0        0        0      612 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/project.py
--rw-r--r--   0        0        0        0 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/sphinx/__init__.py
--rw-r--r--   0        0        0        0 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/sphinx/github.py
--rw-r--r--   0        0        0      976 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/sphinx/multiversion/__init__.py
--rwxr-xr-x   0        0        0       76 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/sphinx/multiversion/__main__.py
--rw-r--r--   0        0        0     4488 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/sphinx/multiversion/git.py
--rw-r--r--   0        0        0    20685 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/sphinx/multiversion/main.py
--rw-r--r--   0        0        0     8369 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/sphinx/multiversion/sphinx.py
--rw-r--r--   0        0        0      402 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/sphinx/multiversion/templates/multiversion-index.html
--rw-r--r--   0        0        0     1851 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0        0        0      873 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      920 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0        0        0      984 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/refactoring.md
--rw-r--r--   0        0        0     1094 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0        0        0      461 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0        0        0      694 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/actions/python-environment/action.yml
--rw-r--r--   0        0        0      393 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/dependabot.yml
--rw-r--r--   0        0        0      835 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/workflows/build-and-publish.yml
--rw-r--r--   0        0        0      506 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/workflows/check-release-tag.yml
--rw-r--r--   0        0        0     2698 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/workflows/checks.yml
--rw-r--r--   0        0        0      513 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0      395 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/workflows/ci.yml
--rw-r--r--   0        0        0      650 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      292 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/workflows/pr-merge.yml
--rw-r--r--   0        0        0      784 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/.pre-commit-config.yaml
--rw-r--r--   0        0        0      881 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/noxconfig.py
--rw-r--r--   0        0        0      212 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/templates/noxfile.py
--rw-r--r--   0        0        0      233 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/exasol/toolbox/version.py
--rw-r--r--   0        0        0     1968 2022-12-21 13:03:18.679647 exasol_toolbox-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3687 1970-01-01 00:00:00.000000 exasol_toolbox-0.3.0/setup.py
--rw-r--r--   0        0        0     3319 1970-01-01 00:00:00.000000 exasol_toolbox-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-20 07:16:34.026719 exasol_toolbox-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1859 2023-04-20 07:16:34.026719 exasol_toolbox-0.4.0/README.rst
+-rw-r--r--   0        0        0     1098 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/doc/changelog.rst
+-rw-r--r--   0        0        0        0 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/__init__.py
+-rw-r--r--   0        0        0     7139 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/metrics.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/nox/__init__.py
+-rw-r--r--   0        0        0     9781 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/nox/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/pre_commit_hooks/__init__.py
+-rw-r--r--   0        0        0     4021 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/pre_commit_hooks/package_version.py
+-rw-r--r--   0        0        0      612 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/project.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/sphinx/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/sphinx/github.py
+-rw-r--r--   0        0        0      976 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/sphinx/multiversion/__init__.py
+-rwxr-xr-x   0        0        0       76 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/sphinx/multiversion/__main__.py
+-rw-r--r--   0        0        0     4488 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/sphinx/multiversion/git.py
+-rw-r--r--   0        0        0    20685 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/sphinx/multiversion/main.py
+-rw-r--r--   0        0        0     8369 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/sphinx/multiversion/sphinx.py
+-rw-r--r--   0        0        0      402 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/sphinx/multiversion/templates/multiversion-index.html
+-rw-r--r--   0        0        0     1851 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0        0        0      873 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      920 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0        0        0      984 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/refactoring.md
+-rw-r--r--   0        0        0     1094 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0        0        0      461 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0        0        0      694 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/actions/python-environment/action.yml
+-rw-r--r--   0        0        0      393 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/dependabot.yml
+-rw-r--r--   0        0        0      836 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/workflows/build-and-publish.yml
+-rw-r--r--   0        0        0      507 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/workflows/check-release-tag.yml
+-rw-r--r--   0        0        0     2703 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/workflows/checks.yml
+-rw-r--r--   0        0        0      617 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0      497 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      651 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      395 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/workflows/pr-merge.yml
+-rw-r--r--   0        0        0     1526 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/workflows/report.yml
+-rw-r--r--   0        0        0      784 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      881 2023-04-20 07:16:34.030719 exasol_toolbox-0.4.0/exasol/toolbox/templates/noxconfig.py
+-rw-r--r--   0        0        0      212 2023-04-20 07:16:34.034719 exasol_toolbox-0.4.0/exasol/toolbox/templates/noxfile.py
+-rw-r--r--   0        0        0      233 2023-04-20 07:16:34.034719 exasol_toolbox-0.4.0/exasol/toolbox/version.py
+-rw-r--r--   0        0        0     1839 2023-04-20 07:16:34.034719 exasol_toolbox-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 exasol_toolbox-0.4.0/setup.py
+-rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 exasol_toolbox-0.4.0/PKG-INFO
```

### Comparing `exasol_toolbox-0.3.0/LICENSE` & `exasol_toolbox-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/README.rst` & `exasol_toolbox-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/nox/tasks.py` & `exasol_toolbox-0.4.0/exasol/toolbox/nox/tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     "integration_tests",
     "coverage",
     "build_docs",
     "open_docs",
     "clean_docs",
 ]
 
-
 import argparse
 import shutil
 import webbrowser
 from collections import ChainMap
 from enum import (
     Enum,
     auto,
@@ -30,14 +29,19 @@
     Iterable,
     MutableMapping,
 )
 
 import nox
 from nox import Session
 
+from exasol.toolbox.metrics import (
+    Format,
+    create_report,
+    format_report,
+)
 from exasol.toolbox.project import python_files as _python_files
 from noxconfig import (
     PROJECT_CONFIG,
     Config,
 )
 
 _DOCS_OUTPUT_DIR = ".html-documentation"
@@ -267,7 +271,56 @@
 
 @nox.session(name="clean-docs", python=False)
 def clean_docs(_session: Session) -> None:
     """Removes the documentations build folder"""
     docs_folder = PROJECT_CONFIG.root / _DOCS_OUTPUT_DIR
     if docs_folder.exists():
         shutil.rmtree(docs_folder)
+
+
+@nox.session(name="report", python=False)
+def report(session: Session) -> None:
+    """
+    Collects and generates metrics summary for the workspace
+
+    Attention:
+
+        Pre-requisites:
+
+        * Make sure you remove old and outdated artifacts
+            - e.g. by running one of the following commands
+                * :code:`git clean -xdf`
+                * :code:`rm .coverage .lint.txt`
+
+        * Run the following targets:
+            - :code:`nox -s coverage`
+            - :code:`nox -s lint`
+    """
+    formats = tuple(fmt.name.lower() for fmt in Format)
+    usage = "nox -s report -- [options]"
+    parser = argparse.ArgumentParser(
+        description="Generates status report for the project", usage=usage
+    )
+    parser.add_argument(
+        "-f",
+        "--format",
+        type=str,
+        default=formats[0],
+        help="Output format to produce.",
+        choices=formats,
+    )
+    required_files = (
+        PROJECT_CONFIG.root / ".coverage",
+        PROJECT_CONFIG.root / ".lint.txt",
+    )
+    if not all(file.exists() for file in required_files):
+        session.error(
+            "Please make sure you run the `coverage` and the `lint` target first"
+        )
+    sha1 = str(
+        session.run("git", "rev-parse", "HEAD", external=True, silent=True)
+    ).strip()
+    args: argparse.Namespace = parser.parse_args(args=session.posargs)
+    project_report = create_report(commit=sha1)
+    fmt = Format.from_string(args.format)
+
+    print(format_report(project_report, fmt))
```

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/pre_commit_hooks/package_version.py` & `exasol_toolbox-0.4.0/exasol/toolbox/pre_commit_hooks/package_version.py`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/project.py` & `exasol_toolbox-0.4.0/exasol/toolbox/project.py`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/sphinx/multiversion/__init__.py` & `exasol_toolbox-0.4.0/exasol/toolbox/sphinx/multiversion/__init__.py`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/sphinx/multiversion/git.py` & `exasol_toolbox-0.4.0/exasol/toolbox/sphinx/multiversion/git.py`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/sphinx/multiversion/main.py` & `exasol_toolbox-0.4.0/exasol/toolbox/sphinx/multiversion/main.py`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/sphinx/multiversion/sphinx.py` & `exasol_toolbox-0.4.0/exasol/toolbox/sphinx/multiversion/sphinx.py`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/bug.md` & `exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/documentation.md` & `exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/documentation.md`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/feature.md` & `exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/refactoring.md` & `exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/refactoring.md`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/security.md` & `exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/ISSUE_TEMPLATE/security.md`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/actions/python-environment/action.yml` & `exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/actions/python-environment/action.yml`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/workflows/build-and-publish.yml` & `exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/workflows/build-and-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     runs-on: ubuntu-latest
     steps:
 
       - name: SCM Checkout
         uses: actions/checkout@v3
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@main
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.4.0
 
       - name: Build Artifacts
         run: poetry build
 
       - name: PyPi Release
         env:
           POETRY_HTTP_BASIC_PYPI_USERNAME: "__token__"
```

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/workflows/checks.yml` & `exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/workflows/checks.yml`

 * *Files 7% similar despite different names*

```diff
@@ -11,30 +11,30 @@
     steps:
       - name: SCM Checkout
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@main
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.4.0
 
       - name: Check Version(s)
         run: poetry run version-check exasol/toolbox/version.py
 
   build-documentation-job:
     name: Build Documentation
     needs: [version-check-job]
     runs-on: ubuntu-latest
 
     steps:
     - name: SCM Checkout
       uses: actions/checkout@v3
 
     - name: Setup Python & Poetry Environment
-      uses: exasol/python-toolbox/.github/actions/python-environment@main
+      uses: exasol/python-toolbox/.github/actions/python-environment@0.4.0
 
     - name: Build Documentation
       run: |
         poetry run python -m nox -s build-docs
 
   lint-job:
     name: Linting (Python-${{ matrix.python-version }})
@@ -46,15 +46,15 @@
         python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - name: SCM Checkout
         uses: actions/checkout@v3
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@main
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.4.0
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Run Tests
         run: poetry run nox -s lint
 
   type-check-job:
@@ -67,15 +67,15 @@
         python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - name: SCM Checkout
         uses: actions/checkout@v3
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@main
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.4.0
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Run Tests
         run: poetry run nox -s type-check
 
   tests-job:
@@ -89,13 +89,13 @@
         exasol-version: ["7.1.9"]
 
     steps:
       - name: SCM Checkout
         uses: actions/checkout@v3
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@main
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.4.0
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Run Tests
         run: poetry run nox -s coverage -- -- --db-version ${{ matrix.exasol-version }}
```

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/templates/.github/workflows/gh-pages.yml` & `exasol_toolbox-0.4.0/exasol/toolbox/templates/.github/workflows/gh-pages.yml`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     runs-on: ubuntu-latest
 
     steps:
       - name: SCM Checkout
         uses: actions/checkout@v3
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@main
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.4.0
 
       - name: Build Documentation
         run: |
           poetry run python -m nox -s build-docs
 
       - name: Deploy
         uses: JamesIves/github-pages-deploy-action@v4.4.1
```

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/templates/.pre-commit-config.yaml` & `exasol_toolbox-0.4.0/exasol/toolbox/templates/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/exasol/toolbox/templates/noxconfig.py` & `exasol_toolbox-0.4.0/exasol/toolbox/templates/noxconfig.py`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.3.0/pyproject.toml` & `exasol_toolbox-0.4.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "exasol-toolbox"
 packages = [
     { include = "exasol" },
 ]
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = [
     "Nicola Coretti <nicola.coretti@exasol.com>"
 ]
 license = "MIT"
 readme = "README.rst"
 include = [
@@ -31,25 +31,24 @@
 "Source" = "https://github.com/exasol/python-toolbox"
 "Issues" = "https://github.com/exasol/python-toolbox/issues"
 "Changelog" = "https://exasol.github.io/python-toolbox/changelog.html"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nox = "^2022.8.7"
-sphinx = "^5.3.0"
-rich = "^12.6.0"
-pytest = "^7.1.3"
-mypy = ">=0.971,<0.992"
+sphinx = ">=5.3,<7.0"
+rich = "^13.3.2"
+pytest = "^7.2.2"
+mypy = ">=0.971"
 sphinx-copybutton = "^0.5.0"
 furo = "^2022.9.15"
-scriv = ">=0.17,<1.1"
 pyupgrade = ">=2.38.2,<4.0.0"
-black = "^22.8.0"
-isort = "^5.10.1"
-pre-commit = "^2.20.0"
+black = "^23.1.0"
+isort = "^5.12.0"
+pre-commit = "^3.1.1"
 coverage = ">=6.4.4,<8.0.0"
 pylint = "^2.15.4"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
@@ -57,14 +56,15 @@
 
 [tool.poetry.plugins."console_scripts"]
 "sphinx-multiversion" = "exasol.toolbox.sphinx.multiversion.main:main"
 "version-check" = "exasol.toolbox.pre_commit_hooks.package_version:main"
 
 # Tooling
 [tool.coverage.run]
+relative_files = true
 source = [
     "exasol",
 ]
 
 [tool.coverage.report]
 fail_under = 15
 
@@ -77,26 +77,22 @@
 
 [tool.isort]
 profile = "black"
 force_grid_wrap = 2
 
 
 [tool.pylint.master]
-fail-under = 7.8
+fail-under = 7.5
+output-format="colorized,json:.lint.json,text:.lint.txt"
 
 [tool.pylint.format]
 max-line-length = 88
 max-module-lines = 800
 
 
 [[tool.mypy.overrides]]
 module = [
     "exasol.toolbox.sphinx.multiversion.*",
     "test.unit.*",
     "test.integration.*",
 ]
 ignore_errors = true
-
-[tool.scriv]
-new_fragment_template = "file: templates/fragment-template.rst"
-output_file = "doc/changelog.${config:format}"
-version = "literal: pyproject.toml: tool.poetry.version"
```

### Comparing `exasol_toolbox-0.3.0/setup.py` & `exasol_toolbox-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,38 +16,37 @@
  'exasol.toolbox.templates': ['.github/*',
                               '.github/ISSUE_TEMPLATE/*',
                               '.github/PULL_REQUEST_TEMPLATE/*',
                               '.github/actions/python-environment/*',
                               '.github/workflows/*']}
 
 install_requires = \
-['black>=22.8.0,<23.0.0',
+['black>=23.1.0,<24.0.0',
  'coverage>=6.4.4,<8.0.0',
  'furo>=2022.9.15,<2023.0.0',
- 'isort>=5.10.1,<6.0.0',
- 'mypy>=0.971,<0.992',
+ 'isort>=5.12.0,<6.0.0',
+ 'mypy>=0.971',
  'nox>=2022.8.7,<2023.0.0',
- 'pre-commit>=2.20.0,<3.0.0',
+ 'pre-commit>=3.1.1,<4.0.0',
  'pylint>=2.15.4,<3.0.0',
- 'pytest>=7.1.3,<8.0.0',
+ 'pytest>=7.2.2,<8.0.0',
  'pyupgrade>=2.38.2,<4.0.0',
- 'rich>=12.6.0,<13.0.0',
- 'scriv>=0.17,<1.1',
+ 'rich>=13.3.2,<14.0.0',
  'sphinx-copybutton>=0.5.0,<0.6.0',
- 'sphinx>=5.3.0,<6.0.0']
+ 'sphinx>=5.3,<7.0']
 
 entry_points = \
 {'console_scripts': ['sphinx-multiversion = '
                      'exasol.toolbox.sphinx.multiversion.main:main',
                      'version-check = '
                      'exasol.toolbox.pre_commit_hooks.package_version:main']}
 
 setup_kwargs = {
     'name': 'exasol-toolbox',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': '',
     'long_description': 'Exasol Toolbox\n#####################\n\n.. image:: https://img.shields.io/pypi/v/exasol-toolbox\n     :target: https://pypi.org/project/exasol-toolbox/\n     :alt: PyPI Version\n\n.. image:: https://img.shields.io/pypi/pyversions/exasol-toolbox\n    :target: https://pypi.org/project/exasol-toolbox\n    :alt: PyPI - Python Version\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n    :alt: Formatter - Black\n\n.. image:: https://img.shields.io/badge/imports-isort-ef8336.svg\n    :target: https://pycqa.github.io/isort/\n    :alt: Formatter - Isort\n\n.. image:: https://img.shields.io/badge/typing-mypy-blue\n    :target: https://github.com/PyCQA/pylint\n    :alt: Pylint\n\n.. image:: https://img.shields.io/badge/pylint-7.8-green\n    :target: https://github.com/PyCQA/pylint\n    :alt: Pylint\n\n.. image:: https://img.shields.io/pypi/l/exasol-bucketfs\n     :target: https://opensource.org/licenses/MIT\n     :alt: License\n\n.. image:: https://img.shields.io/github/last-commit/nicoretti/python-toolbox\n     :target: https://pypi.org/project/exasol-toolbox/\n     :alt: Last Commit\n\n\n🚀 Features\n------------\n\n* Centrally managed standard tasks\n    - code formatting & upgrading\n    - linting\n    - type-checking\n    - unit-tests\n    - integration-tests\n    - coverage\n    - documentation\n\n* Centrally manged core workflows\n    - workspace/project verification\n    - build and publish releases\n    - build and publish documentation\n\n* Configurable & Extensible\n    - Project configuration\n    - Event hooks\n\n🔌️ Prerequisites\n-----------------\n\n- `Python <https://www.python.org/>`_ >= 3.8\n\n💾 Installation\n----------------\n\n.. code-block:: shell\n\n    pip install exasol-toolbox\n\n📚 Documentation\n----------------\n\nThe latest documentation can be found `here <https://exasol.github.io/python-toolbox/>`_\n',
     'author': 'Nicola Coretti',
     'author_email': 'nicola.coretti@exasol.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `exasol_toolbox-0.3.0/PKG-INFO` & `exasol_toolbox-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: exasol-toolbox
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 License: MIT
 Keywords: nox,tooling,ci,cd,exasol,infrastructure
 Author: Nicola Coretti
 Author-email: nicola.coretti@exasol.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: black (>=22.8.0,<23.0.0)
+Requires-Dist: black (>=23.1.0,<24.0.0)
 Requires-Dist: coverage (>=6.4.4,<8.0.0)
 Requires-Dist: furo (>=2022.9.15,<2023.0.0)
-Requires-Dist: isort (>=5.10.1,<6.0.0)
-Requires-Dist: mypy (>=0.971,<0.992)
+Requires-Dist: isort (>=5.12.0,<6.0.0)
+Requires-Dist: mypy (>=0.971)
 Requires-Dist: nox (>=2022.8.7,<2023.0.0)
-Requires-Dist: pre-commit (>=2.20.0,<3.0.0)
+Requires-Dist: pre-commit (>=3.1.1,<4.0.0)
 Requires-Dist: pylint (>=2.15.4,<3.0.0)
-Requires-Dist: pytest (>=7.1.3,<8.0.0)
+Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: pyupgrade (>=2.38.2,<4.0.0)
-Requires-Dist: rich (>=12.6.0,<13.0.0)
-Requires-Dist: scriv (>=0.17,<1.1)
-Requires-Dist: sphinx (>=5.3.0,<6.0.0)
+Requires-Dist: rich (>=13.3.2,<14.0.0)
+Requires-Dist: sphinx (>=5.3,<7.0)
 Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0)
 Project-URL: Changelog, https://exasol.github.io/python-toolbox/changelog.html
 Project-URL: Documentation, https://exasol.github.io/python-toolbox/
 Project-URL: Homepage, https://www.exasol.com/
 Project-URL: Issues, https://github.com/exasol/python-toolbox/issues
 Project-URL: Source, https://github.com/exasol/python-toolbox
 Description-Content-Type: text/x-rst
```

