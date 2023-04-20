# Comparing `tmp/pdpp-bhi-0.0.4.tar.gz` & `tmp/pdpp-bhi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdpp-bhi-0.0.4.tar", last modified: Thu Apr 20 15:49:27 2023, max compression
+gzip compressed data, was "pdpp-bhi-0.0.5.tar", last modified: Thu Apr 20 16:25:31 2023, max compression
```

## Comparing `pdpp-bhi-0.0.4.tar` & `pdpp-bhi-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:49:27.796075 pdpp-bhi-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 15:49:27.796075 pdpp-bhi-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 15:49:16.000000 pdpp-bhi-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:49:27.796075 pdpp-bhi-0.0.4/pdpp_bhi/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:49:16.000000 pdpp-bhi-0.0.4/pdpp_bhi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-04-20 15:49:16.000000 pdpp-bhi-0.0.4/pdpp_bhi/pdpp_bhi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:49:27.796075 pdpp-bhi-0.0.4/pdpp_bhi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 15:49:27.000000 pdpp-bhi-0.0.4/pdpp_bhi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-20 15:49:27.000000 pdpp-bhi-0.0.4/pdpp_bhi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:49:27.000000 pdpp-bhi-0.0.4/pdpp_bhi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 15:49:27.000000 pdpp-bhi-0.0.4/pdpp_bhi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 15:49:27.000000 pdpp-bhi-0.0.4/pdpp_bhi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:49:27.796075 pdpp-bhi-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-20 15:49:16.000000 pdpp-bhi-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:25:31.905978 pdpp-bhi-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 16:25:31.905978 pdpp-bhi-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 16:25:17.000000 pdpp-bhi-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:25:31.905978 pdpp-bhi-0.0.5/pdpp_bhi/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:25:17.000000 pdpp-bhi-0.0.5/pdpp_bhi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-20 16:25:17.000000 pdpp-bhi-0.0.5/pdpp_bhi/pdpp_bhi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:25:31.905978 pdpp-bhi-0.0.5/pdpp_bhi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 16:25:31.000000 pdpp-bhi-0.0.5/pdpp_bhi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-20 16:25:31.000000 pdpp-bhi-0.0.5/pdpp_bhi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:25:31.000000 pdpp-bhi-0.0.5/pdpp_bhi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 16:25:31.000000 pdpp-bhi-0.0.5/pdpp_bhi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 16:25:31.000000 pdpp-bhi-0.0.5/pdpp_bhi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:25:31.905978 pdpp-bhi-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-20 16:25:17.000000 pdpp-bhi-0.0.5/setup.py
```

### Comparing `pdpp-bhi-0.0.4/pdpp_bhi/pdpp_bhi.py` & `pdpp-bhi-0.0.5/pdpp_bhi/pdpp_bhi.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,32 @@
 from collections import defaultdict
 
 import pandas as pd
 import numpy as np
 
 class MockApi:
     def __init__(
-            self, clinical_path, peptide_path, protein_path, group_id_column='group_key', export_group_id_column=False
+            self, clinical_path, peptide_path, protein_path,
+            month_gaps=[0, 6, 12, 24],
+            group_id_column='group_key', export_group_id_column=False
         ):
         '''
         YOU MUST UPDATE THE FIRST THREE LINES of this method.
         They've been intentionally left in an invalid state.
 
         Variables to set:
             input_paths: a list of two or more paths to the csv files to be served
             group_id_column: the column that identifies which groups of rows the API should serve.
                 A call to iter_test serves all rows of all dataframes with the current group ID value.
             export_group_id_column: if true, the dataframes iter_test serves will include the group_id_column values.
         '''
         clinical = pd.read_csv(clinical_path)
         peptide = pd.read_csv(peptide_path)
         protein = pd.read_csv(protein_path)
+        self.month_gaps = month_gaps
         
         self.input_paths: Sequence[str] = [protein_path, peptide_path, clinical_path]
         self.group_id_column: str = group_id_column
         self.export_group_id_column: bool = export_group_id_column
         # iter_test is only designed to support at least two dataframes, such as test and sample_submission
         assert len(self.input_paths) >= 2
 
@@ -55,15 +58,15 @@
         test_proteins['group_key'] = test_proteins['visit_month']
         self.test_proteins = test_proteins.sort_values('group_key')
 
         # compose `sample_submission` dataframe, which has
         # prediction_id, rating, group_key columns
         prediction_ids, group_keys = [], []
         for r in test.to_records():
-            for month in [0, 6, 12, 24]:
+            for month in self.month_gaps:
                 pid = f'{r.row_id}_plus_{month}_months'
                 prediction_ids.append(pid)
                 group_keys.append(r.visit_month)
         
         self.sample_submission = pd.DataFrame({
             'prediction_id': prediction_ids,
             'rating': [0] * len(prediction_ids),
```

### Comparing `pdpp-bhi-0.0.4/setup.py` & `pdpp-bhi-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pdpp-bhi",
     packages=find_packages(exclude=[]),
     include_package_data=True,
-    version="0.0.4",
+    version="0.0.5",
     license="MIT",
     description="PDPP - BHI",
     author="Dohoon Lee",
     author_email="dohlee.bioinfo@gmail.com",
     long_description_content_type="text/markdown",
     url="https://github.com/dohlee/pdpp",
     keywords=[
```

