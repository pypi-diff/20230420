# Comparing `tmp/jupyter-analysis-tools-0.1.0.tar.gz` & `tmp/jupyter-analysis-tools-0.1.6.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-analysis-tools-0.1.0.tar", last modified: Thu Nov 10 16:02:36 2022, max compression
+gzip compressed data, was "jupyter-analysis-tools-0.1.6.dev5.tar", last modified: Thu Apr 20 13:42:34 2023, max compression
```

## Comparing `jupyter-analysis-tools-0.1.0.tar` & `jupyter-analysis-tools-0.1.6.dev5.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2022-11-10 16:02:36.919009 jupyter-analysis-tools-0.1.0/
--rw-r--r--   0 ingo       (501) staff       (20)      175 2022-11-09 17:11:43.000000 jupyter-analysis-tools-0.1.0/.coveragerc
--rw-r--r--   0 ingo       (501) staff       (20)      353 2022-10-25 15:24:38.000000 jupyter-analysis-tools-0.1.0/.editorconfig
--rw-r--r--   0 ingo       (501) staff       (20)      642 2022-10-26 15:29:36.000000 jupyter-analysis-tools-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 ingo       (501) staff       (20)      100 2022-10-26 16:51:37.000000 jupyter-analysis-tools-0.1.0/AUTHORS.rst
--rw-r--r--   0 ingo       (501) staff       (20)       88 2022-11-01 15:45:44.000000 jupyter-analysis-tools-0.1.0/CHANGELOG.rst
--rw-r--r--   0 ingo       (501) staff       (20)     2490 2022-11-07 13:26:40.000000 jupyter-analysis-tools-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 ingo       (501) staff       (20)     1107 2022-11-10 12:55:16.000000 jupyter-analysis-tools-0.1.0/LICENSE
--rw-r--r--   0 ingo       (501) staff       (20)      308 2022-11-04 13:04:44.000000 jupyter-analysis-tools-0.1.0/MANIFEST.in
--rw-r--r--   0 ingo       (501) staff       (20)     2385 2022-11-10 16:02:36.918629 jupyter-analysis-tools-0.1.0/PKG-INFO
--rw-r--r--   0 ingo       (501) staff       (20)     2915 2022-11-10 15:49:03.000000 jupyter-analysis-tools-0.1.0/README.rst
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2022-11-10 16:02:36.905233 jupyter-analysis-tools-0.1.0/ci/
--rw-r--r--   0 ingo       (501) staff       (20)     6148 2022-11-04 13:03:38.000000 jupyter-analysis-tools-0.1.0/ci/.DS_Store
--rwxr-xr-x   0 ingo       (501) staff       (20)     3230 2022-11-10 12:55:16.000000 jupyter-analysis-tools-0.1.0/ci/bootstrap.py
--rw-r--r--   0 ingo       (501) staff       (20)       66 2022-11-10 12:55:16.000000 jupyter-analysis-tools-0.1.0/ci/requirements.txt
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2022-11-10 16:02:36.905592 jupyter-analysis-tools-0.1.0/ci/templates/
--rw-r--r--   0 ingo       (501) staff       (20)     6148 2022-11-04 13:03:38.000000 jupyter-analysis-tools-0.1.0/ci/templates/.DS_Store
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2022-11-10 16:02:36.905903 jupyter-analysis-tools-0.1.0/ci/templates/.github/
--rw-r--r--   0 ingo       (501) staff       (20)     6148 2022-11-09 15:57:18.000000 jupyter-analysis-tools-0.1.0/ci/templates/.github/.DS_Store
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2022-11-10 16:02:36.906243 jupyter-analysis-tools-0.1.0/ci/templates/.github/workflows/
--rw-r--r--   0 ingo       (501) staff       (20)     2263 2022-11-10 12:03:38.000000 jupyter-analysis-tools-0.1.0/ci/templates/.github/workflows/tests.yml
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2022-11-10 16:02:36.910175 jupyter-analysis-tools-0.1.0/docs/
--rw-r--r--   0 ingo       (501) staff       (20)       28 2022-10-25 15:24:39.000000 jupyter-analysis-tools-0.1.0/docs/authors.rst
--rw-r--r--   0 ingo       (501) staff       (20)       30 2022-10-25 15:24:39.000000 jupyter-analysis-tools-0.1.0/docs/changelog.rst
--rw-r--r--   0 ingo       (501) staff       (20)     1347 2022-11-07 13:25:07.000000 jupyter-analysis-tools-0.1.0/docs/conf.py
--rw-r--r--   0 ingo       (501) staff       (20)       33 2022-10-25 15:24:38.000000 jupyter-analysis-tools-0.1.0/docs/contributing.rst
--rw-r--r--   0 ingo       (501) staff       (20)      244 2022-10-25 15:24:38.000000 jupyter-analysis-tools-0.1.0/docs/index.rst
--rw-r--r--   0 ingo       (501) staff       (20)      102 2022-10-25 15:24:38.000000 jupyter-analysis-tools-0.1.0/docs/installation.rst
--rw-r--r--   0 ingo       (501) staff       (20)       27 2022-10-25 15:24:39.000000 jupyter-analysis-tools-0.1.0/docs/readme.rst
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2022-11-10 16:02:36.911118 jupyter-analysis-tools-0.1.0/docs/reference/
--rw-r--r--   0 ingo       (501) staff       (20)       74 2022-10-25 15:24:39.000000 jupyter-analysis-tools-0.1.0/docs/reference/index.rst
--rw-r--r--   0 ingo       (501) staff       (20)      158 2022-10-25 15:24:39.000000 jupyter-analysis-tools-0.1.0/docs/reference/jupyter_analysis_tools.rst
--rw-r--r--   0 ingo       (501) staff       (20)       35 2022-11-07 13:19:42.000000 jupyter-analysis-tools-0.1.0/docs/requirements.txt
--rw-r--r--   0 ingo       (501) staff       (20)      109 2022-10-25 15:24:38.000000 jupyter-analysis-tools-0.1.0/docs/spelling_wordlist.txt
--rw-r--r--   0 ingo       (501) staff       (20)       96 2022-10-25 15:24:38.000000 jupyter-analysis-tools-0.1.0/docs/usage.rst
--rw-r--r--   0 ingo       (501) staff       (20)     1751 2022-11-10 16:01:29.000000 jupyter-analysis-tools-0.1.0/pyproject.toml
--rw-r--r--   0 ingo       (501) staff       (20)       38 2022-11-10 16:02:36.919160 jupyter-analysis-tools-0.1.0/setup.cfg
--rwxr-xr-x   0 ingo       (501) staff       (20)     2729 2022-11-10 15:48:19.000000 jupyter-analysis-tools-0.1.0/setup.py
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2022-11-10 16:02:36.900199 jupyter-analysis-tools-0.1.0/src/
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2022-11-10 16:02:36.915089 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/
--rw-r--r--   0 ingo       (501) staff       (20)      485 2022-11-02 16:09:54.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/__init__.py
--rw-r--r--   0 ingo       (501) staff       (20)     1800 2022-10-26 15:32:52.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/analysis.py
--rw-r--r--   0 ingo       (501) staff       (20)     4290 2022-10-26 16:38:59.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/datalocations.py
--rw-r--r--   0 ingo       (501) staff       (20)    16280 2022-11-09 17:00:35.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/distrib.py
--rw-r--r--   0 ingo       (501) staff       (20)     2235 2022-10-26 16:46:00.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/git.py
--rw-r--r--   0 ingo       (501) staff       (20)     1189 2022-10-26 16:10:31.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/notebook_utils.py
--rw-r--r--   0 ingo       (501) staff       (20)     1111 2022-10-26 16:00:25.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/plotting.py
--rw-r--r--   0 ingo       (501) staff       (20)    14663 2022-10-26 16:21:10.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/reBin.py
--rw-r--r--   0 ingo       (501) staff       (20)     1382 2022-10-26 16:01:22.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/readdata.py
--rw-r--r--   0 ingo       (501) staff       (20)     4401 2022-10-26 16:38:59.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/utils.py
--rw-r--r--   0 ingo       (501) staff       (20)     3002 2022-10-26 16:02:48.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/widgets.py
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2022-11-10 16:02:36.917089 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools.egg-info/
--rw-r--r--   0 ingo       (501) staff       (20)     2385 2022-11-10 16:02:36.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools.egg-info/PKG-INFO
--rw-r--r--   0 ingo       (501) staff       (20)     1290 2022-11-10 16:02:36.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 ingo       (501) staff       (20)        1 2022-11-10 16:02:36.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 ingo       (501) staff       (20)        1 2022-11-10 16:02:36.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools.egg-info/not-zip-safe
--rw-r--r--   0 ingo       (501) staff       (20)       23 2022-11-10 16:02:36.000000 jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools.egg-info/top_level.txt
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2022-11-10 16:02:36.917910 jupyter-analysis-tools-0.1.0/tests/
--rw-r--r--   0 ingo       (501) staff       (20)       54 2022-11-09 17:10:11.000000 jupyter-analysis-tools-0.1.0/tests/requirements.txt
--rw-r--r--   0 ingo       (501) staff       (20)      100 2022-11-10 13:00:38.000000 jupyter-analysis-tools-0.1.0/tests/test_jupyter_analysis_tools.py
--rw-r--r--   0 ingo       (501) staff       (20)     2603 2022-11-10 14:37:00.000000 jupyter-analysis-tools-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.329642 jupyter-analysis-tools-0.1.6.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-20 13:42:23.000000 jupyter-analysis-tools-0.1.6.dev5/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-20 13:42:34.329642 jupyter-analysis-tools-0.1.6.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-20 13:42:23.000000 jupyter-analysis-tools-0.1.6.dev5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.321642 jupyter-analysis-tools-0.1.6.dev5/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.313642 jupyter-analysis-tools-0.1.6.dev5/ci/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.317642 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.321642 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/ci-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4495 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.325642 jupyter-analysis-tools-0.1.6.dev5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.325642 jupyter-analysis-tools-0.1.6.dev5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-20 13:42:23.000000 jupyter-analysis-tools-0.1.6.dev5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.325642 jupyter-analysis-tools-0.1.6.dev5/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 13:42:34.329642 jupyter-analysis-tools-0.1.6.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.317642 jupyter-analysis-tools-0.1.6.dev5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.329642 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-20 13:42:23.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/datalocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/distrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/readdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.329642 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-20 13:42:34.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-20 13:42:34.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:42:34.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 13:42:34.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.329642 jupyter-analysis-tools-0.1.6.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/tests/test_jupyter_analysis_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/tox.ini
```

### Comparing `jupyter-analysis-tools-0.1.0/.pre-commit-config.yaml` & `jupyter-analysis-tools-0.1.6.dev5/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # To install the git pre-commit hook run:
 #   pre-commit install
 # To update the pre-commit hooks run:
 #   pre-commit install-hooks
-exclude: '^(\.tox|ci/templates|\.bumpversion\.cfg)(/|$)'
+exclude: '^(\.tox|ci/templates|\.bumpversion\.cfg|testdata|docs/\w+\.xml|\w+\.drawio)(/|$)'
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: debug-statements
-  - repo: https://github.com/timothycrosley/isort
-    rev: 5.10.1
+  - repo: https://github.com/pycqa/isort
+    rev: 5.12.0
     hooks:
       - id: isort
-  - repo: https://github.com/grantjenks/blue
-    rev: v0.9.1
+  - repo: https://github.com/psf/black
+    rev: 23.1.0
     hooks:
-      - id: blue
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+      - id: black
+  - repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
```

### Comparing `jupyter-analysis-tools-0.1.0/CONTRIBUTING.rst` & `jupyter-analysis-tools-0.1.6.dev5/CONTRIBUTING.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Contributions are welcome, and they are greatly appreciated! Every
 little bit helps, and credit will always be given.
 
 Bug reports
 ===========
 
-When `reporting a bug <https://github.com/BAMresearch/jupyter_analysis_tools/issues>`_ please include:
+When `reporting a bug <https://github.com/BAMresearch/jupyter-analysis-tools/issues>`_ please include:
 
     * Your operating system name and version.
     * Any details about your local setup that might be helpful in troubleshooting.
     * Detailed steps to reproduce the bug.
 
 Documentation improvements
 ==========================
@@ -20,40 +20,40 @@
 Jupyter Analysis Tools could always use more documentation, whether as part of the
 official Jupyter Analysis Tools docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Feature requests and feedback
 =============================
 
-The best way to send feedback is to file an issue at https://github.com/BAMresearch/jupyter_analysis_tools/issues.
+The best way to send feedback is to file an issue at https://github.com/BAMresearch/jupyter-analysis-tools/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that code contributions are welcome :)
 
 Development
 ===========
 
-To set up `jupyter_analysis_tools` for local development:
+To set up `jupyter-analysis-tools` for local development:
 
-1. Fork `jupyter_analysis_tools <https://github.com/BAMresearch/jupyter_analysis_tools>`_
+1. Fork `jupyter-analysis-tools <https://github.com/BAMresearch/jupyter-analysis-tools>`_
    (look for the "Fork" button).
 2. Clone your fork locally::
 
-    git clone git@github.com:YOURGITHUBNAME/jupyter_analysis_tools.git
+    git clone git@github.com:YOURGITHUBNAME/jupyter-analysis-tools.git
 
 3. Create a branch for local development::
 
     git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
-4. When you're done making changes run all the checks and docs builder with `tox <https://tox.wiki/en/latest/install.html>`_ one command::
+4. When you're done making changes run all the checks and docs builder with `tox <https://tox.wiki/en/latest/installation.html>`_ one command::
 
     tox
 
 5. Commit your changes and push your branch to GitHub::
 
     git add .
     git commit -m "Your detailed description of your changes."
@@ -66,19 +66,17 @@
 
 If you need some code review or feedback while you're developing the code just make the pull request.
 
 For merging, you should:
 
 1. Include passing tests (run ``tox``).
 2. Update documentation when there's new API, functionality etc.
-3. Add a note to ``CHANGELOG.rst`` about the changes.
+3. Add a note to ``CHANGELOG.md`` about the changes.
 4. Add yourself to ``AUTHORS.rst``.
 
-
-
 Tips
 ----
 
 To run a subset of tests::
 
     tox -e envname -- pytest -k test_myfeature
```

### Comparing `jupyter-analysis-tools-0.1.0/LICENSE` & `jupyter-analysis-tools-0.1.6.dev5/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,9 @@
 MIT License
 
-Copyright (c) 2020 Bundesanstalt für Materialforschung und -prüfung
+Copyright (c) 2018-2023, Ingo Breßler
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice (including the next paragraph) shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `jupyter-analysis-tools-0.1.0/README.rst` & `jupyter-analysis-tools-0.1.6.dev5/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,70 @@
 ========
 Overview
 ========
 
-.. start-badges
-
-|  |docs| |tests| |requires|
-|  |license|
+Yet another Python library with helpers and utilities for data analysis and processing.
 
-.. list-table::
-    :stub-columns: 1
+.. start-badges
 
-    * - docs
-      - |docs|
-    * - tests
-      - | |tests| |requires|
-        |
-    * - package
-      - | |version| |wheel| |supported-versions| |supported-implementations|
-        | |commits-since|
-.. |docs| image:: https://github.com/BAMresearch/jupyter_analysis_tools/actions/workflows/docs.yml/badge.svg
-    :target: https://bamresearch.github.io/jupyter_analysis_tools/
-    :alt: Documentation Status
-
-.. |tests| image:: https://github.com/BAMresearch/jupyter_analysis_tools/actions/workflows/tests.yml/badge.svg
-    :alt: GitHub Actions Build Status
-    :target: https://github.com/BAMresearch/jupyter_analysis_tools/actions
-
-.. |requires| image:: https://requires.io/github/BAMresearch/jupyter_analysis_tools/requirements.svg?branch=main
-    :alt: Requirements Status
-    :target: https://requires.io/github/BAMresearch/jupyter_analysis_tools/requirements/?branch=main
+| |version| |commits-since| |license|
+| |supported-versions| |wheel| |downloads|
+| |cicd| |coverage|
 
 .. |version| image:: https://img.shields.io/pypi/v/jupyter-analysis-tools.svg
-    :alt: PyPI Package latest release
     :target: https://pypi.org/project/jupyter-analysis-tools
+    :alt: PyPI Package latest release
+
+.. |commits-since| image:: https://img.shields.io/github/commits-since/BAMresearch/jupyter-analysis-tools/v0.1.6-dev.5.svg
+    :target: https://github.com/BAMresearch/jupyter-analysis-tools/compare/v0.1.6-dev.5...main
+    :alt: Commits since latest release
 
 .. |license| image:: https://img.shields.io/pypi/l/jupyter-analysis-tools.svg
-    :target: https://pypi.org/project/jupyter-analysis-tools/
+    :target: https://en.wikipedia.org/wiki/MIT_license
     :alt: License
 
-.. |wheel| image:: https://img.shields.io/pypi/wheel/jupyter-analysis-tools.svg
-    :alt: PyPI Wheel
-    :target: https://pypi.org/project/jupyter-analysis-tools
-
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/jupyter-analysis-tools.svg
-    :alt: Supported versions
-    :target: https://pypi.org/project/jupyter-analysis-tools
-
-.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/jupyter-analysis-tools.svg
-    :alt: Supported implementations
     :target: https://pypi.org/project/jupyter-analysis-tools
+    :alt: Supported versions
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/BAMresearch/jupyter_analysis_tools/v0.1.0.svg
-    :alt: Commits since latest release
-    :target: https://github.com/BAMresearch/jupyter_analysis_tools/compare/v0.1.0...main
+.. |wheel| image:: https://img.shields.io/pypi/wheel/jupyter-analysis-tools.svg
+    :target: https://pypi.org/project/jupyter-analysis-tools#files
+    :alt: PyPI Wheel
 
+.. |downloads| image:: https://img.shields.io/pypi/dw/jupyter-analysis-tools.svg
+    :target: https://pypi.org/project/jupyter-analysis-tools/
+    :alt: Weekly PyPI downloads
 
+.. |cicd| image:: https://github.com/BAMresearch/jupyter-analysis-tools/actions/workflows/ci-cd.yml/badge.svg
+    :target: https://github.com/BAMresearch/jupyter-analysis-tools/actions/workflows/ci-cd.yml
+    :alt: Continuous Integration and Deployment Status
+
+.. |coverage| image:: https://img.shields.io/endpoint?url=https://BAMresearch.github.io/jupyter-analysis-tools/coverage-report/cov.json
+    :target: https://BAMresearch.github.io/jupyter-analysis-tools/coverage-report/
+    :alt: Coverage report
 
 .. end-badges
 
-Common Python helpers used in data analysis notebooks (.ipynb) with GIT
-
-* Free software: MIT license
 
 Installation
 ============
 
 ::
 
     pip install jupyter-analysis-tools
 
 You can also install the in-development version with::
 
-    pip install https://github.com/BAMresearch/jupyter_analysis_tools/archive/main.zip
+    pip install git+https://github.com/BAMresearch/jupyter-analysis-tools.git@main
 
 
 Documentation
 =============
 
-https://bamresearch.github.io/jupyter_analysis_tools/
+https://BAMresearch.github.io/jupyter-analysis-tools
 
 Development
 ===========
 
 To run all the tests run::
 
     tox
```

### Comparing `jupyter-analysis-tools-0.1.0/ci/bootstrap.py` & `jupyter-analysis-tools-0.1.6.dev5/ci/update.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,120 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-from __future__ import absolute_import
-from __future__ import print_function
-from __future__ import unicode_literals
-
+# Updates any files with templates in <project root>/ci/templates directory by
+# running 'python3 ci/update.py --no-env'
+# Typically, github workflow files are generated with the help of tox and its config.
 import os
+import pathlib
 import subprocess
 import sys
-from os.path import abspath
-from os.path import dirname
-from os.path import exists
-from os.path import join
-from os.path import relpath
 
-base_path = dirname(dirname(abspath(__file__)))
-templates_path = join(base_path, "ci", "templates")
+import jinja2
+import toml
+import yaml
+
+base_path: pathlib.Path = pathlib.Path(__file__).resolve().parent.parent
+templates_path = base_path / "ci" / "templates"
 
 
 def check_call(args):
     print("+", *args)
     subprocess.check_call(args)
 
 
 def exec_in_env():
-    env_path = join(base_path, ".tox", "bootstrap")
+    env_path = base_path / ".tox" / "bootstrap"
     if sys.platform == "win32":
-        bin_path = join(env_path, "Scripts")
+        bin_path = env_path / "Scripts"
     else:
-        bin_path = join(env_path, "bin")
-    if not exists(env_path):
+        bin_path = env_path / "bin"
+    if not env_path.exists():
         import subprocess
 
         print("Making bootstrap env in: {0} ...".format(env_path))
         try:
             check_call([sys.executable, "-m", "venv", env_path])
         except subprocess.CalledProcessError:
             try:
                 check_call([sys.executable, "-m", "virtualenv", env_path])
             except subprocess.CalledProcessError:
                 check_call(["virtualenv", env_path])
         print("Installing `jinja2` into bootstrap environment...")
-        check_call([join(bin_path, "pip"), "install", "jinja2", "tox"])
-    python_executable = join(bin_path, "python")
-    if not os.path.exists(python_executable):
-        python_executable += '.exe'
+        check_call([bin_path / "pip", "install", "jinja2", "tox"])
+    python_executable = bin_path / "python"
+    if not python_executable.exists():
+        python_executable = python_executable.with_suffix(".exe")
 
     print("Re-executing with: {0}".format(python_executable))
     print("+ exec", python_executable, __file__, "--no-env")
     os.execv(python_executable, [python_executable, __file__, "--no-env"])
 
 
-def main():
-    import jinja2
+def loadYaml(filepath: pathlib.Path):
+    if not filepath.is_file():
+        return {}
+    with open(filepath, "r") as fh:
+        try:
+            return yaml.safe_load(fh)
+        except yaml.YAMLError as exc:
+            print(exc)
+            return {}
 
+
+def main():
     print("Project path: {0}".format(base_path))
+    # use pyproject.toml as source for paths and urls
+    project_meta = toml.load(base_path / "pyproject.toml")
+    # use cookiecutter cfg to file template params not rendered yet
+    cc = loadYaml(base_path / ".cookiecutterrc")
+    pypi_host = cc.get("default_context", {}).get("pypi_host", "").split(".")[:-1]
 
     jinja = jinja2.Environment(
-        loader=jinja2.FileSystemLoader(templates_path),
+        loader=jinja2.FileSystemLoader(str(templates_path)),
         trim_blocks=True,
         lstrip_blocks=True,
         keep_trailing_newline=True,
     )
 
     tox_environments = [
         line.strip()
         # 'tox' need not be installed globally, but must be importable
         # by the Python that is running this script.
-        # This uses sys.executable the same way that the call in
-        # cookiecutter-pylibrary/hooks/post_gen_project.py
-        # invokes this bootstrap.py itself.
         for line in subprocess.check_output(
-            [sys.executable, '-m', 'tox', '--listenvs'], universal_newlines=True
+            [sys.executable, "-m", "tox", "--listenvs"], universal_newlines=True
         ).splitlines()
     ]
-    tox_environments = [line for line in tox_environments if line.startswith('py')]
+    # add a version number to the generic Python3 name (just 'py') for templates to build ok
+    tox_environments = [
+        (line if len(line) > 2 else line + "".join(sys.version.split(".")[:2]))
+        for line in tox_environments
+        if line.startswith("py")
+    ]
 
-    for root, _, files in os.walk(templates_path):
-        for name in files:
-            if name == ".DS_Store":
-                continue
-            relative = relpath(root, templates_path)
-            with open(join(base_path, relative, name), "w") as fh:
-                fh.write(
-                    jinja.get_template(join(relative, name)).render(
-                        tox_environments=tox_environments
-                    )
+    for template in templates_path.rglob("*"):
+        if template.is_file() and template.name != ".DS_Store":
+            template_path = str(template.relative_to(templates_path))
+            destination = base_path / template_path
+            destination.parent.mkdir(parents=True, exist_ok=True)
+            destination.write_text(
+                jinja.get_template(template_path).render(
+                    tox_environments=tox_environments,
+                    docs_url=project_meta["project"]["urls"]["documentation"],
+                    cov_report_path=project_meta["tool"]["coverage"]["report"]["path"],
+                    # Python version to use for general tasks: docs (when tox did not set one)
+                    py_ver=".".join(sys.version.split(".")[:2]),
+                    pypi_token=(
+                        "_".join(pypi_host + ["token"]).upper()
+                        if len(pypi_host)
+                        else "TEST_PYPI_TOKEN"
+                    ),
+                    pypi_repo="".join(pypi_host) if len(pypi_host) else "testpypi",
                 )
-            print("Wrote {}".format(name))
+            )
+            print("Wrote {}".format(template_path))
     print("DONE.")
 
 
 if __name__ == "__main__":
     args = sys.argv[1:]
     if args == ["--no-env"]:
         main()
```

### Comparing `jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/analysis.py` & `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/analysis.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,30 +7,33 @@
 # from https://stackoverflow.com/a/22357811
 # and https://github.com/joferkington/oost_paper_code/blob/master/utilities.py#L167
 # (code with MIT License)
 def getModZScore(points):
     """
     Returns a boolean array with True if points are outliers and False
     otherwise.
-    Note: Similar to https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.zscore.html
-          but using the median instead of the mean.
-    Parameters:
-    -----------
-        points : An numobservations by numdimensions array of observations
-        thresh : The modified z-score to use as a threshold. Observations with
-            a modified z-score (based on the median absolute deviation) greater
-            than this value will be classified as outliers.
-    Returns:
-    --------
-        mask : A numobservations-length boolean array.
-    References:
+    **Note**:
+    Similar to https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.zscore.html
+    but uses the median instead of the mean.
+
+    :param points: An numobservations by numdimensions array of observations
+    :param thresh: The modified z-score to use as a threshold. Observations with
+        a modified z-score (based on the median absolute deviation) greater
+        than this value will be classified as outliers.
+
+    Returns
+    -------
+    mask: numpy array
+        A numobservations-length boolean array.
+
+    References
     ----------
-        Boris Iglewicz and David Hoaglin (1993), "Volume 16: How to Detect and
-        Handle Outliers", The ASQC Basic References in Quality Control:
-        Statistical Techniques, Edward F. Mykytka, Ph.D., Editor.
+    Boris Iglewicz and David Hoaglin (1993), "Volume 16: How to Detect and
+    Handle Outliers", The ASQC Basic References in Quality Control:
+    Statistical Techniques, Edward F. Mykytka, Ph.D., Editor.
     """
     if len(points.shape) == 1:
         points = points[:, None]
     median = np.median(points, axis=0)
     diff = np.sqrt(np.sum((points - median) ** 2, axis=-1))
     med_abs_deviation = np.median(diff)
```

### Comparing `jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/datalocations.py` & `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/datalocations.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 
 import glob
 import os
 import shutil
 import tempfile
 from pathlib import Path
 
-from .utils import indent
-from .utils import isList
+from .utils import indent, isList
 
 
 def getWorkDir(workDir=None, skip=False):
     """Find a local work dir for temporary files, created during analysis.
     The default is *$HOME/data*."""
-    if skip:   # stay in the current directory if desired
-        return os.path.abspath('.')
+    if skip:  # stay in the current directory if desired
+        return os.path.abspath(".")
     if not workDir or not len(workDir):
-        workDir = Path.home() / 'data'
+        workDir = Path.home() / "data"
     else:
         workDir = Path(workDir).resolve()
     if not workDir.is_dir():
         os.mkdir(workDir)
     print("Using '{}' as working directory.".format(workDir))
     return workDir
 
@@ -32,61 +31,70 @@
     # source dir has to exist
     if not os.path.isdir(srcDir):
         raise RuntimeError("Provided source directory '{}' not found!".format(srcDir))
     srcDir = os.path.realpath(srcDir)
     # no separate work dir requested?
     if os.path.samefile(workDir, os.getcwd()):
         print("Working in current directory '{}'.".format(os.getcwd()))
-        return srcDir   # nothing to do
-    prefix = os.path.basename(srcDir) + '_'
-    if useExisting:   # use an existing work dir, avoid copying
-        dirs = glob.glob(os.path.join(workDir, prefix + '*'))
+        return srcDir  # nothing to do
+    prefix = os.path.basename(srcDir) + "_"
+    if useExisting:  # use an existing work dir, avoid copying
+        dirs = glob.glob(os.path.join(workDir, prefix + "*"))
         if len(dirs):
-            return dirs[0]   # use the first match
-        print('No existing work dir found, creating a new one.')
+            return dirs[0]  # use the first match
+        print("No existing work dir found, creating a new one.")
     # copy all data from src dir to a newly created work dir
     workDir = tempfile.mkdtemp(dir=workDir, prefix=prefix)
-    print('Copying data to {}:'.format(workDir))
+    print("Copying data to {}:".format(workDir))
     for dn in os.listdir(srcDir):
         srcPath = os.path.join(srcDir, dn)
         dstPath = os.path.join(workDir, dn)
         if os.path.isdir(srcPath):
             shutil.copytree(srcPath, dstPath)
             print(indent, dn)
         if os.path.isfile(srcPath):
             shutil.copy(srcPath, dstPath)
             print(indent, dn)
-    print('Done preparing work dir.')
+    print("Done preparing work dir.")
     return workDir
 
 
 def printFileList(fnlst, numParts=2, limit=20):
     def printlst(lst):
         return [print(indent, fn) for fn in lst]
 
     def shorten(lst):
         return [os.path.join(*Path(fn).parts[-numParts:]) for fn in lst]
 
     if len(fnlst) > limit:
         printlst(shorten(fnlst[:3]))
-        print(indent, '[...]')
+        print(indent, "[...]")
         printlst(shorten(fnlst[-3:]))
     else:
         printlst(shorten(fnlst))
 
 
 def getDataDirs(dataDir, noWorkDir=False, reuseWorkDir=True, workDir=None):
     """Create a local work dir with a copy of the input data and for storing the results.
     (Data might reside in synced folders which creates massive traffic once batch processing
     results get replaced repeately.)
-    Returns a list of absolute directory paths.
-    *noWorkDir*: False: Copy input data to a new working dir (default),
-                 True: otherwise, use data where it is.
-    *reuseWorkDir*: False: Create a new working dir each time,
-                    True: reuse the work dir if it exists already (default)."""
+
+    Parameters
+    ----------
+    noWorkDir: bool
+        False: Copy input data to a new working dir (default),
+        True: otherwise, use data where it is.
+    reuseWorkDir: bool
+        False: Create a new working dir each time,
+        True: reuse the work dir if it exists already (default).
+
+    Returns
+    -------
+    A list of absolute directory paths.
+    """
     basedir = getWorkDir(workDir=workDir, skip=noWorkDir)
     workDir = prepareWorkDir(basedir, dataDir, useExisting=reuseWorkDir)
     print("Entering '{}':".format(workDir))
     dirs = sorted([dn for dn in Path(workDir).iterdir() if dn.is_dir()])
     dirs.append(Path(workDir))
     # [print(os.path.join(*dn.parts[-2:])) for dn in dirs]
     printFileList(dirs, numParts=1)
@@ -94,15 +102,15 @@
 
 
 def getDataFiles(dataDirs, include=None, exclude=None):
     """Return absolute file paths from given directories."""
 
     def getFiles(dn, include=None):
         if not include:
-            include = '*'
+            include = "*"
         if not isList(include):
             include = (include,)
         return [path for inc in include for path in glob.glob(os.path.join(dn, inc))]
 
     if not exclude:
         exclude = ()
     if not isList(exclude):
@@ -112,9 +120,9 @@
 
     files = [
         fn
         for dn in dataDirs
         for fn in getFiles(dn, include)
         if not any([(ex in fn) for ex in exclude])
     ]
-    print('{} files to be analyzed in subdirectories.'.format(len(files)))
+    print("{} files to be analyzed in subdirectories.".format(len(files)))
     return sorted(files)
```

### Comparing `jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/distrib.py` & `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/distrib.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         start, end = max(start - 1, 0), min(end + 1, len(x) - 1)
         monotony = np.sign(np.diff(y[start : end + 1]))
         if not all(monotony == monotony[0]):
             # avoid monotonously increasing/decreasing peaks -> unwanted artefacts
             ranges.append((start, end))
 
     for idx in indexGroups:
-        appendPeakRange(istart, indices[idx])   # add the new range to the list
-        istart = indices[idx + 1]               # start new range
+        appendPeakRange(istart, indices[idx])  # add the new range to the list
+        istart = indices[idx + 1]  # start new range
     appendPeakRange(istart, indices[-1])
     # print("findPeakRanges", ranges)
     return ranges
 
 
 def findLocalMinima(peakRanges, xarr, yarr, doPlot=False, verbose=False):
     """Identify local (non-zero) minima within given peak ranges and separate those
@@ -75,21 +75,21 @@
     # print("findLocalMinima", peakRanges)
     newRanges = []
     if doPlot:
         plt.figure(figsize=(15, 5))
     for ip, (istart, iend) in enumerate(peakRanges):
         if verbose:
             print((istart, iend), xarr[istart], xarr[iend])
-        if iend - istart < 5:   # skip this, can't be fitted and no sub-peaks are likely
+        if iend - istart < 5:  # skip this, can't be fitted and no sub-peaks are likely
             newRanges.append((istart, iend))
             continue
         while yarr[istart] <= 0.0 and istart < iend:
-            istart += 1   # exclude leading zero
+            istart += 1  # exclude leading zero
         while yarr[iend] <= 0.0 and istart < iend:
-            iend -= 1   # exclude trailing zero
+            iend -= 1  # exclude trailing zero
         if istart == iend:
             continue
         if verbose:
             print((istart, iend))
         x, y = xarr[istart : iend + 1], yarr[istart : iend + 1]
         try:
             spline = scipy.interpolate.InterpolatedUnivariateSpline(x, y, k=4)
@@ -146,85 +146,85 @@
 
 
 class Moments(dict):
     @staticmethod
     def nthMoment(x, weights, n):
         """Calculates the nth moment of the given distribution weights."""
         center = 0
-        if n > 0:   # calculate the mean first
+        if n > 0:  # calculate the mean first
             center = np.average(x, weights=weights) if sum(weights) else 0.0
             #          np.sqrt(u**2)/len(u) # center uncertainty
         if n == 1:
-            return center   # the mean
+            return center  # the mean
         var = 1.0
         if n > 1:
             var = np.sum(weights * (x - center) ** 2) / np.sum(weights)
         if n == 2:
-            return var   # the variance
+            return var  # the variance
         return np.sum(weights * (x - center) ** n) / np.sum(weights) / var**n
 
     @classmethod
     def fromData(cls, x, y):
         store = cls()
         mean, var, skew, kurt = [cls.nthMoment(x, y, i) for i in range(1, 5)]
-        store['area'] = integrate(x, y)
-        store['mean'] = mean
-        store['var'] = var
-        store['skew'] = skew
-        store['kurt'] = kurt
+        store["area"] = integrate(x, y)
+        store["mean"] = mean
+        store["var"] = var
+        store["skew"] = skew
+        store["kurt"] = kurt
         return store
 
     @property
     def area(self):
-        return self['area']
+        return self["area"]
 
     @property
     def mean(self):
-        return self['mean']
+        return self["mean"]
 
     @property
     def var(self):
-        return self['var']
+        return self["var"]
 
     @property
     def skew(self):
-        return self['skew']
+        return self["skew"]
 
     @property
     def kurt(self):
-        return self['kurt']
+        return self["kurt"]
 
     def __str__(self):
         return "\n".join(
             [
                 "{: <4s}: {: 9.2g}".format(k, self[k])
                 for k in ("area", "mean", "var", "skew", "kurt")
             ]
         )
 
     @staticmethod
     def logNormParFromMoments(mean, var, N=1.0):
         # SASfit manual, 6.4. Log-Normal distribution
         median = mean**2 / np.sqrt(var + mean**2)
         sigma = np.sqrt(np.log(mean**2 / median**2))
-        return {'N': N, 'sigma': sigma, 'median': median}
+        return {"N": N, "sigma": sigma, "median": median}
 
     def logNormPar(self, N=1.0):
         return self.logNormParFromMoments(self.mean, self.var, N=N)
 
 
 class Distribution:
     x, y, u = None, None, None
-    peaks = None   # list of peak (start, end) indices pointing into x,y,u
+    peaks = None  # list of peak (start, end) indices pointing into x,y,u
     color = None
     xlabel = None
     plotAxes, plotAxisIdx = None, 0
 
     def __init__(self, xvec, yvec, uvec, xlabel=None, maxPeakCount=None):
-        self.xlabel = getattr(xvec, 'name', None)
+        self.xlabel = getattr(xvec, "name", None)
         xvec = xvec.values if isinstance(xvec, pd.Series) else xvec
         yvec = yvec.values if isinstance(yvec, pd.Series) else yvec
         uvec = uvec.values if isinstance(uvec, pd.Series) else uvec
         self.x, self.y, self.u = normalizeDistrib(xvec, yvec, uvec)
         if xlabel is not None:
             self.xlabel = xlabel
         self.peaks = findPeakRanges(self.x, self.y, tol=1e-6)
@@ -264,37 +264,37 @@
         # ax.plot(x, y, 'o', color=cls.color)
         lbl, fmt = [], "{: <7s} {: 9.2g} ±{: 9.2g}"
         for k in "area", "median", "var", "skew", "kurt":
             if k == "median":
                 lbl.append(
                     fmt.format(
                         "median:",
-                        dp['median'],
-                        max(abs(dp['median'] - dpLo['median']), abs(dpHi['median'] - dp['median'])),
+                        dp["median"],
+                        max(abs(dp["median"] - dpLo["median"]), abs(dpHi["median"] - dp["median"])),
                     )
                 )
             else:
                 lbl.append(
-                    fmt.format(k + ':', mom[k], max(abs(mom[k] - momLo[k]), abs(momHi[k] - mom[k])))
+                    fmt.format(k + ":", mom[k], max(abs(mom[k] - momLo[k]), abs(momHi[k] - mom[k])))
                 )
         lbl.append("LogNorm: " + distrParToText(dp)[0])
         ax.bar(x, y, width=self.getBarWidth(x), color=self.color, alpha=0.5, label="\n".join(lbl))
         ax.fill_between(
             x,
             np.maximum(0, y - u),
             y + u,
-            color='red',
+            color="red",
             lw=0,
             alpha=0.1,
             label=f"uncertainties (lvl: {self.uncertRatioMedian(peakRange):.3g})",
         )
         if showFullRange:
             ax.set_xlim((self.x.min(), self.x.max()))
         ax.set_xlabel(self.xlabel)
-        ax.legend(prop=font_manager.FontProperties(family='monospace'))
+        ax.legend(prop=font_manager.FontProperties(family="monospace"))
         ax.grid(True)
 
     def plot(self, ax, distPar, name=""):
         """plot complete distribution as loaded from file"""
         lbl = (
             "from file, "
             + name
@@ -311,15 +311,15 @@
             label=lbl,
         )
         # ax.errorbar(self.x, self.y, yerr=self.u, lw=lineWidth()*2, label=lbl)
         ax.fill_between(
             self.x,
             np.maximum(0, self.y - self.u),
             self.y + self.u,
-            color='red',
+            color="red",
             lw=0,
             alpha=0.1,
             label="uncertainties",
         )
         ax.set_xlabel(self.xlabel)
         ax.legend()
         ax.grid()
@@ -337,40 +337,38 @@
                 lnpLo = momLo.logNormPar(N=N)
                 lnpHi = momHi.logNormPar(N=N)
                 yield (peakRange, mom, momLo, momHi, lnp, lnpLo, lnpHi)
 
         # return a dict of lists, addressable by peak index
         return dict(
             zip(
-                ['peakRange', 'mom', 'momLo', 'momHi', 'lnp', 'lnpLo', 'lnpHi'],
+                ["peakRange", "mom", "momLo", "momHi", "lnp", "lnpLo", "lnpHi"],
                 zip(*[m for m in momentsByPeak()]),
             )
         )
 
     def peakDistrPar(self, plotAxes=None, plotAxisStart=0, **plotPeakKwargs):
         momentsAndLogNormPar = self.moments()
         if plotAxes is not None:
-            for i, peakRange in enumerate(momentsAndLogNormPar['peakRange']):
-                plotPeakKwargs['ax'] = plotAxes[plotAxisStart + i]
+            for i, peakRange in enumerate(momentsAndLogNormPar["peakRange"]):
+                plotPeakKwargs["ax"] = plotAxes[plotAxisStart + i]
                 self.plotPeak(*[v[i] for v in momentsAndLogNormPar.values()], **plotPeakKwargs)
-        return momentsAndLogNormPar['lnp'], momentsAndLogNormPar['mom']
+        return momentsAndLogNormPar["lnp"], momentsAndLogNormPar["mom"]
 
 
 def distrParToText(logNormPar):
     """
     >>> distrParToText({'N':1.1, 'sigma':0.15, 'median':33.1234e-9})
     ['median=3.3e-08 sigma=0.15 N=1.1']
-
     >>> distrParToText({'N':1.2e13, 'sigma':0.15, 'median':3.1234})
     ['median=3.1 sigma=0.15 N=1.2e+13']
-
     >>> distrParToText({'N':(1.,2.), 'sigma':(.2,.4), 'median':(40e-9,7e-8)})
     ['median_0=4e-08 sigma_0=0.20 N_0=1', 'median_1=7e-08 sigma_1=0.40 N_1=2']
     """
-    fmt = {'median': "{:.2g}", 'sigma': "{:.2f}", 'N': "{:.2g}"}
+    fmt = {"median": "{:.2g}", "sigma": "{:.2f}", "N": "{:.2g}"}
     order = {key: list(fmt.keys()).index(key) for key in fmt.keys()}
     return [
         " ".join(p)
         for p in grouper(
             list(
                 zip(
                     *sorted(
@@ -394,49 +392,46 @@
     ]
 
 
 def distrParLatex(distrPar, *kwargs):
     r"""
     >>> distrParLatex({'N':1.1, 'sigma':0.15, 'median':33e-9})
     '$median=3.3e-08\\;sigma=0.15\\;N=1.1$'
-
     >>> distrParLatex({'N':(1.,2.), 'sigma':(.2,.4), 'median':(40e-9,7e-8)})
     '$median_0=4e-08\\;sigma_0=0.20\\;N_0=1$\n$median_1=7e-08\\;sigma_1=0.40\\;N_1=2$'
     """
-    return "\n".join(['$' + txt.replace(' ', r'\;') + '$' for txt in distrParToText(distrPar)])
+    return "\n".join(["$" + txt.replace(" ", r"\;") + "$" for txt in distrParToText(distrPar)])
 
 
-def distrParToFilename(distrPar, prefix=''):
+def distrParToFilename(distrPar, prefix=""):
     """
     >>> distrParToFilename({'N':1.1, 'sigma':0.15, 'median':33e-9})
     '_median=3.3e-08_sigma=0.15_N=1.1'
-
     >>> distrParToFilename({'N':(1.,2.), 'sigma':(.2,.4), 'median':(40e-9,7e-8)})
     '_median_0=4e-08_sigma_0=0.20_N_0=1_median_1=7e-08_sigma_1=0.40_N_1=2'
     """
-    return '_'.join([prefix] + distrParToText(distrPar)).replace(' ', '_')
+    return "_".join([prefix] + distrParToText(distrPar)).replace(" ", "_")
 
 
 def distrParFromFilename(fn):
     """
     >>> distrParFromFilename('_median=_33_sigma=0.15_N=1.1') == {'N':1.1, 'sigma':0.15, 'median':33}
     True
-
     >>> fn = '_median_0=4e-08_sigma_0=0.20_N_0=1_median_1=7e-08_sigma_1=0.40_N_1=2'
     >>> distrParFromFilename(fn) == {'N':(1.,2.), 'sigma':(.2,.4), 'median':(40e-9,7e-8)}
     True
     """
-    fn = fn.split('=')
-    fn = [elem.lstrip('_') for elem in fn]
-    fn = [(elem.split('_', maxsplit=1) if elem[0].isnumeric() else [elem]) for elem in fn]
+    fn = fn.split("=")
+    fn = [elem.lstrip("_") for elem in fn]
+    fn = [(elem.split("_", maxsplit=1) if elem[0].isnumeric() else [elem]) for elem in fn]
     fn = list(itertools.chain(*fn))
     result = {}
     for k, v in grouper(fn, 2):
-        key = k.split('_')[0]
-        value = float(v) if 'median' == key else float(v)
+        key = k.split("_")[0]
+        value = float(v) if "median" == key else float(v)
         result[key] = (
             value
             if key not in result
             else (
                 result[key] + (value,) if isinstance(result[key], tuple) else (result[key], value)
             )
         )
```

### Comparing `jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/git.py` & `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/git.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,41 +35,41 @@
     # is git installed?
     try:
         import git
     except ImportError:
         print("Could not load git module, is GIT installed and in PATH?")
         return
     # check the repository in detail
-    from IPython.display import HTML
-    from IPython.display import display
+    from IPython.display import HTML, display
 
-    repo = git.Repo('.')
+    repo = git.Repo(".")
     #    currentNB = os.path.basename(currentNBpath())
     try:
         editedOn = repo.git.show(no_patch=True, format="%cd, version %h by %cn", date="iso")
     except git.GitCommandError:
         print("Not a GIT repository.")
         return
-    editedOn = editedOn.split(', ')
-    opacity = 0.3   # 1.0 if repo.is_dirty() else 0.5
+    editedOn = editedOn.split(", ")
+    opacity = 0.3  # 1.0 if repo.is_dirty() else 0.5
     display(
         HTML(
             '<div style="opacity: {opacity};">'
-            '<h3>Document updated on {}</h3>'
-            '<h4>({})</h4></div>'.format(*editedOn, opacity=opacity)
+            "<h3>Document updated on {}</h3>"
+            "<h4>({})</h4></div>".format(*editedOn, opacity=opacity)
         )
     )
     if repo.is_dirty():
         edits = repo.git.diff(stat=True)
         import re
 
         edits = re.sub(r" (\++)", r' <span style="color: green;">\1</span>', edits)
         edits = re.sub(r"(\+)?(-+)(\s)", r'\1<span style="color: red;">\2</span>\3', edits)
         display(
             HTML(
                 '<div style="border-style: solid; border-color: darkred; border-width: 1px; '
                 'padding: 0em 1em 1em 1em; margin: 1em 0em;">'
                 '<h4 style="color: darkred;">There are changes in this repository:</h4>'
-                "<pre>" + edits + "</pre>"
-                '</div>'
+                "<pre>"
+                + edits
+                + "</pre></div>"
             )
         )
```

### Comparing `jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/notebook_utils.py` & `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/notebook_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 def currentNBpath():
     """Returns the absolute path of the Notebook or None if it cannot be determined
     NOTE: works only for *Jupyter Notebook* (not Jupyter Lab)
     and when the security is token-based or there is also no password.
     """
     connection_file = os.path.basename(ipykernel.get_connection_file())
-    kernel_id = connection_file.split('-', 1)[1].split('.')[0]
+    kernel_id = connection_file.split("-", 1)[1].split(".")[0]
 
     for srv in notebookapp.list_running_servers():
         try:
-            if srv['token'] == '' and not srv['password']:  # No token and no password, ahem...
-                req = urllib.request.urlopen(srv['url'] + 'api/sessions')
+            if srv["token"] == "" and not srv["password"]:  # No token and no password, ahem...
+                req = urllib.request.urlopen(srv["url"] + "api/sessions")
             else:
-                req = urllib.request.urlopen(srv['url'] + 'api/sessions?token=' + srv['token'])
+                req = urllib.request.urlopen(srv["url"] + "api/sessions?token=" + srv["token"])
             sessions = json.load(req)
             for sess in sessions:
-                if sess['kernel']['id'] == kernel_id:
-                    return os.path.join(srv['notebook_dir'], sess['notebook']['path'])
+                if sess["kernel"]["id"] == kernel_id:
+                    return os.path.join(srv["notebook_dir"], sess["notebook"]["path"])
         except OSError:
             pass  # There may be stale entries in the runtime directory
     return None
```

### Comparing `jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/plotting.py` & `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/plotting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # -*- coding: utf-8 -*-
 # plotting.py
 
 import matplotlib
 import matplotlib.pyplot as plt
 
-# increase the limit for the warning to pop up
-matplotlib.rcParams['figure.max_open_warning'] = 50
+try:
+    # increase the limit for the warning to pop up
+    matplotlib.rcParams["figure.max_open_warning"] = 50
+except TypeError:  # ignore the error with Sphinx
+    pass
 
 
 def initFigure(fig, width=80, aspectRatio=4.0 / 3.0, quiet=False):
     mmInch = 25.4
     fig.set_size_inches(width / mmInch, width / aspectRatio / mmInch)
     w, h = fig.get_size_inches()
     if not quiet:
-        print('initFigure() with ({w:.1f}x{h:.1f}) mm'.format(w=w * mmInch, h=h * mmInch))
+        print("initFigure() with ({w:.1f}x{h:.1f}) mm".format(w=w * mmInch, h=h * mmInch))
     return fig
 
 
 def createFigure(width=80, aspectRatio=4.0 / 3.0, quiet=False, **kwargs):
     """output figure width in mm"""
     fig = plt.figure(
         # tight_layout=dict(pad=0.05),
@@ -28,15 +31,15 @@
 
 
 def plotVertBar(ax, xpos, ymax, **kwargs):
     ax.plot((xpos, xpos), (0, ymax), **kwargs)
 
 
 def plotColor(idx):
-    pltcol = plt.rcParams['axes.prop_cycle'].by_key()['color']
+    pltcol = plt.rcParams["axes.prop_cycle"].by_key()["color"]
     # print(pltcol)
-    pltcol = ['gray', 'lightskyblue', 'steelblue', 'red', 'salmon']
+    pltcol = ["gray", "lightskyblue", "steelblue", "red", "salmon"]
     return pltcol[idx]
 
 
 def lineWidth():
-    return plt.rcParams['lines.linewidth']
+    return plt.rcParams["lines.linewidth"]
```

### Comparing `jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/reBin.py` & `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/binning.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,181 +18,175 @@
 import argparse
 import itertools
 import os
 import sys
 
 import numpy as np
 import pandas
-from numpy import argsort
-from numpy import log10
-from numpy import reshape
-from numpy import shape
-from numpy import size
-from numpy import sqrt
-from numpy import zeros
+from numpy import argsort, log10, reshape, shape, size, sqrt, zeros
 
 
 def argparser():
     parser = argparse.ArgumentParser(
         description="""
             Re-binning function, reads three-column ASCII input files,
             and outputs re-binned three-column ASCII files"""
     )
     # binning options
-    parser.add_argument('-n', '--numBins', type=int, default=50, help='Number of bins to use')
+    parser.add_argument("-n", "--numBins", type=int, default=50, help="Number of bins to use")
     parser.add_argument(
-        '-q',
-        '--qMin',
+        "-q",
+        "--qMin",
         type=float,
         default=0.0,
-        help='Minimum Q to clip from original data',
+        help="Minimum Q to clip from original data",
     )
     parser.add_argument(
-        '-Q',
-        '--qMax',
+        "-Q",
+        "--qMax",
         type=float,
         default=np.inf,
-        help='Minimum Q to clip from original data',
+        help="Minimum Q to clip from original data",
     )
     parser.add_argument(
-        '-e',
-        '--minE',
+        "-e",
+        "--minE",
         type=float,
         default=0.01,
-        help='Minimum error is at least this times intensity value.',
+        help="Minimum error is at least this times intensity value.",
     )
     parser.add_argument(
-        '-s',
-        '--scaling',
+        "-s",
+        "--scaling",
         type=str,
-        action='store',
-        default='logarithmic',
-        help='q-axis scaling for binning, can be linear or logarithmic',
+        action="store",
+        default="logarithmic",
+        help="q-axis scaling for binning, can be linear or logarithmic",
     )
     # csv / datafile options
     parser.add_argument(
-        '-d',
-        '--delimiter',
+        "-d",
+        "--delimiter",
         type=str,
-        action='store',
-        default=',',
+        action="store",
+        default=",",
         help="Delimiter in original file. '\\t' is tab. (with quotes)",
     )
     parser.add_argument(
-        '-H',
-        '--headerLines',
+        "-H",
+        "--headerLines",
         type=int,
         default=0,
-        help='Number of header lines to skip',
+        help="Number of header lines to skip",
     )
     parser.add_argument(
-        '-D',
-        '--outputDelimiter',
+        "-D",
+        "--outputDelimiter",
         type=str,
-        action='store',
+        action="store",
         default=None,
-        help='Delimiter in final file (defaults to input delimiter)',
+        help="Delimiter in final file (defaults to input delimiter)",
     )
     parser.add_argument(
-        '-c',
-        '--cleanEmpty',
-        action='store_true',
+        "-c",
+        "--cleanEmpty",
+        action="store_true",
         default=True,
-        help='Removes empty bins before writing',
+        help="Removes empty bins before writing",
     )
     parser.add_argument(
-        '-i',
-        '--iScale',
+        "-i",
+        "--iScale",
         type=float,
         default=1.0,
-        help='Intensity (and error) scaled by this factor on output.',
+        help="Intensity (and error) scaled by this factor on output.",
     )
     # program options
     parser.add_argument(
-        '-v',
-        '--verbose',
-        action='store_true',
-        help='Be verbose about the steps',
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="Be verbose about the steps",
     )
     parser.add_argument(
-        '-t',
-        '--test',
-        action='store_true',
-        help='Do not save output files, test run only',
+        "-t",
+        "--test",
+        action="store_true",
+        help="Do not save output files, test run only",
     )
     parser.add_argument(
-        '-N',
-        '--noBin',
-        action='store_true',
-        help='Do not bin, just input -> output (for translation and scaling)',
+        "-N",
+        "--noBin",
+        action="store_true",
+        help="Do not bin, just input -> output (for translation and scaling)",
     )
     parser.add_argument(
-        'fnames',
-        nargs='*',
-        metavar='FILENAME',
-        action='store',
-        help='One or more data files to rebin',
+        "fnames",
+        nargs="*",
+        metavar="FILENAME",
+        action="store",
+        help="One or more data files to rebin",
     )
     # show help if no files were provided, no arguments at all
     args = parser.parse_args()
     if len(args.fnames):
         return args
     parser.print_help(sys.stderr)
     sys.exit(1)
 
 
 class reBin(object):
     """all kinds of binning-related functions"""
 
     # set defaults for file reading:
     pandasArgs = {
-        'skipinitialspace': True,
-        'skip_blank_lines': True,
-        'engine': 'python',
-        'header': None,
+        "skipinitialspace": True,
+        "skip_blank_lines": True,
+        "engine": "python",
+        "header": None,
     }
     # set defaults for kwargs, in case this is not called from command line:
     reBinArgs = {
-        'delimiter': ';',
-        'outputDelimiter': ';',
-        'headerLines': 0,
-        'fnames': '',
-        'verbose': False,
-        'qMin': -np.inf,
-        'qMax': np.inf,
-        'numBins': 100,
-        'scaling': 'logarithmic',
-        'cleanEmpty': False,
-        'minE': 0.01,
-        'noBin': False,
+        "delimiter": ";",
+        "outputDelimiter": ";",
+        "headerLines": 0,
+        "fnames": "",
+        "verbose": False,
+        "qMin": -np.inf,
+        "qMax": np.inf,
+        "numBins": 100,
+        "scaling": "logarithmic",
+        "cleanEmpty": False,
+        "minE": 0.01,
+        "noBin": False,
     }
 
     def __init__(self, **kwargs):
         # process defaults:
         for kw in self.reBinArgs:
             setattr(self, kw, self.reBinArgs[kw])
         # process kwargs:
-        if 'verbose' in kwargs:
-            self.verbose = kwargs.pop('verbose')
+        if "verbose" in kwargs:
+            self.verbose = kwargs.pop("verbose")
         for kw in kwargs:
             if self.verbose:
-                print('Processing input argument {}: {}'.format(kw, kwargs[kw]))
+                print("Processing input argument {}: {}".format(kw, kwargs[kw]))
             setattr(self, kw, kwargs[kw])
 
         # process delimiter options
         # decode no longer necessary in python 3
         if sys.version_info <= (3, 0):
-            self.delimiter = self.delimiter.decode('string-escape')
+            self.delimiter = self.delimiter.decode("string-escape")
         if self.outputDelimiter is None:
             self.outputDelimiter = self.delimiter
         else:
             if sys.version_info <= (3, 0):
-                self.outputDelimiter = self.outputDelimiter.decode('string-escape')
+                self.outputDelimiter = self.outputDelimiter.decode("string-escape")
 
-        self.pandasArgs.update({'delimiter': self.delimiter, 'skiprows': self.headerLines})
+        self.pandasArgs.update({"delimiter": self.delimiter, "skiprows": self.headerLines})
         # process files individually:
         for filename in self.fnames:
             self.readFile(filename)
             self.validate()
             self.defineBinEdges()
             self.binning1D()
             if self.cleanEmpty:
@@ -212,42 +206,42 @@
         validi = True ^ np.isnan(self.IBin)
         validi[np.argwhere(self.binMask > 0)] = False
         self.QBin = self.QBin[validi]
         self.IBin = self.IBin[validi]
         self.EBin = self.EBin[validi]
         self.QEBin = self.QEBin[validi]
         if self.verbose:
-            print('valid bins: {} of {}'.format(validi.sum(), len(validi)))
+            print("valid bins: {} of {}".format(validi.sum(), len(validi)))
 
     def outputFilename(self, filename):
         """returns an output filename based on the input filename"""
         of = filename.strip()
         # split at extension
-        ob, oe = of.rsplit('.', 1)
+        ob, oe = of.rsplit(".", 1)
         # add rebin tag and reassemble
-        ofname = '{}_reBin.{}'.format(ob, oe)
+        ofname = "{}_reBin.{}".format(ob, oe)
         if self.verbose:
-            print('output filename: {}'.format(ofname))
+            print("output filename: {}".format(ofname))
         return ofname
 
     def readFile(self, filename):
         if self.verbose:
-            print('reading file: {} with settings: {}'.format(filename, self.pandasArgs))
+            print("reading file: {} with settings: {}".format(filename, self.pandasArgs))
         dval = pandas.read_csv(filename, **self.pandasArgs).values
-        assert isinstance(dval, np.ndarray)   # no problems reading?
-        assert size(dval, axis=1) >= 3   # Q, I and E can be extracted
+        assert isinstance(dval, np.ndarray)  # no problems reading?
+        assert size(dval, axis=1) >= 3  # Q, I and E can be extracted
         if self.verbose:
-            print('data read: {}'.format(dval))
+            print("data read: {}".format(dval))
         self.Q = np.float32(dval[:, 0])
         self.I = np.float32(dval[:, 1])
         self.E = np.maximum(self.minE * self.I, np.float32(dval[:, 2]))
         numChanged = (self.minE * self.I > dval[:, 2]).sum()
         if self.verbose:
             print(
-                'Minimum uncertainty set for {} out of {} ({} %) datapoints'.format(
+                "Minimum uncertainty set for {} out of {} ({} %) datapoints".format(
                     numChanged, size(self.Q), 100.0 * numChanged / size(self.Q)
                 )
             )
 
     # writer modified from imp2/modules/Write1D
     def writeFile(self, ofname, hstrs=None, append=False):
         sep = self.outputDelimiter
@@ -256,17 +250,17 @@
             self.QBin,
             self.IBin * float(self.iScale),
             self.EBin * float(self.iScale),
         )
 
         def writeLine(filename, line=None, append=True):
             if append:
-                openarg = 'a'
+                openarg = "a"
             else:
-                openarg = 'w'
+                openarg = "w"
             with open(filename, openarg) as fh:
                 if isinstance(line, str):
                     fh.write(line)
                 else:
                     # iterable object containing multiple lines
                     fh.writelines(line)
 
@@ -279,24 +273,24 @@
             writeLine(ofname, hstrs)
 
         # store in file
         moreData = True
         while moreData:
             try:
                 # generate formatted datastring containing column data
-                wstr = sep.join(['{}'.format(k) for k in next(iterData)]) + '\n'
+                wstr = sep.join(["{}".format(k) for k in next(iterData)]) + "\n"
             except StopIteration:
                 # end of data reached
                 moreData = False
                 break
             writeLine(ofname, wstr)
 
     def validate(self):
         """Applies limits to the data"""
-        mask = zeros(shape(self.Q), dtype='bool')
+        mask = zeros(shape(self.Q), dtype="bool")
         # appy integration limits:
         iind = np.array(((self.Q < self.qMin) + (self.Q > self.qMax)), dtype=bool)
         mask[iind] = True
 
         # define binning limits
         (qmin, qmax) = (
             np.abs(self.Q[True ^ mask]).min(),
@@ -305,33 +299,33 @@
         self.iqMin = np.maximum(qmin, self.qMin)
         self.iqMax = np.minimum(qmax, self.qMax)
         self.Q = self.Q[True ^ mask]
         self.I = self.I[True ^ mask]
         self.E = self.E[True ^ mask]
         if self.verbose:
             print(
-                'data Q-range: {}, integration Q-range: {}, masked: {} of {} ({}%)'.format(
+                "data Q-range: {}, integration Q-range: {}, masked: {} of {} ({}%)".format(
                     (self.Q.min(), self.Q.max()),
                     (self.iqMin, self.iqMax),
                     mask.sum(),
                     self.Q.size,
                     mask.sum() / self.Q.size,
                 )
             )
 
     def defineBinEdges(self):
         """defines binning edges"""
         # define bin edges
-        if self.scaling.lower() in ('linear', 'lin'):
+        if self.scaling.lower() in ("linear", "lin"):
             qEdges = np.linspace(self.iqMin, self.iqMax, self.numBins + 1)
         else:
             qEdges = np.logspace(log10(self.iqMin), log10(self.iqMax), self.numBins + 1)
         self.qEdges = qEdges
         if self.verbose:
-            print('Bin edges used: {}'.format(self.qEdges))
+            print("Bin edges used: {}".format(self.qEdges))
 
     def binning1D(self, qError=None):
         """An unweighted binning routine.
         imp-version of binning, taking q-bin edges in which binning takes place,
         and calculates the mean q uncertainty in the bin as well from the relative
         Q uncertainties provided.
 
@@ -366,15 +360,15 @@
         # initialise storage:
         numBins = len(qEdges) - 1
         ibin = zeros(numBins)
         qbin = zeros(numBins)
         sdbin = zeros(numBins)
         sebin = zeros(numBins)
         qebin = zeros(numBins)
-        binMask = zeros(numBins)   # set one for masked bin values
+        binMask = zeros(numBins)  # set one for masked bin values
         if error is not None:
             error = reshape(error, size(error))
             error = error[sortInd]
         if qError is not None:
             qError = reshape(qError, size(qError))
             qError = qError[sortInd]
 
@@ -419,31 +413,31 @@
                 sebin[bini] = np.maximum(sebin[bini], sdbin)
                 # qebin is the mean error of the q-values in the bin, should
                 # probably be superseded by the bin width
                 qe = 0.0
                 if qError is not None:
                     qe = np.sqrt((qError[limMask] ** 2).sum())
                 # SSTD of q in bin:
-                qs = np.std(q[limMask], ddof=1)   # sample standard deviation
+                qs = np.std(q[limMask], ddof=1)  # sample standard deviation
                 qebin[bini] = np.maximum(qe, qs)
 
         self.QBin = qbin.copy()
         self.IBin = ibin.copy()
         self.EBin = sebin.copy()
         self.QEBin = qebin.copy()
         self.binMask = binMask.copy()
         if self.verbose:
-            print('qbin: {}'.format(qbin))
-            print('ibin: {}'.format(ibin))
-            print('sebin: {}'.format(sebin))
-            print('qebin: {}'.format(qebin))
-            print('binMask: {}'.format(binMask))
+            print("qbin: {}".format(qbin))
+            print("ibin: {}".format(ibin))
+            print("sebin: {}".format(sebin))
+            print("qebin: {}".format(qebin))
+            print("binMask: {}".format(binMask))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # process input arguments
     adict = argparser()
     # transmogrify into kwargs object
     adict = vars(adict)
     # run the reBin program
     reBin(**adict)
```

### Comparing `jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/readdata.py` & `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/readdata.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,40 +11,40 @@
     extract a file_name
     select q-range: q_min <= q <= q_max
     """
     if print_filename:
         print(f"Reading file '{fn}'")
     if read_csv_args is None:
         read_csv_args = dict()
-    if 'sep' not in read_csv_args:
-        read_csv_args.update(sep=r'\s+')
-    if 'names' not in read_csv_args:
-        read_csv_args.update(names=('q', 'I', 'e'))
-    if 'index_col' not in read_csv_args:
+    if "sep" not in read_csv_args:
+        read_csv_args.update(sep=r"\s+")
+    if "names" not in read_csv_args:
+        read_csv_args.update(names=("q", "I", "e"))
+    if "index_col" not in read_csv_args:
         read_csv_args.update(index_col=False)
     # print("f_read_data, read_csv_args:", read_csv_args) # for debugging
 
     _, file_ext = os.path.splitext(fn)
-    if file_ext.lower() == '.pdh':   # for PDH files
+    if file_ext.lower() == ".pdh":  # for PDH files
         nrows = pd.read_csv(
             fn,
             skiprows=2,
             nrows=1,
             usecols=[
                 0,
             ],
-            sep=r'\s+',
+            sep=r"\s+",
             header=None,
         ).values[0, 0]
         read_csv_args.update(skiprows=5, nrows=nrows)
     df_data = pd.read_csv(fn, **read_csv_args)
 
     # select q-range
     if q_range is not None:
         q_min, q_max = q_range
         df_data = df_data[(df_data.q > q_min) & (df_data.q < q_max)]
 
-    file_name = os.path.basename(fn).split('[')[0]
+    file_name = os.path.basename(fn).split("[")[0]
     return df_data, file_name
 
 
 # vim: set ts=4 sts=4 sw=4 tw=0:
```

### Comparing `jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/utils.py` & `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,45 +9,46 @@
 import platform
 import subprocess
 import sys
 from pathlib import Path
 
 import numpy as np
 
-indent = '    '
+indent = "    "
 
 
 def setLocaleUTF8():
     """Fix the Jupyter locale which is not UTF-8 by default on some systems (older Windows?)."""
     locOld = locale.getpreferredencoding(False).lower()
 
     def getpreferredencoding(do_setlocale=True):
-        return 'utf-8'
+        return "utf-8"
 
     locale.getpreferredencoding = getpreferredencoding
     locNew = locale.getpreferredencoding(False)
     if locOld != locNew:
-        print(f'Updated locale from {locOld} -> {locNew}.')
+        print(f"Updated locale from {locOld} -> {locNew}.")
 
 
 def isLinux():
-    return platform.system().lower() in 'linux'
+    return platform.system().lower() in "linux"
 
 
 def isMac():
-    return platform.system().lower() in 'darwin'
+    return platform.system().lower() in "darwin"
 
 
 def isWindows():
-    return platform.system().lower() in 'windows'
+    return platform.system().lower() in "windows"
 
 
 def isList(obj):
     """Return true if the provided object is list-like including a numpy array
     but not a string.
+
     >>> isList([1, 2, 'a'])
     True
     >>> isList(tuple((1, 2, 'a')))
     True
     >>> import numpy
     >>> isList(numpy.arange(5))
     True
@@ -66,57 +67,57 @@
 
     return win32api.GetShortPathName(path)
 
 
 def appendToPATH(parentPath, subdirs=None):
     """Adds the given path with each subdirectory to the PATH environment variable."""
     if not os.path.isdir(parentPath):
-        return   # nothing to do
+        return  # nothing to do
     if subdirs is None:
-        subdirs = ['.']
+        subdirs = ["."]
     for path in subdirs:
-        path = os.path.realpath(os.path.join(parentPath, *path.split('/')))
-        print(indent, path, '\t[{}]'.format(os.path.isdir(path)))
-        if path in os.environ['PATH']:
+        path = os.path.realpath(os.path.join(parentPath, *path.split("/")))
+        print(indent, path, "\t[{}]".format(os.path.isdir(path)))
+        if path in os.environ["PATH"]:
             continue
-        os.environ['PATH'] += ';' + path
+        os.environ["PATH"] += ";" + path
 
 
 def checkWinFor7z():
     """Extend the PATH environment variable for access to the 7-zip executable."""
     if not isWindows():
-        return   # tests below are intended for Windows
-    sevenzippath = r'C:\Program Files\7-Zip'
+        return  # tests below are intended for Windows
+    sevenzippath = r"C:\Program Files\7-Zip"
     if not os.path.isdir(sevenzippath):
         print(
             "7-Zip not found in '{}'.\n".format(sevenzippath)
-            + '7-Zip is required for managing data files and results!.'
+            + "7-Zip is required for managing data files and results!."
         )
         return
-    print('Adding the following directory to $PATH:')
+    print("Adding the following directory to $PATH:")
     appendToPATH(sevenzippath)
-    print('\nUpdated PATH:')
-    for path in os.environ['PATH'].split(';'):
+    print("\nUpdated PATH:")
+    for path in os.environ["PATH"].split(";"):
         print(indent, path)
 
 
 def extract7z(fn, workdir=None):
     assert os.path.isfile(os.path.join(workdir, fn)), "Provided 7z archive '{}' not found!".format(
         fn
     )
-    print('Extracting archived McDLS results:')
+    print("Extracting archived McDLS results:")
     proc = subprocess.run(
-        ['7z', 'x', fn],
+        ["7z", "x", fn],
         cwd=workdir,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
-    print(proc.stdout.decode(errors='ignore'))
+    print(proc.stdout.decode(errors="ignore"))
     if len(proc.stderr):
-        print('## stderr:\n', proc.stderr.decode(errors='ignore'))
+        print("## stderr:\n", proc.stderr.decode(errors="ignore"))
 
 
 # https://stackoverflow.com/a/13847807
 @contextlib.contextmanager
 def pushd(new_dir):
     previous_dir = os.getcwd()
     os.chdir(new_dir)
@@ -128,32 +129,32 @@
     """Sets the current directory of the notebook as python package
     to make relative module imports work.
     Usage: `setPackage(globals())`"""
     path = Path().resolve()
     searchpath = str(path.parent)
     if searchpath not in sys.path:
         sys.path.insert(0, searchpath)
-    globalsdict['__package__'] = path.name
-    globalsdict['__name__'] = path.name
+    globalsdict["__package__"] = path.name
+    globalsdict["__name__"] = path.name
     print(f"Setting the current directory as package '{path.name}':\n  {path}.")
 
 
 def grouper(iterable, n, fillvalue=None):
     """Returns an iterator over a list of tuples (grouping) for a given flat iterable."""
     args = [iter(iterable)] * n
     return itertools.zip_longest(*args, fillvalue=fillvalue)
 
 
 def fmtErr(val, std, precision=2, width=None):
     """Formats a given value and its std. deviation to physics notation, e.g. '1.23(4)'."""
     if width is None:
-        width = ''
-    fmt = '{:' + str(width) + '.' + str(precision) + 'f}({:.0f})'
+        width = ""
+    fmt = "{:" + str(width) + "." + str(precision) + "f}({:.0f})"
     # print("fmtErr val:", val, "std:", std)
     return fmt.format(val, std * 10 ** (precision))
 
 
 def updatedDict(d, key, value):
-    """Implements the |= operator for dict in Python version <3.9."""
+    """Implements the \\|= operator for dict in Python version <3.9."""
     dd = copy.copy(d)
     dd[key] = value
     return dd
```

### Comparing `jupyter-analysis-tools-0.1.0/src/jupyter_analysis_tools/widgets.py` & `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,82 +6,83 @@
 import ipywidgets as ui
 
 
 def showBoolStatus(value, description, invertcolor=False):
     """Pretty prints the status of a boolean variable *value* along with
     the provided description in a green color for True and in a red color
     for False values. *invertcolor* allows to flip the color assignment."""
-    from IPython.display import HTML
-    from IPython.display import display
+    from IPython.display import HTML, display
 
-    statuscolor = 'darkgreen'
+    statuscolor = "darkgreen"
     if value ^ invertcolor:
-        statuscolor = 'darkred'
+        statuscolor = "darkred"
     descr = description[0].lower() + description[1:-1]
     if description[-1].isalnum():
         descr += description[-1]
     statustext = '<h4 style="color: {};">Yes, {}!</h4>'.format(statuscolor, descr)
     if value:
         statustext = '<h4 style="color: {};">Do not {}!</h4>'.format(statuscolor, descr)
     display(
         HTML(
             f'<div style="border-style: solid; border-color: {statuscolor};'
-            f' border-width: 1px; padding: 0em 1em .5em 1em; margin: 1em 0em;'
-            f' width: {len(descr) * 0.75}em;">' + statustext + '</div>'
+            " border-width: 1px; padding: 0em 1em .5em 1em; margin: 1em 0em;"
+            f' width: {len(descr) * 0.75}em;">'
+            + statustext
+            + "</div>"
         )
     )
 
 
 class PathSelector:
     def __init__(self, start_dir, select_file=True):
         self.file = None
         self.select_file = select_file
         self.cwd = start_dir
-        self.select = ui.SelectMultiple(options=['init'], value=(), rows=10, description='')
+        self.select = ui.SelectMultiple(options=["init"], value=(), rows=10, description="")
         self.accord = ui.Accordion(children=[self.select])
 
-        self.accord.selected_index = None   # Start closed (showing path only)
+        self.accord.selected_index = None  # Start closed (showing path only)
         self.refresh(self.cwd)
-        self.select.observe(self.on_update, 'value')
+        self.select.observe(self.on_update, "value")
 
     def on_update(self, change):
-        if len(change['new']) > 0:
-            self.refresh(change['new'][0])
+        if len(change["new"]) > 0:
+            self.refresh(change["new"][0])
 
     def refresh(self, item):
         path = os.path.abspath(os.path.join(self.cwd, item))
 
         if os.path.isfile(path):
             if self.select_file:
                 self.accord.set_title(0, path)
                 self.file = path
                 self.accord.selected_index = None
             else:
                 self.select.value = ()
 
-        else:   # os.path.isdir(path)
+        else:  # os.path.isdir(path)
             self.file = None
             self.cwd = path
 
             # Build list of files and dirs
-            keys = ['[..]']
+            keys = ["[..]"]
             for item in os.listdir(path):
-                if item[0] == '.':
+                if item[0] == ".":
                     continue
                 elif os.path.isdir(os.path.join(path, item)):
-                    keys.append('[' + item + ']')
+                    keys.append("[" + item + "]")
                 else:
                     keys.append(item)
 
             # Sort and create list of output values
             keys.sort(key=str.lower)
             vals = []
             for k in keys:
-                if k[0] == '[':
-                    vals.append(k[1:-1])   # strip off brackets
+                if k[0] == "[":
+                    vals.append(k[1:-1])  # strip off brackets
                 else:
                     vals.append(k)
 
             # Update widget
             self.accord.set_title(0, path)
             self.select.options = list(zip(keys, vals))
             with self.select.hold_trait_notifications():
```

