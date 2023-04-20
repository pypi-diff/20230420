# Comparing `tmp/arfs-1.0.5.tar.gz` & `tmp/arfs-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-1.0.5.tar", last modified: Wed Jan 11 16:11:39 2023, max compression
+gzip compressed data, was "arfs-1.0.6.tar", last modified: Thu Apr 20 12:50:30 2023, max compression
```

## Comparing `arfs-1.0.5.tar` & `arfs-1.0.6.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-01-11 16:11:39.840844 arfs-1.0.5/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.0.5/LICENSE.md
--rw-rw-rw-   0        0        0    11069 2023-01-11 16:11:39.841843 arfs-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.0.5/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0     1389 2023-01-11 16:11:39.851846 arfs-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-11 16:11:39.489850 arfs-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-01-11 16:11:39.627846 arfs-1.0.5/src/arfs/
--rw-rw-rw-   0        0        0       92 2023-01-11 16:07:39.000000 arfs-1.0.5/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    87331 2023-01-06 14:55:52.000000 arfs-1.0.5/src/arfs/association.py
--rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.0.5/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2023-01-11 16:11:39.491846 arfs-1.0.5/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2023-01-11 16:11:39.715845 arfs-1.0.5/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.0.5/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.0.5/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2023-01-11 16:11:39.830846 arfs-1.0.5/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.0.5/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    84003 2023-01-06 14:55:53.000000 arfs-1.0.5/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.0.5/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    12704 2023-01-06 14:55:49.000000 arfs-1.0.5/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2627 2023-01-06 14:55:48.000000 arfs-1.0.5/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    15051 2023-01-06 14:55:49.000000 arfs-1.0.5/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    14733 2023-01-11 16:06:57.000000 arfs-1.0.5/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    22780 2023-01-09 09:22:51.000000 arfs-1.0.5/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.0.5/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    29121 2023-01-11 15:36:18.000000 arfs-1.0.5/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15581 2023-01-06 14:55:50.000000 arfs-1.0.5/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    22356 2023-01-06 15:03:38.000000 arfs-1.0.5/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-11 16:11:39.697846 arfs-1.0.5/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    11069 2023-01-11 16:11:39.000000 arfs-1.0.5/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      762 2023-01-11 16:11:39.000000 arfs-1.0.5/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-11 16:11:39.000000 arfs-1.0.5/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.0.5/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      365 2023-01-11 16:11:39.000000 arfs-1.0.5/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-01-11 16:11:39.000000 arfs-1.0.5/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 12:50:30.196236 arfs-1.0.6/
+-rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0    11069 2023-04-20 12:50:30.197235 arfs-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.0.6/README.md
+-rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1389 2023-04-20 12:50:30.207234 arfs-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 12:50:29.741232 arfs-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 12:50:29.887245 arfs-1.0.6/src/arfs/
+-rw-rw-rw-   0        0        0       92 2023-04-20 12:35:02.000000 arfs-1.0.6/src/arfs/__init__.py
+-rw-rw-rw-   0        0        0    87331 2023-01-06 14:55:52.000000 arfs-1.0.6/src/arfs/association.py
+-rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.0.6/src/arfs/benchmark.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:50:29.743234 arfs-1.0.6/src/arfs/dataset/
+drwxrwxrwx   0        0        0        0 2023-04-20 12:50:30.033234 arfs-1.0.6/src/arfs/dataset/data/
+-rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.0.6/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.0.6/src/arfs/dataset/data/housing.zip
+drwxrwxrwx   0        0        0        0 2023-04-20 12:50:30.160235 arfs-1.0.6/src/arfs/feature_selection/
+-rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.0.6/src/arfs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0    84003 2023-01-06 14:55:53.000000 arfs-1.0.6/src/arfs/feature_selection/allrelevant.py
+-rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.0.6/src/arfs/feature_selection/base.py
+-rw-rw-rw-   0        0        0    12730 2023-04-20 12:13:54.000000 arfs-1.0.6/src/arfs/feature_selection/mrmr.py
+-rw-rw-rw-   0        0        0     2627 2023-01-06 14:55:48.000000 arfs-1.0.6/src/arfs/feature_selection/summary.py
+-rw-rw-rw-   0        0        0    15051 2023-01-06 14:55:49.000000 arfs-1.0.6/src/arfs/feature_selection/unsupervised.py
+-rw-rw-rw-   0        0        0    14766 2023-01-11 17:15:13.000000 arfs-1.0.6/src/arfs/feature_selection/variable_importance.py
+-rw-rw-rw-   0        0        0    22780 2023-01-09 09:22:51.000000 arfs-1.0.6/src/arfs/gbm.py
+-rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.0.6/src/arfs/parallel.py
+-rw-rw-rw-   0        0        0    29121 2023-01-11 15:36:18.000000 arfs-1.0.6/src/arfs/preprocessing.py
+-rw-rw-rw-   0        0        0    15581 2023-01-06 14:55:50.000000 arfs-1.0.6/src/arfs/sampling.py
+-rw-rw-rw-   0        0        0    22356 2023-01-06 15:03:38.000000 arfs-1.0.6/src/arfs/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-20 12:50:29.962233 arfs-1.0.6/src/arfs.egg-info/
+-rw-rw-rw-   0        0        0    11069 2023-04-20 12:50:29.000000 arfs-1.0.6/src/arfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-04-20 12:50:29.000000 arfs-1.0.6/src/arfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 12:50:29.000000 arfs-1.0.6/src/arfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.0.6/src/arfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      365 2023-04-20 12:50:29.000000 arfs-1.0.6/src/arfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-20 12:50:29.000000 arfs-1.0.6/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 12:50:30.185234 arfs-1.0.6/tests/
+-rw-rw-rw-   0        0        0    10657 2023-01-09 09:22:50.000000 arfs-1.0.6/tests/test_allrelevant.py
+-rw-rw-rw-   0        0        0    19566 2023-01-09 09:22:50.000000 arfs-1.0.6/tests/test_featselect.py
```

### Comparing `arfs-1.0.5/LICENSE.md` & `arfs-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/PKG-INFO` & `arfs-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.0.5
+Version: 1.0.6
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-1.0.5/README.md` & `arfs-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/setup.cfg` & `arfs-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/association.py` & `arfs-1.0.6/src/arfs/association.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/benchmark.py` & `arfs-1.0.6/src/arfs/benchmark.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-1.0.6/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/dataset/data/housing.zip` & `arfs-1.0.6/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/feature_selection/__init__.py` & `arfs-1.0.6/src/arfs/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/feature_selection/allrelevant.py` & `arfs-1.0.6/src/arfs/feature_selection/allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/feature_selection/base.py` & `arfs-1.0.6/src/arfs/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/feature_selection/mrmr.py` & `arfs-1.0.6/src/arfs/feature_selection/mrmr.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,14 +259,16 @@
         # (redundancy with NULL is 0 and dividing by zero is INF)
         self.ranking_.iloc[0, 0] = float("Inf")
         self.selected_features_ = selected_features
         self.support_ = np.asarray(
             [x in selected_features for x in self.feature_names_in_]
         )
         self.not_selected_features_ = not_selected_features
+        
+        return self
 
     def transform(self, X):
         """
         Transform the data, returns a transformed version of `X`.
 
         Parameters
         ----------
@@ -278,15 +280,15 @@
         X_new : ndarray array of shape (n_samples, n_features_new)
             Transformed array.
         """
         if not isinstance(X, pd.DataFrame):
             raise TypeError("X is not a dataframe")
         return X[self.selected_features_]
 
-    def fit_transform(self, X, y=None, sample_weight=None):
+    def fit_transform(self, X, y, sample_weight=None):
         """
         Fit to data, then transform it.
         Fits transformer to `X` and `y` and optionally sample_weight
         with optional parameters `fit_params`
         and returns a transformed version of `X`.
         
         Parameters
```

### Comparing `arfs-1.0.5/src/arfs/feature_selection/summary.py` & `arfs-1.0.6/src/arfs/feature_selection/summary.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/feature_selection/unsupervised.py` & `arfs-1.0.6/src/arfs/feature_selection/unsupervised.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/feature_selection/variable_importance.py` & `arfs-1.0.6/src/arfs/feature_selection/variable_importance.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,16 @@
         )
         non_cum_threshold = df.iloc[importance_index, 2]
         max_norm_importance = 0.99 * df.normalized_importance.max()
 
         if plot_n > df.shape[0]:
             plot_n = df.shape[0] - 1
 
-        figsize = (8, plot_n / n_feat_per_inch)
+        if figsize is None:
+            figsize = (8, plot_n / n_feat_per_inch)
         fig = plt.figure(tight_layout=True, figsize=figsize)
         gs = gridspec.GridSpec(3, 3)
         ax1 = fig.add_subplot(gs[:, 0])
         ax1.scatter(df.normalized_importance, df.feature)
         # ax.set_ylabel('YLabel0')
         ax1.set_xlabel("normalized importance")
         ax1.xaxis.set_label_position("top")
```

### Comparing `arfs-1.0.5/src/arfs/gbm.py` & `arfs-1.0.6/src/arfs/gbm.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/parallel.py` & `arfs-1.0.6/src/arfs/parallel.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/preprocessing.py` & `arfs-1.0.6/src/arfs/preprocessing.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/sampling.py` & `arfs-1.0.6/src/arfs/sampling.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs/utils.py` & `arfs-1.0.6/src/arfs/utils.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.5/src/arfs.egg-info/PKG-INFO` & `arfs-1.0.6/src/arfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.0.5
+Version: 1.0.6
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-1.0.5/src/arfs.egg-info/SOURCES.txt` & `arfs-1.0.6/src/arfs.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -20,8 +20,10 @@
 src/arfs/dataset/data/housing.zip
 src/arfs/feature_selection/__init__.py
 src/arfs/feature_selection/allrelevant.py
 src/arfs/feature_selection/base.py
 src/arfs/feature_selection/mrmr.py
 src/arfs/feature_selection/summary.py
 src/arfs/feature_selection/unsupervised.py
-src/arfs/feature_selection/variable_importance.py
+src/arfs/feature_selection/variable_importance.py
+tests/test_allrelevant.py
+tests/test_featselect.py
```

