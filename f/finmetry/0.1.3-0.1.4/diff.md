# Comparing `tmp/finmetry-0.1.3.tar.gz` & `tmp/finmetry-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finmetry-0.1.3.tar", last modified: Fri Mar 10 14:21:41 2023, max compression
+gzip compressed data, was "finmetry-0.1.4.tar", last modified: Thu Apr 20 14:20:38 2023, max compression
```

## Comparing `finmetry-0.1.3.tar` & `finmetry-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:21:41.355241 finmetry-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-10 14:21:41.355241 finmetry-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-10 14:21:29.000000 finmetry-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-10 14:21:29.000000 finmetry-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 14:21:41.355241 finmetry-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-10 14:21:29.000000 finmetry-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:21:41.355241 finmetry-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:21:41.355241 finmetry-0.1.3/src/finmetry/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-10 14:21:29.000000 finmetry-0.1.3/src/finmetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-10 14:21:29.000000 finmetry-0.1.3/src/finmetry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-10 14:21:29.000000 finmetry-0.1.3/src/finmetry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:21:41.355241 finmetry-0.1.3/src/finmetry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-10 14:21:41.000000 finmetry-0.1.3/src/finmetry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-10 14:21:41.000000 finmetry-0.1.3/src/finmetry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 14:21:41.000000 finmetry-0.1.3/src/finmetry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-10 14:21:41.000000 finmetry-0.1.3/src/finmetry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-10 14:21:41.000000 finmetry-0.1.3/src/finmetry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:38.373339 finmetry-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-04-20 14:20:38.373339 finmetry-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21610 2023-04-20 14:20:28.000000 finmetry-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-20 14:20:28.000000 finmetry-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:20:38.373339 finmetry-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-20 14:20:28.000000 finmetry-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:38.369339 finmetry-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:38.369339 finmetry-0.1.4/src/finmetry/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 14:20:28.000000 finmetry-0.1.4/src/finmetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:38.373339 finmetry-0.1.4/src/finmetry/client_5paisa/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 14:20:28.000000 finmetry-0.1.4/src/finmetry/client_5paisa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-04-20 14:20:28.000000 finmetry-0.1.4/src/finmetry/client_5paisa/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 14:20:28.000000 finmetry-0.1.4/src/finmetry/client_5paisa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-04-20 14:20:28.000000 finmetry-0.1.4/src/finmetry/stock_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-20 14:20:28.000000 finmetry-0.1.4/src/finmetry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 14:20:28.000000 finmetry-0.1.4/src/finmetry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:38.369339 finmetry-0.1.4/src/finmetry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-04-20 14:20:38.000000 finmetry-0.1.4/src/finmetry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-20 14:20:38.000000 finmetry-0.1.4/src/finmetry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:20:38.000000 finmetry-0.1.4/src/finmetry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 14:20:38.000000 finmetry-0.1.4/src/finmetry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 14:20:38.000000 finmetry-0.1.4/src/finmetry.egg-info/top_level.txt
```

### Comparing `finmetry-0.1.3/setup.py` & `finmetry-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 
 requirements = [
-    "numpy",
-    "pandas",
-    "yfinance"
+    "numpy==1.21.5",
+    "pandas==1.4.1",
 ]
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
```

