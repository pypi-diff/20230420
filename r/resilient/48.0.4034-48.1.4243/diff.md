# Comparing `tmp/resilient-48.0.4034.tar.gz` & `tmp/resilient-48.1.4243.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient-48.0.4034.tar", last modified: Tue Feb 28 15:23:05 2023, max compression
+gzip compressed data, was "resilient-48.1.4243.tar", last modified: Thu Apr 20 19:34:54 2023, max compression
```

## Comparing `resilient-48.0.4034.tar` & `resilient-48.1.4243.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:05.486444 resilient-48.0.4034/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7805 2023-02-28 15:22:43.000000 resilient-48.0.4034/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-02-28 15:23:05.486444 resilient-48.0.4034/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2023-02-28 15:22:43.000000 resilient-48.0.4034/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:05.478444 resilient-48.0.4034/co3/
--rw-rw-r--   0 travis    (2000) travis    (2000)      377 2023-02-28 15:22:43.000000 resilient-48.0.4034/co3/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-02-28 15:22:43.000000 resilient-48.0.4034/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:05.482444 resilient-48.0.4034/resilient/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1003 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:05.482444 resilient-48.0.4034/resilient/bin/
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/bin/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/bin/finfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/bin/gadget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/bin/res_keyring.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36857 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/co3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14360 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/co3argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35271 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/co3base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/co3sslutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1577 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      854 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/definitions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12719 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2514 2023-02-28 15:22:43.000000 resilient-48.0.4034/resilient/resilient_rest_mock.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:05.482444 resilient-48.0.4034/resilient.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-02-28 15:23:05.000000 resilient-48.0.4034/resilient.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1425 2023-02-28 15:23:05.000000 resilient-48.0.4034/resilient.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:23:05.000000 resilient-48.0.4034/resilient.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2023-02-28 15:23:05.000000 resilient-48.0.4034/resilient.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      350 2023-02-28 15:23:05.000000 resilient-48.0.4034/resilient.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-02-28 15:23:05.000000 resilient-48.0.4034/resilient.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1854 2023-02-28 15:23:05.486444 resilient-48.0.4034/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-02-28 15:22:43.000000 resilient-48.0.4034/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:05.486444 resilient-48.0.4034/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4241 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:05.486444 resilient-48.0.4034/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/shared_mock_data/mock_paths.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:05.486444 resilient-48.0.4034/tests/shared_mock_data/mock_responses/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/shared_mock_data/mock_responses/session.JSON
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:05.486444 resilient-48.0.4034/tests/shared_mock_data/mock_secrets/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:05.486444 resilient-48.0.4034/tests/shared_mock_data/mock_secrets/.jwk/
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/shared_mock_data/mock_secrets/.jwk/key.jwk
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/shared_mock_data/mock_secrets/.jwk/key_unused.jwk
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/shared_mock_data/mock_secrets/API_KEY
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/shared_mock_data/mock_secrets/EMAIL
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/shared_mock_data/mock_secrets/EMPTY
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/shared_mock_data/mock_secrets/PASSWORD
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/shared_mock_data/mock_secrets/URL
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/template_test.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2951 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/test_co3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20175 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/test_co3_ii.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/test_co3base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      318 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/test_co3sslutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/test_finfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9003 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/xtest_gadget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6988 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/xtest_patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      726 2023-02-28 15:22:43.000000 resilient-48.0.4034/tests/xtest_res_keyring.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-28 15:23:05.486444 resilient-48.0.4034/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10657 2023-02-28 15:22:43.000000 resilient-48.0.4034/tools/res_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      885 2023-02-28 15:22:43.000000 resilient-48.0.4034/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8037 2023-04-20 19:34:29.000000 resilient-48.1.4243/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-04-20 19:34:54.035501 resilient-48.1.4243/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2023-04-20 19:34:29.000000 resilient-48.1.4243/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.031501 resilient-48.1.4243/co3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      377 2023-04-20 19:34:29.000000 resilient-48.1.4243/co3/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-04-20 19:34:29.000000 resilient-48.1.4243/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.031501 resilient-48.1.4243/resilient/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1003 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/resilient/bin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/bin/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/bin/finfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/bin/gadget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/bin/res_keyring.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36857 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/co3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14360 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/co3argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36941 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/co3base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/co3sslutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1577 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      854 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/definitions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12719 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2514 2023-04-20 19:34:29.000000 resilient-48.1.4243/resilient/resilient_rest_mock.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/resilient.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3023 2023-04-20 19:34:53.000000 resilient-48.1.4243/resilient.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1425 2023-04-20 19:34:54.000000 resilient-48.1.4243/resilient.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:53.000000 resilient-48.1.4243/resilient.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      131 2023-04-20 19:34:53.000000 resilient-48.1.4243/resilient.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      350 2023-04-20 19:34:53.000000 resilient-48.1.4243/resilient.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-04-20 19:34:53.000000 resilient-48.1.4243/resilient.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1854 2023-04-20 19:34:54.035501 resilient-48.1.4243/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-04-20 19:34:29.000000 resilient-48.1.4243/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4241 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_paths.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/tests/shared_mock_data/mock_responses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_responses/session.JSON
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/.jwk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/.jwk/key.jwk
+-rw-rw-r--   0 travis    (2000) travis    (2000)       87 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/.jwk/key_unused.jwk
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/API_KEY
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/EMAIL
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/EMPTY
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/PASSWORD
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/shared_mock_data/mock_secrets/URL
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/template_test.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2951 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/test_co3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20175 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/test_co3_ii.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/test_co3base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      318 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/test_co3sslutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/test_finfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9003 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/test_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/xtest_gadget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6988 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/xtest_patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      726 2023-04-20 19:34:29.000000 resilient-48.1.4243/tests/xtest_res_keyring.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-20 19:34:54.035501 resilient-48.1.4243/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10657 2023-04-20 19:34:29.000000 resilient-48.1.4243/tools/res_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      885 2023-04-20 19:34:29.000000 resilient-48.1.4243/tox.ini
```

### Comparing `resilient-48.0.4034/CHANGES` & `resilient-48.1.4243/CHANGES`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+**2023-04: version 48.1**
+
+* REST client updated to use ``include_permissions=false`` by default when authenticating to ``/rest/session`` endpoint.
+  This will give improved performance for SOAR instances with large organizations.
+
 **2023-02: version 48.0**
 
 * Updated project to use ``pyproject.toml`` and ``setup.cfg`` metadata files. Build backend continues to use ``setuptools``.
   Instead of directly invoking setup.py to get a sdist or wheel, use ``build`` as a build frontend:
 
   .. code-block:: bash
```

### Comparing `resilient-48.0.4034/PKG-INFO` & `resilient-48.1.4243/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient
-Version: 48.0.4034
+Version: 48.1.4243
 Summary: Python client module for the IBM SOAR REST API
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient-48.0.4034/README.md` & `resilient-48.1.4243/README.md`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/LICENSE` & `resilient-48.1.4243/resilient/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/__init__.py` & `resilient-48.1.4243/resilient/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/bin/finfo.py` & `resilient-48.1.4243/resilient/bin/finfo.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/bin/gadget.py` & `resilient-48.1.4243/resilient/bin/gadget.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/bin/res_keyring.py` & `resilient-48.1.4243/resilient/bin/res_keyring.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/co3.py` & `resilient-48.1.4243/resilient/co3.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/co3argparse.py` & `resilient-48.1.4243/resilient/co3argparse.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/co3base.py` & `resilient-48.1.4243/resilient/co3base.py`

 * *Files 4% similar despite different names*

```diff
@@ -189,31 +189,47 @@
 
         # Retry configs
         self.max_connection_retries = kwargs.get(constants.APP_CONFIG_MAX_CONNECTION_RETRIES) if kwargs.get(constants.APP_CONFIG_MAX_CONNECTION_RETRIES) is not None else constants.APP_CONFIG_MAX_CONNECTION_RETRIES_DEFAULT
         self.request_max_retries = kwargs.get(constants.APP_CONFIG_REQUEST_MAX_RETRIES) if kwargs.get(constants.APP_CONFIG_REQUEST_MAX_RETRIES) is not None else constants.APP_CONFIG_REQUEST_MAX_RETRIES_DEFAULT
         self.request_retry_delay = kwargs.get(constants.APP_CONFIG_REQUEST_RETRY_DELAY) if kwargs.get(constants.APP_CONFIG_REQUEST_RETRY_DELAY) is not None else constants.APP_CONFIG_REQUEST_RETRY_DELAY_DEFAULT
         self.request_retry_backoff = kwargs.get(constants.APP_CONFIG_REQUEST_RETRY_BACKOFF) if kwargs.get(constants.APP_CONFIG_REQUEST_RETRY_BACKOFF) is not None else constants.APP_CONFIG_REQUEST_RETRY_BACKOFF_DEFAULT
 
-    def set_api_key(self, api_key_id, api_key_secret, timeout=None):
+    def set_api_key(self, api_key_id, api_key_secret, timeout=None, include_permissions=False):
         """
         Call this method instead of the connect method in order to use API key
         Just like the connect method, this method calls the session endpoint
         to get org_id information.
-        :param api_key_id:
-        :param api_key_secret:
+        :param api_key_id: api key ID to use to connect
+        :type api_key_id: string
+        :param api_key_secret: associated secret
+        :type api_key_secret: string
+        :param timeout: timeout limit if desired. None by default
+        :type timeout: float
+        :param include_permissions: whether to include permissions in call to /rest/session.
+            Since SOAR v48 this param has been included and set to "true" by default on the server
+            (until v50 where it will be removed). We don't need permission details in circuits so we
+            set it to False by default, but if there is a use of this elsewhere in app code,
+            and either "perms" or "effective_permissions" details that are returned by the
+            endpoint are needed, the value here should be set to True.
+        :type include_permissions: bool
         :return:
         """
         self.api_key_id = api_key_id
         self.api_key_secret = api_key_secret
         self.use_api_key = True
 
+        if include_permissions:
+            LOG.debug("'include_permissions' is deprecated and scheduled to be removed in v50, use GET " +
+                        "/rest/session/{org_id}/acl instead.\n\t\tAt that time, 'include_permissions' will be " +
+                        "removed and this endpoint will not return org permissions.")
+
         # Wrap self.session.get and its related raise_if_error call in
         # inner function so we can add retry logic with dynamic parameters to it
         def __set_api_key():
-            r = self.session.get(u"{0}/rest/session".format(self.base_url),
+            r = self.session.get(u"{0}/rest/session?include_permissions={1}".format(self.base_url, "true" if include_permissions else "false"),
                                  auth=HTTPBasicAuth(self.api_key_id, self.api_key_secret),
                                  proxies=self.proxies,
                                  headers=self.make_headers(),
                                  verify=self.verify,
                                  timeout=timeout,
                                  cert=self.cert)
             BasicHTTPException.raise_if_error(r)
@@ -308,21 +324,26 @@
                   "The organization requires authentication with a different provider than you are currently using.\n" \
                   "Your IP address is {0}"
             raise Exception(msg.format(response.get("session_ip", "Unknown")))
 
         self.all_orgs = [org for org in orgs if org.get("enabled")]
         self.org_id = selected_org.get("id", None)
 
-    def _connect(self, timeout=None):
+    def _connect(self, timeout=None, include_permissions=False):
         """Connect to SOAR using deprecated username and password method"""
 
+        if include_permissions:
+            LOG.debug("'include_permissions' is deprecated and scheduled to be removed in v50, use GET " +
+                        "/rest/session/{org_id}/acl instead.\n\t\tAt that time, 'include_permissions' will be " +
+                        "removed and this endpoint will not return org permissions.")
+
         # Wrap self.session.post and its related raise_if_error call in
         # inner function so we can add retry logic with dynamic parameters to it
         def __connect():
-            r = self.session.post(u"{0}/rest/session".format(self.base_url),
+            r = self.session.post(u"{0}/rest/session?include_permissions={1}".format(self.base_url, "true" if include_permissions else "false"),
                                   data=json.dumps(self.authdata),
                                   proxies=self.proxies,
                                   headers=self.make_headers(),
                                   verify=self.verify,
                                   timeout=timeout,
                                   cert=self.cert)
```

### Comparing `resilient-48.0.4034/resilient/co3sslutil.py` & `resilient-48.1.4243/resilient/co3sslutil.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/constants.py` & `resilient-48.1.4243/resilient/constants.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/definitions.py` & `resilient-48.1.4243/resilient/definitions.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/helpers.py` & `resilient-48.1.4243/resilient/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/patch.py` & `resilient-48.1.4243/resilient/patch.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient/resilient_rest_mock.py` & `resilient-48.1.4243/resilient/resilient_rest_mock.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/resilient.egg-info/PKG-INFO` & `resilient-48.1.4243/resilient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient
-Version: 48.0.4034
+Version: 48.1.4243
 Summary: Python client module for the IBM SOAR REST API
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient-48.0.4034/resilient.egg-info/SOURCES.txt` & `resilient-48.1.4243/resilient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/setup.cfg` & `resilient-48.1.4243/setup.cfg`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tests/conftest.py` & `resilient-48.1.4243/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tests/helpers.py` & `resilient-48.1.4243/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tests/shared_mock_data/mock_responses/session.JSON` & `resilient-48.1.4243/tests/shared_mock_data/mock_responses/session.JSON`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tests/test_co3.py` & `resilient-48.1.4243/tests/test_co3.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tests/test_co3_ii.py` & `resilient-48.1.4243/tests/test_co3_ii.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tests/test_co3base.py` & `resilient-48.1.4243/tests/test_co3base.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tests/test_finfo.py` & `resilient-48.1.4243/tests/test_finfo.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tests/test_helpers.py` & `resilient-48.1.4243/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tests/xtest_gadget.py` & `resilient-48.1.4243/tests/xtest_gadget.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tests/xtest_patch.py` & `resilient-48.1.4243/tests/xtest_patch.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tests/xtest_res_keyring.py` & `resilient-48.1.4243/tests/xtest_res_keyring.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tools/res_utils.py` & `resilient-48.1.4243/tools/res_utils.py`

 * *Files identical despite different names*

### Comparing `resilient-48.0.4034/tox.ini` & `resilient-48.1.4243/tox.ini`

 * *Files identical despite different names*

