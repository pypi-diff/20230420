# Comparing `tmp/wildlife-datasets-0.3.2.tar.gz` & `tmp/wildlife-datasets-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adamluk3/Projects/wildlife-datasets/dist/.tmp-_3uy5vma/wildlife-datasets-0.3.2.tar", last modified: Tue Apr 18 11:25:14 2023, max compression
+gzip compressed data, was "/home/adamluk3/Projects/wildlife-datasets/dist/.tmp-ecmv4pbx/wildlife-datasets-0.3.3.tar", last modified: Thu Apr 20 13:41:44 2023, max compression
```

## Comparing `wildlife-datasets-0.3.2.tar` & `wildlife-datasets-0.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.096180 wildlife-datasets-0.3.2/
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1090 2023-02-15 08:36:46.000000 wildlife-datasets-0.3.2/LICENSE
--rw-rw-r--   0 adamluk3 (436797) ai         (501)     5224 2023-04-18 11:26:12.094760 wildlife-datasets-0.3.2/PKG-INFO
--rw-r--r--   0 adamluk3 (436797) ai         (501)     3090 2023-04-18 10:47:18.000000 wildlife-datasets-0.3.2/README.md
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1645 2023-04-18 11:26:03.000000 wildlife-datasets-0.3.2/pyproject.toml
--rw-rw-r--   0 adamluk3 (436797) ai         (501)       38 2023-04-18 11:26:12.097306 wildlife-datasets-0.3.2/setup.cfg
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:11.977176 wildlife-datasets-0.3.2/wildlife_datasets/
--rw-r--r--   0 adamluk3 (436797) ai         (501)      133 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.2/wildlife_datasets/__init__.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.008744 wildlife-datasets-0.3.2/wildlife_datasets/analysis/
--rw-r--r--   0 adamluk3 (436797) ai         (501)      107 2023-02-14 10:36:30.000000 wildlife-datasets-0.3.2/wildlife_datasets/analysis/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     5059 2023-03-06 09:03:18.000000 wildlife-datasets-0.3.2/wildlife_datasets/analysis/plots.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2698 2023-02-28 08:53:31.000000 wildlife-datasets-0.3.2/wildlife_datasets/analysis/statistics.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.031554 wildlife-datasets-0.3.2/wildlife_datasets/datasets/
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2784 2023-03-17 15:45:48.000000 wildlife-datasets-0.3.2/wildlife_datasets/datasets/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)    49821 2023-04-17 12:03:18.000000 wildlife-datasets-0.3.2/wildlife_datasets/datasets/datasets.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     8059 2023-03-17 12:53:50.000000 wildlife-datasets-0.3.2/wildlife_datasets/datasets/metadata.csv
--rw-r--r--   0 adamluk3 (436797) ai         (501)      822 2023-02-14 14:45:05.000000 wildlife-datasets-0.3.2/wildlife_datasets/datasets/metadata.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2843 2023-02-10 15:33:13.000000 wildlife-datasets-0.3.2/wildlife_datasets/datasets/utils.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.045010 wildlife-datasets-0.3.2/wildlife_datasets/downloads/
--rw-r--r--   0 adamluk3 (436797) ai         (501)       25 2023-03-11 08:49:06.000000 wildlife-datasets-0.3.2/wildlife_datasets/downloads/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)    26116 2023-04-18 10:44:32.000000 wildlife-datasets-0.3.2/wildlife_datasets/downloads/downloads.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1495 2023-03-16 15:44:33.000000 wildlife-datasets-0.3.2/wildlife_datasets/downloads/utils.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.054015 wildlife-datasets-0.3.2/wildlife_datasets/loader/
--rw-r--r--   0 adamluk3 (436797) ai         (501)       22 2023-02-14 10:26:57.000000 wildlife-datasets-0.3.2/wildlife_datasets/loader/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2958 2023-03-16 15:27:00.000000 wildlife-datasets-0.3.2/wildlife_datasets/loader/loader.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.062970 wildlife-datasets-0.3.2/wildlife_datasets/metrics/
--rw-r--r--   0 adamluk3 (436797) ai         (501)       23 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.2/wildlife_datasets/metrics/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     3269 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.2/wildlife_datasets/metrics/metrics.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.089626 wildlife-datasets-0.3.2/wildlife_datasets/splits/
--rw-r--r--   0 adamluk3 (436797) ai         (501)      191 2023-03-15 15:44:44.000000 wildlife-datasets-0.3.2/wildlife_datasets/splits/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2653 2023-03-07 14:12:11.000000 wildlife-datasets-0.3.2/wildlife_datasets/splits/analysis.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1896 2023-04-17 11:37:36.000000 wildlife-datasets-0.3.2/wildlife_datasets/splits/balanced_split.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)    11625 2023-04-17 12:28:07.000000 wildlife-datasets-0.3.2/wildlife_datasets/splits/identity_split.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1753 2023-03-07 14:02:45.000000 wildlife-datasets-0.3.2/wildlife_datasets/splits/lcg.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     9516 2023-04-17 12:29:03.000000 wildlife-datasets-0.3.2/wildlife_datasets/splits/time_aware_split.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:11.995873 wildlife-datasets-0.3.2/wildlife_datasets.egg-info/
--rw-rw-r--   0 adamluk3 (436797) ai         (501)     5224 2023-04-18 11:26:11.000000 wildlife-datasets-0.3.2/wildlife_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 adamluk3 (436797) ai         (501)     1077 2023-04-18 11:26:11.000000 wildlife-datasets-0.3.2/wildlife_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 adamluk3 (436797) ai         (501)        1 2023-04-18 11:26:11.000000 wildlife-datasets-0.3.2/wildlife_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 adamluk3 (436797) ai         (501)      130 2023-04-18 11:26:11.000000 wildlife-datasets-0.3.2/wildlife_datasets.egg-info/requires.txt
--rw-rw-r--   0 adamluk3 (436797) ai         (501)       18 2023-04-18 11:26:11.000000 wildlife-datasets-0.3.2/wildlife_datasets.egg-info/top_level.txt
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.858718 wildlife-datasets-0.3.3/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1090 2023-02-15 08:36:46.000000 wildlife-datasets-0.3.3/LICENSE
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)     7595 2023-04-20 13:42:42.856993 wildlife-datasets-0.3.3/PKG-INFO
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     5460 2023-04-19 07:30:02.000000 wildlife-datasets-0.3.3/README.md
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1645 2023-04-20 13:42:22.000000 wildlife-datasets-0.3.3/pyproject.toml
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)       38 2023-04-20 13:42:42.860030 wildlife-datasets-0.3.3/setup.cfg
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.676347 wildlife-datasets-0.3.3/wildlife_datasets/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      133 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.3/wildlife_datasets/__init__.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.714094 wildlife-datasets-0.3.3/wildlife_datasets/analysis/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      107 2023-02-14 10:36:30.000000 wildlife-datasets-0.3.3/wildlife_datasets/analysis/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     5059 2023-03-06 09:03:18.000000 wildlife-datasets-0.3.3/wildlife_datasets/analysis/plots.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2698 2023-02-28 08:53:31.000000 wildlife-datasets-0.3.3/wildlife_datasets/analysis/statistics.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.741225 wildlife-datasets-0.3.3/wildlife_datasets/datasets/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2784 2023-03-17 15:45:48.000000 wildlife-datasets-0.3.3/wildlife_datasets/datasets/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)    49977 2023-04-20 12:56:02.000000 wildlife-datasets-0.3.3/wildlife_datasets/datasets/datasets.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     8059 2023-03-17 12:53:50.000000 wildlife-datasets-0.3.3/wildlife_datasets/datasets/metadata.csv
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      822 2023-02-14 14:45:05.000000 wildlife-datasets-0.3.3/wildlife_datasets/datasets/metadata.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2843 2023-02-10 15:33:13.000000 wildlife-datasets-0.3.3/wildlife_datasets/datasets/utils.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.784002 wildlife-datasets-0.3.3/wildlife_datasets/downloads/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)       25 2023-03-11 08:49:06.000000 wildlife-datasets-0.3.3/wildlife_datasets/downloads/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)    26116 2023-04-18 10:44:32.000000 wildlife-datasets-0.3.3/wildlife_datasets/downloads/downloads.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1495 2023-03-16 15:44:33.000000 wildlife-datasets-0.3.3/wildlife_datasets/downloads/utils.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.795113 wildlife-datasets-0.3.3/wildlife_datasets/loader/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)       22 2023-02-14 10:26:57.000000 wildlife-datasets-0.3.3/wildlife_datasets/loader/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2958 2023-03-16 15:27:00.000000 wildlife-datasets-0.3.3/wildlife_datasets/loader/loader.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.806196 wildlife-datasets-0.3.3/wildlife_datasets/metrics/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)       23 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.3/wildlife_datasets/metrics/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     3269 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.3/wildlife_datasets/metrics/metrics.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.842364 wildlife-datasets-0.3.3/wildlife_datasets/splits/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      191 2023-04-20 11:10:08.000000 wildlife-datasets-0.3.3/wildlife_datasets/splits/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2653 2023-03-07 14:12:11.000000 wildlife-datasets-0.3.3/wildlife_datasets/splits/analysis.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1896 2023-04-17 11:37:36.000000 wildlife-datasets-0.3.3/wildlife_datasets/splits/balanced_split.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)    12258 2023-04-20 13:03:08.000000 wildlife-datasets-0.3.3/wildlife_datasets/splits/identity_split.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1753 2023-03-07 14:02:45.000000 wildlife-datasets-0.3.3/wildlife_datasets/splits/lcg.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     9516 2023-04-17 12:29:03.000000 wildlife-datasets-0.3.3/wildlife_datasets/splits/time_aware_split.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-20 13:42:42.698273 wildlife-datasets-0.3.3/wildlife_datasets.egg-info/
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)     7595 2023-04-20 13:42:42.000000 wildlife-datasets-0.3.3/wildlife_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)     1077 2023-04-20 13:42:42.000000 wildlife-datasets-0.3.3/wildlife_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)        1 2023-04-20 13:42:42.000000 wildlife-datasets-0.3.3/wildlife_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)      130 2023-04-20 13:42:42.000000 wildlife-datasets-0.3.3/wildlife_datasets.egg-info/requires.txt
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)       18 2023-04-20 13:42:42.000000 wildlife-datasets-0.3.3/wildlife_datasets.egg-info/top_level.txt
```

### Comparing `wildlife-datasets-0.3.2/LICENSE` & `wildlife-datasets-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/pyproject.toml` & `wildlife-datasets-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wildlife-datasets"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Lukáš Adam", email="lukas.adam.cr@gmail.com" },
   { name="Vojtěch Čermák", email="cermak.vojtech@seznam.cz" },
 ]
 maintainers = [
   { name="Lukáš Adam", email="lukas.adam.cr@gmail.com" },
   { name="Vojtěch Čermák", email="cermak.vojtech@seznam.cz" },
```

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/analysis/plots.py` & `wildlife-datasets-0.3.3/wildlife_datasets/analysis/plots.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/analysis/statistics.py` & `wildlife-datasets-0.3.3/wildlife_datasets/analysis/statistics.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/datasets/__init__.py` & `wildlife-datasets-0.3.3/wildlife_datasets/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/datasets/datasets.py` & `wildlife-datasets-0.3.3/wildlife_datasets/datasets/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1087,14 +1087,16 @@
         path_json = 'annotations.json'
         with open(os.path.join(self.root, path_json)) as file:
             data = json.load(file)
 
         # Extract dtaa from the JSON file
         create_dict = lambda i: {'id': i['id'], 'bbox': i['bbox'], 'image_id': i['image_id'], 'identity': i['identity'], 'segmentation': i['segmentation'], 'orientation': i['position']}
         df_annotation = pd.DataFrame([create_dict(i) for i in data['annotations']])
+        idx_bbox = ~df_annotation['bbox'].isnull()
+        df_annotation.loc[idx_bbox,'bbox'] = df_annotation.loc[idx_bbox,'bbox'].apply(lambda x: eval(x))
         create_dict = lambda i: {'file_name': i['path'].split('/')[-1], 'image_id': i['id'], 'date': i['date']}
         df_images = pd.DataFrame([create_dict(i) for i in data['images']])
 
         # Merge the information from the JSON file
         df = pd.merge(df_annotation, df_images, on='image_id')
         df['path'] = 'images' + os.path.sep + df['identity'] + os.path.sep + df['file_name']        
         df = df.drop(['image_id', 'file_name'], axis=1)
```

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/datasets/metadata.csv` & `wildlife-datasets-0.3.3/wildlife_datasets/datasets/metadata.csv`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/datasets/metadata.py` & `wildlife-datasets-0.3.3/wildlife_datasets/datasets/metadata.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/datasets/utils.py` & `wildlife-datasets-0.3.3/wildlife_datasets/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/downloads/downloads.py` & `wildlife-datasets-0.3.3/wildlife_datasets/downloads/downloads.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/downloads/utils.py` & `wildlife-datasets-0.3.3/wildlife_datasets/downloads/utils.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/loader/loader.py` & `wildlife-datasets-0.3.3/wildlife_datasets/loader/loader.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/metrics/metrics.py` & `wildlife-datasets-0.3.3/wildlife_datasets/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/splits/analysis.py` & `wildlife-datasets-0.3.3/wildlife_datasets/splits/analysis.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/splits/balanced_split.py` & `wildlife-datasets-0.3.3/wildlife_datasets/splits/balanced_split.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/splits/identity_split.py` & `wildlife-datasets-0.3.3/wildlife_datasets/splits/identity_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 import numpy as np
 import pandas as pd
 from typing import List, Tuple
 from .balanced_split import BalancedSplit
 
 
+class FullSplit(BalancedSplit):
+    """Simplest split returning the whole dataset.
+    """
+
+    def __init__(self):
+        pass
+
+    def split(self, df: pd.DataFrame) -> List[Tuple[np.ndarray, np.ndarray]]:
+        """Implementation of the [base splitting method](../reference_splits#splits.balanced_split.BalancedSplit.split).
+
+        Args:
+            df (pd.DataFrame): A dataframe of the data. It must contain column `identity`.
+
+        Returns:
+            List of splits. Each split is list of labels of the training and testing sets.
+        """
+
+        return [ (df.index.values, np.array([], dtype=int)) ]
+    
+
 class IdentitySplit(BalancedSplit):
     """Base class for `ClosedSetSplit`, `OpenSetSplit` and `DisjointSetSplit`.
     """
 
     def modify_df(self, df: pd.DataFrame) -> pd.DataFrame:
         """Prepares dataframe for splits.
 
@@ -189,15 +209,15 @@
         idx = self.lcg.random_permutation(n_class)
         y_counts = y_counts.iloc[idx]
 
         # Compute number of identities in the testing set
         n = len(df)
         if self.n_class_test is None:
             n_test = np.round(n*self.ratio_class_test).astype(int)
-            n_class_test = np.where(np.cumsum(y_counts) >= n_test)[0][0]
+            n_class_test = np.where(np.cumsum(y_counts) >= n_test)[0][0] + 1
         else:
             n_class_test = self.n_class_test
 
         # Specify individuals going purely into training and testing sets
         individual_train = np.array([], dtype=object)
         individual_test = np.array(y_counts.index[:n_class_test])
         return [self.general_split(df, individual_train, individual_test)]
@@ -260,15 +280,15 @@
         idx = self.lcg.random_permutation(n_class)
         y_counts = y_counts.iloc[idx]
 
         # Compute number of identities in the testing set
         n = len(df)
         if self.n_class_test is None:
             n_test = np.round(n*self.ratio_class_test).astype(int)
-            n_class_test = np.where(np.cumsum(y_counts) >= n_test)[0][0]
+            n_class_test = np.where(np.cumsum(y_counts) >= n_test)[0][0] + 1
         else:
             n_class_test = self.n_class_test
 
         # Specify individuals going purely into training and testing sets
         individual_train = np.array(y_counts.index[n_class_test:])
         individual_test = np.array(y_counts.index[:n_class_test])
         return [self.general_split(df, individual_train, individual_test)]
```

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/splits/lcg.py` & `wildlife-datasets-0.3.3/wildlife_datasets/splits/lcg.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets/splits/time_aware_split.py` & `wildlife-datasets-0.3.3/wildlife_datasets/splits/time_aware_split.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.2/wildlife_datasets.egg-info/SOURCES.txt` & `wildlife-datasets-0.3.3/wildlife_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

