# Comparing `tmp/gradient-accumulator-0.4.0.tar.gz` & `tmp/gradient-accumulator-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gradient-accumulator-0.4.0.tar", last modified: Sat Apr 15 11:02:33 2023, max compression
+gzip compressed data, was "dist/gradient-accumulator-0.4.1.tar", last modified: Thu Apr 20 17:37:20 2023, max compression
```

## Comparing `gradient-accumulator-0.4.0.tar` & `gradient-accumulator-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     8328 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6420 2023-04-15 11:01:54.000000 gradient-accumulator-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator/
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-04-15 11:01:54.000000 gradient-accumulator-0.4.0/gradient_accumulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14947 2023-04-15 11:01:54.000000 gradient-accumulator-0.4.0/gradient_accumulator/accumulators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2538 2023-04-15 11:01:54.000000 gradient-accumulator-0.4.0/gradient_accumulator/agc.py
--rw-r--r--   0 runner    (1001) docker     (122)     6463 2023-04-15 11:01:54.000000 gradient-accumulator-0.4.0/gradient_accumulator/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8328 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-04-15 11:01:54.000000 gradient-accumulator-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 17:37:20.000000 gradient-accumulator-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     8336 2023-04-20 17:37:20.000000 gradient-accumulator-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6428 2023-04-20 17:36:42.000000 gradient-accumulator-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 17:37:20.000000 gradient-accumulator-0.4.1/gradient_accumulator/
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-04-20 17:36:42.000000 gradient-accumulator-0.4.1/gradient_accumulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14947 2023-04-20 17:36:42.000000 gradient-accumulator-0.4.1/gradient_accumulator/accumulators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2538 2023-04-20 17:36:42.000000 gradient-accumulator-0.4.1/gradient_accumulator/agc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7702 2023-04-20 17:36:42.000000 gradient-accumulator-0.4.1/gradient_accumulator/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 17:37:20.000000 gradient-accumulator-0.4.1/gradient_accumulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8336 2023-04-20 17:37:20.000000 gradient-accumulator-0.4.1/gradient_accumulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-04-20 17:37:20.000000 gradient-accumulator-0.4.1/gradient_accumulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 17:37:20.000000 gradient-accumulator-0.4.1/gradient_accumulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-20 17:37:20.000000 gradient-accumulator-0.4.1/gradient_accumulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-20 17:37:20.000000 gradient-accumulator-0.4.1/gradient_accumulator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-20 17:37:20.000000 gradient-accumulator-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-04-20 17:36:42.000000 gradient-accumulator-0.4.1/setup.py
```

### Comparing `gradient-accumulator-0.4.0/PKG-INFO` & `gradient-accumulator-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: gradient-accumulator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Package for gradient accumulation in TensorFlow
 Home-page: https://github.com/andreped/GradientAccumulator
 Author: André Pedersen and David Bouget and Javier Pérez de Frutos
 Author-email: andrped94@gmail.com
 License: UNKNOWN
 Description: <div align="center">
-        <img src="assets/accum_grad_v5.png" width="30%" alt='gradient-accumulator'>
+        <img src="assets/accum_grad_v5_reduced.png" width="35%" alt='gradient-accumulator'>
         <h1 align="center">GradientAccumulator</h1>
         <h3 align="center">Seemless gradient accumulation for TensorFlow 2</h3>
         
         [![Pip Downloads](https://img.shields.io/pypi/dm/gradient-accumulator?label=pip%20downloads&logo=python)](https://pypi.org/project/gradient-accumulator/)
         [![PyPI version](https://badge.fury.io/py/gradient-accumulator.svg)](https://badge.fury.io/py/gradient-accumulator)
         [![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
         [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7831244.svg)](https://doi.org/10.5281/zenodo.7831244)
```

### Comparing `gradient-accumulator-0.4.0/README.md` & `gradient-accumulator-0.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div align="center">
-<img src="assets/accum_grad_v5.png" width="30%" alt='gradient-accumulator'>
+<img src="assets/accum_grad_v5_reduced.png" width="35%" alt='gradient-accumulator'>
 <h1 align="center">GradientAccumulator</h1>
 <h3 align="center">Seemless gradient accumulation for TensorFlow 2</h3>
 
 [![Pip Downloads](https://img.shields.io/pypi/dm/gradient-accumulator?label=pip%20downloads&logo=python)](https://pypi.org/project/gradient-accumulator/)
 [![PyPI version](https://badge.fury.io/py/gradient-accumulator.svg)](https://badge.fury.io/py/gradient-accumulator)
 [![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7831244.svg)](https://doi.org/10.5281/zenodo.7831244)
```

### Comparing `gradient-accumulator-0.4.0/gradient_accumulator/accumulators.py` & `gradient-accumulator-0.4.1/gradient_accumulator/accumulators.py`

 * *Files identical despite different names*

### Comparing `gradient-accumulator-0.4.0/gradient_accumulator/agc.py` & `gradient-accumulator-0.4.1/gradient_accumulator/agc.py`

 * *Files identical despite different names*

### Comparing `gradient-accumulator-0.4.0/gradient_accumulator.egg-info/PKG-INFO` & `gradient-accumulator-0.4.1/gradient_accumulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: gradient-accumulator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Package for gradient accumulation in TensorFlow
 Home-page: https://github.com/andreped/GradientAccumulator
 Author: André Pedersen and David Bouget and Javier Pérez de Frutos
 Author-email: andrped94@gmail.com
 License: UNKNOWN
 Description: <div align="center">
-        <img src="assets/accum_grad_v5.png" width="30%" alt='gradient-accumulator'>
+        <img src="assets/accum_grad_v5_reduced.png" width="35%" alt='gradient-accumulator'>
         <h1 align="center">GradientAccumulator</h1>
         <h3 align="center">Seemless gradient accumulation for TensorFlow 2</h3>
         
         [![Pip Downloads](https://img.shields.io/pypi/dm/gradient-accumulator?label=pip%20downloads&logo=python)](https://pypi.org/project/gradient-accumulator/)
         [![PyPI version](https://badge.fury.io/py/gradient-accumulator.svg)](https://badge.fury.io/py/gradient-accumulator)
         [![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
         [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7831244.svg)](https://doi.org/10.5281/zenodo.7831244)
```

### Comparing `gradient-accumulator-0.4.0/setup.py` & `gradient-accumulator-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gradient-accumulator",
-    version="0.4.0",
+    version="0.4.1",
     author="André Pedersen and David Bouget and Javier Pérez de Frutos",
     author_email="andrped94@gmail.com",
     description="Package for gradient accumulation in TensorFlow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andreped/GradientAccumulator",
     packages=setuptools.find_packages(exclude=('tests', 'notebooks', 'assets', 'docs')),
```

