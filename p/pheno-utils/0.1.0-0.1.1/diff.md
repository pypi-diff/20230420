# Comparing `tmp/pheno-utils-0.1.0.tar.gz` & `tmp/pheno-utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.1.0.tar", last modified: Mon Apr 17 14:52:12 2023, max compression
+gzip compressed data, was "pheno-utils-0.1.1.tar", last modified: Thu Apr 20 12:56:30 2023, max compression
```

## Comparing `pheno-utils-0.1.0.tar` & `pheno-utils-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-17 14:52:11.992709 pheno-utils-0.1.0/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.0/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.0/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-17 14:52:11.991619 pheno-utils-0.1.0/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.0/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-17 14:52:11.981687 pheno-utils-0.1.0/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-17 14:49:34.000000 pheno-utils-0.1.0/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13380 2023-04-17 14:49:34.000000 pheno-utils-0.1.0/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-17 14:49:34.000000 pheno-utils-0.1.0/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     5111 2023-04-17 14:49:34.000000 pheno-utils-0.1.0/pheno_utils/basic_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-17 14:49:34.000000 pheno-utils-0.1.0/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-17 14:49:34.000000 pheno-utils-0.1.0/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-17 14:49:34.000000 pheno-utils-0.1.0/pheno_utils/cgm_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-17 14:49:34.000000 pheno-utils-0.1.0/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    15944 2023-04-17 14:49:34.000000 pheno-utils-0.1.0/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-17 14:49:34.000000 pheno-utils-0.1.0/pheno_utils/dates_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-17 14:49:34.000000 pheno-utils-0.1.0/pheno_utils/ecg_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-17 14:49:34.000000 pheno-utils-0.1.0/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-17 14:52:11.990849 pheno-utils-0.1.0/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-17 14:52:11.000000 pheno-utils-0.1.0/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-17 14:52:11.000000 pheno-utils-0.1.0/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-17 14:52:11.000000 pheno-utils-0.1.0/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-17 14:52:11.000000 pheno-utils-0.1.0/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.0/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-17 14:52:11.000000 pheno-utils-0.1.0/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-17 14:52:11.000000 pheno-utils-0.1.0/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-17 14:48:39.000000 pheno-utils-0.1.0/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-17 14:52:11.993550 pheno-utils-0.1.0/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.0/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 12:56:30.177948 pheno-utils-0.1.1/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.1/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.1/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 12:56:30.177617 pheno-utils-0.1.1/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.1/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 12:56:30.173708 pheno-utils-0.1.1/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13667 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     5111 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/basic_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/cgm_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16243 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/dates_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-20 12:54:44.000000 pheno-utils-0.1.1/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-20 12:56:30.177071 pheno-utils-0.1.1/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-20 12:56:30.000000 pheno-utils-0.1.1/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-20 12:56:30.000000 pheno-utils-0.1.1/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-20 12:56:30.000000 pheno-utils-0.1.1/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-20 12:56:30.000000 pheno-utils-0.1.1/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.1/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-20 12:56:30.000000 pheno-utils-0.1.1/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-20 12:56:30.000000 pheno-utils-0.1.1/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-20 12:52:47.000000 pheno-utils-0.1.1/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-20 12:56:30.178090 pheno-utils-0.1.1/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.1/setup.py
```

### Comparing `pheno-utils-0.1.0/LICENSE` & `pheno-utils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.0/PKG-INFO` & `pheno-utils-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.0/pheno_utils/_modidx.py` & `pheno-utils-0.1.1/pheno_utils/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,16 @@
                                                                                     'pheno_utils/config.py'),
                                     'pheno_utils.config.generate_synthetic_data_like': ( 'config.html#generate_synthetic_data_like',
                                                                                          'pheno_utils/config.py')},
             'pheno_utils.data_loader': { 'pheno_utils.data_loader.DataLoader': ( 'data_loader.html#dataloader',
                                                                                  'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.__concat__': ( 'data_loader.html#dataloader.__concat__',
                                                                                             'pheno_utils/data_loader.py'),
+                                         'pheno_utils.data_loader.DataLoader.__get_dataset_path__': ( 'data_loader.html#dataloader.__get_dataset_path__',
+                                                                                                      'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.__get_file_path__': ( 'data_loader.html#dataloader.__get_file_path__',
                                                                                                    'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.__getitem__': ( 'data_loader.html#dataloader.__getitem__',
                                                                                              'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.__init__': ( 'data_loader.html#dataloader.__init__',
                                                                                           'pheno_utils/data_loader.py'),
                                          'pheno_utils.data_loader.DataLoader.__load_age_sex__': ( 'data_loader.html#dataloader.__load_age_sex__',
```

### Comparing `pheno-utils-0.1.0/pheno_utils/age_reference_plots.py` & `pheno-utils-0.1.1/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.0/pheno_utils/basic_analysis.py` & `pheno-utils-0.1.1/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.0/pheno_utils/basic_plots.py` & `pheno-utils-0.1.1/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.0/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.1.1/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.0/pheno_utils/cgm_plots.py` & `pheno-utils-0.1.1/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.0/pheno_utils/config.py` & `pheno-utils-0.1.1/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.0/pheno_utils/data_loader.py` & `pheno-utils-0.1.1/pheno_utils/data_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     
         dict (pd.DataFrame): The data dictionary for the dataset, containing information about each field.
         dfs (dict): A dictionary of dataframes, one for each table in the dataset.
         fields (list): A list of all fields in the dataset.
         dataset (str): The name of the dataset being used.
         cohort (str): The name of the cohort being used.
         base_path (str): The base path where the data is stored.
+        dataset_path (str): The full path to the dataset being used.
         age_sex_dataset (str): The name of the dataset being used to compute age and sex.
         skip_dfs (list): A list of tables to skip when loading the data.
         unique_index (bool): Whether to ensure the index of the data is unique.
         valid_dates (bool): Whether to ensure that all timestamps in the data are valid dates.
         valid_stage (bool): Whether to ensure that all research stages in the data are valid.
         flexible_field_search (bool): Whether to allow regex field search.
         errors (str): Whether to raise an error or issue a warning if missing data is encountered.
@@ -67,14 +68,15 @@
         valid_stage: bool = False,
         flexible_field_search: bool = False,
         errors: str = 'raise'
     ) -> None:
         self.dataset = dataset
         self.cohort = cohort
         self.base_path = base_path
+        self.dataset_path = self.__get_dataset_path__(self.dataset)
         self.age_sex_dataset = age_sex_dataset
         self.skip_dfs = skip_dfs
         self.unique_index = unique_index
         self.valid_dates = valid_dates
         self.valid_stage = valid_stage
         self.flexible_field_search = flexible_field_search
         self.errors = errors
@@ -120,18 +122,15 @@
 
         where_field = self.dict.loc[field_name]
         if isinstance(where_field['parent_dataframe'], str):
             field_name = where_field['parent_dataframe']
 
         sample = self[[field_name] + ['participant_id']].query(query_str).astype({field_name: str})
         missing_participants = np.setdiff1d(participant_id, sample['participant_id'].unique())
-        sample = os.path.join(
-            self.base_path,
-            self.dataset,
-            self.cohort) + '/' + sample.iloc[:, 0]
+        sample = self.dataset_path + '/' + sample.iloc[:, 0]
 
         if len(missing_participants):
             if self.errors == 'raise':
                 raise ValueError(f'Missing samples: {missing_participants}')
             elif self.errors == 'warn':
                 warnings.warn(f'Missing samples: {missing_participants}')
             if len(sample) == 0:
@@ -242,19 +241,15 @@
             return df1
         return df1.join(df2, how='outer')
 
     def __load_age_sex__(self) -> None:
         """
         Add sex and compute age from birth date.
         """
-        age_path = os.path.join(
-            self.base_path,
-            self.age_sex_dataset,
-            self.cohort,
-            'events.parquet')
+        age_path = os.path.join(self.__get_dataset_path__('population'), 'events.parquet')
         align_df = self.dfs[list(self.dfs)[0]]
 
         if ('research_stage' in align_df.columns) or ('research_stage' in align_df.index.names):
             age_df = pd.read_parquet(age_path)
             self.dfs['age_sex'] = align_df.join(
                 age_df[['age_at_research_stage', 'sex']].droplevel('array_index'))\
                 .rename(columns={'age_at_research_stage': 'age'})[['age', 'sex']]
@@ -314,19 +309,15 @@
 
         Args:
             relative_location (str): the location of the dataframe
 
         Returns:
             pd.DataFrame: the loaded dataframe
         """
-        df_path = os.path.join(
-            self.base_path,
-            self.dataset,
-            self.cohort,
-            relative_location)
+        df_path = os.path.join(self.dataset_path, relative_location)
         try:
             data =  pd.read_parquet(df_path)
         except Exception as err:
             if self.errors == 'raise':
                 raise err
             if self.errors == 'warn':
                 warnings.warn(f'Error loading {df_path}:\n{err}')
@@ -366,19 +357,33 @@
         Args:
             dataset (str): the name of the dataset
             extension (str): the extension of the file
 
         Returns:
             str: the path to the file
         """
-        path = os.path.join(self.base_path, dataset, self.cohort, '*.' + extension)
+        path = os.path.join(self.dataset_path, '*.' + extension)
         if path.startswith('s3://'):
            return path
         return glob(path)[0]
-    
+
+    def __get_dataset_path__(self, dataset):
+        """
+        Get the dataset path.
+        
+        Args:
+            dataset (str): the name of the dataset
+
+        Returns:
+            str: the path to the dataset
+        """
+        if self.cohort is not None:
+            return os.path.join(self.base_path, dataset, self.cohort)
+        return os.path.join(self.base_path, dataset)
+
     def describe_field(self, fields: Union[str,List[str]], return_summary: bool=False):
         """
         Display a summary dataframe for the specified fields from all tables
 
         Args:
             fields (List[str]): Fields to return
             return_summary (Bool): whether to return the summary dataframe
```

### Comparing `pheno-utils-0.1.0/pheno_utils/dates_plots.py` & `pheno-utils-0.1.1/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.0/pheno_utils/ecg_analysis.py` & `pheno-utils-0.1.1/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.0/pheno_utils/sleep_plots.py` & `pheno-utils-0.1.1/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.0/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.1.1/pheno_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.0/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.1.1/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.0/settings.ini` & `pheno-utils-0.1.1/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.1.0
+version = 0.1.1
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.1.0/setup.py` & `pheno-utils-0.1.1/setup.py`

 * *Files identical despite different names*

