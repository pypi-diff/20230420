# Comparing `tmp/pheno-utils-0.1.3.tar.gz` & `tmp/pheno-utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.1.3.tar", last modified: Thu Apr 20 19:48:37 2023, max compression
+gzip compressed data, was "pheno-utils-0.1.4.tar", last modified: Thu Apr 20 20:23:44 2023, max compression
```

## Comparing `pheno-utils-0.1.3.tar` & `pheno-utils-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 19:48:37.397258 pheno-utils-0.1.3/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.3/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.3/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 19:48:37.396969 pheno-utils-0.1.3/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.3/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 19:48:37.394197 pheno-utils-0.1.3/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13667 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     5111 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/basic_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/cgm_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     3198 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16345 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/dates_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/ecg_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-20 19:47:01.000000 pheno-utils-0.1.3/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 19:48:37.396503 pheno-utils-0.1.3/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 19:48:37.000000 pheno-utils-0.1.3/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-20 19:48:37.000000 pheno-utils-0.1.3/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-20 19:48:37.000000 pheno-utils-0.1.3/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-20 19:48:37.000000 pheno-utils-0.1.3/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.3/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-20 19:48:37.000000 pheno-utils-0.1.3/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-20 19:48:37.000000 pheno-utils-0.1.3/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-20 19:42:00.000000 pheno-utils-0.1.3/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-20 19:48:37.397393 pheno-utils-0.1.3/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.3/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 20:23:44.902229 pheno-utils-0.1.4/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.4/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.4/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 20:23:44.901822 pheno-utils-0.1.4/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.4/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 20:23:44.894069 pheno-utils-0.1.4/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13667 2023-04-20 20:16:56.000000 pheno-utils-0.1.4/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     5111 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/basic_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/cgm_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     3414 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16326 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/dates_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-20 20:16:55.000000 pheno-utils-0.1.4/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 20:23:44.901224 pheno-utils-0.1.4/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 20:23:44.000000 pheno-utils-0.1.4/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-20 20:23:44.000000 pheno-utils-0.1.4/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-20 20:23:44.000000 pheno-utils-0.1.4/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-20 20:23:44.000000 pheno-utils-0.1.4/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.4/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-20 20:23:44.000000 pheno-utils-0.1.4/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-20 20:23:44.000000 pheno-utils-0.1.4/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-20 20:11:29.000000 pheno-utils-0.1.4/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-20 20:23:44.902415 pheno-utils-0.1.4/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.4/setup.py
```

### Comparing `pheno-utils-0.1.3/LICENSE` & `pheno-utils-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.3/PKG-INFO` & `pheno-utils-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.3/pheno_utils/_modidx.py` & `pheno-utils-0.1.4/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.3/pheno_utils/age_reference_plots.py` & `pheno-utils-0.1.4/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.3/pheno_utils/basic_analysis.py` & `pheno-utils-0.1.4/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.3/pheno_utils/basic_plots.py` & `pheno-utils-0.1.4/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.3/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.1.4/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.3/pheno_utils/cgm_plots.py` & `pheno-utils-0.1.4/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.3/pheno_utils/config.py` & `pheno-utils-0.1.4/pheno_utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_config.ipynb.
 
 # %% auto 0
-__all__ = ['REF_COLOR', 'FEMALE_COLOR', 'MALE_COLOR', 'ALL_COLOR', 'GLUC_COLOR', 'FOOD_COLOR', 'DATASETS_PATH',
+__all__ = ['REF_COLOR', 'FEMALE_COLOR', 'MALE_COLOR', 'ALL_COLOR', 'GLUC_COLOR', 'FOOD_COLOR', 'DATASETS_PATH', 'COHORT',
            'POPULATION_DATASET', 'CONFIG_FILES', 'generate_synthetic_data', 'generate_synthetic_data_like']
 
 # %% ../nbs/00_config.ipynb 3
 import os
 
 import numpy as np
 import pandas as pd
@@ -16,27 +16,32 @@
 MALE_COLOR = "C0"
 ALL_COLOR = "C5"
 
 GLUC_COLOR = "C0"
 FOOD_COLOR = "C1"
 
 DATASETS_PATH = '/home/ec2-user/studies/hpp/'
+COHORT = '10k'
 POPULATION_DATASET = 'population'
 CONFIG_FILES = ['~/.pheno/config', '/efs/.pheno/config']
 
 for cf in CONFIG_FILES:
     cf = os.path.expanduser(cf)
     if not os.path.isfile(cf):
         continue
     with open(cf, 'r') as f:
         for line in f:
             if line.startswith('DATASETS_PATH'):
                 DATASETS_PATH = line.split('=')[1].strip()
             elif line.startswith('POPULATION_DATASET'):
                 POPULATION_DATASET = line.split('=')[1].strip()
+            elif line.startswith('COHORT'):
+                COHORT = line.split('=')[1].strip()
+                if (len(COHORT) == 0) or (COHORT == 'None'):
+                    COHORT = None
 
 
 # %% ../nbs/00_config.ipynb 5
 def generate_synthetic_data(n: int = 1000) -> pd.DataFrame:
     """
     Generates a sample DataFrame containing age, gender, and value data.
```

### Comparing `pheno-utils-0.1.3/pheno_utils/data_loader.py` & `pheno-utils-0.1.4/pheno_utils/data_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     """
     Class to load multiple tables from a dataset and allows to easily access
     their fields.
 
     Args:
     
         dataset (str): The name of the dataset to load.
-        base_path (str, optional): The base path where the data is stored. Defaults to '/home/ec2-user/studies'.
-        cohort (str, optional): The name of the cohort within the dataset. Defaults to '10k'.
-        age_sex_dataset (str, optional): The name of the dataset to use for computing age and sex. Defaults to 'Population_Characteristics'.
+        base_path (str, optional): The base path where the data is stored. Defaults to DATASETS_PATH.
+        cohort (str, optional): The name of the cohort within the dataset. Defaults to COHORT.
+        age_sex_dataset (str, optional): The name of the dataset to use for computing age and sex. Defaults to POPULATION_DATASET.
         skip_dfs (list, optional): A list of tables (or substrings that match to tables) to skip when loading the data. Defaults to [].
         unique_index (bool, optional): Whether to ensure the index of the data is unique. Defaults to False.
         valid_dates (bool, optional): Whether to ensure that all timestamps in the data are valid dates. Defaults to False.
         valid_stage (bool, optional): Whether to ensure that all research stages in the data are valid. Defaults to False.
         flexible_field_search (bool, optional): Whether to allow regex field search. Defaults to False.
         errors (str, optional): Whether to raise an error or issue a warning if missing data is encountered.
             Possible values are 'raise' and 'warn'. Defaults to 'raise'.
@@ -56,15 +56,15 @@
         errors (str): Whether to raise an error or issue a warning if missing data is encountered.
     """
 
     def __init__(
         self,
         dataset: str,
         base_path: str = DATASETS_PATH,
-        cohort: str = '10k',
+        cohort: str = COHORT,
         age_sex_dataset: str = POPULATION_DATASET,
         skip_dfs: List[str] = [],
         unique_index: bool = False,
         valid_dates: bool = False,
         valid_stage: bool = False,
         flexible_field_search: bool = False,
         errors: str = 'raise'
```

### Comparing `pheno-utils-0.1.3/pheno_utils/dates_plots.py` & `pheno-utils-0.1.4/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.3/pheno_utils/ecg_analysis.py` & `pheno-utils-0.1.4/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.3/pheno_utils/sleep_plots.py` & `pheno-utils-0.1.4/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.3/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.1.4/pheno_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.3/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.1.4/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.3/settings.ini` & `pheno-utils-0.1.4/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.1.3
+version = 0.1.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.1.3/setup.py` & `pheno-utils-0.1.4/setup.py`

 * *Files identical despite different names*

