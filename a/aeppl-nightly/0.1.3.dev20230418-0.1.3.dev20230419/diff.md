# Comparing `tmp/aeppl-nightly-0.1.3.dev20230418.tar.gz` & `tmp/aeppl-nightly-0.1.3.dev20230419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeppl-nightly-0.1.3.dev20230418.tar", last modified: Tue Apr 18 00:29:28 2023, max compression
+gzip compressed data, was "aeppl-nightly-0.1.3.dev20230419.tar", last modified: Wed Apr 19 00:31:50 2023, max compression
```

## Comparing `aeppl-nightly-0.1.3.dev20230418.tar` & `aeppl-nightly-0.1.3.dev20230419.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:29:28.459647 aeppl-nightly-0.1.3.dev20230418/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-18 00:29:28.459647 aeppl-nightly-0.1.3.dev20230418/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:29:28.463647 aeppl-nightly-0.1.3.dev20230418/aeppl/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-18 00:29:28.463647 aeppl-nightly-0.1.3.dev20230418/aeppl/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30620 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/aeppl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:29:28.459647 aeppl-nightly-0.1.3.dev20230418/aeppl_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-18 00:29:28.000000 aeppl-nightly-0.1.3.dev20230418/aeppl_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-18 00:29:28.000000 aeppl-nightly-0.1.3.dev20230418/aeppl_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:29:28.000000 aeppl-nightly-0.1.3.dev20230418/aeppl_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:29:28.000000 aeppl-nightly-0.1.3.dev20230418/aeppl_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 00:29:28.000000 aeppl-nightly-0.1.3.dev20230418/aeppl_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 00:29:28.000000 aeppl-nightly-0.1.3.dev20230418/aeppl_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-18 00:29:28.463647 aeppl-nightly-0.1.3.dev20230418/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:29:28.459647 aeppl-nightly-0.1.3.dev20230418/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_composite_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    23229 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-04-18 00:29:11.000000 aeppl-nightly-0.1.3.dev20230418/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:31:50.016165 aeppl-nightly-0.1.3.dev20230419/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-19 00:31:50.016165 aeppl-nightly-0.1.3.dev20230419/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:31:50.020166 aeppl-nightly-0.1.3.dev20230419/aeppl/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 00:31:50.020166 aeppl-nightly-0.1.3.dev20230419/aeppl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30620 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/aeppl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:31:50.016165 aeppl-nightly-0.1.3.dev20230419/aeppl_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-19 00:31:50.000000 aeppl-nightly-0.1.3.dev20230419/aeppl_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-19 00:31:50.000000 aeppl-nightly-0.1.3.dev20230419/aeppl_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:31:50.000000 aeppl-nightly-0.1.3.dev20230419/aeppl_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:31:49.000000 aeppl-nightly-0.1.3.dev20230419/aeppl_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 00:31:50.000000 aeppl-nightly-0.1.3.dev20230419/aeppl_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 00:31:50.000000 aeppl-nightly-0.1.3.dev20230419/aeppl_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-19 00:31:50.020166 aeppl-nightly-0.1.3.dev20230419/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:31:50.016165 aeppl-nightly-0.1.3.dev20230419/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_composite_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-04-19 00:31:38.000000 aeppl-nightly-0.1.3.dev20230419/versioneer.py
```

### Comparing `aeppl-nightly-0.1.3.dev20230418/LICENSE` & `aeppl-nightly-0.1.3.dev20230419/LICENSE`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/PKG-INFO` & `aeppl-nightly-0.1.3.dev20230419/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.3.dev20230418
+Version: 0.1.3.dev20230419
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.3.dev20230418/README.md` & `aeppl-nightly-0.1.3.dev20230419/README.md`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/abstract.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/censoring.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/cumsum.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/dists.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/dists.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/joint_logprob.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/logprob.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/mixture.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/printing.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/rewriting.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/scan.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/tensor.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/transforms.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl/utils.py` & `aeppl-nightly-0.1.3.dev20230419/aeppl/utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl_nightly.egg-info/PKG-INFO` & `aeppl-nightly-0.1.3.dev20230419/aeppl_nightly.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.3.dev20230418
+Version: 0.1.3.dev20230419
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.3.dev20230418/aeppl_nightly.egg-info/SOURCES.txt` & `aeppl-nightly-0.1.3.dev20230419/aeppl_nightly.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 versioneer.py
 aeppl/__init__.py
 aeppl/_version.py
 aeppl/abstract.py
 aeppl/censoring.py
+aeppl/convolutions.py
 aeppl/cumsum.py
 aeppl/dists.py
 aeppl/joint_logprob.py
 aeppl/logprob.py
 aeppl/mixture.py
 aeppl/printing.py
 aeppl/rewriting.py
@@ -24,14 +25,15 @@
 aeppl_nightly.egg-info/dependency_links.txt
 aeppl_nightly.egg-info/not-zip-safe
 aeppl_nightly.egg-info/requires.txt
 aeppl_nightly.egg-info/top_level.txt
 tests/test_abstract.py
 tests/test_censoring.py
 tests/test_composite_logprob.py
+tests/test_convolutions.py
 tests/test_cumsum.py
 tests/test_dist.py
 tests/test_joint_logprob.py
 tests/test_logprob.py
 tests/test_mixture.py
 tests/test_printing.py
 tests/test_rewriting.py
```

### Comparing `aeppl-nightly-0.1.3.dev20230418/setup.cfg` & `aeppl-nightly-0.1.3.dev20230419/setup.cfg`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/setup.py` & `aeppl-nightly-0.1.3.dev20230419/setup.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_abstract.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_censoring.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_composite_logprob.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_composite_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_cumsum.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_dist.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_joint_logprob.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_logprob.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_mixture.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_printing.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_rewriting.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_scan.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_tensor.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_transforms.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -671,25 +671,14 @@
 
     assert np.isclose(
         logp_fn(y_test_val),
         sp.stats.halfnorm(0, 1).logpdf(np.exp(y_test_val)) + y_test_val,
     )
 
 
-def test_loc_transform_multiple_rvs_fails1():
-    srng = at.random.RandomStream(0)
-
-    x_rv1 = srng.normal(name="x_rv1")
-    x_rv2 = srng.normal(name="x_rv2")
-    y_rv = x_rv1 + x_rv2
-
-    with pytest.raises(DensityNotFound):
-        joint_logprob(y_rv)
-
-
 def test_nested_loc_transform_multiple_rvs_fails2():
     srng = at.random.RandomStream(0)
 
     x_rv1 = srng.normal(name="x_rv1")
     x_rv2 = at.cos(srng.normal(name="x_rv2"))
     y_rv = x_rv1 + x_rv2
 
@@ -812,10 +801,11 @@
     srng = at.random.RandomStream(0)
 
     A_rv = srng.normal(1.0, name="A")
     X_rv = srng.normal(1.0, name="X")
     Z_rv = A_rv - X_rv
 
     logp, (z_vv, a_vv) = joint_logprob(Z_rv, A_rv)
+
     z_logp_fn = aesara.function([z_vv, a_vv], logp)
     exp_logp = sp.stats.norm.logpdf(5.0 - 7.3, 1.0) + sp.stats.norm.logpdf(5.0, 1.0)
     assert np.isclose(z_logp_fn(7.3, 5.0), exp_logp)
```

### Comparing `aeppl-nightly-0.1.3.dev20230418/tests/test_utils.py` & `aeppl-nightly-0.1.3.dev20230419/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230418/versioneer.py` & `aeppl-nightly-0.1.3.dev20230419/versioneer.py`

 * *Files identical despite different names*

