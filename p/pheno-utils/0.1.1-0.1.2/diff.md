# Comparing `tmp/pheno-utils-0.1.1.tar.gz` & `tmp/pheno-utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.1.1.tar", last modified: Thu Apr 20 12:56:30 2023, max compression
+gzip compressed data, was "pheno-utils-0.1.2.tar", last modified: Thu Apr 20 19:11:15 2023, max compression
```

## Comparing `pheno-utils-0.1.1.tar` & `pheno-utils-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 12:56:30.177948 pheno-utils-0.1.1/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.1/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.1/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 12:56:30.177617 pheno-utils-0.1.1/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.1/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 12:56:30.173708 pheno-utils-0.1.1/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13667 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     5111 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/basic_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/cgm_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16243 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/dates_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/ecg_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 12:56:30.177071 pheno-utils-0.1.1/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 12:56:30.000000 pheno-utils-0.1.1/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-20 12:56:30.000000 pheno-utils-0.1.1/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-20 12:56:30.000000 pheno-utils-0.1.1/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-20 12:56:30.000000 pheno-utils-0.1.1/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.1/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-20 12:56:30.000000 pheno-utils-0.1.1/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-20 12:56:30.000000 pheno-utils-0.1.1/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-20 12:52:47.000000 pheno-utils-0.1.1/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-20 12:56:30.178090 pheno-utils-0.1.1/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.1/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 19:11:15.874888 pheno-utils-0.1.2/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.2/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.2/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 19:11:15.874463 pheno-utils-0.1.2/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.2/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 19:11:15.870638 pheno-utils-0.1.2/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13667 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     5111 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/basic_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/cgm_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16345 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/dates_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-20 19:03:56.000000 pheno-utils-0.1.2/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 19:11:15.873766 pheno-utils-0.1.2/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 19:11:15.000000 pheno-utils-0.1.2/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-20 19:11:15.000000 pheno-utils-0.1.2/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-20 19:11:15.000000 pheno-utils-0.1.2/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-20 19:11:15.000000 pheno-utils-0.1.2/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.2/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-20 19:11:15.000000 pheno-utils-0.1.2/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-20 19:11:15.000000 pheno-utils-0.1.2/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-20 19:03:40.000000 pheno-utils-0.1.2/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-20 19:11:15.875044 pheno-utils-0.1.2/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.2/setup.py
```

### Comparing `pheno-utils-0.1.1/LICENSE` & `pheno-utils-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.1/PKG-INFO` & `pheno-utils-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.1/pheno_utils/_modidx.py` & `pheno-utils-0.1.2/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.1/pheno_utils/age_reference_plots.py` & `pheno-utils-0.1.2/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.1/pheno_utils/basic_analysis.py` & `pheno-utils-0.1.2/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.1/pheno_utils/basic_plots.py` & `pheno-utils-0.1.2/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.1/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.1.2/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.1/pheno_utils/cgm_plots.py` & `pheno-utils-0.1.2/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.1/pheno_utils/config.py` & `pheno-utils-0.1.2/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.1/pheno_utils/data_loader.py` & `pheno-utils-0.1.2/pheno_utils/data_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     """
     Class to load multiple tables from a dataset and allows to easily access
     their fields.
 
     Args:
     
         dataset (str): The name of the dataset to load.
-        cohort (str, optional): The name of the cohort within the dataset. Defaults to '10k'.
         base_path (str, optional): The base path where the data is stored. Defaults to '/home/ec2-user/studies'.
+        cohort (str, optional): The name of the cohort within the dataset. Defaults to '10k'.
         age_sex_dataset (str, optional): The name of the dataset to use for computing age and sex. Defaults to 'Population_Characteristics'.
         skip_dfs (list, optional): A list of tables (or substrings that match to tables) to skip when loading the data. Defaults to [].
         unique_index (bool, optional): Whether to ensure the index of the data is unique. Defaults to False.
         valid_dates (bool, optional): Whether to ensure that all timestamps in the data are valid dates. Defaults to False.
         valid_stage (bool, optional): Whether to ensure that all research stages in the data are valid. Defaults to False.
         flexible_field_search (bool, optional): Whether to allow regex field search. Defaults to False.
         errors (str, optional): Whether to raise an error or issue a warning if missing data is encountered.
@@ -55,29 +55,32 @@
         flexible_field_search (bool): Whether to allow regex field search.
         errors (str): Whether to raise an error or issue a warning if missing data is encountered.
     """
 
     def __init__(
         self,
         dataset: str,
-        cohort: str = '10k',
         base_path: str = DATASETS_PATH,
+        cohort: str = '10k',
         age_sex_dataset: str = POPULATION_DATASET,
         skip_dfs: List[str] = [],
         unique_index: bool = False,
         valid_dates: bool = False,
         valid_stage: bool = False,
         flexible_field_search: bool = False,
         errors: str = 'raise'
     ) -> None:
         self.dataset = dataset
         self.cohort = cohort
         self.base_path = base_path
         self.dataset_path = self.__get_dataset_path__(self.dataset)
-        self.age_sex_dataset = age_sex_dataset
+        if self.dataset != age_sex_dataset:
+            self.age_sex_dataset = age_sex_dataset
+        else:
+            self.age_sex_dataset = None
         self.skip_dfs = skip_dfs
         self.unique_index = unique_index
         self.valid_dates = valid_dates
         self.valid_stage = valid_stage
         self.flexible_field_search = flexible_field_search
         self.errors = errors
```

### Comparing `pheno-utils-0.1.1/pheno_utils/dates_plots.py` & `pheno-utils-0.1.2/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.1/pheno_utils/ecg_analysis.py` & `pheno-utils-0.1.2/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.1/pheno_utils/sleep_plots.py` & `pheno-utils-0.1.2/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.1/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.1.2/pheno_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.1/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.1.2/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.1/settings.ini` & `pheno-utils-0.1.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.1.1
+version = 0.1.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.1.1/setup.py` & `pheno-utils-0.1.2/setup.py`

 * *Files identical despite different names*

