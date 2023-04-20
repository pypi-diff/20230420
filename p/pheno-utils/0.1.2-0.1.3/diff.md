# Comparing `tmp/pheno-utils-0.1.2.tar.gz` & `tmp/pheno-utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.1.2.tar", last modified: Thu Apr 20 19:11:15 2023, max compression
+gzip compressed data, was "pheno-utils-0.1.3.tar", last modified: Thu Apr 20 19:48:37 2023, max compression
```

## Comparing `pheno-utils-0.1.2.tar` & `pheno-utils-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 19:11:15.874888 pheno-utils-0.1.2/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.2/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.2/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 19:11:15.874463 pheno-utils-0.1.2/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.2/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 19:11:15.870638 pheno-utils-0.1.2/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13667 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     5111 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/basic_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/cgm_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16345 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/dates_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/ecg_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 19:11:15.873766 pheno-utils-0.1.2/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 19:11:15.000000 pheno-utils-0.1.2/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-20 19:11:15.000000 pheno-utils-0.1.2/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-20 19:11:15.000000 pheno-utils-0.1.2/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-20 19:11:15.000000 pheno-utils-0.1.2/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.2/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-20 19:11:15.000000 pheno-utils-0.1.2/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-20 19:11:15.000000 pheno-utils-0.1.2/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-20 19:03:40.000000 pheno-utils-0.1.2/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-20 19:11:15.875044 pheno-utils-0.1.2/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.2/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 19:48:37.397258 pheno-utils-0.1.3/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.3/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.3/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 19:48:37.396969 pheno-utils-0.1.3/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.3/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 19:48:37.394197 pheno-utils-0.1.3/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13667 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     5111 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/basic_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/cgm_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     3198 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16345 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/dates_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 19:48:37.396503 pheno-utils-0.1.3/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 19:48:37.000000 pheno-utils-0.1.3/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-20 19:48:37.000000 pheno-utils-0.1.3/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-20 19:48:37.000000 pheno-utils-0.1.3/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-20 19:48:37.000000 pheno-utils-0.1.3/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.3/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-20 19:48:37.000000 pheno-utils-0.1.3/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-20 19:48:37.000000 pheno-utils-0.1.3/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-20 19:42:00.000000 pheno-utils-0.1.3/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-20 19:48:37.397393 pheno-utils-0.1.3/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.3/setup.py
```

### Comparing `pheno-utils-0.1.2/LICENSE` & `pheno-utils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.2/PKG-INFO` & `pheno-utils-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.2/pheno_utils/_modidx.py` & `pheno-utils-0.1.3/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.2/pheno_utils/age_reference_plots.py` & `pheno-utils-0.1.3/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.2/pheno_utils/basic_analysis.py` & `pheno-utils-0.1.3/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.2/pheno_utils/basic_plots.py` & `pheno-utils-0.1.3/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.2/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.1.3/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.2/pheno_utils/cgm_plots.py` & `pheno-utils-0.1.3/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.2/pheno_utils/config.py` & `pheno-utils-0.1.3/pheno_utils/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_config.ipynb.
 
 # %% auto 0
 __all__ = ['REF_COLOR', 'FEMALE_COLOR', 'MALE_COLOR', 'ALL_COLOR', 'GLUC_COLOR', 'FOOD_COLOR', 'DATASETS_PATH',
-           'POPULATION_DATASET', 'generate_synthetic_data', 'generate_synthetic_data_like']
+           'POPULATION_DATASET', 'CONFIG_FILES', 'generate_synthetic_data', 'generate_synthetic_data_like']
 
 # %% ../nbs/00_config.ipynb 3
+import os
+
 import numpy as np
 import pandas as pd
 
 # %% ../nbs/00_config.ipynb 4
 REF_COLOR = "k"
 FEMALE_COLOR = "C1"
 MALE_COLOR = "C0"
 ALL_COLOR = "C5"
 
 GLUC_COLOR = "C0"
 FOOD_COLOR = "C1"
 
-# DATASETS_PATH = '/home/ec2-user/studies/'
-# POPULATION_DATASET = 'Population_Characteristics'
-
 DATASETS_PATH = '/home/ec2-user/studies/hpp/'
 POPULATION_DATASET = 'population'
+CONFIG_FILES = ['~/.pheno/config', '/efs/.pheno/config']
+
+for cf in CONFIG_FILES:
+    cf = os.path.expanduser(cf)
+    if not os.path.isfile(cf):
+        continue
+    with open(cf, 'r') as f:
+        for line in f:
+            if line.startswith('DATASETS_PATH'):
+                DATASETS_PATH = line.split('=')[1].strip()
+            elif line.startswith('POPULATION_DATASET'):
+                POPULATION_DATASET = line.split('=')[1].strip()
+
 
 # %% ../nbs/00_config.ipynb 5
 def generate_synthetic_data(n: int = 1000) -> pd.DataFrame:
     """
     Generates a sample DataFrame containing age, gender, and value data.
 
     Args:
```

### Comparing `pheno-utils-0.1.2/pheno_utils/data_loader.py` & `pheno-utils-0.1.3/pheno_utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.2/pheno_utils/dates_plots.py` & `pheno-utils-0.1.3/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.2/pheno_utils/ecg_analysis.py` & `pheno-utils-0.1.3/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.2/pheno_utils/sleep_plots.py` & `pheno-utils-0.1.3/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.2/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.1.3/pheno_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.2/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.1.3/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.2/settings.ini` & `pheno-utils-0.1.3/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.1.2
+version = 0.1.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.1.2/setup.py` & `pheno-utils-0.1.3/setup.py`

 * *Files identical despite different names*

