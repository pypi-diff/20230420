# Comparing `tmp/oslili-cli-0.6.tar.gz` & `tmp/oslili-cli-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslili-cli-0.6.tar", last modified: Thu Apr 20 13:03:38 2023, max compression
+gzip compressed data, was "oslili-cli-0.7.tar", last modified: Thu Apr 20 13:09:48 2023, max compression
```

## Comparing `oslili-cli-0.6.tar` & `oslili-cli-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:03:38.237239 oslili-cli-0.6/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2023-04-09 07:38:24.000000 oslili-cli-0.6/LICENSE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       42 2023-04-09 07:38:24.000000 oslili-cli-0.6/NOTICE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1816 2023-04-20 13:03:38.237554 oslili-cli-0.6/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1277 2023-04-20 04:48:46.000000 oslili-cli-0.6/README.md
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:03:38.234796 oslili-cli-0.6/oslili_cli.egg-info/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1816 2023-04-20 13:03:38.000000 oslili-cli-0.6/oslili_cli.egg-info/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      276 2023-04-20 13:03:38.000000 oslili-cli-0.6/oslili_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2023-04-20 13:03:38.000000 oslili-cli-0.6/oslili_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       44 2023-04-20 13:03:38.000000 oslili-cli-0.6/oslili_cli.egg-info/entry_points.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        7 2023-04-20 13:03:38.000000 oslili-cli-0.6/oslili_cli.egg-info/requires.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        4 2023-04-20 13:03:38.000000 oslili-cli-0.6/oslili_cli.egg-info/top_level.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       79 2023-04-20 13:03:38.239046 oslili-cli-0.6/setup.cfg
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1054 2023-04-20 13:03:34.000000 oslili-cli-0.6/setup.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:03:38.236396 oslili-cli-0.6/src/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2023-04-09 07:38:24.000000 oslili-cli-0.6/src/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      914 2023-04-13 19:34:18.000000 oslili-cli-0.6/src/cli.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:09:48.510657 oslili-cli-0.7/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2023-04-09 07:38:24.000000 oslili-cli-0.7/LICENSE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       42 2023-04-09 07:38:24.000000 oslili-cli-0.7/NOTICE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1805 2023-04-20 13:09:48.510817 oslili-cli-0.7/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1277 2023-04-20 04:48:46.000000 oslili-cli-0.7/README.md
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:09:48.509113 oslili-cli-0.7/oslili_cli.egg-info/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1805 2023-04-20 13:09:48.000000 oslili-cli-0.7/oslili_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      276 2023-04-20 13:09:48.000000 oslili-cli-0.7/oslili_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2023-04-20 13:09:48.000000 oslili-cli-0.7/oslili_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       44 2023-04-20 13:09:48.000000 oslili-cli-0.7/oslili_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        7 2023-04-20 13:09:48.000000 oslili-cli-0.7/oslili_cli.egg-info/requires.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        4 2023-04-20 13:09:48.000000 oslili-cli-0.7/oslili_cli.egg-info/top_level.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       79 2023-04-20 13:09:48.511507 oslili-cli-0.7/setup.cfg
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1043 2023-04-20 13:08:08.000000 oslili-cli-0.7/setup.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2023-04-20 13:09:48.510072 oslili-cli-0.7/src/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2023-04-09 07:38:24.000000 oslili-cli-0.7/src/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      914 2023-04-13 19:34:18.000000 oslili-cli-0.7/src/cli.py
```

### Comparing `oslili-cli-0.6/LICENSE` & `oslili-cli-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oslili-cli-0.6/PKG-INFO` & `oslili-cli-0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: oslili-cli
-Version: 0.6
+Version: 0.7
 Summary: Open Source License Identification Library
 Home-page: https://github.com/oscarvalenzuelab/oslili-cli
 Author: Oscar Valenzuela B.
-Author-email: oscar.valenzuela.b@gmail.com
+Author-email: alkamod@gmail.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oslili-cli-0.6/README.md` & `oslili-cli-0.7/README.md`

 * *Files identical despite different names*

### Comparing `oslili-cli-0.6/oslili_cli.egg-info/PKG-INFO` & `oslili-cli-0.7/oslili_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: oslili-cli
-Version: 0.6
+Version: 0.7
 Summary: Open Source License Identification Library
 Home-page: https://github.com/oscarvalenzuelab/oslili-cli
 Author: Oscar Valenzuela B.
-Author-email: oscar.valenzuela.b@gmail.com
+Author-email: alkamod@gmail.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oslili-cli-0.6/setup.py` & `oslili-cli-0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pathlib
 import sys
 from setuptools import setup, find_packages
 
 
 HERE = pathlib.Path(__file__).parent
-VERSION = '0.6'
+VERSION = '0.7'
 PACKAGE_NAME = 'oslili-cli'
 AUTHOR = 'Oscar Valenzuela B.'
-AUTHOR_EMAIL = 'oscar.valenzuela.b@gmail.com'
+AUTHOR_EMAIL = 'alkamod@gmail.com'
 URL = 'https://github.com/oscarvalenzuelab/oslili-cli'
 LICENSE = 'Apache-2.0'
 DESCRIPTION = 'Open Source License Identification Library'
 LONG_DESCRIPTION = (HERE / "README.md").read_text()
 LONG_DESC_TYPE = "text/markdown"
 
 setup(
```

### Comparing `oslili-cli-0.6/src/cli.py` & `oslili-cli-0.7/src/cli.py`

 * *Files identical despite different names*

