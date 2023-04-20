# Comparing `tmp/oslili-cli-0.5.tar.gz` & `tmp/oslili-cli-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslili-cli-0.5.tar", last modified: Thu Apr 20 13:01:08 2023, max compression
+gzip compressed data, was "oslili-cli-0.6.tar", last modified: Thu Apr 20 13:03:38 2023, max compression
```

## Comparing `oslili-cli-0.5.tar` & `oslili-cli-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:01:08.539996 oslili-cli-0.5/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2023-04-09 07:38:24.000000 oslili-cli-0.5/LICENSE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       42 2023-04-09 07:38:24.000000 oslili-cli-0.5/NOTICE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      478 2023-04-20 13:01:08.540295 oslili-cli-0.5/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1277 2023-04-20 04:48:46.000000 oslili-cli-0.5/README.md
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:01:08.537710 oslili-cli-0.5/oslili_cli.egg-info/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      478 2023-04-20 13:01:08.000000 oslili-cli-0.5/oslili_cli.egg-info/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      276 2023-04-20 13:01:08.000000 oslili-cli-0.5/oslili_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2023-04-20 13:01:08.000000 oslili-cli-0.5/oslili_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       44 2023-04-20 13:01:08.000000 oslili-cli-0.5/oslili_cli.egg-info/entry_points.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        7 2023-04-20 13:01:08.000000 oslili-cli-0.5/oslili_cli.egg-info/requires.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        4 2023-04-20 13:01:08.000000 oslili-cli-0.5/oslili_cli.egg-info/top_level.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       79 2023-04-20 13:01:08.541525 oslili-cli-0.5/setup.cfg
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      945 2023-04-20 13:01:01.000000 oslili-cli-0.5/setup.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:01:08.539128 oslili-cli-0.5/src/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2023-04-09 07:38:24.000000 oslili-cli-0.5/src/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      914 2023-04-13 19:34:18.000000 oslili-cli-0.5/src/cli.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:03:38.237239 oslili-cli-0.6/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2023-04-09 07:38:24.000000 oslili-cli-0.6/LICENSE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       42 2023-04-09 07:38:24.000000 oslili-cli-0.6/NOTICE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1816 2023-04-20 13:03:38.237554 oslili-cli-0.6/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1277 2023-04-20 04:48:46.000000 oslili-cli-0.6/README.md
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:03:38.234796 oslili-cli-0.6/oslili_cli.egg-info/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1816 2023-04-20 13:03:38.000000 oslili-cli-0.6/oslili_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      276 2023-04-20 13:03:38.000000 oslili-cli-0.6/oslili_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2023-04-20 13:03:38.000000 oslili-cli-0.6/oslili_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       44 2023-04-20 13:03:38.000000 oslili-cli-0.6/oslili_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        7 2023-04-20 13:03:38.000000 oslili-cli-0.6/oslili_cli.egg-info/requires.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        4 2023-04-20 13:03:38.000000 oslili-cli-0.6/oslili_cli.egg-info/top_level.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       79 2023-04-20 13:03:38.239046 oslili-cli-0.6/setup.cfg
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1054 2023-04-20 13:03:34.000000 oslili-cli-0.6/setup.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:03:38.236396 oslili-cli-0.6/src/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2023-04-09 07:38:24.000000 oslili-cli-0.6/src/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      914 2023-04-13 19:34:18.000000 oslili-cli-0.6/src/cli.py
```

### Comparing `oslili-cli-0.5/LICENSE` & `oslili-cli-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oslili-cli-0.5/README.md` & `oslili-cli-0.6/README.md`

 * *Files identical despite different names*

### Comparing `oslili-cli-0.5/src/cli.py` & `oslili-cli-0.6/src/cli.py`

 * *Files identical despite different names*

