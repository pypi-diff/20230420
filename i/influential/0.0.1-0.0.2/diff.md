# Comparing `tmp/influential-0.0.1.tar.gz` & `tmp/influential-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influential-0.0.1.tar", last modified: Tue Apr 18 07:06:31 2023, max compression
+gzip compressed data, was "influential-0.0.2.tar", last modified: Thu Apr 20 02:09:52 2023, max compression
```

## Comparing `influential-0.0.1.tar` & `influential-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-04-18 07:06:31.223788 influential-0.0.1/
--rw-r--r--   0 adriansalavaty   (501) staff       (20)     1548 2023-04-18 07:06:31.223650 influential-0.0.1/PKG-INFO
--rw-------   0 adriansalavaty   (501) staff       (20)     4176 2023-04-18 00:25:09.000000 influential-0.0.1/README.md
-drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-04-18 07:06:31.222587 influential-0.0.1/influential/
--rw-------   0 adriansalavaty   (501) staff       (20)      368 2023-04-18 07:05:27.000000 influential-0.0.1/influential/__init__.py
--rw-------   0 adriansalavaty   (501) staff       (20)    43384 2023-04-18 07:02:15.000000 influential-0.0.1/influential/centrality.py
--rw-r--r--   0 adriansalavaty   (501) staff       (20)    40515 2023-04-18 06:51:52.000000 influential-0.0.1/influential/exir.py
--rw-r--r--   0 adriansalavaty   (501) staff       (20)      997 2023-01-21 23:50:04.000000 influential-0.0.1/influential/ranNorm.py
--rw-r--r--   0 adriansalavaty   (501) staff       (20)      843 2023-04-18 06:52:36.000000 influential-0.0.1/influential/rank.py
--rw-r--r--   0 adriansalavaty   (501) staff       (20)     4011 2023-02-13 05:41:32.000000 influential-0.0.1/influential/sir.py
--rw-r--r--   0 adriansalavaty   (501) staff       (20)     4936 2023-04-18 06:52:30.000000 influential-0.0.1/influential/stats.py
-drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-04-18 07:06:31.223475 influential-0.0.1/influential/test/
--rw-------   0 adriansalavaty   (501) staff       (20)        0 2022-07-27 08:42:02.000000 influential-0.0.1/influential/test/__init__.py
--rw-r--r--   0 adriansalavaty   (501) staff       (20)    37338 2023-04-18 06:53:13.000000 influential-0.0.1/influential/visualize.py
-drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-04-18 07:06:31.223322 influential-0.0.1/influential.egg-info/
--rw-r--r--   0 adriansalavaty   (501) staff       (20)     1548 2023-04-18 07:06:31.000000 influential-0.0.1/influential.egg-info/PKG-INFO
--rw-r--r--   0 adriansalavaty   (501) staff       (20)      399 2023-04-18 07:06:31.000000 influential-0.0.1/influential.egg-info/SOURCES.txt
--rw-r--r--   0 adriansalavaty   (501) staff       (20)        1 2023-04-18 07:06:31.000000 influential-0.0.1/influential.egg-info/dependency_links.txt
--rw-r--r--   0 adriansalavaty   (501) staff       (20)       76 2023-04-18 07:06:31.000000 influential-0.0.1/influential.egg-info/requires.txt
--rw-r--r--   0 adriansalavaty   (501) staff       (20)       12 2023-04-18 07:06:31.000000 influential-0.0.1/influential.egg-info/top_level.txt
--rw-r--r--   0 adriansalavaty   (501) staff       (20)       38 2023-04-18 07:06:31.223832 influential-0.0.1/setup.cfg
--rw-------   0 adriansalavaty   (501) staff       (20)     1923 2023-04-18 04:20:06.000000 influential-0.0.1/setup.py
+drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-04-20 02:09:52.452801 influential-0.0.2/
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)     1548 2023-04-20 02:09:52.452651 influential-0.0.2/PKG-INFO
+-rw-------   0 adriansalavaty   (501) staff       (20)     4401 2023-04-18 07:17:41.000000 influential-0.0.2/README.md
+drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-04-20 02:09:52.451481 influential-0.0.2/influential/
+-rw-------   0 adriansalavaty   (501) staff       (20)      381 2023-04-20 02:01:31.000000 influential-0.0.2/influential/__init__.py
+-rw-------   0 adriansalavaty   (501) staff       (20)    43384 2023-04-18 07:02:15.000000 influential-0.0.2/influential/centrality.py
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)    40515 2023-04-18 06:51:52.000000 influential-0.0.2/influential/exir.py
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)      997 2023-01-21 23:50:04.000000 influential-0.0.2/influential/ranNorm.py
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)      843 2023-04-18 06:52:36.000000 influential-0.0.2/influential/rank.py
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)     4011 2023-02-13 05:41:32.000000 influential-0.0.2/influential/sir.py
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)     4936 2023-04-18 06:52:30.000000 influential-0.0.2/influential/stats.py
+drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-04-20 02:09:52.452444 influential-0.0.2/influential/test/
+-rw-------   0 adriansalavaty   (501) staff       (20)        0 2022-07-27 08:42:02.000000 influential-0.0.2/influential/test/__init__.py
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)    37338 2023-04-18 06:53:13.000000 influential-0.0.2/influential/visualize.py
+drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-04-20 02:09:52.452306 influential-0.0.2/influential.egg-info/
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)     1548 2023-04-20 02:09:52.000000 influential-0.0.2/influential.egg-info/PKG-INFO
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)      399 2023-04-20 02:09:52.000000 influential-0.0.2/influential.egg-info/SOURCES.txt
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)        1 2023-04-20 02:09:52.000000 influential-0.0.2/influential.egg-info/dependency_links.txt
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)       76 2023-04-20 02:09:52.000000 influential-0.0.2/influential.egg-info/requires.txt
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)       12 2023-04-20 02:09:52.000000 influential-0.0.2/influential.egg-info/top_level.txt
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)       38 2023-04-20 02:09:52.452850 influential-0.0.2/setup.cfg
+-rw-------   0 adriansalavaty   (501) staff       (20)     1923 2023-04-20 02:03:16.000000 influential-0.0.2/setup.py
```

### Comparing `influential-0.0.1/PKG-INFO` & `influential-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influential
-Version: 0.0.1
+Version: 0.0.2
 Summary: Identification and Classification of the Most Influential Nodes
 Home-page: http://pypi.python.org/pypi/influential/
 Author: Adrian Salavaty
 Author-email: abbas.salavaty@gmail.com
 License: GPL-3
 Keywords: influential
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `influential-0.0.1/README.md` & `influential-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # influential <a href='https://github.com/asalavaty/python-influential'><img src='https://raw.githubusercontent.com/asalavaty/influential/master/man/figures/Symbol.png' align="right" height="221" /></a>
 
 <!-- badges: start -->
 
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/influential)](https://pypi.python.org/pypi/influential)
+[![PyPI wheels](https://img.shields.io/pypi/wheel/influential.svg)](https://pypi.python.org/pypi/influential)
 [![](https://img.shields.io/badge/Integrated%20Value%20of%20Influence-IVI-blue.svg)](https://doi.org/10.1016/j.patter.2020.100052)
 [![](https://img.shields.io/badge/SIR--based%20Influence%20Ranking-SIRIR-green.svg)](https://doi.org/10.1016/j.patter.2020.100052)
 [![](https://img.shields.io/badge/Experimental%20data--based%20Integrative%20Ranking-ExIR-blue.svg)](https://www.biorxiv.org/content/10.1101/2022.10.03.510585v1.abstract)
 <!-- badges: end -->
 
 ## Overview
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
 # influential [https://raw.githubusercontent.com/asalavaty/influential/master/
-man/figures/Symbol.png]  [![](https://img.shields.io/badge/
+man/figures/Symbol.png]  [![PyPI pyversions](https://img.shields.io/pypi/
+pyversions/influential)](https://pypi.python.org/pypi/influential) [![PyPI
+wheels](https://img.shields.io/pypi/wheel/influential.svg)](https://
+pypi.python.org/pypi/influential) [![](https://img.shields.io/badge/
 Integrated%20Value%20of%20Influence-IVI-blue.svg)](https://doi.org/10.1016/
 j.patter.2020.100052) [![](https://img.shields.io/badge/SIR--
 based%20Influence%20Ranking-SIRIR-green.svg)](https://doi.org/10.1016/
 j.patter.2020.100052) [![](https://img.shields.io/badge/Experimental%20data--
 based%20Integrative%20Ranking-ExIR-blue.svg)](https://www.biorxiv.org/content/
 10.1101/2022.10.03.510585v1.abstract)  ## Overview The goal of `influential` is
 to help identification of the most `influential` nodes in a network as well as
```

### Comparing `influential-0.0.1/influential/centrality.py` & `influential-0.0.2/influential/centrality.py`

 * *Files identical despite different names*

### Comparing `influential-0.0.1/influential/exir.py` & `influential-0.0.2/influential/exir.py`

 * *Files identical despite different names*

### Comparing `influential-0.0.1/influential/ranNorm.py` & `influential-0.0.2/influential/ranNorm.py`

 * *Files identical despite different names*

### Comparing `influential-0.0.1/influential/rank.py` & `influential-0.0.2/influential/rank.py`

 * *Files identical despite different names*

### Comparing `influential-0.0.1/influential/sir.py` & `influential-0.0.2/influential/sir.py`

 * *Files identical despite different names*

### Comparing `influential-0.0.1/influential/stats.py` & `influential-0.0.2/influential/stats.py`

 * *Files identical despite different names*

### Comparing `influential-0.0.1/influential/visualize.py` & `influential-0.0.2/influential/visualize.py`

 * *Files identical despite different names*

### Comparing `influential-0.0.1/influential.egg-info/PKG-INFO` & `influential-0.0.2/influential.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influential
-Version: 0.0.1
+Version: 0.0.2
 Summary: Identification and Classification of the Most Influential Nodes
 Home-page: http://pypi.python.org/pypi/influential/
 Author: Adrian Salavaty
 Author-email: abbas.salavaty@gmail.com
 License: GPL-3
 Keywords: influential
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `influential-0.0.1/setup.py` & `influential-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Identification and Classification of the Most Influential Nodes'
 LONG_DESCRIPTION = """
 
 Contains functions for the classification and ranking of top candidate features, reconstruction of networks from
 adjacency matrices and data frames, analysis of the topology of the network 
 and calculation of centrality measures, and identification of the most
 influential nodes. Also, a function is provided for running SIRIR model, which
```

