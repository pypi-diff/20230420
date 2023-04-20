# Comparing `tmp/pywrapid-0.2.6.tar.gz` & `tmp/pywrapid-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywrapid-0.2.6.tar", last modified: Tue Apr  4 14:02:48 2023, max compression
+gzip compressed data, was "pywrapid-0.2.7.tar", last modified: Thu Apr 20 11:59:05 2023, max compression
```

## Comparing `pywrapid-0.2.6.tar` & `pywrapid-0.2.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.840892 pywrapid-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-04 14:02:33.000000 pywrapid-0.2.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.828892 pywrapid-0.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.832892 pywrapid-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-04 14:02:33.000000 pywrapid-0.2.6/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-04 14:02:33.000000 pywrapid-0.2.6/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-04 14:02:33.000000 pywrapid-0.2.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-04 14:02:33.000000 pywrapid-0.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-04 14:02:33.000000 pywrapid-0.2.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-04 14:02:33.000000 pywrapid-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-04 14:02:48.840892 pywrapid-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-04 14:02:33.000000 pywrapid-0.2.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.828892 pywrapid-0.2.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.832892 pywrapid-0.2.6/docs/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-04 14:02:33.000000 pywrapid-0.2.6/docs/src/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-04 14:02:33.000000 pywrapid-0.2.6/docs/src/developer-guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.836892 pywrapid-0.2.6/docs/src/features/
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-04 14:02:33.000000 pywrapid-0.2.6/docs/src/features/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-04-04 14:02:33.000000 pywrapid-0.2.6/docs/src/features/log.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-04 14:02:33.000000 pywrapid-0.2.6/docs/src/features/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-04 14:02:33.000000 pywrapid-0.2.6/docs/src/features/webclient.rst
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-04 14:02:33.000000 pywrapid-0.2.6/docs/src/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-04 14:02:33.000000 pywrapid-0.2.6/docs/src/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-04 14:02:33.000000 pywrapid-0.2.6/docs/src/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-04 14:02:33.000000 pywrapid-0.2.6/docs/src/user-guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-04 14:02:33.000000 pywrapid-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 14:02:33.000000 pywrapid-0.2.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 14:02:33.000000 pywrapid-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 14:02:48.840892 pywrapid-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.828892 pywrapid-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.836892 pywrapid-0.2.6/src/pywrapid/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.836892 pywrapid-0.2.6/src/pywrapid/config/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10107 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/config/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/config/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.836892 pywrapid-0.2.6/src/pywrapid/log/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/log/application_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.840892 pywrapid-0.2.6/src/pywrapid/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/utils/dict_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/utils/file_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.840892 pywrapid-0.2.6/src/pywrapid/webclient/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/webclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/webclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/webclient/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-04-04 14:02:33.000000 pywrapid-0.2.6/src/pywrapid/webclient/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.836892 pywrapid-0.2.6/src/pywrapid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-04 14:02:48.000000 pywrapid-0.2.6/src/pywrapid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-04 14:02:48.000000 pywrapid-0.2.6/src/pywrapid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:02:48.000000 pywrapid-0.2.6/src/pywrapid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-04 14:02:48.000000 pywrapid-0.2.6/src/pywrapid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-04 14:02:48.000000 pywrapid-0.2.6/src/pywrapid.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:02:48.840892 pywrapid-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-04 14:02:33.000000 pywrapid-0.2.6/tests/test_conf_ok.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-04 14:02:33.000000 pywrapid-0.2.6/tests/test_pywrapid_config_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-04 14:02:33.000000 pywrapid-0.2.6/tests/test_pywrapid_logging_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-04 14:02:33.000000 pywrapid-0.2.6/tests/test_pywrapid_webclient_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-04 14:02:33.000000 pywrapid-0.2.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-20 11:58:52.000000 pywrapid-0.2.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-20 11:58:52.000000 pywrapid-0.2.7/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-20 11:58:52.000000 pywrapid-0.2.7/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-20 11:58:52.000000 pywrapid-0.2.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-20 11:58:52.000000 pywrapid-0.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-20 11:58:52.000000 pywrapid-0.2.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-20 11:58:52.000000 pywrapid-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-20 11:59:05.251779 pywrapid-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-20 11:58:52.000000 pywrapid-0.2.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/developer-guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/docs/src/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/features/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/features/log.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/features/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/features/webclient.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-20 11:58:52.000000 pywrapid-0.2.7/docs/src/user-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-20 11:58:52.000000 pywrapid-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 11:58:52.000000 pywrapid-0.2.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 11:58:52.000000 pywrapid-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 11:59:05.251779 pywrapid-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.247779 pywrapid-0.2.7/src/pywrapid/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/src/pywrapid/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10107 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/config/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/src/pywrapid/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/log/application_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/src/pywrapid/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/utils/dict_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/utils/file_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/src/pywrapid/webclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/webclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/webclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/webclient/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-04-20 11:58:52.000000 pywrapid-0.2.7/src/pywrapid/webclient/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/src/pywrapid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-20 11:59:05.000000 pywrapid-0.2.7/src/pywrapid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-20 11:59:05.000000 pywrapid-0.2.7/src/pywrapid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:59:05.000000 pywrapid-0.2.7/src/pywrapid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-20 11:59:05.000000 pywrapid-0.2.7/src/pywrapid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 11:59:05.000000 pywrapid-0.2.7/src/pywrapid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:59:05.251779 pywrapid-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-20 11:58:52.000000 pywrapid-0.2.7/tests/test_conf_ok.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-20 11:58:52.000000 pywrapid-0.2.7/tests/test_pywrapid_config_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-20 11:58:52.000000 pywrapid-0.2.7/tests/test_pywrapid_logging_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-20 11:58:52.000000 pywrapid-0.2.7/tests/test_pywrapid_webclient_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-20 11:58:52.000000 pywrapid-0.2.7/tox.ini
```

### Comparing `pywrapid-0.2.6/.github/workflows/codeql.yml` & `pywrapid-0.2.7/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/.github/workflows/dependency-review.yml` & `pywrapid-0.2.7/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/.github/workflows/python-publish.yml` & `pywrapid-0.2.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/.gitignore` & `pywrapid-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/CODE_OF_CONDUCT.md` & `pywrapid-0.2.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/LICENSE` & `pywrapid-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/PKG-INFO` & `pywrapid-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywrapid
-Version: 0.2.6
+Version: 0.2.7
 Summary: Collection of wrapper libraries for rapid development of python applications
 Author-email: Jonas Werme <jonas.werme@nsahq.se>, Marcus Wallgren <marcus.wallgren@nsahq.se>
 Maintainer-email: Jonas Werme <jonas.werme@nsahq.se>, Marcus Wallgren <marcus.wallgren@nsahq.se>
 License: MIT License
         
         Copyright (c) 2022 NSAHQ
```

### Comparing `pywrapid-0.2.6/README.rst` & `pywrapid-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/docs/src/conf.py` & `pywrapid-0.2.7/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/docs/src/developer-guide.rst` & `pywrapid-0.2.7/docs/src/developer-guide.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/docs/src/features/config.rst` & `pywrapid-0.2.7/docs/src/features/config.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/docs/src/features/log.rst` & `pywrapid-0.2.7/docs/src/features/log.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/docs/src/features/webclient.rst` & `pywrapid-0.2.7/docs/src/features/webclient.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/docs/src/user-guide.rst` & `pywrapid-0.2.7/docs/src/user-guide.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/pyproject.toml` & `pywrapid-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/src/pywrapid/config/config.py` & `pywrapid-0.2.7/src/pywrapid/config/config.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/src/pywrapid/config/exceptions.py` & `pywrapid-0.2.7/src/pywrapid/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/src/pywrapid/log/application_log.py` & `pywrapid-0.2.7/src/pywrapid/log/application_log.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/src/pywrapid/utils/dict_tools.py` & `pywrapid-0.2.7/src/pywrapid/utils/dict_tools.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/src/pywrapid/utils/file_tools.py` & `pywrapid-0.2.7/src/pywrapid/utils/file_tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,7 +23,61 @@
         and os.path.isfile(path)
         and os.access(path, os.R_OK)
         and os.path.getsize(path) > 0
     ):
         return True
 
     return False
+
+
+def is_file_writable(path: str) -> bool:
+    """Checks a file in a given path to make sure it:
+        - exists
+        - is a file
+        - is writable
+
+    Args:
+        path (str): Path to configuration file.
+
+    Returns:
+        bool: True/False.
+    """
+    if os.path.exists(path) and os.path.isfile(path) and os.access(path, os.W_OK):
+        return True
+
+    return False
+
+
+def is_directory_readable(path: str) -> bool:
+    """Checks a directory in a given path to make sure it:
+        - exists
+        - is a directory
+        - is readable
+
+    Args:
+        path (str): Path to configuration file.
+
+    Returns:
+        bool: True/False.
+    """
+    if os.path.exists(path) and os.path.isdir(path) and os.access(path, os.R_OK):
+        return True
+
+    return False
+
+
+def is_directory_writable(path: str) -> bool:
+    """Checks a directory in a given path to make sure it:
+        - exists
+        - is a directory
+        - is writable
+
+    Args:
+        path (str): Path to configuration file.
+
+    Returns:
+        bool: True/False.
+    """
+    if os.path.exists(path) and os.path.isdir(path) and os.access(path, os.W_OK):
+        return True
+
+    return False
```

### Comparing `pywrapid-0.2.6/src/pywrapid/webclient/__init__.py` & `pywrapid-0.2.7/src/pywrapid/webclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/src/pywrapid/webclient/exceptions.py` & `pywrapid-0.2.7/src/pywrapid/webclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/src/pywrapid/webclient/web.py` & `pywrapid-0.2.7/src/pywrapid/webclient/web.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/src/pywrapid.egg-info/PKG-INFO` & `pywrapid-0.2.7/src/pywrapid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywrapid
-Version: 0.2.6
+Version: 0.2.7
 Summary: Collection of wrapper libraries for rapid development of python applications
 Author-email: Jonas Werme <jonas.werme@nsahq.se>, Marcus Wallgren <marcus.wallgren@nsahq.se>
 Maintainer-email: Jonas Werme <jonas.werme@nsahq.se>, Marcus Wallgren <marcus.wallgren@nsahq.se>
 License: MIT License
         
         Copyright (c) 2022 NSAHQ
```

### Comparing `pywrapid-0.2.6/src/pywrapid.egg-info/SOURCES.txt` & `pywrapid-0.2.7/src/pywrapid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/tests/test_pywrapid_config_config.py` & `pywrapid-0.2.7/tests/test_pywrapid_config_config.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/tests/test_pywrapid_logging_logging.py` & `pywrapid-0.2.7/tests/test_pywrapid_logging_logging.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/tests/test_pywrapid_webclient_web.py` & `pywrapid-0.2.7/tests/test_pywrapid_webclient_web.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.6/tox.ini` & `pywrapid-0.2.7/tox.ini`

 * *Files identical despite different names*

