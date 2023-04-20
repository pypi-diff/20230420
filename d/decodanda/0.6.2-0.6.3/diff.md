# Comparing `tmp/decodanda-0.6.2.tar.gz` & `tmp/decodanda-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decodanda-0.6.2.tar", last modified: Tue Apr 18 20:46:56 2023, max compression
+gzip compressed data, was "decodanda-0.6.3.tar", last modified: Thu Apr 20 17:52:41 2023, max compression
```

## Comparing `decodanda-0.6.2.tar` & `decodanda-0.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:46:56.473711 decodanda-0.6.2/
--rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.2/LICENSE.md
--rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-18 20:46:56.473237 decodanda-0.6.2/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)    35652 2023-02-20 04:52:59.000000 decodanda-0.6.2/README.md
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:46:56.468985 decodanda-0.6.2/decodanda/
--rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.2/decodanda/__init__.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    97881 2023-04-18 20:06:07.000000 decodanda-0.6.2/decodanda/classes.py
--rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.2/decodanda/imports.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    11247 2023-02-17 19:33:24.000000 decodanda-0.6.2/decodanda/in_time.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    39339 2023-02-17 17:08:36.000000 decodanda-0.6.2/decodanda/utilities.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    22115 2023-04-18 20:45:44.000000 decodanda-0.6.2/decodanda/visualize.py
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:46:56.472592 decodanda-0.6.2/decodanda.egg-info/
--rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-18 20:46:56.000000 decodanda-0.6.2/decodanda.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-04-18 20:46:56.000000 decodanda-0.6.2/decodanda.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-04-18 20:46:56.000000 decodanda-0.6.2/decodanda.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-04-18 20:46:56.000000 decodanda-0.6.2/decodanda.egg-info/requires.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-04-18 20:46:56.000000 decodanda-0.6.2/decodanda.egg-info/top_level.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-04-18 20:46:56.473912 decodanda-0.6.2/setup.cfg
--rw-r--r--   0 lorenzo    (501) staff       (20)     1388 2023-04-18 20:46:06.000000 decodanda-0.6.2/setup.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-20 17:52:41.073698 decodanda-0.6.3/
+-rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.3/LICENSE.md
+-rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-20 17:52:41.073360 decodanda-0.6.3/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)    36482 2023-04-19 18:21:22.000000 decodanda-0.6.3/README.md
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-20 17:52:41.068916 decodanda-0.6.3/decodanda/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.3/decodanda/__init__.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    98867 2023-04-19 18:20:38.000000 decodanda-0.6.3/decodanda/classes.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.3/decodanda/imports.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    11247 2023-02-17 19:33:24.000000 decodanda-0.6.3/decodanda/in_time.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    39339 2023-02-17 17:08:36.000000 decodanda-0.6.3/decodanda/utilities.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    22115 2023-04-18 20:45:44.000000 decodanda-0.6.3/decodanda/visualize.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-20 17:52:41.072850 decodanda-0.6.3/decodanda.egg-info/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-20 17:52:41.000000 decodanda-0.6.3/decodanda.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-04-20 17:52:41.000000 decodanda-0.6.3/decodanda.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-04-20 17:52:41.000000 decodanda-0.6.3/decodanda.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-04-20 17:52:41.000000 decodanda-0.6.3/decodanda.egg-info/requires.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-04-20 17:52:41.000000 decodanda-0.6.3/decodanda.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-04-20 17:52:41.073816 decodanda-0.6.3/setup.cfg
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1388 2023-04-20 17:51:43.000000 decodanda-0.6.3/setup.py
```

### Comparing `decodanda-0.6.2/LICENSE.md` & `decodanda-0.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.2/PKG-INFO` & `decodanda-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.6.2
+Version: 0.6.3
 Summary: A python package for neural decoding with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.6.2/README.md` & `decodanda-0.6.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -424,14 +424,15 @@
 | parameter                   | type                                                                                                                                                                      | description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
 |-----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `data`                      | `dict` or `list` of dicts                                                                                                                                                 | The data used to decode, organized in dictionaries. Each data dictionary object must contain <br/> - one or more variables and values we want to decode, each in the format <br/> `<var name>: <Tx1 array of values>` <br/> -`raster: <TxN array>`<br/> the neural features from which we want to decode the variable values <br/> - a `trial: <Tx1 array>`<br/> the number that specify which chunks of data are considered independent for cross validation <br/> <br/> if more than one data dictionaries are passed to the constructor, `Decodanda` will create pseudo-population data by combining trials from the different dictionaries. |
 | `conditions`                | `dict`                                                                                                                                                                    | A dictionary that specifies which values for which variables of `data` we want to decode, in the form `{key: [value1, value2]}` <br/><br/>If more than one variable is specified, `Decodanda` will balance all conditions during each decoding analysis to disentangle the variables and avoid confounding correlations.                                                                                                                                                                                                                                                                                                                        |
 | `classifier`                | Possibly a `scikit-learn` classifier, but any object that exposes `.fit()`, `.predict()`, and `.score()` methods should work. <br/><br/> default: `sklearn.svm.LinearSVC` | The classifier used for all decoding analyses                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
 | `neaural_attr`              | `string` <br/><br/> default: `'raster'`                                                                                                                                   | The key of the neural features in the `data` dictionary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | `trial_attr`                | `string` or `None` <br/><br/> default: `'trial'`                                                                                                                          | The key of the trial attribute in the `data` dictionary. Each different trial is considered as an independent sample to be used in the cross validation routine, i.e., vectors with the same trial number always goes in either the training or the testing batch. If `None`: each contiguous chunk of the same values of all variables will be considered an individual trial.                                                                                                                                                                                                                                                                 |
+| `squeeze_trials`            | `bool`<br/><br/>default: `False`                                                                                                                                          | If True, all population vectors corresponding to the same trial number for the same condition will be squeezed into a single average activity vector.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
 | `trial chunk`               | `int` or `None` <br/><br/>default: `None`                                                                                                                                 | Only used when `trial_attr=None`. The maximum number of consecutive data points with the same value of all variables that are numbered with the same trial number.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 | `exclude_contiguous_chunks` | `bool`<br/><br/>default: `False`                                                                                                                                          | Only used when `trial_attr=None` and `trial_chunks != None`. Discards trials, defined as chunks of `trial_chunk` data each with the same variable values, that are consecutive in time. Useful to avoid decoding temporal artifacts when there are long auto-correlation times in the neural activations (e.g., calcium imaging)                                                                                                                                                                                                                                                                                                                |
 | `min_data_per_condition`    | `int`<br/><br/>default: 2                                                                                                                                                 | The minimum number of data points per each *condition*, defined as a specific combination of variable values, that a data set needs to have to be included in the analysis. In the case of pseudo-simultaneous data, datasets that do not meet this criterion will be excluded from the analysis. If no datasets meet the criterion, the constructor will raise an error.                                                                                                                                                                                                                                                                       |
 | `min_trials_per_condition`  | `int`<br/><br/>default: 2                                                                                                                                                 | The minimum number of unique trial numbers per each *condition*, defined as a specific combination of variable values, that a data set needs to have to be included in the analysis. In the case of pseudo-simultaneous data, datasets that do not meet this criterion will be excluded from the analysis. If no datasets meet the criterion, the constructor will raise an error.                                                                                                                                                                                                                                                              |
 | `exclude_silent`            | `bool`<br/><br/>default: `False`                                                                                                                                          | Excludes all silent population vectors (only zeros) from the analysis.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | `verbose`                   | `bool`<br/><br/>default: `False`                                                                                                                                          | If `True`, prints most operations and analysis results.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | `fault_tolerance`           | `bool`<br/><br/>default: `False`                                                                                                                                          | If `True`, raises a warning instead of an error when no datasets meet the inclusion criteria.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
```

### Comparing `decodanda-0.6.2/decodanda/classes.py` & `decodanda-0.6.3/decodanda/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU General Public License for more details.
 #
 
 import copy
 from typing import Tuple, Union
 
+import numpy as np
 import scipy.stats.stats
 from numpy import ndarray
 from .imports import *
 from .utilities import generate_binary_words, string_bool, sample_training_testing_from_rasters, CrossValidator, \
     log_dichotomy, hamming, sample_from_rasters, generate_dichotomies, semantic_score, z_pval, DictSession, \
     contiguous_chunking, non_contiguous_mask, cosine
 from .visualize import corr_scatter, visualize_decoding, plot_perfs_null_model
@@ -28,14 +29,15 @@
 class Decodanda:
     def __init__(self,
                  data: Union[list, dict],
                  conditions: dict,
                  classifier: any = 'svc',
                  neural_attr: str = 'raster',
                  trial_attr: str = 'trial',
+                 squeeze_trials: bool = False,
                  min_data_per_condition: int = 2,
                  min_trials_per_condition: int = 2,
                  min_activations_per_cell: int = 1,
                  trial_chunk: Optional[int] = None,
                  exclude_contiguous_chunks: bool = False,
                  exclude_silent: bool = False,
                  verbose: bool = False,
@@ -74,14 +76,18 @@
         trial_attr
             The key under which the trial numbers are stored in the ``data`` dictionary.
             Each different trial is considered as an independent sample to be used in
             during cross validation.
             If ``None``, trials are defined as consecutive bouts of data in time
             where all the variables have a constant value.
 
+        squeeze_trials
+            If True, all population vectors corresponding to the same trial number for the same
+            condition will be squeezed into a single average activity vector.
+
         min_data_per_condition
             The minimum number of data points per each condition, defined as a specific
             combination of values of all variables in the ``conditions`` dictionary,
             that a data set needs to have to be included in the analysis.
 
         min_trials_per_condition
             The minimum number of unique trial numbers per each condition, defined as a specific
@@ -222,14 +228,15 @@
         self._debug = debug
         self._zscore = zscore
         self._exclude_silent = exclude_silent
         self._neural_attr = neural_attr
         self._trial_attr = trial_attr
         self._trial_chunk = trial_chunk
         self._exclude_contiguous_trials = exclude_contiguous_chunks
+        self._trial_average = squeeze_trials
 
         # setting session(s) data
         self.n_sessions = len(data)
         self.n_conditions = len(conditions)
         self._max_conditioned_data = 0
         self._min_conditioned_data = 10 ** 6
         self.n_neurons = 0
@@ -257,17 +264,14 @@
         # conditioned null model index is the chunk division used for null model shuffles
         self.conditioned_trial_index = {string_bool(w): [] for w in self._condition_vectors}
 
         #   >>> main part: create conditioned arrays <<< ---------------------------------
         self._divide_data_into_conditions(data)
         #  \ >>> main part: create conditioned arrays <<< --------------------------------
 
-        # if zscore:
-        #     self._zscore_activity()
-
         # raising exceptions
         if self.n_brains == 0:
             if not fault_tolerance:
                 raise RuntimeError(
                     "\n[Decodanda] No session passed the minimum data threshold for conditioned arrays.\n\t\t"
                     "Check for mutually-exclusive conditions or try using less restrictive thresholds.")
         else:
@@ -1365,15 +1369,16 @@
                                                       max_semantic_dist=max_semantic_dist)
             ps[key] = data_ps
             ps_nullmodel[key] = null_ps
 
         if plot:
             if not ax:
                 f, ax = plt.subplots(figsize=(0.5 + 1.8 * len(semantic_dics), 3.5))
-            plot_perfs_null_model(ps, ps_nullmodel, ylabel='Parallelism Score', ax=ax, ylow=-1.05, yhigh=1.05, chance=0, **kwargs)
+            plot_perfs_null_model(ps, ps_nullmodel, ylabel='Parallelism Score', ax=ax, ylow=-1.05, yhigh=1.05, chance=0,
+                                  **kwargs)
 
         return ps, ps_nullmodel
 
     def semantic_score_geometry(self,
                                 training_fraction: float = 0.75,
                                 cross_validations: int = 10,
                                 nshuffles: int = 10,
@@ -1537,15 +1542,15 @@
                     print("\t\t[Decodanda]\tbuilding conditioned rasters for session %s" % session.name)
                 else:
                     print("\t\t[Decodanda]\tbuilding conditioned rasters for session %u" % si)
 
             session_conditioned_rasters = {}
             session_conditioned_trial_index = {}
 
-            # exclude inactive neurons
+            # exclude inactive neurons across the specified conditions
             array = getattr(session, self._neural_attr)
             total_mask = np.zeros(len(array)) > 0
 
             for condition_vec in self._condition_vectors:
                 mask = np.ones(len(array)) > 0
                 for i, sk in enumerate(self._semantic_keys):
                     semantic_values = list(self.conditions[sk])
@@ -1596,14 +1601,27 @@
 
                 # exclude empty time bins (only for binary discrete decoding)
                 if self._exclude_silent:
                     active_mask = np.sum(conditioned_raster, 1) > 0
                     conditioned_raster = conditioned_raster[active_mask, :]
                     conditioned_trial = conditioned_trial[active_mask]
 
+                # squeeze into trials
+                if self._trial_average:
+                    unique_trials = np.unique(conditioned_trial)
+                    squeezed_raster = []
+                    squeezed_trial_index = []
+                    for t in unique_trials:
+                        trial_raster = conditioned_raster[conditioned_trial == t]
+                        squeezed_raster.append(np.nanmean(trial_raster, 0))
+                        squeezed_trial_index.append(t)
+                    # set the new arrays
+                    conditioned_raster = np.asarray(squeezed_raster)
+                    conditioned_trial = np.asarray(squeezed_trial_index)
+
                 # set the conditioned neural data in the conditioned_rasters dictionary
                 session_conditioned_rasters[string_bool(condition_vec)] = conditioned_raster
                 session_conditioned_trial_index[string_bool(condition_vec)] = conditioned_trial
 
                 if self._verbose:
                     semantic_vector_string = []
                     for i, sk in enumerate(self._semantic_keys):
```

### Comparing `decodanda-0.6.2/decodanda/imports.py` & `decodanda-0.6.3/decodanda/imports.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.2/decodanda/in_time.py` & `decodanda-0.6.3/decodanda/in_time.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.2/decodanda/utilities.py` & `decodanda-0.6.3/decodanda/utilities.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.2/decodanda/visualize.py` & `decodanda-0.6.3/decodanda/visualize.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.2/decodanda.egg-info/PKG-INFO` & `decodanda-0.6.3/decodanda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.6.2
+Version: 0.6.3
 Summary: A python package for neural decoding with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.6.2/setup.py` & `decodanda-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.6.2'
+VERSION = '0.6.3'
 DESCRIPTION = 'A python package for neural decoding with built-in best practices.'
 LONG_DESCRIPTION = 'Decodanda (dog latin for "to be decoded") is a best-practices-made-easy Python package for decoding neural data. Decodanda is designed to expose a user-friendly and flexible interface for population activity decoding, with a series of built-in best practices to avoid the most common pitfalls. In addition, Decodanda exposes a series of functions to compute the Cross-Condition Generalization Performance (CCGP, Bernardi et al. 2020) for the geometrical analysis of neural population activity.'
 
 setup(
     name="decodanda",
     version=VERSION,
     author="Lorenzo Posani",
```

