# Comparing `tmp/pdpp-bhi-0.0.5.tar.gz` & `tmp/pdpp-bhi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdpp-bhi-0.0.5.tar", last modified: Thu Apr 20 16:25:31 2023, max compression
+gzip compressed data, was "pdpp-bhi-0.0.6.tar", last modified: Thu Apr 20 16:33:29 2023, max compression
```

## Comparing `pdpp-bhi-0.0.5.tar` & `pdpp-bhi-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:25:31.905978 pdpp-bhi-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 16:25:31.905978 pdpp-bhi-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 16:25:17.000000 pdpp-bhi-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:25:31.905978 pdpp-bhi-0.0.5/pdpp_bhi/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:25:17.000000 pdpp-bhi-0.0.5/pdpp_bhi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-20 16:25:17.000000 pdpp-bhi-0.0.5/pdpp_bhi/pdpp_bhi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:25:31.905978 pdpp-bhi-0.0.5/pdpp_bhi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 16:25:31.000000 pdpp-bhi-0.0.5/pdpp_bhi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-20 16:25:31.000000 pdpp-bhi-0.0.5/pdpp_bhi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:25:31.000000 pdpp-bhi-0.0.5/pdpp_bhi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 16:25:31.000000 pdpp-bhi-0.0.5/pdpp_bhi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 16:25:31.000000 pdpp-bhi-0.0.5/pdpp_bhi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:25:31.905978 pdpp-bhi-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-20 16:25:17.000000 pdpp-bhi-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:33:29.159834 pdpp-bhi-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 16:33:29.159834 pdpp-bhi-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 16:33:18.000000 pdpp-bhi-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:33:29.159834 pdpp-bhi-0.0.6/pdpp_bhi/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:33:18.000000 pdpp-bhi-0.0.6/pdpp_bhi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-04-20 16:33:18.000000 pdpp-bhi-0.0.6/pdpp_bhi/pdpp_bhi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:33:29.159834 pdpp-bhi-0.0.6/pdpp_bhi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 16:33:29.000000 pdpp-bhi-0.0.6/pdpp_bhi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-20 16:33:29.000000 pdpp-bhi-0.0.6/pdpp_bhi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:33:29.000000 pdpp-bhi-0.0.6/pdpp_bhi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 16:33:29.000000 pdpp-bhi-0.0.6/pdpp_bhi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 16:33:29.000000 pdpp-bhi-0.0.6/pdpp_bhi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:33:29.159834 pdpp-bhi-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-20 16:33:18.000000 pdpp-bhi-0.0.6/setup.py
```

### Comparing `pdpp-bhi-0.0.5/pdpp_bhi/pdpp_bhi.py` & `pdpp-bhi-0.0.6/pdpp_bhi/pdpp_bhi.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self.export_group_id_column: bool = export_group_id_column
         # iter_test is only designed to support at least two dataframes, such as test and sample_submission
         assert len(self.input_paths) >= 2
 
         # compose `test` dataframe, which has
         # visit_id, visit_month, patient_id, updrs_test, row_id, group_key columns
         test = clinical[['visit_id', 'visit_month', 'patient_id']].apply(lambda row: row.repeat(4), axis=0).reset_index(drop=True)
-        test['updrs_test'] = [f'updrs_{i}' for i in range(1, 5)] * len(clinical)
+        test['updrs_test'] = [f'updrs_{idx}' for idx in range(1, 5)] * len(clinical)
         test['row_id'] = test.visit_id + '_' + test.updrs_test
         test['group_key'] = test['visit_month']
         self.test = test.sort_values('group_key')
 
         # compose `test_peptides` dataframe, which has
         # visit_id, visit_month, patient_id, UniProt, Peptide, PeptideAbundance, group_key columns
         test_peptides = peptide
@@ -138,15 +138,15 @@
         self._status = 'finished'
     
     def score(self, return_result=False):
         if not self._status == 'finished':
             raise Exception('You must run a full iteration of `iter_test()` first to score.')
         
         merged = self.predictions.merge(self.target, on='prediction_id')
-        merged.dropna(subset='target_rating')
+        merged = merged.dropna(subset='target_rating')
 
         scores = {'total': smape_p1(merged.target_rating, merged.rating)}
         for idx in range(1, 5):
             sub_df = merged[merged.prediction_id.str.contains(f'updrs_{idx}')]
             scores[f'updrs_{idx}'] = smape_p1(sub_df.target_rating, sub_df.rating)
         
         if not return_result:
```

### Comparing `pdpp-bhi-0.0.5/setup.py` & `pdpp-bhi-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pdpp-bhi",
     packages=find_packages(exclude=[]),
     include_package_data=True,
-    version="0.0.5",
+    version="0.0.6",
     license="MIT",
     description="PDPP - BHI",
     author="Dohoon Lee",
     author_email="dohlee.bioinfo@gmail.com",
     long_description_content_type="text/markdown",
     url="https://github.com/dohlee/pdpp",
     keywords=[
```

