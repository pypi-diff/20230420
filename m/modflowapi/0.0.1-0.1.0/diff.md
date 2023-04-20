# Comparing `tmp/modflowapi-0.0.1.tar.gz` & `tmp/modflowapi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modflowapi-0.0.1.tar", last modified: Tue May 11 21:49:28 2021, max compression
+gzip compressed data, was "modflowapi-0.1.0.tar", last modified: Thu Apr 20 13:38:44 2023, max compression
```

## Comparing `modflowapi-0.0.1.tar` & `modflowapi-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,38 @@
-drwxr-xr-x   0 jdhughes (56154) 238731076        0 2021-05-11 21:49:28.721346 modflowapi-0.0.1/
--rw-r--r--   0 jdhughes (56154) 238731076     1050 2021-05-11 21:49:28.720996 modflowapi-0.0.1/PKG-INFO
--rw-r--r--   0 jdhughes (56154) 238731076      414 2021-05-11 20:30:19.000000 modflowapi-0.0.1/README.md
-drwxr-xr-x   0 jdhughes (56154) 238731076        0 2021-05-11 21:49:28.717024 modflowapi-0.0.1/modflowapi/
--rw-r--r--   0 jdhughes (56154) 238731076       78 2021-05-11 20:03:52.000000 modflowapi-0.0.1/modflowapi/__init__.py
--rw-r--r--   0 jdhughes (56154) 238731076      783 2021-05-11 20:44:25.000000 modflowapi-0.0.1/modflowapi/modflowapi.py
-drwxr-xr-x   0 jdhughes (56154) 238731076        0 2021-05-11 21:49:28.720108 modflowapi-0.0.1/modflowapi.egg-info/
--rw-r--r--   0 jdhughes (56154) 238731076     1050 2021-05-11 21:49:28.000000 modflowapi-0.0.1/modflowapi.egg-info/PKG-INFO
--rw-r--r--   0 jdhughes (56154) 238731076      235 2021-05-11 21:49:28.000000 modflowapi-0.0.1/modflowapi.egg-info/SOURCES.txt
--rw-r--r--   0 jdhughes (56154) 238731076        1 2021-05-11 21:49:28.000000 modflowapi-0.0.1/modflowapi.egg-info/dependency_links.txt
--rw-r--r--   0 jdhughes (56154) 238731076        6 2021-05-11 21:49:28.000000 modflowapi-0.0.1/modflowapi.egg-info/requires.txt
--rw-r--r--   0 jdhughes (56154) 238731076       11 2021-05-11 21:49:28.000000 modflowapi-0.0.1/modflowapi.egg-info/top_level.txt
--rw-r--r--   0 jdhughes (56154) 238731076       38 2021-05-11 21:49:28.721454 modflowapi-0.0.1/setup.cfg
--rwxr-xr-x   0 jdhughes (56154) 238731076     1613 2021-05-11 20:49:10.000000 modflowapi-0.0.1/setup.py
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-20 13:38:44.600896 modflowapi-0.1.0/
+-rw-r--r--   0 jdhughes (179580369) 286921933      656 2023-04-19 21:42:36.000000 modflowapi-0.1.0/.flake8
+-rw-r--r--   0 jdhughes (179580369) 286921933      586 2023-04-19 21:42:36.000000 modflowapi-0.1.0/.gitattributes
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-20 13:38:44.507053 modflowapi-0.1.0/.github/
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-20 13:38:44.550936 modflowapi-0.1.0/.github/workflows/
+-rw-r--r--   0 jdhughes (179580369) 286921933     4601 2023-04-19 21:55:54.000000 modflowapi-0.1.0/.github/workflows/ci.yml
+-rw-------   0 jdhughes (179580369) 286921933     1817 2021-05-11 20:52:52.000000 modflowapi-0.1.0/.gitignore
+-rw-------   0 jdhughes (179580369) 286921933    17911 2021-02-19 22:13:10.000000 modflowapi-0.1.0/.pylintrc
+-rw-------   0 jdhughes (179580369) 286921933     7048 2021-05-11 16:23:27.000000 modflowapi-0.1.0/LICENSE
+-rw-r--r--   0 jdhughes (179580369) 286921933     2438 2023-04-20 13:38:44.600601 modflowapi-0.1.0/PKG-INFO
+-rw-r--r--   0 jdhughes (179580369) 286921933     1195 2023-04-19 21:55:43.000000 modflowapi-0.1.0/README.md
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-20 13:38:44.565045 modflowapi-0.1.0/autotest/
+-rw-r--r--   0 jdhughes (179580369) 286921933       22 2023-04-19 21:42:36.000000 modflowapi-0.1.0/autotest/__init__.py
+-rw-r--r--   0 jdhughes (179580369) 286921933     4867 2023-04-19 21:42:36.000000 modflowapi-0.1.0/autotest/conftest.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    12088 2023-04-19 21:42:36.000000 modflowapi-0.1.0/autotest/test_interface.py
+-rw-r--r--   0 jdhughes (179580369) 286921933     1681 2023-04-19 21:42:36.000000 modflowapi-0.1.0/autotest/test_mf6_examples.py
+-rw-r--r--   0 jdhughes (179580369) 286921933      297 2023-04-19 21:42:36.000000 modflowapi-0.1.0/guide-to-publish.md
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-20 13:38:44.572102 modflowapi-0.1.0/modflowapi/
+-rw-r--r--   0 jdhughes (179580369) 286921933      171 2023-04-19 21:42:36.000000 modflowapi-0.1.0/modflowapi/__init__.py
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-20 13:38:44.599845 modflowapi-0.1.0/modflowapi/extensions/
+-rw-r--r--   0 jdhughes (179580369) 286921933      109 2023-04-19 21:42:36.000000 modflowapi-0.1.0/modflowapi/extensions/__init__.py
+-rw-r--r--   0 jdhughes (179580369) 286921933      538 2023-04-19 21:42:36.000000 modflowapi-0.1.0/modflowapi/extensions/apiexchange.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    11204 2023-04-19 21:51:01.000000 modflowapi-0.1.0/modflowapi/extensions/apimodel.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    10271 2023-04-19 21:42:36.000000 modflowapi-0.1.0/modflowapi/extensions/apisimulation.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    21947 2023-04-19 21:42:36.000000 modflowapi-0.1.0/modflowapi/extensions/data.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    19273 2023-04-19 21:51:01.000000 modflowapi-0.1.0/modflowapi/extensions/pakbase.py
+-rw-r--r--   0 jdhughes (179580369) 286921933     4773 2023-04-19 21:42:36.000000 modflowapi-0.1.0/modflowapi/extensions/runner.py
+-rw-------   0 jdhughes (179580369) 286921933      783 2021-05-12 19:30:05.000000 modflowapi-0.1.0/modflowapi/modflowapi.py
+-rw-r--r--   0 jdhughes (179580369) 286921933      102 2023-04-20 13:37:16.000000 modflowapi-0.1.0/modflowapi/version.py
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-20 13:38:44.576716 modflowapi-0.1.0/modflowapi.egg-info/
+-rw-------   0 jdhughes (179580369) 286921933     2438 2023-04-20 13:38:44.000000 modflowapi-0.1.0/modflowapi.egg-info/PKG-INFO
+-rw-------   0 jdhughes (179580369) 286921933      707 2023-04-20 13:38:44.000000 modflowapi-0.1.0/modflowapi.egg-info/SOURCES.txt
+-rw-------   0 jdhughes (179580369) 286921933        1 2023-04-20 13:38:44.000000 modflowapi-0.1.0/modflowapi.egg-info/dependency_links.txt
+-rw-------   0 jdhughes (179580369) 286921933      143 2023-04-20 13:38:44.000000 modflowapi-0.1.0/modflowapi.egg-info/requires.txt
+-rw-------   0 jdhughes (179580369) 286921933       11 2023-04-20 13:38:44.000000 modflowapi-0.1.0/modflowapi.egg-info/top_level.txt
+-rw-r--r--   0 jdhughes (179580369) 286921933     1974 2023-04-19 21:42:36.000000 modflowapi-0.1.0/pyproject.toml
+-rw-r--r--   0 jdhughes (179580369) 286921933       38 2023-04-20 13:38:44.600982 modflowapi-0.1.0/setup.cfg
+-rw-r--r--   0 jdhughes (179580369) 286921933       97 2023-04-19 21:42:36.000000 modflowapi-0.1.0/setup.py
```

### Comparing `modflowapi-0.0.1/modflowapi/modflowapi.py` & `modflowapi-0.1.0/modflowapi/modflowapi.py`

 * *Files identical despite different names*

