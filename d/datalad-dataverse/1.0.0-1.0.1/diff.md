# Comparing `tmp/datalad_dataverse-1.0.0.tar.gz` & `tmp/datalad_dataverse-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad_dataverse-1.0.0.tar", last modified: Fri Mar 17 20:14:31 2023, max compression
+gzip compressed data, was "datalad_dataverse-1.0.1.tar", last modified: Thu Apr 20 09:34:50 2023, max compression
```

## Comparing `datalad_dataverse-1.0.0.tar` & `datalad_dataverse-1.0.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 20:14:31.124762 datalad_dataverse-1.0.0/
--rw-rw-r--   0 mih       (1000) mih       (1000)      101 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/CONTRIBUTORS
--rw-rw-r--   0 mih       (1000) mih       (1000)     1300 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/LICENSE
--rw-rw-r--   0 mih       (1000) mih       (1000)      148 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/MANIFEST.in
--rw-rw-r--   0 mih       (1000) mih       (1000)    10800 2023-03-17 20:14:31.124762 datalad_dataverse-1.0.0/PKG-INFO
--rw-rw-r--   0 mih       (1000) mih       (1000)    10292 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/README.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 20:14:31.120762 datalad_dataverse-1.0.0/_datalad_buildsupport/
--rw-rw-r--   0 mih       (1000) mih       (1000)      529 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/_datalad_buildsupport/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10698 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/_datalad_buildsupport/formatters.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8530 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/_datalad_buildsupport/setup.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 20:14:31.124762 datalad_dataverse-1.0.0/datalad_dataverse/
--rw-rw-r--   0 mih       (1000) mih       (1000)     1768 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      497 2023-03-17 20:14:31.124762 datalad_dataverse-1.0.0/datalad_dataverse/_version.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    16052 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/add_sibling_dataverse.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    16263 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/baseremote.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      522 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/conftest.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    18285 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/dataset.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4337 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/remote.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 20:14:31.120762 datalad_dataverse-1.0.0/datalad_dataverse/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3265 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/tests/fixtures.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     7544 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/tests/test_add_sibling_dataverse.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8604 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/tests/test_dataset.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5960 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/tests/test_pydataverse.py
--rw-rw-r--   0 mih       (1000) mih       (1000)       98 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/tests/test_register.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5300 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/tests/test_remote.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3365 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/tests/test_remote_xdlra.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2287 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/tests/test_utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4022 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/tests/utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10553 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/datalad_dataverse/utils.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 20:14:31.120762 datalad_dataverse-1.0.0/datalad_dataverse.egg-info/
--rw-rw-r--   0 mih       (1000) mih       (1000)    10800 2023-03-17 20:14:31.000000 datalad_dataverse-1.0.0/datalad_dataverse.egg-info/PKG-INFO
--rw-rw-r--   0 mih       (1000) mih       (1000)     1872 2023-03-17 20:14:31.000000 datalad_dataverse-1.0.0/datalad_dataverse.egg-info/SOURCES.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)        1 2023-03-17 20:14:31.000000 datalad_dataverse-1.0.0/datalad_dataverse.egg-info/dependency_links.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)      143 2023-03-17 20:14:31.000000 datalad_dataverse-1.0.0/datalad_dataverse.egg-info/entry_points.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)       75 2023-03-17 20:14:31.000000 datalad_dataverse-1.0.0/datalad_dataverse.egg-info/requires.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)       18 2023-03-17 20:14:31.000000 datalad_dataverse-1.0.0/datalad_dataverse.egg-info/top_level.txt
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 20:14:31.120762 datalad_dataverse-1.0.0/docs/
--rw-rw-r--   0 mih       (1000) mih       (1000)     7516 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/Makefile
--rw-rw-r--   0 mih       (1000) mih       (1000)     1755 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/README.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 20:14:31.120762 datalad_dataverse-1.0.0/docs/source/
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 20:14:31.120762 datalad_dataverse-1.0.0/docs/source/_static/
--rw-rw-r--   0 mih       (1000) mih       (1000)   284086 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/_static/clueless.gif
--rw-rw-r--   0 mih       (1000) mih       (1000)      958 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/_static/datalad_logo.png
--rw-rw-r--   0 mih       (1000) mih       (1000)   233264 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/_static/logo.png
--rw-rw-r--   0 mih       (1000) mih       (1000)    46658 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/_static/logo.svg
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 20:14:31.124762 datalad_dataverse-1.0.0/docs/source/_static/tutorial/
--rw-rw-r--   0 mih       (1000) mih       (1000)    61940 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_add_dataset.png
--rw-rw-r--   0 mih       (1000) mih       (1000)    56532 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_add_dataset_2.png
--rw-rw-r--   0 mih       (1000) mih       (1000)   104326 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_dataset_annex.png
--rw-rw-r--   0 mih       (1000) mih       (1000)   112116 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_dataset_filetree.png
--rw-rw-r--   0 mih       (1000) mih       (1000)   126165 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_obtain_doi.png
--rw-rw-r--   0 mih       (1000) mih       (1000)    60438 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_publish_ds.png
--rw-rw-r--   0 mih       (1000) mih       (1000)    50746 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_token.png
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 20:14:31.120762 datalad_dataverse-1.0.0/docs/source/_templates/
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 20:14:31.124762 datalad_dataverse-1.0.0/docs/source/_templates/autosummary/
--rw-rw-r--   0 mih       (1000) mih       (1000)      436 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/_templates/autosummary/module.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      168 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/cmdline.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)     4870 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/conf.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      358 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/contributing.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)     1326 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/glossary.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)     2023 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/index.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)     6360 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/intro.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      918 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/links.inc
--rw-rw-r--   0 mih       (1000) mih       (1000)      516 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/modref.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)     5895 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/settingup.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)    11236 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/docs/source/tutorial.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)       60 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/pyproject.toml
--rw-rw-r--   0 mih       (1000) mih       (1000)     1151 2023-03-17 20:14:31.124762 datalad_dataverse-1.0.0/setup.cfg
--rwxrwxr-x   0 mih       (1000) mih       (1000)      369 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/setup.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    81295 2023-03-17 20:14:27.000000 datalad_dataverse-1.0.0/versioneer.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-04-20 09:34:50.185963 datalad_dataverse-1.0.1/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      101 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/CONTRIBUTORS
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1300 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/LICENSE
+-rw-rw-r--   0 mih       (1000) mih       (1000)      148 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/MANIFEST.in
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11176 2023-04-20 09:34:50.185963 datalad_dataverse-1.0.1/PKG-INFO
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10668 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/README.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-04-20 09:34:50.181963 datalad_dataverse-1.0.1/_datalad_buildsupport/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      529 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/_datalad_buildsupport/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10698 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/_datalad_buildsupport/formatters.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8530 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/_datalad_buildsupport/setup.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-04-20 09:34:50.185963 datalad_dataverse-1.0.1/datalad_dataverse/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1768 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      497 2023-04-20 09:34:50.185963 datalad_dataverse-1.0.1/datalad_dataverse/_version.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16085 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/add_sibling_dataverse.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16263 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/baseremote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      522 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/conftest.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    18285 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/dataset.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4337 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/remote.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-04-20 09:34:50.185963 datalad_dataverse-1.0.1/datalad_dataverse/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3265 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/tests/fixtures.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7544 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/tests/test_add_sibling_dataverse.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8604 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/tests/test_dataset.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5960 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/tests/test_pydataverse.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)       98 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/tests/test_register.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5300 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/tests/test_remote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3365 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/tests/test_remote_xdlra.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2287 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/tests/test_utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4637 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/tests/utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10553 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/datalad_dataverse/utils.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-04-20 09:34:50.181963 datalad_dataverse-1.0.1/datalad_dataverse.egg-info/
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11176 2023-04-20 09:34:50.000000 datalad_dataverse-1.0.1/datalad_dataverse.egg-info/PKG-INFO
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1872 2023-04-20 09:34:50.000000 datalad_dataverse-1.0.1/datalad_dataverse.egg-info/SOURCES.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)        1 2023-04-20 09:34:50.000000 datalad_dataverse-1.0.1/datalad_dataverse.egg-info/dependency_links.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)      143 2023-04-20 09:34:50.000000 datalad_dataverse-1.0.1/datalad_dataverse.egg-info/entry_points.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)       75 2023-04-20 09:34:50.000000 datalad_dataverse-1.0.1/datalad_dataverse.egg-info/requires.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)       18 2023-04-20 09:34:50.000000 datalad_dataverse-1.0.1/datalad_dataverse.egg-info/top_level.txt
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-04-20 09:34:50.185963 datalad_dataverse-1.0.1/docs/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7516 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/Makefile
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1755 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/README.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-04-20 09:34:50.185963 datalad_dataverse-1.0.1/docs/source/
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-04-20 09:34:50.185963 datalad_dataverse-1.0.1/docs/source/_static/
+-rw-rw-r--   0 mih       (1000) mih       (1000)   284086 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/_static/clueless.gif
+-rw-rw-r--   0 mih       (1000) mih       (1000)      958 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/_static/datalad_logo.png
+-rw-rw-r--   0 mih       (1000) mih       (1000)   233264 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/_static/logo.png
+-rw-rw-r--   0 mih       (1000) mih       (1000)    46658 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/_static/logo.svg
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-04-20 09:34:50.185963 datalad_dataverse-1.0.1/docs/source/_static/tutorial/
+-rw-rw-r--   0 mih       (1000) mih       (1000)    61940 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_add_dataset.png
+-rw-rw-r--   0 mih       (1000) mih       (1000)    56532 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_add_dataset_2.png
+-rw-rw-r--   0 mih       (1000) mih       (1000)   104326 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_dataset_annex.png
+-rw-rw-r--   0 mih       (1000) mih       (1000)   112116 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_dataset_filetree.png
+-rw-rw-r--   0 mih       (1000) mih       (1000)   126165 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_obtain_doi.png
+-rw-rw-r--   0 mih       (1000) mih       (1000)    60438 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_publish_ds.png
+-rw-rw-r--   0 mih       (1000) mih       (1000)    50746 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_token.png
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-04-20 09:34:50.181963 datalad_dataverse-1.0.1/docs/source/_templates/
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-04-20 09:34:50.185963 datalad_dataverse-1.0.1/docs/source/_templates/autosummary/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      436 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/_templates/autosummary/module.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      168 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/cmdline.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4870 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/conf.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      358 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/contributing.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1326 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/glossary.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2023 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/index.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6360 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/intro.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      918 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/links.inc
+-rw-rw-r--   0 mih       (1000) mih       (1000)      516 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/modref.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5895 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/settingup.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11236 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/docs/source/tutorial.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)       60 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/pyproject.toml
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1151 2023-04-20 09:34:50.185963 datalad_dataverse-1.0.1/setup.cfg
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      369 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/setup.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    81295 2023-04-20 09:34:44.000000 datalad_dataverse-1.0.1/versioneer.py
```

### Comparing `datalad_dataverse-1.0.0/LICENSE` & `datalad_dataverse-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/PKG-INFO` & `datalad_dataverse-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad_dataverse
-Version: 1.0.0
+Version: 1.0.1
 Summary: demo DataLad extension package
 Home-page: https://github.com/datalad/datalad-dataverse
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,17 @@
 License-File: LICENSE
 
 # DataLad extension for working Dataverse
 
 [![Build status](https://ci.appveyor.com/api/projects/status/fm24tes0vxlq7qis/branch/main?svg=true)](https://ci.appveyor.com/project/mih/datalad-dataverse/branch/main)
 [![codecov](https://codecov.io/gh/datalad/datalad-dataverse/branch/main/graph/badge.svg?token=cPUPplOH3o)](https://codecov.io/gh/datalad/datalad-dataverse)
 [![Documentation Status](https://readthedocs.org/projects/datalad-dataverse/badge/?version=latest)](http://docs.datalad.org/projects/datalad-dataverse/en/latest/?badge=latest)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![GitHub release](https://img.shields.io/github/release/datalad/datalad-dataverse.svg)](https://GitHub.com/datalad/datalad-dataverse/releases/)
+[![PyPI version fury.io](https://badge.fury.io/py/datalad-dataverse.svg)](https://pypi.python.org/pypi/datalad-dataverse/)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-15-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 [Dataverse](https://dataverse.org) is open source research data repository software that is deployed all over the world as data or metadata repositories.
 It supports sharing, preserving, citing, exploring, and analyzing research data with descriptive metadata, and thus contributes greatly to open, reproducible, and FAIR science.
 [DataLad](https://www.datalad.org), on the other hand, is a data management and data publication tool build on Git and git-annex.
```

#### html2text {}

```diff
@@ -1,22 +1,27 @@
-Metadata-Version: 2.1 Name: datalad_dataverse Version: 1.0.0 Summary: demo
+Metadata-Version: 2.1 Name: datalad_dataverse Version: 1.0.1 Summary: demo
 DataLad extension package Home-page: https://github.com/datalad/datalad-
 dataverse Author: The DataLad Team and Contributors Author-email:
 team@datalad.org License: MIT Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
 markdown; charset=UTF-8 Provides-Extra: devel License-File: LICENSE # DataLad
 extension for working Dataverse [![Build status](https://ci.appveyor.com/api/
 projects/status/fm24tes0vxlq7qis/branch/main?svg=true)](https://
 ci.appveyor.com/project/mih/datalad-dataverse/branch/main) [![codecov](https://
 codecov.io/gh/datalad/datalad-dataverse/branch/main/graph/
 badge.svg?token=cPUPplOH3o)](https://codecov.io/gh/datalad/datalad-dataverse)
 [![Documentation Status](https://readthedocs.org/projects/datalad-dataverse/
 badge/?version=latest)](http://docs.datalad.org/projects/datalad-dataverse/en/
-latest/?badge=latest)  [![All Contributors](https://img.shields.io/badge/
+latest/?badge=latest) [![License: MIT](https://img.shields.io/badge/License-
+MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![GitHub release](https:
+//img.shields.io/github/release/datalad/datalad-dataverse.svg)](https://
+GitHub.com/datalad/datalad-dataverse/releases/) [![PyPI version fury.io](https:
+//badge.fury.io/py/datalad-dataverse.svg)](https://pypi.python.org/pypi/
+datalad-dataverse/)  [![All Contributors](https://img.shields.io/badge/
 all_contributors-15-orange.svg?style=flat-square)](#contributors-)  [Dataverse]
 (https://dataverse.org) is open source research data repository software that
 is deployed all over the world as data or metadata repositories. It supports
 sharing, preserving, citing, exploring, and analyzing research data with
 descriptive metadata, and thus contributes greatly to open, reproducible, and
 FAIR science. [DataLad](https://www.datalad.org), on the other hand, is a data
 management and data publication tool build on Git and git-annex. Its core data
```

### Comparing `datalad_dataverse-1.0.0/README.md` & `datalad_dataverse-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # DataLad extension for working Dataverse
 
 [![Build status](https://ci.appveyor.com/api/projects/status/fm24tes0vxlq7qis/branch/main?svg=true)](https://ci.appveyor.com/project/mih/datalad-dataverse/branch/main)
 [![codecov](https://codecov.io/gh/datalad/datalad-dataverse/branch/main/graph/badge.svg?token=cPUPplOH3o)](https://codecov.io/gh/datalad/datalad-dataverse)
 [![Documentation Status](https://readthedocs.org/projects/datalad-dataverse/badge/?version=latest)](http://docs.datalad.org/projects/datalad-dataverse/en/latest/?badge=latest)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![GitHub release](https://img.shields.io/github/release/datalad/datalad-dataverse.svg)](https://GitHub.com/datalad/datalad-dataverse/releases/)
+[![PyPI version fury.io](https://badge.fury.io/py/datalad-dataverse.svg)](https://pypi.python.org/pypi/datalad-dataverse/)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-15-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 [Dataverse](https://dataverse.org) is open source research data repository software that is deployed all over the world as data or metadata repositories.
 It supports sharing, preserving, citing, exploring, and analyzing research data with descriptive metadata, and thus contributes greatly to open, reproducible, and FAIR science.
 [DataLad](https://www.datalad.org), on the other hand, is a data management and data publication tool build on Git and git-annex.
```

#### html2text {}

```diff
@@ -1,15 +1,20 @@
 # DataLad extension for working Dataverse [![Build status](https://
 ci.appveyor.com/api/projects/status/fm24tes0vxlq7qis/branch/main?svg=true)]
 (https://ci.appveyor.com/project/mih/datalad-dataverse/branch/main) [![codecov]
 (https://codecov.io/gh/datalad/datalad-dataverse/branch/main/graph/
 badge.svg?token=cPUPplOH3o)](https://codecov.io/gh/datalad/datalad-dataverse)
 [![Documentation Status](https://readthedocs.org/projects/datalad-dataverse/
 badge/?version=latest)](http://docs.datalad.org/projects/datalad-dataverse/en/
-latest/?badge=latest)  [![All Contributors](https://img.shields.io/badge/
+latest/?badge=latest) [![License: MIT](https://img.shields.io/badge/License-
+MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![GitHub release](https:
+//img.shields.io/github/release/datalad/datalad-dataverse.svg)](https://
+GitHub.com/datalad/datalad-dataverse/releases/) [![PyPI version fury.io](https:
+//badge.fury.io/py/datalad-dataverse.svg)](https://pypi.python.org/pypi/
+datalad-dataverse/)  [![All Contributors](https://img.shields.io/badge/
 all_contributors-15-orange.svg?style=flat-square)](#contributors-)  [Dataverse]
 (https://dataverse.org) is open source research data repository software that
 is deployed all over the world as data or metadata repositories. It supports
 sharing, preserving, citing, exploring, and analyzing research data with
 descriptive metadata, and thus contributes greatly to open, reproducible, and
 FAIR science. [DataLad](https://www.datalad.org), on the other hand, is a data
 management and data publication tool build on Git and git-annex. Its core data
```

### Comparing `datalad_dataverse-1.0.0/_datalad_buildsupport/__init__.py` & `datalad_dataverse-1.0.1/_datalad_buildsupport/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/_datalad_buildsupport/formatters.py` & `datalad_dataverse-1.0.1/_datalad_buildsupport/formatters.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/_datalad_buildsupport/setup.py` & `datalad_dataverse-1.0.1/_datalad_buildsupport/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/__init__.py` & `datalad_dataverse-1.0.1/datalad_dataverse/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/add_sibling_dataverse.py` & `datalad_dataverse-1.0.1/datalad_dataverse/add_sibling_dataverse.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,16 @@
     _params_ = dict(
         dv_url=Parameter(
             args=("dv_url",),
             metavar='URL',
             doc="""URL identifying the dataverse instance to connect to
             (e.g., https://demo.dataverse.org)""",),
         ds_pid=Parameter(
-            args=("PID",),
+            args=("ds_pid",),
+            metavar=("PID",),
             doc="""Persistent identifier of the dataverse dataset to
             use as a sibling. This PID can be found on the dataset's
             landing page on Dataverse. Either right at the top
             underneath the title of the dataset as an URL or in the dataset's
             metadata. Both formats (doi:10.5072/FK2/PMPMZM and
             https://doi.org/10.5072/FK2/PMPMZM) are supported for this
             parameter.""",
```

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/baseremote.py` & `datalad_dataverse-1.0.1/datalad_dataverse/baseremote.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/conftest.py` & `datalad_dataverse-1.0.1/datalad_dataverse/conftest.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/dataset.py` & `datalad_dataverse-1.0.1/datalad_dataverse/dataset.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/remote.py` & `datalad_dataverse-1.0.1/datalad_dataverse/remote.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/tests/fixtures.py` & `datalad_dataverse-1.0.1/datalad_dataverse/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/tests/test_add_sibling_dataverse.py` & `datalad_dataverse-1.0.1/datalad_dataverse/tests/test_add_sibling_dataverse.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/tests/test_dataset.py` & `datalad_dataverse-1.0.1/datalad_dataverse/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/tests/test_pydataverse.py` & `datalad_dataverse-1.0.1/datalad_dataverse/tests/test_pydataverse.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/tests/test_remote.py` & `datalad_dataverse-1.0.1/datalad_dataverse/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/tests/test_remote_xdlra.py` & `datalad_dataverse-1.0.1/datalad_dataverse/tests/test_remote_xdlra.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/tests/test_utils.py` & `datalad_dataverse-1.0.1/datalad_dataverse/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/tests/utils.py` & `datalad_dataverse-1.0.1/datalad_dataverse/tests/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import json
+
 from pyDataverse.models import (
     Dataverse,
     Dataset as DvDataset,
 )
 from pyDataverse.exceptions import OperationFailedError
 
 from datalad_next.exceptions import CapturedException
@@ -57,21 +59,25 @@
     api: NativeApi
     collection: Dataverse
     dataset_meta: dict
 
     Returns
     -------
     DvDataset
-     """
-    dv_dataset = DvDataset()
-    dv_dataset.set(dataset_meta)
-    if not dv_dataset.validate_json():
-        raise InvalidDatasetMetadata
-    dv_dataset = api.create_dataset(collection['data']['alias'],
-                                    dv_dataset.json())
+    """
+    # we can no longer use pydataverse models, changes in dataverse v5.13
+    # break their assumptions
+    #dv_dataset = DvDataset()
+    #dv_dataset.set(dataset_meta)
+    #if not dv_dataset.validate_json():
+    #    raise InvalidDatasetMetadata
+    dv_dataset = api.create_dataset(
+        collection['data']['alias'],
+        json.dumps(dataset_meta)
+    )
     dv_dataset.raise_for_status()
     return dv_dataset
 
 
 def create_test_dataverse_collection(api, alias, collection):
     dvmeta = Dataverse(dict(
         name="DataLad Test Dataverse",
@@ -94,23 +100,34 @@
 def create_test_dataverse_dataset(api, collection, name):
     """
     Returns
     -------
     str
       The persistent DOI for the dataset
     """
-    meta = dict(
-        title=name,
-        author=[dict(authorName='DataLad')],
-        datasetContact=[dict(
-            datasetContactEmail='team@datalad.org',
-            datasetContactName='DataLad')],
-        dsDescription=[dict(dsDescriptionValue='no description')],
-        subject=['Medicine, Health and Life Sciences']
-    )
+    meta = {
+        "http://purl.org/dc/terms/title": name,
+        "http://purl.org/dc/terms/subject":
+        "Medicine, Health and Life Sciences",
+        "http://purl.org/dc/terms/creator": {
+            "https://dataverse.org/schema/citation/authorName": "DataLad",
+            "https://dataverse.org/schema/citation/authorAffiliation":
+            "datalad.org"
+        },
+        "https://dataverse.org/schema/citation/datasetContact": {
+            "https://dataverse.org/schema/citation/datasetContactEmail":
+            "team@datalad.org",
+            "https://dataverse.org/schema/citation/datasetContactName":
+            "DataLad"
+        },
+        "https://dataverse.org/schema/citation/dsDescription": {
+            "https://dataverse.org/schema/citation/dsDescriptionValue":
+            "no description"
+        }
+    }
     col = _get_dv_collection(api, collection)
     req = _create_dv_dataset(api, col, meta)
     req.raise_for_status()
     return req.json()['data']['persistentId']
 
 
 def list_dataset_files(api, doi: str) -> list:
```

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse/utils.py` & `datalad_dataverse-1.0.1/datalad_dataverse/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse.egg-info/PKG-INFO` & `datalad_dataverse-1.0.1/datalad_dataverse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-dataverse
-Version: 1.0.0
+Version: 1.0.1
 Summary: demo DataLad extension package
 Home-page: https://github.com/datalad/datalad-dataverse
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,17 @@
 License-File: LICENSE
 
 # DataLad extension for working Dataverse
 
 [![Build status](https://ci.appveyor.com/api/projects/status/fm24tes0vxlq7qis/branch/main?svg=true)](https://ci.appveyor.com/project/mih/datalad-dataverse/branch/main)
 [![codecov](https://codecov.io/gh/datalad/datalad-dataverse/branch/main/graph/badge.svg?token=cPUPplOH3o)](https://codecov.io/gh/datalad/datalad-dataverse)
 [![Documentation Status](https://readthedocs.org/projects/datalad-dataverse/badge/?version=latest)](http://docs.datalad.org/projects/datalad-dataverse/en/latest/?badge=latest)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![GitHub release](https://img.shields.io/github/release/datalad/datalad-dataverse.svg)](https://GitHub.com/datalad/datalad-dataverse/releases/)
+[![PyPI version fury.io](https://badge.fury.io/py/datalad-dataverse.svg)](https://pypi.python.org/pypi/datalad-dataverse/)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-15-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 [Dataverse](https://dataverse.org) is open source research data repository software that is deployed all over the world as data or metadata repositories.
 It supports sharing, preserving, citing, exploring, and analyzing research data with descriptive metadata, and thus contributes greatly to open, reproducible, and FAIR science.
 [DataLad](https://www.datalad.org), on the other hand, is a data management and data publication tool build on Git and git-annex.
```

#### html2text {}

```diff
@@ -1,22 +1,27 @@
-Metadata-Version: 2.1 Name: datalad-dataverse Version: 1.0.0 Summary: demo
+Metadata-Version: 2.1 Name: datalad-dataverse Version: 1.0.1 Summary: demo
 DataLad extension package Home-page: https://github.com/datalad/datalad-
 dataverse Author: The DataLad Team and Contributors Author-email:
 team@datalad.org License: MIT Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
 markdown; charset=UTF-8 Provides-Extra: devel License-File: LICENSE # DataLad
 extension for working Dataverse [![Build status](https://ci.appveyor.com/api/
 projects/status/fm24tes0vxlq7qis/branch/main?svg=true)](https://
 ci.appveyor.com/project/mih/datalad-dataverse/branch/main) [![codecov](https://
 codecov.io/gh/datalad/datalad-dataverse/branch/main/graph/
 badge.svg?token=cPUPplOH3o)](https://codecov.io/gh/datalad/datalad-dataverse)
 [![Documentation Status](https://readthedocs.org/projects/datalad-dataverse/
 badge/?version=latest)](http://docs.datalad.org/projects/datalad-dataverse/en/
-latest/?badge=latest)  [![All Contributors](https://img.shields.io/badge/
+latest/?badge=latest) [![License: MIT](https://img.shields.io/badge/License-
+MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![GitHub release](https:
+//img.shields.io/github/release/datalad/datalad-dataverse.svg)](https://
+GitHub.com/datalad/datalad-dataverse/releases/) [![PyPI version fury.io](https:
+//badge.fury.io/py/datalad-dataverse.svg)](https://pypi.python.org/pypi/
+datalad-dataverse/)  [![All Contributors](https://img.shields.io/badge/
 all_contributors-15-orange.svg?style=flat-square)](#contributors-)  [Dataverse]
 (https://dataverse.org) is open source research data repository software that
 is deployed all over the world as data or metadata repositories. It supports
 sharing, preserving, citing, exploring, and analyzing research data with
 descriptive metadata, and thus contributes greatly to open, reproducible, and
 FAIR science. [DataLad](https://www.datalad.org), on the other hand, is a data
 management and data publication tool build on Git and git-annex. Its core data
```

### Comparing `datalad_dataverse-1.0.0/datalad_dataverse.egg-info/SOURCES.txt` & `datalad_dataverse-1.0.1/datalad_dataverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/Makefile` & `datalad_dataverse-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/README.md` & `datalad_dataverse-1.0.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/_static/clueless.gif` & `datalad_dataverse-1.0.1/docs/source/_static/clueless.gif`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/_static/datalad_logo.png` & `datalad_dataverse-1.0.1/docs/source/_static/datalad_logo.png`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/_static/logo.png` & `datalad_dataverse-1.0.1/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/_static/logo.svg` & `datalad_dataverse-1.0.1/docs/source/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_add_dataset.png` & `datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_add_dataset.png`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_add_dataset_2.png` & `datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_add_dataset_2.png`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_dataset_annex.png` & `datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_dataset_annex.png`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_dataset_filetree.png` & `datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_dataset_filetree.png`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_obtain_doi.png` & `datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_obtain_doi.png`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_publish_ds.png` & `datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_publish_ds.png`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/_static/tutorial/dv_token.png` & `datalad_dataverse-1.0.1/docs/source/_static/tutorial/dv_token.png`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/conf.py` & `datalad_dataverse-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/glossary.rst` & `datalad_dataverse-1.0.1/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/index.rst` & `datalad_dataverse-1.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/intro.rst` & `datalad_dataverse-1.0.1/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/links.inc` & `datalad_dataverse-1.0.1/docs/source/links.inc`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/modref.rst` & `datalad_dataverse-1.0.1/docs/source/modref.rst`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/settingup.rst` & `datalad_dataverse-1.0.1/docs/source/settingup.rst`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/docs/source/tutorial.rst` & `datalad_dataverse-1.0.1/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/setup.cfg` & `datalad_dataverse-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `datalad_dataverse-1.0.0/versioneer.py` & `datalad_dataverse-1.0.1/versioneer.py`

 * *Files identical despite different names*

