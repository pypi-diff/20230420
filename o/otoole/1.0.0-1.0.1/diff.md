# Comparing `tmp/otoole-1.0.0.tar.gz` & `tmp/otoole-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otoole-1.0.0.tar", last modified: Sun Feb 26 03:49:05 2023, max compression
+gzip compressed data, was "otoole-1.0.1.tar", last modified: Thu Apr 20 01:53:27 2023, max compression
```

## Comparing `otoole-1.0.0.tar` & `otoole-1.0.1.tar`

### file list

```diff
@@ -1,104 +1,110 @@
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.442753 otoole-1.0.0/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      589 2023-02-26 01:13:12.000000 otoole-1.0.0/.coveragerc
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.322753 otoole-1.0.0/.github/
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.352753 otoole-1.0.0/.github/workflows/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      740 2023-02-26 03:45:17.000000 otoole-1.0.0/.github/workflows/python.yaml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      700 2023-02-26 03:45:17.000000 otoole-1.0.0/.gitignore
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       54 2023-02-26 03:45:17.000000 otoole-1.0.0/.isort.cfg
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1519 2023-02-26 03:45:17.000000 otoole-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      490 2023-02-26 03:45:17.000000 otoole-1.0.0/.readthedocs.yml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      694 2023-02-26 03:45:17.000000 otoole-1.0.0/.zenodo.json
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      217 2023-02-26 03:45:17.000000 otoole-1.0.0/AUTHORS.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2862 2023-02-26 03:45:17.000000 otoole-1.0.0/CHANGELOG.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1077 2023-02-26 03:45:17.000000 otoole-1.0.0/LICENSE.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2382 2023-02-26 03:49:05.442753 otoole-1.0.0/PKG-INFO
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1865 2023-02-26 03:45:17.000000 otoole-1.0.0/README.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      599 2023-02-26 03:45:17.000000 otoole-1.0.0/citation.cff
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.372753 otoole-1.0.0/docs/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1154 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/Makefile
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.372753 otoole-1.0.0/docs/_static/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       18 2023-02-26 01:13:12.000000 otoole-1.0.0/docs/_static/.gitignore
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   135029 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/_static/OSeMOSYS.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    61672 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/_static/logo.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    56337 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/_static/osemosys_dataflow.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5597 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/_static/otoole_figures.drawio
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   178856 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/_static/overview.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   168226 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/_static/overview_v2.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    95949 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/_static/simplicity_res.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    56119 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/_static/validataion_model.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   217753 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/_static/workflow.png
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       41 2023-02-26 01:13:12.000000 otoole-1.0.0/docs/authors.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       43 2023-02-26 01:13:12.000000 otoole-1.0.0/docs/changelog.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    10307 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/conf.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    12076 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/contributing.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11733 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/data.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     8936 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/examples.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     8264 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/functionality.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1334 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/index.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1116 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/install.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       67 2023-02-26 01:13:12.000000 otoole-1.0.0/docs/license.rst
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      276 2023-02-26 03:45:17.000000 otoole-1.0.0/docs/requirements.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      355 2023-02-26 03:45:17.000000 otoole-1.0.0/pyproject.toml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      151 2023-02-26 03:45:17.000000 otoole-1.0.0/requirements.txt
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.382753 otoole-1.0.0/scripts/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      760 2023-02-26 01:13:12.000000 otoole-1.0.0/scripts/prepare_cbc.sh
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      824 2023-02-26 01:13:12.000000 otoole-1.0.0/scripts/prepare_cbc_short.sh
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1440 2023-02-26 03:49:05.442753 otoole-1.0.0/setup.cfg
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      703 2023-02-26 03:45:17.000000 otoole-1.0.0/setup.py
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.332753 otoole-1.0.0/src/
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.392753 otoole-1.0.0/src/otoole/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1059 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/__init__.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    15167 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/cli.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     3040 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/exceptions.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    14369 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/input.py
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.412753 otoole-1.0.0/src/otoole/preprocess/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 01:13:12.000000 otoole-1.0.0/src/otoole/preprocess/__init__.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11432 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/preprocess/config.yaml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2303 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/preprocess/longify_data.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1183 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/preprocess/setup.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5680 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/preprocess/validate_config.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    14054 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/read_strategies.py
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.412753 otoole-1.0.0/src/otoole/results/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 01:13:12.000000 otoole-1.0.0/src/otoole/results/__init__.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    32545 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/results/result_package.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11187 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/results/results.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     8135 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/utils.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     6344 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/validate.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4207 2023-02-26 01:13:12.000000 otoole-1.0.0/src/otoole/validate.yaml
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.412753 otoole-1.0.0/src/otoole/visualise/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      328 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/visualise/__init__.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     7101 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/visualise/res.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     6685 2023-02-26 03:45:17.000000 otoole-1.0.0/src/otoole/write_strategies.py
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.402753 otoole-1.0.0/src/otoole.egg-info/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2382 2023-02-26 03:49:05.000000 otoole-1.0.0/src/otoole.egg-info/PKG-INFO
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2157 2023-02-26 03:49:05.000000 otoole-1.0.0/src/otoole.egg-info/SOURCES.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        1 2023-02-26 03:49:05.000000 otoole-1.0.0/src/otoole.egg-info/dependency_links.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       43 2023-02-26 03:49:05.000000 otoole-1.0.0/src/otoole.egg-info/entry_points.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        1 2023-02-26 03:49:04.000000 otoole-1.0.0/src/otoole.egg-info/not-zip-safe
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      170 2023-02-26 03:49:05.000000 otoole-1.0.0/src/otoole.egg-info/requires.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        7 2023-02-26 03:49:05.000000 otoole-1.0.0/src/otoole.egg-info/top_level.txt
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.432753 otoole-1.0.0/tests/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     3649 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/conftest.py
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.432753 otoole-1.0.0/tests/fixtures/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   111742 2023-02-26 01:13:12.000000 otoole-1.0.0/tests/fixtures/combined_inputs.xlsx
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11533 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/fixtures/config.yaml
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4865 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/fixtures/config_r.yaml
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.442753 otoole-1.0.0/tests/fixtures/data/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      182 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/fixtures/data/AccumulatedAnnualDemand.csv
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       29 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/fixtures/data/AvailabilityFactor.csv
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    44422 2023-02-26 01:13:12.000000 otoole-1.0.0/tests/fixtures/simplicity-v0.2.1.zip
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    43735 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/fixtures/simplicity.txt
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    75398 2023-02-26 01:13:12.000000 otoole-1.0.0/tests/fixtures/simplicity.xlsx
-drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 03:49:05.442753 otoole-1.0.0/tests/results/
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    28520 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/results/test_results_package.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4802 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/test_cli.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2149 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/test_convert.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    10122 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/test_input.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    41815 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/test_read_strategies.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1834 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/test_setup.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5441 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/test_utils.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5223 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/test_validate.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11600 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/test_validate_config.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      377 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/test_visualise.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     6654 2023-02-26 03:45:17.000000 otoole-1.0.0/tests/test_write_strategies.py
--rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2553 2023-02-26 03:45:17.000000 otoole-1.0.0/tox.ini
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.806594 otoole-1.0.1/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      589 2023-02-26 01:13:12.000000 otoole-1.0.1/.coveragerc
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.686594 otoole-1.0.1/.github/
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.686594 otoole-1.0.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2384 2023-04-20 01:42:03.000000 otoole-1.0.1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1277 2023-04-20 01:42:03.000000 otoole-1.0.1/.github/ISSUE_TEMPLATE/docs.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      972 2023-04-20 01:42:03.000000 otoole-1.0.1/.github/ISSUE_TEMPLATE/feature.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      261 2023-04-20 01:42:03.000000 otoole-1.0.1/.github/pull_request_template.md
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.686594 otoole-1.0.1/.github/workflows/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      410 2023-04-20 01:42:03.000000 otoole-1.0.1/.github/workflows/citation.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      951 2023-04-20 01:42:03.000000 otoole-1.0.1/.github/workflows/python.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      700 2023-02-26 03:45:17.000000 otoole-1.0.1/.gitignore
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       54 2023-02-26 03:45:17.000000 otoole-1.0.1/.isort.cfg
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1519 2023-02-26 03:45:17.000000 otoole-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      490 2023-02-26 03:45:17.000000 otoole-1.0.1/.readthedocs.yml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      694 2023-02-26 03:45:17.000000 otoole-1.0.1/.zenodo.json
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      217 2023-02-26 03:45:17.000000 otoole-1.0.1/AUTHORS.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2862 2023-02-26 03:45:17.000000 otoole-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      599 2023-04-20 01:42:03.000000 otoole-1.0.1/CITATION.cff
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1077 2023-02-26 03:45:17.000000 otoole-1.0.1/LICENSE.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2387 2023-04-20 01:53:27.806594 otoole-1.0.1/PKG-INFO
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1870 2023-04-20 01:42:03.000000 otoole-1.0.1/README.rst
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.706594 otoole-1.0.1/docs/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1154 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/Makefile
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.726594 otoole-1.0.1/docs/_static/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       18 2023-02-26 01:13:12.000000 otoole-1.0.1/docs/_static/.gitignore
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   135029 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/_static/OSeMOSYS.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    61672 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/_static/logo.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    56337 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/_static/osemosys_dataflow.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5597 2023-04-20 00:31:02.000000 otoole-1.0.1/docs/_static/otoole_figures.drawio
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   178856 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/_static/overview.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   168226 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/_static/overview_v2.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    95949 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/_static/simplicity_res.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    56119 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/_static/validataion_model.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   217753 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/_static/workflow.png
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       41 2023-02-26 01:13:12.000000 otoole-1.0.1/docs/authors.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       43 2023-02-26 01:13:12.000000 otoole-1.0.1/docs/changelog.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    10307 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/conf.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    12076 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/contributing.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11733 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/data.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     8936 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/examples.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     8264 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/functionality.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1334 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/index.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1116 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/install.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       67 2023-02-26 01:13:12.000000 otoole-1.0.1/docs/license.rst
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      276 2023-02-26 03:45:17.000000 otoole-1.0.1/docs/requirements.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      355 2023-02-26 03:45:17.000000 otoole-1.0.1/pyproject.toml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      125 2023-04-20 01:42:03.000000 otoole-1.0.1/requirements.txt
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.726594 otoole-1.0.1/scripts/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      760 2023-02-26 01:13:12.000000 otoole-1.0.1/scripts/prepare_cbc.sh
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      824 2023-02-26 01:13:12.000000 otoole-1.0.1/scripts/prepare_cbc_short.sh
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1446 2023-04-20 01:53:27.806594 otoole-1.0.1/setup.cfg
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      703 2023-02-26 03:45:17.000000 otoole-1.0.1/setup.py
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.646593 otoole-1.0.1/src/
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.736594 otoole-1.0.1/src/otoole/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1059 2023-02-26 03:45:17.000000 otoole-1.0.1/src/otoole/__init__.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    15167 2023-03-31 16:26:19.000000 otoole-1.0.1/src/otoole/cli.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4184 2023-04-20 01:42:03.000000 otoole-1.0.1/src/otoole/exceptions.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    18250 2023-04-20 01:42:03.000000 otoole-1.0.1/src/otoole/input.py
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.756594 otoole-1.0.1/src/otoole/preprocess/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 01:13:12.000000 otoole-1.0.1/src/otoole/preprocess/__init__.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11432 2023-02-26 03:45:17.000000 otoole-1.0.1/src/otoole/preprocess/config.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2303 2023-02-26 03:45:17.000000 otoole-1.0.1/src/otoole/preprocess/longify_data.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1183 2023-02-26 03:45:17.000000 otoole-1.0.1/src/otoole/preprocess/setup.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5680 2023-02-26 03:45:17.000000 otoole-1.0.1/src/otoole/preprocess/validate_config.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    13306 2023-04-20 01:42:03.000000 otoole-1.0.1/src/otoole/read_strategies.py
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.766594 otoole-1.0.1/src/otoole/results/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        0 2023-02-26 01:13:12.000000 otoole-1.0.1/src/otoole/results/__init__.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    32615 2023-04-20 01:42:03.000000 otoole-1.0.1/src/otoole/results/result_package.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11163 2023-04-20 01:42:03.000000 otoole-1.0.1/src/otoole/results/results.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     8135 2023-02-26 03:45:17.000000 otoole-1.0.1/src/otoole/utils.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     6344 2023-02-26 03:45:17.000000 otoole-1.0.1/src/otoole/validate.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4207 2023-02-26 01:13:12.000000 otoole-1.0.1/src/otoole/validate.yaml
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.766594 otoole-1.0.1/src/otoole/visualise/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      328 2023-02-26 03:45:17.000000 otoole-1.0.1/src/otoole/visualise/__init__.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     7101 2023-02-26 03:45:17.000000 otoole-1.0.1/src/otoole/visualise/res.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     6685 2023-02-26 03:45:17.000000 otoole-1.0.1/src/otoole/write_strategies.py
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.756594 otoole-1.0.1/src/otoole.egg-info/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2387 2023-04-20 01:53:27.000000 otoole-1.0.1/src/otoole.egg-info/PKG-INFO
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2330 2023-04-20 01:53:27.000000 otoole-1.0.1/src/otoole.egg-info/SOURCES.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        1 2023-04-20 01:53:27.000000 otoole-1.0.1/src/otoole.egg-info/dependency_links.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       43 2023-04-20 01:53:27.000000 otoole-1.0.1/src/otoole.egg-info/entry_points.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        1 2023-04-20 01:53:27.000000 otoole-1.0.1/src/otoole.egg-info/not-zip-safe
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      175 2023-04-20 01:53:27.000000 otoole-1.0.1/src/otoole.egg-info/requires.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)        7 2023-04-20 01:53:27.000000 otoole-1.0.1/src/otoole.egg-info/top_level.txt
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.776594 otoole-1.0.1/tests/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     3649 2023-02-26 03:45:17.000000 otoole-1.0.1/tests/conftest.py
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.796594 otoole-1.0.1/tests/fixtures/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)   130205 2023-04-20 01:42:03.000000 otoole-1.0.1/tests/fixtures/combined_inputs.xlsx
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11432 2023-04-20 01:42:03.000000 otoole-1.0.1/tests/fixtures/config.yaml
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4827 2023-04-20 01:42:03.000000 otoole-1.0.1/tests/fixtures/config_r.yaml
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.796594 otoole-1.0.1/tests/fixtures/data/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      182 2023-02-26 03:45:17.000000 otoole-1.0.1/tests/fixtures/data/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)       29 2023-02-26 03:45:17.000000 otoole-1.0.1/tests/fixtures/data/AvailabilityFactor.csv
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    44422 2023-02-26 01:13:12.000000 otoole-1.0.1/tests/fixtures/simplicity-v0.2.1.zip
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    43735 2023-02-26 03:45:17.000000 otoole-1.0.1/tests/fixtures/simplicity.txt
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    75398 2023-02-26 01:13:12.000000 otoole-1.0.1/tests/fixtures/simplicity.xlsx
+drwxr-xr-x   0 trevorb1  (1000) trevorb1  (1000)        0 2023-04-20 01:53:27.806594 otoole-1.0.1/tests/results/
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    28520 2023-02-26 03:45:17.000000 otoole-1.0.1/tests/results/test_results_package.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     4802 2023-02-26 03:45:17.000000 otoole-1.0.1/tests/test_cli.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2149 2023-02-26 03:45:17.000000 otoole-1.0.1/tests/test_convert.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    18062 2023-04-20 01:42:03.000000 otoole-1.0.1/tests/test_input.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    41641 2023-04-20 01:42:03.000000 otoole-1.0.1/tests/test_read_strategies.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     1834 2023-02-26 03:45:17.000000 otoole-1.0.1/tests/test_setup.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5060 2023-04-20 01:42:03.000000 otoole-1.0.1/tests/test_utils.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     5223 2023-02-26 03:45:17.000000 otoole-1.0.1/tests/test_validate.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)    11600 2023-02-26 03:45:17.000000 otoole-1.0.1/tests/test_validate_config.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)      377 2023-02-26 03:45:17.000000 otoole-1.0.1/tests/test_visualise.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     6654 2023-02-26 03:45:17.000000 otoole-1.0.1/tests/test_write_strategies.py
+-rw-r--r--   0 trevorb1  (1000) trevorb1  (1000)     2553 2023-03-30 17:38:39.000000 otoole-1.0.1/tox.ini
```

### Comparing `otoole-1.0.0/.coveragerc` & `otoole-1.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/.gitignore` & `otoole-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/.pre-commit-config.yaml` & `otoole-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/.zenodo.json` & `otoole-1.0.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/CHANGELOG.rst` & `otoole-1.0.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/LICENSE.txt` & `otoole-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/PKG-INFO` & `otoole-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoole
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python toolkit to support use of OSeMOSYS
 Home-page: https://github.com/OSeMOSYS/otoole
 Author: Will Usher
 Author-email: wusher@kth.se
 License: MIT
 Project-URL: Documentation, https://otoole.readthedocs.io/en/latest/?badge=latest
 Platform: any
@@ -15,30 +15,30 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 ==================================================
 otoole: OSeMOSYS tools for energy work
 ==================================================
 
-.. image:: https://coveralls.io/repos/github/OSeMOSYS/otoole/badge.svg?branch=master
+.. image:: https://coveralls.io/repos/github/OSeMOSYS/otoole/badge.svg?branch=master&kill_cache=1
     :target: https://coveralls.io/github/OSeMOSYS/otoole?branch=master
 
 .. image:: https://readthedocs.org/projects/otoole/badge/?version=latest
     :target: https://otoole.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 A Python toolkit to support use of OSeMOSYS
 
 Description
 ===========
 
-OSeMOSYS tools for energy work, or **otoole**, is a Python package
+OSeMOSYS tools for energy work, or otoole, is a Python package
 which provides a command-line interface for users of OSeMOSYS. The aim of the
 package is to provide commonly used pre- and post-processing steps for OSeMOSYS.
 
 **otoole** aims to support different ways of storing input data and results,
 including csv files and Excel workbooks, as well as different implementations
 of the OSeMOSYS model. This improves interoperability of analyses and
 generally makes life a little bit easier.
@@ -54,15 +54,15 @@
 
 For instructions of the use of the tool, run the command line help function::
 
     otoole --help
 
 Documentation
 =============
-Detailed documentation of **otoole**, including examples, can be found here:
+Detailed documentation of otoole, including examples, can be found here:
 https://otoole.readthedocs.io/en/latest/
 
 Contributing
 ============
 
 New ideas and bugs `should be submitted <https://github.com/OSeMOSYS/otoole/issues/new>`_
 to the repository issue tracker. Please do contribute by discussing and developing these
```

### Comparing `otoole-1.0.0/README.rst` & `otoole-1.0.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ==================================================
 otoole: OSeMOSYS tools for energy work
 ==================================================
 
-.. image:: https://coveralls.io/repos/github/OSeMOSYS/otoole/badge.svg?branch=master
+.. image:: https://coveralls.io/repos/github/OSeMOSYS/otoole/badge.svg?branch=master&kill_cache=1
     :target: https://coveralls.io/github/OSeMOSYS/otoole?branch=master
 
 .. image:: https://readthedocs.org/projects/otoole/badge/?version=latest
     :target: https://otoole.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 A Python toolkit to support use of OSeMOSYS
 
 Description
 ===========
 
-OSeMOSYS tools for energy work, or **otoole**, is a Python package
+OSeMOSYS tools for energy work, or otoole, is a Python package
 which provides a command-line interface for users of OSeMOSYS. The aim of the
 package is to provide commonly used pre- and post-processing steps for OSeMOSYS.
 
 **otoole** aims to support different ways of storing input data and results,
 including csv files and Excel workbooks, as well as different implementations
 of the OSeMOSYS model. This improves interoperability of analyses and
 generally makes life a little bit easier.
@@ -37,15 +37,15 @@
 
 For instructions of the use of the tool, run the command line help function::
 
     otoole --help
 
 Documentation
 =============
-Detailed documentation of **otoole**, including examples, can be found here:
+Detailed documentation of otoole, including examples, can be found here:
 https://otoole.readthedocs.io/en/latest/
 
 Contributing
 ============
 
 New ideas and bugs `should be submitted <https://github.com/OSeMOSYS/otoole/issues/new>`_
 to the repository issue tracker. Please do contribute by discussing and developing these
```

### Comparing `otoole-1.0.0/citation.cff` & `otoole-1.0.1/CITATION.cff`

 * *Files 4% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     given-names: Hauke
     orcid: https://orcid.org/0000-0003-0098-8701
   - family-names: Muschner
     given-names: Christoph
     orcid: https://orcid.org/0000-0001-8144-5260
 title: "otoole: OSeMOSYS tools for energy work"
 version: 1.0.0
-doi: 10.5281/zenodo.4730003
-date-released: 2021-04-30
+doi: 10.5281/zenodo.7677990
+date-released: 2023-02-26
```

### Comparing `otoole-1.0.0/docs/Makefile` & `otoole-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/_static/OSeMOSYS.png` & `otoole-1.0.1/docs/_static/OSeMOSYS.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/_static/logo.png` & `otoole-1.0.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/_static/osemosys_dataflow.png` & `otoole-1.0.1/docs/_static/osemosys_dataflow.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/_static/otoole_figures.drawio` & `otoole-1.0.1/docs/_static/otoole_figures.drawio`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/_static/overview.png` & `otoole-1.0.1/docs/_static/overview.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/_static/overview_v2.png` & `otoole-1.0.1/docs/_static/overview_v2.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/_static/simplicity_res.png` & `otoole-1.0.1/docs/_static/simplicity_res.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/_static/validataion_model.png` & `otoole-1.0.1/docs/_static/validataion_model.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/_static/workflow.png` & `otoole-1.0.1/docs/_static/workflow.png`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/conf.py` & `otoole-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/contributing.rst` & `otoole-1.0.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/data.rst` & `otoole-1.0.1/docs/data.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/examples.rst` & `otoole-1.0.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/functionality.rst` & `otoole-1.0.1/docs/functionality.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/index.rst` & `otoole-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/docs/install.rst` & `otoole-1.0.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/scripts/prepare_cbc.sh` & `otoole-1.0.1/scripts/prepare_cbc.sh`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/scripts/prepare_cbc_short.sh` & `otoole-1.0.1/scripts/prepare_cbc_short.sh`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/setup.cfg` & `otoole-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	=src
 python_requires = >=3.8
 install_requires = 
 	xlrd
 	pyyaml
 	pydot
 	importlib_resources; python_version<'3.7'
-	pandas>=1.1
+	pandas>=1.1, <2.0
 	amply>=0.1.4
 	networkx
 	flatten_dict
 	openpyxl
 	pydantic
 
 [options.packages.find]
```

### Comparing `otoole-1.0.0/setup.py` & `otoole-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/src/otoole/__init__.py` & `otoole-1.0.1/src/otoole/__init__.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/src/otoole/cli.py` & `otoole-1.0.1/src/otoole/cli.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/src/otoole/exceptions.py` & `otoole-1.0.1/src/otoole/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -68,26 +68,28 @@
         self.message = message
         super().__init__(self.message)
 
     def __str__(self):
         return f"{self.name} -> {self.message}"
 
 
-class OtooleExcelNameMismatchError(OtooleException):
-    """Name mismatch between config and excel tabs."""
+class OtooleNameMismatchError(OtooleException):
+    """Names not consistent between read in data and config file"""
 
     def __init__(
-        self, excel_name: str, message: str = "Excel tab name not found in config file"
+        self,
+        name: str,
+        message: str = "Name not consistent between data and config file",
     ) -> None:
-        self.excel_name = excel_name
+        self.name = name
         self.message = message
         super().__init__(self.message)
 
     def __str__(self):
-        return f"{self.excel_name} -> {self.message}"
+        return f"{self.name} -> {self.message}"
 
 
 class OtooleDeprecationError(OtooleException):
     """New version of otoole does drops this feature support
 
     Arguments
     ---------
@@ -122,7 +124,49 @@
         message="Data already exists. Delete file/directory or pass the --overwrite flag",
     ):
         self.resource = resource
         self.message = message
 
     def __str__(self):
         return f"{self.resource} -> {self.message}"
+
+
+class OtooleIndexError(OtooleException):
+    """Index data not consistent between data and config file
+
+    Arguments
+    ---------
+    resource : str
+        Name of the resource which is invalid
+    config_indices: List[str]
+        Indices from config file
+    data_indices: List[str]
+        Indices from input data
+    """
+
+    def __init__(self, resource, config_indices, data_indices):
+        self.resource = resource
+        self.config_indices = config_indices
+        self.data_indices = data_indices
+        self.message = "Indices inconsistent between config and data"
+
+    def __str__(self):
+        return f"{self.resource} -> {self.message}. Config indices are {self.config_indices}. Data indices are {self.data_indices}."
+
+
+class OtooleError(OtooleException):
+    """General purpose error
+
+    Arguments
+    ---------
+    resource : str
+        Name of the resource which is invalid
+    message : str
+        Error message
+    """
+
+    def __init__(self, resource, message):
+        self.resource = resource
+        self.message = message
+
+    def __str__(self):
+        return f"{self.resource} -> {self.message}"
```

### Comparing `otoole-1.0.0/src/otoole/input.py` & `otoole-1.0.1/src/otoole/input.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 >>> converter.convert('my_datafile.txt', 'folder_of_csv_files')
 
 """
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
-from typing import Any, Dict, Optional, TextIO, Tuple, Union
+from typing import Any, Dict, List, Optional, TextIO, Tuple, Union
 
 import pandas as pd
 
+from otoole.exceptions import OtooleIndexError, OtooleNameMismatchError
+
 logger = logging.getLogger(__name__)
 
 
 class Context:
     """
     The Context defines the interface of interest to clients.
     """
@@ -120,18 +122,17 @@
     user_config : dict, default=None
         A user configuration for the input parameters and sets
     """
 
     def __init__(self, user_config: Dict[str, Dict]):
 
         self.user_config = user_config
-
-        # self.input_config = {
-        #     x: y for x, y in self.user_config.items() if y["type"] in ["param", 'set']
-        # }
+        self.input_config = {
+            x: y for x, y in self.user_config.items() if y["type"] in ["param", "set"]
+        }
         self.results_config = {
             x: y for x, y in self.user_config.items() if y["type"] == "result"
         }
 
     def _add_dtypes(self, config: Dict):
         for name, details in config.items():
             if details["type"] == "param":
@@ -380,49 +381,143 @@
             Dictionary and pandas DataFrames containing the OSeMOSYS parameters
         """
         for name, df in input_data.items():
 
             details = self.user_config[name]
 
             if details["type"] == "param":
-                logger.debug("Identified {} as a parameter".format(name))
-                try:
-                    df.set_index(details["indices"], inplace=True)
-                except KeyError:
-                    logger.debug("Unable to set index on {}".format(name))
-                    pass
+                self._check_param_index_names(name=name, config=details, df=df)
+            elif details["type"] == "set":
+                self._check_set_index_names(name=name, df=df)
 
-                logger.debug(
-                    "Column dtypes identified: {}".format(details["index_dtypes"])
-                )
-                logger.debug(df.head())
-                # Drop empty rows
-                df = (
-                    df.dropna(axis=0, how="all")
-                    .reset_index()
-                    .astype(details["index_dtypes"])
-                    .set_index(details["indices"])
-                )
-            else:
-                logger.debug("Identified {} as a set".format(name))
-                df = df.astype(details["dtype"])
+            df = self._check_index_dtypes(name=name, config=details, df=df)
 
             input_data[name] = df
 
         return input_data
 
+    @staticmethod
+    def _check_param_index_names(
+        name: str, config: Dict[str, Any], df: pd.DataFrame
+    ) -> None:
+        """Checks parameter index names input data against config file
+
+        Arguments
+        ---------
+        name: str
+            Name of parameter
+        config: Dict[str,Any]
+            Configuration file data for the parameter
+        df: pd.DataFrame
+            Data read in for the parameter
+
+        Raises
+        ------
+        OtooleIndexError
+            If actual indices do not match expected indices
+        """
+
+        actual_indices = df.index.names
+        if actual_indices[0] is None:  # for ReadMemory
+            logger.debug(f"No mulit-index identified for {name}")
+            actual_indices = list(df)[:-1]  # Drop "VALUE"
+
+        logger.debug(f"Actual indices for {name} are {actual_indices}")
+        try:
+            expected_indices = config["indices"]
+            logger.debug(f"Expected indices for {name} are {expected_indices}")
+        except KeyError:
+            logger.debug(f"No expected indices identifed for {name}")
+            return
+
+        if actual_indices == expected_indices:
+            return
+        else:
+            raise OtooleIndexError(
+                resource=name,
+                config_indices=expected_indices,
+                data_indices=actual_indices,
+            )
+
+    @staticmethod
+    def _check_set_index_names(name: str, df: pd.DataFrame) -> None:
+        """Checks for proper set index name
+
+        Arguments
+        ---------
+        name: str
+            Name of set
+        df: pd.DataFrame
+            Data read in for the parameter
+
+        Raises
+        ------
+        OtooleIndexError
+            If actual indices do not match expected indices
+        """
+        if not df.columns == ["VALUE"]:
+            raise OtooleIndexError(
+                resource=name,
+                config_indices=["VALUE"],
+                data_indices=df.columns,
+            )
+
+    @staticmethod
+    def _check_index_dtypes(
+        name: str, config: Dict[str, Any], df: pd.DataFrame
+    ) -> pd.DataFrame:
+        """Checks datatypes of input data against config file
+
+        Arguments
+        ---------
+        name: str
+            Name of parameter
+        config: Dict[str,Any]
+            Configuration file data for the parameter
+        df: pd.DataFrame
+            Data read in for the parameter
+
+        Returns
+        -------
+        pd.DataFrame
+            input_data with corrected datatypes
+        """
+
+        if config["type"] == "param":
+            logger.debug("Identified {} as a parameter".format(name))
+            try:
+                df.set_index(config["indices"], inplace=True)
+            except KeyError:
+                logger.debug("Unable to set index on {}".format(name))
+                pass
+
+            logger.debug("Column dtypes identified: {}".format(config["index_dtypes"]))
+            logger.debug(df.head())
+            # Drop empty rows
+            df = (
+                df.dropna(axis=0, how="all")
+                .reset_index()
+                .astype(config["index_dtypes"])
+                .set_index(config["indices"])
+            )
+        else:
+            logger.debug("Identified {} as a set".format(name))
+            df = df.astype(config["dtype"])
+
+        return df
+
     def _get_missing_input_dataframes(
         self, input_data: Dict[str, pd.DataFrame], config_type: str
     ) -> Dict[str, pd.DataFrame]:
         """Creates empty dataframes if user config data does not exist
 
         Arguments:
         ----------
         input_data: Dict[str, pd.DataFrame]
-            Data read in from the excel notebook
+            Internal datastore
         config_type: str
             Type of value. Must be "set", "param", or "result"
 
         Returns:
         --------
         all_params: Dict[str, pd.DataFrame]
             Input data plus empty dataframes
@@ -446,12 +541,45 @@
             except KeyError:  # set condition
                 df = pd.DataFrame()
             df["VALUE"] = ""
             input_data[value] = df
 
         return input_data
 
+    def _compare_read_to_expected(
+        self, names: List[str], short_names: bool = False
+    ) -> None:
+        """Compares input data definitions to config file definitions
+
+        Arguments:
+        ---------
+        names: List[str]
+            Parameter and set names read in
+        map_names: bool = False
+            If should be checking short_names from config file
+
+        Raises:
+        -------
+        OtooleNameMismatchError
+            If the info in the data and config file do not match
+        """
+        user_config = self.input_config
+        if short_names:
+            expected = []
+            for name in user_config:
+                try:
+                    expected.append(user_config[name]["short_name"])
+                except KeyError:
+                    expected.append(name)
+        else:
+            expected = [x for x in user_config]
+
+        errors = list(set(expected).symmetric_difference(set(names)))
+        if errors:
+            logger.debug(f"data and config name errors are: {errors}")
+            raise OtooleNameMismatchError(name=errors[0])
+
     @abstractmethod
     def read(
         self, filepath: Union[str, TextIO], **kwargs
     ) -> Tuple[Dict[str, pd.DataFrame], Dict[str, Any]]:
         raise NotImplementedError()
```

### Comparing `otoole-1.0.0/src/otoole/preprocess/config.yaml` & `otoole-1.0.1/src/otoole/preprocess/config.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/src/otoole/preprocess/longify_data.py` & `otoole-1.0.1/src/otoole/preprocess/longify_data.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/src/otoole/preprocess/setup.py` & `otoole-1.0.1/src/otoole/preprocess/setup.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/src/otoole/preprocess/validate_config.py` & `otoole-1.0.1/src/otoole/preprocess/validate_config.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/src/otoole/read_strategies.py` & `otoole-1.0.1/src/otoole/read_strategies.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from typing import Any, Dict, List, Optional, TextIO, Tuple, Union
 
 import pandas as pd
 from amply import Amply
 from flatten_dict import flatten
 
-from otoole.exceptions import OtooleDeprecationError, OtooleExcelNameMismatchError
+from otoole.exceptions import OtooleDeprecationError, OtooleError
 from otoole.input import ReadStrategy
 from otoole.preprocess.longify_data import check_datatypes, check_set_datatype
 from otoole.utils import create_name_mappings
 
 logger = logging.getLogger(__name__)
 
 
@@ -41,58 +41,59 @@
     def _check_set(self, df: pd.DataFrame, config_details: Dict, name: str):
 
         logger.info("Checking set %s", name)
         narrow = df
 
         return narrow
 
-    def _check_parameter(self, df: pd.DataFrame, expected_headers: List, name: str):
+    def _convert_wide_2_narrow(self, df: pd.DataFrame, name: str):
         """Converts a dataframe from wide to narrow format
 
         Arguments
         ---------
         df: pd.DataFrame
         expected_headers: List
         name: str
         """
-        actual_headers = df.columns
-        logger.debug("Expected headers for %s: %s", name, expected_headers)
-
-        if "REGION" in expected_headers and "REGION" not in actual_headers:
-            raise ValueError("No REGION column provided for %s", name)
+        actual_headers = list(df.columns)
 
         if "MODEOFOPERATION" in actual_headers:
             df = df.rename(columns={"MODEOFOPERATION": "MODE_OF_OPERATION"})
 
         if actual_headers[-1] == "VALUE":
             logger.info(
-                "%s is already in narrow form with headers %s", name, df.columns
+                f"{name} is already in narrow form with headers {actual_headers}"
             )
             narrow = df
+            converted_headers = actual_headers[:-1]  # remove "VALUE"
         else:
             try:
+                converted_headers = [
+                    x for x in actual_headers if not isinstance(x, int)
+                ]
+                converted_headers += ["YEAR"]
+                if "VALUE" in converted_headers:
+                    raise OtooleError(
+                        resource=name,
+                        message="'VALUE' can not be a header in wide format data",
+                    )
                 narrow = pd.melt(
                     df,
-                    id_vars=expected_headers[:-1],
-                    var_name=expected_headers[-1],  # Normally 'YEAR'
+                    id_vars=converted_headers[:-1],
+                    var_name=converted_headers[-1],  # Normally 'YEAR'
                     value_name="new_VALUE",
                 )
                 narrow = narrow.rename(columns={"new_VALUE": "VALUE"})
+                logger.info(f"{name} reshaped from wide to narrow format")
             except IndexError as ex:
-                logger.debug("Could not reshape %s", df.columns)
+                logger.debug(f"Could not reshape {name}")
                 raise ex
 
-        all_headers = expected_headers + ["VALUE"]
-        for column in all_headers:
-            if column not in narrow.columns:
-                logger.warning("%s not in header of %s", column, name)
-
-        logger.debug("Final all headers for %s: %s", name, all_headers)
-
-        return narrow[all_headers].set_index(expected_headers)
+        all_headers = converted_headers + ["VALUE"]
+        return narrow[all_headers].set_index(converted_headers)
 
     def _whitespace_converter(self, indices: List[str]) -> Dict[str, Any]:
         """Creates converter for striping whitespace in dataframe
 
         Arguments
         ---------
         indicies: List[str]
@@ -117,16 +118,15 @@
     ) -> Tuple[Dict[str, pd.DataFrame], Dict[str, Any]]:
 
         config = self.user_config
         default_values = self._read_default_values(config)
         excel_to_csv = create_name_mappings(config, map_full_to_short=False)
 
         xl = pd.ExcelFile(filepath, engine="openpyxl")
-
-        self._check_input_sheet_names(xl.sheet_names)
+        self._compare_read_to_expected(names=xl.sheet_names, short_names=True)
 
         input_data = {}
 
         for name in xl.sheet_names:
 
             try:
                 mod_name = excel_to_csv[name]
@@ -136,81 +136,58 @@
             config_details = config[mod_name]
 
             df = xl.parse(name)
 
             entity_type = config[mod_name]["type"]
 
             if entity_type == "param":
-                narrow = self._check_parameter(df, config_details["indices"], mod_name)
+                narrow = self._convert_wide_2_narrow(df, mod_name)
             elif entity_type == "set":
                 narrow = self._check_set(df, config_details, mod_name)
 
             input_data[mod_name] = narrow
 
         for config_type in ["param", "set"]:
             input_data = self._get_missing_input_dataframes(
                 input_data, config_type=config_type
             )
 
         input_data = self._check_index(input_data)
 
         return input_data, default_values
 
-    def _check_input_sheet_names(self, sheet_names: List[str]) -> None:
-        """Checks that excel sheet names are in the config file.
-
-        Arguments:
-        ---------
-        sheet_names: list[str]
-            Sheet names from the excel file
-
-        Raises:
-        -------
-        OtooleExcelNameMismatchError
-            If the sheet name is not found in the config files parameter or
-            'short_name' parameter
-        """
-        user_config = self.user_config
-        csv_to_excel = create_name_mappings(user_config)
-        config_param_names = []
-        for name in user_config:
-            try:
-                config_param_names.append(csv_to_excel[name])
-            except KeyError:
-                config_param_names.append(name)
-
-        for sheet_name in sheet_names:
-            if sheet_name not in config_param_names:
-                raise OtooleExcelNameMismatchError(excel_name=sheet_name)
-
 
 class ReadCsv(_ReadTabular):
     """Read in a folder of CSV files"""
 
     def read(
         self, filepath, **kwargs
     ) -> Tuple[Dict[str, pd.DataFrame], Dict[str, Any]]:
 
         input_data = {}
 
         self._check_for_default_values_csv(filepath)
+        self._compare_read_to_expected(
+            names=[f.split(".csv")[0] for f in os.listdir(filepath)]
+        )
+
         default_values = self._read_default_values(self.user_config)
 
         for parameter, details in self.user_config.items():
             logger.info("Looking for %s", parameter)
 
             entity_type = details["type"]
             try:
                 converter = self._whitespace_converter(details["indices"])
             except KeyError:  # sets don't have indices def
                 converter = self._whitespace_converter(["VALUE"])
 
             if entity_type == "param":
                 df = self._get_input_data(filepath, parameter, details, converter)
-                narrow = self._check_parameter(df, details["indices"], parameter)
+                narrow = self._convert_wide_2_narrow(df, parameter)
                 if not narrow.empty:
                     narrow_checked = check_datatypes(
                         narrow, self.user_config, parameter
                     )
                 else:
                     narrow_checked = narrow
```

### Comparing `otoole-1.0.0/src/otoole/results/result_package.py` & `otoole-1.0.1/src/otoole/results/result_package.py`

 * *Files 0% similar despite different names*

```diff
@@ -854,14 +854,15 @@
         param DiscountFactorMid{r in REGION, y in YEAR} :=
                 (1 + DiscountRate[r]) ^ (y - min{yy in YEAR} min(yy) + 0.5);
     """
 
     if regions and years:
         discount_rate["YEAR"] = [years]
         discount_factor = discount_rate.explode("YEAR").reset_index(level="REGION")
+        discount_factor["YEAR"] = discount_factor["YEAR"].astype(int)
         discount_factor["NUM"] = discount_factor["YEAR"] - discount_factor["YEAR"].min()
         discount_factor["RATE"] = discount_factor["VALUE"] + 1
         discount_factor["VALUE"] = (
             discount_factor["RATE"].pow(discount_factor["NUM"] + adj).astype(float)
         )
         return discount_factor.reset_index()[["REGION", "YEAR", "VALUE"]].set_index(
             ["REGION", "YEAR"]
```

### Comparing `otoole-1.0.0/src/otoole/results/results.py` & `otoole-1.0.1/src/otoole/results/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,15 @@
             file_path,
             header=None,
             sep=" ",
             names=["Variable", "Value"],
             skiprows=2,
         )  # type: pd.DataFrame
         df[["Variable", "Index"]] = df["Variable"].str.split("(", expand=True)
-        df["Index"] = df["Index"].str.replace(")", "", regex=True)
+        df["Index"] = df["Index"].str.replace(")", "")
         LOGGER.debug(df)
         df = df[(df["Value"] != 0)].reset_index()
         return df[["Variable", "Index", "Value"]].astype({"Value": float})
 
 
 class ReadCbc(ReadResultsCBC):
     """Read a CBC solution file into memory
@@ -321,10 +321,10 @@
         df["Variable"] = (
             df["Variable"]
             .astype(str)
             .str.replace(r"^\*\*", "", regex=True)
             .str.split(expand=True)[1]
         )
         df[["Index", "Value"]] = df["indexvalue"].str.split(expand=True).loc[:, 0:1]
-        df["Index"] = df["Index"].str.replace(")", "", regex=True)
+        df["Index"] = df["Index"].str.replace(")", "")
         df = df.drop(columns=["indexvalue"])
         return df[["Variable", "Index", "Value"]].astype({"Value": float})
```

### Comparing `otoole-1.0.0/src/otoole/utils.py` & `otoole-1.0.1/src/otoole/utils.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/src/otoole/validate.py` & `otoole-1.0.1/src/otoole/validate.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/src/otoole/validate.yaml` & `otoole-1.0.1/src/otoole/validate.yaml`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/src/otoole/visualise/res.py` & `otoole-1.0.1/src/otoole/visualise/res.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/src/otoole/write_strategies.py` & `otoole-1.0.1/src/otoole/write_strategies.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/src/otoole.egg-info/PKG-INFO` & `otoole-1.0.1/src/otoole.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoole
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python toolkit to support use of OSeMOSYS
 Home-page: https://github.com/OSeMOSYS/otoole
 Author: Will Usher
 Author-email: wusher@kth.se
 License: MIT
 Project-URL: Documentation, https://otoole.readthedocs.io/en/latest/?badge=latest
 Platform: any
@@ -15,30 +15,30 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 ==================================================
 otoole: OSeMOSYS tools for energy work
 ==================================================
 
-.. image:: https://coveralls.io/repos/github/OSeMOSYS/otoole/badge.svg?branch=master
+.. image:: https://coveralls.io/repos/github/OSeMOSYS/otoole/badge.svg?branch=master&kill_cache=1
     :target: https://coveralls.io/github/OSeMOSYS/otoole?branch=master
 
 .. image:: https://readthedocs.org/projects/otoole/badge/?version=latest
     :target: https://otoole.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 A Python toolkit to support use of OSeMOSYS
 
 Description
 ===========
 
-OSeMOSYS tools for energy work, or **otoole**, is a Python package
+OSeMOSYS tools for energy work, or otoole, is a Python package
 which provides a command-line interface for users of OSeMOSYS. The aim of the
 package is to provide commonly used pre- and post-processing steps for OSeMOSYS.
 
 **otoole** aims to support different ways of storing input data and results,
 including csv files and Excel workbooks, as well as different implementations
 of the OSeMOSYS model. This improves interoperability of analyses and
 generally makes life a little bit easier.
@@ -54,15 +54,15 @@
 
 For instructions of the use of the tool, run the command line help function::
 
     otoole --help
 
 Documentation
 =============
-Detailed documentation of **otoole**, including examples, can be found here:
+Detailed documentation of otoole, including examples, can be found here:
 https://otoole.readthedocs.io/en/latest/
 
 Contributing
 ============
 
 New ideas and bugs `should be submitted <https://github.com/OSeMOSYS/otoole/issues/new>`_
 to the repository issue tracker. Please do contribute by discussing and developing these
```

### Comparing `otoole-1.0.0/src/otoole.egg-info/SOURCES.txt` & `otoole-1.0.1/src/otoole.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,27 @@
 .gitignore
 .isort.cfg
 .pre-commit-config.yaml
 .readthedocs.yml
 .zenodo.json
 AUTHORS.rst
 CHANGELOG.rst
+CITATION.cff
 LICENSE.txt
 README.rst
-citation.cff
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
+.github/pull_request_template.md
+.github/ISSUE_TEMPLATE/bug_report.yaml
+.github/ISSUE_TEMPLATE/docs.yaml
+.github/ISSUE_TEMPLATE/feature.yaml
+.github/workflows/citation.yaml
 .github/workflows/python.yaml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/data.rst
```

### Comparing `otoole-1.0.0/tests/conftest.py` & `otoole-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/tests/fixtures/config.yaml` & `otoole-1.0.1/tests/fixtures/config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -80,19 +80,14 @@
     dtype: float
     default: 1
 DiscountRate:
     indices: [REGION]
     type: param
     dtype: float
     default: 0.05
-DiscountRateIdv:
-    indices: [REGION,TECHNOLOGY]
-    type: param
-    dtype: float
-    default: 0.05
 DiscountRateStorage:
     indices: [REGION,STORAGE]
     type: param
     dtype: float
     default: 0.05
 EMISSION:
     dtype: str
```

### Comparing `otoole-1.0.0/tests/fixtures/config_r.yaml` & `otoole-1.0.1/tests/fixtures/config_r.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -198,10 +198,7 @@
     calculated: False
 UseByTechnology:
     indices: [REGION, TIMESLICE, TECHNOLOGY, FUEL, YEAR]
     type: result
     dtype: float
     default: 0
     calculated: False
-_REGION:
-    type: set
-    dtype: str
```

### Comparing `otoole-1.0.0/tests/fixtures/simplicity-v0.2.1.zip` & `otoole-1.0.1/tests/fixtures/simplicity-v0.2.1.zip`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/tests/fixtures/simplicity.txt` & `otoole-1.0.1/tests/fixtures/simplicity.txt`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/tests/fixtures/simplicity.xlsx` & `otoole-1.0.1/tests/fixtures/simplicity.xlsx`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/tests/results/test_results_package.py` & `otoole-1.0.1/tests/results/test_results_package.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/tests/test_cli.py` & `otoole-1.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/tests/test_convert.py` & `otoole-1.0.1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/tests/test_read_strategies.py` & `otoole-1.0.1/tests/test_read_strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List
 
 import pandas as pd
 from amply import Amply
 from pytest import mark, raises
 
 from otoole import ReadCsv, ReadDatafile, ReadExcel, ReadMemory
-from otoole.exceptions import OtooleDeprecationError
+from otoole.exceptions import OtooleDeprecationError, OtooleError
 from otoole.preprocess.longify_data import check_datatypes
 from otoole.results.results import (
     ReadCbc,
     ReadCplex,
     ReadGurobi,
     check_for_duplicates,
     identify_duplicate,
@@ -941,42 +941,25 @@
             0.071232876,
             0.071232876,
             0.071232876,
         ]
 
         assert (actual_data == expected).all()
 
-    def test_read_excel_discount_rate(self, user_config):
-        """Tests that parameters not in excel are saved in datastore"""
-
-        spreadsheet = os.path.join("tests", "fixtures", "combined_inputs.xlsx")
-        xl = pd.ExcelFile(spreadsheet, engine="openpyxl")
-
-        # checks that fixture does not contian discount rate data
-        assert "DiscountRateIdv" not in xl.sheet_names
-
-        reader = ReadExcel(user_config=user_config)
-        actual, _ = reader.read(spreadsheet)
-
-        # checks that discount rate has data after reading in excel data
-        assert "DiscountRateIdv" in actual
-        assert actual["DiscountRateIdv"].empty
-
     def test_narrow_parameters(self, user_config):
         data = [
             ["IW0016", 0.238356164, 0.238356164, 0.238356164],
             ["IW1624", 0.119178082, 0.119178082, 0.119178082],
             ["IH0012", 0.071232876, 0.071232876, 0.071232876],
         ]
         df = pd.DataFrame(data, columns=["TIMESLICE", 2017, 2018, 2019])
-        config_details = ["TIMESLICE", "YEAR"]
         name = "YearSplit"
 
         reader = ReadExcel(user_config=user_config)
-        actual = reader._check_parameter(df, config_details, name)
+        actual = reader._convert_wide_2_narrow(df, name)
         data = [
             ["IW0016", 2017, 0.238356164],
             ["IW1624", 2017, 0.119178082],
             ["IH0012", 2017, 0.071232876],
             ["IW0016", 2018, 0.238356164],
             ["IW1624", 2018, 0.119178082],
             ["IH0012", 2018, 0.071232876],
@@ -987,14 +970,25 @@
         expected = (
             pd.DataFrame(data, columns=["TIMESLICE", "YEAR", "VALUE"])
             .astype({"YEAR": "object"})
             .set_index(["TIMESLICE", "YEAR"])
         )
         pd.testing.assert_frame_equal(actual, expected)
 
+    def test_invalid_column_name(self, user_config):
+        data = [
+            ["ELC", "IW0016", 0.238356164, 0.238356164, 0.238356164],
+            ["ELC", "IW1624", 0.119178082, 0.119178082, 0.119178082],
+            ["ELC", "IH0012", 0.071232876, 0.071232876, 0.071232876],
+        ]
+        df = pd.DataFrame(data, columns=["VALUE", "TIMESLICE", 2017, 2018, 2019])
+        reader = ReadExcel(user_config=user_config)
+        with raises(OtooleError):
+            reader._convert_wide_2_narrow(df=df, name="example")
+
     def test_check_index(self, user_config):
 
         data = [
             ["IW0016", 2017, 0.238356164],
             ["IW0016", 2018, 0.238356164],
             ["IW0016", 2019, 0.238356164],
             ["IW1624", 2017, 0.119178082],
```

### Comparing `otoole-1.0.0/tests/test_setup.py` & `otoole-1.0.1/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/tests/test_utils.py` & `otoole-1.0.1/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from tempfile import NamedTemporaryFile
 
 import pandas as pd
 import pytest
 import yaml
 
-from otoole.exceptions import (
-    OtooleDeprecationError,
-    OtooleExcelNameLengthError,
-    OtooleExcelNameMismatchError,
-)
-from otoole.read_strategies import ReadExcel
+from otoole.exceptions import OtooleDeprecationError, OtooleExcelNameLengthError
 from otoole.utils import (
     UniqueKeyLoader,
     create_name_mappings,
     read_deprecated_datapackage,
 )
 from otoole.write_strategies import WriteExcel
 
@@ -67,21 +62,14 @@
             "TotalTechnologyModelPeriodActLo": "TotalTechnologyModelPeriodActivityLowerLimit",
             "TotalTechnologyModelPeriodActUp": "TotalTechnologyModelPeriodActivityUpperLimit",
         }
         actual = create_name_mappings(user_config, map_full_to_short=False)
         assert actual == expected
 
 
-def test_excel_name_mismatch_error(user_config):
-    read_excel = ReadExcel(user_config=user_config)
-    sheet_names = ["AccumulatedAnnualDemand", "MismatchSheet"]
-    with pytest.raises(OtooleExcelNameMismatchError):
-        read_excel._check_input_sheet_names(sheet_names=sheet_names)
-
-
 user_config_name_errors = ["user_config_long_param_name", "user_config_long_short_name"]
 
 
 @pytest.mark.parametrize(
     "user_config_simple",
     user_config_name_errors,
     ids=["full_name_error", "short_name_error"],
```

### Comparing `otoole-1.0.0/tests/test_validate.py` & `otoole-1.0.1/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/tests/test_validate_config.py` & `otoole-1.0.1/tests/test_validate_config.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/tests/test_write_strategies.py` & `otoole-1.0.1/tests/test_write_strategies.py`

 * *Files identical despite different names*

### Comparing `otoole-1.0.0/tox.ini` & `otoole-1.0.1/tox.ini`

 * *Files identical despite different names*

